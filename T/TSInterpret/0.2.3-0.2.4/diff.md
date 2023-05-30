# Comparing `tmp/TSInterpret-0.2.3.tar.gz` & `tmp/TSInterpret-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSInterpret-0.2.3.tar", last modified: Mon Apr 24 12:44:13 2023, max compression
+gzip compressed data, was "TSInterpret-0.2.4.tar", last modified: Tue May 30 08:14:04 2023, max compression
```

## Comparing `TSInterpret-0.2.3.tar` & `TSInterpret-0.2.4.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.179923 TSInterpret-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.171923 TSInterpret-0.2.3/ClassificationModels/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-24 12:44:01.000000 TSInterpret-0.2.3/ClassificationModels/CNN.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-04-24 12:44:01.000000 TSInterpret-0.2.3/ClassificationModels/CNN_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-24 12:44:01.000000 TSInterpret-0.2.3/ClassificationModels/DecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-24 12:44:01.000000 TSInterpret-0.2.3/ClassificationModels/LSTM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-24 12:44:01.000000 TSInterpret-0.2.3/ClassificationModels/LSTM_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-24 12:44:01.000000 TSInterpret-0.2.3/ClassificationModels/ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:01.000000 TSInterpret-0.2.3/ClassificationModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/ClassificationModels/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-24 12:44:13.179923 TSInterpret-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.171923 TSInterpret-0.2.3/TSInterpret/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.175922 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/FeatureAttribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.175922 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/GradCam/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/GradCam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/InstanceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.175922 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/Saliency/
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/Saliency/TSR.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/Saliency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.175922 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/CF.py
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.175922 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.175922 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.175922 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.175922 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/leftist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/neighbors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.179923 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.179923 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.179923 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.179923 TSInterpret-0.2.3/TSInterpret/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/Models/PyTorchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/Models/SklearnModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/Models/TensorflowModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/Models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/TSInterpret/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:44:13.175922 TSInterpret-0.2.3/TSInterpret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-24 12:44:13.000000 TSInterpret-0.2.3/TSInterpret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-24 12:44:13.000000 TSInterpret-0.2.3/TSInterpret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:44:13.000000 TSInterpret-0.2.3/TSInterpret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-24 12:44:13.000000 TSInterpret-0.2.3/TSInterpret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 12:44:13.000000 TSInterpret-0.2.3/TSInterpret.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 12:44:13.179923 TSInterpret-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-24 12:44:02.000000 TSInterpret-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.814748 TSInterpret-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.806748 TSInterpret-0.2.4/ClassificationModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/CNN_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/DecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/LSTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/LSTM_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/ClassificationModels/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-05-30 08:14:04.814748 TSInterpret-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.806748 TSInterpret-0.2.4/TSInterpret/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.806748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/FeatureAttribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.806748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/GradCam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/GradCam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/InstanceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.806748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/TSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/CF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/leftist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/neighbors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.810748 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.814748 TSInterpret-0.2.4/TSInterpret/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/Models/PyTorchModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/Models/SklearnModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/Models/TensorflowModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/Models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/TSInterpret/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:14:04.806748 TSInterpret-0.2.4/TSInterpret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-05-30 08:14:04.000000 TSInterpret-0.2.4/TSInterpret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-30 08:14:04.000000 TSInterpret-0.2.4/TSInterpret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:14:04.000000 TSInterpret-0.2.4/TSInterpret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-30 08:14:04.000000 TSInterpret-0.2.4/TSInterpret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 08:14:04.000000 TSInterpret-0.2.4/TSInterpret.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:14:04.814748 TSInterpret-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-30 08:13:46.000000 TSInterpret-0.2.4/setup.py
```

### Comparing `TSInterpret-0.2.3/ClassificationModels/CNN.py` & `TSInterpret-0.2.4/ClassificationModels/CNN.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/ClassificationModels/CNN_T.py` & `TSInterpret-0.2.4/ClassificationModels/CNN_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/ClassificationModels/DecisionTree.py` & `TSInterpret-0.2.4/ClassificationModels/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/ClassificationModels/LSTM.py` & `TSInterpret-0.2.4/ClassificationModels/LSTM.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/ClassificationModels/LSTM_T.py` & `TSInterpret-0.2.4/ClassificationModels/LSTM_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/ClassificationModels/ResNet.py` & `TSInterpret-0.2.4/ClassificationModels/ResNet.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/ClassificationModels/utils.py` & `TSInterpret-0.2.4/ClassificationModels/utils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/LICENSE` & `TSInterpret-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/PKG-INFO` & `TSInterpret-0.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.2.3
+Version: 0.2.4
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -33,14 +33,17 @@
   </a>
     <img alt="PyPI" src="https://img.shields.io/pypi/v/tsinterpret">
     <a href="https://codecov.io/gh/fzi-forschungszentrum-informatik/TSInterpret" > 
         <img src="https://codecov.io/gh/fzi-forschungszentrum-informatik/TSInterpret/branch/main/graph/badge.svg?token=1IGZKTLZ4J"/> 
     </a>
     <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/tsinterpret">
     <img alt="GitHub" src="https://img.shields.io/github/license/fzi-forschungszentrum-informatik/TSInterpret">
+    <a style="border-width:0" href="https://doi.org/10.21105/joss.05220">
+  <img src="https://joss.theoj.org/papers/10.21105/joss.05220/status.svg" alt="DOI badge" >
+</a>
 </p>
 
 TSInterpret is a Python library for interpreting time series classification.
 The ambition is to faciliate the usage of time series interpretability methods. The Framework supports Sklearn, Tensorflow, Torch and in some cases predict functions. A listing of implemented algorithms and supported frameworks can be found in our <a href="https://fzi-forschungszentrum-informatik.github.io/TSInterpret/">Documentation</a>. More information on our framework can be found in our <a href="https://arxiv.org/abs/2208.05280"> paper<a>.
 
 ## 💈 Installation
 ```shell
@@ -52,14 +55,29 @@
 ```
 
 Or, through SSH:
 ```shell
 pip install git@github.com:fzi-forschungszentrum-informatik/TSInterpret.git --upgrade
 ```
 
