# Comparing `tmp/redco-0.4.2.tar.gz` & `tmp/redco-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redco-0.4.2.tar", last modified: Thu May 25 03:00:07 2023, max compression
+gzip compressed data, was "redco-0.4.3.tar", last modified: Mon May 29 23:46:07 2023, max compression
```

## Comparing `redco-0.4.2.tar` & `redco-0.4.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.150000 redco-0.4.2/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.2/LICENSE
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-05-25 03:00:07.150000 redco-0.4.2/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3375 2023-05-13 23:56:05.000000 redco-0.4.2/README.md
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.140000 redco-0.4.2/redco/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.2/redco/__init__.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.150000 redco-0.4.2/redco/datasets/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.2/redco/datasets/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-04-19 06:51:00.000000 redco-0.4.2/redco/datasets/dataset.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1109 2023-04-19 06:51:00.000000 redco-0.4.2/redco/datasets/jsonl_dataset.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.150000 redco-0.4.2/redco/deployers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.2/redco/deployers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2065 2023-04-19 06:51:00.000000 redco-0.4.2/redco/deployers/data_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     8051 2023-05-24 01:48:22.000000 redco-0.4.2/redco/deployers/deployer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2656 2023-04-19 06:51:00.000000 redco-0.4.2/redco/deployers/log_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.150000 redco-0.4.2/redco/deployers/model_parallel_utils/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.2/redco/deployers/model_parallel_utils/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5493 2023-05-24 01:48:22.000000 redco-0.4.2/redco/deployers/model_parallel_utils/mesh_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2468 2023-04-19 06:51:00.000000 redco-0.4.2/redco/deployers/model_parallel_utils/partition_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1835 2023-04-19 06:51:00.000000 redco-0.4.2/redco/deployers/opt_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.150000 redco-0.4.2/redco/predictors/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.2/redco/predictors/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4243 2023-04-19 06:51:00.000000 redco-0.4.2/redco/predictors/predictor.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1812 2023-04-19 06:51:00.000000 redco-0.4.2/redco/predictors/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.150000 redco-0.4.2/redco/trainers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.2/redco/trainers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    12098 2023-04-19 06:51:00.000000 redco-0.4.2/redco/trainers/trainer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2168 2023-04-19 06:51:00.000000 redco-0.4.2/redco/trainers/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-25 03:00:07.140000 redco-0.4.2/redco.egg-info/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-05-25 03:00:05.000000 redco-0.4.2/redco.egg-info/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-05-25 03:00:07.000000 redco-0.4.2/redco.egg-info/SOURCES.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-05-25 03:00:05.000000 redco-0.4.2/redco.egg-info/dependency_links.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-05-25 03:00:06.000000 redco-0.4.2/redco.egg-info/requires.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-05-25 03:00:06.000000 redco-0.4.2/redco.egg-info/top_level.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-05-25 03:00:07.150000 redco-0.4.2/setup.cfg
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1001 2023-05-25 02:59:09.000000 redco-0.4.2/setup.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.370000 redco-0.4.3/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.3/LICENSE
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-05-29 23:46:07.370000 redco-0.4.3/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3375 2023-05-13 23:56:05.000000 redco-0.4.3/README.md
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.360000 redco-0.4.3/redco/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.3/redco/__init__.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.370000 redco-0.4.3/redco/datasets/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.3/redco/datasets/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-04-19 06:51:00.000000 redco-0.4.3/redco/datasets/dataset.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1109 2023-04-19 06:51:00.000000 redco-0.4.3/redco/datasets/jsonl_dataset.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.370000 redco-0.4.3/redco/deployers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.3/redco/deployers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2065 2023-04-19 06:51:00.000000 redco-0.4.3/redco/deployers/data_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     8110 2023-05-29 01:02:59.000000 redco-0.4.3/redco/deployers/deployer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2656 2023-04-19 06:51:00.000000 redco-0.4.3/redco/deployers/log_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.370000 redco-0.4.3/redco/deployers/model_parallel_utils/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.3/redco/deployers/model_parallel_utils/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5546 2023-05-29 00:52:43.000000 redco-0.4.3/redco/deployers/model_parallel_utils/mesh_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1854 2023-05-29 01:00:49.000000 redco-0.4.3/redco/deployers/model_parallel_utils/partition_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1835 2023-04-19 06:51:00.000000 redco-0.4.3/redco/deployers/opt_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.370000 redco-0.4.3/redco/predictors/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.3/redco/predictors/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4274 2023-05-29 01:02:59.000000 redco-0.4.3/redco/predictors/predictor.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1812 2023-04-19 06:51:00.000000 redco-0.4.3/redco/predictors/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.370000 redco-0.4.3/redco/trainers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.3/redco/trainers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    12139 2023-05-29 01:12:09.000000 redco-0.4.3/redco/trainers/trainer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2168 2023-04-19 06:51:00.000000 redco-0.4.3/redco/trainers/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-29 23:46:07.360000 redco-0.4.3/redco.egg-info/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-05-29 23:46:06.000000 redco-0.4.3/redco.egg-info/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-05-29 23:46:07.000000 redco-0.4.3/redco.egg-info/SOURCES.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-05-29 23:46:06.000000 redco-0.4.3/redco.egg-info/dependency_links.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-05-29 23:46:07.000000 redco-0.4.3/redco.egg-info/requires.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-05-29 23:46:07.000000 redco-0.4.3/redco.egg-info/top_level.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-05-29 23:46:07.370000 redco-0.4.3/setup.cfg
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1001 2023-05-29 23:46:04.000000 redco-0.4.3/setup.py
```

### Comparing `redco-0.4.2/LICENSE` & `redco-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/PKG-INFO` & `redco-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redco
-Version: 0.4.2
+Version: 0.4.3
 Summary: UNKNOWN
 Home-page: https://github.com/tanyuqian/redco
 Author: Bowen Tan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `redco-0.4.2/README.md` & `redco-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco/__init__.py` & `redco-0.4.3/redco/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco/datasets/__init__.py` & `redco-0.4.3/redco/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco/datasets/dataset.py` & `redco-0.4.3/redco/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco/datasets/jsonl_dataset.py` & `redco-0.4.3/redco/datasets/jsonl_dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco/deployers/__init__.py` & `redco-0.4.3/redco/deployers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco/deployers/data_utils.py` & `redco-0.4.3/redco/deployers/data_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco/deployers/deployer.py` & `redco-0.4.3/redco/deployers/deployer.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,16 +150,17 @@
 
             self.log_info(
                 info='\n'.join([f'{t}' for t in sharding_rules]),
                 title='Sharding rules')
 
             return sharding_rules
 
-    def get_params_spec(self, params, shard_rules):
-        return get_param_spec(params=params, shard_rules=shard_rules)
+    def get_params_spec(self, params, params_sharding_rules):
+        return get_param_spec(
+            params=params, params_sharding_rules=params_sharding_rules)
 
     def shard_params_and_opt_state(self, params, params_spec, optimizer):
         return shard_params_and_opt_state(
             params=params,
             params_spec=params_spec,
             mesh=self._mesh,
             optimizer=optimizer)
@@ -201,18 +202,18 @@
 
     def load_params(self, filepath):
         params = msgpack_restore(open(filepath, 'rb').read())
         self.log_info(f'params loaded from {filepath}')
 
         return params
 
-    def save_params(self, params, filepath, params_shard_rules=None):
+    def save_params(self, params, filepath, params_sharding_rules=None):
         if self._mesh is not None:
             params_spec = self.get_params_spec(
-                params=params, shard_rules=params_shard_rules)
+                params=params, params_sharding_rules=params_sharding_rules)
             params = gather_params_to_cpu(
                 params=params, params_spec=params_spec, mesh=self._mesh)
 
         if jax.process_index() == 0:
             save_dir = '/'.join(filepath.split('/')[:-1])
             os.makedirs(save_dir, exist_ok=True)
```

