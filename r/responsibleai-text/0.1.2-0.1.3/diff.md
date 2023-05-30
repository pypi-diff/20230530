# Comparing `tmp/responsibleai_text-0.1.2.tar.gz` & `tmp/responsibleai_text-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/responsibleai_text-0.1.2.tar", last modified: Thu May  4 21:48:52 2023, max compression
+gzip compressed data, was "dist/responsibleai_text-0.1.3.tar", last modified: Tue May 30 14:50:22 2023, max compression
```

## Comparing `responsibleai_text-0.1.2.tar` & `responsibleai_text-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text/common/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/common/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/managers/error_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/managers/explainer_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text/rai_text_insights/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/rai_text_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25504 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/rai_text_insights/rai_text_insights.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/utils/feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/utils/question_answering.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/responsibleai_text/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/responsibleai_text.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:52.000000 responsibleai_text-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/tests/test_feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/tests/test_rai_text_insights.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-04 21:46:08.000000 responsibleai_text-0.1.2/tests/test_rai_text_insights_save_and_load_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/common/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/managers/error_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/managers/explainer_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text/rai_text_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/rai_text_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34598 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/rai_text_insights/rai_text_insights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/utils/feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/utils/question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/tests/test_feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/tests/test_rai_text_insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/tests/test_rai_text_insights_save_and_load_scenarios.py
```

### Comparing `responsibleai_text-0.1.2/PKG-INFO` & `responsibleai_text-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: responsibleai_text
-Version: 0.1.2
+Version: 0.1.3
 Summary: SDK API to assess text Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: qa
 
 # Responsible AI Text SDK for Python
 
 ### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
 
 The Responsible AI Text sdk enables users to analyze their machine learning models for text data in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
 
@@ -26,8 +27,8 @@
 - `explainer.add()` explains the model
 
 ### Supported scenarios, models and datasets
 
 The Responsible AI Text SDK supports multiclass classification and question answering models on text data currently.
 
 The open source code for the visualization dashboard can be found here:
-https://github.com/microsoft/responsible-ai-widgets
+https://github.com/microsoft/responsible-ai-toolbox
```

### Comparing `responsibleai_text-0.1.2/README.md` & `responsibleai_text-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 - `explainer.add()` explains the model
 
 ### Supported scenarios, models and datasets
 
 The Responsible AI Text SDK supports multiclass classification and question answering models on text data currently.
 
 The open source code for the visualization dashboard can be found here:
-https://github.com/microsoft/responsible-ai-widgets
+https://github.com/microsoft/responsible-ai-toolbox
```

### Comparing `responsibleai_text-0.1.2/responsibleai_text/common/constants.py` & `responsibleai_text-0.1.3/responsibleai_text/common/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.2/responsibleai_text/managers/error_analysis_manager.py` & `responsibleai_text-0.1.3/responsibleai_text/managers/error_analysis_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
 """Defines the Error Analysis Manager class."""
 
 import json
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Union
 
 import jsonschema
 import numpy as np
 import pandas as pd
 from erroranalysis._internal.error_analyzer import ModelAnalyzer
 from erroranalysis._internal.error_report import as_error_report
 from ml_wrappers import wrap_model
 from responsibleai._tools.shared.state_directory_management import \
     DirectoryManager
 from responsibleai.managers.error_analysis_manager import \
     ErrorAnalysisManager as BaseErrorAnalysisManager
 from responsibleai.managers.error_analysis_manager import as_error_config
 
 from responsibleai_text.common.constants import ModelTask
+from responsibleai_text.utils.feature_extractors import get_text_columns
 
 LABELS = 'labels'
 
 
 def _concat_labels_column(dataset, target_column, classes):
     """Concatenate labels column for multilabel models.
 
@@ -63,15 +64,17 @@
         """
         self.model = model
         self.dataset = dataset
         self.classes = classes
         self.is_multilabel = is_multilabel
         self.task_type = task_type
         if self.task_type in [ModelTask.TEXT_CLASSIFICATION, ModelTask.MULTILABEL_TEXT_CLASSIFICATION]:
-            self.predictions = self.model.predict(self.dataset.iloc[:, 0].tolist())
+            dataset = self.dataset.iloc[:, 0].tolist()
+            self.predictions = self.model.predict(dataset)
+            self.predict_proba = self.model.predict_proba(dataset)
         elif self.task_type == ModelTask.QUESTION_ANSWERING:
             self.predictions = self.model.predict(self.dataset.loc[:, ['context', 'questions']])
             self.predictions = np.array(self.predictions)
         else:
             raise ValueError("Unknown task type: {}".format(self.task_type))
 
         if self.is_multilabel:
@@ -82,16 +85,14 @@
                 if self.classes is not None:
                     pred_labels = [self.classes[i] for i in pred_labels]
                 else:
                     pred_labels = [str(i) for i in pred_labels]
                 # concatenate all predicted labels into a single string
                 predictions_joined.append(','.join(pred_labels))
             self.predictions = np.array(predictions_joined)