+On Windows with Anaconda there is a known installation issue due to the <a href='https://github.com/scikit-learn/sklearn-pypi-package'>sklearn brownout</a> in third party dependencies. The workaround (working for python 3.9) till all the dependencies are fixed: 
+
+1. Set Enviroment Variable
+```shell
+set SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=True
+```
+2. Install sklearn in advance 
+```shell
+pip install sklearn=0.0
+```
+
+3. Install TsIntrerpret
+```shell
+pip install TSInterpret
+```
 
 ## 🍫 Quickstart
 The following example creates a simple Neural Network based on tensorflow and interprets the Classfier with Integrated Gradients and Temporal Saliency Rescaling [1].
 For further examples check out the <a href="https://fzi-forschungszentrum-informatik.github.io/TSInterpret/">Documentation</a>.
 
 [1] Ismail, Aya Abdelsalam, et al. "Benchmarking deep learning interpretability in time series predictions." Advances in neural information processing systems 33 (2020): 6441-6452.
 
@@ -128,25 +146,18 @@
 </p>
 
 ## Citation
 
 If you use TSInterpret in your research, please consider citing it and the authors' original papers. The authors' original papers are cited in the documentation and the paper below.
 
 ```
-@misc{https://doi.org/10.48550/arxiv.2208.05280,
-  doi = {10.48550/ARXIV.2208.05280},
-  
-  url = {https://arxiv.org/abs/2208.05280},
-  
-  author = {Höllig, Jacqueline and Kulbach, Cedric and Thoma, Steffen},
-  
-  keywords = {Machine Learning (cs.LG), FOS: Computer and information sciences, FOS: Computer and information sciences},
-  
-  title = {TSInterpret: A unified framework for time series interpretability},
-  
-  publisher = {arXiv},
-  
-  year = {2022},
-  
-  copyright = {Creative Commons Attribution 4.0 International}
-}
+@article{Höllig2023, 
+doi = {10.21105/joss.05220}, 
+url = {https://doi.org/10.21105/joss.05220}, 
+year = {2023}, 
+publisher = {The Open Journal}, 
+volume = {8}, 
+number = {85}, 
+pages = {5220}, 
+author = {Jacqueline Höllig and Cedric Kulbach and Steffen Thoma}, 
+title = {TSInterpret: A Python Package for the Interpretability of Time Series Classification}, journal = {Journal of Open Source Software} } 
 ```
```

#### html2text {}

```diff
@@ -1,45 +1,51 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.3 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.4 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.6.0 Description-Content-Type: text/
 markdown Provides-Extra: dev Provides-Extra: test Provides-Extra: docs
 Provides-Extra: all License-File: LICENSE
                               [TSInterpret Logo]
     [tests] [PyPI] [https://codecov.io/gh/fzi-forschungszentrum-informatik/
  TSInterpret/branch/main/graph/badge.svg?token=1IGZKTLZ4J] [PyPI - Downloads]
-                                   [GitHub]
+                             [GitHub] [DOI_badge]
 TSInterpret is a Python library for interpreting time series classification.
 The ambition is to faciliate the usage of time series interpretability methods.
 The Framework supports Sklearn, Tensorflow, Torch and in some cases predict
 functions. A listing of implemented algorithms and supported frameworks can be
 found in our Documentation. More information on our framework can be found in
 our
 paper
 ._##_ð_Installation_```shell_pip_install_TSInterpret_```_You_can_install_the
 latest_development_version_from_GitHub_as_so:_```shell_pip_install_https://
 github.com/fzi-forschungszentrum-informatik/TSInterpret.git_--upgrade_```_Or,
 through_SSH:_```shell_pip_install_git@github.com:fzi-forschungszentrum-
-informatik/TSInterpret.git_--upgrade_```_##_ð«_Quickstart_The_following
-example_creates_a_simple_Neural_Network_based_on_tensorflow_and_interprets_the
-Classfier_with_Integrated_Gradients_and_Temporal_Saliency_Rescaling_[1]._For
-further_examples_check_out_the_Documentation._[1]_Ismail,_Aya_Abdelsalam,_et
-al._"Benchmarking_deep_learning_interpretability_in_time_series_predictions."
-Advances_in_neural_information_processing_systems_33_(2020):_6441-6452._###
-Import_```python_import_pickle_import_numpy_as_np_import_matplotlib.pyplot_as
-plt_import_seaborn_as_snst_from_tslearn.datasets_import_UCR_UEA_datasets_import
-tensorflow_as_tf_```_###_Create_Classifcation_Model_This_Section_uses_a
-pretrained_Classification_Model_to_illustrate_the_use_of_our_package._For
-running_the_example,_please_clone_our_repository_and_comment_the_variable
+informatik/TSInterpret.git_--upgrade_```_On_Windows_with_Anaconda_there_is_a
+known_installation_issue_due_to_the_sklearn_brownout_in_third_party
+dependencies._The_workaround_(working_for_python_3.9)_till_all_the_dependencies
+are_fixed:_1._Set_Enviroment_Variable_```shell_set
+SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=True_```_2._Install_sklearn_in
+advance_```shell_pip_install_sklearn=0.0_```_3._Install_TsIntrerpret_```shell
+pip_install_TSInterpret_```_##_ð«_Quickstart_The_following_example_creates_a
+simple_Neural_Network_based_on_tensorflow_and_interprets_the_Classfier_with
+Integrated_Gradients_and_Temporal_Saliency_Rescaling_[1]._For_further_examples
+check_out_the_Documentation._[1]_Ismail,_Aya_Abdelsalam,_et_al._"Benchmarking
+deep_learning_interpretability_in_time_series_predictions."_Advances_in_neural
+information_processing_systems_33_(2020):_6441-6452._###_Import_```python
+import_pickle_import_numpy_as_np_import_matplotlib.pyplot_as_plt_import_seaborn
+as_snst_from_tslearn.datasets_import_UCR_UEA_datasets_import_tensorflow_as_tf
+```_###_Create_Classifcation_Model_This_Section_uses_a_pretrained
+Classification_Model_to_illustrate_the_use_of_our_package._For_running_the
+example,_please_clone_our_repository_and_comment_the_variable
 PATH_TO_YOUR_CLASSIFICATION_MODEL_in._The_code_in_this_section_can_also_be
 replaces_with_your_personal_classification_model_written_in_torch_or
 tensorflow._```python_#_Load_data._dataset='BasicMotions'_train_x,train_y,
 test_x,_test_y=UCR_UEA_datasets().load_dataset(dataset)
 enc1=sklearn.OneHotEncoder(sparse=False).fit(train_y.reshape(-1,1))
 train_y=enc1.transform(train_y.reshape(-1,1))_test_y=enc1.transform
 (test_y.reshape(-1,1))_#_Load_a_model._#e.g.,
