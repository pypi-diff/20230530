# Comparing `tmp/bio-attention-0.0.1.tar.gz` & `tmp/bio-attention-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-attention-0.0.1.tar", last modified: Tue Dec  6 14:51:27 2022, max compression
+gzip compressed data, was "bio-attention-0.0.2.tar", last modified: Tue May 30 12:24:22 2023, max compression
```

## Comparing `bio-attention-0.0.1.tar` & `bio-attention-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:51:27.049826 bio-attention-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:51:27.041826 bio-attention-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:51:27.041826 bio-attention-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2022-12-06 14:51:15.000000 bio-attention-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2022-12-06 14:51:15.000000 bio-attention-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-06 14:51:15.000000 bio-attention-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2022-12-06 14:51:27.049826 bio-attention-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2022-12-06 14:51:15.000000 bio-attention-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:51:27.045826 bio-attention-0.0.1/bio_attention/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 14:51:15.000000 bio-attention-0.0.1/bio_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2022-12-06 14:51:15.000000 bio-attention-0.0.1/bio_attention/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:51:27.045826 bio-attention-0.0.1/bio_attention/img/
--rw-r--r--   0 runner    (1001) docker     (123)  2372654 2022-12-06 14:51:15.000000 bio-attention-0.0.1/bio_attention/img/2Dslidingwindow-attention.png
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2022-12-06 14:51:15.000000 bio-attention-0.0.1/bio_attention/sliding_window_attn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:51:27.045826 bio-attention-0.0.1/bio_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2022-12-06 14:51:27.000000 bio-attention-0.0.1/bio_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2022-12-06 14:51:27.000000 bio-attention-0.0.1/bio_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 14:51:27.000000 bio-attention-0.0.1/bio_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-06 14:51:27.000000 bio-attention-0.0.1/bio_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-06 14:51:27.000000 bio-attention-0.0.1/bio_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-06 14:51:15.000000 bio-attention-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2022-12-06 14:51:27.049826 bio-attention-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:22.888790 bio-attention-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:22.880790 bio-attention-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:22.880790 bio-attention-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-30 12:24:11.000000 bio-attention-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-30 12:24:11.000000 bio-attention-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-30 12:24:11.000000 bio-attention-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-30 12:24:22.888790 bio-attention-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-30 12:24:11.000000 bio-attention-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:22.880790 bio-attention-0.0.2/bio_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:11.000000 bio-attention-0.0.2/bio_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-05-30 12:24:11.000000 bio-attention-0.0.2/bio_attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-30 12:24:11.000000 bio-attention-0.0.2/bio_attention/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:22.888790 bio-attention-0.0.2/bio_attention/img/
+-rw-r--r--   0 runner    (1001) docker     (123)  2372654 2023-05-30 12:24:11.000000 bio-attention-0.0.2/bio_attention/img/2Dslidingwindow-attention.png
+-rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-05-30 12:24:11.000000 bio-attention-0.0.2/bio_attention/img/windowed_implementation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21740 2023-05-30 12:24:11.000000 bio-attention-0.0.2/bio_attention/positional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:22.884790 bio-attention-0.0.2/bio_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-30 12:24:22.000000 bio-attention-0.0.2/bio_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 12:24:22.000000 bio-attention-0.0.2/bio_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:24:22.000000 bio-attention-0.0.2/bio_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 12:24:22.000000 bio-attention-0.0.2/bio_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 12:24:22.000000 bio-attention-0.0.2/bio_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-30 12:24:11.000000 bio-attention-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-30 12:24:22.888790 bio-attention-0.0.2/setup.cfg
```

### Comparing `bio-attention-0.0.1/.github/workflows/publish.yml` & `bio-attention-0.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.1/.gitignore` & `bio-attention-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.1/LICENSE` & `bio-attention-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.1/PKG-INFO` & `bio-attention-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,61 @@
-Metadata-Version: 2.1
-Name: bio-attention
-Version: 0.0.1
-Summary: Simple implementations of attention modules adapted for the biological data domain
-Home-page: https://github.com/gdewael/bio-attention
-Author: Gaetan De Waele
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 <h1>bio-attention</h1>
 
 Simple implementations of attention modules adapted for the biological data domain.
 
