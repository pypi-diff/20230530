# Comparing `tmp/bertopic-0.9.3.tar.gz` & `tmp/bertopic-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\bertopic-0.9.3.tar", last modified: Sun Oct 17 06:42:10 2021, max compression
+gzip compressed data, was "bertopic-0.9.4.tar", last modified: Tue Dec 14 11:13:55 2021, max compression
```

## Comparing `bertopic-0.9.3.tar` & `bertopic-0.9.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2021-10-17 06:42:10.000000 bertopic-0.9.3/
--rw-rw-rw-   0        0        0    14486 2021-10-17 06:42:10.000000 bertopic-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0    11090 2021-10-17 06:41:37.000000 bertopic-0.9.3/README.md
-drwxrwxrwx   0        0        0        0 2021-10-17 06:42:09.000000 bertopic-0.9.3/bertopic/
--rw-rw-rw-   0        0        0      101 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/__init__.py
--rw-rw-rw-   0        0        0    86805 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/_bertopic.py
--rw-rw-rw-   0        0        0     2355 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/_ctfidf.py
--rw-rw-rw-   0        0        0     2266 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/_mmr.py
--rw-rw-rw-   0        0        0     3191 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/_utils.py
-drwxrwxrwx   0        0        0        0 2021-10-17 06:42:09.000000 bertopic-0.9.3/bertopic/backend/
--rw-rw-rw-   0        0        0      184 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/backend/__init__.py
--rw-rw-rw-   0        0        0     2457 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/backend/_base.py
--rw-rw-rw-   0        0        0     3061 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/backend/_flair.py
--rw-rw-rw-   0        0        0     2469 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/backend/_gensim.py
--rw-rw-rw-   0        0        0     2306 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/backend/_sentencetransformers.py
--rw-rw-rw-   0        0        0     3464 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/backend/_spacy.py
--rw-rw-rw-   0        0        0     1781 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/backend/_use.py
--rw-rw-rw-   0        0        0     3923 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/backend/_utils.py
--rw-rw-rw-   0        0        0     1672 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/backend/_word_doc.py
-drwxrwxrwx   0        0        0        0 2021-10-17 06:42:09.000000 bertopic-0.9.3/bertopic/plotting/
--rw-rw-rw-   0        0        0      636 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/plotting/__init__.py
--rw-rw-rw-   0        0        0     3207 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/plotting/_barchart.py
--rw-rw-rw-   0        0        0     3416 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/plotting/_distribution.py
--rw-rw-rw-   0        0        0     4299 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/plotting/_heatmap.py
--rw-rw-rw-   0        0        0     3944 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/plotting/_hierarchy.py
--rw-rw-rw-   0        0        0     4188 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/plotting/_term_rank.py
--rw-rw-rw-   0        0        0     5517 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/plotting/_topics.py
--rw-rw-rw-   0        0        0     4019 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/plotting/_topics_over_time.py
--rw-rw-rw-   0        0        0     4207 2021-10-17 06:41:37.000000 bertopic-0.9.3/bertopic/plotting/_topics_per_class.py
-drwxrwxrwx   0        0        0        0 2021-10-17 06:42:09.000000 bertopic-0.9.3/bertopic.egg-info/
--rw-rw-rw-   0        0        0    14486 2021-10-17 06:42:08.000000 bertopic-0.9.3/bertopic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      989 2021-10-17 06:42:08.000000 bertopic-0.9.3/bertopic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-17 06:42:08.000000 bertopic-0.9.3/bertopic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      636 2021-10-17 06:42:08.000000 bertopic-0.9.3/bertopic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2021-10-17 06:42:08.000000 bertopic-0.9.3/bertopic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-10-17 06:42:10.000000 bertopic-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0     2680 2021-10-17 06:41:37.000000 bertopic-0.9.3/setup.py
-drwxrwxrwx   0        0        0        0 2021-10-17 06:42:10.000000 bertopic-0.9.3/tests/
--rw-rw-rw-   0        0        0        0 2021-10-17 06:41:37.000000 bertopic-0.9.3/tests/__init__.py
--rw-rw-rw-   0        0        0      241 2021-10-17 06:41:37.000000 bertopic-0.9.3/tests/conftest.py
--rw-rw-rw-   0        0        0     2679 2021-10-17 06:41:37.000000 bertopic-0.9.3/tests/test_bertopic.py
--rw-rw-rw-   0        0        0    11364 2021-10-17 06:41:37.000000 bertopic-0.9.3/tests/test_models.py
--rw-rw-rw-   0        0        0     1133 2021-10-17 06:41:37.000000 bertopic-0.9.3/tests/test_other.py
--rw-rw-rw-   0        0        0     5088 2021-10-17 06:41:37.000000 bertopic-0.9.3/tests/test_topic_representation.py
--rw-rw-rw-   0        0        0     1337 2021-10-17 06:41:37.000000 bertopic-0.9.3/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2021-12-14 11:13:55.616573 bertopic-0.9.4/
+-rw-rw-rw-   0        0        0    14534 2021-12-14 11:13:55.616573 bertopic-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11138 2021-12-14 11:13:21.000000 bertopic-0.9.4/README.md
+drwxrwxrwx   0        0        0        0 2021-12-14 11:13:55.447575 bertopic-0.9.4/bertopic/
+-rw-rw-rw-   0        0        0      101 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/__init__.py
+-rw-rw-rw-   0        0        0    87224 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/_bertopic.py
+-rw-rw-rw-   0        0        0     2713 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/_ctfidf.py
+-rw-rw-rw-   0        0        0     2266 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/_mmr.py
+-rw-rw-rw-   0        0        0     3191 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/_utils.py
+drwxrwxrwx   0        0        0        0 2021-12-14 11:13:55.520616 bertopic-0.9.4/bertopic/backend/
+-rw-rw-rw-   0        0        0      184 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/backend/__init__.py
+-rw-rw-rw-   0        0        0     2457 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/backend/_base.py
+-rw-rw-rw-   0        0        0     3061 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/backend/_flair.py
+-rw-rw-rw-   0        0        0     2469 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/backend/_gensim.py
+-rw-rw-rw-   0        0        0     2306 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/backend/_sentencetransformers.py
+-rw-rw-rw-   0        0        0     3464 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/backend/_spacy.py
+-rw-rw-rw-   0        0        0     1781 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/backend/_use.py
+-rw-rw-rw-   0        0        0     3923 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/backend/_utils.py
+-rw-rw-rw-   0        0        0     1672 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/backend/_word_doc.py
+drwxrwxrwx   0        0        0        0 2021-12-14 11:13:55.584623 bertopic-0.9.4/bertopic/plotting/
+-rw-rw-rw-   0        0        0      636 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/plotting/__init__.py
+-rw-rw-rw-   0        0        0     3430 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/plotting/_barchart.py
+-rw-rw-rw-   0        0        0     3423 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/plotting/_distribution.py
+-rw-rw-rw-   0        0        0     4306 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/plotting/_heatmap.py
+-rw-rw-rw-   0        0        0     4424 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/plotting/_hierarchy.py
+-rw-rw-rw-   0        0        0     4202 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/plotting/_term_rank.py
+-rw-rw-rw-   0        0        0     5524 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/plotting/_topics.py
+-rw-rw-rw-   0        0        0     4026 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/plotting/_topics_over_time.py
+-rw-rw-rw-   0        0        0     4214 2021-12-14 11:13:21.000000 bertopic-0.9.4/bertopic/plotting/_topics_per_class.py
+drwxrwxrwx   0        0        0        0 2021-12-14 11:13:55.472575 bertopic-0.9.4/bertopic.egg-info/
+-rw-rw-rw-   0        0        0    14534 2021-12-14 11:13:55.000000 bertopic-0.9.4/bertopic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      989 2021-12-14 11:13:55.000000 bertopic-0.9.4/bertopic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-12-14 11:13:55.000000 bertopic-0.9.4/bertopic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      628 2021-12-14 11:13:55.000000 bertopic-0.9.4/bertopic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2021-12-14 11:13:55.000000 bertopic-0.9.4/bertopic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-12-14 11:13:55.616573 bertopic-0.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     2672 2021-12-14 11:13:21.000000 bertopic-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2021-12-14 11:13:55.614577 bertopic-0.9.4/tests/
+-rw-rw-rw-   0        0        0        0 2021-12-14 11:13:21.000000 bertopic-0.9.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      241 2021-12-14 11:13:21.000000 bertopic-0.9.4/tests/conftest.py
+-rw-rw-rw-   0        0        0     2679 2021-12-14 11:13:21.000000 bertopic-0.9.4/tests/test_bertopic.py
+-rw-rw-rw-   0        0        0    11302 2021-12-14 11:13:21.000000 bertopic-0.9.4/tests/test_models.py
+-rw-rw-rw-   0        0        0     1133 2021-12-14 11:13:21.000000 bertopic-0.9.4/tests/test_other.py
+-rw-rw-rw-   0        0        0     5088 2021-12-14 11:13:21.000000 bertopic-0.9.4/tests/test_topic_representation.py
+-rw-rw-rw-   0        0        0     1337 2021-12-14 11:13:21.000000 bertopic-0.9.4/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bertopic-0.9.3/PKG-INFO` & `bertopic-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: bertopic
-Version: 0.9.3
+Version: 0.9.4
 Summary: BERTopic performs topic Modeling with state-of-the-art transformer models.
 Home-page: https://github.com/MaartenGr/BERTopic
 Author: Maarten P. Grootendorst
 Author-email: maartengrootendorst@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://maartengr.github.io/BERTopic/
 Project-URL: Source Code, https://github.com/MaartenGr/BERTopic/
 Project-URL: Issue Tracker, https://github.com/MaartenGr/BERTopic/issues
