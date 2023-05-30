# Comparing `tmp/lazylearn-0.0.3.tar.gz` & `tmp/lazylearn-0.0.4.tar.gz`

## Comparing `lazylearn-0.0.3.tar` & `lazylearn-0.0.4.tar`

### file list

```diff
@@ -1,52 +1,57 @@
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 lazylearn-0.0.3/Pipfile
--rw-r--r--   0        0        0    75211 2020-02-02 00:00:00.000000 lazylearn-0.0.3/Pipfile.lock
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 lazylearn-0.0.3/.github/workflows/verify.yaml
--rw-r--r--   0        0        0    59514 2020-02-02 00:00:00.000000 lazylearn-0.0.3/doc/logo/grayscale_transparent.png
--rw-r--r--   0        0        0    62685 2020-02-02 00:00:00.000000 lazylearn-0.0.3/doc/logo/original.png
--rw-r--r--   0        0        0    66560 2020-02-02 00:00:00.000000 lazylearn-0.0.3/doc/logo/transparent.png
--rw-r--r--   0        0        0    71882 2020-02-02 00:00:00.000000 lazylearn-0.0.3/doc/logo/transparent_small.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/__init__.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/lazylearn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/errors/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/errors/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/__init__.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline_steps/__init__.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline_steps/data_parser_step.py
--rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline_steps/interpreter_step.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline_steps/summary_stats_step.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/utils/__init__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/utils/csv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/model_selection/__init__.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/model_selection/splitters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/models/__init__.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/models/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/pipeline/__init__.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/pipeline/pipeline.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/encoding/__init__.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/encoding/encoders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/imputation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/time/__init__.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/time/date_processor.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/time/duration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/models/randomforest/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/models/randomforest/randomforest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/models/randomforest/random_forest_steps/__init__.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/models/randomforest/random_forest_steps/regressor_step.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/models/xgboost/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/strategies/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/strategies/strategy_builder.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/test/test_mock.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/test/ingestion/ingestion_pipeline_steps/test_data_parser_step.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/test/ingestion/ingestion_pipeline_steps/test_interpreter_step.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/test/ingestion/ingestion_pipeline_steps/test_summary_stats_step.py
--rwxr-xr-x   0        0        0      743 2020-02-02 00:00:00.000000 lazylearn-0.0.3/shell/check.sh
--rwxr-xr-x   0        0        0      382 2020-02-02 00:00:00.000000 lazylearn-0.0.3/shell/tidy.sh
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 lazylearn-0.0.3/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 lazylearn-0.0.3/LICENSE
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 lazylearn-0.0.3/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 lazylearn-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 lazylearn-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 lazylearn-0.0.4/Pipfile
+-rw-r--r--   0        0        0    75211 2020-02-02 00:00:00.000000 lazylearn-0.0.4/Pipfile.lock
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 lazylearn-0.0.4/.github/workflows/verify.yaml
+-rw-r--r--   0        0        0    59514 2020-02-02 00:00:00.000000 lazylearn-0.0.4/doc/logo/grayscale_transparent.png
+-rw-r--r--   0        0        0    62685 2020-02-02 00:00:00.000000 lazylearn-0.0.4/doc/logo/original.png
+-rw-r--r--   0        0        0    66560 2020-02-02 00:00:00.000000 lazylearn-0.0.4/doc/logo/transparent.png
+-rw-r--r--   0        0        0    71882 2020-02-02 00:00:00.000000 lazylearn-0.0.4/doc/logo/transparent_small.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/__init__.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/lazylearn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/errors/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/errors/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/ingestion/__init__.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/ingestion/ingestion_pipeline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/ingestion/ingestion_pipeline_steps/__init__.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/ingestion/ingestion_pipeline_steps/data_parser_step.py
+-rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/ingestion/ingestion_pipeline_steps/interpreter_step.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/ingestion/ingestion_pipeline_steps/summary_stats_step.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/ingestion/utils/__init__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/ingestion/utils/csv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/model_selection/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/model_selection/splitters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/models/__init__.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/models/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/pipeline/__init__.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/pipeline/pipeline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/preprocessing/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/preprocessing/encoding/__init__.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/preprocessing/encoding/encoders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/preprocessing/imputation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/preprocessing/time/__init__.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/preprocessing/time/date_processor.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/preprocessing/time/duration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/regression/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/regression/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/regression/models/randomforest/__init__.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/regression/models/randomforest/randomforest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/regression/models/randomforest/random_forest_steps/__init__.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/regression/models/randomforest/random_forest_steps/regressor_step.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/regression/models/xgboost/__init__.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/regression/models/xgboost/xgb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/regression/models/xgboost/xgb_regressor_steps/__init__.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/regression/models/xgboost/xgb_regressor_steps/hpo_step.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/regression/models/xgboost/xgb_regressor_steps/regressor_step.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/strategies/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/strategies/strategy_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/strategies/strategy_steps/__init__.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/lazylearn/strategies/strategy_steps/evaluation.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/test/ingestion/ingestion_pipeline_steps/test_data_parser_step.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/test/ingestion/ingestion_pipeline_steps/test_interpreter_step.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 lazylearn-0.0.4/python/src/test/ingestion/ingestion_pipeline_steps/test_summary_stats_step.py
+-rwxr-xr-x   0        0        0      743 2020-02-02 00:00:00.000000 lazylearn-0.0.4/shell/check.sh
+-rwxr-xr-x   0        0        0      382 2020-02-02 00:00:00.000000 lazylearn-0.0.4/shell/tidy.sh
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 lazylearn-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 lazylearn-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 lazylearn-0.0.4/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 lazylearn-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 lazylearn-0.0.4/PKG-INFO
```

