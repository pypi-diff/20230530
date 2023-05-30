# Comparing `tmp/habana_lightning_plugins-1.10.0.494-py3-none-any.whl.zip` & `tmp/habana_lightning_plugins-1.9.0.580.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 18581 bytes, number of entries: 12
--rw-r--r--  2.0 unx      601 b- defN 23-May-24 04:06 habana_lightning_plugins/__init__.py
--rw-r--r--  2.0 unx     6983 b- defN 23-May-24 04:06 habana_lightning_plugins/datamodule.py
--rw-r--r--  2.0 unx     6702 b- defN 23-May-24 04:06 habana_lightning_plugins/profiler.py
--rw-r--r--  2.0 unx     1502 b- defN 23-May-24 04:06 habana_lightning_plugins/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-24 04:06 habana_lightning_plugins/dataloaders/__init__.py
--rw-r--r--  2.0 unx     9701 b- defN 23-May-24 04:06 habana_lightning_plugins/dataloaders/resnet_media_pipe.py
--rw-r--r--  2.0 unx     1219 b- defN 23-May-24 04:06 habana_lightning_plugins/fabric/__init__.py
--rw-rw-r--  2.0 unx    11367 b- defN 23-May-24 04:07 habana_lightning_plugins-1.10.0.494.dist-info/LICENSE
--rw-r--r--  2.0 unx     8778 b- defN 23-May-24 04:07 habana_lightning_plugins-1.10.0.494.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 04:07 habana_lightning_plugins-1.10.0.494.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-May-24 04:07 habana_lightning_plugins-1.10.0.494.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1183 b- defN 23-May-24 04:07 habana_lightning_plugins-1.10.0.494.dist-info/RECORD
-12 files, 48153 bytes uncompressed, 16527 bytes compressed:  65.7%
+Zip file size: 17288 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-26 10:16 habana_lightning_plugins/__init__.py
+-rw-r--r--  2.0 unx     6983 b- defN 23-Mar-26 10:16 habana_lightning_plugins/datamodule.py
+-rw-r--r--  2.0 unx     6702 b- defN 23-Mar-26 10:16 habana_lightning_plugins/profiler.py
+-rw-r--r--  2.0 unx     1502 b- defN 23-Mar-26 10:16 habana_lightning_plugins/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-26 10:16 habana_lightning_plugins/dataloaders/__init__.py
+-rw-r--r--  2.0 unx     9701 b- defN 23-Mar-26 10:16 habana_lightning_plugins/dataloaders/resnet_media_pipe.py
+-rw-rw-r--  2.0 unx    11367 b- defN 23-Mar-26 10:16 habana_lightning_plugins-1.9.0.580.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8310 b- defN 23-Mar-26 10:16 habana_lightning_plugins-1.9.0.580.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-26 10:16 habana_lightning_plugins-1.9.0.580.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 23-Mar-26 10:16 habana_lightning_plugins-1.9.0.580.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1086 b- defN 23-Mar-26 10:16 habana_lightning_plugins-1.9.0.580.1.dist-info/RECORD
+11 files, 45768 bytes uncompressed, 15386 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -12,26 +12,23 @@
 
 Filename: habana_lightning_plugins/dataloaders/__init__.py
 Comment: 
 
 Filename: habana_lightning_plugins/dataloaders/resnet_media_pipe.py
 Comment: 
 
-Filename: habana_lightning_plugins/fabric/__init__.py
+Filename: habana_lightning_plugins-1.9.0.580.1.dist-info/LICENSE
 Comment: 
 
-Filename: habana_lightning_plugins-1.10.0.494.dist-info/LICENSE
+Filename: habana_lightning_plugins-1.9.0.580.1.dist-info/METADATA
 Comment: 
 
-Filename: habana_lightning_plugins-1.10.0.494.dist-info/METADATA
+Filename: habana_lightning_plugins-1.9.0.580.1.dist-info/WHEEL
 Comment: 
 
-Filename: habana_lightning_plugins-1.10.0.494.dist-info/WHEEL
+Filename: habana_lightning_plugins-1.9.0.580.1.dist-info/top_level.txt
 Comment: 
 
-Filename: habana_lightning_plugins-1.10.0.494.dist-info/top_level.txt
-Comment: 
-
-Filename: habana_lightning_plugins-1.10.0.494.dist-info/RECORD
+Filename: habana_lightning_plugins-1.9.0.580.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## habana_lightning_plugins/__init__.py

