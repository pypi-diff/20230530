# Comparing `tmp/bytetrade-recommend-model-sdk-0.0.16.tar.gz` & `tmp/bytetrade-recommend-model-sdk-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.16.tar", last modified: Tue May 16 09:22:13 2023, max compression
+gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.17.tar", last modified: Tue May 30 08:54:47 2023, max compression
```

## Comparing `bytetrade-recommend-model-sdk-0.0.16.tar` & `bytetrade-recommend-model-sdk-0.0.17.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:22:13.547504 bytetrade-recommend-model-sdk-0.0.16/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-10 04:37:58.000000 bytetrade-recommend-model-sdk-0.0.16/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-16 09:22:13.543504 bytetrade-recommend-model-sdk-0.0.16/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-04-24 08:15:48.000000 bytetrade-recommend-model-sdk-0.0.16/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:22:13.543504 bytetrade-recommend-model-sdk-0.0.16/bytetrade_recommend_model_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-16 09:22:13.000000 bytetrade-recommend-model-sdk-0.0.16/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      983 2023-05-16 09:22:13.000000 bytetrade-recommend-model-sdk-0.0.16/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-16 09:22:13.000000 bytetrade-recommend-model-sdk-0.0.16/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-05-16 09:22:13.000000 bytetrade-recommend-model-sdk-0.0.16/bytetrade_recommend_model_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-16 09:22:13.000000 bytetrade-recommend-model-sdk-0.0.16/bytetrade_recommend_model_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:22:13.543504 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-20 08:07:33.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:22:13.543504 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/embeddings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 15:19:49.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/embeddings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-04-21 15:20:39.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/embeddings/embedding_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-16 08:59:28.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/embeddings/word2vec_embedding.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:22:13.543504 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/proto_class/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-23 00:13:23.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/proto_class/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2661 2023-04-28 08:19:07.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/proto_class/embedding_pb2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:22:13.543504 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/rank/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-05 03:16:24.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/rank/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-05 03:17:41.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/rank/faiss_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9462 2023-05-11 19:36:12.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/rank/rank_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-05-07 06:11:48.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/rank/time_weight_decay_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:22:13.543504 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 01:30:23.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1432 2023-05-16 09:21:11.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/resources/model_management.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:22:13.543504 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/tools/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-20 12:41:52.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/tools/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3456 2023-04-22 22:25:24.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/tools/aws_s3_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3652 2023-05-06 12:19:45.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/tools/common_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26860 2023-05-16 09:13:12.000000 bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/tools/model_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-16 09:22:13.547504 bytetrade-recommend-model-sdk-0.0.16/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-05-16 09:21:55.000000 bytetrade-recommend-model-sdk-0.0.16/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.771402 bytetrade-recommend-model-sdk-0.0.17/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/bytetrade_recommend_model_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-30 08:54:47.000000 bytetrade-recommend-model-sdk-0.0.17/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1032 2023-05-30 08:54:47.000000 bytetrade-recommend-model-sdk-0.0.17/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-30 08:54:47.000000 bytetrade-recommend-model-sdk-0.0.17/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-05-30 08:54:47.000000 bytetrade-recommend-model-sdk-0.0.17/bytetrade_recommend_model_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-30 08:54:47.000000 bytetrade-recommend-model-sdk-0.0.17/bytetrade_recommend_model_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      495 2023-05-30 08:37:42.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/bert_embedding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/embedding_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/word2vec_embedding.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/proto_class/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/proto_class/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2661 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/proto_class/embedding_pb2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/rank/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/rank/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/rank/faiss_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9322 2023-05-29 08:12:34.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/rank/rank_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/rank/time_weight_decay_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1800 2023-05-30 08:47:17.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/resources/model_management.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3456 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/aws_s3_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3652 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/common_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27487 2023-05-30 08:43:31.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/model_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-30 08:54:47.771402 bytetrade-recommend-model-sdk-0.0.17/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-05-30 08:52:43.000000 bytetrade-recommend-model-sdk-0.0.17/setup.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.16/README.md` & `bytetrade-recommend-model-sdk-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.16/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt` & `bytetrade-recommend-model-sdk-0.0.17/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 bytetrade_recommend_model_sdk.egg-info/PKG-INFO
 bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
 bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
 bytetrade_recommend_model_sdk.egg-info/requires.txt
 bytetrade_recommend_model_sdk.egg-info/top_level.txt
 recommend_model_sdk/__init__.py
 recommend_model_sdk/embeddings/__init__.py