### Comparing `redco-0.4.2/redco/deployers/log_utils.py` & `redco-0.4.3/redco/deployers/log_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco/deployers/model_parallel_utils/__init__.py` & `redco-0.4.3/redco/deployers/model_parallel_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco/deployers/model_parallel_utils/mesh_utils.py` & `redco-0.4.3/redco/deployers/model_parallel_utils/mesh_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     __slots__ = ["shape", "dtype"]
 
     def __init__(self, shape, dtype):
         self.shape = shape
         self.dtype = dtype
 
 
-def get_param_spec(params, shard_rules):
-    return set_partitions(unfreeze(params), shard_rules)
+def get_param_spec(params, params_sharding_rules):
+    return set_partitions(unfreeze(params), params_sharding_rules)
 
 
 def shard_params_and_opt_state(params, params_spec, mesh, optimizer):
     def init_fn(params_):
         opt_state_ = optimizer.init(params_)
         return opt_state_, params_
 
@@ -96,15 +96,15 @@
             return jax.tree_util.tree_map(
                 lambda gather_fn, param: jax.device_get(gather_fn(param)),
                 gather_fns,
                 params)
 
 
 def get_sharding_rules(params, mesh_model_shards, investigate_depth=2):
-    shard_rules = {
+    sharding_rules = {
         ('(bias|scale)',): None,
         ('embedding',): P('mp', None),
     }
 
     last_dense_mp_dim = None
     flat_params = flatten_dict(params)
     for key in sorted(flat_params.keys(), key=lambda t: (len(t), t)):
@@ -114,36 +114,36 @@
 
         if key[-1] in ['bias', 'scale']:
             assert len(param.shape) == 1
 
         elif key[-1] == 'embedding':
             assert len(param.shape) == 2
             if param.shape[0] % mesh_model_shards != 0:
-                shard_rules[('embedding',)] = P(None, 'mp')
+                sharding_rules[('embedding',)] = P(None, 'mp')
 
         else:
             if len(param.squeeze().shape) == 1:
-                shard_rules[rule_key] = None
+                sharding_rules[rule_key] = None
 
-            elif rule_key in shard_rules:
+            elif rule_key in sharding_rules:
                 for dim_size, rule_str in zip(
-                        param.shape, shard_rules[rule_key]):
+                        param.shape, sharding_rules[rule_key]):
                     assert rule_str != 'mp' or dim_size % mesh_model_shards == 0
 
             elif under_attention(key) and rule_key[0][0] == 'o':
