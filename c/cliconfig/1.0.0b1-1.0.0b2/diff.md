# Comparing `tmp/cliconfig-1.0.0b1.tar.gz` & `tmp/cliconfig-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-1.0.0b1.tar", last modified: Tue May 16 13:06:13 2023, max compression
+gzip compressed data, was "cliconfig-1.0.0b2.tar", last modified: Tue May 30 11:29:26 2023, max compression
```

## Comparing `cliconfig-1.0.0b1.tar` & `cliconfig-1.0.0b2.tar`

### file list

```diff
@@ -1,125 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.188370 cliconfig-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.172370 cliconfig-1.0.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.176370 cliconfig-1.0.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-16 13:06:13.188370 cliconfig-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/README_pypi.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.176370 cliconfig-1.0.0b1/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 13:06:13.000000 cliconfig-1.0.0b1/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/cliconfig/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/cliconfig/config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/cliconfig/dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/cliconfig/process_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.180370 cliconfig-1.0.0b1/cliconfig/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/cliconfig/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/cliconfig/processing/_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/cliconfig/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26940 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/cliconfig/processing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/cliconfig/processing/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/cliconfig/tag_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.180370 cliconfig-1.0.0b1/cliconfig/yaml_tags/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/cliconfig/yaml_tags/_yaml_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.176370 cliconfig-1.0.0b1/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-16 13:06:13.000000 cliconfig-1.0.0b1/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-16 13:06:13.000000 cliconfig-1.0.0b1/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:06:13.000000 cliconfig-1.0.0b1/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 13:06:13.000000 cliconfig-1.0.0b1/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 13:06:13.000000 cliconfig-1.0.0b1/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.180370 cliconfig-1.0.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.180370 cliconfig-1.0.0b1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/_static/logo_extend.png
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/cliconfig.processing_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/processing.md
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.180370 cliconfig-1.0.0b1/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.180370 cliconfig-1.0.0b1/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:06:13.188370 cliconfig-1.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.180370 cliconfig-1.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.184370 cliconfig-1.0.0b1/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/configtag1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/configtag2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.184370 cliconfig-1.0.0b1/tests/configs/delete/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/delete/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/delete/config2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.172370 cliconfig-1.0.0b1/tests/configs/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.184370 cliconfig-1.0.0b1/tests/configs/integration/test1/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/integration/test1/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/integration/test1/sub1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/integration/test1/sub2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.184370 cliconfig-1.0.0b1/tests/configs/integration/test2/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/integration/test2/data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/integration/test2/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/integration/test2/exp1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/integration/test2/exp2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/integration/test2/exp3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.184370 cliconfig-1.0.0b1/tests/configs/integration/test2/models/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/integration/test2/models/resnet100.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/integration/test2/models/resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/integration/test2/models/vit_b16.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.184370 cliconfig-1.0.0b1/tests/configs/merge/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/merge/additional1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/merge/additional2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/merge/additional3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/merge/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/merge/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/merge/default3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/configs/multi_files_with_tags.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.184370 cliconfig-1.0.0b1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/integration/test_inte_multiple_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.184370 cliconfig-1.0.0b1/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:06:13.188370 cliconfig-1.0.0b1/tests/unit/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/unit/processing/test_base_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/unit/processing/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/unit/processing/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/unit/processing/test_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/unit/test_base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/unit/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/unit/test_config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/unit/test_dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/unit/test_ex_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/unit/test_process_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-16 13:05:56.000000 cliconfig-1.0.0b1/tests/unit/test_tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.094412 cliconfig-1.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.070412 cliconfig-1.0.0b2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.074412 cliconfig-1.0.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-30 11:29:26.094412 cliconfig-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.074412 cliconfig-1.0.0b2/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 11:29:25.000000 cliconfig-1.0.0b2/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.078412 cliconfig-1.0.0b2/cliconfig/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/processing/_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26940 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/processing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/processing/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.078412 cliconfig-1.0.0b2/cliconfig/yaml_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/cliconfig/yaml_tags/_yaml_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.078412 cliconfig-1.0.0b2/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-30 11:29:26.000000 cliconfig-1.0.0b2/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-30 11:29:26.000000 cliconfig-1.0.0b2/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:29:26.000000 cliconfig-1.0.0b2/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 11:29:26.000000 cliconfig-1.0.0b2/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 11:29:26.000000 cliconfig-1.0.0b2/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.082412 cliconfig-1.0.0b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/README_pypi.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.082412 cliconfig-1.0.0b2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/_static/logo_extend.png
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/cliconfig.processing_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/processing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.082412 cliconfig-1.0.0b2/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.082412 cliconfig-1.0.0b2/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:29:26.098412 cliconfig-1.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.082412 cliconfig-1.0.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.086412 cliconfig-1.0.0b2/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.086412 cliconfig-1.0.0b2/tests/configs/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/delete/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/delete/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/fallback.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.070412 cliconfig-1.0.0b2/tests/configs/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.086412 cliconfig-1.0.0b2/tests/configs/integration/test1/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test1/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test1/sub1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test1/sub2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.090412 cliconfig-1.0.0b2/tests/configs/integration/test2/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/exp1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/exp2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/exp3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.090412 cliconfig-1.0.0b2/tests/configs/integration/test2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/models/resnet100.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/models/resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/integration/test2/models/vit_b16.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.094412 cliconfig-1.0.0b2/tests/configs/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/merge/additional1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/merge/additional2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/merge/additional3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/merge/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/merge/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/merge/default3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/configs/multi_files_with_tags.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.094412 cliconfig-1.0.0b2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/integration/test_inte_multiple_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.094412 cliconfig-1.0.0b2/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:29:26.094412 cliconfig-1.0.0b2/tests/unit/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/processing/test_base_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/processing/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/processing/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/processing/test_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_ex_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-30 11:29:03.000000 cliconfig-1.0.0b2/tests/unit/test_tag_routines.py
```

### Comparing `cliconfig-1.0.0b1/.github/workflows/pipy_deployment.yaml` & `cliconfig-1.0.0b2/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/.github/workflows/pydocstyle.yaml` & `cliconfig-1.0.0b2/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/.github/workflows/pylint.yaml` & `cliconfig-1.0.0b2/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/.github/workflows/tests.yaml` & `cliconfig-1.0.0b2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/.pylintrc` & `cliconfig-1.0.0b2/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/CONTRIBUTING.md` & `cliconfig-1.0.0b2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/LICENSE` & `cliconfig-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/PKG-INFO` & `cliconfig-1.0.0b2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,158 +1,143 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
-Keywords: logging,machine,learning
+Keywords: cli,config,cliconfig,python,yaml,merge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-# CLI Config
+CLI Config
+==========
 