+recommend_model_sdk/embeddings/bert_embedding.py
 recommend_model_sdk/embeddings/embedding_tool.py
 recommend_model_sdk/embeddings/word2vec_embedding.py
 recommend_model_sdk/proto_class/__init__.py
 recommend_model_sdk/proto_class/embedding_pb2.py
 recommend_model_sdk/rank/__init__.py
 recommend_model_sdk/rank/faiss_tool.py
 recommend_model_sdk/rank/rank_tool.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/embeddings/embedding_tool.py` & `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/embedding_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/embeddings/word2vec_embedding.py` & `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/word2vec_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/proto_class/embedding_pb2.py` & `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/proto_class/embedding_pb2.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/rank/rank_tool.py` & `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/rank/rank_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import numpy as np
 from datetime import datetime
 from recommend_model_sdk.rank.time_weight_decay_tool import TimeWeightDecayTool
 from recommend_model_sdk.tools.common_tool import CommonTool
 
 
 class RankTool:
-    def __init__(self,base_document_id_to_embedding) -> None:
+
+    def __init__(self, base_document_id_to_embedding) -> None:
         """_summary_
 
         Args:
             base_document_id_to_embedding (_type_): _description_
             {
                 "document_id":{
                     "embedding":[],numpy
@@ -22,165 +23,160 @@
             ValueError: _description_
             ValueError: _description_
             ValueError: _description_
             ValueError: _description_
             ValueError: _description_
             ValueError: _description_
         """
-        if isinstance(base_document_id_to_embedding,dict) is False:
+        if isinstance(base_document_id_to_embedding, dict) is False:
             raise ValueError("base_document_id_to_embedding is not dict")
         if len(base_document_id_to_embedding) < 1:
             raise ValueError('base_document_id_to_embedding length small than 1')
         set_shape = set()
         list_current_embedding = list()
         self.__base_length = len(base_document_id_to_embedding)
         self.__base_index_to_document_id = dict()
         self.__base_document_id_to_index = dict()
         self.__common_tool = CommonTool()
         self.__logger = self.__common_tool.get_logger()
         current_index = 0
         self.__base_document_id_to_created_at_tuple_list = list()
         for current_document_id, current_embedding_info in base_document_id_to_embedding.items():
-            if isinstance(current_document_id,str) is False:
+            if isinstance(current_document_id, str) is False:
                 raise ValueError(f"current_document_id {current_document_id} is not str")
-            if isinstance(current_embedding_info,dict) is False:
+            if isinstance(current_embedding_info, dict) is False:
                 raise ValueError("current_embedding_info is not dict")
             if "embedding" not in current_embedding_info:
                 raise ValueError("embedding not in current_embedding_info")
             current_embedding = current_embedding_info["embedding"]
             # if isinstance(current_embedding,np.array)
-            if isinstance(current_embedding,np.ndarray) is False:
+            if isinstance(current_embedding, np.ndarray) is False:
                 raise ValueError('there is embedding is not np.ndarray')
             if current_embedding.dtype != np.float32:
                 raise ValueError("embedding_value is not float32")
             if "created_at" not in current_embedding_info:
                 raise ValueError("created_at not in current_embedding_info")
             created_at = current_embedding_info["created_at"]
-            if isinstance(created_at,datetime) is False:
+            if isinstance(created_at, datetime) is False:
                 raise ValueError("created_at is not datetime")
-            self.__base_document_id_to_created_at_tuple_list.append((current_document_id,created_at))
-            
+            self.__base_document_id_to_created_at_tuple_list.append((current_document_id, created_at))
+
             set_shape.add(current_embedding.shape)
             list_current_embedding.append(current_embedding)
             self.__base_index_to_document_id[current_index] = current_document_id
             self.__base_document_id_to_index[current_document_id] = current_index
