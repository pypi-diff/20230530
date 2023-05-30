# Comparing `tmp/mbapy-0.1.0.tar.gz` & `tmp/mbapy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbapy-0.1.0.tar", last modified: Mon May 22 09:51:42 2023, max compression
+gzip compressed data, was "mbapy-0.1.1.tar", last modified: Tue May 30 07:29:02 2023, max compression
```

## Comparing `mbapy-0.1.0.tar` & `mbapy-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-22 09:51:42.624638 mbapy-0.1.0/
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     1064 2023-05-20 15:53:20.000000 mbapy-0.1.0/LICENSE
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     6186 2023-05-22 09:51:42.624638 mbapy-0.1.0/PKG-INFO
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     5435 2023-05-22 08:19:05.000000 mbapy-0.1.0/README.md
-drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-22 09:51:42.624638 mbapy-0.1.0/mbapy/
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      559 2023-05-22 09:16:36.000000 mbapy-0.1.0/mbapy/__init__.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      387 2023-05-22 08:19:53.000000 mbapy-0.1.0/mbapy/__version__.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     3867 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/base.py
-drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-22 09:51:42.624638 mbapy-0.1.0/mbapy/dl_torch/
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      349 2023-05-22 09:18:31.000000 mbapy-0.1.0/mbapy/dl_torch/__init__.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)    21852 2023-05-22 09:19:55.000000 mbapy-0.1.0/mbapy/dl_torch/bb.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     4916 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/dl_torch/data.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     1015 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/dl_torch/hyper_search.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     4018 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/dl_torch/loss.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)    12806 2023-05-22 09:17:48.000000 mbapy-0.1.0/mbapy/dl_torch/m.py
-drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-22 09:51:42.624638 mbapy-0.1.0/mbapy/dl_torch/paper/
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)       17 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/dl_torch/paper/__init__.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     2873 2023-05-22 08:47:43.000000 mbapy-0.1.0/mbapy/dl_torch/paper/bb.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     9067 2023-05-22 09:48:08.000000 mbapy-0.1.0/mbapy/dl_torch/utils.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     2306 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/file.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)    14344 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/plot.py
-drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-22 09:51:42.624638 mbapy-0.1.0/mbapy/stats/
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      512 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/stats/__init__.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     3514 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/stats/df.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)    18970 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/stats/geography.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      727 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/stats/reg.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     9184 2023-05-22 07:21:40.000000 mbapy-0.1.0/mbapy/stats/test.py
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     8696 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/web.py
-drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-22 09:51:42.624638 mbapy-0.1.0/mbapy.egg-info/
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     6186 2023-05-22 09:51:42.000000 mbapy-0.1.0/mbapy.egg-info/PKG-INFO
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      599 2023-05-22 09:51:42.000000 mbapy-0.1.0/mbapy.egg-info/SOURCES.txt
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)        1 2023-05-22 09:51:42.000000 mbapy-0.1.0/mbapy.egg-info/dependency_links.txt
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      379 2023-05-22 09:51:42.000000 mbapy-0.1.0/mbapy.egg-info/requires.txt
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)       54 2023-05-22 09:51:42.000000 mbapy-0.1.0/mbapy.egg-info/top_level.txt
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)       38 2023-05-22 09:51:42.624638 mbapy-0.1.0/setup.cfg
--rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     2551 2023-05-22 08:22:08.000000 mbapy-0.1.0/setup.py
+drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-30 07:29:02.285475 mbapy-0.1.1/
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     1064 2023-05-20 15:53:20.000000 mbapy-0.1.1/LICENSE
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     6186 2023-05-30 07:29:02.285475 mbapy-0.1.1/PKG-INFO
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     5435 2023-05-22 08:19:05.000000 mbapy-0.1.1/README.md
+drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-30 07:29:02.285475 mbapy-0.1.1/mbapy/
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      559 2023-05-22 09:16:36.000000 mbapy-0.1.1/mbapy/__init__.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      387 2023-05-30 07:28:15.000000 mbapy-0.1.1/mbapy/__version__.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     4293 2023-05-29 15:28:04.000000 mbapy-0.1.1/mbapy/base.py
+drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-30 07:29:02.285475 mbapy-0.1.1/mbapy/dl_torch/
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      349 2023-05-22 09:18:31.000000 mbapy-0.1.1/mbapy/dl_torch/__init__.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)    22019 2023-05-30 01:57:23.000000 mbapy-0.1.1/mbapy/dl_torch/bb.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     4916 2023-05-20 15:53:20.000000 mbapy-0.1.1/mbapy/dl_torch/data.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     1015 2023-05-20 15:53:20.000000 mbapy-0.1.1/mbapy/dl_torch/hyper_search.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     4018 2023-05-20 15:53:20.000000 mbapy-0.1.1/mbapy/dl_torch/loss.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)    12806 2023-05-22 09:17:48.000000 mbapy-0.1.1/mbapy/dl_torch/m.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     3788 2023-05-30 01:58:26.000000 mbapy-0.1.1/mbapy/dl_torch/optim.py
+drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-30 07:29:02.285475 mbapy-0.1.1/mbapy/dl_torch/paper/
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)       17 2023-05-20 15:53:20.000000 mbapy-0.1.1/mbapy/dl_torch/paper/__init__.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     2873 2023-05-22 08:47:43.000000 mbapy-0.1.1/mbapy/dl_torch/paper/bb.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     9193 2023-05-27 10:12:49.000000 mbapy-0.1.1/mbapy/dl_torch/utils.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     2753 2023-05-27 15:44:50.000000 mbapy-0.1.1/mbapy/file.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)    14353 2023-05-30 01:14:32.000000 mbapy-0.1.1/mbapy/plot.py
+drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-30 07:29:02.285475 mbapy-0.1.1/mbapy/stats/
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      512 2023-05-20 15:53:20.000000 mbapy-0.1.1/mbapy/stats/__init__.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     3561 2023-05-30 02:00:31.000000 mbapy-0.1.1/mbapy/stats/df.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)    18970 2023-05-20 15:53:20.000000 mbapy-0.1.1/mbapy/stats/geography.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      727 2023-05-20 15:53:20.000000 mbapy-0.1.1/mbapy/stats/reg.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     9184 2023-05-22 07:21:40.000000 mbapy-0.1.1/mbapy/stats/test.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     8696 2023-05-20 15:53:20.000000 mbapy-0.1.1/mbapy/web.py
+drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-30 07:29:02.285475 mbapy-0.1.1/mbapy.egg-info/
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     6186 2023-05-30 07:29:02.000000 mbapy-0.1.1/mbapy.egg-info/PKG-INFO
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      623 2023-05-30 07:29:02.000000 mbapy-0.1.1/mbapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)        1 2023-05-30 07:29:02.000000 mbapy-0.1.1/mbapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      393 2023-05-30 07:29:02.000000 mbapy-0.1.1/mbapy.egg-info/requires.txt
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)       54 2023-05-30 07:29:02.000000 mbapy-0.1.1/mbapy.egg-info/top_level.txt
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)       38 2023-05-30 07:29:02.285475 mbapy-0.1.1/setup.cfg
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     2548 2023-05-30 07:28:30.000000 mbapy-0.1.1/setup.py
```

### Comparing `mbapy-0.1.0/LICENSE` & `mbapy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.0/PKG-INFO` & `mbapy-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.1.0
+Version: 0.1.1
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Keywords: mbapy,Utilities,plot
 Platform: any
