# Comparing `tmp/audiotoolbox-0.65.tar.gz` & `tmp/audiotoolbox-0.65.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiotoolbox-0.65.tar", last modified: Mon May 29 06:14:31 2023, max compression
+gzip compressed data, was "audiotoolbox-0.65.1.tar", last modified: Tue May 30 01:01:03 2023, max compression
```

## Comparing `audiotoolbox-0.65.tar` & `audiotoolbox-0.65.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-29 06:14:31.578071 audiotoolbox-0.65/
--rw-r--r--   0 joerg     (1000) joerg     (1000)    35148 2021-07-02 20:55:17.000000 audiotoolbox-0.65/LICENSE
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     2059 2023-05-29 06:14:31.578071 audiotoolbox-0.65/PKG-INFO
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1537 2022-09-26 07:28:55.000000 audiotoolbox-0.65/README.md
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-29 06:14:31.574071 audiotoolbox-0.65/audiotoolbox.egg-info/
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     2059 2023-05-29 06:14:31.000000 audiotoolbox-0.65/audiotoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 joerg     (1000) joerg     (1000)      989 2023-05-29 06:14:31.000000 audiotoolbox-0.65/audiotoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 joerg     (1000) joerg     (1000)        1 2023-05-29 06:14:31.000000 audiotoolbox-0.65/audiotoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 joerg     (1000) joerg     (1000)       39 2023-05-29 06:14:31.000000 audiotoolbox-0.65/audiotoolbox.egg-info/requires.txt
--rw-rw-r--   0 joerg     (1000) joerg     (1000)       11 2023-05-29 06:14:31.000000 audiotoolbox-0.65/audiotoolbox.egg-info/top_level.txt
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-29 06:14:31.574071 audiotoolbox-0.65/audiotools/
--rw-rw-r--   0 joerg     (1000) joerg     (1000)      400 2023-05-29 06:07:14.000000 audiotoolbox-0.65/audiotools/__init__.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)    51410 2023-05-29 06:07:14.000000 audiotoolbox-0.65/audiotools/audiotools.py
--rw-r--r--   0 joerg     (1000) joerg     (1000)     1139 2021-07-02 20:55:19.000000 audiotoolbox-0.65/audiotools/auditory_filter.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1921 2023-05-29 06:07:14.000000 audiotoolbox-0.65/audiotools/din_iso_226.py
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-29 06:14:31.574071 audiotoolbox-0.65/audiotools/filter/
--rw-rw-r--   0 joerg     (1000) joerg     (1000)      278 2023-05-29 06:07:14.000000 audiotoolbox-0.65/audiotools/filter/__init__.py
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-29 06:14:31.574071 audiotoolbox-0.65/audiotools/filter/bank/
--rw-rw-r--   0 joerg     (1000) joerg     (1000)      127 2023-05-29 06:07:14.000000 audiotoolbox-0.65/audiotools/filter/bank/__init__.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1378 2023-05-29 06:07:14.000000 audiotoolbox-0.65/audiotools/filter/bank/default_banks.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     6441 2023-05-29 06:07:14.000000 audiotoolbox-0.65/audiotools/filter/bank/filterbank.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     3215 2023-05-29 06:07:14.000000 audiotoolbox-0.65/audiotools/filter/bank/octave_bank.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1121 2021-08-20 11:41:33.000000 audiotoolbox-0.65/audiotools/filter/brickwall_filt.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     4694 2023-05-02 01:30:47.000000 audiotoolbox-0.65/audiotools/filter/butterworth_filt.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     3658 2022-08-15 12:42:15.000000 audiotoolbox-0.65/audiotools/filter/filter.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     5414 2023-05-29 06:07:14.000000 audiotoolbox-0.65/audiotools/filter/gammatone_filt.py
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-29 06:14:31.574071 audiotoolbox-0.65/audiotools/oaudio/
--rw-rw-r--   0 joerg     (1000) joerg     (1000)       55 2021-08-20 11:41:33.000000 audiotoolbox-0.65/audiotools/oaudio/__init__.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     6154 2023-05-29 06:07:14.000000 audiotoolbox-0.65/audiotools/oaudio/base_signal.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     5914 2023-05-29 06:07:14.000000 audiotoolbox-0.65/audiotools/oaudio/freqdomain_signal.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)    26505 2023-05-29 06:07:14.000000 audiotoolbox-0.65/audiotools/oaudio/signal.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1132 2022-10-20 08:07:26.000000 audiotoolbox-0.65/audiotools/oaudio/stats.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     3684 2022-09-26 08:51:11.000000 audiotoolbox-0.65/audiotools/wav.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)      126 2022-08-15 12:42:15.000000 audiotoolbox-0.65/pyproject.toml
--rw-rw-r--   0 joerg     (1000) joerg     (1000)       38 2023-05-29 06:14:31.578071 audiotoolbox-0.65/setup.cfg
--rw-rw-r--   0 joerg     (1000) joerg     (1000)      881 2023-05-29 06:10:40.000000 audiotoolbox-0.65/setup.py
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-29 06:14:31.578071 audiotoolbox-0.65/tests/
--rw-rw-r--   0 joerg     (1000) joerg     (1000)    26895 2023-05-29 06:07:14.000000 audiotoolbox-0.65/tests/test_audiotools.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1301 2023-05-29 06:07:14.000000 audiotoolbox-0.65/tests/test_audiotools_stats.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     7468 2023-05-29 06:07:14.000000 audiotoolbox-0.65/tests/test_filter.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     5408 2023-05-29 06:07:14.000000 audiotoolbox-0.65/tests/test_filterbank.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     3553 2023-05-29 06:07:14.000000 audiotoolbox-0.65/tests/test_freqdomainsignal.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)    14681 2023-05-29 06:07:14.000000 audiotoolbox-0.65/tests/test_signal.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1427 2023-05-29 06:07:14.000000 audiotoolbox-0.65/tests/test_wav.py
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/
+-rw-r--r--   0 joerg     (1000) joerg     (1000)    35148 2021-07-02 20:55:17.000000 audiotoolbox-0.65.1/LICENSE
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     2154 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/PKG-INFO
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1630 2023-05-30 00:59:17.000000 audiotoolbox-0.65.1/README.md
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/audiotoolbox.egg-info/
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     2154 2023-05-30 01:01:03.000000 audiotoolbox-0.65.1/audiotoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)      989 2023-05-30 01:01:03.000000 audiotoolbox-0.65.1/audiotoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)        1 2023-05-30 01:01:03.000000 audiotoolbox-0.65.1/audiotoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)       39 2023-05-30 01:01:03.000000 audiotoolbox-0.65.1/audiotoolbox.egg-info/requires.txt
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)       11 2023-05-30 01:01:03.000000 audiotoolbox-0.65.1/audiotoolbox.egg-info/top_level.txt
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/audiotools/
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)      400 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/__init__.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)    51410 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/audiotools.py
+-rw-r--r--   0 joerg     (1000) joerg     (1000)     1139 2021-07-02 20:55:19.000000 audiotoolbox-0.65.1/audiotools/auditory_filter.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1921 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/din_iso_226.py
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/audiotools/filter/
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)      278 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/filter/__init__.py
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/audiotools/filter/bank/
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)      127 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/filter/bank/__init__.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1378 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/filter/bank/default_banks.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     7049 2023-05-30 00:59:17.000000 audiotoolbox-0.65.1/audiotools/filter/bank/filterbank.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     3215 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/filter/bank/octave_bank.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1121 2021-08-20 11:41:33.000000 audiotoolbox-0.65.1/audiotools/filter/brickwall_filt.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     4694 2023-05-02 01:30:47.000000 audiotoolbox-0.65.1/audiotools/filter/butterworth_filt.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     3658 2022-08-15 12:42:15.000000 audiotoolbox-0.65.1/audiotools/filter/filter.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     5415 2023-05-30 00:59:17.000000 audiotoolbox-0.65.1/audiotools/filter/gammatone_filt.py
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/audiotools/oaudio/
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)       55 2021-08-20 11:41:33.000000 audiotoolbox-0.65.1/audiotools/oaudio/__init__.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     6154 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/oaudio/base_signal.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     5914 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/oaudio/freqdomain_signal.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)    26505 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/oaudio/signal.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1132 2022-10-20 08:07:26.000000 audiotoolbox-0.65.1/audiotools/oaudio/stats.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     3684 2022-09-26 08:51:11.000000 audiotoolbox-0.65.1/audiotools/wav.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)      126 2022-08-15 12:42:15.000000 audiotoolbox-0.65.1/pyproject.toml
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)       38 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/setup.cfg
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)      883 2023-05-30 00:59:17.000000 audiotoolbox-0.65.1/setup.py
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/tests/
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)    26895 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/tests/test_audiotools.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1301 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/tests/test_audiotools_stats.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     7468 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/tests/test_filter.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     8403 2023-05-30 00:59:17.000000 audiotoolbox-0.65.1/tests/test_filterbank.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     3553 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/tests/test_freqdomainsignal.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)    14681 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/tests/test_signal.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1427 2023-05-29 06:52:39.000000 audiotoolbox-0.65.1/tests/test_wav.py
```

### Comparing `audiotoolbox-0.65/LICENSE` & `audiotoolbox-0.65.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/PKG-INFO` & `audiotoolbox-0.65.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiotoolbox
-Version: 0.65
+Version: 0.65.1
 Summary: Toolbox for generating and working with audio signals
 Home-page: https://jencke.github.io/audiotools/
 Author: Jörg Encke
 Author-email: joerg.encke@posteo.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Multimedia :: Sound/Audio
