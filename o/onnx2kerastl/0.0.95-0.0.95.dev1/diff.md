# Comparing `tmp/onnx2kerastl-0.0.95.tar.gz` & `tmp/onnx2kerastl-0.0.95.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.95.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.95.dev1.tar", max compression
```

## Comparing `onnx2kerastl-0.0.95.tar` & `onnx2kerastl-0.0.95.dev1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1067 2022-05-24 13:45:54.506384 onnx2kerastl-0.0.95/LICENSE
--rw-r--r--   0        0        0       66 2022-05-26 14:37:02.229998 onnx2kerastl-0.0.95/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-04-30 14:23:13.629683 onnx2kerastl-0.0.95/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2022-07-21 11:24:20.166257 onnx2kerastl-0.0.95/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2022-10-13 14:52:08.546058 onnx2kerastl-0.0.95/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    13572 2023-05-14 16:26:09.893812 onnx2kerastl-0.0.95/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11968 2023-05-14 16:26:09.894508 onnx2kerastl-0.0.95/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      584 2023-05-21 12:41:16.202993 onnx2kerastl-0.0.95/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2022-10-19 12:00:07.113921 onnx2kerastl-0.0.95/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2022-05-30 10:49:29.064709 onnx2kerastl-0.0.95/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2022-05-24 13:45:54.510879 onnx2kerastl-0.0.95/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0     1730 2023-05-14 16:26:09.897336 onnx2kerastl-0.0.95/onnx2kerastl/customonnxlayer/onnxlstm.py
--rw-r--r--   0        0        0      605 2022-08-04 16:14:29.703956 onnx2kerastl-0.0.95/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2022-05-30 11:45:55.347781 onnx2kerastl-0.0.95/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9372 2023-05-30 07:33:24.833301 onnx2kerastl-0.0.95/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2022-07-21 11:24:20.167508 onnx2kerastl-0.0.95/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3947 2023-05-30 07:33:24.835312 onnx2kerastl-0.0.95/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-04-02 11:17:38.561077 onnx2kerastl-0.0.95/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3791 2023-05-14 16:26:09.898000 onnx2kerastl-0.0.95/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2022-05-24 13:45:54.512524 onnx2kerastl-0.0.95/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5551 2023-05-14 16:26:09.898639 onnx2kerastl-0.0.95/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    16027 2023-05-30 07:33:24.835790 onnx2kerastl-0.0.95/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     3015 2023-04-30 14:23:13.631034 onnx2kerastl-0.0.95/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-04-02 11:17:38.563036 onnx2kerastl-0.0.95/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    18024 2023-05-30 07:33:24.836993 onnx2kerastl-0.0.95/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     5006 2023-05-30 07:51:44.935616 onnx2kerastl-0.0.95/onnx2kerastl/sampling_layers.py
--rw-r--r--   0        0        0     1655 2023-04-02 11:17:38.563943 onnx2kerastl-0.0.95/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     4415 2023-04-02 11:17:38.564336 onnx2kerastl-0.0.95/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1030 2023-05-30 09:12:53.130986 onnx2kerastl-0.0.95/pyproject.toml
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.95/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-17 10:05:24.840017 onnx2kerastl-0.0.95.dev1/LICENSE
+-rw-r--r--   0        0        0       66 2023-05-17 10:05:24.840536 onnx2kerastl-0.0.95.dev1/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-05-17 10:05:24.840790 onnx2kerastl-0.0.95.dev1/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2023-05-17 10:05:24.840968 onnx2kerastl-0.0.95.dev1/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2023-05-17 10:05:24.841141 onnx2kerastl-0.0.95.dev1/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    14493 2023-05-30 11:55:43.175666 onnx2kerastl-0.0.95.dev1/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11968 2023-05-17 10:05:24.841507 onnx2kerastl-0.0.95.dev1/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      584 2023-05-23 13:09:48.518074 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-17 10:05:24.841906 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2023-05-17 10:05:24.842046 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2023-05-17 10:05:24.842190 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0     1730 2023-05-17 10:05:24.842337 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxlstm.py
+-rw-r--r--   0        0        0      605 2023-05-17 10:05:24.842473 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2023-05-17 10:05:24.842602 onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9380 2023-05-30 11:55:17.256120 onnx2kerastl-0.0.95.dev1/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2023-05-17 10:05:24.842900 onnx2kerastl-0.0.95.dev1/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3947 2023-05-30 11:43:46.982250 onnx2kerastl-0.0.95.dev1/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-05-30 11:55:17.207286 onnx2kerastl-0.0.95.dev1/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3791 2023-05-17 10:05:24.843376 onnx2kerastl-0.0.95.dev1/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2023-05-17 10:05:24.843508 onnx2kerastl-0.0.95.dev1/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5551 2023-05-17 10:05:24.843673 onnx2kerastl-0.0.95.dev1/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    16027 2023-05-30 11:41:40.091917 onnx2kerastl-0.0.95.dev1/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-05-17 10:05:24.844012 onnx2kerastl-0.0.95.dev1/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-05-17 10:05:24.844205 onnx2kerastl-0.0.95.dev1/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    17737 2023-05-30 11:55:17.264481 onnx2kerastl-0.0.95.dev1/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     5011 2023-05-30 11:38:10.695884 onnx2kerastl-0.0.95.dev1/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-05-17 10:05:24.844792 onnx2kerastl-0.0.95.dev1/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     5629 2023-05-30 11:55:17.248648 onnx2kerastl-0.0.95.dev1/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1035 2023-05-30 12:05:54.899568 onnx2kerastl-0.0.95.dev1/pyproject.toml
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.95.dev1/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.95/LICENSE` & `onnx2kerastl-0.0.95.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/converter.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 import importlib.util
 import inspect
 import logging
 import uuid
 
 import keras
