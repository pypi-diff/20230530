# Comparing `tmp/sd_meh-0.2.1.tar.gz` & `tmp/sd_meh-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.2.1.tar", max compression
+gzip compressed data, was "sd_meh-0.2.2.tar", max compression
```

## Comparing `sd_meh-0.2.1.tar` & `sd_meh-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-05-10 14:42:40.197057 sd_meh-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     1400 2023-05-30 08:54:57.646230 sd_meh-0.2.1/README.md
--rw-r--r--   0        0        0      390 2023-05-30 08:55:01.914476 sd_meh-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-30 08:55:01.915024 sd_meh-0.2.1/sd_meh/__init__.py
--rw-r--r--   0        0        0     5217 2023-05-30 08:55:01.915417 sd_meh-0.2.1/sd_meh/merge.py
--rw-r--r--   0        0        0     1571 2023-05-30 08:55:01.915678 sd_meh-0.2.1/sd_meh/merge_methods.py
--rw-r--r--   0        0        0     1465 2023-05-10 13:19:22.948414 sd_meh-0.2.1/sd_meh/model.py
--rw-r--r--   0        0        0     1924 1970-01-01 00:00:00.000000 sd_meh-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-30 11:34:33.627424 sd_meh-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     1400 2023-05-30 11:34:33.627424 sd_meh-0.2.2/README.md
+-rw-r--r--   0        0        0      390 2023-05-30 11:34:33.627424 sd_meh-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-30 11:34:33.627424 sd_meh-0.2.2/sd_meh/__init__.py
+-rw-r--r--   0        0        0     5399 2023-05-30 11:34:33.627424 sd_meh-0.2.2/sd_meh/merge.py
+-rw-r--r--   0        0        0     1588 2023-05-30 11:34:33.627424 sd_meh-0.2.2/sd_meh/merge_methods.py
+-rw-r--r--   0        0        0     1465 2023-05-30 11:34:33.627424 sd_meh-0.2.2/sd_meh/model.py
+-rw-r--r--   0        0        0     1924 1970-01-01 00:00:00.000000 sd_meh-0.2.2/PKG-INFO
```

### Comparing `sd_meh-0.2.1/LICENSE.txt` & `sd_meh-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.2.1/README.md` & `sd_meh-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sd_meh-0.2.1/sd_meh/merge.py` & `sd_meh-0.2.2/sd_meh/merge.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 import re
+import sys
 from pathlib import Path
-from typing import Dict, Tuple, Optional
+from typing import Dict, Optional, Tuple
 
 import safetensors.torch
 import torch
 from tqdm import tqdm
 
-from sd_meh.model import SDModel
 from sd_meh import merge_methods
+from sd_meh.model import SDModel
 
 MAX_TOKENS = 77
 NUM_INPUT_BLOCKS = 12
 NUM_MID_BLOCK = 1
 NUM_OUTPUT_BLOCKS = 12
 NUM_TOTAL_BLOCKS = NUM_INPUT_BLOCKS + NUM_MID_BLOCK + NUM_OUTPUT_BLOCKS
 
@@ -138,15 +139,20 @@
 
             if weight_index >= NUM_TOTAL_BLOCKS:
                 raise ValueError(f"illegal block index {key}")
 
             if weight_index >= 0:
                 current_bases = {k: w[weight_index] for k, w in weights.items()}
 
-        merge_method = getattr(merge_methods, merge_mode)
+        try:
+            merge_method = getattr(merge_methods, merge_mode)
+        except AttributeError:
+            print(f"{merge_mode} not implemented, aborting merge!")
+            sys.exit(1)
+
         merge_args = get_merge_method_args(current_bases, thetas, key)
         merged_key = merge_method(**merge_args)
 
         if weights_clip:
             t0 = thetas["model_a"][key]
             t1 = thetas["model_b"][key]
             threshold = torch.maximum(torch.abs(t0), torch.abs(t1))
@@ -162,17 +168,19 @@
     merge_method_args = {
         "a": thetas["model_a"][key],
         "b": thetas["model_b"][key],
         **current_bases,
     }
 
     if "model_c" in thetas:
-        merge_method_args.update({
-            "c": thetas["model_c"][key],
-        })
+        merge_method_args.update(
+            {
+                "c": thetas["model_c"][key],
+            }
+        )
 
     return merge_method_args
 
 
 def save_model(model, output_file, file_format) -> None:
     if file_format == "safetensors":
         safetensors.torch.save_file(
```

### Comparing `sd_meh-0.2.1/sd_meh/merge_methods.py` & `sd_meh-0.2.2/sd_meh/merge_methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from torch import Tensor
 
-
 __all__ = [
     "weighted_sum",
     "weighted_subtraction",
     "tensor_sum",
     "add_difference",
     "sum_twice",
     "triple_sum",
@@ -14,15 +13,17 @@
 EPSILON = 1e-10  # Define a small constant EPSILON to prevent division by zero
 
 
 def weighted_sum(a: Tensor, b: Tensor, alpha: float, **kwargs) -> Tensor:
     return (1 - alpha) * a + alpha * b
 
 
-def weighted_subtraction(a: Tensor, b: Tensor, alpha: float, beta: float, **kwargs) -> Tensor:
+def weighted_subtraction(
+    a: Tensor, b: Tensor, alpha: float, beta: float, **kwargs
+) -> Tensor:
     # Adjust beta if both alpha and beta are 1.0 to avoid division by zero
     if alpha == 1.0 and beta == 1.0:
         beta -= EPSILON
 
     return (a - alpha * beta * b) / (1 - alpha * beta)
 
 
@@ -40,13 +41,17 @@
     return tt
 
 
 def add_difference(a: Tensor, b: Tensor, c: Tensor, alpha: float, **kwargs) -> Tensor:
     return a + alpha * (b - c)
 
 
-def sum_twice(a: Tensor, b: Tensor, c: Tensor, alpha: float, beta: float, **kwargs) -> Tensor:
+def sum_twice(
+    a: Tensor, b: Tensor, c: Tensor, alpha: float, beta: float, **kwargs
+) -> Tensor:
     return (1 - beta) * ((1 - alpha) * a + alpha * b) + beta * c
 
 
-def triple_sum(a: Tensor, b: Tensor, c: Tensor, alpha: float, beta: float, **kwargs) -> Tensor:
+def triple_sum(
+    a: Tensor, b: Tensor, c: Tensor, alpha: float, beta: float, **kwargs
+) -> Tensor:
     return (1 - alpha - beta) * a + alpha * b + beta * c
```

### Comparing `sd_meh-0.2.1/sd_meh/model.py` & `sd_meh-0.2.2/sd_meh/model.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.2.1/PKG-INFO` & `sd_meh-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-meh
-Version: 0.2.1
+Version: 0.2.2
 Summary: stable diffusion merging execution helper
 Home-page: https://github.com/s1dlx/meh
 License: MIT
 Author: s1dlx
 Author-email: s1dlx@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

