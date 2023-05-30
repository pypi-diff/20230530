# Comparing `tmp/gad_common_utils-0.22.tar.gz` & `tmp/gad_common_utils-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gad_common_utils-0.22.tar", last modified: Thu May  4 13:02:20 2023, max compression
+gzip compressed data, was "gad_common_utils-0.23.tar", last modified: Tue May 30 14:23:53 2023, max compression
```

## Comparing `gad_common_utils-0.22.tar` & `gad_common_utils-0.23.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:20.449598 gad_common_utils-0.22/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:20.445598 gad_common_utils-0.22/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:20.445598 gad_common_utils-0.22/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-04 13:02:10.000000 gad_common_utils-0.22/.github/workflows/black-format-checker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 13:02:10.000000 gad_common_utils-0.22/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-04 13:02:10.000000 gad_common_utils-0.22/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 13:02:10.000000 gad_common_utils-0.22/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-04 13:02:10.000000 gad_common_utils-0.22/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-04 13:02:20.449598 gad_common_utils-0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-04 13:02:10.000000 gad_common_utils-0.22/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:20.449598 gad_common_utils-0.22/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-04 13:02:20.000000 gad_common_utils-0.22/common_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/data_loading_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/data_type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/date_time_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/dynamodb_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/dynamodb_ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/files_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/gad_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/gad_utils_additionals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/json_schema_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/run_athena_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/s3_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/sql_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/string_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:20.449598 gad_common_utils-0.22/gad_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-04 13:02:20.000000 gad_common_utils-0.22/gad_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-04 13:02:20.000000 gad_common_utils-0.22/gad_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:02:20.000000 gad_common_utils-0.22/gad_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 13:02:20.000000 gad_common_utils-0.22/gad_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 13:02:20.000000 gad_common_utils-0.22/gad_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-04 13:02:10.000000 gad_common_utils-0.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:02:20.449598 gad_common_utils-0.22/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:20.449598 gad_common_utils-0.22/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:10.000000 gad_common_utils-0.22/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-04 13:02:10.000000 gad_common_utils-0.22/tests/test_json_schema_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:23:53.164129 gad_common_utils-0.23/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:23:53.160129 gad_common_utils-0.23/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:23:53.160129 gad_common_utils-0.23/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-30 14:23:43.000000 gad_common_utils-0.23/.github/workflows/black-format-checker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-30 14:23:43.000000 gad_common_utils-0.23/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-30 14:23:43.000000 gad_common_utils-0.23/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 14:23:43.000000 gad_common_utils-0.23/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-30 14:23:43.000000 gad_common_utils-0.23/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-30 14:23:53.164129 gad_common_utils-0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-30 14:23:43.000000 gad_common_utils-0.23/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:23:53.164129 gad_common_utils-0.23/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-30 14:23:53.000000 gad_common_utils-0.23/common_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/data_loading_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/data_type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/date_time_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/dynamodb_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/dynamodb_ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/files_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/gad_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/gad_utils_additionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/json_schema_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/run_athena_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/s3_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/sql_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-30 14:23:43.000000 gad_common_utils-0.23/common_utils/string_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:23:53.164129 gad_common_utils-0.23/gad_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-30 14:23:53.000000 gad_common_utils-0.23/gad_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-30 14:23:53.000000 gad_common_utils-0.23/gad_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:23:53.000000 gad_common_utils-0.23/gad_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 14:23:53.000000 gad_common_utils-0.23/gad_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 14:23:53.000000 gad_common_utils-0.23/gad_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-30 14:23:43.000000 gad_common_utils-0.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:23:53.164129 gad_common_utils-0.23/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:23:53.164129 gad_common_utils-0.23/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:23:43.000000 gad_common_utils-0.23/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-30 14:23:43.000000 gad_common_utils-0.23/tests/test_json_schema_methods.py
```

### Comparing `gad_common_utils-0.22/.github/workflows/black-format-checker.yml` & `gad_common_utils-0.23/.github/workflows/black-format-checker.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/.github/workflows/publish-to-pypi.yml` & `gad_common_utils-0.23/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/.github/workflows/pytest.yml` & `gad_common_utils-0.23/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/PKG-INFO` & `gad_common_utils-0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gad_common_utils
-Version: 0.22
+Version: 0.23
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.22/common_utils/data_loading_management.py` & `gad_common_utils-0.23/common_utils/data_loading_management.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/common_utils/data_type_conversion.py` & `gad_common_utils-0.23/common_utils/data_type_conversion.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/common_utils/date_time_methods.py` & `gad_common_utils-0.23/common_utils/date_time_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/common_utils/dynamodb_methods.py` & `gad_common_utils-0.23/common_utils/dynamodb_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/common_utils/files_methods.py` & `gad_common_utils-0.23/common_utils/files_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/common_utils/gad_utils.py` & `gad_common_utils-0.23/common_utils/gad_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 from airflow import DAG
 from airflow.contrib.operators.kubernetes_pod_operator import KubernetesPodOperator
 from airflow.operators.python_operator import PythonOperator
 from airflow.utils.dates import days_ago
 from kubernetes.client import models as k8s
 
 