```diff
@@ -1,38 +0,0 @@
-00000000: 2320 436f 7079 7269 6768 7420 2863 2920  # Copyright (c) 
-00000010: 3230 3233 2048 6162 616e 6120 4c61 6273  2023 Habana Labs
-00000020: 2c20 4c74 642e 2061 6e20 496e 7465 6c20  , Ltd. an Intel 
-00000030: 436f 6d70 616e 790a 230a 2320 4c69 6365  Company.#.# Lice
-00000040: 6e73 6564 2075 6e64 6572 2074 6865 2041  nsed under the A
-00000050: 7061 6368 6520 4c69 6365 6e73 652c 2056  pache License, V
-00000060: 6572 7369 6f6e 2032 2e30 2028 7468 6520  ersion 2.0 (the 
-00000070: 224c 6963 656e 7365 2229 3b0a 2320 796f  "License");.# yo
-00000080: 7520 6d61 7920 6e6f 7420 7573 6520 7468  u may not use th
-00000090: 6973 2066 696c 6520 6578 6365 7074 2069  is file except i
-000000a0: 6e20 636f 6d70 6c69 616e 6365 2077 6974  n compliance wit
-000000b0: 6820 7468 6520 4c69 6365 6e73 652e 0a23  h the License..#
-000000c0: 2059 6f75 206d 6179 206f 6274 6169 6e20   You may obtain 
-000000d0: 6120 636f 7079 206f 6620 7468 6520 4c69  a copy of the Li
-000000e0: 6365 6e73 6520 6174 0a23 0a23 2020 2020  cense at.#.#    
-000000f0: 2068 7474 703a 2f2f 7777 772e 6170 6163   http://www.apac
-00000100: 6865 2e6f 7267 2f6c 6963 656e 7365 732f  he.org/licenses/
-00000110: 4c49 4345 4e53 452d 322e 300a 230a 2320  LICENSE-2.0.#.# 
-00000120: 556e 6c65 7373 2072 6571 7569 7265 6420  Unless required 
-00000130: 6279 2061 7070 6c69 6361 626c 6520 6c61  by applicable la
-00000140: 7720 6f72 2061 6772 6565 6420 746f 2069  w or agreed to i
-00000150: 6e20 7772 6974 696e 672c 2073 6f66 7477  n writing, softw
-00000160: 6172 650a 2320 6469 7374 7269 6275 7465  are.# distribute
-00000170: 6420 756e 6465 7220 7468 6520 4c69 6365  d under the Lice
-00000180: 6e73 6520 6973 2064 6973 7472 6962 7574  nse is distribut
-00000190: 6564 206f 6e20 616e 2022 4153 2049 5322  ed on an "AS IS"
-000001a0: 2042 4153 4953 2c0a 2320 5749 5448 4f55   BASIS,.# WITHOU
-000001b0: 5420 5741 5252 414e 5449 4553 204f 5220  T WARRANTIES OR 
-000001c0: 434f 4e44 4954 494f 4e53 204f 4620 414e  CONDITIONS OF AN
-000001d0: 5920 4b49 4e44 2c20 6569 7468 6572 2065  Y KIND, either e
-000001e0: 7870 7265 7373 206f 7220 696d 706c 6965  xpress or implie
-000001f0: 642e 0a23 2053 6565 2074 6865 204c 6963  d..# See the Lic
-00000200: 656e 7365 2066 6f72 2074 6865 2073 7065  ense for the spe
-00000210: 6369 6669 6320 6c61 6e67 7561 6765 2067  cific language g
-00000220: 6f76 6572 6e69 6e67 2070 6572 6d69 7373  overning permiss
-00000230: 696f 6e73 2061 6e64 0a23 206c 696d 6974  ions and.# limit
-00000240: 6174 696f 6e73 2075 6e64 6572 2074 6865  ations under the
-00000250: 204c 6963 656e 7365 2e                    License.
```

## Comparing `habana_lightning_plugins-1.10.0.494.dist-info/LICENSE` & `habana_lightning_plugins-1.9.0.580.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `habana_lightning_plugins-1.10.0.494.dist-info/METADATA` & `habana_lightning_plugins-1.9.0.580.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habana-lightning-plugins
-Version: 1.10.0.494
+Version: 1.9.0.580.1
 Summary: Habana's lightning-specific optimized plugins
 Home-page: https://habana.ai/
 Author: Habana Labs Ltd., an Intel Company
 Author-email: support@habana.ai
 License: See LICENSE file
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -127,14 +127,15 @@
 
 ## HPUProfiler
 
 HPUProfiler is a lightning implementation of PyTorch profiler for HPU devices. It aids in obtaining profiling summary of PyTorch functions. 
 It subclasses PyTorch Lightning's [PyTorch profiler](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.profilers.PyTorchProfiler.html#pytorch_lightning.profilers.PyTorchProfiler).
 
 
