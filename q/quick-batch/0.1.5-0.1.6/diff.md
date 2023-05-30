# Comparing `tmp/quick_batch-0.1.5.tar.gz` & `tmp/quick_batch-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_batch-0.1.5.tar", max compression
+gzip compressed data, was "quick_batch-0.1.6.tar", max compression
```

## Comparing `quick_batch-0.1.5.tar` & `quick_batch-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0     3843 2023-05-25 23:05:55.292224 quick_batch-0.1.5/README.md
--rw-r--r--   0        0        0      686 2023-05-25 23:05:55.292224 quick_batch-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      120 2023-05-25 23:05:55.292224 quick_batch-0.1.5/quick_batch/__init__.py
--rw-r--r--   0        0        0      906 2023-05-25 23:05:55.292224 quick_batch-0.1.5/quick_batch/main.py
--rwxr-xr-x   0        0        0     1215 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/processor_app/processor_app/__init__.py
--rwxr-xr-x   0        0        0     1747 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/processor_app/processor_app/activate_process.py
--rwxr-xr-x   0        0        0     2234 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/processor_app/processor_app/api_connects.py
--rwxr-xr-x   0        0        0      409 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/processor_app/processor_app/run.py
--rwxr-xr-x   0        0        0     5224 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/processor_app/wait-for-it.sh
--rw-r--r--   0        0        0      241 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/Dockerfile
--rw-r--r--   0        0        0     1220 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/queue_app/__init__.py
--rw-r--r--   0        0        0     2312 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/queue_app/apis.py
--rw-r--r--   0        0        0     3250 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/queue_app/queues_init.py
--rw-r--r--   0        0        0      424 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/queue_app/run.py
--rwxr-xr-x   0        0        0       21 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/requirements.txt
--rwxr-xr-x   0        0        0     5224 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/queue_app/wait-for-it.sh
--rw-r--r--   0        0        0      551 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/__init__.py
--rw-r--r--   0        0        0     2088 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_containers.py
--rw-r--r--   0        0        0     1244 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_dockerfile.py
--rw-r--r--   0        0        0     4624 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_images.py
--rw-r--r--   0        0        0     1951 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_loggers.py
--rw-r--r--   0        0        0      551 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_networks.py
--rw-r--r--   0        0        0     2487 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_queue.py
--rw-r--r--   0        0        0     2033 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_requirements.py
--rw-r--r--   0        0        0     4722 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_services.py
--rw-r--r--   0        0        0     3201 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_setup.py
--rw-r--r--   0        0        0      229 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/manage_swarm.py
--rw-r--r--   0        0        0     4429 2023-05-25 23:05:55.296224 quick_batch-0.1.5/quick_batch/utilities/param_checks.py
--rw-r--r--   0        0        0     4566 1970-01-01 00:00:00.000000 quick_batch-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3734 2023-05-30 16:09:01.056282 quick_batch-0.1.6/README.md
+-rw-r--r--   0        0        0      729 2023-05-30 16:09:01.056282 quick_batch-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/__init__.py
+-rw-r--r--   0        0        0      906 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/main.py
+-rw-r--r--   0        0        0     1037 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/manual_scaler.py
+-rwxr-xr-x   0        0        0     1215 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/processor_app/processor_app/__init__.py
+-rwxr-xr-x   0        0        0     1747 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/processor_app/processor_app/activate_process.py
+-rwxr-xr-x   0        0        0     2234 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/processor_app/processor_app/api_connects.py
+-rwxr-xr-x   0        0        0      409 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/processor_app/processor_app/run.py
+-rwxr-xr-x   0        0        0     5224 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/processor_app/wait-for-it.sh
+-rw-r--r--   0        0        0      241 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/Dockerfile
+-rw-r--r--   0        0        0     1220 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/queue_app/__init__.py
+-rw-r--r--   0        0        0     2312 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/queue_app/apis.py
+-rw-r--r--   0        0        0     3250 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/queue_app/queues_init.py
+-rw-r--r--   0        0        0      424 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/queue_app/run.py
+-rwxr-xr-x   0        0        0       21 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/requirements.txt
+-rwxr-xr-x   0        0        0     5224 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/queue_app/wait-for-it.sh
+-rw-r--r--   0        0        0      551 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/utilities/__init__.py
+-rw-r--r--   0        0        0      146 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/utilities/manage_client.py
+-rw-r--r--   0        0        0     2088 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/utilities/manage_containers.py
+-rw-r--r--   0        0        0     1244 2023-05-30 16:09:01.056282 quick_batch-0.1.6/quick_batch/utilities/manage_dockerfile.py
+-rw-r--r--   0        0        0     4624 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_images.py
+-rw-r--r--   0        0        0     1951 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_loggers.py
+-rw-r--r--   0        0        0      551 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_networks.py
+-rw-r--r--   0        0        0     2487 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_queue.py
+-rw-r--r--   0        0        0     2033 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_requirements.py
+-rw-r--r--   0        0        0     4722 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_services.py
+-rw-r--r--   0        0        0     3115 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_setup.py
+-rw-r--r--   0        0        0      229 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/manage_swarm.py
+-rw-r--r--   0        0        0     4429 2023-05-30 16:09:01.060282 quick_batch-0.1.6/quick_batch/utilities/param_checks.py
+-rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 quick_batch-0.1.6/PKG-INFO
```

### Comparing `quick_batch-0.1.5/README.md` & `quick_batch-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # Getting started
 
 All you need to scale batch transformations with `quick_batch` is a
 
 - transformation function(s) in a `processor.py` file
 - `Dockerfile` containing a container build appropriate to y our processor
 - an optional `requirements.txt` file containing required python modules
