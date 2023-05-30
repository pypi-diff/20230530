# Comparing `tmp/tree-of-thoughts-0.2.8.tar.gz` & `tmp/tree-of-thoughts-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.2.8.tar", last modified: Mon May 29 23:02:39 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.2.9.tar", last modified: Tue May 30 13:50:46 2023, max compression
```

## Comparing `tree-of-thoughts-0.2.8.tar` & `tree-of-thoughts-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:02:39.691873 tree-of-thoughts-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 23:02:18.000000 tree-of-thoughts-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-29 23:02:39.691873 tree-of-thoughts-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-05-29 23:02:18.000000 tree-of-thoughts-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:02:39.691873 tree-of-thoughts-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:02:39.687873 tree-of-thoughts-0.2.8/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/tree_of_thoughts/abstractLanguageModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/tree_of_thoughts/guidanceModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/tree_of_thoughts/huggingModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/tree_of_thoughts/openaiModels.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-05-29 23:02:19.000000 tree-of-thoughts-0.2.8/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:02:39.691873 tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-29 23:02:39.000000 tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-29 23:02:39.000000 tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:02:39.000000 tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-29 23:02:39.000000 tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 23:02:39.000000 tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:50:46.783895 tree-of-thoughts-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 13:50:35.000000 tree-of-thoughts-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-30 13:50:46.783895 tree-of-thoughts-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-05-30 13:50:35.000000 tree-of-thoughts-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:50:46.783895 tree-of-thoughts-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-30 13:50:35.000000 tree-of-thoughts-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:50:46.783895 tree-of-thoughts-0.2.9/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-30 13:50:35.000000 tree-of-thoughts-0.2.9/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-30 13:50:35.000000 tree-of-thoughts-0.2.9/tree_of_thoughts/abstractLanguageModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-05-30 13:50:35.000000 tree-of-thoughts-0.2.9/tree_of_thoughts/guidanceModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-30 13:50:35.000000 tree-of-thoughts-0.2.9/tree_of_thoughts/huggingModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-30 13:50:35.000000 tree-of-thoughts-0.2.9/tree_of_thoughts/openaiModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10116 2023-05-30 13:50:35.000000 tree-of-thoughts-0.2.9/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:50:46.783895 tree-of-thoughts-0.2.9/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-30 13:50:46.000000 tree-of-thoughts-0.2.9/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-30 13:50:46.000000 tree-of-thoughts-0.2.9/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:50:46.000000 tree-of-thoughts-0.2.9/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 13:50:46.000000 tree-of-thoughts-0.2.9/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 13:50:46.000000 tree-of-thoughts-0.2.9/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.2.8/LICENSE` & `tree-of-thoughts-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.8/PKG-INFO` & `tree-of-thoughts-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.2.8/README.md` & `tree-of-thoughts-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,20 +49,20 @@
 ```pip install tree-of-thoughts ```
 
 
 Create a Python script (e.g., example.py) and import the necessary classes:
 
 ``` python
 import os
-from tree_of_thoughts.openaiModels import OpenAILanguageModel
+from tree_of_thoughts.openaiModels import OptimizedOpenAILanguageModel
 from tree_of_thoughts.treeofthoughts import TreeofThoughts
-from tree_of_thoughts.huggingModel import HuggingLanguageModel
 
 
-model = OptimizedOpenAILanguageModel(api_key='') # api_model="gpt4" # for higher performance base model is not smart
+api_key = os.getenv("OPENAI_API_KEY")
+model = OptimizedOpenAILanguageModel(api_key=api_key) # api_model="gpt4" # for higher performance base model is not smart
 
 
 #choose search algorithm('BFS' or 'DFS')
 search_algorithm = "BFS"
 
 #cot or propose
 strategy="cot"
```

### Comparing `tree-of-thoughts-0.2.8/setup.py` & `tree-of-thoughts-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.2.8',
+  version = '0.2.9',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
```

### Comparing `tree-of-thoughts-0.2.8/tree_of_thoughts/guidanceModels.py` & `tree-of-thoughts-0.2.9/tree_of_thoughts/guidanceModels.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.8/tree_of_thoughts/huggingModels.py` & `tree-of-thoughts-0.2.9/tree_of_thoughts/huggingModels.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.8/tree_of_thoughts/openaiModels.py` & `tree-of-thoughts-0.2.9/tree_of_thoughts/openaiModels.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.8/tree_of_thoughts/treeofthoughts.py` & `tree-of-thoughts-0.2.9/tree_of_thoughts/treeofthoughts.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
               convergence_threshold: Optional[float] = None, 
               convergence_count: Optional[int] = None) -> str:
         start_time = time.time()
         self.file_name = f"logs/tree_of_thoughts_output_{self.search_algorithm}.json"
         try:
             best_thoughts = ""
             if self.search_algorithm == 'BFS':
-                result = self.tot_bfs(initial_prompt, num_thoughts, max_steps, max_states, value_threshold, pruning_threshold)
+                result = self.tot_bfs(initial_prompt, num_thoughts, max_steps, max_states, pruning_threshold)
                 if result:
                     self.save_tree_to_json(self.file_name)
                     best_thoughts = result
             elif self.search_algorithm == 'DFS':
                 result = self.tot_dfs(initial_prompt, num_thoughts, max_steps, value_threshold, 
                                           confidence_threshold=confidence_threshold, max_iterations=max_iterations, convergence_threshold=convergence_threshold, 
                                           convergence_count=convergence_count)
```

### Comparing `tree-of-thoughts-0.2.8/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.2.9/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

