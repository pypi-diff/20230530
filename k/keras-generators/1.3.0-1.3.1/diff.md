# Comparing `tmp/keras_generators-1.3.0-py3-none-any.whl.zip` & `tmp/keras_generators-1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 27904 bytes, number of entries: 16
+Zip file size: 28039 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 examples/__init__.py
 -rw-rw-rw-  2.0 fat     6233 b- defN 23-Apr-13 14:38 examples/predict_stock_price.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 keras_generators/__init__.py
 -rw-rw-rw-  2.0 fat     7068 b- defN 23-Mar-08 16:27 keras_generators/callbacks.py
 -rw-rw-rw-  2.0 fat      520 b- defN 23-Apr-13 14:20 keras_generators/common.py
 -rw-rw-rw-  2.0 fat    10842 b- defN 23-Mar-08 16:27 keras_generators/encoders.py
--rw-rw-rw-  2.0 fat    33395 b- defN 23-Mar-08 16:27 keras_generators/generators.py
+-rw-rw-rw-  2.0 fat    36086 b- defN 23-May-30 11:06 keras_generators/generators.py
 -rw-rw-rw-  2.0 fat     4139 b- defN 23-Mar-08 19:39 keras_generators/splitters.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 keras_generators/model_abstractions/__init__.py
 -rw-rw-rw-  2.0 fat     7224 b- defN 23-Mar-08 20:48 keras_generators/model_abstractions/model_object.py
 -rw-rw-rw-  2.0 fat     3188 b- defN 23-Apr-13 14:19 keras_generators/model_abstractions/model_params.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Apr-13 14:41 keras_generators-1.3.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9891 b- defN 23-Apr-13 14:41 keras_generators-1.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 14:41 keras_generators-1.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 23-Apr-13 14:41 keras_generators-1.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1421 b- defN 23-Apr-13 14:41 keras_generators-1.3.0.dist-info/RECORD
-16 files, 95597 bytes uncompressed, 25518 bytes compressed:  73.3%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-30 11:07 keras_generators-1.3.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9891 b- defN 23-May-30 11:07 keras_generators-1.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 11:07 keras_generators-1.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 23-May-30 11:07 keras_generators-1.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1421 b- defN 23-May-30 11:07 keras_generators-1.3.1.dist-info/RECORD
+16 files, 98288 bytes uncompressed, 25653 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: keras_generators/model_abstractions/model_object.py
 Comment: 
 
 Filename: keras_generators/model_abstractions/model_params.py
 Comment: 
 
-Filename: keras_generators-1.3.0.dist-info/LICENSE
+Filename: keras_generators-1.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: keras_generators-1.3.0.dist-info/METADATA
+Filename: keras_generators-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: keras_generators-1.3.0.dist-info/WHEEL
+Filename: keras_generators-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: keras_generators-1.3.0.dist-info/top_level.txt
+Filename: keras_generators-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: keras_generators-1.3.0.dist-info/RECORD
+Filename: keras_generators-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## keras_generators/generators.py

```diff
@@ -764,7 +764,78 @@
             shuffle=self.shuffle,
             batch_size=self.batch_size,
         )
 
     def get_X_generator(self, batch_size: Optional[int] = None) -> XBatchGenerator:
         batch_size = batch_size or self.batch_size
         return XBatchGenerator(self.inputs, batch_size)
+
+
+class XYWBatchGenerator(XYBatchGenerator):
+    @validate_arguments(config=ArbitraryTypes)
+    def __init__(
+        self,
+        inputs_map: Dict[str, DataSource],
+        targets_map: Dict[str, DataSource],
+        weight_map: Dict[str, DataSource],
+        shuffle: bool = True,
+        batch_size: int = 128,
+    ):
+        super().__init__(inputs_map=inputs_map, targets_map=targets_map, shuffle=shuffle, batch_size=batch_size)
+        self.weights = weight_map
+
+    @validate_arguments
+    def _get_batch(self, start_index: int, end_index: int) -> Tuple[Dict[str, np.ndarray], Dict[str, np.ndarray], Dict[str, np.ndarray]]:
+        inputs = {}
+        rows = None
+        if self.shuffle:
+            rows = self._shuffle_index[start_index:end_index]
+
+        for k, input_seq in self.inputs.items():
+            if self.shuffle:
+                inputs[k] = input_seq.get_by_idx_set(rows)
+            else:
+                inputs[k] = input_seq[start_index:end_index]
+        targets = {}
+        for k, target_seq in self.targets.items():
+            if self.shuffle:
+                targets[k] = target_seq.get_by_idx_set(rows)
+            else:
+                targets[k] = target_seq[start_index:end_index]
+
+        weights = {}
+        for k, weight_seq in self.weights.items():
+            if self.shuffle:
+                weights[k] = weight_seq.get_by_idx_set(rows)
+            else:
+                weights[k] = weight_seq[start_index:end_index]
+
+        return inputs, targets, weights
+
+    def get_config(self):
+        """Returns the configuration of the generator.
+        A generator's configuration is the keyword arguments
+        given to `__init__`.
+
+        # Returns
+            A dictionary.
+        """
+        return {
+            "inputs": json.dumps(self.inputs, cls=NumpyArrayEncoder),
+            "targets": json.dumps(self.targets, cls=NumpyArrayEncoder),
+            "weights": json.dumps(self.weights, cls=NumpyArrayEncoder),
+            "sampling_rate": self.sampling_rate,
+            "shuffle": self.shuffle,
+            "batch_size": self.batch_size,
+        }
+
+    def __add__(self, other: "XYWBatchGenerator") -> "XYWBatchGenerator":
+        inputs = {k: v + other.inputs[k] for k, v in self.inputs.items()}
+        targets = {k: v + other.targets[k] for k, v in self.targets.items()}
+        weights = {k: v + other.weight_map[k] for k, v in self.weights.items()}
+        return self.__class__(
+            inputs_map=inputs,
+            targets_map=targets,
+            weight_map=weights,
+            shuffle=self.shuffle,
+            batch_size=self.batch_size,
+        )
```

## Comparing `keras_generators-1.3.0.dist-info/LICENSE` & `keras_generators-1.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `keras_generators-1.3.0.dist-info/METADATA` & `keras_generators-1.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-generators
-Version: 1.3.0
+Version: 1.3.1
 Summary: Multi-dimensional/Multi-input/Multi-output Data preprocessing and Batch Generators for Keras models
 Home-page: https://github.com/asuiu/keras-generators
 Author: Andrei Suiu
 Author-email: andrei.suiu@gmail.com
 License: Apache License 2.0
 Keywords: ML,DataGenerators,Keras,tensorflow
 Classifier: Intended Audience :: Developers
```

