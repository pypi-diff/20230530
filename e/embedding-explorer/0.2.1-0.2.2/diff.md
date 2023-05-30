# Comparing `tmp/embedding_explorer-0.2.1.tar.gz` & `tmp/embedding_explorer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedding_explorer-0.2.1.tar", max compression
+gzip compressed data, was "embedding_explorer-0.2.2.tar", max compression
```

## Comparing `embedding_explorer-0.2.1.tar` & `embedding_explorer-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1095 2023-03-13 11:52:25.053838 embedding_explorer-0.2.1/LICENSE
--rw-r--r--   0        0        0       95 2023-03-13 11:52:25.057838 embedding_explorer-0.2.1/README.md
--rw-r--r--   0        0        0      142 2023-03-27 13:50:12.710655 embedding_explorer-0.2.1/embedding_explorer/__init__.py
--rw-r--r--   0        0        0     4796 2023-05-30 07:29:44.478265 embedding_explorer-0.2.1/embedding_explorer/app.py
--rw-r--r--   0        0        0    16170 2023-03-21 14:13:23.726074 embedding_explorer-0.2.1/embedding_explorer/assets/favicon.ico
--rw-r--r--   0        0        0     2087 2023-05-30 07:32:54.398474 embedding_explorer-0.2.1/embedding_explorer/blueprints/dashboard.py
--rw-r--r--   0        0        0     5295 2023-05-30 07:32:35.514453 embedding_explorer-0.2.1/embedding_explorer/blueprints/explorer.py
--rw-r--r--   0        0        0     2299 2023-05-30 07:36:09.082811 embedding_explorer-0.2.1/embedding_explorer/components/model_card.py
--rw-r--r--   0        0        0     2000 2023-03-27 13:28:01.367900 embedding_explorer-0.2.1/embedding_explorer/components/network.py
--rw-r--r--   0        0        0     1078 2023-05-30 07:36:19.538867 embedding_explorer-0.2.1/embedding_explorer/components/slider.py
--rw-r--r--   0        0        0     4004 2023-05-30 07:59:25.331036 embedding_explorer-0.2.1/embedding_explorer/components/word_selector.py
--rw-r--r--   0        0        0      886 2023-05-30 07:29:20.382238 embedding_explorer-0.2.1/embedding_explorer/model.py
--rw-r--r--   0        0        0     5920 2023-05-30 08:37:04.843835 embedding_explorer-0.2.1/embedding_explorer/plots/network.py
--rw-r--r--   0        0        0     5843 2023-03-27 14:42:08.501085 embedding_explorer-0.2.1/embedding_explorer/prepare/semkern.py
--rw-r--r--   0        0        0     1147 2023-05-30 07:36:59.059074 embedding_explorer-0.2.1/embedding_explorer/prepare/thumbnails.py
--rw-r--r--   0        0        0      684 2023-05-30 08:39:46.464153 embedding_explorer-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 embedding_explorer-0.2.1/setup.py
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 embedding_explorer-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-03-13 11:52:25.053838 embedding_explorer-0.2.2/LICENSE
+-rw-r--r--   0        0        0       95 2023-03-13 11:52:25.057838 embedding_explorer-0.2.2/README.md
+-rw-r--r--   0        0        0      142 2023-03-27 13:50:12.710655 embedding_explorer-0.2.2/embedding_explorer/__init__.py
+-rw-r--r--   0        0        0     4796 2023-05-30 07:29:44.478265 embedding_explorer-0.2.2/embedding_explorer/app.py
+-rw-r--r--   0        0        0    16170 2023-03-21 14:13:23.726074 embedding_explorer-0.2.2/embedding_explorer/assets/favicon.ico
+-rw-r--r--   0        0        0     2087 2023-05-30 07:32:54.398474 embedding_explorer-0.2.2/embedding_explorer/blueprints/dashboard.py
+-rw-r--r--   0        0        0     5295 2023-05-30 07:32:35.514453 embedding_explorer-0.2.2/embedding_explorer/blueprints/explorer.py
+-rw-r--r--   0        0        0     2299 2023-05-30 07:36:09.082811 embedding_explorer-0.2.2/embedding_explorer/components/model_card.py
+-rw-r--r--   0        0        0     2000 2023-03-27 13:28:01.367900 embedding_explorer-0.2.2/embedding_explorer/components/network.py
+-rw-r--r--   0        0        0     1078 2023-05-30 07:36:19.538867 embedding_explorer-0.2.2/embedding_explorer/components/slider.py
+-rw-r--r--   0        0        0     4004 2023-05-30 07:59:25.331036 embedding_explorer-0.2.2/embedding_explorer/components/word_selector.py
+-rw-r--r--   0        0        0      886 2023-05-30 07:29:20.382238 embedding_explorer-0.2.2/embedding_explorer/model.py
+-rw-r--r--   0        0        0     5920 2023-05-30 08:37:04.843835 embedding_explorer-0.2.2/embedding_explorer/plots/network.py
+-rw-r--r--   0        0        0     5860 2023-05-30 08:45:09.132836 embedding_explorer-0.2.2/embedding_explorer/prepare/semkern.py
+-rw-r--r--   0        0        0     1147 2023-05-30 07:36:59.059074 embedding_explorer-0.2.2/embedding_explorer/prepare/thumbnails.py
+-rw-r--r--   0        0        0      684 2023-05-30 08:46:46.517136 embedding_explorer-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 embedding_explorer-0.2.2/setup.py
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 embedding_explorer-0.2.2/PKG-INFO
```

### Comparing `embedding_explorer-0.2.1/LICENSE` & `embedding_explorer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.1/embedding_explorer/app.py` & `embedding_explorer-0.2.2/embedding_explorer/app.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.1/embedding_explorer/assets/favicon.ico` & `embedding_explorer-0.2.2/embedding_explorer/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.1/embedding_explorer/blueprints/dashboard.py` & `embedding_explorer-0.2.2/embedding_explorer/blueprints/dashboard.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.1/embedding_explorer/blueprints/explorer.py` & `embedding_explorer-0.2.2/embedding_explorer/blueprints/explorer.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.1/embedding_explorer/components/model_card.py` & `embedding_explorer-0.2.2/embedding_explorer/components/model_card.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.1/embedding_explorer/components/network.py` & `embedding_explorer-0.2.2/embedding_explorer/components/network.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.1/embedding_explorer/components/slider.py` & `embedding_explorer-0.2.2/embedding_explorer/components/slider.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.1/embedding_explorer/components/word_selector.py` & `embedding_explorer-0.2.2/embedding_explorer/components/word_selector.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.1/embedding_explorer/model.py` & `embedding_explorer-0.2.2/embedding_explorer/model.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.1/embedding_explorer/plots/network.py` & `embedding_explorer-0.2.2/embedding_explorer/plots/network.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.1/embedding_explorer/prepare/semkern.py` & `embedding_explorer-0.2.2/embedding_explorer/prepare/semkern.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     return connections
 
 
 def calculate_dist_matrix(
     kernel_words: List[int], embeddings: np.ndarray
 ) -> np.ndarray:
     """Creates distance matrix of kernel words."""