@@ -29,21 +29,14 @@
 ### From GitHub
  * Clone the repository: `git clone https://github.com/Jencke/audiotools.git`
  * Install the package: `pip install ./`
  * Optionally run the tests: `pytest`
 
 ## Documentation
 The package documentation can be found at: https://audiotools.readthedocs.io/en/master/
+However, it is a bit outdated and does not document all the features. Help would be highly appreciated
 
 ## Contributions
-The Project is happy about any kind of contribution. If you find bugs,
-think the documentation could be improved, have comments or ideas,
-just open a ticket within the issue tracker
-https://github.com/Jencke/audiotools/issues or contact me via email.
-If you implement new features, I'm happy to receive merge requests or
-code-snippets.
+The Project is happy about any contribution. If you find bugs, think the documentation could be improved, or have comments or ideas, open a ticket within the issue tracker https://github.com/Jencke/audiotools/issues or contact me via email. If you implement new features, I'm happy to receive merge requests or code-snippets.
 
 ## Acknowledgments
-This software package was developed during my PHD in the group of
-Prof. Werner Hemmert at the Technical University of Munich and further
-developed during my time as a post-doc in the Group of Prof. Mathias
-Dietz at the University of Oldenburg.
+This software package was developed during my PHD in the group of Prof. Werner Hemmert at the Technical University of Munich and further developed during my time as a post-doc in the Group of Prof. Mathias Dietz at the University of Oldenburg.
```

### Comparing `audiotoolbox-0.65/README.md` & `audiotoolbox-0.65.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,14 @@
 ### From GitHub
  * Clone the repository: `git clone https://github.com/Jencke/audiotools.git`
  * Install the package: `pip install ./`
  * Optionally run the tests: `pytest`
 
 ## Documentation
 The package documentation can be found at: https://audiotools.readthedocs.io/en/master/
