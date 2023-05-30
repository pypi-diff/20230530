# Comparing `tmp/FlyBrainLab-1.1.8.tar.gz` & `tmp/FlyBrainLab-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/FlyBrainLab-1.1.8.tar", last modified: Wed Jun 15 06:45:40 2022, max compression
+gzip compressed data, was "dist/FlyBrainLab-1.1.9.tar", last modified: Tue Aug  2 14:45:23 2022, max compression
```

## Comparing `FlyBrainLab-1.1.8.tar` & `FlyBrainLab-1.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-06-15 06:45:40.000000 FlyBrainLab-1.1.8/
-drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-06-15 06:45:40.000000 FlyBrainLab-1.1.8/FlyBrainLab.egg-info/
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2277 2022-06-15 06:45:39.000000 FlyBrainLab-1.1.8/FlyBrainLab.egg-info/PKG-INFO
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      797 2022-06-15 06:45:39.000000 FlyBrainLab-1.1.8/FlyBrainLab.egg-info/SOURCES.txt
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)        1 2022-06-15 06:45:39.000000 FlyBrainLab-1.1.8/FlyBrainLab.egg-info/dependency_links.txt
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      427 2022-06-15 06:45:39.000000 FlyBrainLab-1.1.8/FlyBrainLab.egg-info/requires.txt
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       12 2022-06-15 06:45:39.000000 FlyBrainLab-1.1.8/FlyBrainLab.egg-info/top_level.txt
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2277 2022-06-15 06:45:40.000000 FlyBrainLab-1.1.8/PKG-INFO
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     1601 2021-04-29 14:44:09.000000 FlyBrainLab-1.1.8/README.md
-drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-06-15 06:45:40.000000 FlyBrainLab-1.1.8/flybrainlab/
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)   136124 2022-06-15 06:38:37.000000 FlyBrainLab-1.1.8/flybrainlab/Client.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    23583 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.8/flybrainlab/GFXComponent.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    35457 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.8/flybrainlab/NeurokernelComponent.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      769 2022-06-15 06:38:37.000000 FlyBrainLab-1.1.8/flybrainlab/__init__.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    34474 2022-06-15 06:38:37.000000 FlyBrainLab-1.1.8/flybrainlab/circuit.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     5465 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.8/flybrainlab/diagram_generator.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      520 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.8/flybrainlab/exceptions.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     1924 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.8/flybrainlab/ffbolabRunGFX.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    14287 2022-06-15 06:38:37.000000 FlyBrainLab-1.1.8/flybrainlab/graph.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2663 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.8/flybrainlab/nk_component_runner.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    23316 2021-04-27 18:01:14.000000 FlyBrainLab-1.1.8/flybrainlab/query.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      597 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.8/flybrainlab/run_nk_component.py
-drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-06-15 06:45:40.000000 FlyBrainLab-1.1.8/flybrainlab/utilities/
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      210 2021-04-27 18:01:14.000000 FlyBrainLab-1.1.8/flybrainlab/utilities/__init__.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    23809 2021-04-27 18:01:14.000000 FlyBrainLab-1.1.8/flybrainlab/utilities/neuroembed.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    27059 2022-06-15 06:38:37.000000 FlyBrainLab-1.1.8/flybrainlab/utilities/neurograph.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    14136 2022-06-15 06:38:37.000000 FlyBrainLab-1.1.8/flybrainlab/utilities/neurometry.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    23724 2021-04-27 18:01:14.000000 FlyBrainLab-1.1.8/flybrainlab/utilities/neurosynapsis.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2745 2022-06-15 06:38:37.000000 FlyBrainLab-1.1.8/flybrainlab/utilities/neurowatch.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     5859 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.8/flybrainlab/utils.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     7009 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.8/flybrainlab/widget.py
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      103 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.8/pyproject.toml
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       38 2022-06-15 06:45:40.000000 FlyBrainLab-1.1.8/setup.cfg
--rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     1540 2022-06-15 06:39:54.000000 FlyBrainLab-1.1.8/setup.py
+drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-08-02 14:45:23.000000 FlyBrainLab-1.1.9/
+drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-08-02 14:45:23.000000 FlyBrainLab-1.1.9/FlyBrainLab.egg-info/
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2277 2022-08-02 14:45:23.000000 FlyBrainLab-1.1.9/FlyBrainLab.egg-info/PKG-INFO
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      797 2022-08-02 14:45:23.000000 FlyBrainLab-1.1.9/FlyBrainLab.egg-info/SOURCES.txt
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)        1 2022-08-02 14:45:23.000000 FlyBrainLab-1.1.9/FlyBrainLab.egg-info/dependency_links.txt
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      427 2022-08-02 14:45:23.000000 FlyBrainLab-1.1.9/FlyBrainLab.egg-info/requires.txt
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       12 2022-08-02 14:45:23.000000 FlyBrainLab-1.1.9/FlyBrainLab.egg-info/top_level.txt
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2277 2022-08-02 14:45:23.000000 FlyBrainLab-1.1.9/PKG-INFO
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     1601 2021-04-29 14:44:09.000000 FlyBrainLab-1.1.9/README.md
+drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-08-02 14:45:23.000000 FlyBrainLab-1.1.9/flybrainlab/
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)   136286 2022-08-02 14:42:47.000000 FlyBrainLab-1.1.9/flybrainlab/Client.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    23583 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.9/flybrainlab/GFXComponent.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    35457 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.9/flybrainlab/NeurokernelComponent.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      769 2022-06-15 06:38:37.000000 FlyBrainLab-1.1.9/flybrainlab/__init__.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    38938 2022-08-02 14:42:47.000000 FlyBrainLab-1.1.9/flybrainlab/circuit.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     5465 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.9/flybrainlab/diagram_generator.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      520 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.9/flybrainlab/exceptions.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     1924 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.9/flybrainlab/ffbolabRunGFX.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    14285 2022-08-02 14:42:47.000000 FlyBrainLab-1.1.9/flybrainlab/graph.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2663 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.9/flybrainlab/nk_component_runner.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    26008 2022-08-02 14:42:47.000000 FlyBrainLab-1.1.9/flybrainlab/query.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      597 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.9/flybrainlab/run_nk_component.py
+drwxrwxr-x   0 yiyin     (1001) yiyin     (1001)        0 2022-08-02 14:45:23.000000 FlyBrainLab-1.1.9/flybrainlab/utilities/
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      210 2021-04-27 18:01:14.000000 FlyBrainLab-1.1.9/flybrainlab/utilities/__init__.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    23809 2021-04-27 18:01:14.000000 FlyBrainLab-1.1.9/flybrainlab/utilities/neuroembed.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    27059 2022-06-15 06:38:37.000000 FlyBrainLab-1.1.9/flybrainlab/utilities/neurograph.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    14136 2022-06-15 06:38:37.000000 FlyBrainLab-1.1.9/flybrainlab/utilities/neurometry.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)    23724 2021-04-27 18:01:14.000000 FlyBrainLab-1.1.9/flybrainlab/utilities/neurosynapsis.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     2745 2022-06-15 06:38:37.000000 FlyBrainLab-1.1.9/flybrainlab/utilities/neurowatch.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     5859 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.9/flybrainlab/utils.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     7009 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.9/flybrainlab/widget.py
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)      103 2021-02-23 19:43:41.000000 FlyBrainLab-1.1.9/pyproject.toml
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)       38 2022-08-02 14:45:23.000000 FlyBrainLab-1.1.9/setup.cfg
+-rw-rw-r--   0 yiyin     (1001) yiyin     (1001)     1540 2022-08-02 14:44:46.000000 FlyBrainLab-1.1.9/setup.py
```

### Comparing `FlyBrainLab-1.1.8/FlyBrainLab.egg-info/PKG-INFO` & `FlyBrainLab-1.1.9/FlyBrainLab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyBrainLab
-Version: 1.1.8
+Version: 1.1.9
 Summary: Main Client of the FlyBrainLab Project
 Home-page: https://flybrainlab.fruitflybrain.org
 Author: Mehmet Kerem Turkcan
 Author-email: mkt2126@columbia.edu
 License: BSD-3-Clause
 Description: # FlyBrainLab Client
