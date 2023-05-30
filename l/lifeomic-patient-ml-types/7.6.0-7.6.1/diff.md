# Comparing `tmp/lifeomic_patient_ml_types-7.6.0.tar.gz` & `tmp/lifeomic_patient_ml_types-7.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeomic_patient_ml_types-7.6.0.tar", max compression
+gzip compressed data, was "lifeomic_patient_ml_types-7.6.1.tar", max compression
```

## Comparing `lifeomic_patient_ml_types-7.6.0.tar` & `lifeomic_patient_ml_types-7.6.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    14300 2023-05-30 15:17:55.675490 lifeomic_patient_ml_types-7.6.0/lifeomic_patient_ml_types/schemas.py
--rw-r--r--   0        0        0      664 2023-05-30 15:19:10.623242 lifeomic_patient_ml_types-7.6.0/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.6.0/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.6.0/PKG-INFO
+-rw-r--r--   0        0        0    14545 2023-05-30 17:37:25.675744 lifeomic_patient_ml_types-7.6.1/lifeomic_patient_ml_types/schemas.py
+-rw-r--r--   0        0        0      664 2023-05-30 17:38:45.752365 lifeomic_patient_ml_types-7.6.1/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.6.1/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.6.1/PKG-INFO
```

### Comparing `lifeomic_patient_ml_types-7.6.0/lifeomic_patient_ml_types/schemas.py` & `lifeomic_patient_ml_types-7.6.1/lifeomic_patient_ml_types/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -575,14 +575,18 @@
     True if this run has been archived. Archived runs' related artifacts are deleted, and they can no longer be deployed.
     """
     splits: Optional[RunSplits] = None
     hyperparameters: List[Parameter]
     """
     The hyperparameters used to train the model version created by this run.
     """
+    championId: Optional[str] = None
+    """
+    The ID of the model run that was the current champion while this model run was running. All champion metrics on this model run represent that champion's performance on this run's dataset.
+    """
     metrics: RunMetrics
     approvals: List[ApprovalDecision]
     """
     Decisions made by various actors representing whether they think this model version should be used in production and become the new champion.
     """
     problemDefinition: MlProblemDefinition
     trainingApproach: TrainingApproach
```

### Comparing `lifeomic_patient_ml_types-7.6.0/pyproject.toml` & `lifeomic_patient_ml_types-7.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lifeomic-patient-ml-types"
-version = "7.6.0"
+version = "7.6.1"
 description = "Shared types for the patient-ml-service repos."
 authors = ["LifeOmic <development@lifeomic.com>"]
 license = "UNLICENSED"
 
 [tool.poe.tasks]
 format = "black lifeomic_patient_ml_types"
 lint = "pyright lifeomic_patient_ml_types"
```

### Comparing `lifeomic_patient_ml_types-7.6.0/setup.py` & `lifeomic_patient_ml_types-7.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['lifeomic_patient_ml_types']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'lifeomic-patient-ml-types',
-    'version': '7.6.0',
+    'version': '7.6.1',
     'description': 'Shared types for the patient-ml-service repos.',
     'long_description': 'None',
     'author': 'LifeOmic',
     'author_email': 'development@lifeomic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