-
 from .customonnxlayer import onnx_custom_objects_map
 from .exceptions import UnsupportedLayer, OnnxUnsupported
 from .layers import AVAILABLE_CONVERTERS
 
 onnx_imported = False
 package_name = 'onnx'
 spec = importlib.util.find_spec(package_name)
@@ -110,26 +109,29 @@
         for onnx_i in onnx_inputs:
             if onnx_i.name == input_name:
                 dtype = None if input_types is None else input_types[i]
                 input_shape = [i.dim_value for i in onnx_i.type.tensor_type.shape.dim]
                 input_shape = [shape if shape != 0 else None for shape in input_shape]
                 batch_size = input_shape[0]
                 input_shape = input_shape[1:]
+                if len(input_shape) == 0:
+                    input_shape = 1
                 if batch_size is None:
                     layers[input_name] = keras.layers.InputLayer(
                         input_shape=input_shape, name=input_name, dtype=dtype).output
                 else:
                     layers[input_name] = keras.layers.InputLayer(
                         input_shape=input_shape, name=input_name, dtype=dtype, batch_size=batch_size).output
                 keras_inputs.append(layers[input_name])
 
                 logger.debug('Found input {0} with shape {1}'.format(input_name, input_shape))
 
     # Convert every operation separable
     node_names = []
+    embedding_weights_mapping = {}
     for node_index, node in enumerate(onnx_nodes):
         if node.op_type == 'If':
             if layers[node.input[0]][0]:
                 replace_node = node.attribute[0].g.node[0]
             else:
                 replace_node = node.attribute[1].g.node[0]
             replace_node.output.pop()
@@ -193,24 +195,36 @@
         logger.debug('node_name: %s', node_name)
         logger.debug('node_params: %s', node_params)
         logger.debug('...')
 
         logger.debug('Check if all inputs are available:')
         if len(node.input) == 0 and node_type != 'Constant':
             raise AttributeError('Operation doesn\'t have an input. Aborting.')
-
         for i, node_input in enumerate(node.input):
             logger.debug('Check input %i (name %s).', i, node_input)
+
+            # for case of weights sharing, map the shared weights to determine
+            # if a Gather layer is an embedding layer
+            if node_type == 'Identity' and node_input in weights:
+                embedding_weights_mapping[node_name] = node_input
+
+            # check conditions for embedding layer
+            is_in_weights = node_input in weights  # is this node input in weights
+            is_mapped_to_weights = embedding_weights_mapping.get(node_input, '') in weights  # is this node inputs weights are shared with other input
+            is_embedding = is_in_weights or is_mapped_to_weights  # if either is true this layer is a possible embedding layer
+
+            # if a layer is of type Gather and its input is in weights (or mapped to a weights input)
+            # it's an embedding layer
+            if node_type == "Gather" and is_embedding:
+                node_params['is_embedding'] = True
+
             if node_input not in layers:
                 logger.debug('The input not found in layers / model inputs.')
-
                 if node_input in weights:
                     logger.debug('Found in weights, add as a numpy constant.')
-                    if node_type == "Gather" and i == 0:
-                        node_params['is_embedding'] = True
                     layers[node_input] = weights[node_input]
                 else:
                     if node_input == "" and node_type in ('Pad', 'Resize', 'Clip', 'LSTM'):
                         continue
                     else:
                         raise AttributeError('Current node is not in weights / model inputs / layers.')
         else:
