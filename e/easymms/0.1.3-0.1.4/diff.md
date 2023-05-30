# Comparing `tmp/easymms-0.1.3.tar.gz` & `tmp/easymms-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easymms-0.1.3.tar", last modified: Tue May 30 00:43:15 2023, max compression
+gzip compressed data, was "easymms-0.1.4.tar", last modified: Tue May 30 05:45:07 2023, max compression
```

## Comparing `easymms-0.1.3.tar` & `easymms-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:15.811291 easymms-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-05-30 00:43:08.000000 easymms-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-30 00:43:15.811291 easymms-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-30 00:43:08.000000 easymms-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:15.807291 easymms-0.1.3/easymms/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:15.807291 easymms-0.1.3/easymms/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/models/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/models/asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-30 00:43:08.000000 easymms-0.1.3/easymms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:15.811291 easymms-0.1.3/easymms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-30 00:43:15.000000 easymms-0.1.3/easymms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-30 00:43:15.000000 easymms-0.1.3/easymms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:43:15.000000 easymms-0.1.3/easymms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:43:15.000000 easymms-0.1.3/easymms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 00:43:15.000000 easymms-0.1.3/easymms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 00:43:15.000000 easymms-0.1.3/easymms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 00:43:15.811291 easymms-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-30 00:43:08.000000 easymms-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:15.807291 easymms-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 00:43:08.000000 easymms-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-30 00:43:08.000000 easymms-0.1.3/tests/test_asr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:07.891826 easymms-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-05-30 05:44:59.000000 easymms-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-30 05:45:07.891826 easymms-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-30 05:44:59.000000 easymms-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:07.887826 easymms-0.1.4/easymms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:07.887826 easymms-0.1.4/easymms/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/models/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/models/asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:07.891826 easymms-0.1.4/easymms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-30 05:45:07.000000 easymms-0.1.4/easymms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-30 05:45:07.000000 easymms-0.1.4/easymms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 05:45:07.000000 easymms-0.1.4/easymms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 05:45:07.000000 easymms-0.1.4/easymms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-30 05:45:07.000000 easymms-0.1.4/easymms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 05:45:07.000000 easymms-0.1.4/easymms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 05:45:07.891826 easymms-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-30 05:44:59.000000 easymms-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:07.887826 easymms-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:44:59.000000 easymms-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-30 05:44:59.000000 easymms-0.1.4/tests/test_asr.py
```

### Comparing `easymms-0.1.3/LICENSE` & `easymms-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easymms-0.1.3/PKG-INFO` & `easymms-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-Metadata-Version: 2.1
-Name: easymms
-Version: 0.1.3
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
+[![wheels](https://github.com/abdeladim-s/easymms/actions/workflows/wheels.yml/badge.svg)](https://github.com/abdeladim-s/easymms/actions/workflows/wheels.yml)
 <a target="_blank" href="https://colab.research.google.com/github/abdeladim-s/easymms/blob/main/examples/EasyMMS.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
+The [current MMS code](https://github.com/facebookresearch/fairseq/blob/main/examples/mms/asr/infer/mms_infer.py) is using subprocess to call another Python script, which is not very convenient to use, and might lead to several [issues](https://github.com/facebookresearch/fairseq/issues/5117).
+This package is created to address those problems and to wrap up the project in an API to easily integrate it with other projects. 
 <!-- TOC -->
 * [Installation](#installation)
 * [Quickstart](#quickstart)
   * [ASR](#asr)
   * [ASR with Alignment](#asr-with-alignment)
   * [TTS](#tts)
   * [LID](#lid)
@@ -48,14 +38,18 @@
 ```bash
 pip install easymms
 ```
 or from source 
 ```bash
 pip install git+https://github.com/abdeladim-s/easymms
 ```
+4. `Fairseq` has not included the `MMS` project yet in the released PYPI version, so until the next release, you will need to install `fairseq` from source:
+```shell
+pip uninstall fairseq && pip install git+https://github.com/facebookresearch/fairseq
+```
 
 # Quickstart
 
 ## ASR 
 You will need first to download the model weights, you can find and download all the supported models from [here](https://github.com/facebookresearch/fairseq/tree/main/examples/mms#asr).
```

### Comparing `easymms-0.1.3/README.md` & `easymms-0.1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,32 @@
+Metadata-Version: 2.1
+Name: easymms
+Version: 0.1.4
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
+[![wheels](https://github.com/abdeladim-s/easymms/actions/workflows/wheels.yml/badge.svg)](https://github.com/abdeladim-s/easymms/actions/workflows/wheels.yml)
 <a target="_blank" href="https://colab.research.google.com/github/abdeladim-s/easymms/blob/main/examples/EasyMMS.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
+The [current MMS code](https://github.com/facebookresearch/fairseq/blob/main/examples/mms/asr/infer/mms_infer.py) is using subprocess to call another Python script, which is not very convenient to use, and might lead to several [issues](https://github.com/facebookresearch/fairseq/issues/5117).
+This package is created to address those problems and to wrap up the project in an API to easily integrate it with other projects. 
 <!-- TOC -->
 * [Installation](#installation)
 * [Quickstart](#quickstart)
   * [ASR](#asr)
   * [ASR with Alignment](#asr-with-alignment)
   * [TTS](#tts)
   * [LID](#lid)
@@ -35,14 +51,18 @@
 ```bash
 pip install easymms
 ```
 or from source 
 ```bash
 pip install git+https://github.com/abdeladim-s/easymms
 ```
+4. `Fairseq` has not included the `MMS` project yet in the released PYPI version, so until the next release, you will need to install `fairseq` from source:
+```shell
+pip uninstall fairseq && pip install git+https://github.com/facebookresearch/fairseq
+```
 
 # Quickstart
 
 ## ASR 
 You will need first to download the model weights, you can find and download all the supported models from [here](https://github.com/facebookresearch/fairseq/tree/main/examples/mms#asr).
```

### Comparing `easymms-0.1.3/easymms/__init__.py` & `easymms-0.1.4/easymms/__init__.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.3/easymms/_logger.py` & `easymms-0.1.4/easymms/_logger.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.3/easymms/constants.py` & `easymms-0.1.4/easymms/constants.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.3/easymms/models/alignment.py` & `easymms-0.1.4/easymms/models/alignment.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.3/easymms/models/asr.py` & `easymms-0.1.4/easymms/models/asr.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.3/easymms/utils.py` & `easymms-0.1.4/easymms/utils.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.3/easymms.egg-info/PKG-INFO` & `easymms-0.1.4/easymms.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymms
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/easymms/
 Project-URL: Source, https://abdeladim-s.github.io/easymms/
 Project-URL: Tracker, https://abdeladim-s.github.io/easymms/issues
 Requires-Python: >=3.8
@@ -12,18 +12,21 @@
 License-File: LICENSE
 
 # EasyMMS
 
 A simple Python package to easily use [Meta's Massively Multilingual Speech (MMS) project](https://github.com/facebookresearch/fairseq/tree/main/examples/mms). 
 
 [![PyPi version](https://badgen.net/pypi/v/easymms)](https://pypi.org/project/easymms/)
+[![wheels](https://github.com/abdeladim-s/easymms/actions/workflows/wheels.yml/badge.svg)](https://github.com/abdeladim-s/easymms/actions/workflows/wheels.yml)
 <a target="_blank" href="https://colab.research.google.com/github/abdeladim-s/easymms/blob/main/examples/EasyMMS.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
+The [current MMS code](https://github.com/facebookresearch/fairseq/blob/main/examples/mms/asr/infer/mms_infer.py) is using subprocess to call another Python script, which is not very convenient to use, and might lead to several [issues](https://github.com/facebookresearch/fairseq/issues/5117).
+This package is created to address those problems and to wrap up the project in an API to easily integrate it with other projects. 
 <!-- TOC -->
 * [Installation](#installation)
 * [Quickstart](#quickstart)
   * [ASR](#asr)
   * [ASR with Alignment](#asr-with-alignment)
   * [TTS](#tts)
   * [LID](#lid)
@@ -48,14 +51,18 @@
 ```bash
 pip install easymms
 ```
 or from source 
 ```bash
 pip install git+https://github.com/abdeladim-s/easymms
 ```
+4. `Fairseq` has not included the `MMS` project yet in the released PYPI version, so until the next release, you will need to install `fairseq` from source:
+```shell
+pip uninstall fairseq && pip install git+https://github.com/facebookresearch/fairseq
+```
 
 # Quickstart
 
 ## ASR 
 You will need first to download the model weights, you can find and download all the supported models from [here](https://github.com/facebookresearch/fairseq/tree/main/examples/mms#asr).
```

### Comparing `easymms-0.1.3/setup.py` & `easymms-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 
 setup(
     name="easymms",
-    version="0.1.3",
+    version="0.1.4",
     author="Abdeladim Sadiki",
     description="A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project",
     long_description=long_description,
     ext_modules=[],
     zip_safe=False,
     python_requires=">=3.8",
     packages=find_packages('.'),
@@ -22,9 +22,9 @@
     long_description_content_type="text/markdown",
     license='MIT',
     project_urls={
         'Documentation': 'https://abdeladim-s.github.io/easymms/',
         'Source': 'https://abdeladim-s.github.io/easymms/',
         'Tracker': 'https://abdeladim-s.github.io/easymms/issues',
     },
-    install_requires=["fairseq~=0.12.2", "pydub~=0.25.1", "platformdirs==3.5.1", "editdistance", "sox", "dataclasses"],
+    install_requires=["fairseq~=0.12.2", "pydub~=0.25.1", "platformdirs==3.5.1", "editdistance", "sox", "dataclasses", "soundfile"],
 )
```

### Comparing `easymms-0.1.3/tests/test_asr.py` & `easymms-0.1.4/tests/test_asr.py`

 * *Files identical despite different names*

