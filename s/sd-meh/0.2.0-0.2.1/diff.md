# Comparing `tmp/sd_meh-0.2.0.tar.gz` & `tmp/sd_meh-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.2.0.tar", max compression
+gzip compressed data, was "sd_meh-0.2.1.tar", max compression
```

## Comparing `sd_meh-0.2.0.tar` & `sd_meh-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-05-10 14:42:40.197057 sd_meh-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1359 2023-05-12 08:39:24.814256 sd_meh-0.2.0/README.md
--rw-r--r--   0        0        0      390 2023-05-17 11:14:54.463646 sd_meh-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-17 11:14:54.463955 sd_meh-0.2.0/sd_meh/__init__.py
--rw-r--r--   0        0        0     6236 2023-05-17 11:14:54.464545 sd_meh-0.2.0/sd_meh/merge.py
--rw-r--r--   0        0        0     1465 2023-05-10 13:19:22.948414 sd_meh-0.2.0/sd_meh/model.py
--rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 sd_meh-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-10 14:42:40.197057 sd_meh-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     1400 2023-05-30 08:54:57.646230 sd_meh-0.2.1/README.md
+-rw-r--r--   0        0        0      390 2023-05-30 08:55:01.914476 sd_meh-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-30 08:55:01.915024 sd_meh-0.2.1/sd_meh/__init__.py
+-rw-r--r--   0        0        0     5217 2023-05-30 08:55:01.915417 sd_meh-0.2.1/sd_meh/merge.py
+-rw-r--r--   0        0        0     1571 2023-05-30 08:55:01.915678 sd_meh-0.2.1/sd_meh/merge_methods.py
+-rw-r--r--   0        0        0     1465 2023-05-10 13:19:22.948414 sd_meh-0.2.1/sd_meh/model.py
+-rw-r--r--   0        0        0     1924 1970-01-01 00:00:00.000000 sd_meh-0.2.1/PKG-INFO
```

### Comparing `sd_meh-0.2.0/LICENSE.txt` & `sd_meh-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.2.0/README.md` & `sd_meh-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,23 +27,25 @@
 Usage: merge_models.py [OPTIONS]
 
 Options:
   -a, --model_a TEXT
   -b, --model_b TEXT
   -c, --model_c TEXT
   -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum]
+  -wc, --weights_clip
   -p, --precision INTEGER
   -o, --output_path TEXT
   -f, --output_format [safetensors|ckpt]
   -wa, --weights_alpha TEXT
   -ba, --base_alpha FLOAT
   -wb, --weights_beta TEXT
   -bb, --base_beta FLOAT
   --help                          Show this message and exit.
 ```
 
 ## Features
 
+- weights clipping
 - registered pypi package
 - block merge
 - merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`
 - `fp16` and `fp32`
```

### Comparing `sd_meh-0.2.0/sd_meh/merge.py` & `sd_meh-0.2.1/sd_meh/merge.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from typing import Dict, Tuple, Optional
 
 import safetensors.torch
 import torch
 from tqdm import tqdm
 
 from sd_meh.model import SDModel
+from sd_meh import merge_methods
 
 MAX_TOKENS = 77
 NUM_INPUT_BLOCKS = 12
 NUM_MID_BLOCK = 1
 NUM_OUTPUT_BLOCKS = 12
 NUM_TOTAL_BLOCKS = NUM_INPUT_BLOCKS + NUM_MID_BLOCK + NUM_OUTPUT_BLOCKS
