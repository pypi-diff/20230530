# Comparing `tmp/audiolm-pytorch-1.0.6.tar.gz` & `tmp/audiolm-pytorch-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm-pytorch-1.0.6.tar", last modified: Thu May 25 01:46:47 2023, max compression
+gzip compressed data, was "audiolm-pytorch-1.1.0.tar", last modified: Tue May 30 01:15:11 2023, max compression
```

## Comparing `audiolm-pytorch-1.0.6.tar` & `audiolm-pytorch-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:46:47.122420 audiolm-pytorch-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 01:46:47.122420 audiolm-pytorch-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:46:47.122420 audiolm-pytorch-1.0.6/audiolm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65656 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/audiolm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/encodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/hubert_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30165 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/soundstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/audiolm_pytorch/vq_wav2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:46:47.122420 audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 01:46:47.000000 audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 01:46:47.000000 audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 01:46:47.000000 audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-25 01:46:47.000000 audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 01:46:47.000000 audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 01:46:47.122420 audiolm-pytorch-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-25 01:46:28.000000 audiolm-pytorch-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 01:15:11.709440 audiolm-pytorch-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-30 01:15:11.709440 audiolm-pytorch-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18271 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 01:15:11.709440 audiolm-pytorch-1.1.0/audiolm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/audiolm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65656 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/audiolm_pytorch/audiolm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/audiolm_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/audiolm_pytorch/encodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/audiolm_pytorch/hubert_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/audiolm_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/audiolm_pytorch/soundstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/audiolm_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/audiolm_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/audiolm_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/audiolm_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/audiolm_pytorch/vq_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 01:15:11.709440 audiolm-pytorch-1.1.0/audiolm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-30 01:15:11.000000 audiolm-pytorch-1.1.0/audiolm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-30 01:15:11.000000 audiolm-pytorch-1.1.0/audiolm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 01:15:11.000000 audiolm-pytorch-1.1.0/audiolm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-30 01:15:11.000000 audiolm-pytorch-1.1.0/audiolm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 01:15:11.000000 audiolm-pytorch-1.1.0/audiolm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 01:15:11.709440 audiolm-pytorch-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-30 01:14:58.000000 audiolm-pytorch-1.1.0/setup.py
```

### Comparing `audiolm-pytorch-1.0.6/LICENSE` & `audiolm-pytorch-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.6/PKG-INFO` & `audiolm-pytorch-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.0.6
+Version: 1.1.0
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.0.6/README.md` & `audiolm-pytorch-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
 - <a href="https://github.com/alexdemartos">Alejandro</a> and <a href="https://github.com/ilya16">Ilya</a> for sharing their results with training soundstream, and for working through a few issues with the local attention positional embeddings
 
 - <a href="https://github.com/LWprogramming">LWprogramming</a> for adding Encodec compatibility!
 
 - <a href="https://github.com/YoungloLee">@YoungloLee</a> for identifying a big bug in the 1d causal convolution for soundstream related to padding not accounting for strides!
 
+- <a href="https://github.com/haydenshively">Hayden</a> for pointing out some discrepancies in the multi-scale discriminator for Soundstream
+
 ## Install
 
 ```bash
 $ pip install audiolm-pytorch
 ```
 
 ## Usage
```

#### html2text {}

```diff
@@ -20,23 +20,24 @@
 submitting bug fixes! - Ilya for finding an issue with multi-scale
 discriminator downsampling and for soundstream trainer improvements - Andrey
 for identifying a missing loss in soundstream and guiding me through the proper
 mel spectrogram hyperparameters - Alejandro and Ilya for sharing their results
 with training soundstream, and for working through a few issues with the local
 attention positional embeddings - LWprogramming for adding Encodec
 compatibility! - @YoungloLee for identifying a big bug in the 1d causal
