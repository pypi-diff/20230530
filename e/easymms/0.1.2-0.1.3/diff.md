# Comparing `tmp/easymms-0.1.2.tar.gz` & `tmp/easymms-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easymms-0.1.2.tar", last modified: Mon May 29 04:24:23 2023, max compression
+gzip compressed data, was "easymms-0.1.3.tar", last modified: Tue May 30 00:43:15 2023, max compression
```

## Comparing `easymms-0.1.2.tar` & `easymms-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:23.548463 easymms-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-05-29 04:24:12.000000 easymms-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-29 04:24:23.548463 easymms-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-29 04:24:12.000000 easymms-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:23.548463 easymms-0.1.2/easymms/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:23.548463 easymms-0.1.2/easymms/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/models/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/models/asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:23.548463 easymms-0.1.2/easymms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-29 04:24:23.000000 easymms-0.1.2/easymms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-29 04:24:23.000000 easymms-0.1.2/easymms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 04:24:23.000000 easymms-0.1.2/easymms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 04:24:23.000000 easymms-0.1.2/easymms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 04:24:23.000000 easymms-0.1.2/easymms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 04:24:23.000000 easymms-0.1.2/easymms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 04:24:23.548463 easymms-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-29 04:24:12.000000 easymms-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:23.548463 easymms-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:12.000000 easymms-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-29 04:24:12.000000 easymms-0.1.2/tests/test_asr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:15.811291 easymms-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-05-30 00:43:08.000000 easymms-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-30 00:43:15.811291 easymms-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-30 00:43:08.000000 easymms-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:15.807291 easymms-0.1.3/easymms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:15.807291 easymms-0.1.3/easymms/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/models/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/models/asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:15.811291 easymms-0.1.3/easymms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-30 00:43:15.000000 easymms-0.1.3/easymms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-30 00:43:15.000000 easymms-0.1.3/easymms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:43:15.000000 easymms-0.1.3/easymms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:43:15.000000 easymms-0.1.3/easymms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 00:43:15.000000 easymms-0.1.3/easymms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 00:43:15.000000 easymms-0.1.3/easymms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 00:43:15.811291 easymms-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-30 00:43:08.000000 easymms-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:15.807291 easymms-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:08.000000 easymms-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-30 00:43:08.000000 easymms-0.1.3/tests/test_asr.py
```

### Comparing `easymms-0.1.2/LICENSE` & `easymms-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easymms-0.1.2/PKG-INFO` & `easymms-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,15 @@
-Metadata-Version: 2.1
-Name: easymms
-Version: 0.1.2
-Summary: A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project
-Author: Abdeladim Sadiki
-License: MIT
-Project-URL: Documentation, https://abdeladim-s.github.io/easymms/
-Project-URL: Source, https://abdeladim-s.github.io/easymms/
-Project-URL: Tracker, https://abdeladim-s.github.io/easymms/issues
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # EasyMMS
 
 A simple Python package to easily use [Meta's Massively Multilingual Speech (MMS) project](https://github.com/facebookresearch/fairseq/tree/main/examples/mms). 
 
 [![PyPi version](https://badgen.net/pypi/v/easymms)](https://pypi.org/project/easymms/)
+<a target="_blank" href="https://colab.research.google.com/github/abdeladim-s/easymms/blob/main/examples/EasyMMS.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
 
 <!-- TOC -->
 * [Installation](#installation)
 * [Quickstart](#quickstart)
   * [ASR](#asr)
   * [ASR with Alignment](#asr-with-alignment)
   * [TTS](#tts)
@@ -41,14 +31,18 @@
 ```
 * You might need [sox](https://arielvb.readthedocs.io/en/latest/docs/commandline/sox.html) as well.
 
 3. Install `easymms` from Pypi
 ```bash
 pip install easymms
 ```
+or from source 
+```bash
+pip install git+https://github.com/abdeladim-s/easymms
+```
 
 # Quickstart
 
 ## ASR 
 You will need first to download the model weights, you can find and download all the supported models from [here](https://github.com/facebookresearch/fairseq/tree/main/examples/mms#asr).
```

### Comparing `easymms-0.1.2/README.md` & `easymms-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,28 @@
+Metadata-Version: 2.1
+Name: easymms
+Version: 0.1.3
+Summary: A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project
+Author: Abdeladim Sadiki
+License: MIT
+Project-URL: Documentation, https://abdeladim-s.github.io/easymms/
+Project-URL: Source, https://abdeladim-s.github.io/easymms/
+Project-URL: Tracker, https://abdeladim-s.github.io/easymms/issues
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # EasyMMS
 
 A simple Python package to easily use [Meta's Massively Multilingual Speech (MMS) project](https://github.com/facebookresearch/fairseq/tree/main/examples/mms). 
 
 [![PyPi version](https://badgen.net/pypi/v/easymms)](https://pypi.org/project/easymms/)
+<a target="_blank" href="https://colab.research.google.com/github/abdeladim-s/easymms/blob/main/examples/EasyMMS.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
 
 <!-- TOC -->
 * [Installation](#installation)
 * [Quickstart](#quickstart)
   * [ASR](#asr)
   * [ASR with Alignment](#asr-with-alignment)
   * [TTS](#tts)
@@ -28,14 +44,18 @@
 ```
 * You might need [sox](https://arielvb.readthedocs.io/en/latest/docs/commandline/sox.html) as well.
 
 3. Install `easymms` from Pypi
 ```bash
 pip install easymms
 ```
+or from source 
+```bash
+pip install git+https://github.com/abdeladim-s/easymms
+```
 
 # Quickstart
 
 ## ASR 
 You will need first to download the model weights, you can find and download all the supported models from [here](https://github.com/facebookresearch/fairseq/tree/main/examples/mms#asr).
```

### Comparing `easymms-0.1.2/easymms/__init__.py` & `easymms-0.1.3/easymms/__init__.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.2/easymms/_logger.py` & `easymms-0.1.3/easymms/_logger.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.2/easymms/constants.py` & `easymms-0.1.3/easymms/constants.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.2/easymms/models/alignment.py` & `easymms-0.1.3/easymms/models/alignment.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.2/easymms/models/asr.py` & `easymms-0.1.3/easymms/models/asr.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,23 +148,24 @@
         """
         processed_files = self._prepare_media_files(media_files)
         self._setup_tmp_dir(processed_files)
         # edit cfg
         if cfg is None:
             self.cfg['task']['data'] = self.cfg['decoding']['results_path'] = str(self.tmp_dir_path.resolve())
             self.cfg['dataset']['gen_subset'] = f'{lang}:dev'
-            if device is None or device == 'cuda':
+            if device is None:
                 if torch.cuda.is_available():
                     device = 'cuda'
-                    pass  # default
                 else:
                     device = 'cpu'
-            if device == 'cpu':
+            if device == 'cuda':
+                pass  # default
+            elif device == 'cpu':
                 self.cfg['common']['cpu'] = True
-            elif device == 'tpu':
+            if device == 'tpu':
                 self.cfg['common']['tpu'] = True
             else:
                 logging.warning(f'Unknown device option {device}, Use one of (cuda, cpu, tpu)')
             cfg = OmegaConf.structured(self.cfg)
 
         self.wer = hydra_main(cfg)
         # get results: will just read from hypo.word as I don't want to change fairseq repo to get the hypo array
```

### Comparing `easymms-0.1.2/easymms/utils.py` & `easymms-0.1.3/easymms/utils.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.2/easymms.egg-info/PKG-INFO` & `easymms-0.1.3/easymms.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymms
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/easymms/
 Project-URL: Source, https://abdeladim-s.github.io/easymms/
 Project-URL: Tracker, https://abdeladim-s.github.io/easymms/issues
 Requires-Python: >=3.8
@@ -12,14 +12,17 @@
 License-File: LICENSE
 
 # EasyMMS
 
 A simple Python package to easily use [Meta's Massively Multilingual Speech (MMS) project](https://github.com/facebookresearch/fairseq/tree/main/examples/mms). 
 
 [![PyPi version](https://badgen.net/pypi/v/easymms)](https://pypi.org/project/easymms/)
+<a target="_blank" href="https://colab.research.google.com/github/abdeladim-s/easymms/blob/main/examples/EasyMMS.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
 
 <!-- TOC -->
 * [Installation](#installation)
 * [Quickstart](#quickstart)
   * [ASR](#asr)
   * [ASR with Alignment](#asr-with-alignment)
   * [TTS](#tts)
@@ -41,14 +44,18 @@
 ```
 * You might need [sox](https://arielvb.readthedocs.io/en/latest/docs/commandline/sox.html) as well.
 
 3. Install `easymms` from Pypi
 ```bash
 pip install easymms
 ```
+or from source 
+```bash
+pip install git+https://github.com/abdeladim-s/easymms
+```
 
 # Quickstart
 
 ## ASR 
 You will need first to download the model weights, you can find and download all the supported models from [here](https://github.com/facebookresearch/fairseq/tree/main/examples/mms#asr).
```

### Comparing `easymms-0.1.2/setup.py` & `easymms-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 
 setup(
     name="easymms",
-    version="0.1.2",
+    version="0.1.3",
     author="Abdeladim Sadiki",
     description="A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project",
     long_description=long_description,
     ext_modules=[],
     zip_safe=False,
     python_requires=">=3.8",
     packages=find_packages('.'),
```

### Comparing `easymms-0.1.2/tests/test_asr.py` & `easymms-0.1.3/tests/test_asr.py`

 * *Files identical despite different names*