```

### Comparing `FlyBrainLab-1.1.8/FlyBrainLab.egg-info/SOURCES.txt` & `FlyBrainLab-1.1.9/FlyBrainLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/PKG-INFO` & `FlyBrainLab-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyBrainLab
-Version: 1.1.8
+Version: 1.1.9
 Summary: Main Client of the FlyBrainLab Project
 Home-page: https://flybrainlab.fruitflybrain.org
 Author: Mehmet Kerem Turkcan
 Author-email: mkt2126@columbia.edu
 License: BSD-3-Clause
 Description: # FlyBrainLab Client
```

### Comparing `FlyBrainLab-1.1.8/README.md` & `FlyBrainLab-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/Client.py` & `FlyBrainLab-1.1.9/flybrainlab/Client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1492,16 +1492,17 @@
             else:
                 # try:
                 resNA['NLPquery'] = query
                 self.compiled = False
                 res = self.executeNAquery(
                     resNA, queryID=queryID, threshold=self.query_threshold
                 )
-                if 'show ' in query or 'add ' in query or 'remove ' in query:
-                    self.sendNeuropils()
+                # Since they don't do much here, should be called instead in more specific methods that require neuropil information after the NLPquery call.
+                # if 'show ' in query or 'add ' in query or 'remove ' in query:
+                #     self.sendNeuropils()
                 """
                 a = {}
                 a['data'] = {'info': {'success': 'Finished fetching results from database'}}
                 a['messageType'] = 'Data'
                 a['widget'] = 'NLP'
                 self.tryComms(a)
                 """