-                shard_rules[rule_key] = P('mp', None)
+                sharding_rules[rule_key] = P('mp', None)
 
             elif under_attention(key) and rule_key[0][0] in ['q', 'k', 'v']:
-                shard_rules[rule_key] = P(None, 'mp')
+                sharding_rules[rule_key] = P(None, 'mp')
 
             elif under_attention(key) and rule_key[0][-1] == 'o':
-                shard_rules[rule_key] = P('mp', None)
+                sharding_rules[rule_key] = P('mp', None)
 
             elif under_attention(key) and rule_key[0][-1] in ['q', 'k', 'v']:
-                shard_rules[rule_key] = P(None, 'mp')
+                sharding_rules[rule_key] = P(None, 'mp')
 
             else:
                 rule_tuple = [None for _ in range(len(param.shape))]
                 for dim in range(-1, -len(param.shape) - 1, -1):
                     if dim != last_dense_mp_dim and \
                             param.shape[dim] % mesh_model_shards == 0:
                         last_dense_mp_dim = dim
@@ -151,17 +151,17 @@
                         break
                 if all([t is None for t in rule_tuple]):
                     if last_dense_mp_dim is not None and \
                             param.shape[last_dense_mp_dim] % \
                             mesh_model_shards == 0:
                         rule_tuple[last_dense_mp_dim] = 'mp'
 
-                shard_rules[rule_key] = P(*rule_tuple)
+                sharding_rules[rule_key] = P(*rule_tuple)
 
-    return list(shard_rules.items())
+    return list(sharding_rules.items())
 
 
 def under_attention(flat_param_key):
     for key in flat_param_key:
         if 'attention' in key.lower() or 'attn' in key.lower():
             return True
     return False
```

### Comparing `redco-0.4.2/redco/deployers/model_parallel_utils/partition_utils.py` & `redco-0.4.3/redco/deployers/model_parallel_utils/partition_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,33 @@
-#!/usr/bin/env python
-# coding=utf-8
 #  Copyright 2021 Google LLC
 #  #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #  #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #  #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+#  adapted from https://github.com/google-research/google-research/blob/fce923e9dad97cd67492c2a65b9ecdc4b2495204/flax_models/t5x/partitions.py
 """Utilities for constructing PyTrees of PartitionSpecs."""
 
