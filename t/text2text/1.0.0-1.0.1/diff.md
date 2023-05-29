# Comparing `tmp/text2text-1.0.0.tar.gz` & `tmp/text2text-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.0.0.tar", last modified: Sat May 13 23:07:45 2023, max compression
+gzip compressed data, was "text2text-1.0.1.tar", last modified: Mon May 29 23:38:44 2023, max compression
```

## Comparing `text2text-1.0.0.tar` & `text2text-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 23:07:45.611461 text2text-1.0.0/
--rwxr-xr-x   0 root         (0) root         (0)     1334 2023-05-13 22:14:45.000000 text2text-1.0.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    60334 2023-05-13 23:07:45.611461 text2text-1.0.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    59520 2023-05-13 23:04:11.000000 text2text-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-13 23:07:45.611461 text2text-1.0.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1225 2023-05-13 23:04:31.000000 text2text-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 23:07:45.607460 text2text-1.0.0/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      666 2023-05-13 22:39:09.000000 text2text-1.0.0/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     9928 2023-05-13 22:49:09.000000 text2text-1.0.0/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 23:07:45.609460 text2text-1.0.0/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-05-13 22:47:11.000000 text2text-1.0.0/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 23:07:45.610461 text2text-1.0.0/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-05-13 22:15:54.000000 text2text-1.0.0/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/searcher.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-05-13 22:19:58.000000 text2text-1.0.0/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 23:07:45.608461 text2text-1.0.0/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    60334 2023-05-13 23:07:45.000000 text2text-1.0.0/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2023-05-13 23:07:45.000000 text2text-1.0.0/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-13 23:07:45.000000 text2text-1.0.0/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      127 2023-05-13 23:07:45.000000 text2text-1.0.0/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-13 23:07:45.000000 text2text-1.0.0/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:38:44.315004 text2text-1.0.1/
+-rwxr-xr-x   0 root         (0) root         (0)     1337 2023-05-29 23:12:34.000000 text2text-1.0.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    60334 2023-05-29 23:38:44.315004 text2text-1.0.1/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    59520 2023-05-29 22:48:34.000000 text2text-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 23:38:44.315004 text2text-1.0.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1229 2023-05-29 23:37:58.000000 text2text-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:38:44.312004 text2text-1.0.1/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-29 23:34:43.000000 text2text-1.0.1/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:38:44.313004 text2text-1.0.1/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:38:44.315004 text2text-1.0.1/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-05-29 23:35:06.000000 text2text-1.0.1/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/searcher.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:38:44.313004 text2text-1.0.1/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    60334 2023-05-29 23:38:44.000000 text2text-1.0.1/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-05-29 23:38:44.000000 text2text-1.0.1/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 23:38:44.000000 text2text-1.0.1/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2023-05-29 23:38:44.000000 text2text-1.0.1/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-29 23:38:44.000000 text2text-1.0.1/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.0.0/LICENSE.txt` & `text2text-1.0.1/LICENSE.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-I am providing code in the repository to you under an open source license. Because this is my personal repository, the license you receive to my code is from me and not my employer (Facebook).
+This open source software utilizes other open source components with their own 
+licensing agreements. As the consumer of this software, you agree to abide by 
+the licensing requirements set forth by the respective components used.
 
 The MIT License (MIT)
 
 Copyright (c) Artit Wangperawong
-Copyright (c) Microsoft Corporation
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `text2text-1.0.0/PKG-INFO` & `text2text-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.0
+Version: 1.0.1
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2text-1.0.0/README.md` & `text2text-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/setup.py` & `text2text-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.0.0",
+  version="1.0.1",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
@@ -18,19 +18,20 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
   ],
   keywords='multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot',
   install_requires=[
     'accelerate',
     'bitsandbytes',
+    'peft',
     'faiss-cpu',
     'flask',
     'googledrivedownloader',
     'numpy',
     'pandas',
     'scipy',
     'sentencepiece',
     'torch',
     'tqdm',
-    'transformers==4.25.1',
+    'transformers',
   ],
 )
```

### Comparing `text2text-1.0.0/text2text/__init__.py` & `text2text-1.0.1/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/abstractor.py` & `text2text-1.0.1/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/answerer.py` & `text2text-1.0.1/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/biunilm/loader_utils.py` & `text2text-1.0.1/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/biunilm/seq2seq_loader.py` & `text2text-1.0.1/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/bm25er.py` & `text2text-1.0.1/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/counter.py` & `text2text-1.0.1/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/fitter.py` & `text2text-1.0.1/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/handler.py` & `text2text-1.0.1/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/identifier.py` & `text2text-1.0.1/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/indexer.py` & `text2text-1.0.1/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/measurer.py` & `text2text-1.0.1/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.0.1/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.0.1/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.0.1/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.0.1/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.0.1/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/questioner.py` & `text2text-1.0.1/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/responder.py` & `text2text-1.0.1/text2text/responder.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,17 @@
       pretrained_model = self.__class__.pretrained_model
     self.__class__.tokenizer = AutoTokenizer.from_pretrained(pretrained_model)
     self.__class__.model = AutoModelForSeq2SeqLM.from_pretrained(pretrained_model, device_map="auto", load_in_8bit=True)
 
   def _get_responses(self, input_lines):
     tokenizer = self.__class__.tokenizer
     model = self.__class__.model
-
     inputs = tokenizer(input_lines, return_tensors="pt", padding=True)
-
     outputs = model.generate(
-        input_ids=inputs['input_ids'],
+        input_ids=inputs['input_ids'].to(model.device),
         attention_mask=inputs['attention_mask'],
         max_length=128, min_length=8,
     )
 
     return [tokenizer.decode(out, skip_special_tokens=True) for out in outputs]
 
   def transform(self, input_lines, src_lang='en', knowledge_base=None, **kwargs):
```

### Comparing `text2text-1.0.0/text2text/searcher.py` & `text2text-1.0.1/text2text/searcher.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/server.py` & `text2text-1.0.1/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/summarizer.py` & `text2text-1.0.1/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/tfidfer.py` & `text2text-1.0.1/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/tokenizer.py` & `text2text-1.0.1/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/transformer.py` & `text2text-1.0.1/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/translator.py` & `text2text-1.0.1/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text/vectorizer.py` & `text2text-1.0.1/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.0/text2text.egg-info/PKG-INFO` & `text2text-1.0.1/text2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.0
+Version: 1.0.1
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2text-1.0.0/text2text.egg-info/SOURCES.txt` & `text2text-1.0.1/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

