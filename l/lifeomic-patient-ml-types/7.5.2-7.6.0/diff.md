# Comparing `tmp/lifeomic_patient_ml_types-7.5.2.tar.gz` & `tmp/lifeomic_patient_ml_types-7.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeomic_patient_ml_types-7.5.2.tar", max compression
+gzip compressed data, was "lifeomic_patient_ml_types-7.6.0.tar", max compression
```

## Comparing `lifeomic_patient_ml_types-7.5.2.tar` & `lifeomic_patient_ml_types-7.6.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    14150 2023-05-19 21:47:09.063811 lifeomic_patient_ml_types-7.5.2/lifeomic_patient_ml_types/schemas.py
--rw-r--r--   0        0        0      664 2023-05-19 21:48:24.752074 lifeomic_patient_ml_types-7.5.2/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.5.2/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.5.2/PKG-INFO
+-rw-r--r--   0        0        0    14300 2023-05-30 15:17:55.675490 lifeomic_patient_ml_types-7.6.0/lifeomic_patient_ml_types/schemas.py
+-rw-r--r--   0        0        0      664 2023-05-30 15:19:10.623242 lifeomic_patient_ml_types-7.6.0/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.6.0/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.6.0/PKG-INFO
```

### Comparing `lifeomic_patient_ml_types-7.5.2/lifeomic_patient_ml_types/schemas.py` & `lifeomic_patient_ml_types-7.6.0/lifeomic_patient_ml_types/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,15 +519,19 @@
     """
     UUID uniquely identifying this model config.
     """
     accountId: str
     problemDefinition: MlProblemDefinition
     deployedId: Optional[str] = None
     """
-    The ID of the model version currently deployed for this model config.
+    The ID of the model version currently deployed for this model config. (deprecated, use championId instead)
+    """
+    championId: Optional[str] = None
+    """
+    The ID of the champion model run for this model config.
     """
 
 
 class ModelRun(BaseModel):
     class Config:
         extra = Extra.forbid
```

### Comparing `lifeomic_patient_ml_types-7.5.2/pyproject.toml` & `lifeomic_patient_ml_types-7.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lifeomic-patient-ml-types"
-version = "7.5.2"
+version = "7.6.0"
 description = "Shared types for the patient-ml-service repos."
 authors = ["LifeOmic <development@lifeomic.com>"]
 license = "UNLICENSED"
 
 [tool.poe.tasks]
 format = "black lifeomic_patient_ml_types"
 lint = "pyright lifeomic_patient_ml_types"
```

### Comparing `lifeomic_patient_ml_types-7.5.2/setup.py` & `lifeomic_patient_ml_types-7.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['lifeomic_patient_ml_types']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'lifeomic-patient-ml-types',
-    'version': '7.5.2',
+    'version': '7.6.0',
     'description': 'Shared types for the patient-ml-service repos.',
     'long_description': 'None',
     'author': 'LifeOmic',
     'author_email': 'development@lifeomic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

