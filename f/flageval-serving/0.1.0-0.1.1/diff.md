# Comparing `tmp/flageval_serving-0.1.0.tar.gz` & `tmp/flageval_serving-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flageval_serving-0.1.0.tar", max compression
+gzip compressed data, was "flageval_serving-0.1.1.tar", max compression
```

## Comparing `flageval_serving-0.1.0.tar` & `flageval_serving-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1288 2023-05-29 07:14:03.234350 flageval_serving-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-29 07:08:57.310781 flageval_serving-0.1.0/flageval/serving/__init__.py
--rw-r--r--   0        0        0      791 2023-05-29 07:09:21.686007 flageval_serving-0.1.0/flageval/serving/app.py
--rw-r--r--   0        0        0     3902 2023-05-29 07:09:29.693749 flageval_serving-0.1.0/flageval/serving/cli.py
--rw-r--r--   0        0        0       26 2023-05-29 07:08:57.326678 flageval_serving-0.1.0/flageval/serving/extensions.py
--rw-r--r--   0        0        0     2649 2023-05-23 13:32:07.184516 flageval_serving-0.1.0/flageval/serving/finder.py
--rw-r--r--   0        0        0     2290 2023-05-29 07:09:33.651902 flageval_serving-0.1.0/flageval/serving/flagenv.py
--rw-r--r--   0        0        0     4127 2023-05-29 07:14:10.771573 flageval_serving-0.1.0/flageval/serving/flageval.py
--rw-r--r--   0        0        0     1973 2023-05-29 07:14:10.771889 flageval_serving-0.1.0/flageval/serving/guniconf.py
--rw-r--r--   0        0        0      174 2023-05-23 13:32:07.186126 flageval_serving-0.1.0/flageval/serving/service/__init__.py
--rw-r--r--   0        0        0      944 2023-05-23 13:32:07.186579 flageval_serving-0.1.0/flageval/serving/service/base.py
--rw-r--r--   0        0        0      512 2023-05-23 13:32:07.187004 flageval_serving-0.1.0/flageval/serving/service/demo_service.py
--rw-r--r--   0        0        0      336 2023-05-23 13:32:07.187325 flageval_serving-0.1.0/flageval/serving/service/guniconf.py
--rw-r--r--   0        0        0     2344 2023-05-23 13:32:07.187853 flageval_serving-0.1.0/flageval/serving/service/nlp.py
--rw-r--r--   0        0        0      265 2023-05-23 13:32:07.188185 flageval_serving-0.1.0/flageval/serving/service/settings.py
--rw-r--r--   0        0        0      190 2023-05-23 13:32:07.188576 flageval_serving-0.1.0/flageval/serving/service/views.py
--rw-r--r--   0        0        0      928 2023-05-29 07:10:10.100369 flageval_serving-0.1.0/flageval/serving/signals.py
--rw-r--r--   0        0        0     2664 2023-05-29 07:08:57.342203 flageval_serving-0.1.0/flageval/serving/util.py
--rw-r--r--   0        0        0      567 2023-05-23 13:32:07.191605 flageval_serving-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2107 1970-01-01 00:00:00.000000 flageval_serving-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1289 2023-05-29 08:11:29.020506 flageval_serving-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 07:08:57.310781 flageval_serving-0.1.1/flageval/serving/__init__.py
+-rw-r--r--   0        0        0      791 2023-05-29 07:09:21.686007 flageval_serving-0.1.1/flageval/serving/app.py
+-rw-r--r--   0        0        0     3902 2023-05-29 07:09:29.693749 flageval_serving-0.1.1/flageval/serving/cli.py
+-rw-r--r--   0        0        0       26 2023-05-29 07:08:57.326678 flageval_serving-0.1.1/flageval/serving/extensions.py
+-rw-r--r--   0        0        0     2649 2023-05-23 13:32:07.184516 flageval_serving-0.1.1/flageval/serving/finder.py
+-rw-r--r--   0        0        0     2290 2023-05-29 07:09:33.651902 flageval_serving-0.1.1/flageval/serving/flagenv.py
+-rw-r--r--   0        0        0     4224 2023-05-30 07:00:42.215950 flageval_serving-0.1.1/flageval/serving/flageval.py
+-rw-r--r--   0        0        0     1973 2023-05-29 07:14:10.771889 flageval_serving-0.1.1/flageval/serving/guniconf.py
+-rw-r--r--   0        0        0      174 2023-05-23 13:32:07.186126 flageval_serving-0.1.1/flageval/serving/service/__init__.py
+-rw-r--r--   0        0        0      944 2023-05-23 13:32:07.186579 flageval_serving-0.1.1/flageval/serving/service/base.py
+-rw-r--r--   0        0        0      512 2023-05-23 13:32:07.187004 flageval_serving-0.1.1/flageval/serving/service/demo_service.py
+-rw-r--r--   0        0        0      336 2023-05-23 13:32:07.187325 flageval_serving-0.1.1/flageval/serving/service/guniconf.py
+-rw-r--r--   0        0        0     2344 2023-05-23 13:32:07.187853 flageval_serving-0.1.1/flageval/serving/service/nlp.py
+-rw-r--r--   0        0        0      265 2023-05-23 13:32:07.188185 flageval_serving-0.1.1/flageval/serving/service/settings.py
+-rw-r--r--   0        0        0      190 2023-05-23 13:32:07.188576 flageval_serving-0.1.1/flageval/serving/service/views.py
+-rw-r--r--   0        0        0      928 2023-05-29 07:10:10.100369 flageval_serving-0.1.1/flageval/serving/signals.py
+-rw-r--r--   0        0        0     2664 2023-05-29 07:08:57.342203 flageval_serving-0.1.1/flageval/serving/util.py
+-rw-r--r--   0        0        0      567 2023-05-30 07:01:04.642331 flageval_serving-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 flageval_serving-0.1.1/PKG-INFO
```

### Comparing `flageval_serving-0.1.0/README.md` & `flageval_serving-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 ``` shell
 pip install --upgrade flageval-serving
 ```
 
 ## Usage
 