@@ -75,14 +81,13 @@
 informatik/TSInterpret/issues/new/choose)._-_Before_opening_a_pull_request,_we
 also_encourage_users_to_open_an_issue_for_discussion._Details_on_how_to
 Contribute_can_be_found_[here](https://github.com/fzi-forschungszentrum-
 informatik/TSInterpret/blob/main/CONTRIBUTING.md)._##_ð«_Affiliations
                                   [FZI_Logo]
 ##_Citation_If_you_use_TSInterpret_in_your_research,_please_consider_citing_it
 and_the_authors'_original_papers._The_authors'_original_papers_are_cited_in_the
-documentation_and_the_paper_below._```_@misc{https://doi.org/10.48550/
-arxiv.2208.05280,_doi_=_{10.48550/ARXIV.2208.05280},_url_=_{https://arxiv.org/
-abs/2208.05280},_author_=_{HÃ¶llig,_Jacqueline_and_Kulbach,_Cedric_and_Thoma,
-Steffen},_keywords_=_{Machine_Learning_(cs.LG),_FOS:_Computer_and_information
-sciences,_FOS:_Computer_and_information_sciences},_title_=_{TSInterpret:_A
-unified_framework_for_time_series_interpretability},_publisher_=_{arXiv},_year
-=_{2022},_copyright_=_{Creative_Commons_Attribution_4.0_International}_}_```
+documentation_and_the_paper_below._```_@article{HÃ¶llig2023,_doi_=_{10.21105/
+joss.05220},_url_=_{https://doi.org/10.21105/joss.05220},_year_=_{2023},
+publisher_=_{The_Open_Journal},_volume_=_{8},_number_=_{85},_pages_=_{5220},
+author_=_{Jacqueline_HÃ¶llig_and_Cedric_Kulbach_and_Steffen_Thoma},_title_=
+{TSInterpret:_A_Python_Package_for_the_Interpretability_of_Time_Series
+Classification},_journal_=_{Journal_of_Open_Source_Software}_}_```
```

### Comparing `TSInterpret-0.2.3/README.md` & `TSInterpret-0.2.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,17 @@
   </a>
     <img alt="PyPI" src="https://img.shields.io/pypi/v/tsinterpret">
     <a href="https://codecov.io/gh/fzi-forschungszentrum-informatik/TSInterpret" > 
         <img src="https://codecov.io/gh/fzi-forschungszentrum-informatik/TSInterpret/branch/main/graph/badge.svg?token=1IGZKTLZ4J"/> 
     </a>
     <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/tsinterpret">
     <img alt="GitHub" src="https://img.shields.io/github/license/fzi-forschungszentrum-informatik/TSInterpret">
+    <a style="border-width:0" href="https://doi.org/10.21105/joss.05220">
+  <img src="https://joss.theoj.org/papers/10.21105/joss.05220/status.svg" alt="DOI badge" >
+</a>
 </p>
 
 TSInterpret is a Python library for interpreting time series classification.
 The ambition is to faciliate the usage of time series interpretability methods. The Framework supports Sklearn, Tensorflow, Torch and in some cases predict functions. A listing of implemented algorithms and supported frameworks can be found in our <a href="https://fzi-forschungszentrum-informatik.github.io/TSInterpret/">Documentation</a>. More information on our framework can be found in our <a href="https://arxiv.org/abs/2208.05280"> paper<a>.
 
 ## 💈 Installation
 ```shell
@@ -26,14 +29,29 @@
 ```
 
 Or, through SSH:
 ```shell
 pip install git@github.com:fzi-forschungszentrum-informatik/TSInterpret.git --upgrade
 ```
 
+On Windows with Anaconda there is a known installation issue due to the <a href='https://github.com/scikit-learn/sklearn-pypi-package'>sklearn brownout</a> in third party dependencies. The workaround (working for python 3.9) till all the dependencies are fixed: 
+
+1. Set Enviroment Variable
+```shell
+set SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=True
+```
+2. Install sklearn in advance 
+```shell
+pip install sklearn=0.0
+```
+
+3. Install TsIntrerpret
+```shell
+pip install TSInterpret
+```
 
 ## 🍫 Quickstart
 The following example creates a simple Neural Network based on tensorflow and interprets the Classfier with Integrated Gradients and Temporal Saliency Rescaling [1].
 For further examples check out the <a href="https://fzi-forschungszentrum-informatik.github.io/TSInterpret/">Documentation</a>.
 
 [1] Ismail, Aya Abdelsalam, et al. "Benchmarking deep learning interpretability in time series predictions." Advances in neural information processing systems 33 (2020): 6441-6452.
 
@@ -102,25 +120,18 @@
 </p>
 
 ## Citation
 
 If you use TSInterpret in your research, please consider citing it and the authors' original papers. The authors' original papers are cited in the documentation and the paper below.
 
 ```
-@misc{https://doi.org/10.48550/arxiv.2208.05280,
-  doi = {10.48550/ARXIV.2208.05280},
-  
-  url = {https://arxiv.org/abs/2208.05280},
-  
-  author = {Höllig, Jacqueline and Kulbach, Cedric and Thoma, Steffen},
-  
-  keywords = {Machine Learning (cs.LG), FOS: Computer and information sciences, FOS: Computer and information sciences},
-  
-  title = {TSInterpret: A unified framework for time series interpretability},
-  
-  publisher = {arXiv},
-  
-  year = {2022},
-  
-  copyright = {Creative Commons Attribution 4.0 International}
-}
+@article{Höllig2023, 
+doi = {10.21105/joss.05220}, 
+url = {https://doi.org/10.21105/joss.05220}, 
+year = {2023}, 
+publisher = {The Open Journal}, 
+volume = {8}, 
+number = {85}, 
+pages = {5220}, 
+author = {Jacqueline Höllig and Cedric Kulbach and Steffen Thoma}, 
+title = {TSInterpret: A Python Package for the Interpretability of Time Series Classification}, journal = {Journal of Open Source Software} } 
 ```
