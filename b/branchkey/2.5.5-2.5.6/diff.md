# Comparing `tmp/branchkey-2.5.5.tar.gz` & `tmp/branchkey-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "branchkey-2.5.5.tar", last modified: Thu Feb 23 13:00:31 2023, max compression
+gzip compressed data, was "branchkey-2.5.6.tar", last modified: Tue May 30 11:02:28 2023, max compression
```

## Comparing `branchkey-2.5.5.tar` & `branchkey-2.5.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 13:00:31.857914 branchkey-2.5.5/
--rw-r--r--   0 root         (0) root         (0)     4803 2023-02-23 13:00:31.857914 branchkey-2.5.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4271 2023-02-23 13:00:19.000000 branchkey-2.5.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-02-07 14:31:52.000000 branchkey-2.5.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 13:00:31.857914 branchkey-2.5.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-02-23 13:00:30.000000 branchkey-2.5.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 13:00:31.853915 branchkey-2.5.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 13:00:31.857914 branchkey-2.5.5/src/branchkey/
--rw-rw-rw-   0 root         (0) root         (0)     5125 2023-02-23 13:00:19.000000 branchkey-2.5.5/src/branchkey/__consumer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-07 14:31:52.000000 branchkey-2.5.5/src/branchkey/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10142 2023-02-23 13:00:19.000000 branchkey-2.5.5/src/branchkey/client.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-02-07 14:31:52.000000 branchkey-2.5.5/src/branchkey/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 13:00:31.857914 branchkey-2.5.5/src/branchkey.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4803 2023-02-23 13:00:31.000000 branchkey-2.5.5/src/branchkey.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2023-02-23 13:00:31.000000 branchkey-2.5.5/src/branchkey.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 13:00:31.000000 branchkey-2.5.5/src/branchkey.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-02-23 13:00:31.000000 branchkey-2.5.5/src/branchkey.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-02-23 13:00:31.000000 branchkey-2.5.5/src/branchkey.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:02:28.402993 branchkey-2.5.6/
+-rw-r--r--   0 root         (0) root         (0)     5342 2023-05-30 11:02:28.402993 branchkey-2.5.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4810 2023-05-25 09:40:36.000000 branchkey-2.5.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-05-25 09:40:36.000000 branchkey-2.5.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 11:02:28.402993 branchkey-2.5.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-05-30 11:02:27.000000 branchkey-2.5.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:02:28.402993 branchkey-2.5.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:02:28.402993 branchkey-2.5.6/src/branchkey/
+-rw-rw-rw-   0 root         (0) root         (0)     5125 2023-05-25 09:40:36.000000 branchkey-2.5.6/src/branchkey/__consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 09:40:36.000000 branchkey-2.5.6/src/branchkey/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10685 2023-05-30 11:02:16.000000 branchkey-2.5.6/src/branchkey/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-05-25 09:40:36.000000 branchkey-2.5.6/src/branchkey/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:02:28.402993 branchkey-2.5.6/src/branchkey.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5342 2023-05-30 11:02:28.000000 branchkey-2.5.6/src/branchkey.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2023-05-30 11:02:28.000000 branchkey-2.5.6/src/branchkey.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 11:02:28.000000 branchkey-2.5.6/src/branchkey.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-30 11:02:28.000000 branchkey-2.5.6/src/branchkey.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-30 11:02:28.000000 branchkey-2.5.6/src/branchkey.egg-info/top_level.txt
```

### Comparing `branchkey-2.5.5/PKG-INFO` & `branchkey-2.5.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: branchkey
-Version: 2.5.5
+Version: 2.5.6
 Summary: Client application to interface with the BranchKey system
 Home-page: https://branchkey.com
 Author: BranchKey
 Author-email: info@branchkey.com
 Project-URL: Homepage, https://branchkey.com
 Project-URL: Repository, https://gitlab.com/branchkey/client_application
 Classifier: Programming Language :: Python :: 3
@@ -47,31 +47,48 @@
                  "leaf_session_token": "46780841-9787-41e6-ac14-e3ee160e158a",
                  "performance_analyser_username": "hello",
                  "performance_analyser_password": "world",
                  "response_host":"response.branchkey.com"}
 
   host = "http://api.branchkey.com"
 