-    delta = pairwise_distances(embeddings[kernel_words])
+    delta = pairwise_distances(embeddings[kernel_words], metric="cosine")
     # Cut connections between the word and itself.
     np.fill_diagonal(delta, 0.0)
     # Cut connections that are over median distance
     # delta[delta < np.median(delta)] = 0.0
     return delta
```

### Comparing `embedding_explorer-0.2.1/embedding_explorer/prepare/thumbnails.py` & `embedding_explorer-0.2.2/embedding_explorer/prepare/thumbnails.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.1/pyproject.toml` & `embedding_explorer-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length=79
 
 [tool.ruff]
 line-length=79
 
 [tool.poetry]
 name = "embedding-explorer"
-version = "0.2.1"
+version = "0.2.2"
 description = "Tools for interactive visual inspection of static word embedding models."
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "embedding_explorer"}]
 
 [tool.poetry.dependencies]
```

### Comparing `embedding_explorer-0.2.1/setup.py` & `embedding_explorer-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'numpy>=1.23.0',
  'pandas>=1.5.2,<1.6.0',
  'scikit-learn>=1.1.0,<1.2.0',
  'wordcloud>=1.8.2.2,<1.9.0.0']
 
 setup_kwargs = {
     'name': 'embedding-explorer',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Tools for interactive visual inspection of static word embedding models.',
     'long_description': '# embedding-explorer\nTools for interactive visual exploration of static word embedding models.\n',
     'author': 'Márton Kardos',
     'author_email': 'power.up1163@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `embedding_explorer-0.2.1/PKG-INFO` & `embedding_explorer-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedding-explorer
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tools for interactive visual inspection of static word embedding models.
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

