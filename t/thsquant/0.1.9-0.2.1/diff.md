# Comparing `tmp/thsquant-0.1.9.tar.gz` & `tmp/thsquant-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thsquant-0.1.9.tar", last modified: Mon May 29 12:44:56 2023, max compression
+gzip compressed data, was "thsquant-0.2.1.tar", last modified: Tue May 30 03:10:49 2023, max compression
```

## Comparing `thsquant-0.1.9.tar` & `thsquant-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,35 @@
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 12:44:56.055817 thsquant-0.1.9/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-25 12:56:47.000000 thsquant-0.1.9/LICENSE.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-29 12:44:56.055817 thsquant-0.1.9/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       18 2023-05-29 12:07:48.000000 thsquant-0.1.9/README.md
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-29 12:44:56.055817 thsquant-0.1.9/setup.cfg
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     1008 2023-05-29 12:44:38.000000 thsquant-0.1.9/setup.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 12:44:56.055817 thsquant-0.1.9/thsquant/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 09:25:35.000000 thsquant-0.1.9/thsquant/__init__.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       17 2023-05-29 12:43:02.000000 thsquant-0.1.9/thsquant/config.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      366 2023-05-29 12:43:55.000000 thsquant-0.1.9/thsquant/quant.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 12:44:56.055817 thsquant-0.1.9/thsquant.egg-info/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-29 12:44:55.000000 thsquant-0.1.9/thsquant.egg-info/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      251 2023-05-29 12:44:56.000000 thsquant-0.1.9/thsquant.egg-info/SOURCES.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 12:44:55.000000 thsquant-0.1.9/thsquant.egg-info/dependency_links.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       59 2023-05-29 12:44:55.000000 thsquant-0.1.9/thsquant.egg-info/entry_points.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        9 2023-05-29 12:44:55.000000 thsquant-0.1.9/thsquant.egg-info/top_level.txt
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-30 03:10:49.459635 thsquant-0.2.1/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-30 02:01:43.000000 thsquant-0.2.1/LICENSE.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-30 03:10:49.459635 thsquant-0.2.1/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       18 2023-05-30 02:01:43.000000 thsquant-0.2.1/README.md
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-30 03:10:49.459635 thsquant-0.2.1/setup.cfg
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     1341 2023-05-30 03:10:45.000000 thsquant-0.2.1/setup.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-30 03:10:49.459635 thsquant-0.2.1/thsquant/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        0 2023-05-30 02:01:43.000000 thsquant-0.2.1/thsquant/__init__.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     1112 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/convert_llama_weights_to_hf.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     7695 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/gptq.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    19618 2023-05-30 02:11:50.000000 thsquant-0.2.1/thsquant/llama.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     4629 2023-05-30 02:27:44.000000 thsquant-0.2.1/thsquant/llama_inference.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    13161 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/llama_inference_offload.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    15967 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/neox.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    17497 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/opt.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-30 03:10:49.459635 thsquant-0.2.1/thsquant/quant/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      317 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/quant/__init__.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     8775 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/quant/custom_autotune.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     8799 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/quant/fused_attn.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    12139 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/quant/fused_mlp.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    18730 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/quant/quant_linear.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     4263 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/quant/quantizer.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     3120 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/quant/triton_norm.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-30 03:10:49.459635 thsquant-0.2.1/thsquant/utils/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      215 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/utils/__init__.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     6712 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/utils/datautils.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     1019 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/utils/export.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     2563 2023-05-30 02:02:36.000000 thsquant-0.2.1/thsquant/utils/modelutils.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-30 03:10:49.459635 thsquant-0.2.1/thsquant.egg-info/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-30 03:10:49.000000 thsquant-0.2.1/thsquant.egg-info/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      733 2023-05-30 03:10:49.000000 thsquant-0.2.1/thsquant.egg-info/SOURCES.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       69 2023-05-30 03:10:49.000000 thsquant-0.2.1/thsquant.egg-info/dependency_links.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       62 2023-05-30 03:10:49.000000 thsquant-0.2.1/thsquant.egg-info/entry_points.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      121 2023-05-30 03:10:49.000000 thsquant-0.2.1/thsquant.egg-info/requires.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        9 2023-05-30 03:10:49.000000 thsquant-0.2.1/thsquant.egg-info/top_level.txt
```

### Comparing `thsquant-0.1.9/LICENSE.txt` & `thsquant-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thsquant-0.1.9/PKG-INFO` & `thsquant-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.1.9
+Version: 0.2.1
 Summary: A short description of your awesome package
 Home-page: https://github.com/qinbo23/ths-quant
 Author: qinbo
 Author-email: qinbo@myhexin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `thsquant-0.1.9/thsquant.egg-info/PKG-INFO` & `thsquant-0.2.1/thsquant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.1.9
+Version: 0.2.1
 Summary: A short description of your awesome package
 Home-page: https://github.com/qinbo23/ths-quant
 Author: qinbo
 Author-email: qinbo@myhexin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