-EPSILON = 1e-10  # Define a small constant EPSILON to prevent division by zero
 
 KEY_POSITION_IDS = ".".join(
     [
         "cond_stage_model",
         "transformer",
         "text_model",
         "embeddings",
@@ -138,61 +138,43 @@
 
             if weight_index >= NUM_TOTAL_BLOCKS:
                 raise ValueError(f"illegal block index {key}")
 
             if weight_index >= 0:
                 current_bases = {k: w[weight_index] for k, w in weights.items()}
 
-        merged_key = merge(current_bases, thetas, key, merge_mode)
+        merge_method = getattr(merge_methods, merge_mode)
+        merge_args = get_merge_method_args(current_bases, thetas, key)
+        merged_key = merge_method(**merge_args)
 
         if weights_clip:
             t0 = thetas["model_a"][key]
             t1 = thetas["model_b"][key]
             threshold = torch.maximum(torch.abs(t0), torch.abs(t1))
             merged_key = torch.minimum(torch.maximum(merged_key, -threshold), threshold)
 
         if precision == 16:
             merged_key = merged_key.half()
 
         return key, merged_key
 
 
-def merge(current_bases: Dict, thetas: Dict, key: str, merge_mode: str) -> torch.Tensor:
-    t0 = thetas["model_a"][key]
-    t1 = thetas["model_b"][key]
-    alpha = current_bases["alpha"]
-    if merge_mode == "weighted_sum":
-        return (1 - alpha) * t0 + alpha * t1
-    elif merge_mode == "weighted_subtraction":
-        beta = current_bases["beta"]
-        # Adjust beta if both alpha and beta are 1.0 to avoid division by zero
-        if alpha == 1.0 and beta == 1.0:
-            beta -= EPSILON
-        return (t0 - alpha * beta * t1) / (1 - alpha * beta)
-    elif merge_mode == "tensor_sum":
-        beta = current_bases["beta"]
-        if alpha + beta <= 1:
-            tt = t0.clone()
-            talphas = int(t0.shape[0] * (beta))
-            talphae = int(t0.shape[0] * (alpha + beta))
-            tt[talphas:talphae] = t1[talphas:talphae].clone()
-        else:
-            talphas = int(t0.shape[0] * (alpha + beta - 1))
-            talphae = int(t0.shape[0] * (beta))
-            tt = t1.clone()
-            tt[talphas:talphae] = t0[talphas:talphae].clone()
-        return tt
-    t2 = thetas["model_c"][key]
-    if merge_mode == "add_difference":
-        return t0 + alpha * (t1 - t2)
-    beta = current_bases["beta"]
-    if merge_mode == "sum_twice":
-        return (1 - beta) * ((1 - alpha) * t0 + alpha * t1) + beta * t2
-    elif merge_mode == "triple_sum":
-        return (1 - alpha - beta) * t0 + alpha * t1 + beta * t2
+def get_merge_method_args(current_bases: Dict, thetas: Dict, key: str) -> Dict:
+    merge_method_args = {
+        "a": thetas["model_a"][key],
+        "b": thetas["model_b"][key],
+        **current_bases,
+    }
+
+    if "model_c" in thetas:
+        merge_method_args.update({
+            "c": thetas["model_c"][key],
+        })
+
+    return merge_method_args
 
 
 def save_model(model, output_file, file_format) -> None:
     if file_format == "safetensors":
         safetensors.torch.save_file(
             model, f"{output_file}.safetensors", metadata={"format": "pt"}
         )
```

### Comparing `sd_meh-0.2.0/sd_meh/model.py` & `sd_meh-0.2.1/sd_meh/model.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.2.0/PKG-INFO` & `sd_meh-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-meh
-Version: 0.2.0
+Version: 0.2.1
 Summary: stable diffusion merging execution helper
 Home-page: https://github.com/s1dlx/meh
 License: MIT
 Author: s1dlx
 Author-email: s1dlx@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -43,24 +43,26 @@
 Usage: merge_models.py [OPTIONS]
 
 Options:
   -a, --model_a TEXT
   -b, --model_b TEXT
   -c, --model_c TEXT
   -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum]
+  -wc, --weights_clip
   -p, --precision INTEGER
   -o, --output_path TEXT
   -f, --output_format [safetensors|ckpt]
   -wa, --weights_alpha TEXT
   -ba, --base_alpha FLOAT
   -wb, --weights_beta TEXT
   -bb, --base_beta FLOAT
   --help                          Show this message and exit.
 ```
 
 ## Features
 
+- weights clipping
 - registered pypi package
 - block merge
 - merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`
 - `fp16` and `fp32`
```

