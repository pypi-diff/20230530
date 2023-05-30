# Comparing `tmp/embedding_explorer-0.1.4.tar.gz` & `tmp/embedding_explorer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedding_explorer-0.1.4.tar", max compression
+gzip compressed data, was "embedding_explorer-0.2.0.tar", max compression
```

## Comparing `embedding_explorer-0.1.4.tar` & `embedding_explorer-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1095 2023-03-13 11:52:25.053838 embedding_explorer-0.1.4/LICENSE
--rw-r--r--   0        0        0       95 2023-03-13 11:52:25.057838 embedding_explorer-0.1.4/README.md
--rw-r--r--   0        0        0      142 2023-03-27 13:50:12.710655 embedding_explorer-0.1.4/embedding_explorer/__init__.py
--rw-r--r--   0        0        0     4732 2023-04-17 11:46:15.047242 embedding_explorer-0.1.4/embedding_explorer/app.py
--rw-r--r--   0        0        0    16170 2023-03-21 14:13:23.726074 embedding_explorer-0.1.4/embedding_explorer/assets/favicon.ico
--rw-r--r--   0        0        0     2041 2023-04-17 11:40:06.279827 embedding_explorer-0.1.4/embedding_explorer/blueprints/dashboard.py
--rw-r--r--   0        0        0     5273 2023-04-17 13:17:44.237811 embedding_explorer-0.1.4/embedding_explorer/blueprints/explorer.py
--rw-r--r--   0        0        0     2277 2023-03-27 13:27:51.091877 embedding_explorer-0.1.4/embedding_explorer/components/model_card.py
--rw-r--r--   0        0        0     2000 2023-03-27 13:28:01.367900 embedding_explorer-0.1.4/embedding_explorer/components/network.py
--rw-r--r--   0        0        0     1106 2023-03-17 13:45:00.203784 embedding_explorer-0.1.4/embedding_explorer/components/slider.py
--rw-r--r--   0        0        0     4007 2023-04-17 13:17:17.169774 embedding_explorer-0.1.4/embedding_explorer/components/word_selector.py
--rw-r--r--   0        0        0      853 2023-03-27 13:36:18.356965 embedding_explorer-0.1.4/embedding_explorer/model.py
--rw-r--r--   0        0        0     4907 2023-03-20 14:01:46.998402 embedding_explorer-0.1.4/embedding_explorer/plots/network.py
--rw-r--r--   0        0        0     5843 2023-03-27 14:42:08.501085 embedding_explorer-0.1.4/embedding_explorer/prepare/semkern.py
--rw-r--r--   0        0        0     1125 2023-03-27 14:47:02.041747 embedding_explorer-0.1.4/embedding_explorer/prepare/thumbnails.py
--rw-r--r--   0        0        0      684 2023-04-17 13:22:11.570119 embedding_explorer-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 embedding_explorer-0.1.4/setup.py
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 embedding_explorer-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-03-13 11:52:25.053838 embedding_explorer-0.2.0/LICENSE
+-rw-r--r--   0        0        0       95 2023-03-13 11:52:25.057838 embedding_explorer-0.2.0/README.md
+-rw-r--r--   0        0        0      142 2023-03-27 13:50:12.710655 embedding_explorer-0.2.0/embedding_explorer/__init__.py
+-rw-r--r--   0        0        0     4796 2023-05-30 07:29:44.478265 embedding_explorer-0.2.0/embedding_explorer/app.py
+-rw-r--r--   0        0        0    16170 2023-03-21 14:13:23.726074 embedding_explorer-0.2.0/embedding_explorer/assets/favicon.ico
+-rw-r--r--   0        0        0     2087 2023-05-30 07:32:54.398474 embedding_explorer-0.2.0/embedding_explorer/blueprints/dashboard.py
+-rw-r--r--   0        0        0     5295 2023-05-30 07:32:35.514453 embedding_explorer-0.2.0/embedding_explorer/blueprints/explorer.py
+-rw-r--r--   0        0        0     2299 2023-05-30 07:36:09.082811 embedding_explorer-0.2.0/embedding_explorer/components/model_card.py
+-rw-r--r--   0        0        0     2000 2023-03-27 13:28:01.367900 embedding_explorer-0.2.0/embedding_explorer/components/network.py
+-rw-r--r--   0        0        0     1078 2023-05-30 07:36:19.538867 embedding_explorer-0.2.0/embedding_explorer/components/slider.py
+-rw-r--r--   0        0        0     4004 2023-05-30 07:59:25.331036 embedding_explorer-0.2.0/embedding_explorer/components/word_selector.py
+-rw-r--r--   0        0        0      886 2023-05-30 07:29:20.382238 embedding_explorer-0.2.0/embedding_explorer/model.py
+-rw-r--r--   0        0        0     5795 2023-05-30 08:04:52.399673 embedding_explorer-0.2.0/embedding_explorer/plots/network.py
+-rw-r--r--   0        0        0     5843 2023-03-27 14:42:08.501085 embedding_explorer-0.2.0/embedding_explorer/prepare/semkern.py
+-rw-r--r--   0        0        0     1147 2023-05-30 07:36:59.059074 embedding_explorer-0.2.0/embedding_explorer/prepare/thumbnails.py
+-rw-r--r--   0        0        0      684 2023-05-30 07:34:07.926554 embedding_explorer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 embedding_explorer-0.2.0/setup.py
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 embedding_explorer-0.2.0/PKG-INFO
```

### Comparing `embedding_explorer-0.1.4/LICENSE` & `embedding_explorer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.4/embedding_explorer/app.py` & `embedding_explorer-0.2.0/embedding_explorer/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 from typing import Callable, Dict, Optional
 
 from dash_extensions.enrich import Dash, DashBlueprint
 
 from embedding_explorer.blueprints.dashboard import create_dashboard
 from embedding_explorer.blueprints.explorer import create_explorer