```

### Comparing `mbapy-0.1.0/README.md` & `mbapy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.0/mbapy/__init__.py` & `mbapy-0.1.1/mbapy/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.0/mbapy/base.py` & `mbapy-0.1.1/mbapy/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-10-19 22:46:30
-LastEditors: BHM-Bob
-LastEditTime: 2023-05-06 16:51:09
+LastEditors: BHM-Bob 2262029386@qq.com
+LastEditTime: 2023-05-29 23:28:04
 Description: 
 '''
 import sys
 import time
 from functools import wraps
 
 import numpy as np
@@ -81,14 +81,17 @@
     if not __NO_ERR__:
         print(f'\nERR : {sys._getframe().f_code.co_name:s} : {info:s}\n')
     return ret
 def put_log(info:str, head = "log", ret = None):
     print(f'\n{head:s} : {sys._getframe().f_code.co_name:s} : {info:s}\n')
     return ret
 
+def get_time(chr:str = ':')->str:
+    return time.asctime(time.localtime()).replace(':', chr)
+
 class MyArgs():
     def __init__(self, args:dict) -> None:
         self.args = dict()
         args = self.get_args(args)
     def get_args(self, args:dict, force_update = True, del_origin = False):
         for arg_name in list(args.keys()):
             if arg_name in self.args and not force_update:
@@ -108,8 +111,17 @@
 
 def get_wanted_args(defalut_args:dict, kwargs:dict, del_kwargs = True):
     """
     wanted_args:dict with default value
     localVar = locals()
     """
     return MyArgs(defalut_args).get_args(kwargs, True, del_kwargs)
-            
+            
+def split_list(lst:list, n = 1, drop_last = False):
+    """
+    return split sub lists.\n
+    when drop_last is True and last one is less than n, drop the last one
+    """
+    result = [lst[i:i+n] for i in range(0, len(lst), n)]
+    if drop_last and len(result[-1]) < n:
+        del result[-1]
+    return result
```

### Comparing `mbapy-0.1.0/mbapy/dl_torch/bb.py` & `mbapy-0.1.1/mbapy/dl_torch/bb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2023-03-23 21:50:21
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-05-22 17:19:55
+LastEditTime: 2023-05-30 09:56:55
 Description: Basic Blocks
 '''
 
 import math
 from typing import Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from . import paper
