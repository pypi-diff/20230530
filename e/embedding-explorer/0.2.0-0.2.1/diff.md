# Comparing `tmp/embedding_explorer-0.2.0.tar.gz` & `tmp/embedding_explorer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedding_explorer-0.2.0.tar", max compression
+gzip compressed data, was "embedding_explorer-0.2.1.tar", max compression
```

## Comparing `embedding_explorer-0.2.0.tar` & `embedding_explorer-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1095 2023-03-13 11:52:25.053838 embedding_explorer-0.2.0/LICENSE
--rw-r--r--   0        0        0       95 2023-03-13 11:52:25.057838 embedding_explorer-0.2.0/README.md
--rw-r--r--   0        0        0      142 2023-03-27 13:50:12.710655 embedding_explorer-0.2.0/embedding_explorer/__init__.py
--rw-r--r--   0        0        0     4796 2023-05-30 07:29:44.478265 embedding_explorer-0.2.0/embedding_explorer/app.py
--rw-r--r--   0        0        0    16170 2023-03-21 14:13:23.726074 embedding_explorer-0.2.0/embedding_explorer/assets/favicon.ico
--rw-r--r--   0        0        0     2087 2023-05-30 07:32:54.398474 embedding_explorer-0.2.0/embedding_explorer/blueprints/dashboard.py
--rw-r--r--   0        0        0     5295 2023-05-30 07:32:35.514453 embedding_explorer-0.2.0/embedding_explorer/blueprints/explorer.py
--rw-r--r--   0        0        0     2299 2023-05-30 07:36:09.082811 embedding_explorer-0.2.0/embedding_explorer/components/model_card.py
--rw-r--r--   0        0        0     2000 2023-03-27 13:28:01.367900 embedding_explorer-0.2.0/embedding_explorer/components/network.py
--rw-r--r--   0        0        0     1078 2023-05-30 07:36:19.538867 embedding_explorer-0.2.0/embedding_explorer/components/slider.py
--rw-r--r--   0        0        0     4004 2023-05-30 07:59:25.331036 embedding_explorer-0.2.0/embedding_explorer/components/word_selector.py
--rw-r--r--   0        0        0      886 2023-05-30 07:29:20.382238 embedding_explorer-0.2.0/embedding_explorer/model.py
--rw-r--r--   0        0        0     5795 2023-05-30 08:04:52.399673 embedding_explorer-0.2.0/embedding_explorer/plots/network.py
--rw-r--r--   0        0        0     5843 2023-03-27 14:42:08.501085 embedding_explorer-0.2.0/embedding_explorer/prepare/semkern.py
--rw-r--r--   0        0        0     1147 2023-05-30 07:36:59.059074 embedding_explorer-0.2.0/embedding_explorer/prepare/thumbnails.py
--rw-r--r--   0        0        0      684 2023-05-30 07:34:07.926554 embedding_explorer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 embedding_explorer-0.2.0/setup.py
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 embedding_explorer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-03-13 11:52:25.053838 embedding_explorer-0.2.1/LICENSE
+-rw-r--r--   0        0        0       95 2023-03-13 11:52:25.057838 embedding_explorer-0.2.1/README.md
+-rw-r--r--   0        0        0      142 2023-03-27 13:50:12.710655 embedding_explorer-0.2.1/embedding_explorer/__init__.py
+-rw-r--r--   0        0        0     4796 2023-05-30 07:29:44.478265 embedding_explorer-0.2.1/embedding_explorer/app.py
+-rw-r--r--   0        0        0    16170 2023-03-21 14:13:23.726074 embedding_explorer-0.2.1/embedding_explorer/assets/favicon.ico
+-rw-r--r--   0        0        0     2087 2023-05-30 07:32:54.398474 embedding_explorer-0.2.1/embedding_explorer/blueprints/dashboard.py
+-rw-r--r--   0        0        0     5295 2023-05-30 07:32:35.514453 embedding_explorer-0.2.1/embedding_explorer/blueprints/explorer.py
+-rw-r--r--   0        0        0     2299 2023-05-30 07:36:09.082811 embedding_explorer-0.2.1/embedding_explorer/components/model_card.py
+-rw-r--r--   0        0        0     2000 2023-03-27 13:28:01.367900 embedding_explorer-0.2.1/embedding_explorer/components/network.py
+-rw-r--r--   0        0        0     1078 2023-05-30 07:36:19.538867 embedding_explorer-0.2.1/embedding_explorer/components/slider.py
+-rw-r--r--   0        0        0     4004 2023-05-30 07:59:25.331036 embedding_explorer-0.2.1/embedding_explorer/components/word_selector.py
+-rw-r--r--   0        0        0      886 2023-05-30 07:29:20.382238 embedding_explorer-0.2.1/embedding_explorer/model.py
+-rw-r--r--   0        0        0     5920 2023-05-30 08:37:04.843835 embedding_explorer-0.2.1/embedding_explorer/plots/network.py
+-rw-r--r--   0        0        0     5843 2023-03-27 14:42:08.501085 embedding_explorer-0.2.1/embedding_explorer/prepare/semkern.py
+-rw-r--r--   0        0        0     1147 2023-05-30 07:36:59.059074 embedding_explorer-0.2.1/embedding_explorer/prepare/thumbnails.py
+-rw-r--r--   0        0        0      684 2023-05-30 08:39:46.464153 embedding_explorer-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 embedding_explorer-0.2.1/setup.py
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 embedding_explorer-0.2.1/PKG-INFO
```

### Comparing `embedding_explorer-0.2.0/LICENSE` & `embedding_explorer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.0/embedding_explorer/app.py` & `embedding_explorer-0.2.1/embedding_explorer/app.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.0/embedding_explorer/assets/favicon.ico` & `embedding_explorer-0.2.1/embedding_explorer/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.0/embedding_explorer/blueprints/dashboard.py` & `embedding_explorer-0.2.1/embedding_explorer/blueprints/dashboard.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.0/embedding_explorer/blueprints/explorer.py` & `embedding_explorer-0.2.1/embedding_explorer/blueprints/explorer.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.0/embedding_explorer/components/model_card.py` & `embedding_explorer-0.2.1/embedding_explorer/components/model_card.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.0/embedding_explorer/components/network.py` & `embedding_explorer-0.2.1/embedding_explorer/components/network.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.0/embedding_explorer/components/slider.py` & `embedding_explorer-0.2.1/embedding_explorer/components/slider.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.0/embedding_explorer/components/word_selector.py` & `embedding_explorer-0.2.1/embedding_explorer/components/word_selector.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.0/embedding_explorer/model.py` & `embedding_explorer-0.2.1/embedding_explorer/model.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.0/embedding_explorer/plots/network.py` & `embedding_explorer-0.2.1/embedding_explorer/plots/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """Plotting utilities for networks."""
 from typing import Tuple
 
 import numpy as np
 import plotly.graph_objects as go
 from plotly.express.colors import cyclical, sample_colorscale
 