-Description: [![PyPI - Python](https://img.shields.io/badge/python-v3.6+-blue.svg)](https://pypi.org/project/bertopic/)
+Description: [![PyPI - Python](https://img.shields.io/badge/python-v3.7+-blue.svg)](https://pypi.org/project/bertopic/)
         [![Build](https://img.shields.io/github/workflow/status/MaartenGr/BERTopic/Code%20Checks/master)](https://pypi.org/project/bertopic/)
         [![docs](https://img.shields.io/badge/docs-Passing-green.svg)](https://maartengr.github.io/BERTopic/)
         [![PyPI - PyPi](https://img.shields.io/pypi/v/BERTopic)](https://pypi.org/project/bertopic/)
         [![PyPI - License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/MaartenGr/VLAC/blob/master/LICENSE)
         [![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.4381785-blue)](https://doi.org/10.5281/zenodo.4381785)
         
         # BERTopic
         
         <img src="images/logo.png" width="35%" height="35%" align="right" />
         
         BERTopic is a topic modeling technique that leverages ðŸ¤— transformers and c-TF-IDF to create dense clusters
         allowing for easily interpretable topics whilst keeping important words in the topic descriptions.
         
         BERTopic supports 
-        [**guided**](https://maartengr.github.io/BERTopic/tutorial/guided/guided.html), 
-        (semi-) [**supervised**](https://maartengr.github.io/BERTopic/tutorial/supervised/supervised.html), 
-        and [**dynamic**](https://maartengr.github.io/BERTopic/tutorial/topicsovertime/topicsovertime.html) topic modeling. It even supports visualizations similar to LDAvis!
+        [**guided**](https://maartengr.github.io/BERTopic/getting_started/guided/guided.html), 
+        (semi-) [**supervised**](https://maartengr.github.io/BERTopic/getting_started/supervised/supervised.html), 
+        and [**dynamic**](https://maartengr.github.io/BERTopic/getting_started/topicsovertime/topicsovertime.html) topic modeling. It even supports visualizations similar to LDAvis!
         
         Corresponding medium posts can be found [here](https://towardsdatascience.com/topic-modeling-with-bert-779f7db187e6?source=friends_link&sk=0b5a470c006d1842ad4c8a3057063a99) 
         and [here](https://towardsdatascience.com/interactive-topic-modeling-with-bertopic-1ea55e7d73d8?sk=03c2168e9e74b6bda2a1f3ed953427e4).
         
         ## Installation
         
         Installation, with sentence-transformers, can be done using [pypi](https://pypi.org/project/bertopic/):
@@ -61,27 +61,27 @@
         | Advanced Customization in BERTopic  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ClTYut039t-LDtlcd-oQAdXWgcsSGTw9?usp=sharing) |
         | (semi-)Supervised Topic Modeling with BERTopic  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1bxizKzv5vfxJEB29sntU__ZC7PBSIPaQ?usp=sharing)  |
         | Dynamic Topic Modeling with Trump's Tweets  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1un8ooI-7ZNlRoK0maVkYhmNRl0XGK88f?usp=sharing)  |
         | Topic Modeling arXiv Abstracts | [![Kaggle](https://img.shields.io/static/v1?style=for-the-badge&message=Kaggle&color=222222&logo=Kaggle&logoColor=20BEFF&label=)](https://www.kaggle.com/maartengr/topic-modeling-arxiv-abstract-with-bertopic) |
         
         
         ## Quick Start
-        We start by extracting topics from the well-known 20 newsgroups dataset which is comprised of english documents:
+        We start by extracting topics from the well-known 20 newsgroups dataset containing English documents:
         
         ```python
         from bertopic import BERTopic
         from sklearn.datasets import fetch_20newsgroups
          
         docs = fetch_20newsgroups(subset='all',  remove=('headers', 'footers', 'quotes'))['data']
         
         topic_model = BERTopic()
         topics, probs = topic_model.fit_transform(docs)
         ```
         
-        After generating topics, we can access the frequent topics that were generated:
+        After generating topics and their probabilities, we can access the frequent topics that were generated:
         
         ```python
         >>> topic_model.get_topic_info()
         
         Topic	Count	Name
         -1	4630	-1_can_your_will_any
         0	693	49_windows_drive_dos_file
@@ -130,15 +130,15 @@
         topic_model.visualize_barchart()
         ``` 
         
         <img src="images/topics.png" width="70%" height="70%" align="center" />
         
         
         Find all possible visualizations with interactive examples in the documentation 
-        [here](https://maartengr.github.io/BERTopic/tutorial/visualization/visualization.html). 
+        [here](https://maartengr.github.io/BERTopic/getting_started/visualization/visualization.html). 
         
         ## Embedding Models
         BERTopic supports many embedding models that can be used to embed the documents and words:
         * Sentence-Transformers
         * Flair
         * Spacy
         * Gensim
@@ -158,15 +158,15 @@
         ```python
         from flair.embeddings import TransformerDocumentEmbeddings
         
         roberta = TransformerDocumentEmbeddings('roberta-base')
         topic_model = BERTopic(embedding_model=roberta)
         ```
         
-        Click [here](https://maartengr.github.io/BERTopic/tutorial/embeddings/embeddings.html) 
+        Click [here](https://maartengr.github.io/BERTopic/getting_started/embeddings/embeddings.html) 
         for a full overview of all supported embedding models. 
         
         ## Dynamic Topic Modeling
         Dynamic topic modeling (DTM) is a collection of techniques aimed at analyzing the evolution of topics 
         over time. These methods allow you to understand how a topic is represented over time. 
         Here, we will be using all of Donald Trump's tweet to see how he talked over certain topics over time: 
         
@@ -245,15 +245,15 @@
         
         ```bibtex
         @misc{grootendorst2020bertopic,
           author       = {Maarten Grootendorst},
           title        = {BERTopic: Leveraging BERT and c-TF-IDF to create easily interpretable topics.},
           year         = 2020,
           publisher    = {Zenodo},
-          version      = {v0.9.2},
+          version      = {v0.9.4},
           doi          = {10.5281/zenodo.4381785},
           url          = {https://doi.org/10.5281/zenodo.4381785}
         }
         ```
         
 Keywords: nlp bert topic modeling embeddings
 Platform: UNKNOWN
@@ -264,18 +264,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: docs
 Provides-Extra: dev
-Provides-Extra: spacy
 Provides-Extra: flair
-Provides-Extra: test
-Provides-Extra: gensim
+Provides-Extra: spacy
 Provides-Extra: use
-Provides-Extra: docs
+Provides-Extra: gensim
```

### Comparing `bertopic-0.9.3/README.md` & `bertopic-0.9.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-[![PyPI - Python](https://img.shields.io/badge/python-v3.6+-blue.svg)](https://pypi.org/project/bertopic/)
+[![PyPI - Python](https://img.shields.io/badge/python-v3.7+-blue.svg)](https://pypi.org/project/bertopic/)
 [![Build](https://img.shields.io/github/workflow/status/MaartenGr/BERTopic/Code%20Checks/master)](https://pypi.org/project/bertopic/)
 [![docs](https://img.shields.io/badge/docs-Passing-green.svg)](https://maartengr.github.io/BERTopic/)
 [![PyPI - PyPi](https://img.shields.io/pypi/v/BERTopic)](https://pypi.org/project/bertopic/)
 [![PyPI - License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/MaartenGr/VLAC/blob/master/LICENSE)
 [![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.4381785-blue)](https://doi.org/10.5281/zenodo.4381785)
 
 # BERTopic
 
 <img src="images/logo.png" width="35%" height="35%" align="right" />
 
 BERTopic is a topic modeling technique that leverages 🤗 transformers and c-TF-IDF to create dense clusters
 allowing for easily interpretable topics whilst keeping important words in the topic descriptions.
 
 BERTopic supports 
-[**guided**](https://maartengr.github.io/BERTopic/tutorial/guided/guided.html), 
-(semi-) [**supervised**](https://maartengr.github.io/BERTopic/tutorial/supervised/supervised.html), 
-and [**dynamic**](https://maartengr.github.io/BERTopic/tutorial/topicsovertime/topicsovertime.html) topic modeling. It even supports visualizations similar to LDAvis!
+[**guided**](https://maartengr.github.io/BERTopic/getting_started/guided/guided.html), 
+(semi-) [**supervised**](https://maartengr.github.io/BERTopic/getting_started/supervised/supervised.html), 
+and [**dynamic**](https://maartengr.github.io/BERTopic/getting_started/topicsovertime/topicsovertime.html) topic modeling. It even supports visualizations similar to LDAvis!
 
 Corresponding medium posts can be found [here](https://towardsdatascience.com/topic-modeling-with-bert-779f7db187e6?source=friends_link&sk=0b5a470c006d1842ad4c8a3057063a99) 
 and [here](https://towardsdatascience.com/interactive-topic-modeling-with-bertopic-1ea55e7d73d8?sk=03c2168e9e74b6bda2a1f3ed953427e4).
 
 ## Installation
 
 Installation, with sentence-transformers, can be done using [pypi](https://pypi.org/project/bertopic/):
@@ -50,27 +50,27 @@
 | Advanced Customization in BERTopic  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ClTYut039t-LDtlcd-oQAdXWgcsSGTw9?usp=sharing) |
 | (semi-)Supervised Topic Modeling with BERTopic  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1bxizKzv5vfxJEB29sntU__ZC7PBSIPaQ?usp=sharing)  |
 | Dynamic Topic Modeling with Trump's Tweets  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1un8ooI-7ZNlRoK0maVkYhmNRl0XGK88f?usp=sharing)  |
 | Topic Modeling arXiv Abstracts | [![Kaggle](https://img.shields.io/static/v1?style=for-the-badge&message=Kaggle&color=222222&logo=Kaggle&logoColor=20BEFF&label=)](https://www.kaggle.com/maartengr/topic-modeling-arxiv-abstract-with-bertopic) |
 
 
 ## Quick Start
-We start by extracting topics from the well-known 20 newsgroups dataset which is comprised of english documents:
+We start by extracting topics from the well-known 20 newsgroups dataset containing English documents:
 
 ```python
 from bertopic import BERTopic
 from sklearn.datasets import fetch_20newsgroups
  
 docs = fetch_20newsgroups(subset='all',  remove=('headers', 'footers', 'quotes'))['data']
 
 topic_model = BERTopic()
 topics, probs = topic_model.fit_transform(docs)
 ```
 
-After generating topics, we can access the frequent topics that were generated:
+After generating topics and their probabilities, we can access the frequent topics that were generated:
 
 ```python
 >>> topic_model.get_topic_info()
 
 Topic	Count	Name
 -1	4630	-1_can_your_will_any
 0	693	49_windows_drive_dos_file
@@ -119,15 +119,15 @@
 topic_model.visualize_barchart()
 ``` 
 
 <img src="images/topics.png" width="70%" height="70%" align="center" />
 
 
 Find all possible visualizations with interactive examples in the documentation 
-[here](https://maartengr.github.io/BERTopic/tutorial/visualization/visualization.html). 
+[here](https://maartengr.github.io/BERTopic/getting_started/visualization/visualization.html). 
 
 ## Embedding Models
 BERTopic supports many embedding models that can be used to embed the documents and words:
 * Sentence-Transformers
 * Flair
 * Spacy
 * Gensim
@@ -147,15 +147,15 @@
 ```python
 from flair.embeddings import TransformerDocumentEmbeddings
 
 roberta = TransformerDocumentEmbeddings('roberta-base')
 topic_model = BERTopic(embedding_model=roberta)
 ```
 
-Click [here](https://maartengr.github.io/BERTopic/tutorial/embeddings/embeddings.html) 
+Click [here](https://maartengr.github.io/BERTopic/getting_started/embeddings/embeddings.html) 
 for a full overview of all supported embedding models. 
 
 ## Dynamic Topic Modeling
 Dynamic topic modeling (DTM) is a collection of techniques aimed at analyzing the evolution of topics 
 over time. These methods allow you to understand how a topic is represented over time. 
 Here, we will be using all of Donald Trump's tweet to see how he talked over certain topics over time: 
 
@@ -234,12 +234,12 @@
 
 ```bibtex
 @misc{grootendorst2020bertopic,
   author       = {Maarten Grootendorst},
   title        = {BERTopic: Leveraging BERT and c-TF-IDF to create easily interpretable topics.},
   year         = 2020,
   publisher    = {Zenodo},
-  version      = {v0.9.2},
+  version      = {v0.9.4},
   doi          = {10.5281/zenodo.4381785},
   url          = {https://doi.org/10.5281/zenodo.4381785}
 }
 ```
```

### Comparing `bertopic-0.9.3/bertopic/_bertopic.py` & `bertopic-0.9.4/bertopic/_bertopic.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
                  language: str = "english",
                  top_n_words: int = 10,
                  n_gram_range: Tuple[int, int] = (1, 1),
                  min_topic_size: int = 10,
                  nr_topics: Union[int, str] = None,
                  low_memory: bool = False,
                  calculate_probabilities: bool = False,
+                 diversity: float = None,
                  seed_topic_list: List[List[str]] = None,
                  embedding_model=None,
                  umap_model: UMAP = None,
                  hdbscan_model: hdbscan.HDBSCAN = None,
                  vectorizer_model: CountVectorizer = None,
                  verbose: bool = False,
                  ):
@@ -101,25 +102,27 @@
                           CountVectorizer.
             min_topic_size: The minimum size of the topic. Increasing this value will lead
                             to a lower number of clusters/topics.
             nr_topics: Specifying the number of topics will reduce the initial
                        number of topics to the value specified. This reduction can take
                        a while as each reduction in topics (-1) activates a c-TF-IDF
                        calculation. If this is set to None, no reduction is applied. Use
-                       "auto" to automatically reduce topics that have a similarity of at
-                       least 0.9, do not maps all others.
+                       "auto" to automatically reduce topics using HDBSCAN.
             low_memory: Sets UMAP low memory to True to make sure less memory is used.
             calculate_probabilities: Whether to calculate the probabilities of all topics
                                      per document instead of the probability of the assigned
                                      topic per document. This could slow down the extraction
                                      of topics if you have many documents (> 100_000). Set this
                                      only to True if you have a low amount of documents or if
                                      you do not mind more computation time.
                                      NOTE: If false you cannot use the corresponding
                                      visualization method `visualize_probabilities`.
+            diversity: Whether to use MMR to diversify the resulting topic representations.
+                       If set to None, MMR will not be used. Accepted values lie between 
+                       0 and 1 with 0 being not at all diverse and 1 being very diverse. 
             seed_topic_list: A list of seed words per topic to converge around
             verbose: Changes the verbosity of the model, Set to True if you want
                      to track the stages of the model.
             embedding_model: Use a custom embedding model.
                              The following backends are currently supported
                                * SentenceTransformers
                                * Flair
@@ -137,14 +140,15 @@
         if top_n_words > 30:
             raise ValueError("top_n_words should be lower or equal to 30. The preferred value is 10.")
         self.top_n_words = top_n_words
         self.min_topic_size = min_topic_size
         self.nr_topics = nr_topics
         self.low_memory = low_memory
         self.calculate_probabilities = calculate_probabilities
+        self.diversity = diversity
         self.verbose = verbose
         self.seed_topic_list = seed_topic_list
 
         # Embedding model
         self.language = language if not embedding_model else None
         self.embedding_model = embedding_model
 
@@ -366,18 +370,22 @@
 
         if embeddings is None:
             embeddings = self._extract_embeddings(documents,
                                                   method="document",
                                                   verbose=self.verbose)
 
         umap_embeddings = self.umap_model.transform(embeddings)
+        logger.info("Reduced dimensionality with UMAP")
+
         predictions, probabilities = hdbscan.approximate_predict(self.hdbscan_model, umap_embeddings)
+        logger.info("Predicted clusters with HDBSCAN")
 
         if self.calculate_probabilities:
             probabilities = hdbscan.membership_vector(self.hdbscan_model, umap_embeddings)
+            logger.info("Calculated probabilities with HDBSCAN")
         else:
             probabilities = None
 
         probabilities = self._map_probabilities(probabilities, original_topics=True)
         predictions = self._map_predictions(predictions)
         return predictions, probabilities
 
@@ -472,15 +480,15 @@
         topics_over_time = []
         for index, timestamp in tqdm(enumerate(timestamps), disable=not self.verbose):
 
             # Calculate c-TF-IDF representation for a specific timestamp
             selection = documents.loc[documents.Timestamps == timestamp, :]
             documents_per_topic = selection.groupby(['Topic'], as_index=False).agg({'Document': ' '.join,
                                                                                     "Timestamps": "count"})
-            c_tf_idf, words = self._c_tf_idf(documents_per_topic, m=len(selection), fit=False)
+            c_tf_idf, words = self._c_tf_idf(documents_per_topic, fit=False)
 
             if global_tuning or evolution_tuning:
                 c_tf_idf = normalize(c_tf_idf, axis=1, norm='l1', copy=False)
 
             # Fine-tune the c-TF-IDF matrix at timestamp t by averaging it with the c-TF-IDF
             # matrix at timestamp t-1
             if evolution_tuning and index != 0:
@@ -565,15 +573,15 @@
         topics_per_class = []
         for index, class_ in tqdm(enumerate(set(classes)), disable=not self.verbose):
 
             # Calculate c-TF-IDF representation for a specific timestamp
             selection = documents.loc[documents.Class == class_, :]
             documents_per_topic = selection.groupby(['Topic'], as_index=False).agg({'Document': ' '.join,
                                                                                     "Class": "count"})
-            c_tf_idf, words = self._c_tf_idf(documents_per_topic, m=len(selection), fit=False)
+            c_tf_idf, words = self._c_tf_idf(documents_per_topic, fit=False)
 
             # Fine-tune the timestamp c-TF-IDF representation based on the global c-TF-IDF representation
             # by simply taking the average of the two
             if global_tuning:
                 c_tf_idf = normalize(c_tf_idf, axis=1, norm='l1', copy=False)
                 c_tf_idf = (global_c_tf_idf[documents_per_topic.Topic.values + 1] + c_tf_idf) / 2.0
 
@@ -1103,16 +1111,16 @@
         matrix between topic embeddings.
 
         Arguments:
             orientation: The orientation of the figure.
                          Either 'left' or 'bottom'
             topics: A selection of topics to visualize
             top_n_topics: Only select the top n most frequent topics
-            width: The width of the figure.
-            height: The height of the figure.
+            width: The width of the figure. Only works if orientation is set to 'left'
+            height: The height of the figure. Only works if orientation is set to 'bottom'
 
         Returns:
             fig: A plotly figure
 
         Usage:
 
         To visualize the hierarchical structure of
@@ -1181,26 +1189,26 @@
                                           top_n_topics=top_n_topics,
                                           n_clusters=n_clusters,
                                           width=width,
                                           height=height)
 
     def visualize_barchart(self,
                            topics: List[int] = None,
-                           top_n_topics: int = 6,
+                           top_n_topics: int = 8,
                            n_words: int = 5,
-                           width: int = 800,
-                           height: int = 600) -> go.Figure:
+                           width: int = 250,
+                           height: int = 250) -> go.Figure:
         """ Visualize a barchart of selected topics
 
         Arguments:
             topics: A selection of topics to visualize.
             top_n_topics: Only select the top n most frequent topics.
             n_words: Number of words to show in a topic
-            width: The width of the figure.
-            height: The height of the figure.
+            width: The width of each figure.
+            height: The height of each figure.
 
         Returns:
             fig: A plotly figure
 
         Usage:
 
         To visualize the barchart of selected topics
@@ -1443,15 +1451,15 @@
         Arguments:
             documents: Dataframe with documents and their corresponding IDs
 
         Returns:
             c_tf_idf: The resulting matrix giving a value (importance score) for each word per topic
         """
         documents_per_topic = documents.groupby(['Topic'], as_index=False).agg({'Document': ' '.join})
-        self.c_tf_idf, words = self._c_tf_idf(documents_per_topic, m=len(documents))
+        self.c_tf_idf, words = self._c_tf_idf(documents_per_topic)
         self.topics = self._extract_words_per_topic(words)
         self._create_topic_vectors()
         self.topic_names = {key: f"{key}_" + "_".join([word[0] for word in values[:4]])
                             for key, values in
                             self.topics.items()}
 
     def _save_representative_docs(self, documents: pd.DataFrame):
@@ -1549,15 +1557,15 @@
                 if sum(word_importance) == 0:
                     word_importance = [1 for _ in range(len(self.get_topic(topic)))]
                 topic_embedding = np.average(embeddings[i * n: n + (i * n)], weights=word_importance, axis=0)
                 topic_embeddings.append(topic_embedding)
 
             self.topic_embeddings = topic_embeddings
 
-    def _c_tf_idf(self, documents_per_topic: pd.DataFrame, m: int, fit: bool = True) -> Tuple[csr_matrix, List[str]]:
+    def _c_tf_idf(self, documents_per_topic: pd.DataFrame, fit: bool = True) -> Tuple[csr_matrix, List[str]]:
         """ Calculate a class-based TF-IDF where m is the number of total documents.
 
         Arguments:
             documents_per_topic: The joined documents per topic such that each topic has a single
                                  string made out of multiple documents
             m: The total number of documents (unjoined)
             fit: Whether to fit a new vectorizer or use the fitted self.vectorizer_model
@@ -1577,15 +1585,15 @@
         if self.seed_topic_list:
             seed_topic_list = [seed for seeds in self.seed_topic_list for seed in seeds]
             multiplier = np.array([1.2 if word in seed_topic_list else 1 for word in words])
         else:
             multiplier = None
 
         if fit:
-            self.transformer = ClassTFIDF().fit(X, n_samples=m, multiplier=multiplier)
+            self.transformer = ClassTFIDF().fit(X, multiplier=multiplier)
 
         c_tf_idf = self.transformer.transform(X)
 
         self.topic_sim_matrix = cosine_similarity(c_tf_idf)
 
         return c_tf_idf, words
 
@@ -1637,27 +1645,28 @@
                           else ("", 0.00001)
                           for word_index, score in zip(indices[index][::-1], scores[index][::-1])
                           ]
                   for index, label in enumerate(labels)}
 
         # Extract word embeddings for the top 30 words per topic and compare it
         # with the topic embedding to keep only the words most similar to the topic embedding
-        if self.embedding_model is not None:
+        if self.diversity is not None:
+            if self.embedding_model is not None:
 
-            for topic, topic_words in topics.items():
-                words = [word[0] for word in topic_words]
-                word_embeddings = self._extract_embeddings(words,
-                                                           method="word",
-                                                           verbose=False)
-                topic_embedding = self._extract_embeddings(" ".join(words),
-                                                           method="word",
-                                                           verbose=False).reshape(1, -1)
-                topic_words = mmr(topic_embedding, word_embeddings, words,
-                                  top_n=self.top_n_words, diversity=0)
-                topics[topic] = [(word, value) for word, value in topics[topic] if word in topic_words]
+                for topic, topic_words in topics.items():
+                    words = [word[0] for word in topic_words]
+                    word_embeddings = self._extract_embeddings(words,
+                                                            method="word",
+                                                            verbose=False)
+                    topic_embedding = self._extract_embeddings(" ".join(words),
+                                                            method="word",
+                                                            verbose=False).reshape(1, -1)
+                    topic_words = mmr(topic_embedding, word_embeddings, words,
+                                    top_n=self.top_n_words, diversity=self.diversity)
+                    topics[topic] = [(word, value) for word, value in topics[topic] if word in topic_words]
         topics = {label: values[:self.top_n_words] for label, values in topics.items()}
 
         return topics
 
     def _reduce_topics(self, documents: pd.DataFrame) -> pd.DataFrame:
         """ Reduce topics to self.nr_topics
 
@@ -1690,18 +1699,15 @@
             documents: Updated dataframe with documents and the reduced number of Topics
         """
         # Track which topics where originally merged
         if not self.merged_topics:
             self.merged_topics = []
 
         # Create topic similarity matrix
-        if self.topic_embeddings is not None:
-            similarities = cosine_similarity(np.array(self.topic_embeddings))
-        else:
-            similarities = cosine_similarity(self.c_tf_idf)
+        similarities = cosine_similarity(self.c_tf_idf)
         np.fill_diagonal(similarities, 0)
 
         # Find most similar topic to least common topic
         topics = documents.Topic.tolist().copy()
         mapped_topics = {}
         while len(self.get_topic_freq()) > self.nr_topics + 1:
             topic_to_merge = self.get_topic_freq().iloc[-1].Topic
```

### Comparing `bertopic-0.9.3/bertopic/_ctfidf.py` & `bertopic-0.9.4/bertopic/_ctfidf.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,41 +17,51 @@
     each class **i** and divided by the total number of words **w**.
     Next, the total, unjoined, number of documents across all classes **m** is divided by the total
     sum of word **i** across all classes.
     """
     def __init__(self, *args, **kwargs):
         super(ClassTFIDF, self).__init__(*args, **kwargs)
 
-    def fit(self, X: sp.csr_matrix, n_samples: int, multiplier: np.ndarray = None):
+    def fit(self, X: sp.csr_matrix, multiplier: np.ndarray = None):
         """Learn the idf vector (global term weights).
 
         Arguments:
             X: A matrix of term/token counts.
-            n_samples: Number of total documents
+            multiplier: A multiplier for increasing/decreasing certain IDF scores
         """
         X = check_array(X, accept_sparse=('csr', 'csc'))
         if not sp.issparse(X):
             X = sp.csr_matrix(X)
         dtype = np.float64
 
         if self.use_idf:
             _, n_features = X.shape
+
+            # Calculate the frequency of words across all classes
             df = np.squeeze(np.asarray(X.sum(axis=0)))
+
+            # Calculate the average number of samples as regularization
             avg_nr_samples = int(X.sum(axis=1).mean())
-            idf = np.log(avg_nr_samples / df)
+
+            # Divide the average number of samples by the word frequency
+            # +1 is added to force values to be positive
+            idf = np.log((avg_nr_samples / df)+1)
+
+            # Multiplier to increase/decrease certain idf scores
             if multiplier is not None:
                 idf = idf * multiplier
+
             self._idf_diag = sp.diags(idf, offsets=0,
                                       shape=(n_features, n_features),
                                       format='csr',
                                       dtype=dtype)
 
         return self
 
-    def transform(self, X: sp.csr_matrix, copy=True):
+    def transform(self, X: sp.csr_matrix):
         """Transform a count-based matrix to c-TF-IDF
 
         Arguments:
             X (sparse matrix): A matrix of term/token counts.
 
         Returns:
             X (sparse matrix): A c-TF-IDF matrix
```

### Comparing `bertopic-0.9.3/bertopic/_mmr.py` & `bertopic-0.9.4/bertopic/_mmr.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/bertopic/_utils.py` & `bertopic-0.9.4/bertopic/_utils.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/bertopic/backend/_base.py` & `bertopic-0.9.4/bertopic/backend/_base.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/bertopic/backend/_flair.py` & `bertopic-0.9.4/bertopic/backend/_flair.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/bertopic/backend/_gensim.py` & `bertopic-0.9.4/bertopic/backend/_gensim.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/bertopic/backend/_sentencetransformers.py` & `bertopic-0.9.4/bertopic/backend/_sentencetransformers.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/bertopic/backend/_spacy.py` & `bertopic-0.9.4/bertopic/backend/_spacy.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/bertopic/backend/_use.py` & `bertopic-0.9.4/bertopic/backend/_use.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/bertopic/backend/_utils.py` & `bertopic-0.9.4/bertopic/backend/_utils.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/bertopic/backend/_word_doc.py` & `bertopic-0.9.4/bertopic/backend/_word_doc.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/bertopic/plotting/__init__.py` & `bertopic-0.9.4/bertopic/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/bertopic/plotting/_barchart.py` & `bertopic-0.9.4/bertopic/plotting/_barchart.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+import itertools
 import numpy as np
 from typing import List
 
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 
 def visualize_barchart(topic_model,
                        topics: List[int] = None,
-                       top_n_topics: int = 6,
+                       top_n_topics: int = 8,
                        n_words: int = 5,
-                       width: int = 800,
-                       height: int = 600) -> go.Figure:
+                       width: int = 250,
+                       height: int = 250) -> go.Figure:
     """ Visualize a barchart of selected topics
 
     Arguments:
         topic_model: A fitted BERTopic instance.
         topics: A selection of topics to visualize.
         top_n_topics: Only select the top n most frequent topics.
         n_words: Number of words to show in a topic
-        width: The width of the figure.
-        height: The height of the figure.
+        width: The width of each figure.
+        height: The height of each figure.
 
     Returns:
         fig: A plotly figure
 
     Usage:
 
     To visualize the barchart of selected topics
@@ -35,71 +36,73 @@
 
     Or if you want to save the resulting figure:
 
     ```python
     fig = topic_model.visualize_barchart()
     fig.write_html("path/to/file.html")
     ```
-    <iframe src="../../tutorial/visualization/bar_chart.html"
+    <iframe src="../../getting_started/visualization/bar_chart.html"
     style="width:1100px; height: 660px; border: 0px;""></iframe>
     """
+    colors = itertools.cycle(["#D55E00", "#0072B2", "#CC79A7", "#E69F00", "#56B4E9", "#009E73", "#F0E442"])
+
     # Select topics based on top_n and topics args
     if topics is not None:
         topics = list(topics)
     elif top_n_topics is not None:
         topics = topic_model.get_topic_freq().Topic.to_list()[1:top_n_topics + 1]
     else:
         topics = topic_model.get_topic_freq().Topic.to_list()[1:7]
 
     # Initialize figure
     subplot_titles = [f"Topic {topic}" for topic in topics]
-    columns = 3
+    columns = 4
     rows = int(np.ceil(len(topics) / columns))
     fig = make_subplots(rows=rows,
                         cols=columns,
-                        shared_xaxes=True,
-                        horizontal_spacing=.15,
-                        vertical_spacing=.15,
+                        shared_xaxes=False,
+                        horizontal_spacing=.1,
+                        vertical_spacing=.4 / rows if rows > 1 else 0,
                         subplot_titles=subplot_titles)
 
     # Add barchart for each topic
     row = 1
     column = 1
     for topic in topics:
         words = [word + "  " for word, _ in topic_model.get_topic(topic)][:n_words][::-1]
         scores = [score for _, score in topic_model.get_topic(topic)][:n_words][::-1]
 
         fig.add_trace(
             go.Bar(x=scores,
                    y=words,
-                   orientation='h'),
+                   orientation='h',
+                   marker_color=next(colors)),
             row=row, col=column)
 
         if column == columns:
             column = 1
             row += 1
         else:
             column += 1
 
     # Stylize graph
     fig.update_layout(
         template="plotly_white",
         showlegend=False,
         title={
             'text': "<b>Topic Word Scores",
-            'y': .95,
-            'x': .15,
+            'x': .5,
             'xanchor': 'center',
             'yanchor': 'top',
             'font': dict(
                 size=22,
                 color="Black")
         },
-        width=width,
-        height=height,
+        width=width*4,
+        height=height*rows if rows > 1 else height * 1.3,
         hoverlabel=dict(
             bgcolor="white",
             font_size=16,
             font_family="Rockwell"
         ),
     )
```

### Comparing `bertopic-0.9.3/bertopic/plotting/_distribution.py` & `bertopic-0.9.4/bertopic/plotting/_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     Or if you want to save the resulting figure:
 
     ```python
     fig = topic_model.visualize_distribution(probabilities[0])
     fig.write_html("path/to/file.html")
     ```
-    <iframe src="../../tutorial/visualization/probabilities.html"
+    <iframe src="../../getting_started/visualization/probabilities.html"
     style="width:1000px; height: 500px; border: 0px;""></iframe>
     """
     if len(probabilities.shape) != 1:
         raise ValueError("This visualization cannot be used if you have set `calculate_probabilities` to False "
                          "as it uses the topic probabilities of all topics. ")
     if len(probabilities[probabilities > min_probability]) == 0:
         raise ValueError("There are no values where `min_probability` is higher than the "
```

### Comparing `bertopic-0.9.3/bertopic/plotting/_heatmap.py` & `bertopic-0.9.4/bertopic/plotting/_heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     Or if you want to save the resulting figure:
 
     ```python
     fig = topic_model.visualize_heatmap()
     fig.write_html("path/to/file.html")
     ```
-    <iframe src="../../tutorial/visualization/heatmap.html"
+    <iframe src="../../getting_started/visualization/heatmap.html"
     style="width:1000px; height: 720px; border: 0px;""></iframe>
     """
 
     # Select topic embeddings
     if topic_model.topic_embeddings is not None:
         embeddings = np.array(topic_model.topic_embeddings)
     else:
```

### Comparing `bertopic-0.9.3/bertopic/plotting/_hierarchy.py` & `bertopic-0.9.4/bertopic/plotting/_hierarchy.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
     Arguments:
         topic_model: A fitted BERTopic instance.
         orientation: The orientation of the figure.
                      Either 'left' or 'bottom'
         topics: A selection of topics to visualize
         top_n_topics: Only select the top n most frequent topics
-        width: The width of the figure.
-        height: The height of the figure.
+        width: The width of the figure. Only works if orientation is set to 'left'
+        height: The height of the figure. Only works if orientation is set to 'bottom'
 
     Returns:
         fig: A plotly figure
 
     Usage:
 
     To visualize the hierarchical structure of
@@ -42,15 +42,15 @@
 
     Or if you want to save the resulting figure:
 
     ```python
     fig = topic_model.visualize_hierarchy()
     fig.write_html("path/to/file.html")
     ```
-    <iframe src="../../tutorial/visualization/hierarchy.html"
+    <iframe src="../../getting_started/visualization/hierarchy.html"
     style="width:1000px; height: 680px; border: 0px;""></iframe>
     """
 
     # Select topic embeddings
     if topic_model.topic_embeddings is not None:
         embeddings = np.array(topic_model.topic_embeddings)
     else:
@@ -85,33 +85,39 @@
 
     # Stylize layout
     fig.update_layout(
         plot_bgcolor='#ECEFF1',
         template="plotly_white",
         title={
             'text': "<b>Hierarchical Clustering",
-            'y': .95,
             'x': 0.5,
             'xanchor': 'center',
             'yanchor': 'top',
             'font': dict(
                 size=22,
                 color="Black")
         },
-        width=width,
-        height=height,
         hoverlabel=dict(
             bgcolor="white",
             font_size=16,
             font_family="Rockwell"
         ),
-
     )
 
     # Stylize orientation
     if orientation == "left":
-        fig.update_layout(yaxis=dict(tickmode="array",
+        fig.update_layout(height=200+(15*len(topics)),
+                          width=width,
+                          yaxis=dict(tickmode="array",
                                      ticktext=new_labels))
+        
+        # Fix empty space on the bottom of the graph
+        y_max = max([trace['y'].max()+5 for trace in fig['data']])
+        y_min = min([trace['y'].min()-5 for trace in fig['data']])
+        fig.update_layout(yaxis=dict(range=[y_min, y_max]))
+
     else:
-        fig.update_layout(xaxis=dict(tickmode="array",
+        fig.update_layout(width=200+(15*len(topics)),
+                          height=height,
+                          xaxis=dict(tickmode="array",
                                      ticktext=new_labels))
     return fig
```

### Comparing `bertopic-0.9.3/bertopic/plotting/_term_rank.py` & `bertopic-0.9.4/bertopic/plotting/_term_rank.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,18 +38,18 @@
     Or if you want to save the resulting figure:
 
     ```python
     fig = topic_model.visualize_term_rank()
     fig.write_html("path/to/file.html")
     ```
 
-    <iframe src="../../tutorial/visualization/term_rank.html"
+    <iframe src="../../getting_started/visualization/term_rank.html"
     style="width:1000px; height: 530px; border: 0px;""></iframe>
 
-    <iframe src="../../tutorial/visualization/term_rank_log.html"
+    <iframe src="../../getting_started/visualization/term_rank_log.html"
     style="width:1000px; height: 530px; border: 0px;""></iframe>
 
     Reference:
 
     This visualization was heavily inspired by the
     "Term Probability Decline" visualization found in an
     analysis by the amazing [tmtoolkit](https://tmtoolkit.readthedocs.io/).
```

### Comparing `bertopic-0.9.3/bertopic/plotting/_topics.py` & `bertopic-0.9.4/bertopic/plotting/_topics.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     Or if you want to save the resulting figure:
 
     ```python
     fig = topic_model.visualize_topics()
     fig.write_html("path/to/file.html")
     ```
-    <iframe src="../../tutorial/visualization/viz.html"
+    <iframe src="../../getting_started/visualization/viz.html"
     style="width:1000px; height: 680px; border: 0px;""></iframe>
     """
     # Select topics based on top_n and topics args
     if topics is not None:
         topics = list(topics)
     elif top_n_topics is not None:
         topics = sorted(topic_model.get_topic_freq().Topic.to_list()[1:top_n_topics + 1])
@@ -83,21 +83,21 @@
 
     # Prepare figure range
     x_range = (df.x.min() - abs((df.x.min()) * .15), df.x.max() + abs((df.x.max()) * .15))
     y_range = (df.y.min() - abs((df.y.min()) * .15), df.y.max() + abs((df.y.max()) * .15))
 
     # Plot topics
     fig = px.scatter(df, x="x", y="y", size="Size", size_max=40, template="simple_white", labels={"x": "", "y": ""},
-                     hover_data={"x": False, "y": False, "Topic": True, "Words": True, "Size": True})
+                     hover_data={"Topic": True, "Words": True, "Size": True, "x": False, "y": False})
     fig.update_traces(marker=dict(color="#B0BEC5", line=dict(width=2, color='DarkSlateGrey')))
 
     # Update hover order
-    fig.update_traces(hovertemplate="<br>".join(["<b>Topic %{customdata[2]}</b>",
-                                                 "Words: %{customdata[3]}",
-                                                 "Size: %{customdata[4]}"]))
+    fig.update_traces(hovertemplate="<br>".join(["<b>Topic %{customdata[0]}</b>",
+                                                 "Words: %{customdata[1]}",
+                                                 "Size: %{customdata[2]}"]))
 
     # Create a slider for topic selection
     steps = [dict(label=f"Topic {topic}", method="update", args=get_color(topic)) for topic in topic_list[1:]]
     sliders = [dict(active=0, pad={"t": 50}, steps=steps)]
 
     # Stylize layout
     fig.update_layout(
```

### Comparing `bertopic-0.9.3/bertopic/plotting/_topics_over_time.py` & `bertopic-0.9.4/bertopic/plotting/_topics_over_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     Or if you want to save the resulting figure:
 
     ```python
     fig = topic_model.visualize_topics_over_time(topics_over_time)
     fig.write_html("path/to/file.html")
     ```
-    <iframe src="../../tutorial/visualization/trump.html"
+    <iframe src="../../getting_started/visualization/trump.html"
     style="width:1000px; height: 680px; border: 0px;""></iframe>
     """
     colors = ["#E69F00", "#56B4E9", "#009E73", "#F0E442", "#D55E00", "#0072B2", "#CC79A7"]
 
     # Select topics
     if topics:
         selected_topics = topics
```

### Comparing `bertopic-0.9.3/bertopic/plotting/_topics_per_class.py` & `bertopic-0.9.4/bertopic/plotting/_topics_per_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     Or if you want to save the resulting figure:
 
     ```python
     fig = topic_model.visualize_topics_per_class(topics_per_class)
     fig.write_html("path/to/file.html")
     ```
-    <iframe src="../../tutorial/visualization/topics_per_class.html"
+    <iframe src="../../getting_started/visualization/topics_per_class.html"
     style="width:1400px; height: 1000px; border: 0px;""></iframe>
     """
     colors = ["#E69F00", "#56B4E9", "#009E73", "#F0E442", "#D55E00", "#0072B2", "#CC79A7"]
 
     # Select topics
     if topics:
         selected_topics = topics
```

### Comparing `bertopic-0.9.3/bertopic.egg-info/PKG-INFO` & `bertopic-0.9.4/bertopic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: bertopic
-Version: 0.9.3
+Version: 0.9.4
 Summary: BERTopic performs topic Modeling with state-of-the-art transformer models.
 Home-page: https://github.com/MaartenGr/BERTopic
 Author: Maarten P. Grootendorst
 Author-email: maartengrootendorst@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://maartengr.github.io/BERTopic/
 Project-URL: Source Code, https://github.com/MaartenGr/BERTopic/
 Project-URL: Issue Tracker, https://github.com/MaartenGr/BERTopic/issues
-Description: [![PyPI - Python](https://img.shields.io/badge/python-v3.6+-blue.svg)](https://pypi.org/project/bertopic/)
+Description: [![PyPI - Python](https://img.shields.io/badge/python-v3.7+-blue.svg)](https://pypi.org/project/bertopic/)
         [![Build](https://img.shields.io/github/workflow/status/MaartenGr/BERTopic/Code%20Checks/master)](https://pypi.org/project/bertopic/)
         [![docs](https://img.shields.io/badge/docs-Passing-green.svg)](https://maartengr.github.io/BERTopic/)
         [![PyPI - PyPi](https://img.shields.io/pypi/v/BERTopic)](https://pypi.org/project/bertopic/)
         [![PyPI - License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/MaartenGr/VLAC/blob/master/LICENSE)
         [![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.4381785-blue)](https://doi.org/10.5281/zenodo.4381785)
         
         # BERTopic
         
         <img src="images/logo.png" width="35%" height="35%" align="right" />
         
         BERTopic is a topic modeling technique that leverages ðŸ¤— transformers and c-TF-IDF to create dense clusters
         allowing for easily interpretable topics whilst keeping important words in the topic descriptions.
         
         BERTopic supports 
-        [**guided**](https://maartengr.github.io/BERTopic/tutorial/guided/guided.html), 
-        (semi-) [**supervised**](https://maartengr.github.io/BERTopic/tutorial/supervised/supervised.html), 
-        and [**dynamic**](https://maartengr.github.io/BERTopic/tutorial/topicsovertime/topicsovertime.html) topic modeling. It even supports visualizations similar to LDAvis!
+        [**guided**](https://maartengr.github.io/BERTopic/getting_started/guided/guided.html), 
+        (semi-) [**supervised**](https://maartengr.github.io/BERTopic/getting_started/supervised/supervised.html), 
+        and [**dynamic**](https://maartengr.github.io/BERTopic/getting_started/topicsovertime/topicsovertime.html) topic modeling. It even supports visualizations similar to LDAvis!
         
         Corresponding medium posts can be found [here](https://towardsdatascience.com/topic-modeling-with-bert-779f7db187e6?source=friends_link&sk=0b5a470c006d1842ad4c8a3057063a99) 
         and [here](https://towardsdatascience.com/interactive-topic-modeling-with-bertopic-1ea55e7d73d8?sk=03c2168e9e74b6bda2a1f3ed953427e4).
         
         ## Installation
         
         Installation, with sentence-transformers, can be done using [pypi](https://pypi.org/project/bertopic/):
@@ -61,27 +61,27 @@
         | Advanced Customization in BERTopic  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ClTYut039t-LDtlcd-oQAdXWgcsSGTw9?usp=sharing) |
         | (semi-)Supervised Topic Modeling with BERTopic  |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1bxizKzv5vfxJEB29sntU__ZC7PBSIPaQ?usp=sharing)  |
         | Dynamic Topic Modeling with Trump's Tweets  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1un8ooI-7ZNlRoK0maVkYhmNRl0XGK88f?usp=sharing)  |
         | Topic Modeling arXiv Abstracts | [![Kaggle](https://img.shields.io/static/v1?style=for-the-badge&message=Kaggle&color=222222&logo=Kaggle&logoColor=20BEFF&label=)](https://www.kaggle.com/maartengr/topic-modeling-arxiv-abstract-with-bertopic) |
         
         
         ## Quick Start
-        We start by extracting topics from the well-known 20 newsgroups dataset which is comprised of english documents:
+        We start by extracting topics from the well-known 20 newsgroups dataset containing English documents:
         
         ```python
         from bertopic import BERTopic
         from sklearn.datasets import fetch_20newsgroups
          
         docs = fetch_20newsgroups(subset='all',  remove=('headers', 'footers', 'quotes'))['data']
         
         topic_model = BERTopic()
         topics, probs = topic_model.fit_transform(docs)
         ```
         
-        After generating topics, we can access the frequent topics that were generated:
+        After generating topics and their probabilities, we can access the frequent topics that were generated:
         
         ```python
         >>> topic_model.get_topic_info()
         
         Topic	Count	Name
         -1	4630	-1_can_your_will_any
         0	693	49_windows_drive_dos_file
@@ -130,15 +130,15 @@
         topic_model.visualize_barchart()
         ``` 
         
         <img src="images/topics.png" width="70%" height="70%" align="center" />
         
         
         Find all possible visualizations with interactive examples in the documentation 
-        [here](https://maartengr.github.io/BERTopic/tutorial/visualization/visualization.html). 
+        [here](https://maartengr.github.io/BERTopic/getting_started/visualization/visualization.html). 
         
         ## Embedding Models
         BERTopic supports many embedding models that can be used to embed the documents and words:
         * Sentence-Transformers
         * Flair
         * Spacy
         * Gensim
@@ -158,15 +158,15 @@
         ```python
         from flair.embeddings import TransformerDocumentEmbeddings
         
         roberta = TransformerDocumentEmbeddings('roberta-base')
         topic_model = BERTopic(embedding_model=roberta)
         ```
         
-        Click [here](https://maartengr.github.io/BERTopic/tutorial/embeddings/embeddings.html) 
+        Click [here](https://maartengr.github.io/BERTopic/getting_started/embeddings/embeddings.html) 
         for a full overview of all supported embedding models. 
         
         ## Dynamic Topic Modeling
         Dynamic topic modeling (DTM) is a collection of techniques aimed at analyzing the evolution of topics 
         over time. These methods allow you to understand how a topic is represented over time. 
         Here, we will be using all of Donald Trump's tweet to see how he talked over certain topics over time: 
         
@@ -245,15 +245,15 @@
         
         ```bibtex
         @misc{grootendorst2020bertopic,
           author       = {Maarten Grootendorst},
           title        = {BERTopic: Leveraging BERT and c-TF-IDF to create easily interpretable topics.},
           year         = 2020,
           publisher    = {Zenodo},
-          version      = {v0.9.2},
+          version      = {v0.9.4},
           doi          = {10.5281/zenodo.4381785},
           url          = {https://doi.org/10.5281/zenodo.4381785}
         }
         ```
         
 Keywords: nlp bert topic modeling embeddings
 Platform: UNKNOWN
@@ -264,18 +264,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: docs
 Provides-Extra: dev
-Provides-Extra: spacy
 Provides-Extra: flair
-Provides-Extra: test
-Provides-Extra: gensim
+Provides-Extra: spacy
 Provides-Extra: use
-Provides-Extra: docs
+Provides-Extra: gensim
```

### Comparing `bertopic-0.9.3/bertopic.egg-info/SOURCES.txt` & `bertopic-0.9.4/bertopic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/setup.py` & `bertopic-0.9.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "numpy>=1.20.0",
     "hdbscan>=0.8.27",
     "umap-learn>=0.5.0",
     "pandas>=1.1.5",
     "scikit-learn>=0.22.2.post1",
     "tqdm>=4.41.1",
     "sentence-transformers>=0.4.1",
-    "plotly>=4.7.0,<4.14.3",
+    "plotly>=4.7.0",
     "pyyaml<6.0"
 ]
 
 flair_packages = [
     "transformers==3.5.1",
     "torch>=1.4.0,<1.7.1",
     "flair==0.7"
@@ -49,15 +49,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bertopic",
     packages=find_packages(exclude=["notebooks", "docs"]),
-    version="0.9.3",
+    version="0.9.4",
     author="Maarten P. Grootendorst",
     author_email="maartengrootendorst@gmail.com",
     description="BERTopic performs topic Modeling with state-of-the-art transformer models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MaartenGr/BERTopic",
     project_urls={
@@ -74,22 +74,22 @@
         "License :: OSI Approved :: MIT License",
         "Topic :: Scientific/Engineering",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Operating System :: MacOS",
         "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.8",
     ],
     install_requires=base_packages,
     extras_require={
         "test": test_packages,
         "docs": docs_packages,
         "dev": dev_packages,
         "flair": flair_packages,
         "spacy": spacy_packages,
         "use": use_packages,
         "gensim": gensim_packages
     },
-    python_requires='>=3.6',
+    python_requires='>=3.7',
 )
```

### Comparing `bertopic-0.9.3/tests/test_bertopic.py` & `bertopic-0.9.4/tests/test_bertopic.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/tests/test_models.py` & `bertopic-0.9.4/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
                               "ID": range(len(newsgroup_docs)),
                               "Topic": np.random.randint(-1, nr_topics, len(newsgroup_docs))})
     documents_per_topic = documents.groupby(['Topic'], as_index=False).agg({'Document': ' '.join})
     documents = base_bertopic._preprocess_text(documents_per_topic.Document.values)
     count = base_bertopic.vectorizer_model.fit(documents)
     words = count.get_feature_names()
     X = count.transform(documents)
-    transformer = ClassTFIDF().fit(X, n_samples=len(newsgroup_docs))
+    transformer = ClassTFIDF().fit(X)
     c_tf_idf = transformer.transform(X)
 
     assert len(words) > 1000
     assert all([isinstance(x, str) for x in words])
 
     assert isinstance(X, csr_matrix)
     assert isinstance(c_tf_idf, csr_matrix)
@@ -214,15 +214,15 @@
                               "ID": range(len(newsgroup_docs)),
                               "Topic": np.random.randint(-1, nr_topics, len(newsgroup_docs))})
     documents_per_topic = documents.groupby(['Topic'], as_index=False).agg({'Document': ' '.join})
     documents = model._preprocess_text(documents_per_topic.Document.values)
     count = model.vectorizer_model.fit(documents)
     words = count.get_feature_names()
     X = count.transform(documents)
-    transformer = ClassTFIDF().fit(X, n_samples=len(newsgroup_docs))
+    transformer = ClassTFIDF().fit(X)
     c_tf_idf = transformer.transform(X)
 
     assert len(words) > 1000
     assert all([isinstance(x, str) for x in words])
 
     assert isinstance(X, csr_matrix)
     assert isinstance(c_tf_idf, csr_matrix)
```

### Comparing `bertopic-0.9.3/tests/test_other.py` & `bertopic-0.9.4/tests/test_other.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/tests/test_topic_representation.py` & `bertopic-0.9.4/tests/test_topic_representation.py`

 * *Files identical despite different names*

### Comparing `bertopic-0.9.3/tests/test_utils.py` & `bertopic-0.9.4/tests/test_utils.py`

 * *Files identical despite different names*