```

#### html2text {}

```diff
@@ -1,33 +1,39 @@
                               [TSInterpret Logo]
     [tests] [PyPI] [https://codecov.io/gh/fzi-forschungszentrum-informatik/
  TSInterpret/branch/main/graph/badge.svg?token=1IGZKTLZ4J] [PyPI - Downloads]
-                                   [GitHub]
+                             [GitHub] [DOI_badge]
 TSInterpret is a Python library for interpreting time series classification.
 The ambition is to faciliate the usage of time series interpretability methods.
 The Framework supports Sklearn, Tensorflow, Torch and in some cases predict
 functions. A listing of implemented algorithms and supported frameworks can be
 found in our Documentation. More information on our framework can be found in
 our
 paper
 ._##_ð_Installation_```shell_pip_install_TSInterpret_```_You_can_install_the
 latest_development_version_from_GitHub_as_so:_```shell_pip_install_https://
 github.com/fzi-forschungszentrum-informatik/TSInterpret.git_--upgrade_```_Or,
 through_SSH:_```shell_pip_install_git@github.com:fzi-forschungszentrum-
-informatik/TSInterpret.git_--upgrade_```_##_ð«_Quickstart_The_following
-example_creates_a_simple_Neural_Network_based_on_tensorflow_and_interprets_the
-Classfier_with_Integrated_Gradients_and_Temporal_Saliency_Rescaling_[1]._For
-further_examples_check_out_the_Documentation._[1]_Ismail,_Aya_Abdelsalam,_et
-al._"Benchmarking_deep_learning_interpretability_in_time_series_predictions."
-Advances_in_neural_information_processing_systems_33_(2020):_6441-6452._###
-Import_```python_import_pickle_import_numpy_as_np_import_matplotlib.pyplot_as
-plt_import_seaborn_as_snst_from_tslearn.datasets_import_UCR_UEA_datasets_import
-tensorflow_as_tf_```_###_Create_Classifcation_Model_This_Section_uses_a
-pretrained_Classification_Model_to_illustrate_the_use_of_our_package._For
-running_the_example,_please_clone_our_repository_and_comment_the_variable
+informatik/TSInterpret.git_--upgrade_```_On_Windows_with_Anaconda_there_is_a
+known_installation_issue_due_to_the_sklearn_brownout_in_third_party
+dependencies._The_workaround_(working_for_python_3.9)_till_all_the_dependencies
+are_fixed:_1._Set_Enviroment_Variable_```shell_set
+SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=True_```_2._Install_sklearn_in
+advance_```shell_pip_install_sklearn=0.0_```_3._Install_TsIntrerpret_```shell
+pip_install_TSInterpret_```_##_ð«_Quickstart_The_following_example_creates_a
+simple_Neural_Network_based_on_tensorflow_and_interprets_the_Classfier_with
+Integrated_Gradients_and_Temporal_Saliency_Rescaling_[1]._For_further_examples
+check_out_the_Documentation._[1]_Ismail,_Aya_Abdelsalam,_et_al._"Benchmarking
+deep_learning_interpretability_in_time_series_predictions."_Advances_in_neural
+information_processing_systems_33_(2020):_6441-6452._###_Import_```python
+import_pickle_import_numpy_as_np_import_matplotlib.pyplot_as_plt_import_seaborn
+as_snst_from_tslearn.datasets_import_UCR_UEA_datasets_import_tensorflow_as_tf
+```_###_Create_Classifcation_Model_This_Section_uses_a_pretrained
+Classification_Model_to_illustrate_the_use_of_our_package._For_running_the
+example,_please_clone_our_repository_and_comment_the_variable
 PATH_TO_YOUR_CLASSIFICATION_MODEL_in._The_code_in_this_section_can_also_be
 replaces_with_your_personal_classification_model_written_in_torch_or
 tensorflow._```python_#_Load_data._dataset='BasicMotions'_train_x,train_y,
 test_x,_test_y=UCR_UEA_datasets().load_dataset(dataset)
 enc1=sklearn.OneHotEncoder(sparse=False).fit(train_y.reshape(-1,1))
 train_y=enc1.transform(train_y.reshape(-1,1))_test_y=enc1.transform
 (test_y.reshape(-1,1))_#_Load_a_model._#e.g.,
@@ -63,14 +69,13 @@
 informatik/TSInterpret/issues/new/choose)._-_Before_opening_a_pull_request,_we
 also_encourage_users_to_open_an_issue_for_discussion._Details_on_how_to
 Contribute_can_be_found_[here](https://github.com/fzi-forschungszentrum-
 informatik/TSInterpret/blob/main/CONTRIBUTING.md)._##_ð«_Affiliations
                                   [FZI_Logo]
 ##_Citation_If_you_use_TSInterpret_in_your_research,_please_consider_citing_it
 and_the_authors'_original_papers._The_authors'_original_papers_are_cited_in_the
