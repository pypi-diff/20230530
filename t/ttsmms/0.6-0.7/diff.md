# Comparing `tmp/ttsmms-0.6.tar.gz` & `tmp/ttsmms-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttsmms-0.6.tar", last modified: Fri May 26 07:30:44 2023, max compression
+gzip compressed data, was "ttsmms-0.7.tar", last modified: Tue May 30 14:50:42 2023, max compression
```

## Comparing `ttsmms-0.6.tar` & `ttsmms-0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:30:44.738598 ttsmms-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-26 07:30:31.000000 ttsmms-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-26 07:30:44.738598 ttsmms-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-26 07:30:31.000000 ttsmms-0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:30:44.738598 ttsmms-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 07:30:31.000000 ttsmms-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:30:44.738598 ttsmms-0.6/ttsmms/
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/attentions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/mel_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:30:44.738598 ttsmms-0.6/ttsmms/text/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/text/cleaners.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/text/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:30:44.738598 ttsmms-0.6/ttsmms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-26 07:30:44.000000 ttsmms-0.6/ttsmms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-26 07:30:44.000000 ttsmms-0.6/ttsmms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:30:44.000000 ttsmms-0.6/ttsmms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:30:44.000000 ttsmms-0.6/ttsmms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 07:30:44.000000 ttsmms-0.6/ttsmms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 07:30:44.000000 ttsmms-0.6/ttsmms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:42.955827 ttsmms-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-30 14:50:30.000000 ttsmms-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-30 14:50:42.955827 ttsmms-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-30 14:50:30.000000 ttsmms-0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:50:42.955827 ttsmms-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-30 14:50:30.000000 ttsmms-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:42.951827 ttsmms-0.7/ttsmms/
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-05-30 14:50:30.000000 ttsmms-0.7/ttsmms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-30 14:50:30.000000 ttsmms-0.7/ttsmms/attentions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-30 14:50:30.000000 ttsmms-0.7/ttsmms/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-05-30 14:50:30.000000 ttsmms-0.7/ttsmms/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-30 14:50:31.000000 ttsmms-0.7/ttsmms/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-30 14:50:31.000000 ttsmms-0.7/ttsmms/mel_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-05-30 14:50:31.000000 ttsmms-0.7/ttsmms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-05-30 14:50:31.000000 ttsmms-0.7/ttsmms/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 14:50:31.000000 ttsmms-0.7/ttsmms/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:42.955827 ttsmms-0.7/ttsmms/text/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-30 14:50:31.000000 ttsmms-0.7/ttsmms/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-30 14:50:31.000000 ttsmms-0.7/ttsmms/text/cleaners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-30 14:50:31.000000 ttsmms-0.7/ttsmms/text/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-05-30 14:50:31.000000 ttsmms-0.7/ttsmms/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-05-30 14:50:31.000000 ttsmms-0.7/ttsmms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:42.955827 ttsmms-0.7/ttsmms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-30 14:50:42.000000 ttsmms-0.7/ttsmms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-30 14:50:42.000000 ttsmms-0.7/ttsmms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:50:42.000000 ttsmms-0.7/ttsmms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:50:42.000000 ttsmms-0.7/ttsmms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-30 14:50:42.000000 ttsmms-0.7/ttsmms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 14:50:42.000000 ttsmms-0.7/ttsmms.egg-info/top_level.txt
```

### Comparing `ttsmms-0.6/LICENSE` & `ttsmms-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/PKG-INFO` & `ttsmms-0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttsmms
-Version: 0.6
+Version: 0.7
 Summary: Text-to-speech with The Massively Multilingual Speech (MMS) project
 Home-page: https://github.com/wannaphong/ttsmms
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: MIT License
 Project-URL: Source, https://github.com/wannaphong/ttsmms
 Keywords: tts,NLP
@@ -39,30 +39,40 @@
 > pip install ttsmms
 
 
 ## Usage
 
 First, you need to download the model by
 
+```python
+from ttsmms import download
+
+dir_path = download("eng","./data") # lang_code, dir for save model
+```
+
+or download file by yourself
+
 **Linux/Mac**
 
+1. download
+
 > curl https://dl.fbaipublicfiles.com/mms/tts/lang_code.tar.gz --output lang_code.tar.gz
 
-and extract a tar ball archive.
+2. extract a tar ball archive.
 
 **Linux/Mac**
 
 > mkdir -p data && tar -xzf lang_code.tar.gz -C data/
 
 and use code in python :D
 
 ```python
 from ttsmms import TTS
 
-tts=TTS("model_dir_path") # your path dir that extract a tar ball archive
+tts=TTS(dir_path) # or "model_dir_path" your path dir that extract a tar ball archive
 wav=tts.synthesis("txt")
 # output:
 # {
 #    "x":array(wav array),
 #    "sampling_rate": 16000
 # }
```

### Comparing `ttsmms-0.6/README.md` & `ttsmms-0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -17,33 +17,43 @@
 > pip install ttsmms
 
 
 ## Usage
 
 First, you need to download the model by
 
+```python
+from ttsmms import download
+
+dir_path = download("eng","./data") # lang_code, dir for save model
+```
+
+or download file by yourself
+
 **Linux/Mac**
 
+1. download
+
 > curl https://dl.fbaipublicfiles.com/mms/tts/lang_code.tar.gz --output lang_code.tar.gz
 