-        if self.task_type != ModelTask.QUESTION_ANSWERING:
-            self.predict_proba = self.model.predict_proba(self.dataset.iloc[:, 0].tolist())
 
     def predict(self, X):
         """Predict the class labels for the provided data.
 
         :param X: Data to predict the labels for.
         :type X: pandas.DataFrame
         :return: Predicted class labels.
@@ -120,14 +121,15 @@
 
 class ErrorAnalysisManager(BaseErrorAnalysisManager):
 
     """Defines a wrapper class of Error Analysis for text scenario."""
 
     def __init__(self, model: Any, dataset: pd.DataFrame,
                  ext_dataset: pd.DataFrame, target_column: str,
+                 text_column: Optional[Union[str, List]],
                  task_type: str, classes: Optional[List] = None,
                  categorical_features: Optional[List[str]] = None):
         """Creates an ErrorAnalysisManager object.
 
         :param model: The model to analyze errors on.
             A model that implements sklearn.predict or sklearn.predict_proba
             or function that accepts a 2d ndarray.
@@ -136,14 +138,17 @@
         :type dataset: pandas.DataFrame
         :param ext_dataset: The dataset of extracted features including the
                             label column.
         :type ext_dataset: pandas.DataFrame
         :param target_column: The name of the label column or list of columns.
             This is a list of columns for multilabel models.
         :type target_column: str or list[str]
+        :param text_column: The name of the text column or list of columns.
+            This is a list of columns for question answering models.
+        :type text_column: str or list[str]
         :param task_type: The task to run.
         :type task_type: str
         :param classes: Class names as a list of strings.
             The order of the class names should match that of the model
             output.  Only required if analyzing a classifier.
         :type classes: list
         :param categorical_features: The categorical feature names.
@@ -160,50 +165,53 @@
             dataset[LABELS] = labels
             ext_dataset[LABELS] = dataset[LABELS]
             dataset.drop(columns=target_column, inplace=True)
             ext_dataset.drop(columns=target_column, inplace=True)
             target_column = LABELS
             is_multilabel = True
         index_predictor = ErrorAnalysisManager._create_index_predictor(
-            model, dataset, target_column, is_multilabel, task_type,
-            index_classes)
-        if task_type == ModelTask.QUESTION_ANSWERING:
-            categorical_features = ['question_type']
-        else:
+            model, dataset, target_column, text_column, is_multilabel,
+            task_type, index_classes)
+        if categorical_features is None:
             categorical_features = []
         super(ErrorAnalysisManager, self).__init__(
             index_predictor, ext_dataset, target_column,
             classes, categorical_features)
 
     @staticmethod
     def _create_index_predictor(model, dataset, target_column,
-                                is_multilabel, task_type, classes=None):
+                                text_column, is_multilabel,
+                                task_type, classes=None):
         """Creates a wrapped predictor that uses index to retrieve text data.
 
         :param model: The model to analyze errors on.
             A model that implements sklearn.predict or sklearn.predict_proba
             or function that accepts a 2d ndarray.
         :type model: object
         :param dataset: The dataset including the label column.
         :type dataset: pandas.DataFrame
         :param target_column: The name of the label column or list of columns.
             This is a list of columns for multilabel models.
         :type target_column: str or list[str]
+        :param text_column: The name of the text column or list of columns.
+            This is a list of columns for question answering models.
+        :type text_column: str or list[str]
         :param is_multilabel: Whether the model is multilabel.
         :type is_multilabel: bool
         :param task_type: The task to run.
         :type task_type: str
         :param classes: Class names as a list of strings.
             The order of the class names should match that of the model
             output.
         :type classes: list
         :return: A wrapped predictor that uses index to retrieve text data.
         :rtype: WrappedIndexPredictorModel
         """
         dataset = dataset.drop(columns=[target_column])
