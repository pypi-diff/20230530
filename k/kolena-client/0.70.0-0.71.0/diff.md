# Comparing `tmp/kolena_client-0.70.0.tar.gz` & `tmp/kolena_client-0.71.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.70.0.tar", max compression
+gzip compressed data, was "kolena_client-0.71.0.tar", max compression
```

## Comparing `kolena_client-0.70.0.tar` & `kolena_client-0.71.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0    11346 2023-05-23 21:36:32.093116 kolena_client-0.70.0/LICENSE
--rw-r--r--   0        0        0      556 2023-05-23 21:36:32.093116 kolena_client-0.70.0/LICENSE_HEADER
--rw-r--r--   0        0        0     1546 2023-05-23 21:36:32.093116 kolena_client-0.70.0/README.md
--rw-r--r--   0        0        0     1356 2023-05-23 21:47:49.721301 kolena_client-0.70.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1737 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     8201 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7531 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5540 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      833 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0     1616 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     5313 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      783 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/consts.py
--rw-r--r--   0        0        0      579 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1183 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2990 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     4970 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-05-23 21:36:32.097116 kolena_client-0.70.0/kolena/_utils/log.py
--rw-r--r--   0        0        0     1003 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     5481 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     1942 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0      852 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1134 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1339 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3357 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3354 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    15677 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3566 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     3237 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2547 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2184 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4468 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6069 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/classification/test_run.py
--rw-r--r--   0        0        0     2813 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1351 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1321 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5454 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8566 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    13755 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1405 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     2049 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12341 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    13033 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     6309 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5232 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/inference.py
--rw-r--r--   0        0        0     1334 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/metadata.py
--rw-r--r--   0        0        0     2970 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/model.py
--rw-r--r--   0        0        0     2264 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3018 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/test_config.py
--rw-r--r--   0        0        0     5327 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5564 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2506 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2536 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/fr/__init__.py
--rw-r--r--   0        0        0     2171 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/fr/_utils.py
--rw-r--r--   0        0        0    20512 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/fr/datatypes.py
--rw-r--r--   0        0        0     9316 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/fr/model.py
--rw-r--r--   0        0        0    14583 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12193 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/fr/test_images.py
--rw-r--r--   0        0        0    16915 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/fr/test_run.py
--rw-r--r--   0        0        0    15376 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     3544 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/initialize.py
--rw-r--r--   0        0        0     4550 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13815 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     2559 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/workflow/_helpers.py
--rw-r--r--   0        0        0     6052 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0     8158 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     3842 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0    15849 2023-05-23 21:36:32.101117 kolena_client-0.70.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0    10725 2023-05-23 21:36:32.105116 kolena_client-0.70.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     3359 2023-05-23 21:36:32.105116 kolena_client-0.70.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     3433 2023-05-23 21:36:32.105116 kolena_client-0.70.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0      846 2023-05-23 21:36:32.105116 kolena_client-0.70.0/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0    14420 2023-05-23 21:36:32.105116 kolena_client-0.70.0/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     7589 2023-05-23 21:36:32.105116 kolena_client-0.70.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    13369 2023-05-23 21:36:32.105116 kolena_client-0.70.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    22768 2023-05-23 21:36:32.105116 kolena_client-0.70.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0     9155 2023-05-23 21:36:32.105116 kolena_client-0.70.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    14458 2023-05-23 21:36:32.105116 kolena_client-0.70.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0     9349 2023-05-23 21:36:32.105116 kolena_client-0.70.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     2560 2023-05-23 21:47:49.721301 kolena_client-0.70.0/pyproject.toml
--rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 kolena_client-0.70.0/setup.py
--rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 kolena_client-0.70.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-05-30 20:02:48.900738 kolena_client-0.71.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-05-30 20:02:48.900738 kolena_client-0.71.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     1546 2023-05-30 20:02:48.900738 kolena_client-0.71.0/README.md
+-rw-r--r--   0        0        0     1356 2023-05-30 20:11:54.468129 kolena_client-0.71.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     8201 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7531 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5540 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     1616 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     5313 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      783 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1183 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2990 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     4970 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     5450 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1942 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0      852 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1134 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1339 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3357 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3354 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    15698 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3566 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     3255 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2547 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2184 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4468 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6069 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     2813 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1351 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1321 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5454 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8566 2023-05-30 20:02:48.904738 kolena_client-0.71.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    13755 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1405 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     2049 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12341 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    13033 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     6309 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5232 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1334 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     2970 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2264 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3018 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     5327 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5564 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2506 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2536 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0     2171 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/fr/_utils.py
+-rw-r--r--   0        0        0    20512 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0     9316 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14583 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12193 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    16915 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    15376 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     3544 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/initialize.py
+-rw-r--r--   0        0        0     4550 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13815 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     2559 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/_helpers.py
+-rw-r--r--   0        0        0     6052 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0     8158 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     3842 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0    16970 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0    10725 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     3359 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     3433 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0      846 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0    14420 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     7589 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    13369 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    22768 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0     9155 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    14458 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0     9349 2023-05-30 20:02:48.908738 kolena_client-0.71.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     2560 2023-05-30 20:11:54.468129 kolena_client-0.71.0/pyproject.toml
+-rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 kolena_client-0.71.0/setup.py
+-rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 kolena_client-0.71.0/PKG-INFO
```

### Comparing `kolena_client-0.70.0/LICENSE` & `kolena_client-0.71.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/LICENSE_HEADER` & `kolena_client-0.71.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/README.md` & `kolena_client-0.71.0/README.md`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/__init__.py` & `kolena_client-0.71.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_api/__init__.py` & `kolena_client-0.71.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_api/v1/__init__.py` & `kolena_client-0.71.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_api/v1/batched_load.py` & `kolena_client-0.71.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_api/v1/client_log.py` & `kolena_client-0.71.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_api/v1/core.py` & `kolena_client-0.71.0/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_api/v1/detection.py` & `kolena_client-0.71.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_api/v1/fr.py` & `kolena_client-0.71.0/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_api/v1/generic.py` & `kolena_client-0.71.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_api/v1/repository.py` & `kolena_client-0.71.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_api/v1/token.py` & `kolena_client-0.71.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_api/v1/workflow.py` & `kolena_client-0.71.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/__init__.py` & `kolena_client-0.71.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/asset_path_mapper.py` & `kolena_client-0.71.0/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/batched_load.py` & `kolena_client-0.71.0/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/cli.py` & `kolena_client-0.71.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/consts.py` & `kolena_client-0.71.0/kolena/_utils/consts.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/dataframes/__init__.py` & `kolena_client-0.71.0/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/dataframes/validators.py` & `kolena_client-0.71.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/datatypes.py` & `kolena_client-0.71.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/endpoints.py` & `kolena_client-0.71.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/frozen.py` & `kolena_client-0.71.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/geometry.py` & `kolena_client-0.71.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/inference_validators.py` & `kolena_client-0.71.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/instrumentation.py` & `kolena_client-0.71.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/krequests.py` & `kolena_client-0.71.0/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/log.py` & `kolena_client-0.71.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/repository.py` & `kolena_client-0.71.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/serde.py` & `kolena_client-0.71.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/serializable.py` & `kolena_client-0.71.0/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/state.py` & `kolena_client-0.71.0/kolena/_utils/state.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 from kolena._utils.serde import from_dict
 from kolena.errors import InvalidClientStateError
 from kolena.errors import InvalidTokenError
 from kolena.errors import UnauthenticatedError
 from kolena.errors import UninitializedError
 
 API_VERSION = "v1"
-API_BASE_URL = "https://api.kolena.io"
-API_BASE_URL_ENV_VAR = "KOLENA_CLIENT_BASE_URL"
+API_URL = "https://api.kolena.io"
+API_URL_ENV_VAR = "KOLENA_API_URL"
 CLIENT_STATE = contextvars.ContextVar("client_state")
 
 
 class _ClientState:
     def __init__(
         self,
-        base_url: Optional[str] = API_BASE_URL,
+        base_url: Optional[str] = API_URL,
         api_token: Optional[str] = None,
         jwt_token: Optional[str] = None,
         tenant: Optional[str] = None,
         verbose: bool = False,
         telemetry: bool = False,
         proxies: Optional[Dict[str, str]] = None,
     ):
@@ -99,15 +99,15 @@
         self.jwt_token = None
         self.tenant = None
         self.verbose = False
         self.telemetry = False
 
 
 def _get_api_base_url() -> str:
-    return os.environ.get(API_BASE_URL_ENV_VAR, API_BASE_URL)
+    return os.environ.get(API_URL_ENV_VAR) or API_URL
 
 
 _client_state = _ClientState(base_url=_get_api_base_url())
 
 
 def get_client_state() -> _ClientState:
     return CLIENT_STATE.get(_client_state)
```