-from embedding_explorer.model import Model
+from embedding_explorer.model import StaticEmbeddings
 
 
 def get_dash_app(blueprint: DashBlueprint, **kwargs) -> Dash:
     """Returns app based on a blueprint with
     tailwindcss and font awesome added."""
     additional_scripts = kwargs.get("external_scripts", [])
     use_pages = kwargs.get("use_pages", False)
@@ -100,21 +100,21 @@
         return thread
     else:
         open_url(url)
         app.run_server(port=port)
 
 
 def show_explorer(
-    model: Model, port: int = 8050, fuzzy_search: bool = False
+    model: StaticEmbeddings, port: int = 8050, fuzzy_search: bool = False
 ) -> Optional[threading.Thread]:
     """Visually inspect word embedding model with embedding-explorer.
 
     Parameters
     ----------
-    model: Model
+    model: StaticEmbeddings
         Named tuple of model vocabulary and matrix of embeddings.
     port: int
         Port for the app to run on.
     fuzzy_search: bool, default False
         Specifies whether you want to fuzzy search in the vocabulary.
         This is recommended for production use, but the index takes
         time to set up, therefore the startup time is expected to
@@ -128,21 +128,23 @@
     """
     blueprint = create_explorer(model=model, fuzzy_search=fuzzy_search)
     app = get_dash_app(blueprint=blueprint, use_pages=False)
     return run_app(app, port=port)
 
 
 def show_dashboard(
-    models: Dict[str, Model], port: int = 8050, fuzzy_search: bool = False
+    models: Dict[str, StaticEmbeddings],
+    port: int = 8050,
+    fuzzy_search: bool = False,
 ) -> Optional[threading.Thread]:
     """Show dashboard for all given word embeddings.
 
     Parameters
     ----------
-    models: dict of str to Model
+    models: dict of str to StaticEmbeddings
         Mapping of model names to models.
     fuzzy_search: bool, default False
         Specifies whether you want to fuzzy search in the vocabulary.
         This is recommended for production use, but the index takes
         time to set up, therefore the startup time is expected to
         be greater.
```

### Comparing `embedding_explorer-0.1.4/embedding_explorer/assets/favicon.ico` & `embedding_explorer-0.2.0/embedding_explorer/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.4/embedding_explorer/blueprints/dashboard.py` & `embedding_explorer-0.2.0/embedding_explorer/blueprints/dashboard.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 from urllib.parse import quote
 
 import dash_mantine_components as dmc
 from dash_extensions.enrich import Dash, DashBlueprint, dash, dcc, html
 
 from embedding_explorer.blueprints.explorer import create_explorer
 from embedding_explorer.components.model_card import create_card
-from embedding_explorer.model import Model
+from embedding_explorer.model import StaticEmbeddings
 
 
-def create_dashboard(models: Dict[str, Model], fuzzy_search: bool = False):
-    """Creates dashboard for all embedding models.
+def create_dashboard(
+    models: Dict[str, StaticEmbeddings], fuzzy_search: bool = False
+):
+    """Creates dashboard for all static embedding models.
 
     Parameters
     ----------
-    models: dict of str to Model
+    models: dict of str to StaticEmbeddings
         Mapping of names to models.
     """
     print("Creating Dashboard")
     dashboard = DashBlueprint()
 
     # Collecting cards and registering pages
     cards = []
