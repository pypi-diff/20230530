# Comparing `tmp/vector_quantize_pytorch-1.6.6.tar.gz` & `tmp/vector_quantize_pytorch-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.6.6.tar", last modified: Mon May 29 16:34:57 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.6.7.tar", last modified: Tue May 30 19:54:17 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.6.6.tar` & `vector_quantize_pytorch-1.6.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:34:57.425223 vector_quantize_pytorch-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-29 16:34:57.425223 vector_quantize_pytorch-1.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:34:57.425223 vector_quantize_pytorch-1.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:34:57.425223 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    30182 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:34:57.425223 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-29 16:34:57.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-29 16:34:57.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:34:57.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-29 16:34:57.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 16:34:57.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:54:17.210549 vector_quantize_pytorch-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-30 19:54:17.210549 vector_quantize_pytorch-1.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:54:17.210549 vector_quantize_pytorch-1.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:54:17.206549 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30174 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:54:17.210549 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-30 19:54:17.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-30 19:54:17.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:54:17.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 19:54:17.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 19:54:17.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.6.6/LICENSE` & `vector_quantize_pytorch-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.6/PKG-INFO` & `vector_quantize_pytorch-1.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.6.6
+Version: 1.6.7
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.6.6/README.md` & `vector_quantize_pytorch-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.6/setup.py` & `vector_quantize_pytorch-1.6.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.6.6',
+  version = '1.6.7',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
         flatten, ps = pack_one(x, 'h * d')
 
         self.init_embed_(flatten)
 
         if self.affine_param:
             self.update_affine(flatten, self.embed)
 
-        embed = self.embed if not self.learnable_codebook else self.embed.detach()
+        embed = self.embed if self.learnable_codebook else self.embed.detach()
 
         if self.affine_param:
             codebook_std = self.codebook_variance.clamp(min = 1e-5).sqrt()
             batch_std = self.batch_variance.clamp(min = 1e-5).sqrt()
             embed = (embed - self.codebook_mean) * (batch_std / codebook_std) + self.batch_mean
 
         dist = -torch.cdist(flatten, embed, p = 2)
@@ -568,15 +568,15 @@
 
         dtype = x.dtype
 
         flatten, ps = pack_one(x, 'h * d')
 
         self.init_embed_(flatten)
 
-        embed = self.embed if not self.learnable_codebook else self.embed.detach()
+        embed = self.embed if self.learnable_codebook else self.embed.detach()
 
         dist = einsum('h n d, h c d -> h n c', flatten, embed)
 
         embed_ind, embed_onehot, straight_through_mult = self.gumbel_sample(dist, dim = -1, temperature = sample_codebook_temp, training = self.training)
         embed_ind = unpack_one(embed_ind, ps, 'h *')
 
         quantize = batched_embedding(embed_ind, self.embed)
```

### Comparing `vector_quantize_pytorch-1.6.6/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.6.6
+Version: 1.6.7
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