### Comparing `lazylearn-0.0.3/Pipfile.lock` & `lazylearn-0.0.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/.github/workflows/verify.yaml` & `lazylearn-0.0.4/.github/workflows/verify.yaml`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/doc/logo/grayscale_transparent.png` & `lazylearn-0.0.4/doc/logo/grayscale_transparent.png`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/doc/logo/original.png` & `lazylearn-0.0.4/doc/logo/original.png`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/doc/logo/transparent.png` & `lazylearn-0.0.4/doc/logo/transparent.png`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/doc/logo/transparent_small.png` & `lazylearn-0.0.4/doc/logo/transparent_small.png`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline.py` & `lazylearn-0.0.4/python/src/lazylearn/ingestion/ingestion_pipeline.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline_steps/data_parser_step.py` & `lazylearn-0.0.4/python/src/lazylearn/ingestion/ingestion_pipeline_steps/data_parser_step.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline_steps/interpreter_step.py` & `lazylearn-0.0.4/python/src/lazylearn/ingestion/ingestion_pipeline_steps/interpreter_step.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline_steps/summary_stats_step.py` & `lazylearn-0.0.4/python/src/lazylearn/ingestion/ingestion_pipeline_steps/summary_stats_step.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/python/src/lazylearn/models/models.py` & `lazylearn-0.0.4/python/src/lazylearn/models/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,37 @@
+from typing import Dict
+
 from pandas import DataFrame
 
 
 class Dataset:
     def __init__(
         self,
         df: DataFrame,
         column_type_map: dict,
         summary_stats: dict,
         type_collections: dict,
     ):
         self.name = None
         self.description = None
-        self.df = df
+        self.df: DataFrame = df
         self.column_type_map = column_type_map
         self.summary_stats = summary_stats
         self.type_collections = type_collections
         self.partitions: dict = {}
 
     def save(self):
         raise NotImplementedError
 
 
 class Model:
-    def __init__(self):
-        self.name = None
+    def __init__(self, name: str, score: Dict[str, float], pipeline):
+        self.name = name
+        self.score = score
+        self.pipeline = pipeline
 
     def save(self, path: str):
         raise NotImplementedError
 
 
 class Project:
     def __init__(self):
```

### Comparing `lazylearn-0.0.3/python/src/lazylearn/pipeline/pipeline.py` & `lazylearn-0.0.4/python/src/lazylearn/pipeline/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,7 +70,8 @@
     def __init__(self):
         super().__init__()
         self.train_features_df: DataFrame = None
         self.train_targets: Series = None
         self.holdout_features_df: DataFrame = None
         self.holdout_targets: Series = None
         self.holdout_score: float = None