-def return_dag_ingrediants(project):
+def return_dag_ingrediants(content_path, project):
     """
     This function returns a tuple that contains various objects used in an Airflow DAG
     for the specified project.
 
     Parameters:
+        content_path (str): The path of the content we want to run via DAG.
         project (str): The name of the project for which to return the DAG ingredients.
 
     Returns:
         tuple: A tuple containing the following objects:
             - paths (dict): A dictionary that maps path-related variables to their respective names.
             - default_args (dict): A dictionary that specifies default arguments for the DAG.
             - envFromSource (k8s.V1EnvFromSource): An object that specifies the ConfigMap to use as a source of environment variables.
             - volumes (list): A list of V1Volume objects that specify the volumes to mount in the Kubernetes Pod.
             - volumes_mounts (list): A list of V1VolumeMount objects that specify the volume mounts to use in the Kubernetes Pod.
     """
     WORK_DIR = "/opt/aiola/projects"
-    SUB_FOLDER = os.environ.get("DEPLOYMENT_DIR", "gad-deliveries")
+    SUB_FOLDER = os.environ.get("DEPLOYMENT_DIR", content_path)
     PROJECT_DIR = f"{WORK_DIR}/{SUB_FOLDER}/{project}"
     DBT_OUTPUT_DIR = "/opt/airflow/logs"
     PYTHON_DIR = f"{PROJECT_DIR}/python"
     DBT_DIR = f"{PROJECT_DIR}/dbt"
     CONFIG_DIR = f"{PROJECT_DIR}/configuration"
 
     paths = {
@@ -69,30 +70,37 @@
 
     volumes = [volume]
     volumes_mounts = [volume_mount]
 
     return paths, default_args, envFromSource, volumes, volumes_mounts
 
 
-def generate_airflow_dag(project: str, dag_id: str, schedule_interval, tasks: list):
+def generate_airflow_dag(
+    project: str,
+    dag_id: str,
+    schedule_interval,
+    tasks: list,
+    content_path: str = "gad-deliveries",
+):
     """
     Creates a DAG using the specified parameters.
 
     Args:
         project (str): The name of the project.
         dag_id (str): The ID of the DAG.
         schedule_interval (str): The schedule interval for the DAG.
         tasks (list): A list of dictionaries containing information about each task.
+        content_path (str): The path of the content we want to run via DAG. by default it would get "gad-deliveries" as its the local content.
 
     Returns:
         dag (DAG): A DAG object.
     """
 
     paths, default_args, envConfigMap, volumes, volumes_mounts = return_dag_ingrediants(
-        project
+        content_path, project
     )
 
     def return_image_name(task_type):
         """
         Returns the image name based on the task type.
 
         Parameters:
```

### Comparing `gad_common_utils-0.22/common_utils/gad_utils_additionals.py` & `gad_common_utils-0.23/common_utils/gad_utils_additionals.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/common_utils/json_schema_methods.py` & `gad_common_utils-0.23/common_utils/json_schema_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/common_utils/run_athena_query.py` & `gad_common_utils-0.23/common_utils/run_athena_query.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/common_utils/s3_methods.py` & `gad_common_utils-0.23/common_utils/s3_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/common_utils/sql_methods.py` & `gad_common_utils-0.23/common_utils/sql_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/common_utils/string_transformations.py` & `gad_common_utils-0.23/common_utils/string_transformations.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/gad_common_utils.egg-info/PKG-INFO` & `gad_common_utils-0.23/gad_common_utils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gad-common-utils
-Version: 0.22
+Version: 0.23
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.22/gad_common_utils.egg-info/SOURCES.txt` & `gad_common_utils-0.23/gad_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/pyproject.toml` & `gad_common_utils-0.23/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.22/tests/test_json_schema_methods.py` & `gad_common_utils-0.23/tests/test_json_schema_methods.py`

 * *Files identical despite different names*