+        dataset = get_text_columns(dataset, text_column)
         index_predictor = WrappedIndexPredictorModel(
             model, dataset, is_multilabel, task_type, classes)
         return index_predictor
 
     @staticmethod
     def _load(path, rai_insights):
         """Load the ErrorAnalysisManager from the given path.
@@ -242,15 +250,16 @@
                 jsonschema.validate(
                     json.loads(ea_report.to_json()), schema)
                 ea_report_list.append(ea_report)
 
         inst.__dict__['_ea_report_list'] = ea_report_list
         inst.__dict__['_ea_config_list'] = ea_config_list
 
-        categorical_features = []
+        feature_metadata = rai_insights._feature_metadata
+        categorical_features = feature_metadata.categorical_features
         inst.__dict__['_categorical_features'] = categorical_features
         target_column = rai_insights.target_column
         true_y = rai_insights._ext_test_df[target_column]
         if isinstance(target_column, list):
             dropped_cols = target_column
         else:
             dropped_cols = [target_column]
@@ -271,16 +280,17 @@
             index_dataset.drop(columns=target_column, inplace=True)
             index_dataset[LABELS] = labels
             target_column = LABELS
             is_multilabel = True
             true_y = index_dataset[target_column]
         inst.__dict__['_true_y'] = true_y
         inst.__dict__['_task_type'] = rai_insights.task_type
+        text_column = rai_insights._text_column
         index_predictor = ErrorAnalysisManager._create_index_predictor(
-            wrapped_model, index_dataset, target_column, is_multilabel,
-            rai_insights.task_type, index_classes)
+            wrapped_model, index_dataset, target_column, text_column,
+            is_multilabel, rai_insights.task_type, index_classes)
         inst.__dict__['_analyzer'] = ModelAnalyzer(index_predictor,
                                                    dataset,
                                                    true_y,
                                                    feature_names,
                                                    categorical_features)
         return inst
```

### Comparing `responsibleai_text-0.1.2/responsibleai_text/managers/explainer_manager.py` & `responsibleai_text-0.1.3/responsibleai_text/managers/explainer_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.2/responsibleai_text/rai_text_insights/rai_text_insights.py` & `responsibleai_text-0.1.3/responsibleai_text/rai_text_insights/rai_text_insights.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
 """Defines the RAITextInsights class."""
 
 import json
+import logging
 import pickle
 import warnings
 from enum import Enum
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
 import numpy as np
@@ -16,48 +17,110 @@
 from ml_wrappers import wrap_model
 from raiutils.data_processing import convert_to_list, serialize_json_safe
 from raiutils.models import SKLearn, is_classifier
 from responsibleai._interfaces import Dataset, RAIInsightsData
 from responsibleai._internal.constants import (ManagerNames, Metadata,
                                                SerializationAttributes)
 from responsibleai.exceptions import UserConfigValidationException
+from responsibleai.feature_metadata import FeatureMetadata
 from responsibleai.rai_insights.rai_base_insights import RAIBaseInsights
 
 from responsibleai_text.common.constants import ModelTask
 from responsibleai_text.managers.error_analysis_manager import \
     ErrorAnalysisManager
 from responsibleai_text.managers.explainer_manager import ExplainerManager
-from responsibleai_text.utils.feature_extractors import extract_features
+from responsibleai_text.utils.feature_extractors import (extract_features,
+                                                         get_text_columns)
+
+module_logger = logging.getLogger(__name__)
+module_logger.setLevel(logging.INFO)
+
+try:
+    import evaluate
+except ImportError:
+    module_logger.debug(
+        'Could not import evaluate, required if using a QA model')
 
 _PREDICTIONS = 'predictions'
 _PREDICT_OUTPUT = 'predict_output'
 _TEST = 'test'
 _TARGET_COLUMN = 'target_column'
 _TASK_TYPE = 'task_type'
 _CLASSES = 'classes'
 _META_JSON = Metadata.META_JSON
 _JSON_EXTENSION = '.json'
 _PREDICT = 'predict'
 _PREDICT_PROBA = 'predict_proba'
 _EXT_TEST = '_ext_test'
 _EXT_FEATURES = '_ext_features'
+_FEATURE_METADATA = Metadata.FEATURE_METADATA
+_IDENTITY_FEATURE_NAME = 'identity_feature_name'
+_DATETIME_FEATURES = 'datetime_features'
+_TIME_SERIES_ID_FEATURES = 'time_series_id_features'
+_CATEGORICAL_FEATURES = 'categorical_features'
+_DROPPED_FEATURES = 'dropped_features'
+_QUESTION_TYPE = 'question_type'
+_TEXT_COLUMN = '_text_column'
+
+
+def _feature_metadata_from_dict(feature_meta_dict):
+    """Create a FeatureMetadata from a dictionary.
+
+    :param feature_meta_dict: The dictionary to create the FeatureMetadata
+        from.
+    :type feature_meta_dict: dict
+    :return: The FeatureMetadata created from the dictionary.
+    :rtype: FeatureMetadata
+    """
+    return FeatureMetadata(
+        identity_feature_name=feature_meta_dict[_IDENTITY_FEATURE_NAME],
+        datetime_features=feature_meta_dict[_DATETIME_FEATURES],
+        time_series_id_features=feature_meta_dict[_TIME_SERIES_ID_FEATURES],
+        categorical_features=feature_meta_dict[_CATEGORICAL_FEATURES],
+        dropped_features=feature_meta_dict[_DROPPED_FEATURES])
+
+
+def _add_extra_metadata_features(task_type, feature_metadata):
+    """Add extra metadata features for the given task type.
+
+    For question answering task, adds the question type feature.
+
+    :param task_type: The task type.
+    :type task_type: str
+    :param feature_metadata: The feature metadata.
+    :type feature_metadata: FeatureMetadata
+    :return: The feature metadata with extra metadata features added.
+    :rtype: FeatureMetadata
+    """
+    is_qa = task_type == ModelTask.QUESTION_ANSWERING
+    categorical_features = feature_metadata.categorical_features
+    is_cat_empty = categorical_features is None
+    if is_qa and (is_cat_empty or _QUESTION_TYPE not in categorical_features):
+        feature_metadata = _feature_metadata_from_dict(
+            feature_metadata.to_dict().copy())
+        if is_cat_empty:
+            feature_metadata.categorical_features = []
+        feature_metadata.categorical_features.append(_QUESTION_TYPE)
+    return feature_metadata
 
 
 class RAITextInsights(RAIBaseInsights):
     """Defines the top-level RAITextInsights API.
 
     Use RAITextInsights to assess text machine learning models in a
     single API.
     """
 
     def __init__(self, model: Any, test: pd.DataFrame,
                  target_column: str, task_type: str,
                  classes: Optional[np.ndarray] = None,
                  serializer: Optional[Any] = None,
-                 maximum_rows_for_test: int = 5000):
+                 maximum_rows_for_test: int = 5000,
+                 feature_metadata: Optional[FeatureMetadata] = None,
+                 text_column: Optional[Union[str, List]] = None):
         """Creates an RAITextInsights object.
 
         :param model: The model to compute RAI insights for.
             A model that implements sklearn.predict or sklearn.predict_proba
             or function that accepts a 2d ndarray.
         :type model: object
         :param test: The test dataset including the label column.