+        self.regressor = None
```

### Comparing `lazylearn-0.0.3/python/src/lazylearn/preprocessing/encoding/encoders.py` & `lazylearn-0.0.4/python/src/lazylearn/preprocessing/encoding/encoders.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/python/src/lazylearn/preprocessing/time/date_processor.py` & `lazylearn-0.0.4/python/src/lazylearn/preprocessing/time/date_processor.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/python/src/lazylearn/preprocessing/time/duration.py` & `lazylearn-0.0.4/python/src/lazylearn/preprocessing/time/duration.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/python/src/lazylearn/regression/models/randomforest/randomforest.py` & `lazylearn-0.0.4/python/src/lazylearn/regression/models/randomforest/randomforest.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from preprocessing.encoding.encoders import OrdinalConverter
 from regression.models.randomforest.random_forest_steps.regressor_step import (
     RandomForestRegressorStep,
 )
 
 
 class RandomForestRegressionRunner:
-    def __init__(self, target, dataset, random_state=42):
+    def __init__(self, target, dataset, random_state=None):
+        self.name = "RandomForestRegressor"
         self.target = target
         self.dataset: Dataset = dataset
         self.random_state = random_state
         self.pipeline = RegressionPipeline()
         self.pipeline.target = target
 
         self.pipeline.train_features_df = self.dataset.partitions[
@@ -27,14 +28,16 @@
         # preprocess numeric vars
         cat_vars = self.dataset.type_collections["categorical"]
         num_vars = self.dataset.type_collections["numeric"]
         self.pipeline.feature_list.extend(num_vars)
 
         self.pipeline.add(OrdinalConverter(cat_vars=cat_vars))
 
-        self.pipeline.add(RandomForestRegressorStep())
+        self.pipeline.add(
+            RandomForestRegressorStep(random_state=self.random_state)
+        )  # noqa
 
         self.pipeline.fit()
 
     def predict(self, features):
         self.pipeline.tmp_test = features
         return self.pipeline.predict()
```

### Comparing `lazylearn-0.0.3/python/src/lazylearn/regression/models/randomforest/random_forest_steps/regressor_step.py` & `lazylearn-0.0.4/python/src/lazylearn/regression/models/randomforest/random_forest_steps/regressor_step.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/python/src/test/ingestion/ingestion_pipeline_steps/test_interpreter_step.py` & `lazylearn-0.0.4/python/src/test/ingestion/ingestion_pipeline_steps/test_interpreter_step.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/python/src/test/ingestion/ingestion_pipeline_steps/test_summary_stats_step.py` & `lazylearn-0.0.4/python/src/test/ingestion/ingestion_pipeline_steps/test_summary_stats_step.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/shell/check.sh` & `lazylearn-0.0.4/shell/check.sh`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/.gitignore` & `lazylearn-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/LICENSE` & `lazylearn-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.3/README.md` & `lazylearn-0.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,49 @@
 
 <img width="500" src="doc/logo/transparent_small.png">
 
 **lazy-learn** is a high-level Python interface for automated machine learning (AutoML). While there are many AutoML libraries available each typically solves a niche area of the overall ML pipeline without providing a covering and approachable end-to-end system.
 
-The aim of lazy-learn is exactly that. Given a dataset, easy-learn will analyse types and distributions of attributes, preprocess, feature-engineer and ultimately train models to be used for further evaluation or inference. 
+The aim of lazy-learn is exactly that. Given a dataset, lazy-learn will analyse types and distributions of attributes, preprocess, feature-engineer and ultimately train models to be used for further evaluation or inference. 
 
 ## Upcoming features
 
 Current stable version is 0.0.3. The upcoming updates will support:
 - Abstract construction of model architectures
 - XGBoost, LightGBM, Adaboost and Catboost architectures
-- Time partitioning of datasets
-- Automated Hyperparameter Optimisation (HPO)
+- Time partitioning of datasets (Added in 0.0.4)
+- Automated Hyperparameter Optimisation (HPO) (Added in 0.0.4)
 - Text features
 - An interface to AutoGluon
 - Outlier detection and handling
 - Automated suggestions of performance metrics
 
 ## Usage
 
-Using lazy-learn revolves around the `LazyLearner` class. You can think of it as a kind of project, and it is the wrapper for any experiment within lazy-learn.
+Using lazy-learn revolves around the `LazyLearner` class. You can think of it as a kind of project, and it is the wrapper for any experiment within lazy-learn. You can consider a simple example with the California Housing dataset:
+
+```python
+from lazylearn import LazyLearner
+from sklearn.datasets import fetch_california_housing
+
+
+# get some data
+data = fetch_california_housing(as_frame=True)
+df = data["data"]
+df["MedHouseVal"] = data["target"]
+
+# instantiate and run the LazyLearner
+learner = LazyLearner()
+learner.create_project(data=df, target="MedHouseVal")
+learner.run_autopilot()
+
+# evaluate results
+print(learner.leaderboard())
+
+```
 
 ## Installation
 
 ### Dependencies
 
 lazy-learn requires:
 
@@ -35,8 +55,8 @@
 ```
 pip install lazy-learn
 ```
 
 ## Help and Support
 ### Documentation
 
-### Citation
+### Citation
```

### Comparing `lazylearn-0.0.3/pyproject.toml` & `lazylearn-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lazylearn"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Frederik P. Høngaard", email="mail@frederikhoengaard.com" },
 ]
 description = "lazy-learn is a high-level Python interface for automated machine learning (AutoML) for the lazy data scientist. While there are many AutoML libraries available each typically solves a niche area of the overall ML pipeline without providing a covering and approachable end-to-end system. lazy-learn aims at providing the most approachable and fastest access to building baseline models."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lazylearn-0.0.3/PKG-INFO` & `lazylearn-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazylearn
-Version: 0.0.3
+Version: 0.0.4
 Summary: lazy-learn is a high-level Python interface for automated machine learning (AutoML) for the lazy data scientist. While there are many AutoML libraries available each typically solves a niche area of the overall ML pipeline without providing a covering and approachable end-to-end system. lazy-learn aims at providing the most approachable and fastest access to building baseline models.
 Project-URL: Homepage, https://github.com/frederikhoengaard/lazy-learn
 Author-email: "Frederik P. Høngaard" <mail@frederikhoengaard.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -12,31 +12,51 @@
 Description-Content-Type: text/markdown
 
 
 <img width="500" src="doc/logo/transparent_small.png">
 
 **lazy-learn** is a high-level Python interface for automated machine learning (AutoML). While there are many AutoML libraries available each typically solves a niche area of the overall ML pipeline without providing a covering and approachable end-to-end system.
 
-The aim of lazy-learn is exactly that. Given a dataset, easy-learn will analyse types and distributions of attributes, preprocess, feature-engineer and ultimately train models to be used for further evaluation or inference. 
+The aim of lazy-learn is exactly that. Given a dataset, lazy-learn will analyse types and distributions of attributes, preprocess, feature-engineer and ultimately train models to be used for further evaluation or inference. 
 
 ## Upcoming features
 
 Current stable version is 0.0.3. The upcoming updates will support:
 - Abstract construction of model architectures
 - XGBoost, LightGBM, Adaboost and Catboost architectures
-- Time partitioning of datasets
-- Automated Hyperparameter Optimisation (HPO)
+- Time partitioning of datasets (Added in 0.0.4)
+- Automated Hyperparameter Optimisation (HPO) (Added in 0.0.4)
 - Text features
 - An interface to AutoGluon
 - Outlier detection and handling
 - Automated suggestions of performance metrics
 
 ## Usage
 
-Using lazy-learn revolves around the `LazyLearner` class. You can think of it as a kind of project, and it is the wrapper for any experiment within lazy-learn.
+Using lazy-learn revolves around the `LazyLearner` class. You can think of it as a kind of project, and it is the wrapper for any experiment within lazy-learn. You can consider a simple example with the California Housing dataset:
+
+```python
+from lazylearn import LazyLearner
+from sklearn.datasets import fetch_california_housing
+
+
+# get some data
+data = fetch_california_housing(as_frame=True)
+df = data["data"]
+df["MedHouseVal"] = data["target"]
+
+# instantiate and run the LazyLearner
+learner = LazyLearner()
+learner.create_project(data=df, target="MedHouseVal")
+learner.run_autopilot()
+
+# evaluate results
+print(learner.leaderboard())
+
+```
 
 ## Installation
 
 ### Dependencies
 
 lazy-learn requires:
 
@@ -48,8 +68,8 @@
 ```
 pip install lazy-learn
 ```
 
 ## Help and Support
 ### Documentation
 
-### Citation
+### Citation
```