-documentation_and_the_paper_below._```_@misc{https://doi.org/10.48550/
-arxiv.2208.05280,_doi_=_{10.48550/ARXIV.2208.05280},_url_=_{https://arxiv.org/
-abs/2208.05280},_author_=_{HÃ¶llig,_Jacqueline_and_Kulbach,_Cedric_and_Thoma,
-Steffen},_keywords_=_{Machine_Learning_(cs.LG),_FOS:_Computer_and_information
-sciences,_FOS:_Computer_and_information_sciences},_title_=_{TSInterpret:_A
-unified_framework_for_time_series_interpretability},_publisher_=_{arXiv},_year
-=_{2022},_copyright_=_{Creative_Commons_Attribution_4.0_International}_}_```
+documentation_and_the_paper_below._```_@article{HÃ¶llig2023,_doi_=_{10.21105/
+joss.05220},_url_=_{https://doi.org/10.21105/joss.05220},_year_=_{2023},
+publisher_=_{The_Open_Journal},_volume_=_{8},_number_=_{85},_pages_=_{5220},
+author_=_{Jacqueline_HÃ¶llig_and_Cedric_Kulbach_and_Steffen_Thoma},_title_=
+{TSInterpret:_A_Python_Package_for_the_Interpretability_of_Time_Series
+Classification},_journal_=_{Journal_of_Open_Source_Software}_}_```
```

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/FeatureAttribution.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/FeatureAttribution.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/InterpretabilityBase.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/InterpretabilityBase.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,26 +44,28 @@
     def __init__(
         self,
         model,
         NumTimeSteps: int,
         NumFeatures: int,
         method: str = "GRAD",
         mode: str = "time",
+        tsr: bool = True,
         device: str = "cpu",
     ) -> None:
         """Initialization
         Arguments:
             model [torch.nn.Module]: model to be explained
             NumTimeSteps int : Number of Time Step
             NumFeatures int : Number Features
             method str: Saliency Methode to be used
             mode str: Second dimension 'time'->`(1,time,feat)`  or 'feat'->`(1,feat,time)`
         """
         super().__init__(model, NumTimeSteps, NumFeatures, method, mode)
         self.method = method
+        self.tsr = tsr
         if method == "GRAD":
             self.Grad = Saliency(model)
         elif method == "IG":
             self.Grad = IntegratedGradients(model)
         elif method == "GS":
             self.Grad = GradientShap(model)
         elif method == "DL":
@@ -79,29 +81,29 @@
         #    self.Grad = FeaturePermutation(model)
         elif method == "FA":
             self.Grad = FeatureAblation(model)
         elif method == "FO":
             self.Grad = Occlusion(model)
         self.device = device
 
-    def explain(self, item: np.ndarray, labels: int, TSR: bool = True):
+    def explain(self, item: np.ndarray, labels: int, TSR=None):
         """Method to explain the model based on the item.
         Arguments:
             item np.array: item to get feature attribution for, if `mode = time`->`(1,time,feat)`  or `mode = feat`->`(1,feat,time)`
             labels int: label
             TSR bool: if True time series rescaling according to [1] is used, else plain (scaled) weights are returened
         Returns:
             np.array: feature attribution weights `mode = time`->`(time,feat)` or `mode = feat`->`(feat,time)`
         """
         mask = np.zeros((self.NumTimeSteps, self.NumFeatures), dtype=int)
         for i in range(self.NumTimeSteps):
             mask[i, :] = i
         rescaledGrad = np.zeros(item.shape)
         idx = 0
-        item = np.array(item.tolist(), dtype=np.float64)
+        item = np.array(item.tolist())  # , dtype=np.float64)
         input = torch.from_numpy(item)
 
         input = input.reshape(-1, self.NumTimeSteps, self.NumFeatures).to(self.device)
         input = Variable(input, volatile=False, requires_grad=True)
 
         batch_size = input.shape[0]
 
@@ -168,16 +170,18 @@
             has_sliding_window = (1, self.NumFeatures)
             attributions = self.Grad.attribute(
                 input,
                 sliding_window_shapes=(1, self.NumFeatures),
                 target=labels,
                 baselines=baseline_single,
             )
+        if TSR is not None:
+            self.tsr = TSR
 
-        if TSR:
+        if self.tsr:
             # print('TSR', TSR)
             TSR_attributions = self._getTwoStepRescaling(
                 input,
                 labels,
                 hasBaseline=base,
                 hasSliding_window_shapes=has_sliding_window,
             )
```

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     For Tensorflow the following saliency methods are available:
         + Gradients (GRAD)
         + Integrated Gradients (IG)
         + Gradient Shap (GS))
         + DeepLiftShap (DLS)
         + SmoothGrad (SG)
         + Occlusion (FO)
+
+    Attention: GS and DLS only work for Python < 3.10.
+
     References
     ----------
     [1] Ismail, Aya Abdelsalam, et al.
     "Benchmarking deep learning interpretability in time series predictions."
     Advances in neural information processing systems 33 (2020): 6441-6452.
 
     [2] Meudec, Raphael: , tf-explain. https://github.com/sicara/tf-explain
@@ -40,28 +43,30 @@
     def __init__(
         self,
         model,
         NumTimeSteps: int,
         NumFeatures: int,
         method: str = "GRAD",
         mode: str = "time",
+        tsr: bool = True,
         device: str = "cpu",
     ) -> None:
         """
         Arguments:
             model [tf.keras.models]: model to be explained
             NumTimeSteps int : Number of Time Step
             NumFeatures int : Number Features
             method str: Saliency Methode to be used
             mode str: Second dimension 'time'->`(1,time,feat)`  or 'feat'->`(1,feat,time)`
         """
         # tf explain does not provide baseline !
         super().__init__(model, NumTimeSteps, NumFeatures, method, mode)
         print("Mode in TF Saliency", self.mode)
         self.method = method
+        self.tsr = tsr
         if method == "GRAD":
             self.Grad = VanillaGradients()
         if method == "IG":
             self.Grad = IntegratedGradients()
         # elif method == 'DL':
         #    self.Grad = DeepLift(model)
         elif method == "DLS":
@@ -76,15 +81,15 @@
         # elif method == 'FP':
         #    self.Grad = FeaturePermutation(model)
         # elif method == 'FA':
         #    self.Grad = FeatureAblation(model)
         elif method == "FO":
             self.Grad = OcclusionSensitivity()
 
