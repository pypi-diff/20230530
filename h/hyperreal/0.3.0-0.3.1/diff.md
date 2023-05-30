# Comparing `tmp/hyperreal-0.3.0.tar.gz` & `tmp/hyperreal-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperreal-0.3.0.tar", last modified: Thu Mar 30 05:16:30 2023, max compression
+gzip compressed data, was "hyperreal-0.3.1.tar", last modified: Tue May 30 06:25:56 2023, max compression
```

## Comparing `hyperreal-0.3.0.tar` & `hyperreal-0.3.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:16:30.497550 hyperreal-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-30 05:15:48.000000 hyperreal-0.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:16:30.493550 hyperreal-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:16:30.497550 hyperreal-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-30 05:15:48.000000 hyperreal-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-30 05:15:48.000000 hyperreal-0.3.0/.github/workflows/test_python.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 05:15:48.000000 hyperreal-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-30 05:15:48.000000 hyperreal-0.3.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-30 05:15:48.000000 hyperreal-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-30 05:15:48.000000 hyperreal-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-03-30 05:16:30.497550 hyperreal-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-03-30 05:15:48.000000 hyperreal-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:16:30.497550 hyperreal-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-30 05:15:48.000000 hyperreal-0.3.0/docs/definitions.md
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-30 05:15:48.000000 hyperreal-0.3.0/docs/design.md
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-30 05:15:48.000000 hyperreal-0.3.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:16:30.497550 hyperreal-0.3.0/hyperreal/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/_index_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    32888 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/db_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    68610 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:16:30.497550 hyperreal-0.3.0/hyperreal/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/templates/cluster.html
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/templates/details.html
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/templates/index_listing.html
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/templates/macros.html
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-03-30 05:15:48.000000 hyperreal-0.3.0/hyperreal/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:16:30.497550 hyperreal-0.3.0/hyperreal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-03-30 05:16:30.000000 hyperreal-0.3.0/hyperreal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-30 05:16:30.000000 hyperreal-0.3.0/hyperreal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 05:16:30.000000 hyperreal-0.3.0/hyperreal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-30 05:16:30.000000 hyperreal-0.3.0/hyperreal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-30 05:16:30.000000 hyperreal-0.3.0/hyperreal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-30 05:16:30.000000 hyperreal-0.3.0/hyperreal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 05:16:30.497550 hyperreal-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-30 05:15:48.000000 hyperreal-0.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-30 05:15:49.000000 hyperreal-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.370131 hyperreal-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-30 06:25:08.000000 hyperreal-0.3.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.362131 hyperreal-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.366131 hyperreal-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 06:25:08.000000 hyperreal-0.3.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-30 06:25:08.000000 hyperreal-0.3.1/.github/workflows/test_python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 06:25:08.000000 hyperreal-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-30 06:25:08.000000 hyperreal-0.3.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 06:25:08.000000 hyperreal-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 06:25:08.000000 hyperreal-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-30 06:25:56.370131 hyperreal-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-30 06:25:08.000000 hyperreal-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.370131 hyperreal-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 06:25:08.000000 hyperreal-0.3.1/docs/definitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-30 06:25:08.000000 hyperreal-0.3.1/docs/design.md
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-30 06:25:08.000000 hyperreal-0.3.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.370131 hyperreal-0.3.1/hyperreal/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/_index_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32888 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/db_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72458 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.370131 hyperreal-0.3.1/hyperreal/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/cluster.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/details.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/index_listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-30 06:25:08.000000 hyperreal-0.3.1/hyperreal/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:56.370131 hyperreal-0.3.1/hyperreal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-30 06:25:56.000000 hyperreal-0.3.1/hyperreal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-30 06:25:56.000000 hyperreal-0.3.1/hyperreal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:25:56.000000 hyperreal-0.3.1/hyperreal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 06:25:56.000000 hyperreal-0.3.1/hyperreal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-30 06:25:56.000000 hyperreal-0.3.1/hyperreal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 06:25:56.000000 hyperreal-0.3.1/hyperreal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:25:56.370131 hyperreal-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-30 06:25:08.000000 hyperreal-0.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-30 06:25:08.000000 hyperreal-0.3.1/tox.ini
```

### Comparing `hyperreal-0.3.0/.coveragerc` & `hyperreal-0.3.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/.github/workflows/publish.yml` & `hyperreal-0.3.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/.github/workflows/test_python.yml` & `hyperreal-0.3.1/.github/workflows/test_python.yml`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/CITATION.cff` & `hyperreal-0.3.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/LICENSE.txt` & `hyperreal-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/PKG-INFO` & `hyperreal-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperreal
-Version: 0.3.0
+Version: 0.3.1
 Summary: Hyperreal is a library and tool for intepretive topic modelling.
 Home-page: https://github.com/SamHames/hyperreal/
 Author: Sam Hames
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `hyperreal-0.3.0/README.md` & `hyperreal-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/docs/design.md` & `hyperreal-0.3.1/docs/design.md`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/hyperreal/_index_schema.py` & `hyperreal-0.3.1/hyperreal/_index_schema.py`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/hyperreal/cli.py` & `hyperreal-0.3.1/hyperreal/cli.py`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/hyperreal/corpus.py` & `hyperreal-0.3.1/hyperreal/corpus.py`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/hyperreal/db_utilities.py` & `hyperreal-0.3.1/hyperreal/db_utilities.py`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/hyperreal/index.py` & `hyperreal-0.3.1/hyperreal/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 An Index is a boolean inverted index, mapping field, value tuples in documents
 to document keys.
 
 """
 
 import array
+import atexit
 import collections
 from collections.abc import Sequence, Iterable
 import concurrent.futures as cf
 from functools import wraps
 import heapq
 import logging
 import math
@@ -168,18 +169,31 @@
         self._changed = False
 
         # Set up a context specific adapter for this index.
         self.logger = logging.LoggerAdapter(logger, {"index_db_path": self.db_path})
 
     @property
     def pool(self):
-        """Lazily initialised multiprocessing pool if none is provided on init."""
+        """
+        Lazily initialised multiprocessing pool if none is provided on init.
+
+        Note that if a pool is generated on demand an atexit handler will be created
+        to cleanup the pool and pending tasks. If a pool is passed in to this instance,
+        no cleanup action will be taken.
+
+        """
         if self._pool is None:
             self._pool = cf.ProcessPoolExecutor(mp_context=mp.get_context("spawn"))
 
+            def shutdown_pool(pool):
+                "Create an exit handler to ensure that the pool is cleaned up on exit."
+                pool.shutdown(wait=False, cancel_futures=True)
+
+            atexit.register(shutdown_pool, self._pool)
+
         return self._pool
 
     @classmethod
     def is_index_db(cls, db_path):
         """Returns True if a db exists at db_path and is an index db."""
         try:
             db = sqlite3.connect(f"file:{db_path}?mode=ro", uri=True)
@@ -979,63 +993,174 @@
         """Return the bitmap of documents covered by this cluster."""
         return list(
             self.db.execute(
                 "select doc_ids from cluster where cluster_id = ?", [cluster_id]
             )
         )[0][0]
 
-    def _refine_feature_groups(
+    def _measure_feature_cluster_contributions(
         self,
         cluster_feature: dict[Hashable, set[int]],
+        probe_query: Optional[AbstractBitMap] = None,
+    ) -> dict[Hashable, tuple[array.array, array.array, float]]:
+        """
+        Return the estimated contribution of each feature to its own cluster.
+
+        The return type is arrays of features and associated scores to keep
+        things compact in memory and limit serialisation overhead when dealing
+        with large numbers of features/clusters.
+
+        """
+        futures = {
+            self.pool.submit(
+                measure_feature_contribution_to_cluster,
+                self.db_path,
+                cluster,
+                features,
+                probe_query,
+            )
+            for cluster, features in cluster_feature.items()
+        }
+
+        feature_contributions = {}
+
+        for future in cf.as_completed(futures):
+            result = future.result()
+            feature_contributions[result[0]] = result[1:]
+
+        return feature_contributions
+
+    def _calculate_best_feature_moves(
+        self,
+        cluster_feature: dict[Hashable, set[int]],
+        cluster_check_feature: dict[Hashable, set[int]],
+        probe_query: Optional[AbstractBitMap] = None,
+        top_k: int = 1,
+    ) -> dict[int, tuple[float, Hashable]]:
+        """
+        Return the estimated best cluster/s for each feature.
+
+        This should be used in conjunction with the scores output from
+        `_measure_feature_cluster_contributions`, which describes the contribution
+        of each feature to its own cluster.
+
+        The input is two mappings:
+
+        cluster_feature - the current cluster: features mapping
+        cluster_check_features - mapping of cluster: features to check
+            against moving into this cluster. Note that features will
+            be removed from this set if they are already in this cluster
+            in cluster_feature.
+
+        acceptance_probability is a softening factor, used to prevent
+        cycling between the same states on repeated iteration.
+
+        top_k: the number of best scores to keep - the default is to only
+            the single best scoring feature.
+
+        """
+
+        # preflight check:
+        missing_clusters = {
+            cluster_key
+            for cluster_key in cluster_check_feature
+            if cluster_key not in cluster_feature
+        }
+
+        if missing_clusters:
+            raise KeyError(
+                f"`cluster_feature` is missing clusters with keys: {missing_clusters}"
+            )
+
+        futures = [
+            self.pool.submit(
+                measure_add_features_to_cluster,
+                self.db_path,
+                cluster_key,
+                cluster_feature[cluster_key],
+                cluster_check_feature[cluster_key] - cluster_feature[cluster_key],
+                probe_query,
+            )
+            # dispatch in sort order for reproducibility with randomisation
+            for cluster_key in sorted(cluster_check_feature)
+        ]
+
+        best_clusters = collections.defaultdict(list)
+
+        for future in futures:
+            test_cluster, feature_array, delta_array = future.result()
+
+            for feature, delta in zip(feature_array, delta_array):
+                current_scores = len(best_clusters[feature])
+
+                if current_scores < top_k:
+                    heapq.heappush(best_clusters[feature], (delta, test_cluster))
+                else:
+                    heapq.heappushpop(best_clusters[feature], (delta, test_cluster))
+
+        return {
+            key: sorted(feature_scores, reverse=True)
+            for key, feature_scores in best_clusters.items()
+        }
+
+    def _refine_feature_groups(
+        self,
+        cluster_feature: dict[int, set[int]],
         iterations: int = 10,
         group_test: bool = True,
         minimum_cluster_features: int = 1,
         pinned_features: Optional[Iterable[int]] = None,
         probe_query: Optional[AbstractBitMap] = None,
-        max_clusters: Optional[int] = None,
+        target_clusters: Optional[int] = None,
         tolerance: float = 0.01,
-    ) -> dict[Hashable, set[int]]:
+        acceptance_probability: float = 0.75,
+    ) -> tuple[dict[int, set[int]], set[int]]:
         """
         Low level function for iteratively refining a feature clustering.
 
         cluster_features is a mapping from a cluster_key to a set of feature_ids.
 
         This is most useful if you want to explore specific clustering
         approaches without the constraint of the saved clusters.
 
-        To expand the number of clusters in a model, empty cluster_ids can be
-        provided and will be used for additional clusters made by splitting
-        the largest clusters up.
+        To change the number of clusters in the model, set target clusters to
+        a different number of clusters than in cluster_feature - the clustering
+        will be adjusted to the target. The newly generated IDs will be returned
+        along with the new feature clustering.
 
         Pinned features will not be considered as candidates for moving.
 
         If a probe_query is provided, it will be intersected with all features
         for clustering: this is used to generate a clustering for a subset of
         the data. Note that features may not intersect with the probe query -
         clustering is not well defined in this case and should be used with
         care.
 
-        max_clusters: specifies a maximum number of clusters for the model: if
+        target_clusters: specifies a target number of clusters for the model: if
         there are more clusters, the clusters that contribute least to the
         objective will be dissolved. Dissolves will be conducted evenly per
-        iteration, rather than all at once.
+        iteration, rather than all at once. If there are fewer clusters than
+        target, new clusters will be created and filled randomly.
 
         tolerance: specifies a termination tolerance. If fewer than
         tolerance * total_features features move in an iteration, terminate
         early. The default is set at 0.01, or 1% - the model is considered
         converged if less than 1% of the features have moved during an
         iteration.
 
+        acceptance_probability: the probability a move that is estimated to
+            improve the score will be accepted.
+
         """
 
-        max_clusters = max_clusters or len(cluster_feature)
+        target_clusters = target_clusters or len(cluster_feature)
 
         # If cluster_feature is empty, return immediately
         if not len(cluster_feature.keys()):
-            return cluster_feature
+            return cluster_feature, set()
 
         # Make sure to copy the input dict
         cluster_feature = {
             cluster_id: features.copy()
             for cluster_id, features in cluster_feature.items()
         }
 
@@ -1058,37 +1183,47 @@
             f
             for features in cluster_feature.values()
             for f in features
             if f not in pinned_features
         }
 
         movable_feature_list = list(movable_features)
+        moved_features = len(movable_features)
 
-        # Used to determine the size of newly sampled clusters when filling in
-        # too-small clusters.
-        sample_cluster_size = max(
-            minimum_cluster_features, len(movable_features) // (2 * max_clusters)
-        )
+        available_workers = self.pool._max_workers
+
+        current_cluster_scores = {}
+        changed_clusters = set(cluster_feature)
+
+        # Generate new cluster_ids and emtpy clusters if we have less clusters
+        # than target_clusters
+        next_cluster_id = max(cluster_feature) + 1
+        new_clusters = target_clusters - len(cluster_feature)
+        new_cluster_ids = list(range(next_cluster_id, next_cluster_id + new_clusters))
+
+        for cluster_id in new_cluster_ids:
+            cluster_feature[cluster_id] = set()
 
         # Use initial cluster ids to keep track of whether any clusters
         # are fully emptied out and can be used to split larger clusters up.
         assigned_cluster_ids = set(cluster_feature)
 
+        # Used to determine the size of newly sampled clusters when filling in
+        # too-small clusters.
+        sample_cluster_size = max(
+            minimum_cluster_features, len(movable_features) // (2 * target_clusters)
+        )
+
         # Work out how many low objective clusters to dissolve on each iteration.
-        dissolve_clusters = max(0, len(assigned_cluster_ids) - max_clusters)
+        dissolve_clusters = max(0, len(assigned_cluster_ids) - target_clusters)
         # Note that we try to structure it so the very last iteration does not dissolve
         # anything.
         dissolve_per_iteration = math.ceil(dissolve_clusters / max(1, iterations - 1))
         dissolve_cluster_ids = set()
 
-        available_workers = self.pool._max_workers
-
-        current_cluster_scores = {}
-        changed_clusters = set(cluster_feature)
-
         prev_obj = 0
 
         for iteration in range(iterations):
             # Prepation phase: handle empty/too small clusters, but taking
             # into account possible dissolves as well. Note that we should
             # only drop a cluster_id that was dissolved on the last
             # iteration - this allows us to be incremental in our approach.
@@ -1138,31 +1273,20 @@
                         self.logger.debug(
                             f"Filled cluster {cluster_id} by sampling {sample_cluster_size} features"
                         )
                 else:
                     break
 
             # Compute current feature assignments and contributions to each cluster
-            futures = {
-                self.pool.submit(
-                    measure_feature_contribution_to_cluster,
-                    self.db_path,
-                    cluster,
-                    features,
-                    probe_query,
-                )
-                for cluster, features in cluster_feature.items()
-                if features and cluster in changed_clusters
-            }
-
-            for f in cf.as_completed(futures):
-                r = f.result()
-                current_cluster_scores[r[0]] = r[1:]
+            current_cluster_scores = self._measure_feature_cluster_contributions(
+                cluster_feature, probe_query=probe_query
+            )
 
             total_objective = sum(r[2] for r in current_cluster_scores.values())
+
             self.logger.info(
                 f"Iteration {iteration}, current objective: {total_objective}"
             )
 
             # Dissolve target low objective clusters for this iteration
             if dissolve_clusters:
                 n_dissolve = min(dissolve_clusters, dissolve_per_iteration)
@@ -1190,156 +1314,120 @@
             cluster_ids = list(current_cluster_scores.keys() - dissolve_cluster_ids)
             self.random.shuffle(cluster_ids)
 
             n_batches = math.ceil(len(cluster_ids) ** 0.5)
 
             if group_test and n_batches > 2:
                 cluster_groups = [
-                    tuple(cluster_ids[i::n_batches]) for i in range(n_batches)
+                    set(cluster_ids[i::n_batches]) for i in range(n_batches)
                 ]
 
-                futures = set()
+                group_features = {}
+                group_feature_checks = {}
 
                 for group in cluster_groups:
-                    group_features = {
-                        f for c in group for f in current_cluster_scores[c][0]
-                    }
-
-                    # Note that we don't test adding the feature to it's own group!
-                    comparison_features = {
-                        f
-                        for c in current_cluster_scores.keys() - set(group)
-                        for f in current_cluster_scores[c][0]
-                    } - pinned_features
+                    group_key = tuple(sorted(group))
+                    this_group_features = set.union(
+                        *(cluster_feature[key] for key in group_key)
+                    )
 
-                    futures.add(
-                        self.pool.submit(
-                            measure_add_features_to_cluster,
-                            self.db_path,
-                            group,
-                            group_features,
-                            comparison_features,
-                            probe_query,
+                    group_features[group_key] = this_group_features
+                    group_feature_checks[group_key] = movable_features
+
+                    # Handle features in the current group specially by generating specific smaller
+                    # groups excluding the self cluster.
+                    for cluster_key in group_key:
+                        subgroup_key = tuple(sorted(group - set([cluster_key])))
+                        subgroup_features = (
+                            this_group_features - cluster_feature[cluster_key]
+                        )
+                        subgroup_feature_checks = (
+                            cluster_feature[cluster_key] - pinned_features
                         )
-                    )
 
-                # Accumulate the best group to do a detailed check against
-                best_groups = {}
+                        group_features[subgroup_key] = subgroup_features
+                        group_feature_checks[subgroup_key] = subgroup_feature_checks
 
-                for f in cf.as_completed(futures):
-                    group_key, feature_array, delta_array = f.result()
+                best_groups = self._calculate_best_feature_moves(
+                    group_features, group_feature_checks, probe_query=probe_query
+                )
 
-                    for feature, delta in zip(feature_array, delta_array):
-                        # Note that we can't use a defaultdict for this, as
-                        # we would need to know the structure of group_key for
-                        # comparison purposes.
-                        try:
-                            best_groups[feature] = max(
-                                best_groups[feature], (delta, group_key)
-                            )
-                        except KeyError:
-                            best_groups[feature] = (delta, group_key)
+                cluster_feature_checks = collections.defaultdict(set)
 
-                # Individual cluster checks against the selected comparison group
-                comparison_features = collections.defaultdict(list)
-                for feature, (_, group_key) in best_groups.items():
-                    for c in group_key:
-                        comparison_features[c].append(feature)
+                # Convert best group results into individual cluster checks
+                for feature, groups in best_groups.items():
+                    for _, group_key in groups:
+                        for cluster_key in group_key:
+                            cluster_feature_checks[cluster_key].add(feature)
 
             else:
-                comparison_features = {
-                    c: movable_features - set(current_cluster[0])
-                    for c, current_cluster in current_cluster_scores.items()
-                    if c not in dissolve_cluster_ids
-                }
+                cluster_feature_checks = {c: movable_features for c in cluster_ids}
 
-            # Implementation detail: we're going to make this deterministic,
-            # by processing return values in the order than they were submitted,
-            # and *not* in the order they complete!
-            futures = []
+            best_feature_clusters = self._calculate_best_feature_moves(
+                cluster_feature,
+                cluster_feature_checks,
+                probe_query=probe_query,
+            )
 
-            for c in sorted(comparison_features):
-                futures.append(
-                    self.pool.submit(
-                        measure_add_features_to_cluster,
-                        self.db_path,
-                        c,
-                        current_cluster_scores[c][0],
-                        comparison_features[c],
-                        probe_query,
-                    )
-                )
+            moved_features = 0
+            features_with_possible_improvements = 0
+            changed_clusters = set()
 
-            current_feature_scores = {
-                # This will track delta, proposed cluster, existing cluster
-                f: (
-                    (d, c, c)
-                    if c not in dissolve_cluster_ids
-                    # Randomly choose a base cluster if the cluster is being dissolved.
-                    else (-math.inf, self.random.choice(cluster_ids), c)
-                )
-                for c, (features, deltas, _) in current_cluster_scores.items()
-                for f, d in zip(features, deltas)
-            }
+            for current_cluster in sorted(current_cluster_scores):
+                features, deltas, _ = current_cluster_scores[current_cluster]
 
-            changed_features = set()
-            changed_clusters = set()
+                # When a cluster is dissolved, just reassign to the best cluster
+                # immediately.
+                if current_cluster in dissolve_cluster_ids:
+                    for feature_id, current_delta in zip(features, deltas):
+                        new_cluster = best_feature_clusters[feature_id][0][1]
+                        cluster_feature[current_cluster].discard(feature_id)
+                        cluster_feature[new_cluster].add(feature_id)
+                        feature_cluster[feature_id] = new_cluster
 
-            # Make sure to process moves for dissolved clusters
-            for cluster_id in dissolve_cluster_ids:
-                changed_features |= cluster_feature[cluster_id]
+                        changed_clusters.add(new_cluster)
 
-            # Implementation note: cf.as_completed(futures) might be faster,
-            # but is not deterministic like we'd want.
-            for f in futures:
-                test_cluster, feature_array, delta_array = f.result()
-
-                # Note that we're not accumulating to the best possible score here!
-                # We accept any change that improves the cluster score with a certain
-                # probability. Note also that the group testing means that we won't
-                # see all possible moves, there might be better moves we haven't
-                # tested.
-                for f, d in zip(feature_array, delta_array):
-                    score, _, existing_cluster = current_feature_scores[f]
-
-                    # Almost greedy choice - the small randomness is to break
-                    # ties and avoid spinning between the same two
-                    # positions.
-                    if d > score and self.random.random() < 0.99:
-                        changed_features.add(f)
-                        current_feature_scores[f] = (
-                            d,
-                            test_cluster,
-                            existing_cluster,
-                        )
+                else:
+                    for feature_id, current_delta in zip(features, deltas):
+                        if feature_id in pinned_features:
+                            continue
+
+                        comparison_delta, comparison_cluster = best_feature_clusters[
+                            feature_id
+                        ][0]
+
+                        if (
+                            comparison_delta >= current_delta
+                            and self.random.random() < acceptance_probability
+                        ):
+                            cluster_feature[current_cluster].discard(feature_id)
+                            cluster_feature[comparison_cluster].add(feature_id)
+                            feature_cluster[feature_id] = comparison_cluster
+
+                            changed_clusters.add(comparison_cluster)
 
-            # Actually assign to the new clusters, having done all of that.
-            for f in changed_features:
-                _, new_cluster, old_cluster = current_feature_scores[f]
-                changed_clusters.add(new_cluster)
-                changed_clusters.add(old_cluster)
-                cluster_feature[old_cluster].discard(f)
-                cluster_feature[new_cluster].add(f)
+                            moved_features += 1
 
             for cluster_id in dissolve_cluster_ids:
                 del current_cluster_scores[cluster_id]
                 del cluster_feature[cluster_id]
 
             if not dissolve_cluster_ids:
-                if (len(changed_features) / len(movable_features)) < tolerance:
+                if (moved_features / len(movable_features)) < tolerance:
                     self.logger.info(
                         "Terminating refinement due to small number of feature moves."
                     )
                     break
 
             self.logger.info(
-                f"Finished iteration {iteration + 1}/{iterations}, {len(changed_clusters)} changed clusters, {len(changed_features)} features"
+                f"Finished iteration {iteration + 1}/{iterations}, changed "
+                f"{len(changed_clusters)} clusters, moved {moved_features} features."
             )
 
-        return cluster_feature
+        return cluster_feature, new_cluster_ids
 
     @atomic()
     def refine_clusters(
         self,
         iterations: int = 10,
         cluster_ids: Optional[Sequence[int]] = None,
         target_clusters: Optional[int] = None,
@@ -1379,43 +1467,53 @@
             """
         ):
             if cluster_id in cluster_ids:
                 cluster_feature[cluster_id].add(feature_id)
                 if pinned:
                     pinned_features.add(feature_id)
 
-        # If the target clusters is greater than the current clusters, create
-        # empty clusters to expand into. The other case where there are
-        # more clusters than desired will be handled in _refine_feature_groups
+        # Set target clusters to the current number of clusters, or the
+        # provided value. But we also need to account for pinned clusters in
+        # the next step, otherwise this will be the wrong count.
+        # TODO: move pinned cluster handling down to _refine_feature_groups.
         target_clusters = target_clusters or len(cluster_feature)
-        n_empty_required = target_clusters - len(cluster_feature)
 
-        if n_empty_required > 0:
-            next_cluster_id = self.next_cluster_id()
+        # Remove pinned clusters from refinement, and don't count them towards
+        # target clusters.
+        pinned_clusters = set(self.pinned_cluster_ids)
 
-            for i in range(n_empty_required):
-                cluster_feature[next_cluster_id + i] = set()
-
-        # Remove pinned clusters from refinement. Note we do this after
-        # creating empty clusters because a pinned cluster still needs to be
-        # counted.
-        pinned_clusters = self.pinned_cluster_ids
         for cluster_id in pinned_clusters:
-            cluster_feature.pop(cluster_id, None)
+            if cluster_id in cluster_feature:
+                del cluster_feature[cluster_id]
+                target_clusters -= 1
 
-        cluster_feature = self._refine_feature_groups(
+        cluster_feature, new_cluster_ids = self._refine_feature_groups(
             cluster_feature,
             iterations=iterations,
             group_test=True,
             pinned_features=pinned_features,
             minimum_cluster_features=minimum_cluster_features,
-            max_clusters=target_clusters,
+            target_clusters=target_clusters,
             tolerance=tolerance,
         )
 
+        # Map new_cluster_ids generated to actual globally unique IDs.
+        # Make sure to copy these out first, as new_cluster_ids might overlap
+        # with the global clustering model!
+        new_cluster_feature = {
+            cluster_id: cluster_feature[cluster_id] for cluster_id in new_cluster_ids
+        }
+
+        next_cluster_id = self.next_cluster_id()
+
+        for cluster_id in new_cluster_ids:
+            del cluster_feature[cluster_id]
+            cluster_feature[next_cluster_id] = new_cluster_feature[cluster_id]
+            next_cluster_id += 1
+
         # Serialise the actual results of the clustering!
         self._update_cluster_feature(cluster_feature)
 
     @atomic(writes=True)
     def _update_cluster_feature(self, cluster_feature):
         """
         Update the given cluster: feature mapping.
@@ -1807,15 +1905,15 @@
 
 
 def measure_feature_contribution_to_cluster(
     index_db_path,
     group_key,
     feature_group: set[int],
     probe_query: Optional[AbstractBitMap],
-):
+) -> tuple[Any, array.array, array.array, float]:
     """
     Measure the contribution of each feature to this cluster.
 
     The contribution is the delta between the objective of the cluster without
     the feature and with the feature.
 
     This function also has the side effect of approximating the objective
@@ -1836,14 +1934,17 @@
         # The set of all docs covered at least twice.
         # This will be used to work out which documents are only covered once.
         covered_twice = BitMap()
 
         hits = 0
         n_features = len(feature_group)
 
+        if not n_features:
+            return group_key, array.array("q"), array.array("d"), 0
+
         # Construct the union of all cluster tokens, and also the set of
         # documents only covered by a single feature.
         for feature in feature_group:
             docs = index[feature]
 
             if probe_query:
                 docs &= probe_query
@@ -1883,15 +1984,16 @@
             old_c = c - only_once_hits
 
             # Check if this feature intersects with any other feature in this cluster
             intersects_with_other_feature = only_once_hits < feature_hits
 
             # It's okay for the cluster to become empty - we'll just prune it.
             if old_c and intersects_with_other_feature:
-                old_objective = old_hits / (old_c + n_features - 1)
+                old_objective = old_hits / (old_c + (n_features - 1))
+
                 delta = objective - old_objective
 
             # Penalises features that don't intersect with other features in the cluster.
             elif old_c:
                 delta = -1
             # If it would otherwise be a singleton cluster, just mark it as no change
             else:
@@ -1922,14 +2024,18 @@
 
     try:
         index = Index(index_db_path)
         index.db.execute("begin")
 
         # PHASE 1: Current cluster objective and cover.
 
+        # Handle the case of the empty cluster.
+        if not feature_group:
+            return group_key, array.array("q", []), array.array("d", [])
+
         # The union of all docs covered by the cluster
         cluster_union = BitMap()
 
         hits = 0
         n_features = len(feature_group)
 
         # Construct the union of all cluster tokens, and also the set of
@@ -1961,15 +2067,15 @@
                 docs &= probe_query
 
             feature_hits = len(docs)
 
             if docs.intersect(cluster_union):
                 new_hits = hits + feature_hits
                 new_c = docs.union_cardinality(cluster_union)
-                new_objective = new_hits / (new_c + n_features + 1)
+                new_objective = new_hits / (new_c + (n_features + 1))
 
                 delta = new_objective - objective
 
             # If the feature doesn't intersect with the cluster at all,
             # give it a bad delta.
             else:
                 delta = -1
```