-
 [![PyPi Version](https://img.shields.io/pypi/v/bio-attention.svg)](https://pypi.python.org/pypi/bio-attention/)
 [![GitHub license](https://img.shields.io/github/license/gdewael/bio-attention)](https://github.com/gdewael/bio-attention/blob/main/LICENSE)
 
 </div>
 
 
 
+# :construction: THIS CODE IS BEING ACTIVELY DEVELOPED :construction:
+
+Don't look for stability here (yet).
+
 ## Install
-Since PyTorch is a dependency of `h5torch`, we recommend [installing PyTorch](https://pytorch.org/get-started/locally/) independently first, as your system may require a specific version (e.g. CUDA drivers).
+Since PyTorch is a dependency of `bio-attention`, we recommend [installing PyTorch](https://pytorch.org/get-started/locally/) independently first, as your system may require a specific version (e.g. CUDA drivers).
 
-After PyTorch installation, `h5torch` can be installed using `pip`
+After PyTorch installation, `bio-attention` can be installed using `pip`
 ```bash
 pip install bio-attention
 ```
 
 ## Usage
 
 ## Package roadmap
-- [x] Implement typing
+
+- [x] Embedding layers
+  - [x] Continuous
+  - [x] Discrete
+  - [x] Binary
+  - [x] Bin
+- [~] Positional encoding schemes
+  - [x] Sinusoidal
+  - [x] Embedding
+  - [x] Continuous
+  - [x] Rotary
+  - [x] AliBi
+  - [x] DPB
+  - [x] XL
+  - [x] Test support for multi-dimensional inputs
+- [~] Attention modules
+  - [x] Vanilla
+  - [x] Windowed
+  - [x] Random
+  - [x] Performer
+  - [x] Encoder
+  - [x] Decoder
+  - [ ] Cross
+  - [x] Support for multi-dim inputs
+- [ ] Tests
+- [ ] Typing
+- [ ] Docs
 
 
 # LEGACY documentation
 ## THIS REPO USED TO BE A 2D SLIDING WINDOW ATTENTION REPO
 
 ### 2D Sliding Window Attention
```

### Comparing `bio-attention-0.0.1/README.md` & `bio-attention-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,71 @@
+Metadata-Version: 2.1
+Name: bio-attention
+Version: 0.0.2
+Summary: Simple implementations of attention modules adapted for the biological data domain
+Home-page: https://github.com/gdewael/bio-attention
+Author: Gaetan De Waele
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 <h1>bio-attention</h1>
 
 Simple implementations of attention modules adapted for the biological data domain.
 
-
 [![PyPi Version](https://img.shields.io/pypi/v/bio-attention.svg)](https://pypi.python.org/pypi/bio-attention/)
 [![GitHub license](https://img.shields.io/github/license/gdewael/bio-attention)](https://github.com/gdewael/bio-attention/blob/main/LICENSE)
 
 </div>
 
 
 
+# :construction: THIS CODE IS BEING ACTIVELY DEVELOPED :construction:
+
+Don't look for stability here (yet).
+
 ## Install
-Since PyTorch is a dependency of `h5torch`, we recommend [installing PyTorch](https://pytorch.org/get-started/locally/) independently first, as your system may require a specific version (e.g. CUDA drivers).
+Since PyTorch is a dependency of `bio-attention`, we recommend [installing PyTorch](https://pytorch.org/get-started/locally/) independently first, as your system may require a specific version (e.g. CUDA drivers).
 
-After PyTorch installation, `h5torch` can be installed using `pip`
+After PyTorch installation, `bio-attention` can be installed using `pip`
 ```bash
 pip install bio-attention
 ```
 
 ## Usage
 
 ## Package roadmap
-- [x] Implement typing
+
+- [x] Embedding layers
+  - [x] Continuous
+  - [x] Discrete
+  - [x] Binary
+  - [x] Bin
+- [~] Positional encoding schemes
+  - [x] Sinusoidal
+  - [x] Embedding
+  - [x] Continuous
+  - [x] Rotary
+  - [x] AliBi
+  - [x] DPB
+  - [x] XL
+  - [x] Test support for multi-dimensional inputs
+- [~] Attention modules
+  - [x] Vanilla
+  - [x] Windowed
+  - [x] Random
+  - [x] Performer
+  - [x] Encoder
+  - [x] Decoder
+  - [ ] Cross
+  - [x] Support for multi-dim inputs
+- [ ] Tests
+- [ ] Typing
+- [ ] Docs
 
 
 # LEGACY documentation
 ## THIS REPO USED TO BE A 2D SLIDING WINDOW ATTENTION REPO
 
 ### 2D Sliding Window Attention
```

### Comparing `bio-attention-0.0.1/bio_attention/img/2Dslidingwindow-attention.png` & `bio-attention-0.0.2/bio_attention/img/2Dslidingwindow-attention.png`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.1/bio_attention.egg-info/PKG-INFO` & `bio-attention-0.0.2/bio_attention.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,71 @@
 Metadata-Version: 2.1
 Name: bio-attention
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple implementations of attention modules adapted for the biological data domain
 Home-page: https://github.com/gdewael/bio-attention
 Author: Gaetan De Waele
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 <h1>bio-attention</h1>
 
 Simple implementations of attention modules adapted for the biological data domain.
 
-
 [![PyPi Version](https://img.shields.io/pypi/v/bio-attention.svg)](https://pypi.python.org/pypi/bio-attention/)
 [![GitHub license](https://img.shields.io/github/license/gdewael/bio-attention)](https://github.com/gdewael/bio-attention/blob/main/LICENSE)
 
 </div>
 
 
 
+# :construction: THIS CODE IS BEING ACTIVELY DEVELOPED :construction:
+
+Don't look for stability here (yet).
+
 ## Install
-Since PyTorch is a dependency of `h5torch`, we recommend [installing PyTorch](https://pytorch.org/get-started/locally/) independently first, as your system may require a specific version (e.g. CUDA drivers).
+Since PyTorch is a dependency of `bio-attention`, we recommend [installing PyTorch](https://pytorch.org/get-started/locally/) independently first, as your system may require a specific version (e.g. CUDA drivers).
 
-After PyTorch installation, `h5torch` can be installed using `pip`
+After PyTorch installation, `bio-attention` can be installed using `pip`
 ```bash
 pip install bio-attention
 ```
 
 ## Usage
 
 ## Package roadmap
-- [x] Implement typing
+
+- [x] Embedding layers
+  - [x] Continuous
+  - [x] Discrete
+  - [x] Binary
+  - [x] Bin
+- [~] Positional encoding schemes
+  - [x] Sinusoidal
+  - [x] Embedding
+  - [x] Continuous
+  - [x] Rotary
+  - [x] AliBi
+  - [x] DPB
+  - [x] XL
+  - [x] Test support for multi-dimensional inputs
+- [~] Attention modules
+  - [x] Vanilla
+  - [x] Windowed
+  - [x] Random
+  - [x] Performer
+  - [x] Encoder
+  - [x] Decoder
+  - [ ] Cross
+  - [x] Support for multi-dim inputs
+- [ ] Tests
+- [ ] Typing
+- [ ] Docs
 
 
 # LEGACY documentation
 ## THIS REPO USED TO BE A 2D SLIDING WINDOW ATTENTION REPO
 
 ### 2D Sliding Window Attention
```