```

### Comparing `embedding_explorer-0.1.4/embedding_explorer/blueprints/explorer.py` & `embedding_explorer-0.2.0/embedding_explorer/blueprints/explorer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Blueprint for the main application."""
 import dash_mantine_components as dmc
 import numpy as np
 from dash_extensions.enrich import DashBlueprint, dcc, html
 
 from embedding_explorer.components.network import create_network
 from embedding_explorer.components.word_selector import create_word_selector
-from embedding_explorer.model import Model
+from embedding_explorer.model import StaticEmbeddings
 
 
 def create_explorer(
-    model: Model, model_name: str = "", fuzzy_search: bool = False
+    model: StaticEmbeddings, model_name: str = "", fuzzy_search: bool = False
 ) -> DashBlueprint:
     # --------[ Collecting blueprints ]--------
     word_selector = create_word_selector(
         vocab=model.vocab, model_name=model_name, fuzzy_search=fuzzy_search
     )
     network = create_network(
         vocab=model.vocab, embeddings=model.embeddings, model_name=model_name
```

### Comparing `embedding_explorer-0.1.4/embedding_explorer/components/model_card.py` & `embedding_explorer-0.2.0/embedding_explorer/components/model_card.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from urllib.parse import quote
 
 import dash_mantine_components as dmc
 import numpy as np
 from dash_extensions.enrich import DashBlueprint, html
 from dash_iconify import DashIconify
 
-from embedding_explorer.model import Model
+from embedding_explorer.model import StaticEmbeddings
 from embedding_explorer.prepare.thumbnails import generate_thumbnail
 
 COOL_ICONS = [
     "wind",
     "zap",
     "anchor",
     "cloud-drizzle",
@@ -24,15 +24,15 @@
     "smile",
     "sun",
     "truck",
     "umbrella",
 ]
 
 
-def create_card(model: Model, model_name: str) -> DashBlueprint:
+def create_card(model: StaticEmbeddings, model_name: str) -> DashBlueprint:
     """Creates card for model."""
     card = DashBlueprint()
     thumbnail = generate_thumbnail(model)
     encoded_thumbnail = base64.b64encode(thumbnail.encode("utf-8")).decode(
         "utf-8"
     )
     random_icon = COOL_ICONS[np.random.randint(0, len(COOL_ICONS))]
```

### Comparing `embedding_explorer-0.1.4/embedding_explorer/components/network.py` & `embedding_explorer-0.2.0/embedding_explorer/components/network.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.4/embedding_explorer/components/slider.py` & `embedding_explorer-0.2.0/embedding_explorer/components/slider.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Association slider components."""
-from typing import Optional
 
 import dash_mantine_components as dmc
 from dash_extensions.enrich import DashBlueprint
 from typing_extensions import TypedDict
 
 Gradient = TypedDict("Gradient", {"from": str, "to": str, "deg": int})
```

### Comparing `embedding_explorer-0.1.4/embedding_explorer/components/word_selector.py` & `embedding_explorer-0.2.0/embedding_explorer/components/word_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 
     word_selector = DashBlueprint()
     vocab_lookup = {word: index for index, word in enumerate(vocab)}
     if fuzzy_search:
         print("Indexing vocabulary for fuzzy search")
         vectorizer = make_pipeline(
             TfidfVectorizer(
-                analyzer="char", ngram_range=(1, 5), max_features=50_000
+                analyzer="char", ngram_range=(1, 4), max_features=20_000
             ),
-            NMF(n_components=10),
+            NMF(n_components=25),
         )
         fuzzy_process = Process(
             vectorizer,
-            metric="euclidean",
+            metric="cosine",
             low_memory=True,
         )
         fuzzy_process.index(vocab)
         print("Indexing done")
     else:
         fuzzy_process = DummyProcess()