### Comparing `hyperreal-0.3.0/hyperreal/server.py` & `hyperreal-0.3.1/hyperreal/server.py`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/hyperreal/templates/base.html` & `hyperreal-0.3.1/hyperreal/templates/base.html`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/hyperreal/templates/cluster.html` & `hyperreal-0.3.1/hyperreal/templates/cluster.html`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/hyperreal/templates/details.html` & `hyperreal-0.3.1/hyperreal/templates/details.html`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/hyperreal/templates/index.html` & `hyperreal-0.3.1/hyperreal/templates/index.html`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/hyperreal/templates/macros.html` & `hyperreal-0.3.1/hyperreal/templates/macros.html`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/hyperreal/utilities.py` & `hyperreal-0.3.1/hyperreal/utilities.py`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/hyperreal.egg-info/PKG-INFO` & `hyperreal-0.3.1/hyperreal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperreal
-Version: 0.3.0
+Version: 0.3.1
 Summary: Hyperreal is a library and tool for intepretive topic modelling.
 Home-page: https://github.com/SamHames/hyperreal/
 Author: Sam Hames
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `hyperreal-0.3.0/hyperreal.egg-info/SOURCES.txt` & `hyperreal-0.3.1/hyperreal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/setup.py` & `hyperreal-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `hyperreal-0.3.0/tox.ini` & `hyperreal-0.3.1/tox.ini`

 * *Files identical despite different names*

