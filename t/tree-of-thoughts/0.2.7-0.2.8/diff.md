# Comparing `tmp/tree-of-thoughts-0.2.7.tar.gz` & `tmp/tree-of-thoughts-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.2.7.tar", last modified: Mon May 29 14:50:24 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.2.8.tar", last modified: Mon May 29 23:02:39 2023, max compression
```

## Comparing `tree-of-thoughts-0.2.7.tar` & `tree-of-thoughts-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:50:24.092428 tree-of-thoughts-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-29 14:50:24.092428 tree-of-thoughts-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 14:50:24.092428 tree-of-thoughts-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:50:24.092428 tree-of-thoughts-0.2.7/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/tree_of_thoughts/abstractLanguageModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/tree_of_thoughts/guidanceModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/tree_of_thoughts/huggingModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/tree_of_thoughts/openaiModels.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:50:24.092428 tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-29 14:50:24.000000 tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-29 14:50:24.000000 tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:50:24.000000 tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 14:50:24.000000 tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 14:50:24.000000 tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:02:39.691873 tree-of-thoughts-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 23:02:18.000000 tree-of-thoughts-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-29 23:02:39.691873 tree-of-thoughts-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-05-29 23:02:18.000000 tree-of-thoughts-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:02:39.691873 tree-of-thoughts-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:02:39.687873 tree-of-thoughts-0.2.8/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/tree_of_thoughts/abstractLanguageModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/tree_of_thoughts/guidanceModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/tree_of_thoughts/huggingModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/tree_of_thoughts/openaiModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:02:39.691873 tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-29 23:02:39.000000 tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-29 23:02:39.000000 tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:02:39.000000 tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-29 23:02:39.000000 tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 23:02:39.000000 tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.2.7/LICENSE` & `tree-of-thoughts-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.7/PKG-INFO` & `tree-of-thoughts-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.2.7
+Version: 0.2.8
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.2.7/README.md` & `tree-of-thoughts-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.7/setup.py` & `tree-of-thoughts-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.2.7',
+  version = '0.2.8',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
@@ -16,16 +16,14 @@
     'optimizers',
     "Prompt Engineering"
   ],
   install_requires=[
     'guidance',
     'openai',
     'transformers',
-    'dotenv',
-    ''
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

### Comparing `tree-of-thoughts-0.2.7/tree_of_thoughts/guidanceModels.py` & `tree-of-thoughts-0.2.8/tree_of_thoughts/guidanceModels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import guidance
 from tree_of_thoughts.abstractLanguageModel import AbstractLanguageModel
 import time
 import os
 import openai
-from dotenv import load_dotenv
-load_dotenv()
+
+
 class GuidanceLanguageModel(AbstractLanguageModel):
     def __init__(self, model, strategy="cot", evaluation_strategy="value", enable_ReAct_prompting=False):
         # gpt4 = guidance.llms.OpenAI("gpt-4")
         # vicuna = guidance.llms.transformers.Vicuna("your_path/vicuna_13B", device_map="auto")
         self.model = model
         
         # reference : https://www.promptingguide.ai/techniques/react
```

### Comparing `tree-of-thoughts-0.2.7/tree_of_thoughts/huggingModels.py` & `tree-of-thoughts-0.2.8/tree_of_thoughts/huggingModels.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.7/tree_of_thoughts/openaiModels.py` & `tree-of-thoughts-0.2.8/tree_of_thoughts/openaiModels.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.7/tree_of_thoughts/treeofthoughts.py` & `tree-of-thoughts-0.2.8/tree_of_thoughts/treeofthoughts.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.2.7
+Version: 0.2.8
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