+However, it is a bit outdated and does not document all the features. Help would be highly appreciated
 
 ## Contributions
-The Project is happy about any kind of contribution. If you find bugs,
-think the documentation could be improved, have comments or ideas,
-just open a ticket within the issue tracker
-https://github.com/Jencke/audiotools/issues or contact me via email.
-If you implement new features, I'm happy to receive merge requests or
-code-snippets.
+The Project is happy about any contribution. If you find bugs, think the documentation could be improved, or have comments or ideas, open a ticket within the issue tracker https://github.com/Jencke/audiotools/issues or contact me via email. If you implement new features, I'm happy to receive merge requests or code-snippets.
 
 ## Acknowledgments
-This software package was developed during my PHD in the group of
-Prof. Werner Hemmert at the Technical University of Munich and further
-developed during my time as a post-doc in the Group of Prof. Mathias
-Dietz at the University of Oldenburg.
+This software package was developed during my PHD in the group of Prof. Werner Hemmert at the Technical University of Munich and further developed during my time as a post-doc in the Group of Prof. Mathias Dietz at the University of Oldenburg.
```

### Comparing `audiotoolbox-0.65/audiotoolbox.egg-info/PKG-INFO` & `audiotoolbox-0.65.1/audiotoolbox.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiotoolbox
-Version: 0.65
+Version: 0.65.1
 Summary: Toolbox for generating and working with audio signals
 Home-page: https://jencke.github.io/audiotools/
 Author: Jörg Encke
 Author-email: joerg.encke@posteo.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Multimedia :: Sound/Audio