```

### Comparing `embedding_explorer-0.1.4/embedding_explorer/model.py` & `embedding_explorer-0.2.0/embedding_explorer/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from pathlib import Path
 from typing import NamedTuple
 
 import numpy as np
 
 
-class Model(NamedTuple):
+class StaticEmbeddings(NamedTuple):
     vocab: np.ndarray
     embeddings: np.ndarray
 
     @classmethod
-    def from_keyed_vectors(cls, keyed_vectors) -> "Model":
+    def from_keyed_vectors(cls, keyed_vectors) -> "StaticEmbeddings":
         """Creates static embedding model from keyed vectors in Gensim."""
         vocab = np.array(keyed_vectors.index_to_key)
         embeddings = keyed_vectors.vectors
         return cls(vocab=vocab, embeddings=embeddings)
 
     def save(self, path: Path) -> None:
         """Saves static embedding model to the given path."""
         np.savez(path, vocab=self.vocab, embeddings=self.embeddings)
 
     @classmethod
-    def load(cls, path: Path) -> "Model":
+    def load(cls, path: Path) -> "StaticEmbeddings":
         """Loads static word embedding model from disk"""
         npzfile = np.load(path)
         return cls(vocab=npzfile["vocab"], embeddings=npzfile["embeddings"])
```

### Comparing `embedding_explorer-0.1.4/embedding_explorer/plots/network.py` & `embedding_explorer-0.2.0/embedding_explorer/plots/network.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Plotting utilities for networks."""
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Tuple
 
 import numpy as np
 import plotly.graph_objects as go
 from plotly.express.colors import cyclical, sample_colorscale
 
-from embedding_explorer.prepare.semkern import (SemanticKernel,
-                                                calculate_n_connections,
-                                                calculate_positions,
-                                                get_closest_seed)
+from embedding_explorer.prepare.semkern import (
+    SemanticKernel,
+    calculate_n_connections,
+    calculate_positions,
+    get_closest_seed,
+)
 
 
 def _edge_pos(edges: np.ndarray, x_y: np.ndarray) -> np.ndarray:
     """
     Through a series of nasty numpy tricks, that I® wrote
     this function transforms edges and either the x or the y positions
     of nodes to the x or y positions for the lines in the plotly figure.
@@ -58,14 +60,48 @@
         showlegend=False,
         opacity=0.2,
         line=dict(color="black"),
     )
     return trace
 
 
+def minmax(a: np.ndarray) -> np.ndarray:
+    """Min-max normalizes an array."""
+    return (a - np.min(a)) / (np.max(a) - np.min(a))
+
+
+def add_edges(
+    fig: go.Figure,
+    edges: np.ndarray,
+    x: np.ndarray,
+    y: np.ndarray,
+    distance_matrix: np.ndarray,
+) -> go.Figure:
+    """Adds edges to a figure as shapes."""
+    opacities = np.array(
+        [-distance_matrix[start, end] for start, end in edges]
+    )
+    opacities = minmax(opacities)
+    for (start, end), opacity in zip(edges, opacities):
+        fig.add_shape(
+            dict(
+                type="line",
+                xref="x",
+                yref="y",
+                x0=x[start],
+                y0=y[start],
+                x1=x[end],
+                y1=y[end],
+                layer="below",
+                opacity=opacity,
+            )
+        )
+    return fig
+
+
 def get_seed_colors(kernel: SemanticKernel) -> np.ndarray:
     """Returns array of RGB colors for each seed."""
     n_seeds = np.sum(kernel.priorities == 0)
     samplepoints = np.arange(n_seeds) / n_seeds
     colors = sample_colorscale(
         colorscale=cyclical.Phase, samplepoints=samplepoints
     )
@@ -77,42 +113,42 @@
 ) -> Tuple[go.Scatter, go.Scatter, go.Scatter]:
     """Creates node traces for the different levels of association."""
     closest_seed = get_closest_seed(kernel)
     scale = get_seed_colors(kernel)
     is_seed = kernel.priorities == 0
     sizes = calculate_n_connections(kernel.connections)
     sizes = (sizes / np.max(sizes)) * 60