-    def explain(self, item, labels, TSR=True):
+    def explain(self, item, labels, TSR=None):
         """Method to explain the model based on the item.
         Arguments:
             item np.array: item to get feature attribution for, if `mode = time`->`(1,time,feat)`  or `mode = feat`->`(1,feat,time)`
             labels int: label
             TSR bool: if True time series rescaling according to [1] is used, else plain (scaled) weights are returened
         Returns:
             np.array: feature attribution weights `mode = time`->`(time,feat)` or `mode = feat`->`(feat,time)`
@@ -109,16 +114,17 @@
             input = input.reshape(-1, self.NumFeatures, self.NumTimeSteps, 1)
             attributions = self.Grad.explain(
                 (input, None),
                 self.model,
                 class_index=labels,
                 patch_size=self.NumFeatures,
             )
-
-        if TSR:
+        if TSR is not None:
+            self.tsr = TSR
+        if self.tsr:
             # print(base)
             TSR_attributions = self._getTwoStepRescaling(input, labels)
             TSR_saliency = self._givenAttGetRescaledSaliency(TSR_attributions)
             return TSR_saliency
         else:
             rescaledGrad[
                 idx : idx + batch_size, :, :
```

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/Saliency/TSR.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/Saliency/TSR.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/Ates.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/Ates.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/CF.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/CF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             distance_measure str: sklearn appreviation for distance of knn.
             n_neighbore int: # neighbors to select from.
             max_iter int : max number of runs
         """
         super().__init__(model, mode)
         self.backend = backend
         test_x, test_y = reference_set
-        test_x = np.array(test_x, dtype=np.float32)
+        test_x = np.array(test_x)  # , dtype=np.float32)
 
         if mode == "time":
             # Parse test data into (1, feat, time):
             self.ts_length = shape[-2]
             test_x = test_x.reshape(test_x.shape[0], test_x.shape[2], test_x.shape[1])
         elif mode == "feat":
             self.ts_length = shape[-1]
@@ -121,15 +121,15 @@
         x_train.reshape(-1, 1, ts_length)
         return dist[0], x_train[np.where(y != predicted_label)][ind[0]]
 
     def _native_guide_wrapper(self, query, predicted_label, distance, n_neighbors):
         _, nun = self._native_guide_retrieval(
             query, predicted_label, distance, n_neighbors
         )
-        individual = np.array(nun.tolist(), dtype=np.float64)
+        individual = np.array(nun.tolist())  # , dtype=np.float64)
         out = self.predict(individual)
         return nun, np.argmax(out)
 
     def _findSubarray(
         self, a, k
     ):  # used to find the maximum contigious subarray of length k in the explanation weight vector
 
@@ -160,44 +160,45 @@
         print(label)
         _, nun = self._native_guide_retrieval(instance, label, self.distance_measure, 1)
         if np.count_nonzero(nun.reshape(-1) - instance.reshape(-1)) == 0:
             print("Starting and nun are Identical !")
 
         test_x, test_y = self.reference_set
         train_x = test_x
-        individual = np.array(nun.tolist(), dtype=np.float64)
+        individual = np.array(nun.tolist())  # , dtype=np.float64)
         out = self.predict(individual)
         if self.backend == "PYT":
             training_weights = (
                 self.cam_extractor(out.squeeze(0).argmax().item(), out)[0]
                 .detach()
                 .numpy()
             )
         elif self.backend == "TF":
             data = (instance.reshape(1, -1, 1), None)
             training_weights = self.cam_extractor.explain(
                 data, self.model, class_index=label[0]
             )  # grad_cam(self.model, instance.reshape(1,-1,1))#self.cam_extractor.explain(data, self.model,class_index=label)#instance
         # Classify Original
-        individual = np.array(instance.tolist(), dtype=np.float64)
+        individual = np.array(instance.tolist())  # , dtype=np.float64)
         out = self.predict(individual)
 
         most_influencial_array = self._findSubarray((training_weights), subarray_length)
 
         starting_point = np.where(training_weights == most_influencial_array[0])[0][0]
 
         X_example = instance.copy().reshape(1, -1)
 
         nun = nun.reshape(1, -1)
         X_example[0, starting_point : subarray_length + starting_point] = nun[
             0, starting_point : subarray_length + starting_point
         ]
         individual = np.array(
-            X_example.reshape(-1, 1, train_x.shape[-1]).tolist(), dtype=np.float64
-        )
+            X_example.reshape(-1, 1, train_x.shape[-1]).tolist()
+        )  # , dtype=np.float64
+        # )
         out = self.predict(individual)
         prob_target = out[0][
             label
         ]  # torch.nn.functional.softmax(model(torch.from_numpy(test_x))).detach().numpy()[0][y_pred[instance]]
         counter = 0
         while prob_target > 0.5 and counter < max_iter:
 
@@ -209,16 +210,17 @@
                 0
             ]
             X_example = instance.copy().reshape(1, -1)
             X_example[:, starting_point : subarray_length + starting_point] = nun[
                 :, starting_point : subarray_length + starting_point
             ]
             individual = np.array(
-                X_example.reshape(-1, 1, train_x.shape[-1]).tolist(), dtype=np.float64
-            )
+                X_example.reshape(-1, 1, train_x.shape[-1]).tolist()
+            )  # , dtype=np.float64
+            # )
             out = self.predict(individual)
             prob_target = out[0][label]
             counter = counter + 1
             if counter == max_iter or subarray_length == self.ts_length:
                 print("No Counterfactual found")
                 return None, None
 
@@ -226,36 +228,36 @@
 
     def _instance_based_cf(self, query, label, target, distance="dtw", max_iter=500):
 
         d, nan = self._native_guide_retrieval(query, label, distance, 1)
         beta = 0
         insample_cf = nan.reshape(1, 1, -1)
 
-        individual = np.array(query.tolist(), dtype=np.float64)
+        individual = np.array(query.tolist())  # , dtype=np.float64)
 
         output = self.predict(individual)
         pred_treshold = 0.5
         target = np.argsort(output)[0][-2:-1][0]
         query = query.reshape(-1)
         insample_cf = insample_cf.reshape(-1)
         generated_cf = dtw_barycenter_averaging(
             [query, insample_cf], weights=np.array([(1 - beta), beta])
         )
         generated_cf = generated_cf.reshape(1, 1, -1)
-        individual = np.array(generated_cf.tolist(), dtype=np.float64)
+        individual = np.array(generated_cf.tolist())  # , dtype=np.float64)
         prob_target = self.predict(individual)[0][target]
         counter = 0
 
         while prob_target < pred_treshold and counter < max_iter:
             beta += 0.01
             generated_cf = dtw_barycenter_averaging(
                 [query, insample_cf], weights=np.array([(1 - beta), beta])
             )
             generated_cf = generated_cf.reshape(1, 1, -1)