```

### Comparing `FlyBrainLab-1.1.8/flybrainlab/GFXComponent.py` & `FlyBrainLab-1.1.9/flybrainlab/GFXComponent.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/NeurokernelComponent.py` & `FlyBrainLab-1.1.9/flybrainlab/NeurokernelComponent.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/__init__.py` & `FlyBrainLab-1.1.9/flybrainlab/__init__.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/circuit.py` & `FlyBrainLab-1.1.9/flybrainlab/circuit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 import time
 import json
 from copy import deepcopy
 import traceback, sys
+import os
 
 import numpy as np
 import networkx as nx
 import pandas as pd
 import seaborn as sns
 sns.set(color_codes=True)
 
@@ -35,32 +36,33 @@
                 The connections between neurons that are larger than synapse_threshold will added (default 5).
             complete_synapses (bool or None):
                 Whether or not to include all synapses between pairs of neurons in the query_result.
                 If True, all synapses will be considered even they are not in the query_result.
                 If False, only the synapses in the query_result will be used to construct the graph.
                 (default True).
             model_name (str or None), model_version (str or None):
-                If specified, the model_name and model_version will be used to retrieve a executable circuit
+                If specified, the model_name and model_version will be used to retrieve an executable circuit
         """
         self.client = client
         if callback:
             client.experimentWatcher = self
         self.number_generator = numberGenerator()
-        self._js = []
+        self._submodules = {}
+        self._diagrams = {}
 
         # obtain self.circuit as a CircuitGraph
         # and self.model circuit as an empty graph or CircuitGraph
         if circuit is not None:
             self.circuit = client.get_circuit_graph(
                                 circuit,
                                 synapse_threshold = synapse_threshold,
                                 complete_synapses = complete_synapses)
             existing_models = self.query_for_models()
             if model_name is not None:
-                if model_name in existing_models:
+                if model_name in set(v['name'] for v in existing_models.values()):
                     if model_version is None:
                         self.current_model = self.prompt_to_choose_model(
                                     {rid: v for rid, v in existing_models.items() \
                                      if v['name'] == model_name})
                     else:
                         tmp = [rid for rid, v in existing_models.items() \
                                if v['name'] == model_name and v['version'] == model_version]
@@ -89,14 +91,15 @@
                     self.current_model_version = model_version
             else:
                 print(self.current_model)
                 tmp = existing_models[self.current_model]
                 self.current_model_name = tmp['name']
                 self.current_model_version = tmp['version']
                 self.graph = self._get_graph_from_circuit_and_model(self.circuit, self.current_model)
+                self.initialize_diagram_config(no_send = True)
                 self._get_diagram(self.current_model)
         else:
             if model_name is None:
                 raise ValueError('Executable Circuit must be speicified by a circuit or model name.')
             else:
                 existing_models = self.query_for_models_by_name(model_name)
                 if len(existing_models) == 0:
@@ -116,14 +119,15 @@
                                Cannot initialize without a circuit'.format(model_name, model_version))
 
             tmp = existing_models[self.current_model]
             self.current_model_name = tmp['name']
             self.current_model_version = tmp['version']
             self.ciruit = self._get_circuit_from_model(self.current_model)
             self.graph = self._get_graph_from_model(self.current_model)
+            self.initialize_diagram_config(no_send = True)
             self._get_diagram(self.current_model)
         self._updated = False
 
     def prompt_to_choose_model(self, models):
         list_of_models = list(models.items())
         res = input('Please select from the exisiting models to initialize the executable circuit, or press a to abort\n{}'.format('\n'.join(['{}: {} version {} (rid {})'.format(i, v['name'], v['version'], rid) for i, (rid, v) in enumerate(list_of_models)])))
         while True:
@@ -251,25 +255,26 @@
                      name of the neuron
         """
         if neuron_name in self.config['active']['neuron']:
             self.config['inactive']['neuron'][neuron_name] = \
                 self.config['active']['neuron'].pop(neuron_name)
             self._disable_single_neuron(neuron_name)
 