@@ -29,21 +29,14 @@
 ### From GitHub
  * Clone the repository: `git clone https://github.com/Jencke/audiotools.git`
  * Install the package: `pip install ./`
  * Optionally run the tests: `pytest`
 
 ## Documentation
 The package documentation can be found at: https://audiotools.readthedocs.io/en/master/
+However, it is a bit outdated and does not document all the features. Help would be highly appreciated
 
 ## Contributions
-The Project is happy about any kind of contribution. If you find bugs,
-think the documentation could be improved, have comments or ideas,
-just open a ticket within the issue tracker
-https://github.com/Jencke/audiotools/issues or contact me via email.
-If you implement new features, I'm happy to receive merge requests or
-code-snippets.
+The Project is happy about any contribution. If you find bugs, think the documentation could be improved, or have comments or ideas, open a ticket within the issue tracker https://github.com/Jencke/audiotools/issues or contact me via email. If you implement new features, I'm happy to receive merge requests or code-snippets.
 
 ## Acknowledgments
-This software package was developed during my PHD in the group of
-Prof. Werner Hemmert at the Technical University of Munich and further
-developed during my time as a post-doc in the Group of Prof. Mathias
-Dietz at the University of Oldenburg.
+This software package was developed during my PHD in the group of Prof. Werner Hemmert at the Technical University of Munich and further developed during my time as a post-doc in the Group of Prof. Mathias Dietz at the University of Oldenburg.
```

### Comparing `audiotoolbox-0.65/audiotoolbox.egg-info/SOURCES.txt` & `audiotoolbox-0.65.1/audiotoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/audiotools/audiotools.py` & `audiotoolbox-0.65.1/audiotools/audiotools.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/audiotools/auditory_filter.py` & `audiotoolbox-0.65.1/audiotools/auditory_filter.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/audiotools/din_iso_226.py` & `audiotoolbox-0.65.1/audiotools/din_iso_226.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/audiotools/filter/bank/default_banks.py` & `audiotoolbox-0.65.1/audiotools/filter/bank/default_banks.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/audiotools/filter/bank/filterbank.py` & `audiotoolbox-0.65.1/audiotools/filter/bank/filterbank.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from typing import Literal
+from copy import deepcopy
+
 import numpy as np
+from numpy.typing import ArrayLike
 
-from .. import gammatone_filt as gamma
-from .. import butterworth_filt as butter
+from .. import gammatone_filt as gamma, butterworth_filt as butter
 from .. import brickwall_filt as brick
 from ... import audiotools as audio