-            
+
             current_index = current_index + 1
-        self.__base_document_id_to_created_at_tuple_list.sort(key=lambda tup: tup[1],reverse=True)
-        self.__logger.debug(self.__base_document_id_to_created_at_tuple_list)
+        self.__base_document_id_to_created_at_tuple_list.sort(key=lambda tup: tup[1], reverse=True)
+        #self.__logger.debug(self.__base_document_id_to_created_at_tuple_list)
         if len(set_shape) > 1:
             raise ValueError(f'have different shape embeddings')
         self.__embedding_shape = set_shape.pop()
         self.__original_base_embedding = np.stack(list_current_embedding)
         self.__normalized_base_embedding = np.copy(self.__original_base_embedding)
         faiss.normalize_L2(self.__normalized_base_embedding)
         # self.__original_base_embedding_index =  faiss.IndexFlatL2(self.__original_base_embedding)
         self.__cosin_index = faiss.index_factory(self.__embedding_shape[0], "Flat", faiss.METRIC_INNER_PRODUCT)
         self.__cosin_index.add(self.__normalized_base_embedding)
         self.__time_weight_decay_tool = TimeWeightDecayTool()
-    
-    def get_latest_article(self,rank_limit=100):
-        
+
+    def get_latest_article(self, rank_limit=100):
+
         pass
-    
-    def rank(self,document_id_to_document_info,rank_limit = 100):
+
+    def rank(self, document_id_to_document_info, rank_limit=100):
         # https://github.com/facebookresearch/faiss/issues/396
-        # 
+        #
         """_summary_
         {
             "document_id":{
                 "embedding":[] numpy
                 "last_reviewed":datetime
             }
         }
         [0-50]
         Args:
             document_id_to_document_info (_type_): _description_
         """
         query_document_length = len(document_id_to_document_info)
-        self.__logger.debug(f'query_document_length {query_document_length}')
+        #self.__logger.debug(f'query_document_length {query_document_length}')
         if rank_limit > self.__base_length:
             raise ValueError("rank_limit is bigger than base length")
         full_weight = 50
 
         if len(document_id_to_document_info) == 0:
             current_tuple_list = self.__base_document_id_to_created_at_tuple_list[:rank_limit]
             document_id_to_weight_tuple_list = list()
             for current_document_id, current_created_at in current_tuple_list:
-                document_id_to_weight_tuple_list.append((current_document_id,self.__time_weight_decay_tool.compute(full_weight,current_created_at,datetime.now())))
+                document_id_to_weight_tuple_list.append((current_document_id, self.__time_weight_decay_tool.compute(full_weight, current_created_at, datetime.now())))
             return document_id_to_weight_tuple_list
-            
+
         search_k = 3
-        while(query_document_length*search_k < 2 * rank_limit):
+        while (query_document_length * search_k < 2 * rank_limit):
             search_k = search_k + 1
         self.__logger.debug(f"search_k {search_k}")
         # previous review weight
-        
+
         # currently weight
         query_index_to_query_document_id = dict()
         query_document_id_to_query_index = dict()
         query_index = 0
         list_query_embedding = list()
         query_document_id_to_weight = dict()
         query_index_to_weight = dict()
         current_time = datetime.now()
         for current_document_id, current_embedding_info in document_id_to_document_info.items():
-            if isinstance(current_document_id,str) is False:
+            if isinstance(current_document_id, str) is False:
                 raise ValueError("current_document_id is not str")
-            if isinstance(current_embedding_info,dict) is False:
+            if isinstance(current_embedding_info, dict) is False:
                 raise ValueError('current_embedding_info is not dict')
             if "embedding" not in current_embedding_info:
                 raise ValueError("embedding not in current_embedding_info")
             current_embedding = current_embedding_info["embedding"]
