# Comparing `tmp/DeepUtilities-0.1.0.tar.gz` & `tmp/deeputilities-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepUtilities-0.1.0.tar", max compression
+gzip compressed data, was "deeputilities-0.1.1.tar", max compression
```

## Comparing `DeepUtilities-0.1.0.tar` & `deeputilities-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,58 @@
--rw-r--r--   0        0        0    11324 2022-03-19 16:21:25.005548 DeepUtilities-0.1.0/LICENSE
--rw-r--r--   0        0        0       16 2022-03-19 15:44:14.628502 DeepUtilities-0.1.0/README.md
--rw-r--r--   0        0        0      893 2022-03-19 16:54:22.249454 DeepUtilities-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-03-19 17:05:43.765806 DeepUtilities-0.1.0/src/deeputilities/__init__.py
--rw-r--r--   0        0        0      823 2022-03-19 17:34:23.379419 DeepUtilities-0.1.0/setup.py
--rw-r--r--   0        0        0      873 2022-03-19 17:34:23.379584 DeepUtilities-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2527 2023-05-28 23:40:29.935366 deeputilities-0.1.1/README.md
+-rw-r--r--   0        0        0     1133 2023-05-30 15:54:53.177955 deeputilities-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-28 23:40:29.931012 deeputilities-0.1.1/src/deeputilities/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:40:29.931220 deeputilities-0.1.1/src/deeputilities/client/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-30 15:25:14.668123 deeputilities-0.1.1/src/deeputilities/client/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      967 2023-05-30 15:40:49.614034 deeputilities-0.1.1/src/deeputilities/client/__pycache__/deeputils_app.cpython-311.pyc
+-rw-r--r--   0        0        0        4 2023-05-28 23:40:29.931344 deeputilities-0.1.1/src/deeputilities/client/commands/__init__.py
+-rw-r--r--   0        0        0      199 2023-05-30 15:26:11.645219 deeputilities-0.1.1/src/deeputilities/client/commands/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2126 2023-05-30 15:33:31.068312 deeputilities-0.1.1/src/deeputilities/client/commands/__pycache__/config_maker_command.cpython-311.pyc
+-rw-r--r--   0        0        0     7894 2023-05-30 15:49:08.472197 deeputilities-0.1.1/src/deeputilities/client/commands/__pycache__/demo_command.cpython-311.pyc
+-rw-r--r--   0        0        0     4812 2023-05-30 15:27:47.652935 deeputilities-0.1.1/src/deeputilities/client/commands/__pycache__/fullrun_command.cpython-311.pyc
+-rw-r--r--   0        0        0     3943 2023-05-30 15:30:21.279791 deeputilities-0.1.1/src/deeputilities/client/commands/__pycache__/ingest_command.cpython-311.pyc
+-rw-r--r--   0        0        0     1288 2023-05-29 23:01:19.382276 deeputilities-0.1.1/src/deeputilities/client/commands/config_maker_command.py
+-rw-r--r--   0        0        0     6220 2023-05-30 15:52:09.209497 deeputilities-0.1.1/src/deeputilities/client/commands/demo_command.py
+-rw-r--r--   0        0        0     4900 2023-05-30 15:27:12.577771 deeputilities-0.1.1/src/deeputilities/client/commands/diagnosis_command.py
+-rw-r--r--   0        0        0     4249 2023-05-30 15:27:32.797695 deeputilities-0.1.1/src/deeputilities/client/commands/fullrun_command.py
+-rw-r--r--   0        0        0     3355 2023-05-30 15:27:45.975539 deeputilities-0.1.1/src/deeputilities/client/commands/ingest_command.py
+-rw-r--r--   0        0        0      368 2023-05-30 15:40:47.725976 deeputilities-0.1.1/src/deeputilities/client/deeputils_app.py
+-rw-r--r--   0        0        0        0 2023-05-29 01:02:53.701894 deeputilities-0.1.1/src/deeputilities/client/options/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-30 15:30:21.280034 deeputilities-0.1.1/src/deeputilities/client/options/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1655 2023-05-30 15:30:50.760648 deeputilities-0.1.1/src/deeputilities/client/options/__pycache__/options.cpython-311.pyc
+-rw-r--r--   0        0        0     1684 2023-05-30 15:30:49.237225 deeputilities-0.1.1/src/deeputilities/client/options/options.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:40:29.931707 deeputilities-0.1.1/src/deeputilities/configuration/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-30 15:30:55.105611 deeputilities-0.1.1/src/deeputilities/configuration/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      177 2023-05-28 23:40:29.931842 deeputilities-0.1.1/src/deeputilities/configuration/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4670 2023-05-30 15:30:55.109996 deeputilities-0.1.1/src/deeputilities/configuration/__pycache__/configuration_object.cpython-311.pyc
+-rw-r--r--   0        0        0     5674 2023-05-30 15:32:22.394473 deeputilities-0.1.1/src/deeputilities/configuration/__pycache__/yaml_functions.cpython-311.pyc
+-rw-r--r--   0        0        0     2987 2023-05-28 23:40:29.931933 deeputilities-0.1.1/src/deeputilities/configuration/__pycache__/yaml_functions.cpython-39.pyc
+-rw-r--r--   0        0        0     3701 2023-05-29 22:55:36.030252 deeputilities-0.1.1/src/deeputilities/configuration/configuration_object.py
+-rw-r--r--   0        0        0      240 2023-05-29 03:44:25.676279 deeputilities-0.1.1/src/deeputilities/configuration/example_config.yaml
+-rw-r--r--   0        0        0     2900 2023-05-30 15:32:13.747070 deeputilities-0.1.1/src/deeputilities/configuration/yaml_functions.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:40:29.932163 deeputilities-0.1.1/src/deeputilities/diagnosis/__init__.py
+-rw-r--r--   0        0        0      438 2023-05-29 21:57:06.370255 deeputilities-0.1.1/src/deeputilities/diagnosis/diagnose.py
+-rw-r--r--   0        0        0     8941 2023-05-29 16:55:36.435680 deeputilities-0.1.1/src/deeputilities/diagnosis/diagnostics.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:40:29.932356 deeputilities-0.1.1/src/deeputilities/ingest/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-30 15:32:22.418959 deeputilities-0.1.1/src/deeputilities/ingest/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2040 2023-05-30 15:32:22.419430 deeputilities-0.1.1/src/deeputilities/ingest/__pycache__/ingestion.cpython-311.pyc
+-rw-r--r--   0        0        0      877 2023-05-29 13:01:45.177181 deeputilities-0.1.1/src/deeputilities/ingest/custom_dataset.py
+-rw-r--r--   0        0        0        0 2023-05-29 00:15:26.017197 deeputilities-0.1.1/src/deeputilities/ingest/datasets/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-29 00:51:06.729917 deeputilities-0.1.1/src/deeputilities/ingest/datasets/h5_dataset.py
+-rw-r--r--   0        0        0      278 2023-05-29 00:47:38.076248 deeputilities-0.1.1/src/deeputilities/ingest/datasets/image.py
+-rw-r--r--   0        0        0      263 2023-05-30 00:36:41.037038 deeputilities-0.1.1/src/deeputilities/ingest/datasets/image_dataset.py
+-rw-r--r--   0        0        0      225 2023-05-29 00:49:31.428773 deeputilities-0.1.1/src/deeputilities/ingest/datasets/numpy_dataset.py
+-rw-r--r--   0        0        0     1411 2023-05-30 00:29:47.607560 deeputilities-0.1.1/src/deeputilities/ingest/ingestion.py
+-rw-r--r--   0        0        0     7477 2023-05-28 23:40:29.932575 deeputilities-0.1.1/src/deeputilities/ingest/ingestor.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:40:29.932661 deeputilities-0.1.1/src/deeputilities/model/__init__.py
+-rw-r--r--   0        0        0     6653 2023-05-28 23:40:29.932809 deeputilities-0.1.1/src/deeputilities/model/architecture_search.py
+-rw-r--r--   0        0        0      865 2023-05-29 19:55:56.409461 deeputilities-0.1.1/src/deeputilities/model/deep_learning_models.py
+-rw-r--r--   0        0        0     5805 2023-05-28 23:40:29.932902 deeputilities-0.1.1/src/deeputilities/model/lazy_neural_network.py
+-rw-r--r--   0        0        0     1659 2023-05-28 23:40:29.932997 deeputilities-0.1.1/src/deeputilities/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:40:29.933070 deeputilities-0.1.1/src/deeputilities/preprocess/__init__.py
+-rw-r--r--   0        0        0      924 2023-05-29 14:45:17.168796 deeputilities-0.1.1/src/deeputilities/preprocess/preprocess.py
+-rw-r--r--   0        0        0     5620 2023-05-28 23:40:29.933206 deeputilities-0.1.1/src/deeputilities/preprocess/preprocessor.py
+-rw-r--r--   0        0        0     8819 2023-05-28 23:40:29.933323 deeputilities-0.1.1/src/deeputilities/preprocess/preprocessor_core.py
+-rw-r--r--   0        0        0     1828 2023-05-30 15:43:19.228338 deeputilities-0.1.1/src/deeputilities/settings.py
+-rw-r--r--   0        0        0      404 2023-05-28 23:40:29.933533 deeputilities-0.1.1/src/deeputilities/stand_in_pkg/deepbench.py
+-rw-r--r--   0        0        0      431 2023-05-28 23:40:29.933633 deeputilities-0.1.1/src/deeputilities/stand_in_pkg/deepgotdata.py
+-rw-r--r--   0        0        0     3565 1970-01-01 00:00:00.000000 deeputilities-0.1.1/PKG-INFO
```

### Comparing `DeepUtilities-0.1.0/pyproject.toml` & `deeputilities-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 [tool.poetry]
 name = "DeepUtilities"