@@ -74,34 +137,49 @@
             The save method writes the model to file given a parent directory.
             The load method returns the deserialized model from the same
             parent directory.
         :type serializer: object
         :param maximum_rows_for_test: Limit on size of test data
             (for performance reasons)
         :type maximum_rows_for_test: int
+        :param feature_metadata: Feature metadata for the dataset
+            to identify different kinds of features.
+        :type feature_metadata: Optional[FeatureMetadata]
+        :param text_column: The name of the optional text column(s).
+            If not provided, and there is additional feature metadata, then
+            an exception will be raised.
+        :type text_column: str or list[str]
         """
         # drop index as this can cause issues later like when copying
         # target column below from test dataset to _ext_test_df
         test = test.reset_index(drop=True)
+        if feature_metadata is None:
+            # initialize to avoid having to keep checking if it is None
+            feature_metadata = FeatureMetadata()
+        feature_metadata = _add_extra_metadata_features(
+            task_type, feature_metadata)
+        self._text_column = text_column
+        self._feature_metadata = feature_metadata
         self._wrapped_model = wrap_model(model, test, task_type)
         self._validate_rai_insights_input_parameters(
             model=self._wrapped_model, test=test,
             target_column=target_column, task_type=task_type,
             classes=classes,
             serializer=serializer,
-            maximum_rows_for_test=maximum_rows_for_test)
+            maximum_rows_for_test=maximum_rows_for_test,
+            text_column=self._text_column)
         self._classes = RAITextInsights._get_classes(
             task_type=task_type,
             test=test,
             target_column=target_column,
             classes=classes
         )
-        ext_test, ext_features = extract_features(test,
-                                                  target_column,
-                                                  task_type)
+        ext_test, ext_features = extract_features(
+            test, target_column, task_type,
+            self._feature_metadata.dropped_features)
         self._ext_test = ext_test
         self._ext_features = ext_features
         self._ext_test_df = pd.DataFrame(ext_test, columns=ext_features)
         self._ext_test_df[target_column] = test[target_column]
         self.predict_output = None
 
         super(RAITextInsights, self).__init__(
@@ -117,15 +195,16 @@
         self._explainer_manager = ExplainerManager(
             self.model, self.test,
             self.target_column,
             self.task_type,
             self._classes)
         self._error_analysis_manager = ErrorAnalysisManager(
             self._wrapped_model, self.test, self._ext_test_df,
-            self.target_column, self.task_type, self._classes)
+            self.target_column, self._text_column, self.task_type,
+            self._classes, self._feature_metadata.categorical_features)
         self._managers = [self._explainer_manager,
                           self._error_analysis_manager]
 
     @staticmethod
     def _get_classes(task_type, test, target_column, classes):
         if task_type == ModelTask.TEXT_CLASSIFICATION:
             if classes is None:
@@ -160,33 +239,40 @@
         try:
             pickle.dumps(serializer)
         except Exception:
             raise UserConfigValidationException(
                 'The serializer should be serializable via pickle')
 
     def _validate_model(self, model: Any, test: pd.DataFrame,
-                        target_column: Union[str, List], task_type: str):
+                        target_column: Union[str, List], task_type: str,
+                        text_column: Optional[Union[str, List]]):
         """Validate the model.
 
         :param model: The model to validate.
         :type model: object
         :param test: The test dataset including the label column.
         :type test: pandas.DataFrame
         :param target_column: The name of the label column or list of columns.
             This is a list of columns for multilabel models.
         :type target_column: str or list[str]
         :param task_type: The task to run, can be `classification` or
             `regression`.
         :type task_type: str
+        :param text_column: The name of the optional text column(s).
+            If not provided, and there is additional feature metadata, then
+            an exception will be raised.
+        :type text_column: str or list[str]
         """
         if not isinstance(target_column, list):
             target_column = [target_column]
         # Pick one row from test data
         small_test_data = test.iloc[0:1].drop(
-            target_column, axis=1).iloc[0]
+            target_column, axis=1)
+        small_test_data = get_text_columns(small_test_data, text_column)
+        small_test_data = small_test_data.iloc[0]
         if task_type != ModelTask.QUESTION_ANSWERING:
             small_test_data = small_test_data.tolist()
         # Call the model
         try:
             model.predict(small_test_data)
         except Exception:
             raise UserConfigValidationException(
@@ -195,15 +281,16 @@
             )
 
     def _validate_rai_insights_input_parameters(
             self, model: Any, test: pd.DataFrame,
             target_column: Union[str, List], task_type: str,
             classes: np.ndarray,
             serializer,
-            maximum_rows_for_test: int):
+            maximum_rows_for_test: int,
+            text_column: Optional[Union[str, List]]):
         """Validate the inputs for the RAITextInsights constructor.
 
         :param model: The model to compute RAI insights for.
             A model that implements sklearn.predict or sklearn.predict_proba
             or function that accepts a 2d ndarray.
         :type model: object
         :param test: The test dataset including the label column.