-from embedding_explorer.prepare.semkern import (
-    SemanticKernel,
-    calculate_n_connections,
-    calculate_positions,
-    get_closest_seed,
-)
+from embedding_explorer.prepare.semkern import (SemanticKernel,
+                                                calculate_n_connections,
+                                                calculate_positions,
+                                                get_closest_seed)
 
 
 def _edge_pos(edges: np.ndarray, x_y: np.ndarray) -> np.ndarray:
     """
     Through a series of nasty numpy tricks, that I® wrote
     this function transforms edges and either the x or the y positions
     of nodes to the x or y positions for the lines in the plotly figure.
@@ -76,15 +74,15 @@
     y: np.ndarray,
     distance_matrix: np.ndarray,
 ) -> go.Figure:
     """Adds edges to a figure as shapes."""
     opacities = np.array(
         [-distance_matrix[start, end] for start, end in edges]
     )
-    opacities = minmax(opacities)
+    opacities = minmax(opacities) / 1.5
     for (start, end), opacity in zip(edges, opacities):
         fig.add_shape(
             dict(
                 type="line",
                 xref="x",
                 yref="y",
                 x0=x[start],
@@ -113,42 +111,42 @@
 ) -> Tuple[go.Scatter, go.Scatter, go.Scatter]:
     """Creates node traces for the different levels of association."""
     closest_seed = get_closest_seed(kernel)
     scale = get_seed_colors(kernel)
     is_seed = kernel.priorities == 0
     sizes = calculate_n_connections(kernel.connections)
     sizes = (sizes / np.max(sizes)) * 60
-    seed_trace = go.Scattergl(
+    seed_trace = go.Scatter(
         name="",
         text=kernel.vocabulary[is_seed],
         x=x[is_seed],
         y=y[is_seed],
         mode="markers+text",
         hoverinfo="text",
         marker=dict(
             color=scale[closest_seed[is_seed]], size=sizes[is_seed], opacity=1
         ),
         textfont=dict(size=12, color="white"),
     )
     is_first_level = kernel.priorities == 1
-    first_level_trace = go.Scattergl(
+    first_level_trace = go.Scatter(
         name="",
         text=kernel.vocabulary[is_first_level],
         x=x[is_first_level],
         y=y[is_first_level],
         mode="markers+text",
         hoverinfo="text",
         marker=dict(
             color=scale[closest_seed[is_first_level]],
             size=sizes[is_first_level],
             opacity=0.6,
         ),
     )
     is_second_level = kernel.priorities == 2
-    second_level_trace = go.Scattergl(
+    second_level_trace = go.Scatter(
         name="",
         text=kernel.vocabulary[is_second_level],
         x=x[is_second_level],
         y=y[is_second_level],
         mode="markers+text",
         hoverinfo="text",
         marker=dict(
```

### Comparing `embedding_explorer-0.2.0/embedding_explorer/prepare/semkern.py` & `embedding_explorer-0.2.1/embedding_explorer/prepare/semkern.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.0/embedding_explorer/prepare/thumbnails.py` & `embedding_explorer-0.2.1/embedding_explorer/prepare/thumbnails.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.2.0/pyproject.toml` & `embedding_explorer-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length=79
 
 [tool.ruff]
 line-length=79
 
 [tool.poetry]
 name = "embedding-explorer"
-version = "0.2.0"
+version = "0.2.1"
 description = "Tools for interactive visual inspection of static word embedding models."
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "embedding_explorer"}]
 
 [tool.poetry.dependencies]
```

### Comparing `embedding_explorer-0.2.0/setup.py` & `embedding_explorer-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'numpy>=1.23.0',
  'pandas>=1.5.2,<1.6.0',
  'scikit-learn>=1.1.0,<1.2.0',
  'wordcloud>=1.8.2.2,<1.9.0.0']
 
 setup_kwargs = {
     'name': 'embedding-explorer',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Tools for interactive visual inspection of static word embedding models.',
     'long_description': '# embedding-explorer\nTools for interactive visual exploration of static word embedding models.\n',
     'author': 'Márton Kardos',
     'author_email': 'power.up1163@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `embedding_explorer-0.2.0/PKG-INFO` & `embedding_explorer-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedding-explorer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tools for interactive visual inspection of static word embedding models.
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