-  - custom `requirements.txt` require `flask`, `requests`, and `pyyaml`
 
 Document paths to these objects as well as other parameters in a `config.yaml` config file of the form below
 
 
 ```yaml
 data:
   input_path: /path/to/your/input/data
@@ -32,15 +31,14 @@
   log_path: /path/to/your/log/file
 
 queue:
   feed_rate: <int - number of examples processed per processor instance>
   order_files: <boolean - whether or not to order input files by size>
 
 processor:
-  image_name: <pre-built-image-name>
   dockerfile_path: /path/to/your/Dockerfile
   requirements_path: /path/to/your/requirements.txt
   processor_path: /path/to/your/processor/processor.py
   num_processors: <int - instances of processor to run in parallel>
 
 ```
```

### Comparing `quick_batch-0.1.5/pyproject.toml` & `quick_batch-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "quick_batch"
-version = "0.1.5"
+version = "0.1.6"
 description = "ultra simple command line tool for docker-scaling batch processing"
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jermwatt/quick_batch"
 license = "MIT"
 
 [tool.poetry.scripts]
 quick_batch = "quick_batch.main:main"
-
+qb_scale = "quick_batch.manual_scaler:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docker = "^6.1.2"
 fire = "^0.5.0"
 pyyaml = "<5.5"
 dockerfile-parse = "^2.0.0"
```

### Comparing `quick_batch-0.1.5/quick_batch/main.py` & `quick_batch-0.1.6/quick_batch/main.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/processor_app/processor_app/__init__.py` & `quick_batch-0.1.6/quick_batch/processor_app/processor_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/processor_app/processor_app/activate_process.py` & `quick_batch-0.1.6/quick_batch/processor_app/processor_app/activate_process.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/processor_app/processor_app/api_connects.py` & `quick_batch-0.1.6/quick_batch/processor_app/processor_app/api_connects.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/processor_app/wait-for-it.sh` & `quick_batch-0.1.6/quick_batch/processor_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/queue_app/queue_app/__init__.py` & `quick_batch-0.1.6/quick_batch/queue_app/queue_app/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/queue_app/queue_app/apis.py` & `quick_batch-0.1.6/quick_batch/queue_app/queue_app/apis.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/queue_app/queue_app/queues_init.py` & `quick_batch-0.1.6/quick_batch/queue_app/queue_app/queues_init.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/queue_app/wait-for-it.sh` & `quick_batch-0.1.6/quick_batch/queue_app/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/utilities/__init__.py` & `quick_batch-0.1.6/quick_batch/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/utilities/manage_containers.py` & `quick_batch-0.1.6/quick_batch/utilities/manage_containers.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/utilities/manage_dockerfile.py` & `quick_batch-0.1.6/quick_batch/utilities/manage_dockerfile.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/utilities/manage_images.py` & `quick_batch-0.1.6/quick_batch/utilities/manage_images.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/utilities/manage_loggers.py` & `quick_batch-0.1.6/quick_batch/utilities/manage_loggers.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/utilities/manage_networks.py` & `quick_batch-0.1.6/quick_batch/utilities/manage_networks.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/utilities/manage_queue.py` & `quick_batch-0.1.6/quick_batch/utilities/manage_queue.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/utilities/manage_requirements.py` & `quick_batch-0.1.6/quick_batch/utilities/manage_requirements.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/utilities/manage_services.py` & `quick_batch-0.1.6/quick_batch/utilities/manage_services.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/quick_batch/utilities/manage_setup.py` & `quick_batch-0.1.6/quick_batch/utilities/manage_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 import time
 from utilities import log_exceptions
 from utilities import manage_images