@@ -278,24 +365,38 @@
         else:
             if target_column not in list(test.columns):
                 raise UserConfigValidationException(
                     'Target name {0} not present in test data'.format(
                         target_column)
                 )
 
+        if text_column:
+            if task_type == ModelTask.QUESTION_ANSWERING.value:
+                if not isinstance(text_column, list):
+                    raise UserConfigValidationException(
+                        'The text_column should be a list for question answering')
+                text_columns_set = set(text_column)
+                if not text_columns_set.issubset(set(test.columns)):
+                    raise UserConfigValidationException(
+                        'The list of text_column(s) should be in test data')
+            else:
+                if text_column not in test.columns:
+                    raise UserConfigValidationException(
+                        'The text_column should be in test data')
+
         if classes is not None and task_type == ModelTask.TEXT_CLASSIFICATION:
             if len(set(test[target_column].unique()) -
                     set(classes)) != 0:
                 raise UserConfigValidationException(
                     'The test labels are not a subset of the '
                     'distinct values in target (test data)')
 
         if model is not None:
             self._validate_model(model, test, target_column,
-                                 task_type)
+                                 task_type, text_column)
 
     def get_filtered_test_data(self, filters, composite_filters,
                                include_original_columns_only=False,
                                use_entire_test_data=False):
         """Get the filtered test data based on cohort filters.
 
         :param filters: The filters to apply.
@@ -392,33 +493,35 @@
         self._save_list_data(ext_path, self._ext_test)
         self._save_list_data(ext_features_path, self._ext_features)
 
     def _save_list_data(self, data_path, data):
         with open(data_path, 'w') as file:
             json.dump(data, file, default=serialize_json_safe)
 
-    def _get_test_without_target(self, is_classification_task):
-        """Get the test data without the target column.
+    def _get_test_text_data(self, is_classification_task):
+        """Get the test data without the target and metadata columns.
 
         :param is_classification_task: Whether the task is a
             classification task.
         :type is_classification_task: bool
-        :return: The test data without the target column.
-        :rtype: pandas.DataFrame
+        :return: The test data without the target and metadata columns.
+        :rtype: pandas.DataFrame or list[str]
         """
         if is_classification_task:
             target_column = self.target_column
             if not isinstance(target_column, list):
                 target_column = [target_column]
-            dataset = self.test.drop(
-                target_column, axis=1).iloc[:, 0].tolist()
+            dataset = self.test.drop(target_column, axis=1)
         elif self.task_type == ModelTask.QUESTION_ANSWERING:
             dataset = self.test.drop([self.target_column], axis=1)
         else:
             raise ValueError("Unknown task type: {}".format(self.task_type))
+        dataset = get_text_columns(dataset, self._text_column)
+        if is_classification_task:
+            dataset = dataset.iloc[:, 0].tolist()
         return dataset
 
     @property
     def _is_classification_task(self):
         """Whether the task is a classification task.
 
         :return: Whether the task is a classification task.
@@ -430,19 +533,22 @@
 
     def _get_dataset(self):
         dashboard_dataset = Dataset()
         tasktype = self.task_type
         if isinstance(tasktype, Enum):
             tasktype = tasktype.value
         dashboard_dataset.task_type = tasktype
-        dashboard_dataset.categorical_features = []
+        categorical_features = self._feature_metadata.categorical_features
+        if categorical_features is None:
+            categorical_features = []
+        dashboard_dataset.categorical_features = categorical_features
         dashboard_dataset.class_names = convert_to_list(
             self._classes)
         is_classification_task = self._is_classification_task
-        dataset = self._get_test_without_target(is_classification_task)
+        dataset = self._get_test_text_data(is_classification_task)
 
         predicted_y = None
         if dataset is not None and self._wrapped_model is not None:
             try:
                 predicted_y = self._wrapped_model.predict(dataset)
             except Exception as ex:
                 msg = ("Model does not support predict method for given "
@@ -522,15 +628,15 @@
         """
         prediction_output_path = Path(path) / _PREDICTIONS
         prediction_output_path.mkdir(parents=True, exist_ok=True)
 
         if self.model is None:
             return
         is_classification_task = self._is_classification_task