+from ..base import autoparse
 
 class CnnCfg:
-    @torch.jit.ignore
+    @autoparse
     def __init__(self, inc:int, outc:int, kernel_size:int = 3, stride:int = 1, padding:int = 1):
         self.inc:int = inc
         self.outc:int = outc
         self.kernel_size:int = kernel_size 
         self.stride:int = stride
         self.padding:int = padding
         self._str_:str = ','.join([attr+'='+str(getattr(self, attr)) for attr in vars(self)])
@@ -86,15 +87,15 @@
         stride : int=2,
         padding : int=1,# F.unflod的padding是两边（四周）均pad padding个0
         kernel_size : int=3,
         outway : str="linear", # linear or avg
         dropout : float=0.2,
     ):
         super(SCANN, self).__init__()
-        assert inc % group == 0
+        assert inc % group == 0, r'NOT inc % group == 0'
         self.inc = inc
         self.group = group
         self.stride = stride
         self.padding = padding
         self.kernel_size = kernel_size
         self.patch_size = kernel_size**2
 
@@ -167,15 +168,15 @@
     if kwargs['use_enhanced_fc_q'] and 'q_len' in kwargs and 'out_len' in kwargs\n
     use fc_q mlp like PositionwiseFeedforwardLayer to output a tensor with out_len\n
     if 'out_dim' in kwargs\n
     self.fc_o = nn.Linear(hid_dim, kwargs['out_dim'])
     """
     def __init__(self, hid_dim, n_heads, dropout, device = 'cuda', **kwargs):
         super().__init__()
-        assert hid_dim % n_heads == 0
+        assert hid_dim % n_heads == 0, 'NOT hid_dim % n_heads == 0'
         self.hid_dim = hid_dim
         self.n_heads = n_heads
         self.head_dim = hid_dim // n_heads
         self.fc_q = nn.Linear(hid_dim, hid_dim)
         self.fc_k = nn.Linear(hid_dim, hid_dim)
         self.fc_v = nn.Linear(hid_dim, hid_dim)
         self.fc_o = nn.Linear(hid_dim, hid_dim)
@@ -203,15 +204,15 @@
         # x = [batch size, query len, hid dim]
         return self.fc_o(x)
     
 class FastMultiHeadAttentionLayer(nn.Module):
     """wrapper for FlashAttention, just import flash_attn and adjust dtype"""
     def __init__(self, hid_dim, n_heads, dropout, device = 'cuda', **kwargs):
         super().__init__()
-        assert paper.bb.FlashMHA is not None
+        assert paper.bb.FlashMHA is not None, 'paper.bb.FlashMHA is None'
         self.net = paper.bb.FlashMHA(hid_dim, n_heads,
                                      device=device, dtype = torch.float16)
     def forward(self, query, key, value):
         ori_type = query.dtype
         query = query.to(dtype = torch.float16)
         query = self.net(query)[0]
         return query.to(dtype = ori_type)
@@ -307,15 +308,15 @@
         return self.ff_layer_norm(self.dropout(_src))
 
 class Trans(nn.Module):
     """[batch size, src len, hid dim]"""
     def __init__(self, q_len:int, class_num:int, hid_dim:int, n_layers:int, n_heads:int, pf_dim:int,
                  dropout:float, device:str, out_encoder_layer = OutEncoderLayer, **kwargs):
         super().__init__()
-        assert n_layers > 0
+        assert n_layers > 0, 'n_layers < 0'
         self.nn = nn.Sequential(
             *([EncoderLayer(q_len, class_num, hid_dim, n_heads, pf_dim, dropout, device, **kwargs) \
                 for _ in range(n_layers - 1)]+\
                 [out_encoder_layer(q_len, class_num, hid_dim, n_heads, pf_dim, dropout, device, **kwargs)]))
     def forward(self, src):
         return self.nn(src)
     
@@ -333,26 +334,26 @@
 class OutEncoderLayerAvg(EncoderLayer):
     def __init__(self, q_len:int, class_num:int, hid_dim:int, n_heads:int,
                  pf_dim:int, dropout:float, device:str = 'cuda', **kwargs):
         """AvgPool1d handle [N, C, L] and output [N, C, L']"""
         super().__init__(q_len, class_num, hid_dim, n_heads, pf_dim, dropout, device, **kwargs)
         self.self_attention = MultiHeadAttentionLayer(hid_dim, n_heads, dropout, device)
         if q_len > class_num:
-            assert q_len % class_num == 0
-            self.fc_out = nn.Sequential(
+            assert q_len % class_num == 0, r'q_len % class_num != 0'
+            self.avg = nn.Sequential(
                 nn.AvgPool1d(hid_dim, 1, 0),
                 reshape(-1, q_len),
                 nn.AvgPool1d(int(q_len/class_num), int(q_len/class_num), 0),
             )
         elif q_len < class_num:
-            assert class_num % q_len == 0
+            assert class_num % q_len == 0, r'q_len % class_num != 0'
             ks = int(q_len * hid_dim / class_num)
-            self.fc_out = nn.AvgPool1d(ks, ks, 0)
+            self.avg = nn.AvgPool1d(ks, ks, 0)
         elif q_len == class_num:
-            self.fc_out = nn.AvgPool1d(hid_dim, 1, 0)
+            self.avg = nn.AvgPool1d(hid_dim, 1, 0)
         self.outc = class_num
             
     def forward(self, src):
         # src = [batch size, src len, hid dim]
         b, l, c = src.shape
         # self attention
         _src = self.self_attention(src, src, src)
```

### Comparing `mbapy-0.1.0/mbapy/dl_torch/data.py` & `mbapy-0.1.1/mbapy/dl_torch/data.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.0/mbapy/dl_torch/hyper_search.py` & `mbapy-0.1.1/mbapy/dl_torch/hyper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.0/mbapy/dl_torch/loss.py` & `mbapy-0.1.1/mbapy/dl_torch/loss.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.0/mbapy/dl_torch/m.py` & `mbapy-0.1.1/mbapy/dl_torch/m.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.0/mbapy/dl_torch/paper/bb.py` & `mbapy-0.1.1/mbapy/dl_torch/paper/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.0/mbapy/dl_torch/utils.py` & `mbapy-0.1.1/mbapy/dl_torch/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,21 +118,24 @@
             [ print(attr,' : ',dic[attr]) for attr in dic.keys()]
         return dic
     def set_resume(self):
         self.resume_paths = glob.glob(os.path.join(self.model_root,'*.tar'))
         self.resume = self.resume_paths[0] if len(self.resume_paths) > 0 else 'None'
 
 def init_model_parameter(model):
-    # model initilization
+    """model initilization"""
     for m in model.modules():
         if isinstance(m, nn.Conv2d) or isinstance(m, nn.Conv1d):
-            nn.init.kaiming_normal_(m.weight, mode='fan_out', nonlinearity='leaky_relu')
+            if m.weight is not None:
+                nn.init.kaiming_normal_(m.weight, mode='fan_out', nonlinearity='leaky_relu')
         elif isinstance(m, nn.BatchNorm2d) or isinstance(m, nn.BatchNorm1d):
-            nn.init.constant_(m.weight, 1)
-            nn.init.constant_(m.bias, 0)
+            if m.weight is not None:
+                nn.init.constant_(m.weight, 1)
+            if m.bias is not None:
+                nn.init.constant_(m.bias, 0)
     return model
 
 def adjust_learning_rate(optimizer, now_epoch, args):
     """Decay the learning rate based on schedule
     args"""
     lr = args.lr
     if args.cos:  # cosine lr schedule
@@ -212,15 +215,15 @@
         "arch": args.arch,
         "state_dict": model.state_dict(),
         "optimizer": optimizer.state_dict(),
         "loss": loss,
         "args":args.toDict(),
     }
     state.update(other)
-    filename = os.path.join(args.model_oot,
+    filename = os.path.join(args.model_root,
                             f"checkpoint_{tailName:s}_{time.asctime(time.localtime()).replace(':', '-'):s}.pth.tar")
     torch.save(state, filename)
 
 def resume(args, model, optimizer, other:dict = {}):
     if args.resume and os.path.isfile(args.resume):
         args.mp.mprint("=> loading checkpoint '{}'".format(args.resume))
         if args.gpu is None:
```

### Comparing `mbapy-0.1.0/mbapy/file.py` & `mbapy-0.1.1/mbapy/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 19:09:54
-LastEditors: BHM-Bob
-LastEditTime: 2023-04-27 13:01:20
+LastEditors: BHM-Bob 2262029386@qq.com
+LastEditTime: 2023-05-27 23:44:35
 Description: 
 '''
 import chardet
 import json
 import os
 
 import pandas as pd
 
-
 def detect_byte_coding(bits:bytes):
     adchar = chardet.detect(bits[:(1000 if len(bits) > 1000 else len(bits))])['encoding']
     if adchar == 'gbk' or adchar == 'GBK' or adchar == 'GB2312':
         true_text = bits.decode('GB2312', "ignore")
     else:
         true_text = bits.decode('utf-8', "ignore")
     return true_text
 
+def get_byte_coding(bits:bytes, max_detect_len = 1000):
+    return chardet.detect(bits[ : min(max_detect_len, len(bits))])['encoding']
+
+def decode_bits_to_str(bits:bytes):
+    adchar = get_byte_coding(bits, max_detect_len = 1000)
+    if adchar == 'gbk' or adchar == 'GBK' or adchar == 'GB2312':
+        true_text = bits.decode('GB2312', "ignore")
+    else:
+        true_text = bits.decode('utf-8', "ignore")
+    return true_text
+
 def save_json(path:str, obj, encoding:str = 'utf-8', forceUpdate = True):
     if forceUpdate or not os.path.isfile(path):
         json_str = json.dumps(obj, indent=1)
         with open(path, 'w' ,encoding=encoding, errors='ignore') as json_file:
             json_file.write(json_str)
 def read_json(path:str, encoding:str = 'utf-8', invalidPathReturn = None):
     if os.path.isfile(path):
```

### Comparing `mbapy-0.1.0/mbapy/plot.py` & `mbapy-0.1.1/mbapy/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     n: how many colors required
     mode: kind of colors
         - hls : [default] sns.color_palette('hls', n)
         - green : sum 5 grenns
         - pair : plt.get_cmap('tab20')
         - None : plt.get_cmap('Set1') for n<=9 or plt.get_cmap('Set3') for n<= 12
     """
-    assert n >= 1
+    assert n >= 1, 'n < 1'
     if mode == 'hls':
         return rgbs2hexs(sns.color_palette('hls', n))
     if n <= 5 and mode == 'green':
         return ['#80ab1c', '#405535', '#99b69b', '#92e4ce', '#72cb87'][0:n]
     elif n <= 9:
         return rgbs2hexs(plt.get_cmap('Set1').colors)
     elif n <= 12:
```

### Comparing `mbapy-0.1.0/mbapy/stats/__init__.py` & `mbapy-0.1.1/mbapy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.0/mbapy/stats/df.py` & `mbapy-0.1.1/mbapy/stats/df.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2023-04-10 20:59:26
-LastEditors: BHM-Bob
-LastEditTime: 2023-04-30 18:56:49
+LastEditors: BHM-Bob 2262029386@qq.com
+LastEditTime: 2023-05-30 10:00:31
 Description: pd.dataFrame utils
 '''
 
 import pandas as pd
 import numpy as np
 
 from mbapy.plot import pro_bar_data, get_df_data, sort_df_factors
@@ -75,16 +75,16 @@
                 to_remove_idx.append(i+1)
             i += 1
     ndf.drop(labels = to_remove_idx, inplace=True)
     return ndf, to_remove_idx
 
 def interp(long_one:pd.Series, short_one:pd.Series):
     """
-    给定两个pd.Series，一长一短，用线性插值给短的插值，使其长度与长的pd.Series一样\n
+    给定两个pd.Series,一长一短,用线性插值给短的插值,使其长度与长的pd.Series一样\n
     Given two pd.Series, one long and one short, use linear interpolation to give the short one the same length as the long pd.Series\n
     """
-    assert len(long_one) > len(short_one)
+    assert len(long_one) > len(short_one), 'len(long_one) <= len(short_one)'
     short_one_idx = np.array(np.arange(short_one.shape[0])*(long_one.shape[0]/short_one.shape[0]), dtype=np.int32)
     if short_one_idx[-1] < long_one.shape[0]-1:
         short_one_idx[-1] = long_one.shape[0]-1
     return np.interp(np.arange(long_one.shape[0]), short_one_idx, short_one)
```

### Comparing `mbapy-0.1.0/mbapy/stats/geography.py` & `mbapy-0.1.1/mbapy/stats/geography.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.0/mbapy/stats/reg.py` & `mbapy-0.1.1/mbapy/stats/reg.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.0/mbapy/stats/test.py` & `mbapy-0.1.1/mbapy/stats/test.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.0/mbapy/web.py` & `mbapy-0.1.1/mbapy/web.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.0/mbapy.egg-info/PKG-INFO` & `mbapy-0.1.1/mbapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.1.0
+Version: 0.1.1
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Keywords: mbapy,Utilities,plot
 Platform: any
```

### Comparing `mbapy-0.1.0/mbapy.egg-info/SOURCES.txt` & `mbapy-0.1.1/mbapy.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 mbapy.egg-info/top_level.txt
 mbapy/dl_torch/__init__.py
 mbapy/dl_torch/bb.py
 mbapy/dl_torch/data.py
 mbapy/dl_torch/hyper_search.py
 mbapy/dl_torch/loss.py
 mbapy/dl_torch/m.py
+mbapy/dl_torch/optim.py
 mbapy/dl_torch/utils.py
 mbapy/dl_torch/paper/__init__.py
 mbapy/dl_torch/paper/bb.py
 mbapy/stats/__init__.py
 mbapy/stats/df.py
 mbapy/stats/geography.py
 mbapy/stats/reg.py
```

### Comparing `mbapy-0.1.0/setup.py` & `mbapy-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 18:30:01
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-05-22 16:21:54
+LastEditTime: 2023-05-27 17:38:26
 Description: 
 '''
 """
 something is from https://github.com/pypa/sampleproject
 thanks to https://zetcode.com/python/package/
 """
 
@@ -33,15 +33,15 @@
     "cn2an>=0.5.17",
     "holoviews>=1.13.1",
     "imageio>=2.20.2",
     "jieba>=0.42.1",
     "Markdown>=3.4.1",
     "matplotlib>=3.5.3",
     "multiprocess>=0.70.13",
-    # "numpy>=1.22.1",
+    "numpy>=1.22.1",
     "pandas>=1.4.3",
     "pathtools>=0.1.2",
     "pdfkit>=1.0.0",
     "Pillow>=9.2.0",
     "plotly>=5.10.0",
     "requests>=2.25.1",
     "scikit-learn>=1.1.2",
@@ -52,15 +52,15 @@
     "openpyxl",
     "statsmodels",
     "scikit_posthocs",
 ]
 
 setup(
     name = "mbapy",
-    version = "0.1.0",
+    version = "0.1.1",
 
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Topic :: Utilities",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
@@ -92,8 +92,8 @@
     install_requires=requires,
 )
 
 # pip install .
 
 
 # python setup.py sdist
-# twine upload dist/mbapy-0.0.15.tar.gz
+# twine upload dist/mbapy-0.1.1.tar.gz
```