-</p>
-<p align="center">
-  <img src="https://raw.githubusercontent.com/valentingol/cliconfig/main/docs/_static/logo_extend.png" />
-</p>
+|
+
+.. image:: _static/logo_extend.png
+  :align: center
+  :width: 1000
+  :alt: CLI config logo
+
+|
 
 *CLI Config*: Lightweight library that provides routines to merge nested configs
 and set parameters from command line. It is also provide processing functions
 that can change the whole configuration before and after each config merge, config
 saving, config loading and at the end of config building. It also contains many
 routines to manipulate the config as flatten or nested dicts.
 
-## Documentation: [read-the-docs](https://cliconfig.readthedocs.io/en/stable)
-
-## Source code: [github](https://github.com/valentingol/cliconfig)
+`Pypi project <https://pypi.org/project/cliconfig/>`_
 
-[![Release](https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow)](https://pypi.org/project/cliconfig/)
-![PythonVersion](https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational)
-[![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
+`Github project <https://github.com/valentingol/cliconfig>`_
 
-[![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
-[![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-[![Ruff](https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml)
-[![Flake8](https://github.com/valentingol/cliconfig/actions/workflows/flake.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/flake.yaml)
-[![Pydocstyle](https://github.com/valentingol/cliconfig/actions/workflows/pydocstyle.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/pydocstyle.yaml)
-[![MyPy](https://github.com/valentingol/cliconfig/actions/workflows/mypy.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/mypy.yaml)
-[![PyLint](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/ab12676c87f0eaa715bef0f8ad31a604/raw/cliconfig_pylint.json)](https://github.com/valentingol/cliconfig/actions/workflows/pylint.yaml)
+|PyPI version| |PythonVersion| |License| |Waka_Time|
 
-[![Tests](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml)
-[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/098e9c7c53be88779ee52ef2f2bc8803/raw/cliconfig_tests.json)](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml)
-[![Documentation Status](https://readthedocs.org/projects/cliconfig/badge/?version=latest)](https://cliconfig.readthedocs.io/en/latest/?badge=latest)
+|Ruff_logo| |Black_logo|
 
-## Installation
+|Ruff| |Flake8| |Pydocstyle| |MyPy| |PyLint|
 
-In a new virtual environment, simply install the package with:
+|Tests| |Coverage| |Documentation Status|
 
-```bash
-pip install cliconfig
-```
+Make default config file(s) in your project (configs are merged from left to right):
 
-This package is OS independent and supported on Linux, macOS and Windows.
+.. code:: python
 
-## Minimal usage
+   # main.py
+   from cliconfig import make_config
 
-Make default config file(s) in your project (configs are merged from left to right):
-
-```python
-# main.py
-from cliconfig import make_config
-
-config = make_config('default1.yaml', 'default2.yaml')
-config_dict = config.dict  # native python dict
-```
+   config = make_config('default1.yaml', 'default2.yaml')
+   config_dict = config.dict  # native python dict
 
 Then launch your script with additional config(s) file(s) and parameters by command line.
 The additional configs are merge on the default ones then the parameters are set.
 
-```bash
-python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
-```
+.. code:: bash
+
+   python main.py --config first.yaml,second.yaml --param1=1 --subconfig.param2='foo'
 
 **By default, these additional configs cannot add new parameters to the default config
 (for security and retro-compatibility reasons).**
 
-See [*Quick Start*](https://cliconfig.readthedocs.io/en/stable/quick_start.html) section
-of the documentation for more details.
-
-## With processing
+With processing
+---------------
 
 The library provide powerfull tools to modify the configuration called "processings".
 One of the possibility they add is to merge multiple configurations,
 copy a parameter on another, enforce type and more. To do so, simply adding the
 corresponding tags to your parameter names (on config files or CLI parameters).
 
 For instance with these config files:
 
-```yaml
-# main.yaml
-path_1@merge_add: sub1.yaml
-path_2@merge_add: sub2.yaml
-config3.select@select: config3.param1
-
-# sub1.yaml
-config1:
-  param@copy@type:int: config2.param
-  param2@type:int: 1
-
-# sub2.yaml
-config2.param@type:None|int: 2
-config3:
-  param1: 0
-  param2: 1
-```
+.. code:: yaml
+
+    # main.yaml
+    path_1@merge_add: sub1.yaml
+    path_2@merge_add: sub2.yaml
+    config3.select@select: config3.param1
+
+    # sub1.yaml
+    config1:
+      param@copy@type:int: config2.param
+      param2@type:None|int: 1
+
+    # sub2.yaml
+    config2.param@type:int: 2
+    config3:
+      param1: 0
+      param2: 1
 
 Note that can also use YAML tags separated with "@" (like `key: !tag@tag2 value`)
 to add tags instead of putting them in the parameter name (like `key@tag@tag2: value`).
 
-Here `main.yaml` is interpreted like:
+Here `main.yaml` will be interpreted like:
 
-```yaml
-path_1: sub1.yaml
-path_2: sub2.yaml
-config1:
-  param: 2  # the value of config2.param
-  param2: 1
-config2:
-  param: 2
-config3:
-  select: config3.param1
-  param1: 0
-  # param2 is deleted because it is not in the selection
-```
+.. code:: yaml
+
+    path_1: sub1.yaml
+    path_2: sub2.yaml
+    config1:
+      param: 2  # the value of config2.param
+      param2: 1
+    config2:
+      param: 2
+    config3:
+      select: config3.param1
+      param1: 0
+      # param2 is deleted because it is not in the selection
 
 Then, all the parameters in `config1` and `config2` have enforced types
 (`config2.param` can also be None) and changing `config2.param` will also update
 `config1.param` accordingly (which is protected by direct update).
 
-See [*Processing*](https://cliconfig.readthedocs.io/en/stable/processing.html) section
-of the documentation for details on processing and how to create your own.
-
-## How to contribute
-
-For **development**, install the package dynamically and dev requirements with:
-
-```bash
-pip install -e .
-pip install -r requirements-dev.txt
-```
-
-Everyone can contribute to CLI Config, and we value everyone’s contributions.
-Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
-
-## License
-
-Copyright (C) 2023  Valentin Goldité
-
-This program is free software: you can redistribute it and/or modify it under the
-terms of the [MIT License](LICENSE). This program is distributed in the hope that
-it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See *Quickstart* section for more details and *Processing* section for advanced usage.
 
-This project is free to use for COMMERCIAL USE, MODIFICATION, DISTRIBUTION and
-PRIVATE USE as long as the original license is include as well as this copy
-right notice at the top of the modified files.
+.. |PyPI version| image:: https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow
+   :target: https://pypi.org/project/cliconfig/
+.. |PythonVersion| image:: https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational
+.. |License| image:: https://img.shields.io/github/license/valentingol/cliconfig?color=999
+   :target: https://stringfixer.com/fr/MIT_license
+.. |Waka_Time| image:: https://wakatime.com/badge/github/valentingol/cliconfig.svg
+    :target: https://wakatime.com/badge/github/valentingol/cliconfig
+.. |Ruff_logo| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+   :target: https://github.com/charliermarsh/ruff
+.. |Black_logo| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+.. |Ruff| image:: https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml
+.. |Flake8| image:: https://github.com/valentingol/cliconfig/actions/workflows/flake.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/flake.yaml
+.. |Pydocstyle| image:: https://github.com/valentingol/cliconfig/actions/workflows/pydocstyle.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/pydocstyle.yaml
+.. |MyPy| image:: https://github.com/valentingol/cliconfig/actions/workflows/mypy.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/mypy.yaml
+.. |PyLint| image:: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/ab12676c87f0eaa715bef0f8ad31a604/raw/cliconfig_pylint.json
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/pylint.yaml
+.. |Tests| image:: https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml
+.. |Coverage| image:: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/098e9c7c53be88779ee52ef2f2bc8803/raw/cliconfig_tests.json
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml
+.. |Documentation Status| image:: https://readthedocs.org/projects/cliconfig/badge/?version=latest
+   :target: https://cliconfig.readthedocs.io/en/latest/?badge=latest
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cliconfig-1.0.0b1/README.md` & `cliconfig-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/README_pypi.md` & `cliconfig-1.0.0b2/docs/README_pypi.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,146 +1,131 @@
-# CLI Config
+CLI Config
+==========
 
-</p>
-<p align="center">
-  <img src="https://raw.githubusercontent.com/valentingol/cliconfig/main/docs/_static/logo_extend.png" />
-</p>
+|
+
+.. image:: _static/logo_extend.png
+  :align: center
+  :width: 1000
+  :alt: CLI config logo
+
+|
 
 *CLI Config*: Lightweight library that provides routines to merge nested configs
 and set parameters from command line. It is also provide processing functions
 that can change the whole configuration before and after each config merge, config
 saving, config loading and at the end of config building. It also contains many
 routines to manipulate the config as flatten or nested dicts.
 
-## Documentation: [read-the-docs](https://cliconfig.readthedocs.io/en/stable)
-
-## Source code: [github](https://github.com/valentingol/cliconfig)
+`Pypi project <https://pypi.org/project/cliconfig/>`_
 
-[![Release](https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow)](https://pypi.org/project/cliconfig/)
-![PythonVersion](https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational)
-[![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
+`Github project <https://github.com/valentingol/cliconfig>`_
 
-[![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
-[![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-[![Ruff](https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml)
-[![Flake8](https://github.com/valentingol/cliconfig/actions/workflows/flake.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/flake.yaml)
-[![Pydocstyle](https://github.com/valentingol/cliconfig/actions/workflows/pydocstyle.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/pydocstyle.yaml)
-[![MyPy](https://github.com/valentingol/cliconfig/actions/workflows/mypy.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/mypy.yaml)
-[![PyLint](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/ab12676c87f0eaa715bef0f8ad31a604/raw/cliconfig_pylint.json)](https://github.com/valentingol/cliconfig/actions/workflows/pylint.yaml)
+|PyPI version| |PythonVersion| |License| |Waka_Time|
 
-[![Tests](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml)
-[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/098e9c7c53be88779ee52ef2f2bc8803/raw/cliconfig_tests.json)](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml)
-[![Documentation Status](https://readthedocs.org/projects/cliconfig/badge/?version=latest)](https://cliconfig.readthedocs.io/en/latest/?badge=latest)
+|Ruff_logo| |Black_logo|
 
-## Installation
+|Ruff| |Flake8| |Pydocstyle| |MyPy| |PyLint|
 
-In a new virtual environment, simply install the package with:
+|Tests| |Coverage| |Documentation Status|
 
-```bash
-pip install cliconfig
-```
+Make default config file(s) in your project (configs are merged from left to right):
 
-This package is OS independent and supported on Linux, macOS and Windows.
+.. code:: python
 
-## Minimal usage
+   # main.py
+   from cliconfig import make_config
 
-Make default config file(s) in your project (configs are merged from left to right):
-
-```python
-# main.py
-from cliconfig import make_config
-
-config = make_config('default1.yaml', 'default2.yaml')
-config_dict = config.dict  # native python dict
-```
+   config = make_config('default1.yaml', 'default2.yaml')
+   config_dict = config.dict  # native python dict
 
 Then launch your script with additional config(s) file(s) and parameters by command line.
 The additional configs are merge on the default ones then the parameters are set.
 
-```bash
-python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
-```
+.. code:: bash
+
+   python main.py --config first.yaml,second.yaml --param1=1 --subconfig.param2='foo'
 
 **By default, these additional configs cannot add new parameters to the default config
 (for security and retro-compatibility reasons).**
 
-See [*Quick Start*](https://cliconfig.readthedocs.io/en/stable/quick_start.html) section
-of the documentation for more details.
-
-## With processing
+With processing
+---------------
 
 The library provide powerfull tools to modify the configuration called "processings".
 One of the possibility they add is to merge multiple configurations,
 copy a parameter on another, enforce type and more. To do so, simply adding the
 corresponding tags to your parameter names (on config files or CLI parameters).
 
 For instance with these config files:
 
-```yaml
-# main.yaml
-path_1@merge_add: sub1.yaml
-path_2@merge_add: sub2.yaml
-config3.select@select: config3.param1
-
-# sub1.yaml
-config1:
-  param@copy@type:int: config2.param
-  param2@type:int: 1
-
-# sub2.yaml
-config2.param@type:None|int: 2
-config3:
-  param1: 0
-  param2: 1
-```
+.. code:: yaml
+
+    # main.yaml
+    path_1@merge_add: sub1.yaml
+    path_2@merge_add: sub2.yaml
+    config3.select@select: config3.param1
+
+    # sub1.yaml
+    config1:
+      param@copy@type:int: config2.param
+      param2@type:None|int: 1
+
+    # sub2.yaml
+    config2.param@type:int: 2
+    config3:
+      param1: 0
+      param2: 1
 
 Note that can also use YAML tags separated with "@" (like `key: !tag@tag2 value`)
 to add tags instead of putting them in the parameter name (like `key@tag@tag2: value`).
 
-Here `main.yaml` is interpreted like:
+Here `main.yaml` will be interpreted like:
 
-```yaml
-path_1: sub1.yaml
-path_2: sub2.yaml
-config1:
-  param: 2  # the value of config2.param
-  param2: 1
-config2:
-  param: 2
-config3:
-  select: config3.param1
-  param1: 0
-  # param2 is deleted because it is not in the selection
-```
+.. code:: yaml
+
+    path_1: sub1.yaml
+    path_2: sub2.yaml
+    config1:
+      param: 2  # the value of config2.param
+      param2: 1
+    config2:
+      param: 2
+    config3:
+      select: config3.param1
+      param1: 0
+      # param2 is deleted because it is not in the selection
 
 Then, all the parameters in `config1` and `config2` have enforced types
 (`config2.param` can also be None) and changing `config2.param` will also update
 `config1.param` accordingly (which is protected by direct update).
 
-See [*Processing*](https://cliconfig.readthedocs.io/en/stable/processing.html) section
-of the documentation for details on processing and how to create your own.
-
-## How to contribute
-
-For **development**, install the package dynamically and dev requirements with:
-
-```bash
-pip install -e .
-pip install -r requirements-dev.txt
-```
-
-Everyone can contribute to CLI Config, and we value everyone’s contributions.
-Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
-
-## License
-
-Copyright (C) 2023  Valentin Goldité
-
-This program is free software: you can redistribute it and/or modify it under the
-terms of the [MIT License](LICENSE). This program is distributed in the hope that
-it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See *Quickstart* section for more details and *Processing* section for advanced usage.
 
-This project is free to use for COMMERCIAL USE, MODIFICATION, DISTRIBUTION and
-PRIVATE USE as long as the original license is include as well as this copy
-right notice at the top of the modified files.
+.. |PyPI version| image:: https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow
+   :target: https://pypi.org/project/cliconfig/
+.. |PythonVersion| image:: https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational
+.. |License| image:: https://img.shields.io/github/license/valentingol/cliconfig?color=999
+   :target: https://stringfixer.com/fr/MIT_license
+.. |Waka_Time| image:: https://wakatime.com/badge/github/valentingol/cliconfig.svg
+    :target: https://wakatime.com/badge/github/valentingol/cliconfig
+.. |Ruff_logo| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+   :target: https://github.com/charliermarsh/ruff
+.. |Black_logo| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+.. |Ruff| image:: https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml
+.. |Flake8| image:: https://github.com/valentingol/cliconfig/actions/workflows/flake.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/flake.yaml
+.. |Pydocstyle| image:: https://github.com/valentingol/cliconfig/actions/workflows/pydocstyle.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/pydocstyle.yaml
+.. |MyPy| image:: https://github.com/valentingol/cliconfig/actions/workflows/mypy.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/mypy.yaml
+.. |PyLint| image:: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/ab12676c87f0eaa715bef0f8ad31a604/raw/cliconfig_pylint.json
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/pylint.yaml
+.. |Tests| image:: https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml
+.. |Coverage| image:: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/098e9c7c53be88779ee52ef2f2bc8803/raw/cliconfig_tests.json
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml
+.. |Documentation Status| image:: https://readthedocs.org/projects/cliconfig/badge/?version=latest
+   :target: https://cliconfig.readthedocs.io/en/latest/?badge=latest
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cliconfig-1.0.0b1/cliconfig/__init__.py` & `cliconfig-1.0.0b2/cliconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/cliconfig/base.py` & `cliconfig-1.0.0b2/cliconfig/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         The list of Processing objects. If None, an empty list is used.
         The default is None.
     """
 
     def __init__(
         self,
         config_dict: Dict[str, Any],
-        process_list: Optional[List["Processing"]] = None
+        process_list: Optional[List["Processing"]] = None,
     ) -> None:
         self.dict = config_dict
         self.process_list = process_list if process_list else []
 
     def __repr__(self) -> str:
         """Representation of Config object."""
         process_classes = [process.__class__.__name__ for process in self.process_list]
```

### Comparing `cliconfig-1.0.0b1/cliconfig/cli_parser.py` & `cliconfig-1.0.0b2/cliconfig/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/cliconfig/config_routines.py` & `cliconfig-1.0.0b2/cliconfig/config_routines.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from cliconfig.tag_routines import clean_all_tags
 
 
 def make_config(
     *default_config_paths: str,
     process_list: Optional[List[Processing]] = None,
     add_default_processing: bool = True,
+    fallback: str = "",
 ) -> Config:
     r"""Make a config from default config(s) and CLI argument(s) with processing.
 
     The function uses the CLI Config routines :func:`.parse_cli` to parse the CLI
     arguments and merge them with :func:`.merge_flat_paths_processing`, applying
     the pre-merge and post-merge processing functions on each merge.
 
@@ -36,14 +37,18 @@
     process_list: Optional[List[Processing]], optional
         The list of processing to apply during each merge. None for empty list.
         By default None.
     add_default_processing : bool, optional
         If add_default_processing is True, the default processings
         (found on :class:`.DefaultProcessings`) are added to the list of
         processings. By default True.
+    fallback : str, optional
+        Path of the configuration to use if no additional config is provided
+        with ``--config``. No fallback config if empty string (default),
+        in that case, the config is the default configs plus the CLI arguments.
 
     Raises
     ------
     ValueError
         If additional configs have new keys that are not in default configs.
 
     Returns
@@ -73,19 +78,20 @@
               --architecture.layers.hidden_dim=64
 
     """
     # Create the processing list
     process_list_: List[Processing] = [] if process_list is None else process_list
     if add_default_processing:
         process_list_ += DefaultProcessings().list
-
     config = Config({}, process_list_)
-
-    # Merge default configs and additional configs
     additional_config_paths, cli_params_dict = parse_cli(sys.argv)
+    if not additional_config_paths and fallback:
+        # Add fallback config
+        additional_config_paths = [fallback]
+    # Merge default configs and additional configs
     for i, paths in enumerate([default_config_paths, additional_config_paths]):
         # Allow new keys for default configs only
         allow_new_keys = i == 0
         for path in paths:
             config = merge_flat_paths_processing(
                 config,
                 path,
```

### Comparing `cliconfig-1.0.0b1/cliconfig/dict_routines.py` & `cliconfig-1.0.0b2/cliconfig/dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/cliconfig/process_routines.py` & `cliconfig-1.0.0b2/cliconfig/process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/cliconfig/processing/_type_parser.py` & `cliconfig-1.0.0b2/cliconfig/processing/_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/cliconfig/processing/base.py` & `cliconfig-1.0.0b2/cliconfig/processing/base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/cliconfig/processing/builtin.py` & `cliconfig-1.0.0b2/cliconfig/processing/builtin.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/cliconfig/processing/create.py` & `cliconfig-1.0.0b2/cliconfig/processing/create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/cliconfig/tag_routines.py` & `cliconfig-1.0.0b2/cliconfig/tag_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/cliconfig/yaml_tags/_yaml_tags.py` & `cliconfig-1.0.0b2/cliconfig/yaml_tags/_yaml_tags.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/cliconfig.egg-info/PKG-INFO` & `cliconfig-1.0.0b2/cliconfig.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,158 +1,143 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
-Keywords: logging,machine,learning
+Keywords: cli,config,cliconfig,python,yaml,merge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-# CLI Config
+CLI Config
+==========
 
-</p>
-<p align="center">
-  <img src="https://raw.githubusercontent.com/valentingol/cliconfig/main/docs/_static/logo_extend.png" />
-</p>
+|
+
+.. image:: _static/logo_extend.png
+  :align: center
+  :width: 1000
+  :alt: CLI config logo
+
+|
 
 *CLI Config*: Lightweight library that provides routines to merge nested configs
 and set parameters from command line. It is also provide processing functions
 that can change the whole configuration before and after each config merge, config
 saving, config loading and at the end of config building. It also contains many
 routines to manipulate the config as flatten or nested dicts.
 
-## Documentation: [read-the-docs](https://cliconfig.readthedocs.io/en/stable)
-
-## Source code: [github](https://github.com/valentingol/cliconfig)
+`Pypi project <https://pypi.org/project/cliconfig/>`_
 
-[![Release](https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow)](https://pypi.org/project/cliconfig/)
-![PythonVersion](https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational)
-[![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
+`Github project <https://github.com/valentingol/cliconfig>`_
 
-[![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
-[![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-[![Ruff](https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml)
-[![Flake8](https://github.com/valentingol/cliconfig/actions/workflows/flake.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/flake.yaml)
-[![Pydocstyle](https://github.com/valentingol/cliconfig/actions/workflows/pydocstyle.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/pydocstyle.yaml)
-[![MyPy](https://github.com/valentingol/cliconfig/actions/workflows/mypy.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/mypy.yaml)
-[![PyLint](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/ab12676c87f0eaa715bef0f8ad31a604/raw/cliconfig_pylint.json)](https://github.com/valentingol/cliconfig/actions/workflows/pylint.yaml)
+|PyPI version| |PythonVersion| |License| |Waka_Time|
 
-[![Tests](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml)
-[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/098e9c7c53be88779ee52ef2f2bc8803/raw/cliconfig_tests.json)](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml)
-[![Documentation Status](https://readthedocs.org/projects/cliconfig/badge/?version=latest)](https://cliconfig.readthedocs.io/en/latest/?badge=latest)
+|Ruff_logo| |Black_logo|
 
-## Installation
+|Ruff| |Flake8| |Pydocstyle| |MyPy| |PyLint|
 
-In a new virtual environment, simply install the package with:
+|Tests| |Coverage| |Documentation Status|
 
-```bash
-pip install cliconfig
-```
+Make default config file(s) in your project (configs are merged from left to right):
 
-This package is OS independent and supported on Linux, macOS and Windows.
+.. code:: python
 
-## Minimal usage
+   # main.py
+   from cliconfig import make_config
 
-Make default config file(s) in your project (configs are merged from left to right):
-
-```python
-# main.py
-from cliconfig import make_config
-
-config = make_config('default1.yaml', 'default2.yaml')
-config_dict = config.dict  # native python dict
-```
+   config = make_config('default1.yaml', 'default2.yaml')
+   config_dict = config.dict  # native python dict
 
 Then launch your script with additional config(s) file(s) and parameters by command line.
 The additional configs are merge on the default ones then the parameters are set.
 
-```bash
-python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
-```
+.. code:: bash
+
+   python main.py --config first.yaml,second.yaml --param1=1 --subconfig.param2='foo'
 
 **By default, these additional configs cannot add new parameters to the default config
 (for security and retro-compatibility reasons).**
 
-See [*Quick Start*](https://cliconfig.readthedocs.io/en/stable/quick_start.html) section
-of the documentation for more details.
-
-## With processing
+With processing
+---------------
 
 The library provide powerfull tools to modify the configuration called "processings".
 One of the possibility they add is to merge multiple configurations,
 copy a parameter on another, enforce type and more. To do so, simply adding the
 corresponding tags to your parameter names (on config files or CLI parameters).
 
 For instance with these config files:
 
-```yaml
-# main.yaml
-path_1@merge_add: sub1.yaml
-path_2@merge_add: sub2.yaml
-config3.select@select: config3.param1
-
-# sub1.yaml
-config1:
-  param@copy@type:int: config2.param
-  param2@type:int: 1
-
-# sub2.yaml
-config2.param@type:None|int: 2
-config3:
-  param1: 0
-  param2: 1
-```
+.. code:: yaml
+
+    # main.yaml
+    path_1@merge_add: sub1.yaml
+    path_2@merge_add: sub2.yaml
+    config3.select@select: config3.param1
+
+    # sub1.yaml
+    config1:
+      param@copy@type:int: config2.param
+      param2@type:None|int: 1
+
+    # sub2.yaml
+    config2.param@type:int: 2
+    config3:
+      param1: 0
+      param2: 1
 
 Note that can also use YAML tags separated with "@" (like `key: !tag@tag2 value`)
 to add tags instead of putting them in the parameter name (like `key@tag@tag2: value`).
 
-Here `main.yaml` is interpreted like:
+Here `main.yaml` will be interpreted like:
 
-```yaml
-path_1: sub1.yaml
-path_2: sub2.yaml
-config1:
-  param: 2  # the value of config2.param
-  param2: 1
-config2:
-  param: 2
-config3:
-  select: config3.param1
-  param1: 0
-  # param2 is deleted because it is not in the selection
-```
+.. code:: yaml
+
+    path_1: sub1.yaml
+    path_2: sub2.yaml
+    config1:
+      param: 2  # the value of config2.param
+      param2: 1
+    config2:
+      param: 2
+    config3:
+      select: config3.param1
+      param1: 0
+      # param2 is deleted because it is not in the selection
 
 Then, all the parameters in `config1` and `config2` have enforced types
 (`config2.param` can also be None) and changing `config2.param` will also update
 `config1.param` accordingly (which is protected by direct update).
 
-See [*Processing*](https://cliconfig.readthedocs.io/en/stable/processing.html) section
-of the documentation for details on processing and how to create your own.
-
-## How to contribute
-
-For **development**, install the package dynamically and dev requirements with:
-
-```bash
-pip install -e .
-pip install -r requirements-dev.txt
-```
-
-Everyone can contribute to CLI Config, and we value everyone’s contributions.
-Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
-
-## License
-
-Copyright (C) 2023  Valentin Goldité
-
-This program is free software: you can redistribute it and/or modify it under the
-terms of the [MIT License](LICENSE). This program is distributed in the hope that
-it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See *Quickstart* section for more details and *Processing* section for advanced usage.
 
-This project is free to use for COMMERCIAL USE, MODIFICATION, DISTRIBUTION and
-PRIVATE USE as long as the original license is include as well as this copy
-right notice at the top of the modified files.
+.. |PyPI version| image:: https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow
+   :target: https://pypi.org/project/cliconfig/
+.. |PythonVersion| image:: https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational
+.. |License| image:: https://img.shields.io/github/license/valentingol/cliconfig?color=999
+   :target: https://stringfixer.com/fr/MIT_license
+.. |Waka_Time| image:: https://wakatime.com/badge/github/valentingol/cliconfig.svg
+    :target: https://wakatime.com/badge/github/valentingol/cliconfig
+.. |Ruff_logo| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+   :target: https://github.com/charliermarsh/ruff
+.. |Black_logo| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+.. |Ruff| image:: https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml
+.. |Flake8| image:: https://github.com/valentingol/cliconfig/actions/workflows/flake.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/flake.yaml
+.. |Pydocstyle| image:: https://github.com/valentingol/cliconfig/actions/workflows/pydocstyle.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/pydocstyle.yaml
+.. |MyPy| image:: https://github.com/valentingol/cliconfig/actions/workflows/mypy.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/mypy.yaml
+.. |PyLint| image:: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/ab12676c87f0eaa715bef0f8ad31a604/raw/cliconfig_pylint.json
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/pylint.yaml
+.. |Tests| image:: https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml/badge.svg
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml
+.. |Coverage| image:: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/098e9c7c53be88779ee52ef2f2bc8803/raw/cliconfig_tests.json
+   :target: https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml
+.. |Documentation Status| image:: https://readthedocs.org/projects/cliconfig/badge/?version=latest
+   :target: https://cliconfig.readthedocs.io/en/latest/?badge=latest
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cliconfig-1.0.0b1/cliconfig.egg-info/SOURCES.txt` & `cliconfig-1.0.0b2/cliconfig.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .flake8
 .gitignore
 .markdownlint.json
 .pylintrc
 CONTRIBUTING.md
 LICENSE
 README.md
-README_pypi.md
 pre-commit-checks.sh
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.py
 .github/workflows/flake.yaml
 .github/workflows/mypy.yaml
@@ -35,14 +34,15 @@
 cliconfig/processing/__init__.py
 cliconfig/processing/_type_parser.py
 cliconfig/processing/base.py
 cliconfig/processing/builtin.py
 cliconfig/processing/create.py
 cliconfig/yaml_tags/_yaml_tags.py
 docs/Makefile
+docs/README_pypi.rst
 docs/cliconfig.processing_api.rst
 docs/cliconfig_api.rst
 docs/conf.py
 docs/contribute.md
 docs/edge_cases.md
 docs/index.rst
 docs/installation.md
@@ -63,14 +63,15 @@
 tests/conftest.py
 tests/configs/config1.yaml
 tests/configs/config2.yaml
 tests/configs/configtag1.yaml
 tests/configs/configtag2.yaml
 tests/configs/default1.yaml
 tests/configs/default2.yaml
+tests/configs/fallback.yaml
 tests/configs/multi_files_with_tags.yaml
 tests/configs/delete/config1.yaml
 tests/configs/delete/config2.yaml
 tests/configs/integration/test1/main.yaml
 tests/configs/integration/test1/sub1.yaml
 tests/configs/integration/test1/sub2.yaml
 tests/configs/integration/test2/data.yaml
```

### Comparing `cliconfig-1.0.0b1/docs/Makefile` & `cliconfig-1.0.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/docs/_static/logo.png` & `cliconfig-1.0.0b2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/docs/_static/logo_extend.png` & `cliconfig-1.0.0b2/docs/_static/logo_extend.png`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/docs/cliconfig_api.rst` & `cliconfig-1.0.0b2/docs/cliconfig_api.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/docs/conf.py` & `cliconfig-1.0.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/docs/edge_cases.md` & `cliconfig-1.0.0b2/docs/edge_cases.md`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/docs/license.md` & `cliconfig-1.0.0b2/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/docs/make.bat` & `cliconfig-1.0.0b2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/docs/processing.md` & `cliconfig-1.0.0b2/docs/processing.md`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/docs/quickstart.md` & `cliconfig-1.0.0b2/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/github_actions_utils/pydocstyle_manager.py` & `cliconfig-1.0.0b2/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/github_actions_utils/pylint_manager.py` & `cliconfig-1.0.0b2/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/github_actions_utils/pytest_manager.py` & `cliconfig-1.0.0b2/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-1.0.0b2/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/pre-commit-checks.sh` & `cliconfig-1.0.0b2/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/tests/configs/integration/test2/default.yaml` & `cliconfig-1.0.0b2/tests/configs/integration/test2/default.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/tests/conftest.py` & `cliconfig-1.0.0b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/tests/integration/test_inte_multiple_tags.py` & `cliconfig-1.0.0b2/tests/integration/test_inte_multiple_tags.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/tests/unit/processing/test_base_processing.py` & `cliconfig-1.0.0b2/tests/unit/processing/test_base_processing.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/tests/unit/processing/test_builtin.py` & `cliconfig-1.0.0b2/tests/unit/processing/test_builtin.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/tests/unit/processing/test_create.py` & `cliconfig-1.0.0b2/tests/unit/processing/test_create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/tests/unit/processing/test_type_parser.py` & `cliconfig-1.0.0b2/tests/unit/processing/test_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/tests/unit/test_base_config.py` & `cliconfig-1.0.0b2/tests/unit/test_base_config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/tests/unit/test_cli_parser.py` & `cliconfig-1.0.0b2/tests/unit/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/tests/unit/test_config_routines.py` & `cliconfig-1.0.0b2/tests/unit/test_config_routines.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         "--unknown2=8",  # check that not error but a warning in console
     ]
     capsys.readouterr()  # Clear stdout and stderr
     config = make_config(
         "tests/configs/default1.yaml",
         "tests/configs/default2.yaml",
         process_list=[process_add1],
+        fallback="tests/configs/fallback.yaml",
     )
     captured = capsys.readouterr()
     out = captured.out
     expected_config = {
         "param1": 4,
         "param2": 7,
         "param3": 3,
@@ -48,25 +49,29 @@
         "  - unknown2\n"
         "[CONFIG] Info: Merged 2 default config(s), "
         "2 additional config(s) and 1 CLI parameter(s).\n"
     )
     check.equal(config.dict, expected_config)
     check.equal(out, expected_out)
 
-    # No additional configs
+    # No additional configs and fallback
     sys.argv = [
         "tests/test_make_config.py.py",
     ]
-    config = make_config("tests/configs/default1.yaml", "tests/configs/default2.yaml")
+    config = make_config(
+        "tests/configs/default1.yaml",
+        "tests/configs/default2.yaml",
+        fallback="tests/configs/fallback.yaml",
+    )
     expected_config = {
         "param1": 1,
-        "param2": 2,
+        "param2": -1,
         "param3": 3,
         "letters": {
-            "letter1": "a",
+            "letter1": "z",
             "letter2": "b",
             "letter3": "c",
             "letter4": "d",
         },
     }
     check.equal(config.dict, expected_config)
     config = make_config(add_default_processing=False)
```

### Comparing `cliconfig-1.0.0b1/tests/unit/test_dict_routines.py` & `cliconfig-1.0.0b2/tests/unit/test_dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/tests/unit/test_ex_docs.py` & `cliconfig-1.0.0b2/tests/unit/test_ex_docs.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/tests/unit/test_process_routines.py` & `cliconfig-1.0.0b2/tests/unit/test_process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b1/tests/unit/test_tag_routines.py` & `cliconfig-1.0.0b2/tests/unit/test_tag_routines.py`

 * *Files identical despite different names*