-        test_without_target_column = self._get_test_without_target(
+        test_without_target_column = self._get_test_text_data(
             is_classification_task)
         predict_output = self._wrapped_model.predict(
             test_without_target_column)
         self._write_to_file(
             prediction_output_path / (_PREDICT + _JSON_EXTENSION),
             json.dumps(predict_output.tolist()))
 
@@ -546,18 +652,21 @@
            task type and the classes (if any).
 
         :param path: The directory path to save the RAITextInsights to.
         :type path: str
         """
         top_dir = Path(path)
         classes = convert_to_list(self._classes)
+        feature_metadata_dict = self._feature_metadata.to_dict()
         meta = {
             _TARGET_COLUMN: self.target_column,
             _TASK_TYPE: self.task_type,
-            _CLASSES: classes
+            _CLASSES: classes,
+            _FEATURE_METADATA: feature_metadata_dict,
+            _TEXT_COLUMN: self._text_column
         }
         with open(top_dir / _META_JSON, 'w') as file:
             json.dump(meta, file)
 
     @staticmethod
     def _load_metadata(inst, path):
         """Load the metadata.
@@ -570,22 +679,36 @@
         top_dir = Path(path)
         with open(top_dir / _META_JSON, 'r') as meta_file:
             meta = meta_file.read()
         meta = json.loads(meta)
         inst.__dict__[_TARGET_COLUMN] = meta[_TARGET_COLUMN]
         inst.__dict__[_TASK_TYPE] = meta[_TASK_TYPE]
         inst.__dict__[_PREDICT_OUTPUT] = None
+        text_column = None
+        if _TEXT_COLUMN in meta:
+            text_column = meta[_TEXT_COLUMN]
+        inst.__dict__[_TEXT_COLUMN] = text_column
         classes = meta[_CLASSES]
 
         inst.__dict__['_' + _CLASSES] = RAITextInsights._get_classes(
             task_type=meta[_TASK_TYPE],
             test=inst.__dict__[_TEST],
             target_column=meta[_TARGET_COLUMN],
             classes=classes
         )
+
+        if (Metadata.FEATURE_METADATA not in meta or
+                meta[Metadata.FEATURE_METADATA] is None):
+            inst.__dict__['_' + Metadata.FEATURE_METADATA] = FeatureMetadata()
+        else:
+            feature_metadata_dict = meta[Metadata.FEATURE_METADATA]
+            feature_metadata = _feature_metadata_from_dict(
+                feature_metadata_dict)
+            inst.__dict__['_' + Metadata.FEATURE_METADATA] = feature_metadata
+
         # load the extracted features as part of metadata
         RAITextInsights._load_ext_data(inst, path)
 
     @staticmethod
     def _load_ext_data(inst, path):
         """Load the extracted features data.
 
@@ -616,19 +739,91 @@
         :type path: str
         :return: The RAITextInsights object after loading.
         :rtype: RAITextInsights
         """
         # create the RAITextInsights without any properties using the __new__
         # function, similar to pickle
         inst = RAITextInsights.__new__(RAITextInsights)
-        inst.categorical_features = []
 
         manager_map = {
             ManagerNames.EXPLAINER: ExplainerManager,
             ManagerNames.ERROR_ANALYSIS: ErrorAnalysisManager,
         }
 
         # load current state
         RAIBaseInsights._load(path, inst, manager_map,
                               RAITextInsights._load_metadata)
         inst._wrapped_model = wrap_model(inst.model, inst.test, inst.task_type)
         return inst
+
+    def normalize_text(self, s):
+        """Removing articles and punctuation, and standardizing whitespace are all typical text processing steps."""
+        import re
+        import string
+
+        def remove_articles(text):
+            regex = re.compile(r"\b(a|an|the)\b", re.UNICODE)
+            return re.sub(regex, " ", text)
+
+        def white_space_fix(text):
+            return " ".join(text.split())
+
+        def remove_punc(text):
+            exclude = set(string.punctuation)
+            return "".join(ch for ch in text if ch not in exclude)
+
+        def lower(text):
+            return text.lower()
+
+        return white_space_fix(remove_articles(remove_punc(lower(s))))
+
+    def compute_f1(self, prediction, truth):
+        pred_tokens = self.normalize_text(prediction).split()
+        truth_tokens = self.normalize_text(truth).split()
+
+        # if either the prediction or the truth is no-answer then f1 = 1 if they agree, 0 otherwise
+        if len(pred_tokens) == 0 or len(truth_tokens) == 0:
+            return int(pred_tokens == truth_tokens)
+
+        common_tokens = set(pred_tokens) & set(truth_tokens)
+
+        # if there are no common tokens then f1 = 0
+        if len(common_tokens) == 0:
+            return 0
+
+        prec = len(common_tokens) / len(pred_tokens)
+        rec = len(common_tokens) / len(truth_tokens)
+
+        return 2 * (prec * rec) / (prec + rec)
+
+    def compute_question_answering_metrics(self, selection_indexes):
+        dashboard_dataset = self.get_data().dataset
+        true_y = dashboard_dataset.true_y
+        predicted_y = dashboard_dataset.predicted_y
+        all_cohort_metrics = []
+        for cohort_indices in selection_indexes:
+            true_y_cohort = [true_y[cohort_index] for cohort_index
+                             in cohort_indices]
+            predicted_y_cohort = [predicted_y[cohort_index] for cohort_index
+                                  in cohort_indices]
+            f1_score = []
+            for cohort_index in cohort_indices:
+                f1_score.append(self.compute_f1(predicted_y[cohort_index], true_y[cohort_index]))
+            try:
+                exact_match = evaluate.load('exact_match')
+                exact_match_results = exact_match.compute(predictions=predicted_y_cohort, references=true_y_cohort)
+                rouge = evaluate.load('rouge')
+                rouge_results = rouge.compute(predictions=predicted_y_cohort, references=true_y_cohort)
+                bleu = evaluate.load('bleu')
+                bleu_results = bleu.compute(predictions=predicted_y_cohort, references=true_y_cohort)
+                meteor = evaluate.load('meteor')
+                meteor_results = meteor.compute(predictions=predicted_y_cohort, references=true_y_cohort)
+                bert_score = evaluate.load('bertscore')
+                bert_score_results = bert_score.compute(predictions=predicted_y_cohort, references=true_y_cohort,
+                                                        model_type="distilbert-base-uncased")
+                bert_f1_score = np.mean(bert_score_results['f1'])
+                all_cohort_metrics.append([exact_match_results['exact_match'], np.mean(f1_score),
+                                           meteor_results['meteor'], bleu_results['bleu'], bert_f1_score,
+                                           rouge_results['rougeL']])
+            except ValueError:
+                all_cohort_metrics.append([0, 0, 0, 0, 0, 0])
+        return all_cohort_metrics
```

### Comparing `responsibleai_text-0.1.2/responsibleai_text/utils/question_answering.py` & `responsibleai_text-0.1.3/responsibleai_text/utils/question_answering.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.2/responsibleai_text.egg-info/PKG-INFO` & `responsibleai_text-0.1.3/responsibleai_text.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: responsibleai-text
-Version: 0.1.2
+Version: 0.1.3
 Summary: SDK API to assess text Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: qa
 
 # Responsible AI Text SDK for Python
 
 ### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
 
 The Responsible AI Text sdk enables users to analyze their machine learning models for text data in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
 
@@ -26,8 +27,8 @@
 - `explainer.add()` explains the model
 
 ### Supported scenarios, models and datasets
 
 The Responsible AI Text SDK supports multiclass classification and question answering models on text data currently.
 
 The open source code for the visualization dashboard can be found here:
-https://github.com/microsoft/responsible-ai-widgets
+https://github.com/microsoft/responsible-ai-toolbox
```

### Comparing `responsibleai_text-0.1.2/responsibleai_text.egg-info/SOURCES.txt` & `responsibleai_text-0.1.3/responsibleai_text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.2/setup.py` & `responsibleai_text-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,27 +14,35 @@
 # Fetch ReadMe
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 # Use requirements.txt to set the install_requires
 with open('requirements.txt') as f:
     install_requires = [line.strip() for line in f]
-
+EXTRAS = {
+    "qa": [
+        'evaluate',
+        'bert_score',
+        'nltk',
+        'rouge_score'
+    ]
+}
 setuptools.setup(
     name=name,  # noqa: F821
     version=version,  # noqa: F821
     author="Roman Lutz, Ilya Matiach, Ke Xu",
     author_email="raiwidgets-maintain@microsoft.com",
     description="SDK API to assess text "
                 "Machine Learning models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/microsoft/responsible-ai-toolbox",
     packages=setuptools.find_packages(),
     python_requires='>=3.6',
+    extras_require=EXTRAS,
     install_requires=install_requires,
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
```

### Comparing `responsibleai_text-0.1.2/tests/test_feature_extractors.py` & `responsibleai_text-0.1.3/tests/test_feature_extractors.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.2/tests/test_rai_text_insights.py` & `responsibleai_text-0.1.3/tests/test_rai_text_insights.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
-from common_text_utils import (ANSWERS, COVID19_EVENTS_LABELS, EMOTION,
+from common_text_utils import (ANSWERS, BLBOOKS_LABEL, COVID19_EVENTS_LABELS,
+                               EMOTION, create_blbooks_pipeline,
                                create_multilabel_pipeline,
                                create_question_answering_pipeline,
                                create_text_classification_pipeline,
+                               load_blbooks_genre_dataset,
                                load_covid19_emergency_event_dataset,
                                load_emotion_dataset, load_squad_dataset)
 from rai_text_insights_validator import validate_rai_text_insights
+from responsibleai.feature_metadata import FeatureMetadata
 
 from responsibleai_text import ModelTask, RAITextInsights
 
 
 class TestRAITextInsights(object):
 
     def test_rai_insights_emotion_classification(self):
@@ -22,33 +25,67 @@
 
     def test_rai_insights_question_answering(self):
         data = load_squad_dataset()
         pred = create_question_answering_pipeline()
         task_type = ModelTask.QUESTION_ANSWERING
         run_rai_insights(pred, data, data[:5], ANSWERS, task_type)
 
+    def test_rai_insights_question_answering_metadata(self):
+        data = load_squad_dataset(with_metadata=True)
+        pred = create_question_answering_pipeline()
+        task_type = ModelTask.QUESTION_ANSWERING
+        feature_metadata = FeatureMetadata()
+        feature_metadata.categorical_features = ['title']
+        run_rai_insights(pred, data, data[:5], ANSWERS, task_type,
+                         feature_metadata)
+
     def test_rai_insights_multilabel(self):
         data = load_covid19_emergency_event_dataset()
         pred = create_multilabel_pipeline()
         task_type = ModelTask.MULTILABEL_TEXT_CLASSIFICATION
         labels = COVID19_EVENTS_LABELS
         run_rai_insights(pred, data, data[:5], labels, task_type)
 
+    def test_rai_insights_multilabel_metadata(self):
+        data = load_covid19_emergency_event_dataset(with_metadata=True)
+        pred = create_multilabel_pipeline()
+        task_type = ModelTask.MULTILABEL_TEXT_CLASSIFICATION
+        labels = COVID19_EVENTS_LABELS
+        feature_metadata = FeatureMetadata()
+        feature_metadata.categorical_features = ['language', 'country']
+        run_rai_insights(pred, data, data[:5], labels, task_type,
+                         feature_metadata)
+
+    def test_rai_insights_blbooks_genre_metadata(self):
+        data = load_blbooks_genre_dataset()
+        pred = create_blbooks_pipeline()
+        task_type = ModelTask.TEXT_CLASSIFICATION
+        feature_metadata = FeatureMetadata()
+        feature_metadata.categorical_features = ['annotator_country',
+                                                 'annotator_place_pub',
+                                                 'annotated']
+        run_rai_insights(pred, data, data[:5], BLBOOKS_LABEL, task_type,
+                         feature_metadata, text_column='text')
+
 
 def run_rai_insights(model, train_data, test_data,
-                     target_column, task_type):
+                     target_column, task_type,
+                     feature_metadata=None,
+                     text_column=None):
     if task_type == ModelTask.TEXT_CLASSIFICATION:
         classes = train_data[target_column].unique()
         classes.sort()
     else:
         classes = None
     rai_insights = RAITextInsights(model, test_data,
                                    target_column,
                                    task_type=task_type,
-                                   classes=classes)
+                                   classes=classes,
+                                   feature_metadata=feature_metadata,
+                                   text_column=text_column)
     rai_insights.explainer.add()
     if task_type != ModelTask.QUESTION_ANSWERING:
         rai_insights.error_analysis.add()
     rai_insights.compute()
     rai_insights.get_data()
     # Validate
     validate_rai_text_insights(
```

### Comparing `responsibleai_text-0.1.2/tests/test_rai_text_insights_save_and_load_scenarios.py` & `responsibleai_text-0.1.3/tests/test_rai_text_insights_save_and_load_scenarios.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,19 +3,24 @@
 
 import os
 import shutil
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import pytest
-from common_text_utils import (EMOTION, TextClassificationPipelineSerializer,
+from common_text_utils import (COVID19_EVENTS_LABELS, EMOTION,
+                               MultilabelTextClassificationSerializer,
+                               TextClassificationPipelineSerializer,
+                               create_multilabel_pipeline,
                                create_text_classification_pipeline,
+                               load_covid19_emergency_event_dataset,
                                load_emotion_dataset)
 from rai_text_insights_validator import validate_rai_text_insights
 from responsibleai._internal.constants import ManagerNames
+from responsibleai.feature_metadata import FeatureMetadata
 
 from responsibleai_text import ModelTask, RAITextInsights
 
 
 class TestRAITextInsightsSaveAndLoadScenarios(object):
 
     def test_rai_insights_empty_save_load_save(self):
@@ -168,7 +173,55 @@
             # Validate
             validate_rai_text_insights(
                 rai_2, classes, test,
                 EMOTION, ModelTask.TEXT_CLASSIFICATION)
 
             # Save again
             rai_2.save(save_2)
+
+    @pytest.mark.skip(reason="Test takes too long to run. Enable if needed.")
+    @pytest.mark.parametrize('manager_type', [ManagerNames.EXPLAINER,
+                                              ManagerNames.ERROR_ANALYSIS])
+    def test_rai_insights_metadata_save_load_save(self, manager_type):
+        data = load_covid19_emergency_event_dataset(with_metadata=True)
+        pred = create_multilabel_pipeline()
+        task_type = ModelTask.MULTILABEL_TEXT_CLASSIFICATION
+        labels = COVID19_EVENTS_LABELS
+        feature_metadata = FeatureMetadata()
+        feature_metadata.categorical_features = ['language', 'country']
+        test = data[:3]
+        classes = None
+
+        rai_insights = RAITextInsights(
+            pred, test, labels,
+            task_type=task_type,
+            serializer=MultilabelTextClassificationSerializer(),
+            feature_metadata=feature_metadata)
+
+        # Call a single manager
+        if manager_type == ManagerNames.EXPLAINER:
+            rai_insights.explainer.add()
+        elif manager_type == ManagerNames.ERROR_ANALYSIS:
+            rai_insights.error_analysis.add()
+        else:
+            raise ValueError(
+                "Bad manager_type: {0}".format(manager_type))
+
+        rai_insights.compute()
+
+        with TemporaryDirectory() as tmpdir:
+            save_1 = Path(tmpdir) / "first_save"
+            save_2 = Path(tmpdir) / "second_save"
+
+            # Save it
+            rai_insights.save(save_1)
+
+            # Load
+            rai_2 = RAITextInsights.load(save_1)
+
+            # Validate
+            validate_rai_text_insights(
+                rai_2, classes, test,
+                labels, ModelTask.MULTILABEL_TEXT_CLASSIFICATION)
+
+            # Save again
+            rai_2.save(save_2)
```