-    def disable_neurons(self, neurons):
+    def disable_neurons(self, neurons, no_send = False):
         """
         Disable neurons that exist in the diagram.
 
         Parameters
         ----------
         neurons:  list of neuron names
         """
         for neuron in neurons:
             self._disable_neuron(neuron)
-        self.send_to_GFX()
+        if not no_send:
+            self.send_to_GFX()
 
     def _disable_synapse(self, synapse_name):
         """
         Remove a synapse from the diagram.
         Should be called by GUI after simExperimentConfig is updated.
 
         Parameters
@@ -278,37 +283,39 @@
                      uname of the synapse
         """
         if synapse_name in self.config['active']['synapse']:
             self.config['inactive']['synapse'][synapse_name] = \
                 self.config['active']['synapse'].pop(synapse_name)
 
 
-    def disable_synapses(self, synapses):
+    def disable_synapses(self, synapses, no_send = False):
         """
         Disable synapses that exist in the diagram.
 
         Parameters
         ----------
         synapses:  list of synapse names
         """
         for synapse in synapses:
             self._disable_synapse(synapse)
-        self.send_to_GFX()
+        if not no_send:
+            self.send_to_GFX()
 
-    def enable_neurons(self, neurons):
+    def enable_neurons(self, neurons, no_send = False):
         """
         Enable neurons that exist in the diagram.
 
         Parameters
         ----------
         neurons:  list of neuron names
         """
         for neuron in neurons:
             self._enable_neuron(neuron)