```

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/convolution_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/customonnxlayer/__init__.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/customonnxlayer/onnxlstm.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxlstm.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/elementwise_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,19 +221,19 @@
     for i, inp in enumerate(node.input):
         input_ = ensure_tf_type(layers[inp], layers[list(layers)[0]], name="%s_const%i" % (keras_name, i + 1))
         inputs.append(input_)
     layers[node_name] = keras.layers.Average(name=keras_name)(inputs)
 
 
 def convert_equal(node, params, layers, lambda_func, node_name, keras_name):
-    layers[node_name] = layers[node.input[0]] == layers[node.input[1]]
+    layers[node_name] = tf.equal(layers[node.input[0]], layers[node.input[1]])
 
 
 def convert_where(node, params, layers, lambda_func, node_name, keras_name):
-    layers[node_name] = np.where(layers[node.input[0]], layers[node.input[1]], layers[node.input[2]])
+    layers[node_name] = tf.where(layers[node.input[0]], layers[node.input[1]], layers[node.input[2]])
 
 
 def convert_scatter_nd(node, params, layers, lambda_func, node_name, keras_name):
     """
     Convert ScatterND layer
     :param node: current operation node
     :param params: operation attributes
```

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/ltsm_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/reshape_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import keras
 import numpy as np
 import tensorflow as tf
 from keras import backend as K
 from keras.layers import SlicingOpLambda
 
-from .utils import is_numpy, ensure_tf_type, ensure_numpy_type
+from .utils import is_numpy, ensure_tf_type, ensure_numpy_type, match_tensors_rank
 
 
 def convert_transpose(node, params, layers, lambda_func, node_name, keras_name):
     """
     Convert transpose.
     :param node: current operation node
     :param params: operation attributes
@@ -145,14 +145,15 @@
                 try:
                     layers[node_name] = tf.concat(layer_input, axis=params['axis'], name=keras_name)
                 except Exception as ex:
                     # might be due to type mismatch between different inputs of tf.concat
                     raise
 
             else:
+                layer_input = match_tensors_rank(layer_input)
                 layers[node_name] = keras.layers.concatenate(inputs=layer_input,
                                                              axis=params['axis'],
                                                              name=keras_name)
         else:
             layers[node_name] = layer_input[0]
 
 
@@ -216,24 +217,19 @@
                     tf_shape = tf.shape(input_0)
                     layers[node_name] = tf.reshape(input_0, [*tf_shape[:first_mismatch], -1, *tf_shape[end_idx_match:]])
                 else:
                     logger.debug('The first argument is Keras/tf layer. Apply keras.Reshape.')
                     logger.debug('Target shape :')
                     logger.debug(np.int32(input_1[1:]))
 
-                    if len(np.int32(input_1[1:])) == 1 and np.int32(input_1[1:])[0] == -1:
-                        logger.debug('The first argument is Keras/tf layer. Apply keras.Flatten.')
-                        flatten = keras.layers.Flatten(name=keras_name)
-                        layers[node_name] = flatten(input_0)
+                    if input_0.shape[0] != input_1[0]:  # keras reshape don't work
+                        layers[node_name] = tf.reshape(input_0, input_1, name=keras_name)
                     else:
-                        if input_0.shape[0] != input_1[0]:  # keras reshape don't work
-                            layers[node_name] = tf.reshape(input_0, input_1, name=keras_name)
-                        else:
-                            reshape = keras.layers.Reshape(np.int32(input_1[1:]), name=keras_name)
-                            layers[node_name] = reshape(input_0)
+                        reshape = keras.layers.Reshape(np.int32(input_1[1:]), name=keras_name)
+                        layers[node_name] = reshape(input_0)
     else:
         raise AttributeError('Can\'t reshape dynamic size.')
 
 
 def convert_unsqueeze(node, params, layers, lambda_func, node_name, keras_name):
     """
     Convert unsqueeze.
```

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/sampling_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/sampling_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     alphas = []
     floors = []
     ceils = []
     index_order = [0, 1] if indexing == "ij" else [1, 0]
     # unstacked_query_points = tf.unstack(query_points, axis=2, num=2)
 
     for i, dim in enumerate(index_order):
-        queries = query_points[:, :, dim]
+        queries = query_points[:, :, dim, ...]
         # queries = unstacked_query_points[dim]
 
         size_in_indexing_dimension = grid_shape[i + 1]
 
         # max_floor is size_in_indexing_dimension - 2 so that max_floor + 1
         # is still a valid index into the grid.
         max_floor = tf.cast(size_in_indexing_dimension - 2, query_type)
```

### Comparing `onnx2kerastl-0.0.95/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.95.dev1/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.95/pyproject.toml` & `onnx2kerastl-0.0.95.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.95"
+version = "0.0.95.dev1"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.95/PKG-INFO` & `onnx2kerastl-0.0.95.dev1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.95
+Version: 0.0.95.dev1
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