-            individual = np.array(generated_cf.tolist(), dtype=np.float64)
+            individual = np.array(generated_cf.tolist())  # , dtype=np.float64)
             prob_target = self.predict(individual)[0][target]
 
             counter = counter + 1
         if counter == max_iter:
             print("No Counterfactual found")
             return None, None
```

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/leftist.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/leftist.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/neighbors.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/neighbors.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/InterpretabilityModels/leftist/transform.py` & `TSInterpret-0.2.4/TSInterpret/InterpretabilityModels/leftist/transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/Models/PyTorchModel.py` & `TSInterpret-0.2.4/TSInterpret/Models/PyTorchModel.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def predict(self, item) -> List:
         """Unified prediction function.
         Arguments:
             item np.array: item to be classified.
          Returns:
             an array of output scores for a classifier.
         """
-        item = np.array(item.tolist(), dtype=np.float64)
+        item = np.array(item.tolist())  # , dtype=np.float64)
         if self.change:
             item = torch.from_numpy(item.reshape(-1, item.shape[-1], item.shape[-2]))
 
         else:
             item = torch.from_numpy(item)
         out = self.model(item.float())
         y_pred = torch.nn.functional.softmax(out).detach().numpy()
```

### Comparing `TSInterpret-0.2.3/TSInterpret/Models/SklearnModel.py` & `TSInterpret-0.2.4/TSInterpret/Models/SklearnModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/Models/TensorflowModel.py` & `TSInterpret-0.2.4/TSInterpret/Models/TensorflowModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret/Models/base_model.py` & `TSInterpret-0.2.4/TSInterpret/Models/base_model.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret.egg-info/PKG-INFO` & `TSInterpret-0.2.4/TSInterpret.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.2.3
+Version: 0.2.4
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -33,14 +33,17 @@
   </a>
     <img alt="PyPI" src="https://img.shields.io/pypi/v/tsinterpret">
     <a href="https://codecov.io/gh/fzi-forschungszentrum-informatik/TSInterpret" > 
         <img src="https://codecov.io/gh/fzi-forschungszentrum-informatik/TSInterpret/branch/main/graph/badge.svg?token=1IGZKTLZ4J"/> 
     </a>
     <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/tsinterpret">
     <img alt="GitHub" src="https://img.shields.io/github/license/fzi-forschungszentrum-informatik/TSInterpret">
+    <a style="border-width:0" href="https://doi.org/10.21105/joss.05220">
+  <img src="https://joss.theoj.org/papers/10.21105/joss.05220/status.svg" alt="DOI badge" >
+</a>
 </p>
 
 TSInterpret is a Python library for interpreting time series classification.
 The ambition is to faciliate the usage of time series interpretability methods. The Framework supports Sklearn, Tensorflow, Torch and in some cases predict functions. A listing of implemented algorithms and supported frameworks can be found in our <a href="https://fzi-forschungszentrum-informatik.github.io/TSInterpret/">Documentation</a>. More information on our framework can be found in our <a href="https://arxiv.org/abs/2208.05280"> paper<a>.
 
 ## 💈 Installation
 ```shell
@@ -52,14 +55,29 @@
 ```
 
 Or, through SSH:
 ```shell
 pip install git@github.com:fzi-forschungszentrum-informatik/TSInterpret.git --upgrade
 ```
 
+On Windows with Anaconda there is a known installation issue due to the <a href='https://github.com/scikit-learn/sklearn-pypi-package'>sklearn brownout</a> in third party dependencies. The workaround (working for python 3.9) till all the dependencies are fixed: 
+
+1. Set Enviroment Variable
+```shell
+set SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=True
+```
+2. Install sklearn in advance 
+```shell
+pip install sklearn=0.0
+```
+
+3. Install TsIntrerpret
+```shell
+pip install TSInterpret
+```
 
 ## 🍫 Quickstart
 The following example creates a simple Neural Network based on tensorflow and interprets the Classfier with Integrated Gradients and Temporal Saliency Rescaling [1].
 For further examples check out the <a href="https://fzi-forschungszentrum-informatik.github.io/TSInterpret/">Documentation</a>.
 
 [1] Ismail, Aya Abdelsalam, et al. "Benchmarking deep learning interpretability in time series predictions." Advances in neural information processing systems 33 (2020): 6441-6452.
 
@@ -128,25 +146,18 @@
 </p>
 
 ## Citation
 
 If you use TSInterpret in your research, please consider citing it and the authors' original papers. The authors' original papers are cited in the documentation and the paper below.
 
 ```
-@misc{https://doi.org/10.48550/arxiv.2208.05280,
-  doi = {10.48550/ARXIV.2208.05280},
-  
-  url = {https://arxiv.org/abs/2208.05280},
-  
-  author = {Höllig, Jacqueline and Kulbach, Cedric and Thoma, Steffen},
-  
-  keywords = {Machine Learning (cs.LG), FOS: Computer and information sciences, FOS: Computer and information sciences},
-  
-  title = {TSInterpret: A unified framework for time series interpretability},
-  
-  publisher = {arXiv},
-  
-  year = {2022},
-  
-  copyright = {Creative Commons Attribution 4.0 International}
-}
+@article{Höllig2023, 
+doi = {10.21105/joss.05220}, 
+url = {https://doi.org/10.21105/joss.05220}, 
+year = {2023}, 
+publisher = {The Open Journal}, 
+volume = {8}, 
+number = {85}, 
+pages = {5220}, 
+author = {Jacqueline Höllig and Cedric Kulbach and Steffen Thoma}, 
+title = {TSInterpret: A Python Package for the Interpretability of Time Series Classification}, journal = {Journal of Open Source Software} } 
 ```
```

#### html2text {}

```diff
@@ -1,45 +1,51 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.3 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.4 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.6.0 Description-Content-Type: text/
 markdown Provides-Extra: dev Provides-Extra: test Provides-Extra: docs
 Provides-Extra: all License-File: LICENSE
                               [TSInterpret Logo]
     [tests] [PyPI] [https://codecov.io/gh/fzi-forschungszentrum-informatik/
  TSInterpret/branch/main/graph/badge.svg?token=1IGZKTLZ4J] [PyPI - Downloads]
