# Comparing `tmp/text2text-1.0.1.tar.gz` & `tmp/text2text-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.0.1.tar", last modified: Mon May 29 23:38:44 2023, max compression
+gzip compressed data, was "text2text-1.0.2.tar", last modified: Tue May 30 00:03:29 2023, max compression
```

## Comparing `text2text-1.0.1.tar` & `text2text-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:38:44.315004 text2text-1.0.1/
--rwxr-xr-x   0 root         (0) root         (0)     1337 2023-05-29 23:12:34.000000 text2text-1.0.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    60334 2023-05-29 23:38:44.315004 text2text-1.0.1/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    59520 2023-05-29 22:48:34.000000 text2text-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 23:38:44.315004 text2text-1.0.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1229 2023-05-29 23:37:58.000000 text2text-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:38:44.312004 text2text-1.0.1/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      666 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-29 23:34:43.000000 text2text-1.0.1/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:38:44.313004 text2text-1.0.1/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:38:44.315004 text2text-1.0.1/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-05-29 23:35:06.000000 text2text-1.0.1/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/searcher.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-29 22:48:34.000000 text2text-1.0.1/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:38:44.313004 text2text-1.0.1/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    60334 2023-05-29 23:38:44.000000 text2text-1.0.1/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2023-05-29 23:38:44.000000 text2text-1.0.1/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 23:38:44.000000 text2text-1.0.1/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      124 2023-05-29 23:38:44.000000 text2text-1.0.1/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-29 23:38:44.000000 text2text-1.0.1/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:03:29.633010 text2text-1.0.2/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-05-29 23:46:11.000000 text2text-1.0.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    60436 2023-05-30 00:03:29.633010 text2text-1.0.2/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    59622 2023-05-29 23:43:37.000000 text2text-1.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 00:03:29.633010 text2text-1.0.2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1229 2023-05-29 23:44:03.000000 text2text-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:03:29.630010 text2text-1.0.2/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-29 23:34:43.000000 text2text-1.0.2/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:03:29.631009 text2text-1.0.2/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:03:29.632010 text2text-1.0.2/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-05-29 23:35:06.000000 text2text-1.0.2/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/searcher.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-29 22:48:34.000000 text2text-1.0.2/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:03:29.631009 text2text-1.0.2/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    60436 2023-05-30 00:03:29.000000 text2text-1.0.2/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-05-30 00:03:29.000000 text2text-1.0.2/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:03:29.000000 text2text-1.0.2/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2023-05-30 00:03:29.000000 text2text-1.0.2/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-30 00:03:29.000000 text2text-1.0.2/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.0.1/LICENSE.txt` & `text2text-1.0.2/LICENSE.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 This open source software utilizes other open source components with their own 
 licensing agreements. As the consumer of this software, you agree to abide by 
-the licensing requirements set forth by the respective components used.
+the licensing requirements set forth by the respective components used, e.g.
+Assistant is based on the LLaMA model, which is non-commercially licensed.
 
 The MIT License (MIT)
 
 Copyright (c) Artit Wangperawong
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `text2text-1.0.1/PKG-INFO` & `text2text-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.1
+Version: 1.0.2
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -743,17 +743,21 @@
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Assistant
-Not chatGPT level but it works
+Based on LLaMA, which is not commercially licensed.
 ```
-res = t2t.Handler(["Outline steps for contributing to open source code"]).assist()
+instructions = """
+Generate a JSON output mapping with keys as English characters and values as Greek equivalents.
+{
+"""
+res = t2t.Handler([instructions]).assist()
 # 1) Find an open source project that you are interested in. You can do this by searching the internet for the project name or using a search engine to find the project page on GitHub.
 # 2) Verify that you have the necessary permissions to make changes to the code. If the project uses basic permissions, you can use git to check out the code. If the code uses more advanced permissions, you can find a way to use those permissions.
 # 3) Perform a code review to ensure that your contributions are properly credits and, if necessary, include a reasoning of your changes.
 ```
 
 ### Training / Finetuning
 Finetune cross-lingual model on your data
```

### Comparing `text2text-1.0.1/README.md` & `text2text-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -729,17 +729,21 @@
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Assistant
-Not chatGPT level but it works
+Based on LLaMA, which is not commercially licensed.
 ```
-res = t2t.Handler(["Outline steps for contributing to open source code"]).assist()
+instructions = """
+Generate a JSON output mapping with keys as English characters and values as Greek equivalents.
+{
+"""
+res = t2t.Handler([instructions]).assist()
 # 1) Find an open source project that you are interested in. You can do this by searching the internet for the project name or using a search engine to find the project page on GitHub.
 # 2) Verify that you have the necessary permissions to make changes to the code. If the project uses basic permissions, you can use git to check out the code. If the code uses more advanced permissions, you can find a way to use those permissions.
 # 3) Perform a code review to ensure that your contributions are properly credits and, if necessary, include a reasoning of your changes.
 ```
 
 ### Training / Finetuning
 Finetune cross-lingual model on your data
```

### Comparing `text2text-1.0.1/setup.py` & `text2text-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.0.1",
+  version="1.0.2",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.0.1/text2text/__init__.py` & `text2text-1.0.2/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/abstractor.py` & `text2text-1.0.2/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/answerer.py` & `text2text-1.0.2/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/assistant.py` & `text2text-1.0.2/text2text/assistant.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/biunilm/loader_utils.py` & `text2text-1.0.2/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/biunilm/seq2seq_loader.py` & `text2text-1.0.2/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/bm25er.py` & `text2text-1.0.2/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/counter.py` & `text2text-1.0.2/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/fitter.py` & `text2text-1.0.2/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/handler.py` & `text2text-1.0.2/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/identifier.py` & `text2text-1.0.2/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/indexer.py` & `text2text-1.0.2/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/measurer.py` & `text2text-1.0.2/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.0.2/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.0.2/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.0.2/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.0.2/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.0.2/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/questioner.py` & `text2text-1.0.2/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/responder.py` & `text2text-1.0.2/text2text/responder.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/searcher.py` & `text2text-1.0.2/text2text/searcher.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/server.py` & `text2text-1.0.2/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/summarizer.py` & `text2text-1.0.2/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/tfidfer.py` & `text2text-1.0.2/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/tokenizer.py` & `text2text-1.0.2/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/transformer.py` & `text2text-1.0.2/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/translator.py` & `text2text-1.0.2/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text/vectorizer.py` & `text2text-1.0.2/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.1/text2text.egg-info/PKG-INFO` & `text2text-1.0.2/text2text.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.1
+Version: 1.0.2
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -743,17 +743,21 @@
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Assistant
-Not chatGPT level but it works
+Based on LLaMA, which is not commercially licensed.
 ```
-res = t2t.Handler(["Outline steps for contributing to open source code"]).assist()
+instructions = """
+Generate a JSON output mapping with keys as English characters and values as Greek equivalents.
+{
+"""
+res = t2t.Handler([instructions]).assist()
 # 1) Find an open source project that you are interested in. You can do this by searching the internet for the project name or using a search engine to find the project page on GitHub.
 # 2) Verify that you have the necessary permissions to make changes to the code. If the project uses basic permissions, you can use git to check out the code. If the code uses more advanced permissions, you can find a way to use those permissions.
 # 3) Perform a code review to ensure that your contributions are properly credits and, if necessary, include a reasoning of your changes.
 ```
 
 ### Training / Finetuning
 Finetune cross-lingual model on your data
```

### Comparing `text2text-1.0.1/text2text.egg-info/SOURCES.txt` & `text2text-1.0.2/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