-1. **Model**: of cuase we have a model that is ready be evaluated, let's assume it lives in the path: `/path/to/model`;
+1. **Model**: of course we have a model that is ready be evaluated, let's assume it lives in the path: `/path/to/model`;
 2. Then we can write our service code, let's put the service code in `service.py` and take a NLP model as the example:
 
 
     ``` python
     from flageval.serving.service import NLPModelService, NLPEvalRequest, NLPEvalResponse, NLPCompletion
```

### Comparing `flageval_serving-0.1.0/flageval/serving/app.py` & `flageval_serving-0.1.1/flageval/serving/app.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.0/flageval/serving/cli.py` & `flageval_serving-0.1.1/flageval/serving/cli.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.0/flageval/serving/finder.py` & `flageval_serving-0.1.1/flageval/serving/finder.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.0/flageval/serving/flagenv.py` & `flageval_serving-0.1.1/flageval/serving/flagenv.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.0/flageval/serving/flageval.py` & `flageval_serving-0.1.1/flageval/serving/flageval.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,16 @@
                 {
                     'filename': item.filename,
                     'sizeKb': item.size_kb,
                 }
                 for item in local_files
             ]
         })
+        if resp.status_code >= 400:
+            raise FlagEvalError(resp.status_code, resp.text)
         return resp.json()
 
     def _do_upload(self, item: File):
         url = f'{self.host}{self.CHUNKS_PATH.format(item.id_)}'
         with open(item.path,'rb') as f:
             for i, chunk in tqdm.tqdm(enumerate(item.chunks), desc=item.filename):
                 buf = io.BytesIO()
```

### Comparing `flageval_serving-0.1.0/flageval/serving/guniconf.py` & `flageval_serving-0.1.1/flageval/serving/guniconf.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.0/flageval/serving/service/base.py` & `flageval_serving-0.1.1/flageval/serving/service/base.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.0/flageval/serving/service/demo_service.py` & `flageval_serving-0.1.1/flageval/serving/service/demo_service.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.0/flageval/serving/service/nlp.py` & `flageval_serving-0.1.1/flageval/serving/service/nlp.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.0/flageval/serving/signals.py` & `flageval_serving-0.1.1/flageval/serving/signals.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.0/flageval/serving/util.py` & `flageval_serving-0.1.1/flageval/serving/util.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.0/pyproject.toml` & `flageval_serving-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flageval-serving"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["FlagEval <flageval@baai.ac.cn>"]
 readme = "README.md"
 packages = [{ include = "flageval" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `flageval_serving-0.1.0/PKG-INFO` & `flageval_serving-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flageval-serving
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: FlagEval
 Author-email: flageval@baai.ac.cn
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -30,15 +30,15 @@
 
 ``` shell
 pip install --upgrade flageval-serving
 ```
 
 ## Usage
 
-1. **Model**: of cuase we have a model that is ready be evaluated, let's assume it lives in the path: `/path/to/model`;
+1. **Model**: of course we have a model that is ready be evaluated, let's assume it lives in the path: `/path/to/model`;
 2. Then we can write our service code, let's put the service code in `service.py` and take a NLP model as the example:
 
 
     ``` python
     from flageval.serving.service import NLPModelService, NLPEvalRequest, NLPEvalResponse, NLPCompletion
```