+
 ### Default Profiling
 For auto profiling, create a HPUProfiler instance and pass it to trainer.
 At the end of ``profiler.fit()``, it will generate a json trace for the run.
 In case ``accelerator = "hpu"`` is not used with HPUProfiler, then it will dump only CPU traces, similar to PyTorchProfiler.
 
 ``` python
 # Import profiler
@@ -192,59 +193,45 @@
 profiler = HPUProfiler()
 model = MyModel(profiler)
 trainer = Trainer(profiler=profiler, accelerator="hpu")
 ```
 For more details on profiler, refer to [PyTorchProfiler](https://pytorch-lightning.readthedocs.io/en/stable/tuning/profiler_intermediate.html)
 
 ### Visualize Profiled Operations
-Profiler will dump traces in json format. The traces can be visualized in 2 ways:
+Profiler will dump traces in json format. The traces can be
+visualized in 2 ways:
 
 #### Using PyTorch TensorBoard Profiler 
 
 For further instructions see, https://github.com/pytorch/kineto/tree/master/tb_plugin.
 
 ``` python
-# Install tensorboard
+# Install tensorbaord
 python -um pip install tensorboard torch-tb-profiler
 
 # Start the TensorBoard server (default at port 6006):
 tensorboard --logdir ./tensorboard --port 6006
 
 # Now open the following url on your browser
 http://localhost:6006/#profile
 ```
 
 #### Using Chrome
 
     1. Open Chrome and copy/paste this URL: `chrome://tracing/`.
     2. Once tracing opens, click on `Load` at the top-right and load one of the generated traces.
 
-
 ### Limitations
 
-- When using the HPUProfiler, wall clock time will not be representative of the true wall clock time. This is due to forcing profiled operations to be measured synchronously, when many HPU ops happen asynchronously.
-  It is recommended to use this Profiler to find bottlenecks/breakdowns, however for end to end wall clock time use the SimpleProfiler.
+- When using the HPUProfiler, wall clock time will not be representative of the true wall clock time. This is due to forcing profiled operations to be measured synchronously, when many HPU ops happen asynchronously. It is recommended to use this Profiler to find bottlenecks/breakdowns, however for end to end wall clock time use the SimpleProfiler.
 
 - HPUProfiler.summary() is not supported
 
 - Passing profiler name as string "hpu" to the trainer is not supported.
 
-
-## Supported Configurations
-
-| Validated on | SynapseAI Version | PyTorch Version | PyTorch Lightning Version |
-|--------------|-------------------|-----------------|---------------------------|
-| Gaudi        | 1.9.0             | 1.13.1          | 1.9.4                     |
-| Gaudi2       | 1.9.0             | 1.13.1          | 1.9.4                     |
-
-
-## Changelog
- - habana-lightning-plugins introduced with support for datamodule and profiler plugins
-
-
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

## Comparing `habana_lightning_plugins-1.10.0.494.dist-info/RECORD` & `habana_lightning_plugins-1.9.0.580.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-habana_lightning_plugins/__init__.py,sha256=F8WDaGwcg3_aq8d8udoqdwf2UnOg95HR2pHY4T_ulu0,601
+habana_lightning_plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 habana_lightning_plugins/datamodule.py,sha256=3LoC8VQ6a8EY04Eiz4utqkyTafcYJQPBHfYrJqCBjXA,6983
 habana_lightning_plugins/profiler.py,sha256=O4F7k14QUoUosXious_za3Cf-Lo5ELoUk1_3lN22HtU,6702
 habana_lightning_plugins/utils.py,sha256=_Wh71r1lMVUr0AwT0kghXfXLqGoL8X6zLZD8uG4q-sg,1502
 habana_lightning_plugins/dataloaders/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 habana_lightning_plugins/dataloaders/resnet_media_pipe.py,sha256=lcIsktSY8Tno2pzhdRlQdy1iaAkIPcQZJpgiis6M8rM,9701
-habana_lightning_plugins/fabric/__init__.py,sha256=7HyrT1qBufkfF1fBcQxAhIAWsKii_ltBjdUvViPMPg8,1219
-habana_lightning_plugins-1.10.0.494.dist-info/LICENSE,sha256=7toR6zQhxMjsOe1FXgUKsMm2ty1eYOCWZq9shku47ss,11367
-habana_lightning_plugins-1.10.0.494.dist-info/METADATA,sha256=kEqGmI2qmD8pwhHI9qWrRfVxPllQ_stHQsKrB_A0pQE,8778
-habana_lightning_plugins-1.10.0.494.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-habana_lightning_plugins-1.10.0.494.dist-info/top_level.txt,sha256=c6Qbzd1byEn9mFao6JWzkPj1GkvgjyOyP88WOWl0E4s,25
-habana_lightning_plugins-1.10.0.494.dist-info/RECORD,,
+habana_lightning_plugins-1.9.0.580.1.dist-info/LICENSE,sha256=7toR6zQhxMjsOe1FXgUKsMm2ty1eYOCWZq9shku47ss,11367
+habana_lightning_plugins-1.9.0.580.1.dist-info/METADATA,sha256=CKtyAfldIP7bzeDY6ciLL7P6e1XJmDV629f7xH32OYQ,8310
+habana_lightning_plugins-1.9.0.580.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+habana_lightning_plugins-1.9.0.580.1.dist-info/top_level.txt,sha256=c6Qbzd1byEn9mFao6JWzkPj1GkvgjyOyP88WOWl0E4s,25
+habana_lightning_plugins-1.9.0.580.1.dist-info/RECORD,,
```