-from typing import Literal
-from numpy.typing import ArrayLike
 
 
 class FilterBank(object):
     '''Parent Class for all filterbanks
 
     Parameters
     ----------
@@ -26,44 +27,59 @@
         single value in which case this value is used for all filters.
 
     '''
     def __init__(self, fc, bw, fs, **kwargs):
         self.fc = np.asarray([fc]).flatten()
         self.bw = np.asarray([bw]).flatten()
         self.fs = fs
-        self.n_filters = len(self.fc)
+        self.params = dict()
 
         if self.fc.shape != self.bw.shape:
             raise Exception(
                 'Length of center frequencies must equal length of bandwidths')
 
+        self._update_params(**kwargs)
 
-def _update_params(param, n_val, **kwargs):
-    ''' Used to update the parameter dict
-    '''
-    for k, v in kwargs.items():
-        if k in param:
+    @property
+    def n_filters(self):
+        return len(self.fc)
+
+    def _update_params(self, **kwargs):
+        ''' Used to update the parameter dict
+        '''
+        n_val = self.n_filters
+        for k, v in kwargs.items():
             if np.ndim(v):
                 if len(v) == n_val:
-                    param[k] = v
+                    self.params[k] = np.asarray(v)
                 else:
                     raise Exception(f'Size missmatch in parameter \'{k}\'')
             else:
-                param[k] = n_val * [v]
-    return param
+                self.params[k] = np.asarray(n_val * [v])
+
+    def __len__(self):
+        return self.n_filters
+
+    def __getitem__(self, i):
+        bank = deepcopy(self)
+        bank.bw = self.bw[i]
+        bank.fc = self.fc[i]
+        bank.fs = self.fs
+        for k, v in self.params.items():
+            bank.params[k] = v[i]
+        return bank
 
 
 class ButterworthBank(FilterBank):
     def __init__(self, fc, bw, fs, **kwargs):
         super().__init__(fc, bw, fs, **kwargs)
 
         # set default parameters
-        self.params = {'order': self.n_filters * [2]}
-        # update defaults with predefined parameters
-        self.params = _update_params(self.params, self.n_filters, **kwargs)
+        if 'order' not in self.params.keys():
+            self._update_params(order=2)
 
         # Calculate filter coefficents
         self.coefficents = np.zeros((np.max(self.params['order']), 6,
                                      self.n_filters))
         for i_filt in range(self.n_filters):
             # extract parameter set for current filter
             current_params = {k: v[i_filt] for k, v in self.params.items()}
@@ -83,24 +99,30 @@
             order = self.params['order'][i_filt]
             # sos has to be C-contigous
             sos = self.coefficents[:order, :, i_filt].copy(order='C')
             out, states = butter.apply_sos(signal, sos)
             out_sig.T[i_filt] = out.T
         return out_sig
 
+    def __getitem__(self, i):
+        bank = super().__getitem__(i)
+        bank.coefficents = self.coefficents[:, :, i]
+        return bank
+
 
 class GammaToneBank(FilterBank):
     def __init__(self, fc, bw, fs, **kwargs):
         FilterBank.__init__(self, fc, bw, fs, **kwargs)
 
+        self._update_params(**kwargs)
         # set default parameters
-        self.params = {'order': self.n_filters * [4],
-                       'attenuation_db': self.n_filters * ['erb']}
-        # update defaults with predefined parameters
-        self.params = _update_params(self.params, self.n_filters, **kwargs)
+        if 'order' not in self.params.keys():
+            self._update_params(order=4)
+        if 'attenuation_db' not in self.params.keys():
+            self._update_params(attenuation_db='erb')
 
         # Calculate filter coefficents
         self.coefficents = np.zeros([4, self.n_filters], complex)
 
         for i_filt in range(self.n_filters):
             current_params = {k: v[i_filt]
                               for k, v in self.params.items()}