-and extract a tar ball archive.
+2. extract a tar ball archive.
 
 **Linux/Mac**
 
 > mkdir -p data && tar -xzf lang_code.tar.gz -C data/
 
 and use code in python :D
 
 ```python
 from ttsmms import TTS
 
-tts=TTS("model_dir_path") # your path dir that extract a tar ball archive
+tts=TTS(dir_path) # or "model_dir_path" your path dir that extract a tar ball archive
 wav=tts.synthesis("txt")
 # output:
 # {
 #    "x":array(wav array),
 #    "sampling_rate": 16000
 # }
 
 tts.synthesis("txt",wav_path="example.wav")
 # output: example.wav file
-```
+```
```

### Comparing `ttsmms-0.6/setup.py` & `ttsmms-0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     "librosa",
     "scipy",
     "numpy",
     "phonemizer",
     "torch",
     "torchvision",
     "Unidecode",
-    "monotonic-align"
+    "monotonic-align",
 ]
 
 setup(
     name="ttsmms",
-    version="0.6",
+    version="0.7",
     description="Text-to-speech with The Massively Multilingual Speech (MMS) project",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Wannaphong",
     author_email="wannaphong@yahoo.com",
     url="https://github.com/wannaphong/ttsmms",
     packages=find_packages(),
```

### Comparing `ttsmms-0.6/ttsmms/__init__.py` & `ttsmms-0.7/ttsmms/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,38 @@
 import numpy as np
 import ttsmms.commons
 import ttsmms.utils
 import argparse
 from ttsmms.data_utils import TextAudioLoader, TextAudioCollate, TextAudioSpeakerLoader, TextAudioSpeakerCollate
 from ttsmms.models import SynthesizerTrn
 from scipy.io.wavfile import write
+from pathlib import Path
+
+
+def download(lang, tgt_dir="./"):
+    lang_fn, lang_dir = os.path.join(tgt_dir, lang+'.tar.gz'), os.path.join(tgt_dir, lang)
+    isExist = os.path.exists(lang_dir)
+    if isExist:
+        return lang_dir
+    Path(tgt_dir).mkdir(parents=True, exist_ok=True)
+    if isExist:
+        return lang_dir
+    from urllib.request import urlretrieve
+    url = f"https://dl.fbaipublicfiles.com/mms/tts/{lang}.tar.gz"
+    print(f"downloading {lang} from {url}")
+    urlretrieve(url, lang_fn)
+    Path(lang_dir).mkdir(parents=True, exist_ok=True)
+    import tarfile
+    file = tarfile.open(lang_fn)
+    print(f"extract all {lang} to {lang_dir}")
+    file.extractall(tgt_dir)
+    file.close()
+    print("Done")
+    return lang_dir
+
 
 class TextMapper(object):
     def __init__(self, vocab_file):
         self.symbols = [x.replace("\n", "") for x in open(vocab_file, encoding="utf-8").readlines()]
         self.SPACE_ID = self.symbols.index(" ")
         self._symbol_to_id = {s: i for i, s in enumerate(self.symbols)}
         self._id_to_symbol = {i: s for i, s in enumerate(self.symbols)}
```

### Comparing `ttsmms-0.6/ttsmms/attentions.py` & `ttsmms-0.7/ttsmms/attentions.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/ttsmms/commons.py` & `ttsmms-0.7/ttsmms/commons.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/ttsmms/data_utils.py` & `ttsmms-0.7/ttsmms/data_utils.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/ttsmms/losses.py` & `ttsmms-0.7/ttsmms/losses.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/ttsmms/mel_processing.py` & `ttsmms-0.7/ttsmms/mel_processing.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/ttsmms/models.py` & `ttsmms-0.7/ttsmms/models.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/ttsmms/modules.py` & `ttsmms-0.7/ttsmms/modules.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/ttsmms/preprocess.py` & `ttsmms-0.7/ttsmms/preprocess.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/ttsmms/text/__init__.py` & `ttsmms-0.7/ttsmms/text/__init__.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/ttsmms/text/cleaners.py` & `ttsmms-0.7/ttsmms/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/ttsmms/text/symbols.py` & `ttsmms-0.7/ttsmms/text/symbols.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/ttsmms/transforms.py` & `ttsmms-0.7/ttsmms/transforms.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/ttsmms/utils.py` & `ttsmms-0.7/ttsmms/utils.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.6/ttsmms.egg-info/PKG-INFO` & `ttsmms-0.7/ttsmms.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttsmms
-Version: 0.6
+Version: 0.7
 Summary: Text-to-speech with The Massively Multilingual Speech (MMS) project
 Home-page: https://github.com/wannaphong/ttsmms
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: MIT License
 Project-URL: Source, https://github.com/wannaphong/ttsmms
 Keywords: tts,NLP
@@ -39,30 +39,40 @@
 > pip install ttsmms
 
 
 ## Usage
 
 First, you need to download the model by
 
+```python
+from ttsmms import download
+
+dir_path = download("eng","./data") # lang_code, dir for save model
+```
+
+or download file by yourself
+
 **Linux/Mac**
 
+1. download
+
 > curl https://dl.fbaipublicfiles.com/mms/tts/lang_code.tar.gz --output lang_code.tar.gz
 
-and extract a tar ball archive.
+2. extract a tar ball archive.
 
 **Linux/Mac**
 
 > mkdir -p data && tar -xzf lang_code.tar.gz -C data/
 
 and use code in python :D
 
 ```python
 from ttsmms import TTS
 
-tts=TTS("model_dir_path") # your path dir that extract a tar ball archive
+tts=TTS(dir_path) # or "model_dir_path" your path dir that extract a tar ball archive
 wav=tts.synthesis("txt")
 # output:
 # {
 #    "x":array(wav array),
 #    "sampling_rate": 16000
 # }
```