+from utilities.manage_client import create_client
 from utilities.param_checks import setup_logger
 from utilities.param_checks import check_config
 from utilities.param_checks import check_config_data_paths
 from utilities.param_checks import check_processor
-from utilities.param_checks import check_dockerfile
 from utilities.manage_containers import remove_all_containers
 from utilities.manage_networks import remove_network
 from utilities.manage_services import remove_all_services
 from utilities.manage_swarm import leave_swarm
 from utilities.manage_swarm import create_swarm
 from utilities.manage_networks import create_network
 from utilities.manage_services import create_queue_service
 from utilities.manage_services import create_processor_service
 from utilities.manage_queue import monitor_queue_app_containers
-from utilities.manage_images import pull_and_tag_image
 
 
 @log_exceptions
 def setup_client(config):
     # setup logger
     logger = setup_logger(config)
 
     # check that input files exist
     check_config(config)
 
     # check config data paths
     input_path, output_path, processor, num_processors, \
-        dockerfile_path, requirements_path, image_name = check_config_data_paths(config)
+        dockerfile_path, requirements_path, image_name =\
+        check_config_data_paths(config)
 
     # check processor
     check_processor(processor)
-    
+
     # check dockerfile - seems to save a copy local to the project - not using for now
     # check_dockerfile(dockerfile_path)
 
     # create docker client
-    client = manage_images.create_client()
+    client = create_client()
 
     # # try to pull and tag image
     # pull_success = pull_and_tag_image(client, 'jermwatt/quick_batch_queue_app', 'quick_batch_queue_app')
-    
+
     # # if not successful, build image
     # if not pull_success:
-        
+
     manage_images.build_queue_image(client)
-    
+
     # # try to pull and tag image
     # pull_success = pull_and_tag_image(client, image_name, 'quick_batch_processor_app')
-    
+
     # # if not successful, build image
     # if not pull_success:
     manage_images.build_processor_image(client,
                                         dockerfile_path,
                                         requirements_path,
                                         processor)
```

### Comparing `quick_batch-0.1.5/quick_batch/utilities/param_checks.py` & `quick_batch-0.1.6/quick_batch/utilities/param_checks.py`

 * *Files identical despite different names*

### Comparing `quick_batch-0.1.5/PKG-INFO` & `quick_batch-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-batch
-Version: 0.1.5
+Version: 0.1.6
 Summary: ultra simple command line tool for docker-scaling batch processing
 Home-page: https://github.com/jermwatt/quick_batch
 License: MIT
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -36,15 +36,14 @@
 # Getting started
 
 All you need to scale batch transformations with `quick_batch` is a
 
 - transformation function(s) in a `processor.py` file
 - `Dockerfile` containing a container build appropriate to y our processor
 - an optional `requirements.txt` file containing required python modules
-  - custom `requirements.txt` require `flask`, `requests`, and `pyyaml`
 
 Document paths to these objects as well as other parameters in a `config.yaml` config file of the form below
 
 
 ```yaml
 data:
   input_path: /path/to/your/input/data
@@ -52,15 +51,14 @@
   log_path: /path/to/your/log/file
 
 queue:
   feed_rate: <int - number of examples processed per processor instance>
   order_files: <boolean - whether or not to order input files by size>
 
 processor:
-  image_name: <pre-built-image-name>
   dockerfile_path: /path/to/your/Dockerfile
   requirements_path: /path/to/your/requirements.txt
   processor_path: /path/to/your/processor/processor.py
   num_processors: <int - instances of processor to run in parallel>
 
 ```
```