### Comparing `kolena_client-0.70.0/kolena/_utils/uninstantiable.py` & `kolena_client-0.71.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/_utils/validators.py` & `kolena_client-0.71.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/classification/__init__.py` & `kolena_client-0.71.0/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/classification/metadata.py` & `kolena_client-0.71.0/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/classification/model.py` & `kolena_client-0.71.0/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/classification/multiclass/__init__.py` & `kolena_client-0.71.0/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/classification/multiclass/_utils.py` & `kolena_client-0.71.0/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/classification/multiclass/evaluator.py` & `kolena_client-0.71.0/kolena/classification/multiclass/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         _as_class_metric_plot(field.name, metrics_by_label, labels)
         for field in dataclasses.fields(AggregatedMetrics)
         if len(gt_labels) > 2
         or field.name not in ["Precision", "Recall"]  # Omit single-class TC from precision and recall plots
     ]
 
     plots.extend(_compute_confidence_histograms(test_case_name, metrics, confidence_range))
-    plots.append(_compute_test_case_ovr_roc_curve(test_case_name, labels, ground_truths, inferences))
+    plots.append(_compute_test_case_ovr_roc_curve(test_case_name, gt_labels, ground_truths, inferences))
     plots.append(_compute_test_case_confusion_matrix(test_case_name, ground_truths, metrics))
     plots = list(filter(lambda plot: plot is not None, plots))
 
     return plots
 
 
 def _compute_test_case_confusion_matrix(
@@ -212,27 +212,27 @@
 
 def _compute_test_case_ovr_roc_curve(
     test_case_name: str,
     labels: List[str],
     ground_truths: List[GroundTruth],
     inferences: List[Inference],
 ) -> Optional[Plot]:
+    if len(labels) > 10:
+        log.warn(f"skipping one-vs-rest ROC curve for {test_case_name}: too many labels")
+        return None
+
     curves = []
     for label in labels:
         y_true = [1 if gt.classification.label == label else 0 for gt in ground_truths]
         y_score = [get_label_confidence(label, inf.inferences) for inf in inferences]
         fpr_values, tpr_values = roc_curve(y_true, y_score)
         if len(fpr_values) > 0 and len(tpr_values) > 0:
             curves.append(Curve(x=fpr_values, y=tpr_values, label=label))
 
     if len(curves) > 0:
-        if len(curves) > 10:
-            log.warn(f"skipping one-vs-rest ROC curve for {test_case_name}: too many labels")
-            return None
-
         return CurvePlot(
             title="Receiver Operating Characteristic (One-vs-Rest)",
             x_label="False Positive Rate (FPR)",
             y_label="True Positive Rate (TPR)",
             curves=curves,
         )
     return None
@@ -290,14 +290,15 @@
     macro_metrics_by_name: Dict[str, float] = {}
     for field in dataclasses.fields(AggregatedMetrics):
         metric_name = field.name
         metrics = [getattr(metrics_by_label[label], metric_name) for label in labels]
         macro_metrics_by_name[metric_name] = sum(metrics) / len(metrics)
 
     return TestCaseMetrics(
+        n_labels=len(labels),
         n_correct=n_correct,
         n_incorrect=n_incorrect,
         accuracy=accuracy,
         macro_precision=macro_metrics_by_name["Precision"],
         macro_recall=macro_metrics_by_name["Recall"],
         macro_f1=macro_metrics_by_name["F1"],
         macro_tpr=macro_metrics_by_name["Recall"],
```

### Comparing `kolena_client-0.70.0/kolena/classification/multiclass/test_run.py` & `kolena_client-0.71.0/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/classification/multiclass/workflow.py` & `kolena_client-0.71.0/kolena/classification/multiclass/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     Precision: float
     Recall: float
     FPR: float
 
 
 @dataclass(frozen=True)
 class TestCaseMetrics(MetricsTestCase):
+    n_labels: int
     n_correct: int
     n_incorrect: int
     accuracy: float
     macro_precision: float
     macro_recall: float
     macro_f1: float
     macro_tpr: float
```

### Comparing `kolena_client-0.70.0/kolena/classification/test_case.py` & `kolena_client-0.71.0/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/classification/test_config.py` & `kolena_client-0.71.0/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/classification/test_image.py` & `kolena_client-0.71.0/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/classification/test_run.py` & `kolena_client-0.71.0/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/classification/test_suite.py` & `kolena_client-0.71.0/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/__init__.py` & `kolena_client-0.71.0/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/_datatypes.py` & `kolena_client-0.71.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/_internal/__init__.py` & `kolena_client-0.71.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/_internal/datatypes.py` & `kolena_client-0.71.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/_internal/ground_truth.py` & `kolena_client-0.71.0/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/_internal/inference.py` & `kolena_client-0.71.0/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/_internal/metadata.py` & `kolena_client-0.71.0/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/_internal/model.py` & `kolena_client-0.71.0/kolena/detection/_internal/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/_internal/test_case.py` & `kolena_client-0.71.0/kolena/detection/_internal/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/_internal/test_config.py` & `kolena_client-0.71.0/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/_internal/test_image.py` & `kolena_client-0.71.0/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/_internal/test_run.py` & `kolena_client-0.71.0/kolena/detection/_internal/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/_internal/test_suite.py` & `kolena_client-0.71.0/kolena/detection/_internal/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/ground_truth.py` & `kolena_client-0.71.0/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/inference.py` & `kolena_client-0.71.0/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/metadata.py` & `kolena_client-0.71.0/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/model.py` & `kolena_client-0.71.0/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/test_case.py` & `kolena_client-0.71.0/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/test_config.py` & `kolena_client-0.71.0/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/test_image.py` & `kolena_client-0.71.0/kolena/detection/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/test_run.py` & `kolena_client-0.71.0/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/detection/test_suite.py` & `kolena_client-0.71.0/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/errors.py` & `kolena_client-0.71.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/fr/__init__.py` & `kolena_client-0.71.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/fr/_utils.py` & `kolena_client-0.71.0/kolena/fr/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/fr/datatypes.py` & `kolena_client-0.71.0/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/fr/model.py` & `kolena_client-0.71.0/kolena/fr/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/fr/test_case.py` & `kolena_client-0.71.0/kolena/fr/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/fr/test_images.py` & `kolena_client-0.71.0/kolena/fr/test_images.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/fr/test_run.py` & `kolena_client-0.71.0/kolena/fr/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/fr/test_suite.py` & `kolena_client-0.71.0/kolena/fr/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/initialize.py` & `kolena_client-0.71.0/kolena/initialize.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/__init__.py` & `kolena_client-0.71.0/kolena/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/_datatypes.py` & `kolena_client-0.71.0/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/_helpers.py` & `kolena_client-0.71.0/kolena/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/_validators.py` & `kolena_client-0.71.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/annotation.py` & `kolena_client-0.71.0/kolena/workflow/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/asset.py` & `kolena_client-0.71.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/evaluator.py` & `kolena_client-0.71.0/kolena/workflow/evaluator.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Type
 from typing import Union
 
+import numpy as np
 from pydantic import validate_arguments
 from pydantic.dataclasses import dataclass
 from pydantic.typing import Literal
 
 from kolena._api.v1.generic import TestRun as API
 from kolena._utils.validators import ValidatorConfig
 from kolena.workflow import GroundTruth
@@ -155,48 +156,60 @@
     def _data_type() -> _PlotType:
         return _PlotType.CURVE
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Histogram(Plot):
     """
-    A plot visualizing a histogram per test case.
+    A plot visualizing distribution of one or more continuous values, e.g. distribution of an error metric across all
+    samples within a test case.
 
-    Histograms allow for easy visualizations of data distributions.
+    For visualization of discrete values, see :class:`BarPlot`.
     """
 
     title: str
     x_label: str
     y_label: str
 
-    #: A Histogram requires intervals to bucket the data.
-    #: For n buckets, n+1 consecutive bounds must be specified in increasing order.
+    #: A Histogram requires intervals to bucket the data. For ``n`` buckets, ``n+1`` consecutive bounds must be
+    #: specified in increasing order.
     buckets: NumberSeries
 
-    #: For n buckets, there are n frequencies that define each bucket's height.
-    #: The nth frequency corresponds to the nth bucket.
-    frequency: NumberSeries
+    #: For ``n`` buckets, there are ``n`` frequencies corresponding to the height of each bucket. The frequency at index
+    #: ``i`` corresponds to the bucket with bounds (``i``, ``i+1``) in ``buckets``.
+    #:
+    #: To specify multiple distributions for a given test case, multiple frequency series can be provided, corresponding
+    #: e.g. to the distribution for a given class within a test case, with name specified in ``labels``.
+    frequency: Union[NumberSeries, Sequence[NumberSeries]]
+
+    #: Specify a list of labels corresponding to the different ``frequency`` series when multiple series are provided.
+    #: Can be omitted when a single ``frequency`` series is provided.
+    labels: Optional[List[str]] = None
 
     #: Custom format options to allow for control over the display of the plot axes.
     x_config: Optional[AxisConfig] = None
     y_config: Optional[AxisConfig] = None
 
     def __post_init_post_parse__(self) -> None:
-        if len(self.frequency) + 1 != len(self.buckets):
-            long_err_msg = (
-                f"Series 'frequency' (length: {len(self.frequency)}) "
-                f"and 'buckets' (length: {len(self.buckets)}) should be 1 apart"
-            )
-            raise ValueError(long_err_msg)
-
-        for i in range(len(self.buckets) - 1):
-            if self.buckets[i] >= self.buckets[i + 1]:
-                raise ValueError(
-                    f"At index {i}, {i + 1}, series 'buckets' is ({self.buckets[i]}, {self.buckets[i + 1]})",
-                )
+        n_buckets = len(self.buckets)
+        if n_buckets < 2:
+            raise ValueError(f"Minimum 2 entries required in 'buckets' series (length: {n_buckets})")
+        buckets_arr = np.array(self.buckets)
+        if not np.all(buckets_arr[1:] > buckets_arr[:-1]):  # validate strictly increasing
+            raise ValueError("Invalid 'buckets' series: series must be strictly increasing")
+
+        frequency_arr = np.array(self.frequency)
+        actual_frequency_shape = np.shape(frequency_arr)
+        if len(actual_frequency_shape) > 1 and self.labels is None:
+            raise ValueError("'labels' are required when multiple 'frequency' series are provided")
+
+        n_labels = len(self.labels or [])
+        expected_frequency_shape = (n_labels, n_buckets - 1) if n_labels > 0 else (n_buckets - 1,)
+        if actual_frequency_shape != expected_frequency_shape:
+            raise ValueError(f"Invalid 'frequency' shape {actual_frequency_shape}: expected {expected_frequency_shape}")
 
     @staticmethod
     def _data_type() -> _PlotType:
         return _PlotType.HISTOGRAM
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
```

### Comparing `kolena_client-0.70.0/kolena/workflow/evaluator_function.py` & `kolena_client-0.71.0/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/ground_truth.py` & `kolena_client-0.71.0/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/inference.py` & `kolena_client-0.71.0/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/metrics/__init__.py` & `kolena_client-0.71.0/kolena/workflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/metrics/_geometry.py` & `kolena_client-0.71.0/kolena/workflow/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/model.py` & `kolena_client-0.71.0/kolena/workflow/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/test_case.py` & `kolena_client-0.71.0/kolena/workflow/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/test_run.py` & `kolena_client-0.71.0/kolena/workflow/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/test_sample.py` & `kolena_client-0.71.0/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/test_suite.py` & `kolena_client-0.71.0/kolena/workflow/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/kolena/workflow/workflow.py` & `kolena_client-0.71.0/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.70.0/pyproject.toml` & `kolena_client-0.71.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena-client"
-version = "0.70.0"  # version is automatically set to latest git tag during release process
+version = "0.71.0"  # version is automatically set to latest git tag during release process
 description = "Client for Kolena's machine learning (ML) testing and debugging platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
```

### Comparing `kolena_client-0.70.0/setup.py` & `kolena_client-0.71.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                                                           'pandas>=1.1,<1.6']}
 
 entry_points = \
 {'console_scripts': ['kolena = kolena._utils.cli:run']}
 
 setup_kwargs = {
     'name': 'kolena-client',
-    'version': '0.70.0',
+    'version': '0.71.0',
     'description': "Client for Kolena's machine learning (ML) testing and debugging platform.",
     'long_description': '<p align="center">\n  <img src="https://app.kolena.io/api/developer/docs/html/_static/wordmark-purple.svg" width="400" alt="Kolena" />\n</p>\n\n<p align=\'center\'>\n  <a href="https://pypi.python.org/pypi/kolena"><img src="https://img.shields.io/pypi/v/kolena" /></a>\n  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena" /></a>\n  <a href="https://github.com/kolenaIO/kolena/actions"><img src="https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk" /></a>\n  <a href="https://codecov.io/gh/kolenaIO/kolena" ><img src="https://codecov.io/gh/kolenaIO/kolena/branch/trunk/graph/badge.svg?token=8WOY5I8SF1"/></a>\n  <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/resource-docs-6434c1" /></a>\n</p>\n\n---\n\n[Kolena](https://www.kolena.io) is a comprehensive machine learning testing and debugging platform to surface hidden\nmodel behaviors and take the mystery out of model development. Kolena helps you:\n\n- Perform high-resolution model evaluation\n- Understand and track behavioral improvements and regressions\n- Meaningfully communicate model capabilities\n- Automate model testing and deployment workflows\n\nThis `kolena` package contains the Python client library for programmatic interaction with the Kolena ML testing\nplatform.\n\n## Documentation\n\nVisit [docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation and the\n[API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena` typing and\nfunction documentation.\n',
     'author': 'Kolena Engineering',
     'author_email': 'eng@kolena.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kolena.io',
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 'pandera>=0.9.0', 'pyarrow>=8', 'pydantic>=1.8', 'requests-toolbelt',
 'requests>=2.20,<2.30', 'retrying>=1.3.3,<2.0.0', 'termcolor>=1.1.0,<2.0.0',
 'tqdm>=4,<5'] extras_require = \ {':python_version < "3.8"': ['importlib-
 metadata<5.0', 'typing-extensions>=4.5.0,<5.0.0'], ':python_version >= "3.11"':
 ['numpy>=1.23', 'pandas>=1.5,<1.6'], ':python_version >= "3.7" and
 python_version < "3.11"': ['numpy>=1.19', 'pandas>=1.1,<1.6']} entry_points = \
 {'console_scripts': ['kolena = kolena._utils.cli:run']} setup_kwargs =
-{ 'name': 'kolena-client', 'version': '0.70.0', 'description': "Client for
+{ 'name': 'kolena-client', 'version': '0.71.0', 'description': "Client for
 Kolena's machine learning (ML) testing and debugging platform.",
 'long_description': '
                                  \n [Kolena]\n
 \n\n
 \n [https://img.shields.io/pypi/v/kolena]\n [https://img.shields.io/pypi/l/
 kolena]\n [https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk]\n
 [https://codecov.io/gh/kolenaIO/kolena/branch/trunk/graph/
```

### Comparing `kolena_client-0.70.0/PKG-INFO` & `kolena_client-0.71.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena-client
-Version: 0.70.0
+Version: 0.71.0
 Summary: Client for Kolena's machine learning (ML) testing and debugging platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena-client Version: 0.70.0 Summary: Client for
+Metadata-Version: 2.1 Name: kolena-client Version: 0.71.0 Summary: Client for
 Kolena's machine learning (ML) testing and debugging platform. Home-page:
 https://kolena.io License: Apache-2.0 Keywords: Kolena,ML,testing Author:
 Kolena Engineering Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.12
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
```