-  # initialise the client
-  # it implicitly authenticates the leaf_session
-  # and fetches the run_details of the parent branch
-  c = Client(credentials,host)
-
-  # upload the file to the system
+  '''initialise the client
+  it implicitly authenticates the leaf_session
+  and fetches the run_details of the parent branch
+
+  ssl: Whether to verify the SSL certificates of the remote host or not
+
+  wait_for_run: When trying to upload file, if the
+  run is stopped/paused, this parameter decides whether
+  to throw exception and stop the process, or wait for
+  the run to be started again. Default is False
+
+  run_check_interval_s: if wait_for_run=True, this
+  parameter decides the sleeping interval of the
+  program until the run status is checked again.
+  Default is 30 seconds
+  '''
+  c = Client(credentials,host, ssl=False,wait_for_run=True, run_check_interval_s=15)
+
+  '''
+  upload the file to the system
+  '''
   c.file_upload("./file/path.npy")
 
-  # Download a file with the file_id value
-  # same as the one received from the consumer
-  # It downloads the files in the ./aggregated_files directory
+  '''Download a file with the file_id value
+  same as the one received from the consumer
+  It downloads the files in the ./aggregated_files directory
+  '''
   if not c.queue.empty():
         aggregation_id = c.queue.get(block=False)
         c.file_download(aggregation_id)
 
-        # To push performance analysis metrics for this aggregation:
-        # mode can be test, train or non-federated
+        '''To push performance analysis metrics for this aggregation:
+        mode can be test, train or non-federated
+        '''
         data = json.dumps({"key1":"val1","key2":"val2"})
         mode = "test"
         c.send_performance_metrics(aggregation_id, data, mode)
   ```
 
 ## File format
```

### Comparing `branchkey-2.5.5/README.md` & `branchkey-2.5.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -32,31 +32,48 @@
                  "leaf_session_token": "46780841-9787-41e6-ac14-e3ee160e158a",
                  "performance_analyser_username": "hello",
                  "performance_analyser_password": "world",
                  "response_host":"response.branchkey.com"}
 
   host = "http://api.branchkey.com"
 
-  # initialise the client
-  # it implicitly authenticates the leaf_session
-  # and fetches the run_details of the parent branch
-  c = Client(credentials,host)
-
-  # upload the file to the system
+  '''initialise the client
+  it implicitly authenticates the leaf_session
+  and fetches the run_details of the parent branch
+
+  ssl: Whether to verify the SSL certificates of the remote host or not
+
+  wait_for_run: When trying to upload file, if the
+  run is stopped/paused, this parameter decides whether
+  to throw exception and stop the process, or wait for
+  the run to be started again. Default is False
+
+  run_check_interval_s: if wait_for_run=True, this
+  parameter decides the sleeping interval of the
+  program until the run status is checked again.
+  Default is 30 seconds
+  '''
+  c = Client(credentials,host, ssl=False,wait_for_run=True, run_check_interval_s=15)
+
+  '''
+  upload the file to the system
+  '''
   c.file_upload("./file/path.npy")
 
-  # Download a file with the file_id value
-  # same as the one received from the consumer
-  # It downloads the files in the ./aggregated_files directory
+  '''Download a file with the file_id value
+  same as the one received from the consumer
+  It downloads the files in the ./aggregated_files directory
+  '''
   if not c.queue.empty():
         aggregation_id = c.queue.get(block=False)
         c.file_download(aggregation_id)
 
-        # To push performance analysis metrics for this aggregation:
-        # mode can be test, train or non-federated
+        '''To push performance analysis metrics for this aggregation:
+        mode can be test, train or non-federated
+        '''
         data = json.dumps({"key1":"val1","key2":"val2"})
         mode = "test"
         c.send_performance_metrics(aggregation_id, data, mode)
   ```
 
 ## File format
```