-    seed_trace = go.Scatter(
+    seed_trace = go.Scattergl(
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
-    first_level_trace = go.Scatter(
+    first_level_trace = go.Scattergl(
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
-    second_level_trace = go.Scatter(
+    second_level_trace = go.Scattergl(
         name="",
         text=kernel.vocabulary[is_second_level],
         x=x[is_second_level],
         y=y[is_second_level],
         mode="markers+text",
         hoverinfo="text",
         marker=dict(
@@ -125,17 +161,25 @@
 
 
 def plot_semantic_kernel(kernel: SemanticKernel) -> go.Figure:
     """Plots semantic kernel."""
     x, y = calculate_positions(kernel.distance_matrix)
 
     node_traces = create_node_traces(x=x, y=y, kernel=kernel)
-    edge_trace = create_edge_trace(x=x, y=y, edges=kernel.connections)
+    # edge_trace = create_edge_trace(x=x, y=y, edges=kernel.connections)
 
-    figure = go.Figure(data=[edge_trace, *node_traces])
+    # figure = go.Figure(data=[edge_trace, *node_traces])
+    figure = go.Figure(data=[*node_traces])
+    add_edges(
+        figure,
+        edges=kernel.connections,
+        x=x,
+        y=y,
+        distance_matrix=kernel.distance_matrix,
+    )
     figure.update_xaxes(
         showticklabels=False,
         title="",
         gridcolor="#e5e7eb",
         linecolor="#f9fafb",
         linewidth=6,
         mirror=True,
```

### Comparing `embedding_explorer-0.1.4/embedding_explorer/prepare/semkern.py` & `embedding_explorer-0.2.0/embedding_explorer/prepare/semkern.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.4/embedding_explorer/prepare/thumbnails.py` & `embedding_explorer-0.2.0/embedding_explorer/prepare/thumbnails.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import string
 
 import numpy as np
 from wordcloud import WordCloud
 
-from embedding_explorer.model import Model
+from embedding_explorer.model import StaticEmbeddings
 
 
 def is_alpha(word: str) -> bool:
     return all((c.isalpha() or c in string.printable for c in word))
 
 
 COLORMAPS = [
@@ -17,15 +17,15 @@
     "BuGn",
     "PuRd",
     "Purples",
     "Blues",
 ]
 
 
-def generate_thumbnail(model: Model) -> str:
+def generate_thumbnail(model: StaticEmbeddings) -> str:
     """Generates thumbnail for given model and returns it as SVG string."""
     vocab = model.vocab
     alphabetical = np.vectorize(is_alpha)(vocab)
     if vocab.shape[0] > 30:
         vocab = vocab[alphabetical]
     n_vocab = vocab.shape[0]
     n_top = min(n_vocab, 100)
```

### Comparing `embedding_explorer-0.1.4/pyproject.toml` & `embedding_explorer-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length=79
 
 [tool.ruff]
 line-length=79
 
 [tool.poetry]
 name = "embedding-explorer"
-version = "0.1.4"
+version = "0.2.0"
 description = "Tools for interactive visual inspection of static word embedding models."
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "embedding_explorer"}]
 
 [tool.poetry.dependencies]
```

### Comparing `embedding_explorer-0.1.4/setup.py` & `embedding_explorer-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'numpy>=1.23.0',
  'pandas>=1.5.2,<1.6.0',
  'scikit-learn>=1.1.0,<1.2.0',
  'wordcloud>=1.8.2.2,<1.9.0.0']
 
 setup_kwargs = {
     'name': 'embedding-explorer',
-    'version': '0.1.4',
+    'version': '0.2.0',
     'description': 'Tools for interactive visual inspection of static word embedding models.',
     'long_description': '# embedding-explorer\nTools for interactive visual exploration of static word embedding models.\n',
     'author': 'Márton Kardos',
     'author_email': 'power.up1163@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `embedding_explorer-0.1.4/PKG-INFO` & `embedding_explorer-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedding-explorer
-Version: 0.1.4
+Version: 0.2.0
 Summary: Tools for interactive visual inspection of static word embedding models.
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