-convolution for soundstream related to padding not accounting for strides! ##
-Install ```bash $ pip install audiolm-pytorch ``` ## Usage ### SoundStream &
-Encodec There are two options for the neural codec. If you want to use the
-pretrained 24kHz Encodec, just create an Encodec object as follows: ```python
-from audiolm_pytorch import EncodecWrapper encodec = EncodecWrapper() # Now you
-can use the encodec variable in the same way you'd use the soundstream
-variables below. ``` Otherwise, to stay more true to the original paper, you
-can use `SoundStream`. First, `SoundStream` needs to be trained on a large
-corpus of audio data ```python from audiolm_pytorch import SoundStream,
+convolution for soundstream related to padding not accounting for strides! -
+Hayden for pointing out some discrepancies in the multi-scale discriminator for
+Soundstream ## Install ```bash $ pip install audiolm-pytorch ``` ## Usage ###
+SoundStream & Encodec There are two options for the neural codec. If you want
+to use the pretrained 24kHz Encodec, just create an Encodec object as follows:
+```python from audiolm_pytorch import EncodecWrapper encodec = EncodecWrapper()
+# Now you can use the encodec variable in the same way you'd use the
+soundstream variables below. ``` Otherwise, to stay more true to the original
+paper, you can use `SoundStream`. First, `SoundStream` needs to be trained on a
+large corpus of audio data ```python from audiolm_pytorch import SoundStream,
 SoundStreamTrainer soundstream = SoundStream( codebook_size = 1024,
 rq_num_quantizers = 8, rq_groups = 2, # this paper proposes using multi-headed
 residual vector quantization - https://arxiv.org/abs/2305.02765
 attn_window_size = 128, # local attention receptive field at bottleneck
 attn_depth = 2 # 2 local attention transformer blocks - the soundstream folks
 were not experts with attention, so i took the liberty to add some. encodec
 went with lstms, but attention should be better ) trainer = SoundStreamTrainer
```

### Comparing `audiolm-pytorch-1.0.6/audiolm_pytorch/__init__.py` & `audiolm-pytorch-1.1.0/audiolm_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.6/audiolm_pytorch/audiolm_pytorch.py` & `audiolm-pytorch-1.1.0/audiolm_pytorch/audiolm_pytorch.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.6/audiolm_pytorch/data.py` & `audiolm-pytorch-1.1.0/audiolm_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.6/audiolm_pytorch/encodec.py` & `audiolm-pytorch-1.1.0/audiolm_pytorch/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.6/audiolm_pytorch/hubert_kmeans.py` & `audiolm-pytorch-1.1.0/audiolm_pytorch/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.6/audiolm_pytorch/optimizer.py` & `audiolm-pytorch-1.1.0/audiolm_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.6/audiolm_pytorch/soundstream.py` & `audiolm-pytorch-1.1.0/audiolm_pytorch/soundstream.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,43 +84,46 @@
 # discriminators
 
 class MultiScaleDiscriminator(nn.Module):
     def __init__(
         self,
         channels = 16,
         layers = 4,
-        groups = 4,
+        groups = (4, 16, 64, 256),
         chan_max = 1024,
         input_channels = 1
     ):
         super().__init__()
-        self.init_conv = nn.Conv1d(input_channels, channels, 7)
+        self.init_conv = nn.Conv1d(input_channels, channels, 15, padding = 7)
         self.conv_layers = nn.ModuleList([])
 
         curr_channels = channels
 
-        for _ in range(layers):
+        for _, group in zip(range(layers), groups):
             chan_out = min(curr_channels * 4, chan_max)
 
             self.conv_layers.append(nn.Sequential(
-                nn.Conv1d(curr_channels, chan_out, 8, stride = 4, padding = 4, groups = groups),
+                nn.Conv1d(curr_channels, chan_out, 41, stride = 4, padding = 20, groups = group),
                 leaky_relu()
             ))
 
             curr_channels = chan_out
 
         self.final_conv = nn.Sequential(
-            nn.Conv1d(curr_channels, curr_channels, 3),
+            nn.Conv1d(curr_channels, curr_channels, 5, padding = 2),
             leaky_relu(),
-            nn.Conv1d(curr_channels, 1, 1),
+            nn.Conv1d(curr_channels, 1, 3, padding = 1),
         )
 
-    def forward(self, x, return_intermediates = False):
+    def forward(
+        self,
+        x,
+        return_intermediates = False
+    ):
         x = self.init_conv(x)
-
         intermediates = []
 
         for layer in self.conv_layers:
             x = layer(x)
             intermediates.append(x)
 
         out = self.final_conv(x)
```

### Comparing `audiolm-pytorch-1.0.6/audiolm_pytorch/t5.py` & `audiolm-pytorch-1.1.0/audiolm_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.6/audiolm_pytorch/trainer.py` & `audiolm-pytorch-1.1.0/audiolm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.6/audiolm_pytorch/vq_wav2vec.py` & `audiolm-pytorch-1.1.0/audiolm_pytorch/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/PKG-INFO` & `audiolm-pytorch-1.1.0/audiolm_pytorch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.0.6
+Version: 1.1.0
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.0.6/audiolm_pytorch.egg-info/SOURCES.txt` & `audiolm-pytorch-1.1.0/audiolm_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.6/setup.py` & `audiolm-pytorch-1.1.0/setup.py`

 * *Files identical despite different names*