-# utils adapted from https://github.com/google-research/google-research/blob/master/flax_models/t5x/partitions.py
-
 import re
 
 from flax.core.frozen_dict import freeze
 from flax.traverse_util import flatten_dict, unflatten_dict
 
 
 # Sentinels
 _unmatched = object()
 
-# For specifying empty leaf dict `{}`
-empty_dict = object()
-
 
 def _match(qs, ks):
     """Return True if regexes in qs match any window of strings in tuple ks."""
     # compile regexes and force complete match
     qts = tuple(map(lambda x: re.compile(x + "$"), qs))
     for i in range(len(ks) - len(qs) + 1):
         matches = [x.match(y) for x, y in zip(qts, ks[i:])]
```

### Comparing `redco-0.4.2/redco/deployers/opt_utils.py` & `redco-0.4.3/redco/deployers/opt_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco/predictors/__init__.py` & `redco-0.4.3/redco/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco/predictors/predictor.py` & `redco-0.4.3/redco/predictors/predictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 class Predictor:
     def __init__(self,
                  deployer,
                  collate_fn,
                  pred_fn,
                  output_fn=None,
                  params=None,
-                 params_shard_rules=None):
+                 params_sharding_rules=None):
         self._deployer = deployer
         self._collate_fn = partial(collate_fn_wrapper, collate_fn=collate_fn)
 
         self._params = params
-        self._params_shard_rules = params_shard_rules
+        self._params_sharding_rules = params_sharding_rules
         self._pred_fn = partial(
             pred_fn_wrapper,
             pred_fn=pred_fn,
             under_pmap=self._deployer.mesh is None)
         self._p_pred_step = None
 
         if output_fn is None:
@@ -48,25 +48,25 @@
         else:
             self._output_fn = output_fn
 
     def setup_running_step(self,
                            pred_fn,
                            dummy_batch,
                            params,
-                           params_shard_rules):
+                           params_sharding_rules):
         if self._deployer.mesh is None:
             self._p_pred_step = jax.pmap(pred_fn, axis_name='batch')
         else:
             data_spec = {
                 key: P(*(('dp',) + (None,) * (len(value.shape) - 1)))
                 for key, value in dummy_batch.items()
             }
 
             params_spec = self._deployer.get_params_spec(
-                params=params, shard_rules=params_shard_rules)
+                params=params, params_sharding_rules=params_sharding_rules)
 
             self._p_pred_step = pjit(
                 pred_fn,
                 in_axis_resources=(None, params_spec, data_spec),
                 out_axis_resources=None)
 
     def predict(self, examples, per_device_batch_size, params=None, desc=''):
@@ -93,15 +93,15 @@
         preds = []
         for batch in data_batches:
             if self._p_pred_step is None:
                 self.setup_running_step(
                     pred_fn=self._pred_fn,
                     dummy_batch=batch,
                     params=params,
-                    params_shard_rules=self._params_shard_rules)
+                    params_sharding_rules=self._params_sharding_rules)
 
             pred_rng = self._deployer.process_to_run_model(
                 self._deployer.gen_rng(), is_prng_key=True)
 
             batch_preds_with_idxes = self._deployer.run_model_step(
                 step_fn=self._p_pred_step,
                 input_args=(pred_rng, params, batch))
```

### Comparing `redco-0.4.2/redco/predictors/utils.py` & `redco-0.4.3/redco/predictors/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco/trainers/__init__.py` & `redco-0.4.3/redco/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco/trainers/trainer.py` & `redco-0.4.3/redco/trainers/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,21 +33,21 @@
                  deployer,
                  collate_fn,
                  apply_fn,
                  loss_fn,
                  params,
                  optimizer,
                  lr_schedule_fn=None,
-                 params_shard_rules=None,
+                 params_sharding_rules=None,
                  params_grad_weights=None):
         self._deployer = deployer
         self._collate_fn = collate_fn
         self._loss_fn = loss_fn
         self._lr_schedule_fn = lr_schedule_fn
-        self._params_shard_rules = params_shard_rules
+        self._params_sharding_rules = params_sharding_rules
         self._params_grad_weights = freeze(params_grad_weights) \
             if params_grad_weights is not None else None
 
         self._state = None
         self._state_spec = None
         self._p_train_step = None
         self._p_eval_step = None