### Comparing `branchkey-2.5.5/setup.py` & `branchkey-2.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open(os.path.join(current_directory, "README.md"), encoding="utf-8") as f:
         long_description = f.read()
 except Exception:
     long_description = ""
 
 setuptools.setup(
     name="branchkey",
-    version="2.5.5",
+    version="2.5.6",
     author="BranchKey",
     author_email="info@branchkey.com",
     description="Client application to interface with the BranchKey system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://branchkey.com",
     project_urls={
```

### Comparing `branchkey-2.5.5/src/branchkey/__consumer.py` & `branchkey-2.5.6/src/branchkey/__consumer.py`

 * *Files identical despite different names*

### Comparing `branchkey-2.5.5/src/branchkey/client.py` & `branchkey-2.5.6/src/branchkey/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import json
 import logging
 import os
 import warnings
 from http import HTTPStatus
 from queue import Queue
+from time import sleep
 
 import numpy as np
 import requests
 
 from .__consumer import Consumer
 from .utils import AGGREGATED_OUTPUT_DIR, FILE_METADATA
 
 
 class Client:
     def __init__(self,
                  credentials: dict = None,
-                 host: str = "https://api.branchkey.com", ssl: bool = False):
+                 host: str = "https://api.branchkey.com",
+                 ssl: bool = False, wait_for_run: bool = False, run_check_interval_s: int = 30):
 
         if credentials is None:
             credentials = dict(leaf_name="guest", leaf_id="guest", leaf_session_token="guest",
                                response_host="response.branchkey.com", port=5672)
 
         self.__leaf_name = credentials["leaf_name"]
         self.__leaf_id = credentials["leaf_id"]
@@ -34,14 +36,16 @@
         self.__api_host = host
         # Verify SSL certs
         self.__verify = ssl
 
         self.queue = Queue()
         self.__run_status = None
         self.__run_number = None
+        self.__wait_for_run = wait_for_run
+        self.__run_check_interval_s = run_check_interval_s
 
         self.rabbit_credentials = dict(
             leaf_name=self.__leaf_name, leaf_id=self.__leaf_id, queue_password=self.__leaf_session_token, host=credentials["response_host"])
         self.consumer = None
 
         self.__authenticate()
         self.get_run_details()
@@ -147,15 +151,21 @@
         else:
             file.seek(0)
             return True
 
     def file_upload(self, file_path):
         try:
             if self.__run_status != "start":
-                raise Exception("run is blocked")
+                if self.__wait_for_run:
+                    while self.__run_status != "start":
+                        print(
+                            f"run is blocked, going into sleep for {self.__run_check_interval_s} seconds before checking again")
+                        sleep(self.__run_check_interval_s)
+                else:
+                    raise Exception("run is blocked")
 
             with open(file_path, mode="rb") as f:
                 self.validate_weight_shape(f)
 
                 url = self.__api_host + "/v1/file/upload"
                 headers = {"accept": "application/json"}
                 data = {"data": json.dumps({"leaf_name": self.__leaf_name,
```

### Comparing `branchkey-2.5.5/src/branchkey.egg-info/PKG-INFO` & `branchkey-2.5.6/src/branchkey.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: branchkey
-Version: 2.5.5
+Version: 2.5.6
 Summary: Client application to interface with the BranchKey system
 Home-page: https://branchkey.com
 Author: BranchKey
 Author-email: info@branchkey.com
 Project-URL: Homepage, https://branchkey.com
 Project-URL: Repository, https://gitlab.com/branchkey/client_application
 Classifier: Programming Language :: Python :: 3
@@ -47,31 +47,48 @@
                  "leaf_session_token": "46780841-9787-41e6-ac14-e3ee160e158a",
                  "performance_analyser_username": "hello",
                  "performance_analyser_password": "world",
                  "response_host":"response.branchkey.com"}
 
   host = "http://api.branchkey.com"
 
-  # initialise the client
-  # it implicitly authenticates the leaf_session
-  # and fetches the run_details of the parent branch
-  c = Client(credentials,host)
-
-  # upload the file to the system
+  '''initialise the client
+  it implicitly authenticates the leaf_session
+  and fetches the run_details of the parent branch
+
+  ssl: Whether to verify the SSL certificates of the remote host or not
+
+  wait_for_run: When trying to upload file, if the
+  run is stopped/paused, this parameter decides whether
+  to throw exception and stop the process, or wait for
+  the run to be started again. Default is False
+
+  run_check_interval_s: if wait_for_run=True, this
+  parameter decides the sleeping interval of the
+  program until the run status is checked again.
+  Default is 30 seconds
+  '''
+  c = Client(credentials,host, ssl=False,wait_for_run=True, run_check_interval_s=15)
+
+  '''
+  upload the file to the system
+  '''
   c.file_upload("./file/path.npy")
 
-  # Download a file with the file_id value
-  # same as the one received from the consumer
-  # It downloads the files in the ./aggregated_files directory
+  '''Download a file with the file_id value
+  same as the one received from the consumer
+  It downloads the files in the ./aggregated_files directory
+  '''
   if not c.queue.empty():
         aggregation_id = c.queue.get(block=False)
         c.file_download(aggregation_id)
 
-        # To push performance analysis metrics for this aggregation:
-        # mode can be test, train or non-federated
+        '''To push performance analysis metrics for this aggregation:
+        mode can be test, train or non-federated
+        '''
         data = json.dumps({"key1":"val1","key2":"val2"})
         mode = "test"
         c.send_performance_metrics(aggregation_id, data, mode)
   ```
 
 ## File format
```