-            if isinstance(current_embedding,np.ndarray) is False:
+            if isinstance(current_embedding, np.ndarray) is False:
                 raise ValueError('there is embedding is not np.ndarray')
             if current_embedding.dtype != np.float32:
                 raise ValueError("embedding_value is not float32")
             if current_embedding.shape != self.__embedding_shape:
                 raise ValueError("embedding shape is not equal to shape in base embedding")
             current_last_reviewed_time = current_embedding_info['last_reviewed']
-            current_time_weight = self.__time_weight_decay_tool.compute(full_weight,current_last_reviewed_time,current_time)
+            current_time_weight = self.__time_weight_decay_tool.compute(full_weight, current_last_reviewed_time, current_time)
             query_document_id_to_weight[current_document_id] = current_time_weight
             query_index_to_weight[query_index] = current_time_weight
             list_query_embedding.append(current_embedding)
-            query_document_id_to_query_index[current_document_id] = query_index 
+            query_document_id_to_query_index[current_document_id] = query_index
             query_index_to_query_document_id[query_index] = current_document_id
             query_index = query_index + 1
-            
-        
+
         stack_query_embedding = np.stack(list_query_embedding)
         faiss.normalize_L2(stack_query_embedding)
-        
-        
-        while(True):
-            distances, nearest_indexes = self.__cosin_index.search(stack_query_embedding, search_k) #[[]] [[]]
-            article_index_weight_tuple_list = list() # tuple first_element weight, second_element_index
+
+        while (True):
+            distances, nearest_indexes = self.__cosin_index.search(stack_query_embedding, search_k)  #[[]] [[]]
+            article_index_weight_tuple_list = list()  # tuple first_element weight, second_element_index
             for current_query_index in range(query_index):
                 # repeat article
                 current_distance_list = distances[current_query_index]
                 current_nearest_index_list = nearest_indexes[current_query_index]
-                for current_distance,current_neares_index in zip(current_distance_list,current_nearest_index_list):
-                    article_index_weight_tuple_list.append((full_weight * current_distance + query_index_to_weight[current_query_index],current_neares_index))
-            
-            article_index_weight_tuple_list.sort(key=lambda tup: tup[0],reverse=True)
-            
+                for current_distance, current_neares_index in zip(current_distance_list, current_nearest_index_list):
+                    article_index_weight_tuple_list.append((full_weight * current_distance + query_index_to_weight[current_query_index], current_neares_index))
+
+            article_index_weight_tuple_list.sort(key=lambda tup: tup[0], reverse=True)
+
             exist_article_index_set = set()
             new_article_index_weight_list = list()
-            
+
             for current_index_weight_tuple in article_index_weight_tuple_list:
                 if current_index_weight_tuple[1] in exist_article_index_set:
                     continue
                 new_article_index_weight_list.append(current_index_weight_tuple)
                 exist_article_index_set.add(current_index_weight_tuple[1])
             if len(new_article_index_weight_list) >= rank_limit:
                 break
-            search_k = 2*search_k
+            search_k = 2 * search_k
             self.__logger.debug(f"search_k {search_k}")
-        
-        
+
         document_id_to_weight_tuple_list = list()
-        for current_weight,current_base_article_index in article_index_weight_tuple_list:
-            document_id_to_weight_tuple_list.append((self.__base_index_to_document_id[current_base_article_index],current_weight))
+        for current_weight, current_base_article_index in article_index_weight_tuple_list:
+            document_id_to_weight_tuple_list.append((self.__base_index_to_document_id[current_base_article_index], current_weight))
 
-        
         return document_id_to_weight_tuple_list