-version = "0.1.0"
+version = "0.1.1"
 description = "A source-native, automated machine learning workflow"
 license = "Apache 2.0"
 authors = ["Ashia Lewis <pantagruelspendulum@protonmail.com>", "Maggie Voetberg <maggiev@fnal.gov>"]
 maintainers = ["Ashia Lewis <pantagruelspendulum@protonmail.com>", "Maggie Voetberg <maggiev@fnal.gov>"]
 readme = "README.md"
 homepage = "https://github.com/AeRabelais/DeepUtilities"
 repository = "https://github.com/AeRabelais/DeepUtilities"
 documentation = "https://github.com/AeRabelais/DeepUtilities/tree/main/docs"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pytest-cov = "^3.0.0"
+torch = "^2.0.1"
+cleo = "^2.0.1"
+torchvision = "^0.15.2"
+pandas = "^2.0.2"
+sklearn = "^0.0.post5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0.0"
 pre-commit = "^2.17.0"
 mypy = "^0.941"
 pylint = "^2.12.2"
 black = "^22.1.0"
 pyupgrade = "^2.31.1"
 
+[tool.poetry.group.dev.dependencies]
+ipykernel = "^6.21.3"
+
+[tool.poetry.scripts]
+deeputils = "src.deeputilities.client.deeputils_app:main"
+
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

