# Comparing `tmp/cohere-sagemaker-0.6.2.tar.gz` & `tmp/cohere-sagemaker-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-sagemaker-0.6.2.tar", last modified: Tue May  9 20:53:50 2023, max compression
+gzip compressed data, was "cohere-sagemaker-0.6.3.tar", last modified: Tue May 30 19:55:42 2023, max compression
```

## Comparing `cohere-sagemaker-0.6.2.tar` & `cohere-sagemaker-0.6.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-09 20:53:50.072662 cohere-sagemaker-0.6.2/
--rw-r--r--   0 alexandre   (502) staff       (20)     1066 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/LICENSE
--rw-r--r--   0 alexandre   (502) staff       (20)     1412 2023-05-09 20:53:50.072533 cohere-sagemaker-0.6.2/PKG-INFO
--rw-r--r--   0 alexandre   (502) staff       (20)      948 2023-05-09 15:22:05.000000 cohere-sagemaker-0.6.2/README.md
-drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-09 20:53:50.071780 cohere-sagemaker-0.6.2/cohere_sagemaker/
--rw-r--r--   0 alexandre   (502) staff       (20)       57 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/__init__.py
--rw-r--r--   0 alexandre   (502) staff       (20)     1222 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/classification.py
--rw-r--r--   0 alexandre   (502) staff       (20)    19336 2023-05-09 20:02:06.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/client.py
--rw-r--r--   0 alexandre   (502) staff       (20)      623 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/embeddings.py
--rw-r--r--   0 alexandre   (502) staff       (20)      591 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/error.py
--rw-r--r--   0 alexandre   (502) staff       (20)      796 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/generation.py
--rw-r--r--   0 alexandre   (502) staff       (20)     2069 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/rerank.py
--rw-r--r--   0 alexandre   (502) staff       (20)      337 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/response.py
-drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-09 20:53:50.072348 cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/
--rw-r--r--   0 alexandre   (502) staff       (20)     1412 2023-05-09 20:53:50.000000 cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 alexandre   (502) staff       (20)      460 2023-05-09 20:53:50.000000 cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 alexandre   (502) staff       (20)        1 2023-05-09 20:53:50.000000 cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 alexandre   (502) staff       (20)       16 2023-05-09 20:53:50.000000 cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/requires.txt
--rw-r--r--   0 alexandre   (502) staff       (20)       17 2023-05-09 20:53:50.000000 cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 alexandre   (502) staff       (20)       38 2023-05-09 20:53:50.072704 cohere-sagemaker-0.6.2/setup.cfg
--rw-r--r--   0 alexandre   (502) staff       (20)     1525 2023-05-09 20:46:51.000000 cohere-sagemaker-0.6.2/setup.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-30 19:55:42.723928 cohere-sagemaker-0.6.3/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1066 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/LICENSE
+-rw-r--r--   0 alexandre   (502) staff       (20)     1412 2023-05-30 19:55:42.723780 cohere-sagemaker-0.6.3/PKG-INFO
+-rw-r--r--   0 alexandre   (502) staff       (20)      948 2023-05-09 15:22:05.000000 cohere-sagemaker-0.6.3/README.md
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-30 19:55:42.722838 cohere-sagemaker-0.6.3/cohere_sagemaker/
+-rw-r--r--   0 alexandre   (502) staff       (20)       57 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1222 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/classification.py
+-rw-r--r--   0 alexandre   (502) staff       (20)    19616 2023-05-30 19:55:02.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/client.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      623 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/embeddings.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      591 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/error.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      796 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/generation.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     2069 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/rerank.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      337 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.3/cohere_sagemaker/response.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-30 19:55:42.723544 cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1412 2023-05-30 19:55:42.000000 cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 alexandre   (502) staff       (20)      460 2023-05-30 19:55:42.000000 cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)        1 2023-05-30 19:55:42.000000 cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)       16 2023-05-30 19:55:42.000000 cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)       17 2023-05-30 19:55:42.000000 cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)       38 2023-05-30 19:55:42.723978 cohere-sagemaker-0.6.3/setup.cfg
+-rw-r--r--   0 alexandre   (502) staff       (20)     1525 2023-05-30 19:55:02.000000 cohere-sagemaker-0.6.3/setup.py
```

### Comparing `cohere-sagemaker-0.6.2/LICENSE` & `cohere-sagemaker-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.2/PKG-INFO` & `cohere-sagemaker-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere-sagemaker
-Version: 0.6.2
+Version: 0.6.3
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker
 Home-page: https://github.com/cohere-ai/cohere-sagemaker
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cohere-sagemaker-0.6.2/README.md` & `cohere-sagemaker-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.2/cohere_sagemaker/classification.py` & `cohere-sagemaker-0.6.3/cohere_sagemaker/classification.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.2/cohere_sagemaker/client.py` & `cohere-sagemaker-0.6.3/cohere_sagemaker/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import json
 import os