-        self.send_to_GFX()
+        if not no_send:
+            self.send_to_GFX()
 
     def _enable_neuron(self, neuron_name):
         """
         Add a neuron that exists in diagram.
         Should be called by GUI after simExperimentConfig is updated.
 
         Parameters
@@ -331,32 +338,33 @@
                         self._enable_synapse(self.graph.nodes[pre]['uname'])
 
             for pre, post, k in list(out_edges):
                 if k['class'] == 'SendsTo':
                     if self.graph.nodes[post]['class'] == 'Synapse':
                         self._enable_synapse(self.graph.nodes[post]['uname'])
 
-    def enable_synapses(self, synapses):
+    def enable_synapses(self, synapses, no_send = False):
         """
         Enable synapses that exist in the diagram.
 
         Parameters
         ----------
         synapses:  list of synapse unames
         """
         for synapse in synapses:
             self._enable_synapse(synapse)
-        self.send_to_GFX()
+        if not no_send:
+            self.send_to_GFX()
 
     def _enable_synapse(self, synapse_name):
         if synapse_name in self.config['inactive']['synapse']:
             self.config['active']['synapse'][synapse_name] = \
                 self.config['inactive']['synapse'].pop(synapse_name)
 
-    def loadExperimentConfig(self, x):
+    def loadExperimentConfig(self, x, no_send = False):
         try:
             lastObject = x['lastObject']
             lastLabel = x['lastLabel']
             action = x['lastAction']
             if lastObject == "neuron":
                 if action == "deactivated":
                     self._disable_neuron(lastLabel)
@@ -389,15 +397,16 @@
             v = deepcopy(x[self.current_model_name][n])
             if not v.get('params', {}).get('name', 'Default') == 'Default':
                 self.update_model(n, v['params'], v['states'], no_send = True)
         except Exception as e:
             exc_type, exc_value, exc_traceback = sys.exc_info()
             tb = ''.join(traceback.format_exception(exc_type, exc_value, exc_traceback))
             self.client.raise_error(e, "An error occured during model update:\n" + tb)
-        self.send_to_GFX()
+        if not no_send:
+            self.send_to_GFX()
 
     def find_model(self, rid):
         return {pre: self.graph.nodes[pre] for pre, post, v in self.graph.in_edges(rid, data = True) if v['class'] == 'Models'}
 
     def find_neurotransmitter(self, rid):
         return {post: self.graph.nodes[post] for pre, post, v in self.graph.out_edges(rid, data = True) if v['class'] == 'HasData' and self.graph.nodes[post]['class'] == 'NeurotransmitterData'}
 
@@ -427,33 +436,92 @@
                           "object":{"memory": 0}
                          }
                         ]
                 }
         res = self.client.executeNAquery(task, temp = True)
         circuit_diagrams = {rid: v for rid, v in res.graph.nodes(data = True) if v['class'] == 'CircuitDiagram'}
         tmp = circuit_diagrams.popitem()[1]
-        diagram = tmp['diagram']
-        js = tmp['js']
-        self._load_diagram_str(diagram)
-        self._load_js_str(js)
+        diagrams = tmp['diagrams']
+        submodules = tmp['submodules']
+        primary_diagram = diagrams.pop('primary')
+        primary_submodule = submodules.pop('primary')
+        for name, diagram in diagrams.items():
+            self._load_diagram_from_str(diagram, primary = (name == primary_diagram),
+                                   name = name, display = False)
+        for name, submodule in submodules.items():
+            self._load_submodule_from_str(submodule, primary = (name == primary_submodule),
+                                     name = name, exec = False)
+        self.display_diagram()
 
-    def load_diagram(self, filename):
+    def load_diagram(self, filename, primary = False, name = None, display = True):
         with open(filename, 'r') as file:
             data = file.read()
-        self._load_diagram_str(data)
+        if name is None:
+            name = os.path.splitext(os.path.split(filename)[-1])[0]
+        self._load_diagram_from_str(data, primary = primary, name = name, display = display)
+
+    def _load_diagram_from_str(self, data, primary = False, name = None, display = True):
+        if name is None:
+            name = 'diagram{}'.format(
+                len(self._diagrams)-1 if 'primary' in self._diagrams else len(self._diagrams))
+            print('Automatically assigning diagram name as {}'.format(name))
+        self._diagrams[name] = data
+        if primary:
+            self._diagrams['primary'] = name
+        if len(self._diagrams) == 1:
+            self._diagrams['primary'] = name
+        code = """
+window._neuGFX.mods.FlyBrainLab.circuitContent['{name}'] = `{data}`;
+""".format(name = name, data = data.replace('`', '\`'))
+        self.client.tryComms({'widget':'GFX',
+                              'messageType': 'eval',
+                              'data': {'data': code}})
+        if display:
+            self.display_diagram(name)
+    
+    @property
+    def primary_diagram(self):
+        if 'primary' in self._diagrams:
+            return self._diagrams['primary']
+        else:
+            raise ValueError('primary diagram not loaded')
+
+    def display_diagram(self, name = None, submodule = None):
+        if name is None:
+            name = self.primary_diagram
+
+        if submodule is None:
+            try:
+                submodule = self.primary_submodule
+            except ValueError:
+                pass
+            
+        if submodule is None:
+            callback = ""
+        else:
+            callback = """
+eval(window.submodules['{module}']);
+console.log("Submodule {module} loaded.");
+""".format(module = submodule)
+
+        code = """
+window._neuGFX.mods.FlyBrainLab.gfx.loadSVGFromString(
+    window._neuGFX.mods.FlyBrainLab.circuitContent['{name}'],
+    function(){{ {callback} }});
+window._neuGFX.mods.FlyBrainLab.circuitName = '{name}';
+window._neuGFX.mods.FlyBrainLab.addCircuit('{name}');
+""".format(name = name, callback = callback)
 
-    def _load_diagram_str(self, data):
-        self._diagram = data
         self.client.tryComms({'widget':'GFX',
-                           'messageType': 'loadCircuitFromString',
-                           'data': {'string': data, 'name': 'diagram'}})
+                           'messageType': 'eval',
+                           'data': {'data': code}})
         time.sleep(1)
-        self.initialize_diagram_config()
+        self.send_to_GFX()
 
-    def initialize_diagram_config(self):
+    def initialize_diagram_config(self, no_send = False):
         config = {'inactive': {'neuron': {},
                                'synapse': {}},
                   'active': {'neuron': {},
                              'synapse': {}}}
 
         for rid, v in self.get('Neuron').items():
             model_node = self.find_model(rid)
@@ -482,29 +550,63 @@
             else:
                 node_data = {'name': 'Default'}
                 new_node_data = {'params': node_data,
                                  'states': {}}
                 config['active']['synapse'][v['uname']] = new_node_data
 
         self.config = config
-        self.send_to_GFX()
+        if not no_send:
+            self.send_to_GFX()
 
     def load_js(self, filename):
+        DeprecationWarning("load_js method has been deprecated, use load_submodule instead")
+        self.load_submodule(filename)
+
+    def load_submodule(self, filename, primary = False, name = None, exec = True):
         with open(filename, 'r') as file:
             data = file.read()
-        self._load_js_str(data)
+        if name is None:
+            name = os.path.splitext(os.path.split(filename)[-1])[0]
+        self._load_submodule_from_str(data, primary = primary, name = name, exec = exec)
+
+    def _load_submodule_from_str(self, data, primary = False, name = None, exec = True):
+        if name is None:
+            name = 'submodule{}'.format(
+                len(self._submodules)-1 if 'primary' in self._submodules else len(self._submodules))
+        self._submodules[name] = data
+        if primary:
+            self._submodules['primary'] = name
+        else:
+            if len(self._submodules) == 1:
+                self._submodules['primary'] = name
+        self.client.tryComms({'messageType': 'loadSubmodule',
+                              'widget':'GFX',
+                              'data': {'data': data,
+                                       'name': name}
+                            })
+        time.sleep(1)
+        if exec:
+            self.execute_submodule(name)
+        
+    @property
+    def primary_submodule(self):
+        if 'primary' in self._submodules:
+            return self._submodules['primary']
+        else:
+            raise ValueError('primary submodule not loaded')
 
-    def _load_js_str(self, data):
-        self._js.append(data)
-        self.client.tryComms({'messageType': 'eval', 'widget':'GFX',
-                           'data': {'data': data}})
+    def execute_submodule(self, name):
+        code = "window.submodules['{}']".format(name)
+        self.client.tryComms({'widget':'GFX', 
+                        'messageType': 'eval', 
+                        'data': {'data': code}})
         time.sleep(1)
 
     def clear_js(self):
-        self._js = []
+        self._js = {}
 
     def create_executable_graph(self, model_name):
         not_modeled_nodes = [v['uname'] for n, v in self.graph.nodes(data=True) \
                           if v['class'] in ['Neuron', 'Synapse', 'InferredSynapse'] \
                           and not self._exists_model(n)]
         if len(not_modeled_nodes):
             raise ValueError('The following neurons/synapses in the circuit do not have a corresponding model:\n\
@@ -576,36 +678,38 @@
             self.config['inactive'][node_type][node] = pp
         else:
             raise ValueError('{} not in either active or inactive'.format(n))
         self._updated = True
         if not no_send:
             self.send_to_GFX()
 
-    def update_model_like(self, nodes, node_to_copy):
+    def update_model_like(self, nodes, node_to_copy, no_send = False):
         if not isinstance(nodes, list):
             nodes = [nodes]
         # circuit_node = self.graph.nodes[self.uname_to_rid[node_to_copy]]
         model_node = self.find_model(self.uname_to_rid[node_to_copy])
         if len(model_node) == 1:
             rid, v = model_node.popitem()
         elif len(model_node) == 0:
             raise ValueError('No node {} detected.'.format(node_to_copy))
         else:
             raise ValueError('Duplicate nodes {} detected.'.format(node_to_copy))
         vv = deepcopy(v)
         vv['params']['name'] = vv['class']
         for node in nodes:
             self.update_model(node, vv['params'], vv['states'], no_send = True)
-        self.send_to_GFX()
+        if not no_send:
+            self.send_to_GFX()
 
-    def update_models(self, node_params):
+    def update_models(self, node_params, no_send = False):
         for node, v in node_params.items():
             self.update_model(node, v['params'], states = v.get('states', None),
                               no_send = True)
-        self.send_to_GFX()
+        if not no_send:
+            self.send_to_GFX()
 
     def flush_model(self, model_name = None, model_version = None):
         not_modeled_nodes = [v['uname'] for n, v in self.graph.nodes(data=True) \
                           if v['class'] in ['Neuron', 'Synapse', 'InferredSynapse'] \
                           and not self._exists_model(n)]
         if len(not_modeled_nodes):
             raise ValueError('The following neurons/synapses in the circuit do not have a corresponding model:\n\
@@ -614,15 +718,15 @@
         graph = self._reform_graph()
         res = self.client.rpc('ffbo.na.NeuroArch.write.{}'.format(self.client.naServerID),
                         'create_model_from_circuit',
                         model_name if model_name is not None else self.current_model_name,
                         model_version if model_version is not None else self.current_model_version,
                         {'nodes': list(graph.nodes(data=True)),
                          'edges': list(graph.edges(data=True))},
-                        circuit_diagram = self._diagram, js = '\n'.join(self._js))
+                        circuit_diagrams = self._diagrams, submodules = self._submodules)
         if 'success' in res:
             rid_map = res['success']['data']
         else:
             raise FlyBrainLabNAserverException(res['error']['message']+'\n'+res['error']['exception'])
         self._update_node_rids(rid_map)
         if model_name is not None:
             self.current_model_name = model_name
```

### Comparing `FlyBrainLab-1.1.8/flybrainlab/diagram_generator.py` & `FlyBrainLab-1.1.9/flybrainlab/diagram_generator.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/exceptions.py` & `FlyBrainLab-1.1.9/flybrainlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/ffbolabRunGFX.py` & `FlyBrainLab-1.1.9/flybrainlab/ffbolabRunGFX.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/graph.py` & `FlyBrainLab-1.1.9/flybrainlab/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
             if "vertices" in morphology_data:
                 vertices = morphology_data["vertices"]
                 for j in range(len(vertices)//3):
                     vertices[j*3] = vertices[j*3]*self.x_scale + self.x_shift
                     vertices[j*3+1] = vertices[j*3+1]*self.y_scale + self.y_shift
                     vertices[j*3+2] = vertices[j*3+2]*self.z_scale + self.z_shift
 
-
     def _finalize_nx(self):
         while self.locked:
             time.sleep(1)
 
         G = self.graph
         G.add_nodes_from(list(self.data['nodes'].items()))
         G.add_edges_from(self.data['edges'])
@@ -258,15 +257,14 @@
     def getInfo(self, rid):
         pass
 
     #TODO
     def getStats(self, rid = None, neuron_name = None):
         pass
 
-
     @property
     def rids(self):
         return list(self.uname_to_rid.values())
 
     def __getitem__(self, key):
         if key.startswith('#'):
             node = self.graph.nodes[key]
```

### Comparing `FlyBrainLab-1.1.8/flybrainlab/nk_component_runner.py` & `FlyBrainLab-1.1.9/flybrainlab/nk_component_runner.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/query.py` & `FlyBrainLab-1.1.9/flybrainlab/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,19 @@
         res = self.client.rpc(
                 uri,
                 name, version = version,
                 options=CallOptions(timeout=10000) )
         result = self._check_result(res)
         return result
 
+    def flush_edges(self):
+        res = self.NeuroArchWrite_rpc('flush_edges')
+        result = self._check_result(res)
+        return result
+
     def add_Species(self, name, stage, sex, synonyms = None):
         """
         Add a Species.
 
         Parameters
         ----------
         name : str