-
```

### Comparing `bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/rank/time_weight_decay_tool.py` & `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/rank/time_weight_decay_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/resources/model_management.json` & `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/resources/model_management.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'bert'": "OrderedDict([('v1', OrderedDict([('mongodb_embedding_field', 'bert_v1'), "*

 * *           "('pg_embedding_mark_field', 'bert_v1'), ('s3_bucket', 'gpu-model-data'), "*

 * *           "('model_related_files', []), ('model_related_files_suffix', OrderedDict()), "*

 * *           "('model_related_files_public', OrderedDict()), ('active', True)]))])"}*

```diff
@@ -1,8 +1,19 @@
 {
+    "bert": {
+        "v1": {
+            "active": true,
+            "model_related_files": [],
+            "model_related_files_public": {},
+            "model_related_files_suffix": {},
+            "mongodb_embedding_field": "bert_v1",
+            "pg_embedding_mark_field": "bert_v1",
+            "s3_bucket": "gpu-model-data"
+        }
+    },
     "word2vec_google": {
         "v1": {
             "active": true,
             "model_related_files": [
                 "GoogleNews-vectors-negative300.bin",
                 "tfidf.model",
                 "dictionary"
```

### Comparing `bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/tools/aws_s3_tool.py` & `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/aws_s3_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/tools/common_tool.py` & `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/common_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.16/recommend_model_sdk/tools/model_tool.py` & `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/model_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import nltk
 import zlib
 
 from recommend_model_sdk.tools.aws_s3_tool import AWSS3Tool
 from recommend_model_sdk.tools.common_tool import CommonTool
 from recommend_model_sdk.embeddings.word2vec_embedding import Word2VecEmbedding
 import recommend_model_sdk.proto_class.embedding_pb2 as rec_proto_embebding
+from recommend_model_sdk.embeddings.bert_embedding import BertEmbedding
 
 class ModelTool:
     def __init__(self,model_root_dir) -> None:
         if isinstance(model_root_dir,str) is False:
             raise ValueError("model_root_dir is not str")
         if os.path.exists(model_root_dir) is False:
             raise ValueError("model_root_dir is not exist")
@@ -22,14 +23,15 @@
         self.__logger.debug(self.__model_management_file)
 
         self.__model_related_files_suffix_set = set(["gz","direct"])
         self.__model_dict = self.__validate_model_management_file(self.__model_management_file)
         self.__awss3tool = AWSS3Tool()
         self.__model_name_to_infer_method = dict()
         self.__model_name_to_infer_method["word2vec_google"] = self.word2vec_calculate_embedding
+        self.__model_name_to_infer_method["bert"] = self.bert_calculate_embedding
         self.__model_root_dir = model_root_dir
         self.__latest_support_package_number = set([1000,5000,10000])
 
     
     def get_valid_model_and_version(self):
         model_name_to_valid_version_list = dict()
         for current_model_name, current_model_version_dict in self.__model_dict.items():
@@ -97,15 +99,23 @@
         model_related_files_public = current_model_detail["model_related_files_public"]
         for current_file_name in model_related_files:
             if current_file_name not in model_related_files_public:
                 raise ValueError(f"current_file_name {current_file_name} not in model_related_files_public")
             current_file_name_public = model_related_files_public[current_file_name]
             if isinstance(current_file_name_public,bool) is False:
                 raise ValueError(F"current_file_name {current_file_name} current_file_name_public is  not bool")
-        
+
+    def bert_calculate_embedding(self,model_name,model_version,dict_document):
+        self.valid_model_name_and_version(model_name,model_version)
+        self.valid_infer_document(dict_document)
+        bert_embedding_tool = BertEmbedding()
+        id_to_infer_result = dict()
+        for current_id, current_text in dict_document.items():
+            id_to_infer_result[current_id] = bert_embedding_tool.calculate_embedding(current_text)      
+        return id_to_infer_result 
         
     def __validate_model_management_file(self,path):
         if isinstance(path,str) is False:
             raise ValueError(f"path {path} is not str")
         if os.path.exists(path) is False:
             raise ValueError(f"model management file {path} is not exist")
         model_management_dict = self.__common_tool.read_json(path)
```

### Comparing `bytetrade-recommend-model-sdk-0.0.16/setup.py` & `bytetrade-recommend-model-sdk-0.0.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 sys.path.append(os.path.dirname(__file__) + "/recommend-model")
 
 
 
 
 setup(
     name="bytetrade-recommend-model-sdk",
-    version="0.0.16",
+    version="0.0.17",
     # packages=find_packages(exclude="unit_test"),
     install_requires=[
         "pandas==2.0.0",
         "gensim==4.3.1",
         "protobuf==4.21.8",
         "nltk==3.8.1",
         "boto3"
```