-                                   [GitHub]
+                             [GitHub] [DOI_badge]
 TSInterpret is a Python library for interpreting time series classification.
 The ambition is to faciliate the usage of time series interpretability methods.
 The Framework supports Sklearn, Tensorflow, Torch and in some cases predict
 functions. A listing of implemented algorithms and supported frameworks can be
 found in our Documentation. More information on our framework can be found in
 our
 paper
 ._##_ð_Installation_```shell_pip_install_TSInterpret_```_You_can_install_the
 latest_development_version_from_GitHub_as_so:_```shell_pip_install_https://
 github.com/fzi-forschungszentrum-informatik/TSInterpret.git_--upgrade_```_Or,
 through_SSH:_```shell_pip_install_git@github.com:fzi-forschungszentrum-
-informatik/TSInterpret.git_--upgrade_```_##_ð«_Quickstart_The_following
-example_creates_a_simple_Neural_Network_based_on_tensorflow_and_interprets_the
-Classfier_with_Integrated_Gradients_and_Temporal_Saliency_Rescaling_[1]._For
-further_examples_check_out_the_Documentation._[1]_Ismail,_Aya_Abdelsalam,_et
-al._"Benchmarking_deep_learning_interpretability_in_time_series_predictions."
-Advances_in_neural_information_processing_systems_33_(2020):_6441-6452._###
-Import_```python_import_pickle_import_numpy_as_np_import_matplotlib.pyplot_as
-plt_import_seaborn_as_snst_from_tslearn.datasets_import_UCR_UEA_datasets_import
-tensorflow_as_tf_```_###_Create_Classifcation_Model_This_Section_uses_a
-pretrained_Classification_Model_to_illustrate_the_use_of_our_package._For
-running_the_example,_please_clone_our_repository_and_comment_the_variable
+informatik/TSInterpret.git_--upgrade_```_On_Windows_with_Anaconda_there_is_a
+known_installation_issue_due_to_the_sklearn_brownout_in_third_party
+dependencies._The_workaround_(working_for_python_3.9)_till_all_the_dependencies
+are_fixed:_1._Set_Enviroment_Variable_```shell_set
+SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=True_```_2._Install_sklearn_in
+advance_```shell_pip_install_sklearn=0.0_```_3._Install_TsIntrerpret_```shell
+pip_install_TSInterpret_```_##_ð«_Quickstart_The_following_example_creates_a
+simple_Neural_Network_based_on_tensorflow_and_interprets_the_Classfier_with
+Integrated_Gradients_and_Temporal_Saliency_Rescaling_[1]._For_further_examples
+check_out_the_Documentation._[1]_Ismail,_Aya_Abdelsalam,_et_al._"Benchmarking
+deep_learning_interpretability_in_time_series_predictions."_Advances_in_neural
+information_processing_systems_33_(2020):_6441-6452._###_Import_```python
+import_pickle_import_numpy_as_np_import_matplotlib.pyplot_as_plt_import_seaborn
+as_snst_from_tslearn.datasets_import_UCR_UEA_datasets_import_tensorflow_as_tf
+```_###_Create_Classifcation_Model_This_Section_uses_a_pretrained
+Classification_Model_to_illustrate_the_use_of_our_package._For_running_the
+example,_please_clone_our_repository_and_comment_the_variable
 PATH_TO_YOUR_CLASSIFICATION_MODEL_in._The_code_in_this_section_can_also_be
 replaces_with_your_personal_classification_model_written_in_torch_or
 tensorflow._```python_#_Load_data._dataset='BasicMotions'_train_x,train_y,
 test_x,_test_y=UCR_UEA_datasets().load_dataset(dataset)
 enc1=sklearn.OneHotEncoder(sparse=False).fit(train_y.reshape(-1,1))
 train_y=enc1.transform(train_y.reshape(-1,1))_test_y=enc1.transform
 (test_y.reshape(-1,1))_#_Load_a_model._#e.g.,
@@ -75,14 +81,13 @@
 informatik/TSInterpret/issues/new/choose)._-_Before_opening_a_pull_request,_we
 also_encourage_users_to_open_an_issue_for_discussion._Details_on_how_to
 Contribute_can_be_found_[here](https://github.com/fzi-forschungszentrum-
 informatik/TSInterpret/blob/main/CONTRIBUTING.md)._##_ð«_Affiliations
                                   [FZI_Logo]
 ##_Citation_If_you_use_TSInterpret_in_your_research,_please_consider_citing_it
 and_the_authors'_original_papers._The_authors'_original_papers_are_cited_in_the
-documentation_and_the_paper_below._```_@misc{https://doi.org/10.48550/
-arxiv.2208.05280,_doi_=_{10.48550/ARXIV.2208.05280},_url_=_{https://arxiv.org/
-abs/2208.05280},_author_=_{HÃ¶llig,_Jacqueline_and_Kulbach,_Cedric_and_Thoma,
-Steffen},_keywords_=_{Machine_Learning_(cs.LG),_FOS:_Computer_and_information
-sciences,_FOS:_Computer_and_information_sciences},_title_=_{TSInterpret:_A
-unified_framework_for_time_series_interpretability},_publisher_=_{arXiv},_year
-=_{2022},_copyright_=_{Creative_Commons_Attribution_4.0_International}_}_```
+documentation_and_the_paper_below._```_@article{HÃ¶llig2023,_doi_=_{10.21105/
+joss.05220},_url_=_{https://doi.org/10.21105/joss.05220},_year_=_{2023},
+publisher_=_{The_Open_Journal},_volume_=_{8},_number_=_{85},_pages_=_{5220},
+author_=_{Jacqueline_HÃ¶llig_and_Cedric_Kulbach_and_Steffen_Thoma},_title_=
+{TSInterpret:_A_Python_Package_for_the_Interpretability_of_Time_Series
+Classification},_journal_=_{Journal_of_Open_Source_Software}_}_```
```

### Comparing `TSInterpret-0.2.3/TSInterpret.egg-info/SOURCES.txt` & `TSInterpret-0.2.4/TSInterpret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/TSInterpret.egg-info/requires.txt` & `TSInterpret-0.2.4/TSInterpret.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.3/setup.py` & `TSInterpret-0.2.4/setup.py`

 * *Files identical despite different names*