@@ -124,14 +146,19 @@
             out_sig.T[i_filt] = out.T
 
         # squeeze to leave dimensions unchanged if n_filters == 1
         if out_sig.shape[-1] == 1:
             out_sig = out_sig.squeeze(-1)
         return out_sig
 
+    def __getitem__(self, i):
+        bank = super().__getitem__(i)
+        bank.coefficents = self.coefficents[:, i]
+        return bank
+
 
 class BrickBank(FilterBank):
     def __init__(self, fc, bw, fs):
         FilterBank.__init__(self, fc, bw, fs)
 
     def filt(self, signal):
         n_ch_out = (*signal.shape[1:], self.n_filters)
```

### Comparing `audiotoolbox-0.65/audiotools/filter/bank/octave_bank.py` & `audiotoolbox-0.65.1/audiotools/filter/bank/octave_bank.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/audiotools/filter/brickwall_filt.py` & `audiotoolbox-0.65.1/audiotools/filter/brickwall_filt.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/audiotools/filter/butterworth_filt.py` & `audiotoolbox-0.65.1/audiotools/filter/butterworth_filt.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/audiotools/filter/filter.py` & `audiotoolbox-0.65.1/audiotools/filter/filter.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/audiotools/filter/gammatone_filt.py` & `audiotoolbox-0.65.1/audiotools/filter/gammatone_filt.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 def erb_to_3db(
         equivalent_rect_bw: float,
         order: int
 ) -> float:
     """ERB to -3db bw conversion for gammatone filter of given order."""
     c = 2 * np.sqrt(2**(1 / order) - 1)
     alpha = ((np.pi * np.math.factorial(2 * order - 2)
-              * 2**(2 - 2 * order))
+              * 2.**(2 - 2 * order))
              / np.math.factorial(order - 1)**2)
     bw = c / alpha * equivalent_rect_bw
     return bw
 
 
 def gammatonefos_apply(signal, b, a, order, states=None):
     """Process an input signal by applying the filter `order` times.
```

### Comparing `audiotoolbox-0.65/audiotools/oaudio/base_signal.py` & `audiotoolbox-0.65.1/audiotools/oaudio/base_signal.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/audiotools/oaudio/freqdomain_signal.py` & `audiotoolbox-0.65.1/audiotools/oaudio/freqdomain_signal.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/audiotools/oaudio/signal.py` & `audiotoolbox-0.65.1/audiotools/oaudio/signal.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/audiotools/oaudio/stats.py` & `audiotoolbox-0.65.1/audiotools/oaudio/stats.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/audiotools/wav.py` & `audiotoolbox-0.65.1/audiotools/wav.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/setup.py` & `audiotoolbox-0.65.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="audiotoolbox",
-    version="0.65",
+    version="0.65.1",
     author="Jörg Encke",
     author_email="joerg.encke@posteo.de",
     description="Toolbox for generating and working with audio signals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://jencke.github.io/audiotools/",
     python_requires='>=3',
```

### Comparing `audiotoolbox-0.65/tests/test_audiotools.py` & `audiotoolbox-0.65.1/tests/test_audiotools.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/tests/test_audiotools_stats.py` & `audiotoolbox-0.65.1/tests/test_audiotools_stats.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/tests/test_filter.py` & `audiotoolbox-0.65.1/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/tests/test_filterbank.py` & `audiotoolbox-0.65.1/tests/test_filterbank.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,21 +3,97 @@
 import audiotools as audio
 import audiotools.filter.bank.filterbank as bank
 from audiotools.filter import gammatone_filt
 from audiotools.filter import butterworth_filt
 import numpy.testing as testing
 from audiotools.filter.bank import create_filterbank
 from audiotools.filter.bank import auditory_gamma_bank, octave_bank
+from audiotools.filter.bank.filterbank import FilterBank, ButterworthBank
+from audiotools.filter.bank.filterbank import GammaToneBank
+
+
+
+def test_base_signal():
+    bank = FilterBank([500, 200], [10, 2], 48000, myparam=3)
+    assert len(bank) == 2
+    assert np.all(bank.params['myparam'] == [3, 3])
+
+    assert isinstance(bank[0], FilterBank)
+    assert bank[0].bw == 10
+    assert bank[1].fc == 200
+    assert bank[0].fs == bank.fs
+    assert bank[0].params['myparam'] == 3
+
+    bank = FilterBank(np.random.random(10),
+                      np.random.random(10), 48000,
+                      myparam1=np.random.random(10),
+                      myparam2=np.random.random(10))
+    idx_vec = [np.random.randint(0, 10, 3) for i in range(3)]
+
+    for i in idx_vec:
+        sub = bank[i]
+        np.testing.assert_equal(sub.bw, bank.bw[i])
+        np.testing.assert_equal(sub.fs, bank.fs)
+        np.testing.assert_equal(sub.fc, bank.fc[i])
+        np.testing.assert_equal(sub.params['myparam1'],
+                                bank.params['myparam1'][i])
+        np.testing.assert_equal(sub.params['myparam2'],
+                                bank.params['myparam2'][i])
+
+
+def test_sub_butterbank():
+    bank = create_filterbank(fc=np.random.randint(500, 1000, 10),
+                             bw=np.random.randint(10, 50, 10),
+                             fs=48000,
+                             filter_type='butter',
+                             order=np.random.randint(1, 10, 10))
+    idx_vec = [np.random.randint(0, 10, 3) for i in range(3)]
+
+    sig = audio.Signal(1, 1, 48000).add_noise()
+    main_out = bank.filt(sig)
+    for i in idx_vec:
+        sub = bank[i]
+        assert isinstance(sub, ButterworthBank)
+        np.testing.assert_equal(sub.bw, bank.bw[i])
+        np.testing.assert_equal(sub.fs, bank.fs)
+        np.testing.assert_equal(sub.fc, bank.fc[i])
+        np.testing.assert_equal(sub.params['order'],
+                                bank.params['order'][i])
+        sub_out = sub.filt(sig)
+        np.testing.assert_equal(main_out.ch[i], sub_out)
+
+
+def test_sub_gamma():
+    bank = create_filterbank(fc=np.random.randint(500, 1000, 10),
+                             bw=np.random.randint(10, 50, 10),
+                             fs=48000,
+                             filter_type='gammatone',
+                             order=np.random.randint(1, 10, 10))
+    idx_vec = [np.random.randint(0, 10, 3) for i in range(3)]
+
+    sig = audio.Signal(1, 1, 48000).add_noise()
+    main_out = bank.filt(sig)
+    for i in idx_vec:
+        sub = bank[i]
+        assert isinstance(sub, GammaToneBank)
+        np.testing.assert_equal(sub.bw, bank.bw[i])
+        np.testing.assert_equal(sub.fs, bank.fs)
+        np.testing.assert_equal(sub.fc, bank.fc[i])
+        np.testing.assert_equal(sub.params['order'],
+                                bank.params['order'][i])
+        sub_out = sub.filt(sig)
+        np.testing.assert_equal(main_out.ch[i], sub_out)
 
 
 def test_create_filterbank():
     fc = [100, 200]
     bw = [10, 20]
     butter = create_filterbank(fc, bw, "butter", 48000)
     assert isinstance(butter, bank.ButterworthBank)
+    assert butter.n_filters == 2
 
     gamma = create_filterbank(fc, bw, "gammatone", 48000)
     assert isinstance(gamma, bank.GammaToneBank)
 
 
 def test_butterworth():
     fc = [100, 200, 5000]
```

### Comparing `audiotoolbox-0.65/tests/test_freqdomainsignal.py` & `audiotoolbox-0.65.1/tests/test_freqdomainsignal.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/tests/test_signal.py` & `audiotoolbox-0.65.1/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65/tests/test_wav.py` & `audiotoolbox-0.65.1/tests/test_wav.py`

 * *Files identical despite different names*