-from typing import Any, Dict, List, Optional, Tuple, Union
 import tarfile
 import tempfile
-import sagemaker as sage
-from sagemaker.s3 import parse_s3_url, S3Downloader, S3Uploader
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import boto3
-from botocore.exceptions import ClientError, EndpointConnectionError, ParamValidationError
-from cohere_sagemaker.classification import Classification, Classifications
+import sagemaker as sage
+from botocore.exceptions import (ClientError, EndpointConnectionError,
+                                 ParamValidationError)
+from sagemaker.s3 import S3Downloader, S3Uploader, parse_s3_url
 
+from cohere_sagemaker.classification import Classification, Classifications
 from cohere_sagemaker.embeddings import Embeddings
 from cohere_sagemaker.error import CohereError
 from cohere_sagemaker.generation import (Generation, Generations,
                                          TokenLikelihood)
 from cohere_sagemaker.rerank import Reranking
 
 
@@ -46,50 +47,63 @@
         """
         if not self._does_endpoint_exist(endpoint_name):
             raise CohereError(f"Endpoint {endpoint_name} does not exist.")
         self._endpoint_name = endpoint_name
 
     def _s3_models_dir_to_tarfile(self, s3_models_dir: str) -> str:
         """
-        Compress an S3 folder to a `models.tar.gz` file.
-        Here it is mainly used to aggregate fine-tuned models into a single file to deploy them in the same endpoint
-        As this is not possible directly on s3, download the dir to a local temporary dir, tar.gz it, and upload again
+        Compress an S3 folder which contains one or several fine-tuned models to a tar file.
+        If the S3 folder contains only one fine-tuned model, it simply returns the path to that model.
+        If the S3 folder contains several fine-tuned models, it download all models, aggregates them into a single 
+        tar.gz file.
 
         Args:
             s3_models_dir (str): S3 URI pointing to a folder
 
         Returns:
             str: S3 URI pointing to the `models.tar.gz` file
         """
 
         s3_models_dir = s3_models_dir + ("/" if not s3_models_dir.endswith("/") else "")
-        with tempfile.TemporaryDirectory() as tmpdir:
 
-            # Download all fine-tuned models from s3
-            local_models_dir = os.path.join(tmpdir, "models")
-            for item in S3Downloader.list(s3_models_dir, sagemaker_session=self._sess):
-                if (
-                    item.endswith(".tar.gz")  # only tar gz files 
-                    and (item.split("/")[-1] != "models.tar.gz")  # exclude the tar.gz file we are creating
-                    and (item.rsplit("/", 1)[0] == s3_models_dir[:-1])  # only files directly in s3_models_dir
-                ):
-                    print(f"Adding fine-tuned model: {item}")
-                    S3Downloader.download(item, local_models_dir, sagemaker_session=self._sess)
+        # Links of all fine-tuned models in s3_models_dir. Their format should be .tar.gz 
+        s3_tar_models = [
+            s3_path
+            for s3_path in S3Downloader.list(s3_models_dir, sagemaker_session=self._sess)
+            if (
+                s3_path.endswith(".tar.gz")  # only .tar.gz files
+                and (s3_path.split("/")[-1] != "models.tar.gz")  # exclude the .tar.gz file we are creating
+                and (s3_path.rsplit("/", 1)[0] == s3_models_dir[:-1])  # only files at the root of s3_models_dir
+            )
+        ]
 
-            try:
-                assert len(os.listdir(local_models_dir)) > 0
-            except:
-                raise CohereError(f"No fine-tuned models found in {s3_models_dir}")
+        if len(s3_tar_models) == 0:
+            raise CohereError(f"No fine-tuned models found in {s3_models_dir}")
+        elif len(s3_tar_models) == 1:
+            print(f"Found one fine-tuned model: {s3_tar_models[0]}")
+            return s3_tar_models[0]
+
+        # More than one fine-tuned model found, need to aggregate them into a single .tar.gz file
+        with tempfile.TemporaryDirectory() as tmpdir:
+            local_tar_models_dir = os.path.join(tmpdir, "tar")
+            local_models_dir = os.path.join(tmpdir, "models")
 
-            # Tar.gz all files in downloaded dir
+            # Download and extract all fine-tuned models
+            for s3_tar_model in s3_tar_models:
+                print(f"Adding fine-tuned model: {s3_tar_model}")
+                S3Downloader.download(s3_tar_model, local_tar_models_dir, sagemaker_session=self._sess)
+                with tarfile.open(os.path.join(local_tar_models_dir, s3_tar_model.split("/")[-1])) as tar:
+                    tar.extractall(local_models_dir)
+                
+            # Compress local_models_dir to a tar.gz file
             model_tar = os.path.join(tmpdir, "models.tar.gz")
             with tarfile.open(model_tar, "w:gz") as tar:
                 tar.add(local_models_dir, arcname=".")
 
-            # Upload model_tar to s3
+            # Upload the new tarfile containing all models to s3
             # Very important to remove the trailing slash from s3_models_dir otherwise it just doesn't upload
             model_tar_s3 = S3Uploader.upload(model_tar, s3_models_dir[:-1], sagemaker_session=self._sess)
 
             # sanity check
             assert s3_models_dir + "models.tar.gz" in S3Downloader.list(s3_models_dir, sagemaker_session=self._sess)
 
         return model_tar_s3
@@ -170,35 +184,27 @@
                 **validation_params
             )
         except ParamValidationError:
             # For at least some versions of python 3.6, SageMaker SDK does not support the validation_params
             model.deploy(n_instances, instance_type, endpoint_name=endpoint_name)
         self.connect_to_endpoint(endpoint_name)
 
-        if model_data is not None:
-            # Delete the uploaded models.tar.gz it after deployment has completed
-            s3_resource = boto3.resource("s3")
-            bucket, key = parse_s3_url(model_data)
-            s3_resource.Object(bucket, key).delete()
-
     def generate(
         self,
         prompt: str,
         # not applicable to sagemaker deployment
         # model: str = None,
         # requires DB with presets
         # preset: str = None,
         # not implemented in API
         # num_generations: int = 1,
         max_tokens: int = 20,
         temperature: float = 1.0,
         k: int = 0,
         p: float = 0.75,
-        frequency_penalty: float = 0.0,
-        presence_penalty: float = 0.0,
         stop_sequences: Optional[List[str]] = None,
         return_likelihoods: Optional[str] = None,
         truncate: Optional[str] = None,
         variant: Optional[str] = None
     ) -> Generations:
 
         if self._endpoint_name is None:
@@ -206,16 +212,14 @@
 
         json_params = {
             'prompt': prompt,
             'max_tokens': max_tokens,
             'temperature': temperature,
             'k': k,
             'p': p,
-            'frequency_penalty': frequency_penalty,
-            'presence_penalty': presence_penalty,
             'stop_sequences': stop_sequences,
             'return_likelihoods': return_likelihoods,
             'truncate': truncate
         }
         for key, value in list(json_params.items()):
             if value is None:
                 del json_params[key]
@@ -461,8 +465,7 @@
     def close(self) -> None:
         try:
             self._client.close()
             self._service_client.close()
         except AttributeError:
             print("SageMaker client could not be closed. This might be because you are using an old version of SageMaker.")
             raise
-
```

### Comparing `cohere-sagemaker-0.6.2/cohere_sagemaker/embeddings.py` & `cohere-sagemaker-0.6.3/cohere_sagemaker/embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.2/cohere_sagemaker/error.py` & `cohere-sagemaker-0.6.3/cohere_sagemaker/error.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.2/cohere_sagemaker/generation.py` & `cohere-sagemaker-0.6.3/cohere_sagemaker/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.2/cohere_sagemaker/rerank.py` & `cohere-sagemaker-0.6.3/cohere_sagemaker/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/PKG-INFO` & `cohere-sagemaker-0.6.3/cohere_sagemaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere-sagemaker
-Version: 0.6.2
+Version: 0.6.3
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker
 Home-page: https://github.com/cohere-ai/cohere-sagemaker
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cohere-sagemaker-0.6.2/setup.py` & `cohere-sagemaker-0.6.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         return False
 
     def has_ext_modules(foo) -> bool:
         return True
 
 
 setuptools.setup(name='cohere-sagemaker',
-                 version='0.6.2',
+                 version='0.6.3',
                  author='Cohere',
                  author_email='support@cohere.ai',
                  description='A Python library for the Cohere endpoints in AWS Sagemaker',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://github.com/cohere-ai/cohere-sagemaker',
                  packages=setuptools.find_packages(),
```