@@ -333,16 +338,16 @@
             neurotransmitters, and have one to one corresponsdence in the same order.
         data_source : neuroarch.models.DataSource (optional)
             The datasource. If not specified, default DataSource will be used.
         circuit : 
 
         Returns
         -------
-        neuron : neuroarch.models.Neuron
-            Created Neuron object
+        result : dict
+            Properties of the created NeuronFragement object
         """
         res = self.NeuroArchWrite_rpc(
                          'add_Neuron', uname, name,
                          referenceId = referenceId,
                          locality = locality,
                          synonyms = synonyms,
                          info = info,
@@ -351,14 +356,69 @@
                          neurotransmitters = neurotransmitters,
                          neurotransmitters_datasources = neurotransmitters_datasources,
                          data_source = data_source,
                          circuit = circuit)
         result = self._check_result(res)
         return result
 
+    def add_NeuronFragment(self, uname,
+                           name,
+                           referenceId = None,
+                           info = None,
+                           morphology = None,
+                           arborization = None,
+                           data_source = None):
+        """
+        Create a NeuronFragment Record and link it to the related node types.
+
+        Parameters
+        ----------
+        uname : str
+            A unqiue name assigned to the neuron, must be unique within the DataSource
+        name : str
+            Name of the neuron, typically the cell type.
+        referenceId : str (optional)
+            Unique identifier in the original data source
+        info : dict (optional)
+            Additional information about the neuron, values must be str
+        morphology : list of dict (optional)
+            Each dict in the list defines a type of morphology of the neuron.
+            Must be loaded from a file.
+            The dict must include the following key to indicate the type of morphology:
+                {'type': 'swc'/'obj'/...}
+            Additional keys must be provides, either 'filename' with value
+            indicating the file to be read for the morphology,
+            or a full definition of the morphology according the schema.
+            For swc, required fields are ['sample', 'identifier', 'x', 'y, 'z', 'r', 'parent'].
+            More formats pending implementation.
+        arborization : list of dict (optional)
+            A list of dictionaries define the arborization pattern of
+            the neuron in neuropils, subregions, and tracts, if applicable, with
+            {'type': 'neuropil' or 'subregion' or 'tract',
+             'dendrites': {'EB': 20, 'FB': 2},
+             'axons': {'NO': 10, 'MB': 22}}
+            Name of the regions must already be present in the database.
+        data_source : models.DataSource (optional)
+            The datasource. If not specified, default DataSource will be used.
+
+        Returns
+        -------
+        neuron : neuroarch.models.Neuron
+            Created Neuron object
+        """
+        res = self.NeuroArchWrite_rpc(
+                        'add_NeuronFragment', uname, name,
+                         referenceId = referenceId,
+                         info = info,
+                         morphology = morphology,
+                         arborization = arborization,
+                         data_source = data_source)
+        result = self._check_result(res)
+        return result
+
     def add_neurotransmitter(self, neuron, neurotransmitters, data_sources = None):
         """
         Parameters
         ----------
         neuron : neuroarch.models.Neuron subclass
             An instance of Neuron class to which the neurotransmitters will be associated to
         neurotransmitters : str or list of str
```

### Comparing `FlyBrainLab-1.1.8/flybrainlab/run_nk_component.py` & `FlyBrainLab-1.1.9/flybrainlab/run_nk_component.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/utilities/neuroembed.py` & `FlyBrainLab-1.1.9/flybrainlab/utilities/neuroembed.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/utilities/neurograph.py` & `FlyBrainLab-1.1.9/flybrainlab/utilities/neurograph.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/utilities/neurometry.py` & `FlyBrainLab-1.1.9/flybrainlab/utilities/neurometry.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/utilities/neurosynapsis.py` & `FlyBrainLab-1.1.9/flybrainlab/utilities/neurosynapsis.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/utilities/neurowatch.py` & `FlyBrainLab-1.1.9/flybrainlab/utilities/neurowatch.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/utils.py` & `FlyBrainLab-1.1.9/flybrainlab/utils.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/flybrainlab/widget.py` & `FlyBrainLab-1.1.9/flybrainlab/widget.py`

 * *Files identical despite different names*

### Comparing `FlyBrainLab-1.1.8/setup.py` & `FlyBrainLab-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
 setup(
     name="FlyBrainLab",
-    version="1.1.8",
+    version="1.1.9",
     description="Main Client of the FlyBrainLab Project",
     author="Mehmet Kerem Turkcan",
     author_email="mkt2126@columbia.edu",
     url="https://flybrainlab.fruitflybrain.org",
     download_url="",
     license="BSD-3-Clause",
     long_description=long_description,
```

