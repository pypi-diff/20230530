# Comparing `tmp/mypy-boto3-personalize-1.26.12.tar.gz` & `tmp/mypy-boto3-personalize-1.26.143.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-personalize-1.26.12.tar", last modified: Thu Nov 17 20:31:21 2022, max compression
+gzip compressed data, was "mypy-boto3-personalize-1.26.143.tar", last modified: Tue May 30 19:32:53 2023, max compression
```

## Comparing `mypy-boto3-personalize-1.26.12.tar` & `mypy-boto3-personalize-1.26.143.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:31:21.728784 mypy-boto3-personalize-1.26.12/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-17 20:30:34.000000 mypy-boto3-personalize-1.26.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    23582 2022-11-17 20:31:21.728784 mypy-boto3-personalize-1.26.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    22129 2022-11-17 20:30:34.000000 mypy-boto3-personalize-1.26.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:31:21.720784 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/
--rw-r--r--   0 runner    (1001) docker     (121)     3818 2022-11-17 20:30:34.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3817 2022-11-17 20:30:34.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-11-17 20:30:34.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    51001 2022-11-17 20:30:34.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    50912 2022-11-17 20:30:34.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9704 2022-11-17 20:30:35.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9702 2022-11-17 20:30:35.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    18693 2022-11-17 20:30:34.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    18674 2022-11-17 20:30:34.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 20:30:34.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    62181 2022-11-17 20:30:37.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    62146 2022-11-17 20:30:36.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-17 20:30:34.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:31:21.728784 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    23582 2022-11-17 20:31:21.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-11-17 20:31:21.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 20:31:21.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 20:31:21.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-17 20:31:21.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-17 20:31:21.000000 mypy-boto3-personalize-1.26.12/mypy_boto3_personalize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 20:31:21.728784 mypy-boto3-personalize-1.26.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1992 2022-11-17 20:30:34.000000 mypy-boto3-personalize-1.26.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:32:53.431270 mypy-boto3-personalize-1.26.143/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23648 2023-05-30 19:32:53.431270 mypy-boto3-personalize-1.26.143/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22143 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:32:53.419270 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50999 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50910 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-05-30 19:32:22.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-05-30 19:32:22.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18693 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62496 2023-05-30 19:32:23.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62461 2023-05-30 19:32:23.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:32:53.431270 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23648 2023-05-30 19:32:53.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-30 19:32:53.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:32:53.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:32:53.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 19:32:53.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 19:32:53.000000 mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:32:53.431270 mypy-boto3-personalize-1.26.143/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-30 19:32:21.000000 mypy-boto3-personalize-1.26.143/setup.py
```

### Comparing `mypy-boto3-personalize-1.26.12/LICENSE` & `mypy-boto3-personalize-1.26.143/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-personalize-1.26.12/PKG-INFO` & `mypy-boto3-personalize-1.26.143/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize
-Version: 1.26.12
-Summary: Type annotations for boto3.Personalize 1.26.12 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.143
+Summary: Type annotations for boto3.Personalize 1.26.143 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-personalize"></a>
 
 # mypy-boto3-personalize
 
 [![PyPI - mypy-boto3-personalize](https://img.shields.io/pypi/v/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.26.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.26.143](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
 
@@ -403,15 +404,14 @@
     CampaignSummaryTypeDef,
     CategoricalHyperParameterRangeTypeDef,
     ContinuousHyperParameterRangeTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DataSourceTypeDef,
     MetricAttributeTypeDef,
-    RecommenderConfigTypeDef,
     CreateSchemaRequestRequestTypeDef,
     DatasetExportJobSummaryTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetGroupTypeDef,
     DatasetImportJobSummaryTypeDef,
     DatasetSchemaSummaryTypeDef,
     DatasetSchemaTypeDef,
@@ -475,14 +475,15 @@
     ListSchemasRequestRequestTypeDef,
     ListSolutionVersionsRequestRequestTypeDef,
     SolutionVersionSummaryTypeDef,
     ListSolutionsRequestRequestTypeDef,
     SolutionSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     OptimizationObjectiveTypeDef,
+    TrainingDataConfigTypeDef,
     TunedHPOParamsTypeDef,
     StartRecommenderRequestRequestTypeDef,
     StopRecommenderRequestRequestTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
@@ -523,18 +524,14 @@
     StopRecommenderResponseTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateMetricAttributionResponseTypeDef,
     UpdateRecommenderResponseTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobTypeDef,
     ListMetricAttributionMetricsResponseTypeDef,
-    CreateRecommenderRequestRequestTypeDef,
-    RecommenderSummaryTypeDef,
-    RecommenderUpdateSummaryTypeDef,
-    UpdateRecommenderRequestRequestTypeDef,
     ListDatasetExportJobsResponseTypeDef,
     ListDatasetGroupsResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListSchemasResponseTypeDef,
     DescribeSchemaResponseTypeDef,
     ListDatasetsResponseTypeDef,
@@ -563,40 +560,45 @@
     ListSchemasRequestListSchemasPaginateTypeDef,
     ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
     ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListMetricAttributionsResponseTypeDef,
     ListRecipesResponseTypeDef,
     ListSolutionVersionsResponseTypeDef,
     ListSolutionsResponseTypeDef,
+    RecommenderConfigTypeDef,
     BatchInferenceJobTypeDef,
     CreateBatchInferenceJobRequestRequestTypeDef,
     BatchSegmentJobTypeDef,
     CreateBatchSegmentJobRequestRequestTypeDef,
     CreateDatasetExportJobRequestRequestTypeDef,
     DatasetExportJobTypeDef,
     CreateMetricAttributionRequestRequestTypeDef,
     MetricAttributionTypeDef,
     UpdateMetricAttributionRequestRequestTypeDef,
     CampaignTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
-    ListRecommendersResponseTypeDef,
-    RecommenderTypeDef,
     AlgorithmTypeDef,
     HPOConfigTypeDef,
+    CreateRecommenderRequestRequestTypeDef,
+    RecommenderSummaryTypeDef,
+    RecommenderUpdateSummaryTypeDef,
+    UpdateRecommenderRequestRequestTypeDef,
     DescribeBatchInferenceJobResponseTypeDef,
     DescribeBatchSegmentJobResponseTypeDef,
     DescribeDatasetExportJobResponseTypeDef,
     DescribeMetricAttributionResponseTypeDef,
     DescribeCampaignResponseTypeDef,
-    DescribeRecommenderResponseTypeDef,
     DescribeAlgorithmResponseTypeDef,
     SolutionConfigTypeDef,
+    ListRecommendersResponseTypeDef,
+    RecommenderTypeDef,
     CreateSolutionRequestRequestTypeDef,
     SolutionTypeDef,
     SolutionVersionTypeDef,
+    DescribeRecommenderResponseTypeDef,
     DescribeSolutionResponseTypeDef,
     DescribeSolutionVersionResponseTypeDef,
 )
 
 
 def get_structure() -> AlgorithmImageTypeDef:
     return {...}
@@ -605,42 +607,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-personalize-1.26.12/README.md` & `mypy-boto3-personalize-1.26.143/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-personalize"></a>
 
 # mypy-boto3-personalize
 
 [![PyPI - mypy-boto3-personalize](https://img.shields.io/pypi/v/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.26.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.26.143](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
 
@@ -372,15 +372,14 @@
     CampaignSummaryTypeDef,
     CategoricalHyperParameterRangeTypeDef,
     ContinuousHyperParameterRangeTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DataSourceTypeDef,
     MetricAttributeTypeDef,
-    RecommenderConfigTypeDef,
     CreateSchemaRequestRequestTypeDef,
     DatasetExportJobSummaryTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetGroupTypeDef,
     DatasetImportJobSummaryTypeDef,
     DatasetSchemaSummaryTypeDef,
     DatasetSchemaTypeDef,
@@ -444,14 +443,15 @@
     ListSchemasRequestRequestTypeDef,
     ListSolutionVersionsRequestRequestTypeDef,
     SolutionVersionSummaryTypeDef,
     ListSolutionsRequestRequestTypeDef,
     SolutionSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     OptimizationObjectiveTypeDef,
+    TrainingDataConfigTypeDef,
     TunedHPOParamsTypeDef,
     StartRecommenderRequestRequestTypeDef,
     StopRecommenderRequestRequestTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
@@ -492,18 +492,14 @@
     StopRecommenderResponseTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateMetricAttributionResponseTypeDef,
     UpdateRecommenderResponseTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobTypeDef,
     ListMetricAttributionMetricsResponseTypeDef,
-    CreateRecommenderRequestRequestTypeDef,
-    RecommenderSummaryTypeDef,
-    RecommenderUpdateSummaryTypeDef,
-    UpdateRecommenderRequestRequestTypeDef,
     ListDatasetExportJobsResponseTypeDef,
     ListDatasetGroupsResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListSchemasResponseTypeDef,
     DescribeSchemaResponseTypeDef,
     ListDatasetsResponseTypeDef,
@@ -532,40 +528,45 @@
     ListSchemasRequestListSchemasPaginateTypeDef,
     ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
     ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListMetricAttributionsResponseTypeDef,
     ListRecipesResponseTypeDef,
     ListSolutionVersionsResponseTypeDef,
     ListSolutionsResponseTypeDef,
+    RecommenderConfigTypeDef,
     BatchInferenceJobTypeDef,
     CreateBatchInferenceJobRequestRequestTypeDef,
     BatchSegmentJobTypeDef,
     CreateBatchSegmentJobRequestRequestTypeDef,
     CreateDatasetExportJobRequestRequestTypeDef,
     DatasetExportJobTypeDef,
     CreateMetricAttributionRequestRequestTypeDef,
     MetricAttributionTypeDef,
     UpdateMetricAttributionRequestRequestTypeDef,
     CampaignTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
-    ListRecommendersResponseTypeDef,
-    RecommenderTypeDef,
     AlgorithmTypeDef,
     HPOConfigTypeDef,
+    CreateRecommenderRequestRequestTypeDef,
+    RecommenderSummaryTypeDef,
+    RecommenderUpdateSummaryTypeDef,
+    UpdateRecommenderRequestRequestTypeDef,
     DescribeBatchInferenceJobResponseTypeDef,
     DescribeBatchSegmentJobResponseTypeDef,
     DescribeDatasetExportJobResponseTypeDef,
     DescribeMetricAttributionResponseTypeDef,
     DescribeCampaignResponseTypeDef,
-    DescribeRecommenderResponseTypeDef,
     DescribeAlgorithmResponseTypeDef,
     SolutionConfigTypeDef,
+    ListRecommendersResponseTypeDef,
+    RecommenderTypeDef,
     CreateSolutionRequestRequestTypeDef,
     SolutionTypeDef,
     SolutionVersionTypeDef,
+    DescribeRecommenderResponseTypeDef,
     DescribeSolutionResponseTypeDef,
     DescribeSolutionVersionResponseTypeDef,
 )
 
 
 def get_structure() -> AlgorithmImageTypeDef:
     return {...}
@@ -574,42 +575,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/__init__.py` & `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/__init__.pyi` & `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/__main__.py` & `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Personalize 1.26.12\nVersion:         1.26.12\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.Personalize 1.26.143\nVersion:         1.26.143\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.12")
+    print("1.26.143")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/client.py` & `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -820,15 +820,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solutions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solutions)
         """
 
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
-        Get a list of [tags](https://docs.aws.amazon.com/personalize/latest/dev/tagging-
+        Get a list of [tags](https://docs.aws.amazon.com/personalize/latest/dg/tagging-
         resources.html)_ attached to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_tags_for_resource)
         """
 
     def start_recommender(self, *, recommenderArn: str) -> StartRecommenderResponseTypeDef:
@@ -864,15 +864,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#tag_resource)
         """
 
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Remove [tags](https://docs.aws.amazon.com/personalize/latest/dev/tagging-
+        Remove [tags](https://docs.aws.amazon.com/personalize/latest/dg/tagging-
         resources.html)_ that are attached to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#untag_resource)
         """
 
     def update_campaign(
```

### Comparing `mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/client.pyi` & `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -755,15 +755,15 @@
         Returns a list of solutions that use the given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solutions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solutions)
         """
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
-        Get a list of [tags](https://docs.aws.amazon.com/personalize/latest/dev/tagging-
+        Get a list of [tags](https://docs.aws.amazon.com/personalize/latest/dg/tagging-
         resources.html)_ attached to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_tags_for_resource)
         """
     def start_recommender(self, *, recommenderArn: str) -> StartRecommenderResponseTypeDef:
         """
@@ -794,15 +794,15 @@
         Add a list of tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#tag_resource)
         """
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Remove [tags](https://docs.aws.amazon.com/personalize/latest/dev/tagging-
+        Remove [tags](https://docs.aws.amazon.com/personalize/latest/dg/tagging-
         resources.html)_ that are attached to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#untag_resource)
         """
     def update_campaign(
         self,
```

### Comparing `mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/literals.py` & `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -110,27 +111,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -159,14 +164,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -211,51 +217,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -268,14 +280,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -287,28 +300,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -336,57 +354,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssmsap",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/literals.pyi` & `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -108,27 +109,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -157,14 +162,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -209,51 +215,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -266,14 +278,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -285,28 +298,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -334,57 +352,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssmsap",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/paginator.py` & `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/paginator.pyi` & `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/type_defs.py` & `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     "CampaignSummaryTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
     "ContinuousHyperParameterRangeTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DataSourceTypeDef",
     "MetricAttributeTypeDef",
-    "RecommenderConfigTypeDef",
     "CreateSchemaRequestRequestTypeDef",
     "DatasetExportJobSummaryTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetGroupTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DatasetSchemaSummaryTypeDef",
     "DatasetSchemaTypeDef",
@@ -117,14 +116,15 @@
     "ListSchemasRequestRequestTypeDef",
     "ListSolutionVersionsRequestRequestTypeDef",
     "SolutionVersionSummaryTypeDef",
     "ListSolutionsRequestRequestTypeDef",
     "SolutionSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OptimizationObjectiveTypeDef",
+    "TrainingDataConfigTypeDef",
     "TunedHPOParamsTypeDef",
     "StartRecommenderRequestRequestTypeDef",
     "StopRecommenderRequestRequestTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
@@ -165,18 +165,14 @@
     "StopRecommenderResponseTypeDef",
     "UpdateCampaignResponseTypeDef",
     "UpdateMetricAttributionResponseTypeDef",
     "UpdateRecommenderResponseTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobTypeDef",
     "ListMetricAttributionMetricsResponseTypeDef",
-    "CreateRecommenderRequestRequestTypeDef",
-    "RecommenderSummaryTypeDef",
-    "RecommenderUpdateSummaryTypeDef",
-    "UpdateRecommenderRequestRequestTypeDef",
     "ListDatasetExportJobsResponseTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "DescribeDatasetGroupResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "DescribeSchemaResponseTypeDef",
     "ListDatasetsResponseTypeDef",
@@ -205,40 +201,45 @@
     "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
     "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListMetricAttributionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
     "ListSolutionVersionsResponseTypeDef",
     "ListSolutionsResponseTypeDef",
+    "RecommenderConfigTypeDef",
     "BatchInferenceJobTypeDef",
     "CreateBatchInferenceJobRequestRequestTypeDef",
     "BatchSegmentJobTypeDef",
     "CreateBatchSegmentJobRequestRequestTypeDef",
     "CreateDatasetExportJobRequestRequestTypeDef",
     "DatasetExportJobTypeDef",
     "CreateMetricAttributionRequestRequestTypeDef",
     "MetricAttributionTypeDef",
     "UpdateMetricAttributionRequestRequestTypeDef",
     "CampaignTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
-    "ListRecommendersResponseTypeDef",
-    "RecommenderTypeDef",
     "AlgorithmTypeDef",
     "HPOConfigTypeDef",
+    "CreateRecommenderRequestRequestTypeDef",
+    "RecommenderSummaryTypeDef",
+    "RecommenderUpdateSummaryTypeDef",
+    "UpdateRecommenderRequestRequestTypeDef",
     "DescribeBatchInferenceJobResponseTypeDef",
     "DescribeBatchSegmentJobResponseTypeDef",
     "DescribeDatasetExportJobResponseTypeDef",
     "DescribeMetricAttributionResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
-    "DescribeRecommenderResponseTypeDef",
     "DescribeAlgorithmResponseTypeDef",
     "SolutionConfigTypeDef",
+    "ListRecommendersResponseTypeDef",
+    "RecommenderTypeDef",
     "CreateSolutionRequestRequestTypeDef",
     "SolutionTypeDef",
     "SolutionVersionTypeDef",
+    "DescribeRecommenderResponseTypeDef",
     "DescribeSolutionResponseTypeDef",
     "DescribeSolutionVersionResponseTypeDef",
 )
 
 _RequiredAlgorithmImageTypeDef = TypedDict(
     "_RequiredAlgorithmImageTypeDef",
     {
@@ -402,23 +403,14 @@
     {
         "eventType": str,
         "metricName": str,
         "expression": str,
     },
 )
 
-RecommenderConfigTypeDef = TypedDict(
-    "RecommenderConfigTypeDef",
-    {
-        "itemExplorationConfig": Mapping[str, str],
-        "minRecommendationRequestsPerSecond": int,
-    },
-    total=False,
-)
-
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaRequestRequestTypeDef",
     {
         "name": str,
         "schema": str,
     },
 )
@@ -1114,14 +1106,22 @@
     {
         "itemAttribute": str,
         "objectiveSensitivity": ObjectiveSensitivityType,
     },
     total=False,
 )
 
+TrainingDataConfigTypeDef = TypedDict(
+    "TrainingDataConfigTypeDef",
+    {
+        "excludedDatasetColumns": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
 TunedHPOParamsTypeDef = TypedDict(
     "TunedHPOParamsTypeDef",
     {
         "algorithmHyperParameters": Dict[str, str],
     },
     total=False,
 )
@@ -1654,73 +1654,14 @@
     {
         "metrics": List[MetricAttributeTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRecommenderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecommenderRequestRequestTypeDef",
-    {
-        "name": str,
-        "datasetGroupArn": str,
-        "recipeArn": str,
-    },
-)
-_OptionalCreateRecommenderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecommenderRequestRequestTypeDef",
-    {
-        "recommenderConfig": RecommenderConfigTypeDef,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateRecommenderRequestRequestTypeDef(
-    _RequiredCreateRecommenderRequestRequestTypeDef, _OptionalCreateRecommenderRequestRequestTypeDef
-):
-    pass
-
-
-RecommenderSummaryTypeDef = TypedDict(
-    "RecommenderSummaryTypeDef",
-    {
-        "name": str,
-        "recommenderArn": str,
-        "datasetGroupArn": str,
-        "recipeArn": str,
-        "recommenderConfig": RecommenderConfigTypeDef,
-        "status": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-    },
-    total=False,
-)
-
-RecommenderUpdateSummaryTypeDef = TypedDict(
-    "RecommenderUpdateSummaryTypeDef",
-    {
-        "recommenderConfig": RecommenderConfigTypeDef,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "status": str,
-        "failureReason": str,
-    },
-    total=False,
-)
-
-UpdateRecommenderRequestRequestTypeDef = TypedDict(
-    "UpdateRecommenderRequestRequestTypeDef",
-    {
-        "recommenderArn": str,
-        "recommenderConfig": RecommenderConfigTypeDef,
-    },
-)
-
 ListDatasetExportJobsResponseTypeDef = TypedDict(
     "ListDatasetExportJobsResponseTypeDef",
     {
         "datasetExportJobs": List[DatasetExportJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2031,14 +1972,24 @@
     {
         "solutions": List[SolutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RecommenderConfigTypeDef = TypedDict(
+    "RecommenderConfigTypeDef",
+    {
+        "itemExplorationConfig": Mapping[str, str],
+        "minRecommendationRequestsPerSecond": int,
+        "trainingDataConfig": TrainingDataConfigTypeDef,
+    },
+    total=False,
+)
+
 BatchInferenceJobTypeDef = TypedDict(
     "BatchInferenceJobTypeDef",
     {
         "jobName": str,
         "batchInferenceJobArn": str,
         "filterArn": str,
         "failureReason": str,
@@ -2231,41 +2182,14 @@
     "DescribeDatasetImportJobResponseTypeDef",
     {
         "datasetImportJob": DatasetImportJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListRecommendersResponseTypeDef = TypedDict(
-    "ListRecommendersResponseTypeDef",
-    {
-        "recommenders": List[RecommenderSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RecommenderTypeDef = TypedDict(
-    "RecommenderTypeDef",
-    {
-        "recommenderArn": str,
-        "datasetGroupArn": str,
-        "name": str,
-        "recipeArn": str,
-        "recommenderConfig": RecommenderConfigTypeDef,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "status": str,
-        "failureReason": str,
-        "latestRecommenderUpdate": RecommenderUpdateSummaryTypeDef,
-        "modelMetrics": Dict[str, float],
-    },
-    total=False,
-)
-
 AlgorithmTypeDef = TypedDict(
     "AlgorithmTypeDef",
     {
         "name": str,
         "algorithmArn": str,
         "algorithmImage": AlgorithmImageTypeDef,
         "defaultHyperParameters": Dict[str, str],
@@ -2285,14 +2209,73 @@
         "hpoObjective": HPOObjectiveTypeDef,
         "hpoResourceConfig": HPOResourceConfigTypeDef,
         "algorithmHyperParameterRanges": HyperParameterRangesTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateRecommenderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecommenderRequestRequestTypeDef",
+    {
+        "name": str,
+        "datasetGroupArn": str,
+        "recipeArn": str,
+    },
+)
+_OptionalCreateRecommenderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecommenderRequestRequestTypeDef",
+    {
+        "recommenderConfig": RecommenderConfigTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateRecommenderRequestRequestTypeDef(
+    _RequiredCreateRecommenderRequestRequestTypeDef, _OptionalCreateRecommenderRequestRequestTypeDef
+):
+    pass
+
+
+RecommenderSummaryTypeDef = TypedDict(
+    "RecommenderSummaryTypeDef",
+    {
+        "name": str,
+        "recommenderArn": str,
+        "datasetGroupArn": str,
+        "recipeArn": str,
+        "recommenderConfig": RecommenderConfigTypeDef,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+    },
+    total=False,
+)
+
+RecommenderUpdateSummaryTypeDef = TypedDict(
+    "RecommenderUpdateSummaryTypeDef",
+    {
+        "recommenderConfig": RecommenderConfigTypeDef,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "status": str,
+        "failureReason": str,
+    },
+    total=False,
+)
+
+UpdateRecommenderRequestRequestTypeDef = TypedDict(
+    "UpdateRecommenderRequestRequestTypeDef",
+    {
+        "recommenderArn": str,
+        "recommenderConfig": RecommenderConfigTypeDef,
+    },
+)
+
 DescribeBatchInferenceJobResponseTypeDef = TypedDict(
     "DescribeBatchInferenceJobResponseTypeDef",
     {
         "batchInferenceJob": BatchInferenceJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2325,22 +2308,14 @@
     "DescribeCampaignResponseTypeDef",
     {
         "campaign": CampaignTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeRecommenderResponseTypeDef = TypedDict(
-    "DescribeRecommenderResponseTypeDef",
-    {
-        "recommender": RecommenderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAlgorithmResponseTypeDef = TypedDict(
     "DescribeAlgorithmResponseTypeDef",
     {
         "algorithm": AlgorithmTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2350,14 +2325,42 @@
     {
         "eventValueThreshold": str,
         "hpoConfig": HPOConfigTypeDef,
         "algorithmHyperParameters": Mapping[str, str],
         "featureTransformationParameters": Mapping[str, str],
         "autoMLConfig": AutoMLConfigTypeDef,
         "optimizationObjective": OptimizationObjectiveTypeDef,
+        "trainingDataConfig": TrainingDataConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecommendersResponseTypeDef = TypedDict(
+    "ListRecommendersResponseTypeDef",
+    {
+        "recommenders": List[RecommenderSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecommenderTypeDef = TypedDict(
+    "RecommenderTypeDef",
+    {
+        "recommenderArn": str,
+        "datasetGroupArn": str,
+        "name": str,
+        "recipeArn": str,
+        "recommenderConfig": RecommenderConfigTypeDef,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "status": str,
+        "failureReason": str,
+        "latestRecommenderUpdate": RecommenderUpdateSummaryTypeDef,
+        "modelMetrics": Dict[str, float],
     },
     total=False,
 )
 
 _RequiredCreateSolutionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSolutionRequestRequestTypeDef",
     {
@@ -2424,14 +2427,22 @@
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
+DescribeRecommenderResponseTypeDef = TypedDict(
+    "DescribeRecommenderResponseTypeDef",
+    {
+        "recommender": RecommenderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeSolutionResponseTypeDef = TypedDict(
     "DescribeSolutionResponseTypeDef",
     {
         "solution": SolutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-personalize-1.26.12/mypy_boto3_personalize/type_defs.pyi` & `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     "CampaignSummaryTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
     "ContinuousHyperParameterRangeTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DataSourceTypeDef",
     "MetricAttributeTypeDef",
-    "RecommenderConfigTypeDef",
     "CreateSchemaRequestRequestTypeDef",
     "DatasetExportJobSummaryTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetGroupTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DatasetSchemaSummaryTypeDef",
     "DatasetSchemaTypeDef",
@@ -116,14 +115,15 @@
     "ListSchemasRequestRequestTypeDef",
     "ListSolutionVersionsRequestRequestTypeDef",
     "SolutionVersionSummaryTypeDef",
     "ListSolutionsRequestRequestTypeDef",
     "SolutionSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OptimizationObjectiveTypeDef",
+    "TrainingDataConfigTypeDef",
     "TunedHPOParamsTypeDef",
     "StartRecommenderRequestRequestTypeDef",
     "StopRecommenderRequestRequestTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
@@ -164,18 +164,14 @@
     "StopRecommenderResponseTypeDef",
     "UpdateCampaignResponseTypeDef",
     "UpdateMetricAttributionResponseTypeDef",
     "UpdateRecommenderResponseTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobTypeDef",
     "ListMetricAttributionMetricsResponseTypeDef",
-    "CreateRecommenderRequestRequestTypeDef",
-    "RecommenderSummaryTypeDef",
-    "RecommenderUpdateSummaryTypeDef",
-    "UpdateRecommenderRequestRequestTypeDef",
     "ListDatasetExportJobsResponseTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "DescribeDatasetGroupResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "DescribeSchemaResponseTypeDef",
     "ListDatasetsResponseTypeDef",
@@ -204,40 +200,45 @@
     "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
     "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListMetricAttributionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
     "ListSolutionVersionsResponseTypeDef",
     "ListSolutionsResponseTypeDef",
+    "RecommenderConfigTypeDef",
     "BatchInferenceJobTypeDef",
     "CreateBatchInferenceJobRequestRequestTypeDef",
     "BatchSegmentJobTypeDef",
     "CreateBatchSegmentJobRequestRequestTypeDef",
     "CreateDatasetExportJobRequestRequestTypeDef",
     "DatasetExportJobTypeDef",
     "CreateMetricAttributionRequestRequestTypeDef",
     "MetricAttributionTypeDef",
     "UpdateMetricAttributionRequestRequestTypeDef",
     "CampaignTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
-    "ListRecommendersResponseTypeDef",
-    "RecommenderTypeDef",
     "AlgorithmTypeDef",
     "HPOConfigTypeDef",
+    "CreateRecommenderRequestRequestTypeDef",
+    "RecommenderSummaryTypeDef",
+    "RecommenderUpdateSummaryTypeDef",
+    "UpdateRecommenderRequestRequestTypeDef",
     "DescribeBatchInferenceJobResponseTypeDef",
     "DescribeBatchSegmentJobResponseTypeDef",
     "DescribeDatasetExportJobResponseTypeDef",
     "DescribeMetricAttributionResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
-    "DescribeRecommenderResponseTypeDef",
     "DescribeAlgorithmResponseTypeDef",
     "SolutionConfigTypeDef",
+    "ListRecommendersResponseTypeDef",
+    "RecommenderTypeDef",
     "CreateSolutionRequestRequestTypeDef",
     "SolutionTypeDef",
     "SolutionVersionTypeDef",
+    "DescribeRecommenderResponseTypeDef",
     "DescribeSolutionResponseTypeDef",
     "DescribeSolutionVersionResponseTypeDef",
 )
 
 _RequiredAlgorithmImageTypeDef = TypedDict(
     "_RequiredAlgorithmImageTypeDef",
     {
@@ -397,23 +398,14 @@
     {
         "eventType": str,
         "metricName": str,
         "expression": str,
     },
 )
 
-RecommenderConfigTypeDef = TypedDict(
-    "RecommenderConfigTypeDef",
-    {
-        "itemExplorationConfig": Mapping[str, str],
-        "minRecommendationRequestsPerSecond": int,
-    },
-    total=False,
-)
-
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaRequestRequestTypeDef",
     {
         "name": str,
         "schema": str,
     },
 )
@@ -1107,14 +1099,22 @@
     {
         "itemAttribute": str,
         "objectiveSensitivity": ObjectiveSensitivityType,
     },
     total=False,
 )
 
+TrainingDataConfigTypeDef = TypedDict(
+    "TrainingDataConfigTypeDef",
+    {
+        "excludedDatasetColumns": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
 TunedHPOParamsTypeDef = TypedDict(
     "TunedHPOParamsTypeDef",
     {
         "algorithmHyperParameters": Dict[str, str],
     },
     total=False,
 )
@@ -1629,71 +1629,14 @@
     {
         "metrics": List[MetricAttributeTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRecommenderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecommenderRequestRequestTypeDef",
-    {
-        "name": str,
-        "datasetGroupArn": str,
-        "recipeArn": str,
-    },
-)
-_OptionalCreateRecommenderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecommenderRequestRequestTypeDef",
-    {
-        "recommenderConfig": RecommenderConfigTypeDef,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateRecommenderRequestRequestTypeDef(
-    _RequiredCreateRecommenderRequestRequestTypeDef, _OptionalCreateRecommenderRequestRequestTypeDef
-):
-    pass
-
-RecommenderSummaryTypeDef = TypedDict(
-    "RecommenderSummaryTypeDef",
-    {
-        "name": str,
-        "recommenderArn": str,
-        "datasetGroupArn": str,
-        "recipeArn": str,
-        "recommenderConfig": RecommenderConfigTypeDef,
-        "status": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-    },
-    total=False,
-)
-
-RecommenderUpdateSummaryTypeDef = TypedDict(
-    "RecommenderUpdateSummaryTypeDef",
-    {
-        "recommenderConfig": RecommenderConfigTypeDef,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "status": str,
-        "failureReason": str,
-    },
-    total=False,
-)
-
-UpdateRecommenderRequestRequestTypeDef = TypedDict(
-    "UpdateRecommenderRequestRequestTypeDef",
-    {
-        "recommenderArn": str,
-        "recommenderConfig": RecommenderConfigTypeDef,
-    },
-)
-
 ListDatasetExportJobsResponseTypeDef = TypedDict(
     "ListDatasetExportJobsResponseTypeDef",
     {
         "datasetExportJobs": List[DatasetExportJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2004,14 +1947,24 @@
     {
         "solutions": List[SolutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RecommenderConfigTypeDef = TypedDict(
+    "RecommenderConfigTypeDef",
+    {
+        "itemExplorationConfig": Mapping[str, str],
+        "minRecommendationRequestsPerSecond": int,
+        "trainingDataConfig": TrainingDataConfigTypeDef,
+    },
+    total=False,
+)
+
 BatchInferenceJobTypeDef = TypedDict(
     "BatchInferenceJobTypeDef",
     {
         "jobName": str,
         "batchInferenceJobArn": str,
         "filterArn": str,
         "failureReason": str,
@@ -2198,41 +2151,14 @@
     "DescribeDatasetImportJobResponseTypeDef",
     {
         "datasetImportJob": DatasetImportJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListRecommendersResponseTypeDef = TypedDict(
-    "ListRecommendersResponseTypeDef",
-    {
-        "recommenders": List[RecommenderSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RecommenderTypeDef = TypedDict(
-    "RecommenderTypeDef",
-    {
-        "recommenderArn": str,
-        "datasetGroupArn": str,
-        "name": str,
-        "recipeArn": str,
-        "recommenderConfig": RecommenderConfigTypeDef,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "status": str,
-        "failureReason": str,
-        "latestRecommenderUpdate": RecommenderUpdateSummaryTypeDef,
-        "modelMetrics": Dict[str, float],
-    },
-    total=False,
-)
-
 AlgorithmTypeDef = TypedDict(
     "AlgorithmTypeDef",
     {
         "name": str,
         "algorithmArn": str,
         "algorithmImage": AlgorithmImageTypeDef,
         "defaultHyperParameters": Dict[str, str],
@@ -2252,14 +2178,71 @@
         "hpoObjective": HPOObjectiveTypeDef,
         "hpoResourceConfig": HPOResourceConfigTypeDef,
         "algorithmHyperParameterRanges": HyperParameterRangesTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateRecommenderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecommenderRequestRequestTypeDef",
+    {
+        "name": str,
+        "datasetGroupArn": str,
+        "recipeArn": str,
+    },
+)
+_OptionalCreateRecommenderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecommenderRequestRequestTypeDef",
+    {
+        "recommenderConfig": RecommenderConfigTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateRecommenderRequestRequestTypeDef(
+    _RequiredCreateRecommenderRequestRequestTypeDef, _OptionalCreateRecommenderRequestRequestTypeDef
+):
+    pass
+
+RecommenderSummaryTypeDef = TypedDict(
+    "RecommenderSummaryTypeDef",
+    {
+        "name": str,
+        "recommenderArn": str,
+        "datasetGroupArn": str,
+        "recipeArn": str,
+        "recommenderConfig": RecommenderConfigTypeDef,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+    },
+    total=False,
+)
+
+RecommenderUpdateSummaryTypeDef = TypedDict(
+    "RecommenderUpdateSummaryTypeDef",
+    {
+        "recommenderConfig": RecommenderConfigTypeDef,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "status": str,
+        "failureReason": str,
+    },
+    total=False,
+)
+
+UpdateRecommenderRequestRequestTypeDef = TypedDict(
+    "UpdateRecommenderRequestRequestTypeDef",
+    {
+        "recommenderArn": str,
+        "recommenderConfig": RecommenderConfigTypeDef,
+    },
+)
+
 DescribeBatchInferenceJobResponseTypeDef = TypedDict(
     "DescribeBatchInferenceJobResponseTypeDef",
     {
         "batchInferenceJob": BatchInferenceJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2292,22 +2275,14 @@
     "DescribeCampaignResponseTypeDef",
     {
         "campaign": CampaignTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeRecommenderResponseTypeDef = TypedDict(
-    "DescribeRecommenderResponseTypeDef",
-    {
-        "recommender": RecommenderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAlgorithmResponseTypeDef = TypedDict(
     "DescribeAlgorithmResponseTypeDef",
     {
         "algorithm": AlgorithmTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2317,14 +2292,42 @@
     {
         "eventValueThreshold": str,
         "hpoConfig": HPOConfigTypeDef,
         "algorithmHyperParameters": Mapping[str, str],
         "featureTransformationParameters": Mapping[str, str],
         "autoMLConfig": AutoMLConfigTypeDef,
         "optimizationObjective": OptimizationObjectiveTypeDef,
+        "trainingDataConfig": TrainingDataConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecommendersResponseTypeDef = TypedDict(
+    "ListRecommendersResponseTypeDef",
+    {
+        "recommenders": List[RecommenderSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecommenderTypeDef = TypedDict(
+    "RecommenderTypeDef",
+    {
+        "recommenderArn": str,
+        "datasetGroupArn": str,
+        "name": str,
+        "recipeArn": str,
+        "recommenderConfig": RecommenderConfigTypeDef,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "status": str,
+        "failureReason": str,
+        "latestRecommenderUpdate": RecommenderUpdateSummaryTypeDef,
+        "modelMetrics": Dict[str, float],
     },
     total=False,
 )
 
 _RequiredCreateSolutionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSolutionRequestRequestTypeDef",
     {
@@ -2389,14 +2392,22 @@
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
+DescribeRecommenderResponseTypeDef = TypedDict(
+    "DescribeRecommenderResponseTypeDef",
+    {
+        "recommender": RecommenderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeSolutionResponseTypeDef = TypedDict(
     "DescribeSolutionResponseTypeDef",
     {
         "solution": SolutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-personalize-1.26.12/mypy_boto3_personalize.egg-info/PKG-INFO` & `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize
-Version: 1.26.12
-Summary: Type annotations for boto3.Personalize 1.26.12 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.143
+Summary: Type annotations for boto3.Personalize 1.26.143 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-personalize"></a>
 
 # mypy-boto3-personalize
 
 [![PyPI - mypy-boto3-personalize](https://img.shields.io/pypi/v/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.26.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.26.143](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
 
@@ -403,15 +404,14 @@
     CampaignSummaryTypeDef,
     CategoricalHyperParameterRangeTypeDef,
     ContinuousHyperParameterRangeTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DataSourceTypeDef,
     MetricAttributeTypeDef,
-    RecommenderConfigTypeDef,
     CreateSchemaRequestRequestTypeDef,
     DatasetExportJobSummaryTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetGroupTypeDef,
     DatasetImportJobSummaryTypeDef,
     DatasetSchemaSummaryTypeDef,
     DatasetSchemaTypeDef,
@@ -475,14 +475,15 @@
     ListSchemasRequestRequestTypeDef,
     ListSolutionVersionsRequestRequestTypeDef,
     SolutionVersionSummaryTypeDef,
     ListSolutionsRequestRequestTypeDef,
     SolutionSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     OptimizationObjectiveTypeDef,
+    TrainingDataConfigTypeDef,
     TunedHPOParamsTypeDef,
     StartRecommenderRequestRequestTypeDef,
     StopRecommenderRequestRequestTypeDef,
     StopSolutionVersionCreationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
@@ -523,18 +524,14 @@
     StopRecommenderResponseTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateMetricAttributionResponseTypeDef,
     UpdateRecommenderResponseTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobTypeDef,
     ListMetricAttributionMetricsResponseTypeDef,
-    CreateRecommenderRequestRequestTypeDef,
-    RecommenderSummaryTypeDef,
-    RecommenderUpdateSummaryTypeDef,
-    UpdateRecommenderRequestRequestTypeDef,
     ListDatasetExportJobsResponseTypeDef,
     ListDatasetGroupsResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListSchemasResponseTypeDef,
     DescribeSchemaResponseTypeDef,
     ListDatasetsResponseTypeDef,
@@ -563,40 +560,45 @@
     ListSchemasRequestListSchemasPaginateTypeDef,
     ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef,
     ListSolutionsRequestListSolutionsPaginateTypeDef,
     ListMetricAttributionsResponseTypeDef,
     ListRecipesResponseTypeDef,
     ListSolutionVersionsResponseTypeDef,
     ListSolutionsResponseTypeDef,
+    RecommenderConfigTypeDef,
     BatchInferenceJobTypeDef,
     CreateBatchInferenceJobRequestRequestTypeDef,
     BatchSegmentJobTypeDef,
     CreateBatchSegmentJobRequestRequestTypeDef,
     CreateDatasetExportJobRequestRequestTypeDef,
     DatasetExportJobTypeDef,
     CreateMetricAttributionRequestRequestTypeDef,
     MetricAttributionTypeDef,
     UpdateMetricAttributionRequestRequestTypeDef,
     CampaignTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
-    ListRecommendersResponseTypeDef,
-    RecommenderTypeDef,
     AlgorithmTypeDef,
     HPOConfigTypeDef,
+    CreateRecommenderRequestRequestTypeDef,
+    RecommenderSummaryTypeDef,
+    RecommenderUpdateSummaryTypeDef,
+    UpdateRecommenderRequestRequestTypeDef,
     DescribeBatchInferenceJobResponseTypeDef,
     DescribeBatchSegmentJobResponseTypeDef,
     DescribeDatasetExportJobResponseTypeDef,
     DescribeMetricAttributionResponseTypeDef,
     DescribeCampaignResponseTypeDef,
-    DescribeRecommenderResponseTypeDef,
     DescribeAlgorithmResponseTypeDef,
     SolutionConfigTypeDef,
+    ListRecommendersResponseTypeDef,
+    RecommenderTypeDef,
     CreateSolutionRequestRequestTypeDef,
     SolutionTypeDef,
     SolutionVersionTypeDef,
+    DescribeRecommenderResponseTypeDef,
     DescribeSolutionResponseTypeDef,
     DescribeSolutionVersionResponseTypeDef,
 )
 
 
 def get_structure() -> AlgorithmImageTypeDef:
     return {...}
@@ -605,42 +607,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-personalize-1.26.12/mypy_boto3_personalize.egg-info/SOURCES.txt` & `mypy-boto3-personalize-1.26.143/mypy_boto3_personalize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.26.12/setup.py` & `mypy-boto3-personalize-1.26.143/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-personalize.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-personalize",
-    version="1.26.12",
+    version="1.26.143",
     packages=["mypy_boto3_personalize"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Personalize 1.26.12 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.Personalize 1.26.143 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 personalize type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_personalize": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_personalize": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