@@ -59,27 +59,27 @@
             sum(np.prod(param.shape) for param in flatten_dict(params).values())
         self._deployer.log_info(f'{n_params:,}', title='Training parameters')
 
         self._default_predictor_fn = partial(
             Predictor,
             deployer=deployer,
             collate_fn=collate_fn,
-            params=params,
-            params_shard_rules=params_shard_rules)
+            params_sharding_rules=params_sharding_rules)
 
     def create_train_state(self, apply_fn, params, optimizer):
         params = freeze(params)
 
         if self._deployer.mesh is None:
             self._state = TrainState.create(
                 apply_fn=apply_fn, params=params, tx=optimizer)
             self._state = replicate(self._state)
         else:
             params_spec = self._deployer.get_params_spec(
-                params=params, shard_rules=self._params_shard_rules)
+                params=params,
+                params_sharding_rules=self._params_sharding_rules)
 
             params, opt_state, opt_state_spec = \
                 self._deployer.shard_params_and_opt_state(
                     params=params, params_spec=params_spec, optimizer=optimizer)
 
             self._state = TrainState(
                 apply_fn=apply_fn,
@@ -254,52 +254,52 @@
 
                 if save_every_ckpt:
                     assert self._deployer.workdir is not None
                     path_to_save = f'{self._deployer.workdir}/ckpts/' \
                                    f'epoch_{epoch_idx}.msgpack'
                     self._deployer.save_params(
                         params=self.params,
-                        params_shard_rules=self._params_shard_rules,
+                        params_sharding_rules=self._params_sharding_rules,
                         filepath=path_to_save)
 
                 if save_last_ckpt:
                     assert self._deployer.workdir is not None
                     path_to_save = f'{self._deployer.workdir}/ckpts/'\
                                    f'last.msgpack'
                     self._deployer.save_params(
                         params=self.params,
-                        params_shard_rules=self._params_shard_rules,
+                        params_sharding_rules=self._params_sharding_rules,
                         filepath=path_to_save)
 
                 for key in save_argmin_ckpt_by_metrics:
                     assert self._deployer.workdir is not None
                     if eval_metrics[key] < min_metrics.get(key, float('inf')):
                         min_metrics[key] = eval_metrics[key]
                         self._deployer.log_info(
                             f'minimal {key} updated to {min_metrics[key]}')
 
                         path_to_save = f'{self._deployer.workdir}/ckpts/'\
                                        f'min_{key}.msgpack'
                         self._deployer.save_params(
                             params=self.params,
-                            params_shard_rules=self._params_shard_rules,
+                            params_sharding_rules=self._params_sharding_rules,
                             filepath=path_to_save)
 
                 for key in save_argmax_ckpt_by_metrics:
                     assert self._deployer.workdir is not None
                     if eval_metrics[key] > max_metrics.get(key, float('-inf')):
                         max_metrics[key] = eval_metrics[key]
                         self._deployer.log_info(
                             f'minimal {key} updated to {max_metrics[key]}')
 
                         path_to_save = f'{self._deployer.workdir}/ckpts/'\
                                        f'max_{key}.msgpack'
                         self._deployer.save_params(
                             params=self.params,
-                            params_shard_rules=self._params_shard_rules,
+                            params_sharding_rules=self._params_sharding_rules,
                             filepath=path_to_save)
 
     def get_default_predictor(self, pred_fn, output_fn=None):
         return self._default_predictor_fn(pred_fn=pred_fn, output_fn=output_fn)
 
     @property
     def params(self):
```

### Comparing `redco-0.4.2/redco/trainers/utils.py` & `redco-0.4.3/redco/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/redco.egg-info/PKG-INFO` & `redco-0.4.3/redco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redco
-Version: 0.4.2
+Version: 0.4.3
 Summary: UNKNOWN
 Home-page: https://github.com/tanyuqian/redco
 Author: Bowen Tan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `redco-0.4.2/redco.egg-info/SOURCES.txt` & `redco-0.4.3/redco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redco-0.4.2/setup.py` & `redco-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  limitations under the License.
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="redco",
-    version="0.4.2",
+    version="0.4.3",
     author="Bowen Tan",
     packages=find_packages(),
     install_requires=['jax', 'flax', 'optax', 'numpy'],
     include_package_data=True,
     python_requires=">=3.8",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

