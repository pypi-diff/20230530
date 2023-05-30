# Comparing `tmp/peachdb-0.0.3.tar.gz` & `tmp/peachdb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peachdb-0.0.3.tar", last modified: Tue May 30 15:31:28 2023, max compression
+gzip compressed data, was "peachdb-0.0.4.tar", last modified: Tue May 30 16:05:45 2023, max compression
```

## Comparing `peachdb-0.0.3.tar` & `peachdb-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:31:28.359833 peachdb-0.0.3/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11356 2023-05-29 20:30:02.000000 peachdb-0.0.3/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5735 2023-05-30 15:31:28.359833 peachdb-0.0.3/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5415 2023-05-30 13:14:30.000000 peachdb-0.0.3/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:31:28.359833 peachdb-0.0.3/peachdb/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7855 2023-05-30 10:56:06.000000 peachdb-0.0.3/peachdb/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:31:28.359833 peachdb-0.0.3/peachdb/backends/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      923 2023-05-29 16:37:03.000000 peachdb-0.0.3/peachdb/backends/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3161 2023-05-30 10:57:00.000000 peachdb-0.0.3/peachdb/backends/backend_base.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2056 2023-05-30 11:29:19.000000 peachdb-0.0.3/peachdb/backends/hnsw_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2669 2023-05-29 16:37:03.000000 peachdb-0.0.3/peachdb/backends/numpy_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3894 2023-05-29 20:30:02.000000 peachdb-0.0.3/peachdb/backends/torch_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      223 2023-05-29 16:37:03.000000 peachdb-0.0.3/peachdb/constants.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:31:28.359833 peachdb-0.0.3/peachdb/embedder/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4936 2023-05-30 11:00:29.000000 peachdb-0.0.3/peachdb/embedder/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2718 2023-05-30 10:47:11.000000 peachdb-0.0.3/peachdb/embedder/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:31:28.359833 peachdb-0.0.3/peachdb.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5735 2023-05-30 15:31:28.000000 peachdb-0.0.3/peachdb.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      454 2023-05-30 15:31:28.000000 peachdb-0.0.3/peachdb.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       39 2023-05-30 15:31:28.000000 peachdb-0.0.3/peachdb.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      177 2023-05-30 15:31:28.000000 peachdb-0.0.3/peachdb.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-30 15:31:28.000000 peachdb-0.0.3/peachdb.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       64 2023-05-26 17:11:39.000000 peachdb-0.0.3/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-30 15:31:28.359833 peachdb-0.0.3/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      852 2023-05-30 15:30:05.000000 peachdb-0.0.3/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:05:45.596196 peachdb-0.0.4/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11356 2023-05-29 20:30:02.000000 peachdb-0.0.4/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6203 2023-05-30 16:05:45.596196 peachdb-0.0.4/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5884 2023-05-30 16:05:37.000000 peachdb-0.0.4/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:05:45.596196 peachdb-0.0.4/peachdb/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7855 2023-05-30 10:56:06.000000 peachdb-0.0.4/peachdb/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:05:45.596196 peachdb-0.0.4/peachdb/backends/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      923 2023-05-29 16:37:03.000000 peachdb-0.0.4/peachdb/backends/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3161 2023-05-30 10:57:00.000000 peachdb-0.0.4/peachdb/backends/backend_base.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2056 2023-05-30 11:29:19.000000 peachdb-0.0.4/peachdb/backends/hnsw_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2669 2023-05-29 16:37:03.000000 peachdb-0.0.4/peachdb/backends/numpy_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3894 2023-05-29 20:30:02.000000 peachdb-0.0.4/peachdb/backends/torch_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      223 2023-05-29 16:37:03.000000 peachdb-0.0.4/peachdb/constants.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:05:45.596196 peachdb-0.0.4/peachdb/embedder/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4936 2023-05-30 11:00:29.000000 peachdb-0.0.4/peachdb/embedder/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2718 2023-05-30 10:47:11.000000 peachdb-0.0.4/peachdb/embedder/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:05:45.596196 peachdb-0.0.4/peachdb.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6203 2023-05-30 16:05:45.000000 peachdb-0.0.4/peachdb.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      454 2023-05-30 16:05:45.000000 peachdb-0.0.4/peachdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       39 2023-05-30 16:05:45.000000 peachdb-0.0.4/peachdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      177 2023-05-30 16:05:45.000000 peachdb-0.0.4/peachdb.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-30 16:05:45.000000 peachdb-0.0.4/peachdb.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       64 2023-05-26 17:11:39.000000 peachdb-0.0.4/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-30 16:05:45.596196 peachdb-0.0.4/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      852 2023-05-30 16:05:37.000000 peachdb-0.0.4/setup.py
```

### Comparing `peachdb-0.0.3/LICENSE` & `peachdb-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.3/PKG-INFO` & `peachdb-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peachdb
-Version: 0.0.3
+Version: 0.0.4
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/peach-db/peachdb
 Project-URL: Documentation, https://github.com/peach-db/peachdb/blob/master/README.md
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -23,21 +23,21 @@
 
 Setup [Modal](https://modal.com)
 - Create an account at [modal.com](https://modal.com)
 - Install the modal-client package: `pip install modal-client`
 - Setup token: `modal token new`
 
 (optional)
-To use S3 URIs for your dataset and embedding storage, configure your .env file as below.
+PeachDB accepts local & S3 paths to datasets for embedding computation. To use S3 URIs, configure your .env file as below.
 ```python
-# Setup your AWS CLI, if you haven't already done so
 # Fetch the below values from ~/.aws/credentials
 AWS_ACCESS_KEY_ID=
 AWS_SECRET_ACCESS_KEY=
 ```
+Please ensure the credentials have read & write access to the relevant bucket you plan to use.
 
 <br/>
 
 **Our core API has 3 functions**
 
 ```python
 from peachdb import PeachDB
@@ -63,23 +63,25 @@
 
 # Deploy the database as a publicly available FastAPI server
 # Call GET /query?text='An example query'&top_k=5 to fetch 5 most similar results
 db.deploy()
 ```
 
 ## Why another embedding database?
-PeachDB puts embeddings at the forefront! We've streamlined the entire end-to-end lifecycle of managing embeddings, making it developer-friendly, seamless, and cost-effective. You no longer have to build custom pipelines or fret over hardware setups & scalability issues. PeachDB ensures you can get started within minutes, leaving the worries of cost optimization and scale to us.
+We've streamlined the entire end-to-end process of creating, storing, and retrieving embeddings, making it developer-friendly, seamless, and cost-effective. You no longer have to build custom pipelines or fret over hardware setups & scalability issues. PeachDB ensures you can get started within minutes, leaving the worries of cost optimization and scale to us.
 
 Our key features include:
 * **Automated, cost-effective & large-scale embedding computation**: We leverage serverless GPU functions (through [Modal](https://modal.com/)) to compute embeddings on a large scale efficiently and affordably.
     - For instance, we processed the [Kaggle 5M song lyrics dataset](https://www.kaggle.com/datasets/nikhilnayak123/5-million-song-lyrics-dataset?resource=download&select=ds2.csv) in just *12 minutes at a cost of $4.90*, using sentence transformers!
     - We've developed a Modal wrapper for [Sentence Transformer L12](https://huggingface.co/sentence-transformers/all-MiniLM-L12-v2).
-        - Coming soon: Modal wrappers for OpenAI, Cohere, ImageBind, and more.
+        - Coming soon: Modal wrappers for open-source embedding models such as [ImageBind](https://github.com/facebookresearch/ImageBind), [OpenCLIP](https://github.com/mlfoundations/open_clip), and more.
+        - Coming soon: Support for multi-threaded [OpenAI](https://platform.openai.com/docs/guides/embeddings) embedding calculation.
     - Coming soon: Bring your own embeddings.
     - Coming soon: Custom embedding functions for even more flexibility.
+* **Multimodality**: Native support for data with mixture of modalities (such as image/audio/video).
 * **Highly Customizable**: PeachDB allows you to tailor its features to your needs. You can customize:
     - Embedding computation: as described above.
     - Backend: choose between `exact_cpu` (numpy), `exact_gpu` (torch), or `approx` (HNSW).
     - Distance metrics: `cosine` or `l2`.
 * **Effortless Deployment**: Deploy PeachDB as a publicly available server with a single API. No need to worry about nginx or SSL certs.
     - Coming soon: Managed, scalable deployment.
 * **Consistent API**: Experience the same API across all environments - dev, test, and prod.
@@ -97,40 +99,44 @@
 - Create & activate a new conda environment `conda create -n spoti_vibe python=3.10` & `conda activate spoti_vibe`
 - Setup modal as outlined above
 - Install Peachdb `pip install peachdb`
 - `mkdir spoti_vibe/`
 - Create a new module inside the directory `server.py`
 - Add the following code
 ```python
-import kaggle # make sure you've run `pip install kaggle`
-import os
-
 from peachdb import PeachDB
 
+import os
 os.environ['KAGGLE_USERNAME'] = None # set user name
 os.environ['KAGGLE_KEY'] = None # set key
 
-kaggle.api.authenticate()
-kaggle.api.dataset_download_files('nikhilnayak123/5-million-song-lyrics-dataset', path='/path/to/save', unzip=True)
+import kaggle # make sure you've run `pip install kaggle`
 
+kaggle.api.authenticate()
+kaggle.api.dataset_download_files(
+    'nikhilnayak123/5-million-song-lyrics-dataset',
+    path='.',
+    unzip=True
+)
 
 db = PeachDB.create(
     project_name="spoti_vibe",
-    csv_path="/path/to/local/csv",
+    csv_path='./ds2.csv',  # dataset name as observed on Kaggle
     column_to_embed="lyrics",
     id_column_name="id",
     max_rows=None,
     distance_metric="cosine",
     embedding_backend="exact_cpu",
     embedding_generator="sentence_transformer_L12",
 )
 
 db.deploy() # Public URL will be printed to console
 ```
-And that's it! You should now have a publicly available server that can listen to query requests from the user on: `GET <PUBLIC_URL>/query?text=''&top_k=5`
+
+And that's it! You should now have a publicly available server that can listen to query requests from the user on: `GET <PUBLIC_URL>/query?text='Happy, upbeat summer'&top_k=5`
 
 
 ## FAQs
 Q) How can I delete a project?
 Run `db.delete(project_name="my_app")`
 
 ## Get Involved
```

### Comparing `peachdb-0.0.3/README.md` & `peachdb-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
 Setup [Modal](https://modal.com)
 - Create an account at [modal.com](https://modal.com)
 - Install the modal-client package: `pip install modal-client`
 - Setup token: `modal token new`
 
 (optional)
-To use S3 URIs for your dataset and embedding storage, configure your .env file as below.
+PeachDB accepts local & S3 paths to datasets for embedding computation. To use S3 URIs, configure your .env file as below.
 ```python
-# Setup your AWS CLI, if you haven't already done so
 # Fetch the below values from ~/.aws/credentials
 AWS_ACCESS_KEY_ID=
 AWS_SECRET_ACCESS_KEY=
 ```
+Please ensure the credentials have read & write access to the relevant bucket you plan to use.
 
 <br/>
 
 **Our core API has 3 functions**
 
 ```python
 from peachdb import PeachDB
@@ -53,23 +53,25 @@
 
 # Deploy the database as a publicly available FastAPI server
 # Call GET /query?text='An example query'&top_k=5 to fetch 5 most similar results
 db.deploy()
 ```
 
 ## Why another embedding database?
-PeachDB puts embeddings at the forefront! We've streamlined the entire end-to-end lifecycle of managing embeddings, making it developer-friendly, seamless, and cost-effective. You no longer have to build custom pipelines or fret over hardware setups & scalability issues. PeachDB ensures you can get started within minutes, leaving the worries of cost optimization and scale to us.
+We've streamlined the entire end-to-end process of creating, storing, and retrieving embeddings, making it developer-friendly, seamless, and cost-effective. You no longer have to build custom pipelines or fret over hardware setups & scalability issues. PeachDB ensures you can get started within minutes, leaving the worries of cost optimization and scale to us.
 
 Our key features include:
 * **Automated, cost-effective & large-scale embedding computation**: We leverage serverless GPU functions (through [Modal](https://modal.com/)) to compute embeddings on a large scale efficiently and affordably.
     - For instance, we processed the [Kaggle 5M song lyrics dataset](https://www.kaggle.com/datasets/nikhilnayak123/5-million-song-lyrics-dataset?resource=download&select=ds2.csv) in just *12 minutes at a cost of $4.90*, using sentence transformers!
     - We've developed a Modal wrapper for [Sentence Transformer L12](https://huggingface.co/sentence-transformers/all-MiniLM-L12-v2).
-        - Coming soon: Modal wrappers for OpenAI, Cohere, ImageBind, and more.
+        - Coming soon: Modal wrappers for open-source embedding models such as [ImageBind](https://github.com/facebookresearch/ImageBind), [OpenCLIP](https://github.com/mlfoundations/open_clip), and more.
+        - Coming soon: Support for multi-threaded [OpenAI](https://platform.openai.com/docs/guides/embeddings) embedding calculation.
     - Coming soon: Bring your own embeddings.
     - Coming soon: Custom embedding functions for even more flexibility.
+* **Multimodality**: Native support for data with mixture of modalities (such as image/audio/video).
 * **Highly Customizable**: PeachDB allows you to tailor its features to your needs. You can customize:
     - Embedding computation: as described above.
     - Backend: choose between `exact_cpu` (numpy), `exact_gpu` (torch), or `approx` (HNSW).
     - Distance metrics: `cosine` or `l2`.
 * **Effortless Deployment**: Deploy PeachDB as a publicly available server with a single API. No need to worry about nginx or SSL certs.
     - Coming soon: Managed, scalable deployment.
 * **Consistent API**: Experience the same API across all environments - dev, test, and prod.
@@ -87,44 +89,48 @@
 - Create & activate a new conda environment `conda create -n spoti_vibe python=3.10` & `conda activate spoti_vibe`
 - Setup modal as outlined above
 - Install Peachdb `pip install peachdb`
 - `mkdir spoti_vibe/`
 - Create a new module inside the directory `server.py`
 - Add the following code
 ```python
-import kaggle # make sure you've run `pip install kaggle`
-import os
-
 from peachdb import PeachDB
 
+import os
 os.environ['KAGGLE_USERNAME'] = None # set user name
 os.environ['KAGGLE_KEY'] = None # set key
 
-kaggle.api.authenticate()
-kaggle.api.dataset_download_files('nikhilnayak123/5-million-song-lyrics-dataset', path='/path/to/save', unzip=True)
+import kaggle # make sure you've run `pip install kaggle`
 
+kaggle.api.authenticate()
+kaggle.api.dataset_download_files(
+    'nikhilnayak123/5-million-song-lyrics-dataset',
+    path='.',
+    unzip=True
+)
 
 db = PeachDB.create(
     project_name="spoti_vibe",
-    csv_path="/path/to/local/csv",
+    csv_path='./ds2.csv',  # dataset name as observed on Kaggle
     column_to_embed="lyrics",
     id_column_name="id",
     max_rows=None,
     distance_metric="cosine",
     embedding_backend="exact_cpu",
     embedding_generator="sentence_transformer_L12",
 )
 
 db.deploy() # Public URL will be printed to console
 ```
-And that's it! You should now have a publicly available server that can listen to query requests from the user on: `GET <PUBLIC_URL>/query?text=''&top_k=5`
+
+And that's it! You should now have a publicly available server that can listen to query requests from the user on: `GET <PUBLIC_URL>/query?text='Happy, upbeat summer'&top_k=5`
 
 
 ## FAQs
 Q) How can I delete a project?
 Run `db.delete(project_name="my_app")`
 
 ## Get Involved
 We welcome PR contributors and ideas for how to improve the project.
 
 ## License
-[Apache 2.0](./LICENSE)
+[Apache 2.0](./LICENSE)
```

### Comparing `peachdb-0.0.3/peachdb/__init__.py` & `peachdb-0.0.4/peachdb/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.3/peachdb/backends/__init__.py` & `peachdb-0.0.4/peachdb/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.3/peachdb/backends/backend_base.py` & `peachdb-0.0.4/peachdb/backends/backend_base.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.3/peachdb/backends/hnsw_backend.py` & `peachdb-0.0.4/peachdb/backends/hnsw_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.3/peachdb/backends/numpy_backend.py` & `peachdb-0.0.4/peachdb/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.3/peachdb/backends/torch_backend.py` & `peachdb-0.0.4/peachdb/backends/torch_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.3/peachdb/embedder/__init__.py` & `peachdb-0.0.4/peachdb/embedder/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.3/peachdb/embedder/utils.py` & `peachdb-0.0.4/peachdb/embedder/utils.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.3/peachdb.egg-info/PKG-INFO` & `peachdb-0.0.4/peachdb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peachdb
-Version: 0.0.3
+Version: 0.0.4
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/peach-db/peachdb
 Project-URL: Documentation, https://github.com/peach-db/peachdb/blob/master/README.md
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -23,21 +23,21 @@
 
 Setup [Modal](https://modal.com)
 - Create an account at [modal.com](https://modal.com)
 - Install the modal-client package: `pip install modal-client`
 - Setup token: `modal token new`
 
 (optional)
-To use S3 URIs for your dataset and embedding storage, configure your .env file as below.
+PeachDB accepts local & S3 paths to datasets for embedding computation. To use S3 URIs, configure your .env file as below.
 ```python
-# Setup your AWS CLI, if you haven't already done so
 # Fetch the below values from ~/.aws/credentials
 AWS_ACCESS_KEY_ID=
 AWS_SECRET_ACCESS_KEY=
 ```
+Please ensure the credentials have read & write access to the relevant bucket you plan to use.
 
 <br/>
 
 **Our core API has 3 functions**
 
 ```python
 from peachdb import PeachDB
@@ -63,23 +63,25 @@
 
 # Deploy the database as a publicly available FastAPI server
 # Call GET /query?text='An example query'&top_k=5 to fetch 5 most similar results
 db.deploy()
 ```
 
 ## Why another embedding database?
-PeachDB puts embeddings at the forefront! We've streamlined the entire end-to-end lifecycle of managing embeddings, making it developer-friendly, seamless, and cost-effective. You no longer have to build custom pipelines or fret over hardware setups & scalability issues. PeachDB ensures you can get started within minutes, leaving the worries of cost optimization and scale to us.
+We've streamlined the entire end-to-end process of creating, storing, and retrieving embeddings, making it developer-friendly, seamless, and cost-effective. You no longer have to build custom pipelines or fret over hardware setups & scalability issues. PeachDB ensures you can get started within minutes, leaving the worries of cost optimization and scale to us.
 
 Our key features include:
 * **Automated, cost-effective & large-scale embedding computation**: We leverage serverless GPU functions (through [Modal](https://modal.com/)) to compute embeddings on a large scale efficiently and affordably.
     - For instance, we processed the [Kaggle 5M song lyrics dataset](https://www.kaggle.com/datasets/nikhilnayak123/5-million-song-lyrics-dataset?resource=download&select=ds2.csv) in just *12 minutes at a cost of $4.90*, using sentence transformers!
     - We've developed a Modal wrapper for [Sentence Transformer L12](https://huggingface.co/sentence-transformers/all-MiniLM-L12-v2).
-        - Coming soon: Modal wrappers for OpenAI, Cohere, ImageBind, and more.
+        - Coming soon: Modal wrappers for open-source embedding models such as [ImageBind](https://github.com/facebookresearch/ImageBind), [OpenCLIP](https://github.com/mlfoundations/open_clip), and more.
+        - Coming soon: Support for multi-threaded [OpenAI](https://platform.openai.com/docs/guides/embeddings) embedding calculation.
     - Coming soon: Bring your own embeddings.
     - Coming soon: Custom embedding functions for even more flexibility.
+* **Multimodality**: Native support for data with mixture of modalities (such as image/audio/video).
 * **Highly Customizable**: PeachDB allows you to tailor its features to your needs. You can customize:
     - Embedding computation: as described above.
     - Backend: choose between `exact_cpu` (numpy), `exact_gpu` (torch), or `approx` (HNSW).
     - Distance metrics: `cosine` or `l2`.
 * **Effortless Deployment**: Deploy PeachDB as a publicly available server with a single API. No need to worry about nginx or SSL certs.
     - Coming soon: Managed, scalable deployment.
 * **Consistent API**: Experience the same API across all environments - dev, test, and prod.
@@ -97,40 +99,44 @@
 - Create & activate a new conda environment `conda create -n spoti_vibe python=3.10` & `conda activate spoti_vibe`
 - Setup modal as outlined above
 - Install Peachdb `pip install peachdb`
 - `mkdir spoti_vibe/`
 - Create a new module inside the directory `server.py`
 - Add the following code
 ```python
-import kaggle # make sure you've run `pip install kaggle`
-import os
-
 from peachdb import PeachDB
 
+import os
 os.environ['KAGGLE_USERNAME'] = None # set user name
 os.environ['KAGGLE_KEY'] = None # set key
 
-kaggle.api.authenticate()
-kaggle.api.dataset_download_files('nikhilnayak123/5-million-song-lyrics-dataset', path='/path/to/save', unzip=True)
+import kaggle # make sure you've run `pip install kaggle`
 
+kaggle.api.authenticate()
+kaggle.api.dataset_download_files(
+    'nikhilnayak123/5-million-song-lyrics-dataset',
+    path='.',
+    unzip=True
+)
 
 db = PeachDB.create(
     project_name="spoti_vibe",
-    csv_path="/path/to/local/csv",
+    csv_path='./ds2.csv',  # dataset name as observed on Kaggle
     column_to_embed="lyrics",
     id_column_name="id",
     max_rows=None,
     distance_metric="cosine",
     embedding_backend="exact_cpu",
     embedding_generator="sentence_transformer_L12",
 )
 
 db.deploy() # Public URL will be printed to console
 ```
-And that's it! You should now have a publicly available server that can listen to query requests from the user on: `GET <PUBLIC_URL>/query?text=''&top_k=5`
+
+And that's it! You should now have a publicly available server that can listen to query requests from the user on: `GET <PUBLIC_URL>/query?text='Happy, upbeat summer'&top_k=5`
 
 
 ## FAQs
 Q) How can I delete a project?
 Run `db.delete(project_name="my_app")`
 
 ## Get Involved
```

### Comparing `peachdb-0.0.3/setup.py` & `peachdb-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # read the contents README
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="peachdb",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     install_requires=requirements,
     dependency_links=["https://download.pytorch.org/whl/cu113"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     project_urls={
```

