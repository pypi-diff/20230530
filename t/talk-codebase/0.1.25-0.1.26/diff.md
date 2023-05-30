# Comparing `tmp/talk_codebase-0.1.25.tar.gz` & `tmp/talk_codebase-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.25.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.26.tar", max compression
```

## Comparing `talk_codebase-0.1.25.tar` & `talk_codebase-0.1.26.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1684 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/README.md
--rw-r--r--   0        0        0      863 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/pyproject.toml
--rw-r--r--   0        0        0     4442 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/talk_codebase/LLM.py
--rw-r--r--   0        0        0        0 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/talk_codebase/__init__.py
--rw-r--r--   0        0        0     3009 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/talk_codebase/cli.py
--rw-r--r--   0        0        0      891 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/talk_codebase/consts.py
--rw-r--r--   0        0        0     2025 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/talk_codebase/utils.py
--rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 talk_codebase-0.1.25/PKG-INFO
+-rw-r--r--   0        0        0     1845 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/README.md
+-rw-r--r--   0        0        0      888 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/pyproject.toml
+-rw-r--r--   0        0        0     4442 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/talk_codebase/LLM.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     3009 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/talk_codebase/cli.py
+-rw-r--r--   0        0        0     1717 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2403 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/talk_codebase/utils.py
+-rw-r--r--   0        0        0     2847 1970-01-01 00:00:00.000000 talk_codebase-0.1.26/PKG-INFO
```

### Comparing `talk_codebase-0.1.25/README.md` & `talk_codebase-0.1.26/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,55 @@
-# talk-codebase: A Tool for Chatting with Your Codebase
+## talk-codebase: Tool for chatting with your codebase and docs using OpenAI, LlamaCpp, and GPT-4-All
 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
 
 ## Description
 
-Talk-codebase is a powerful tool that allows you to converse with your codebase. It uses LLMs to answer your queries.
+Talk-codebase is a tool that allows you to converse with your codebase using LLMs to answer your queries. It supports
+offline code processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third
+parties, or you can use OpenAI if privacy is not a concern for you. It is only recommended for educational purposes and
+not for production use.
 
-You can use [GPT4All](https://github.com/nomic-ai/gpt4all) for offline code processing without sharing your code with
-third parties. Alternatively, you can use OpenAI if privacy is not a concern for you. You can switch between these two
-options quickly and easily.
+## Installation
 
-Project created for educational purposes. It is not recommended to use it in production.
+To install `talk-codebase`, you need to have Python 3.9 and an OpenAI API
+key [api-keys](https://platform.openai.com/account/api-keys).
+Additionally, if you want to use the GPT4All model, you need to download
+the [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) model and specify its
+path in the configuration. If you want some files to be ignored, add them to .gitignore.
 
-## Installation
+To install `talk-codebase`, run the following command in your terminal:
 
 ```bash
 pip install talk-codebase
 ```
 
-## Usage
-
-Talk-codebase works only with files of popular programming languages and .txt files. All other files will be ignored.
-If you want some files to be ignored, add them to .gitignore.
+Once `talk-codebase` is installed, you can use it to chat with your codebase by running the following command:
 
 ```bash
-# Start chatting with your codebase
-talk-codebase chat <directory>
+talk-codebase chat
+```
 
-# Configure or edit configuration ~/.config.yaml
-talk-codebase configure
+If you need to configure or edit the configuration, you can run:
 
-# Help
-talk-codebase --help
+```bash
+talk-codebase configure
 ```
 
-## Requirements
+## The supported extensions:
 
-- Python 3.9
-- OpenAI API key [api-keys](https://platform.openai.com/account/api-keys)
-- If you want to use GPT4All, you need to download the
-  model [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) and specify the path
-  to it in the configuration.
+- [x] `.csv`
+- [x] `.doc`
+- [x] `.docx`
+- [x] `.epub`
+- [x] `.md`
+- [x] `.pdf`
+- [x] `.txt`
+- [x] `popular programming languages`
 
 ## Contributing
 
 Contributions are always welcome!
```

### Comparing `talk_codebase-0.1.25/pyproject.toml` & `talk_codebase-0.1.26/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.25"
+version = "0.1.26"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
@@ -16,14 +16,15 @@
 faiss-cpu = "^1.7.4"
 halo = "^0.0.31"
 urllib3 = "1.26.6"
 gitpython = "^3.1.31"
 questionary = "^1.10.0"
 gpt4all = "^0.2.3"
 sentence-transformers = "^2.2.2"
+unstructured = "^0.6.10"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project.urls]
```

### Comparing `talk_codebase-0.1.25/talk_codebase/LLM.py` & `talk_codebase-0.1.26/talk_codebase/LLM.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.25/talk_codebase/cli.py` & `talk_codebase-0.1.26/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.25/talk_codebase/utils.py` & `talk_codebase-0.1.26/talk_codebase/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import glob
+import multiprocessing
 import os
 import sys
 
 import tiktoken
 from git import Repo
-from halo import Halo
 from langchain import FAISS
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
-from langchain.document_loaders import TextLoader
 
-from talk_codebase.consts import EXCLUDE_FILES, ALLOW_FILES
+from talk_codebase.consts import LOADER_MAPPING, EXCLUDE_FILES
 
 
 def get_repo(root_dir):
     try:
         return Repo(root_dir)
     except:
         return None
@@ -39,24 +38,36 @@
 
     def on_llm_end(self, response, **kwargs):
         sys.stdout.write("\n")
         sys.stdout.flush()
 
 
 def load_files(root_dir):
-    spinners = Halo(text='Loading files', spinner='dots').start()
-    docs = []
-    for file_path in glob.glob(os.path.join(root_dir, '**/*'), recursive=True):
-        if is_ignored(file_path, root_dir):
-            continue
-        if any(file_path.endswith(allow_file) for allow_file in ALLOW_FILES) and not any(
-                file_path.endswith(exclude_file) for exclude_file in EXCLUDE_FILES):
-            loader = TextLoader(file_path, encoding='utf-8')
-            docs.extend(loader.load_and_split())
-    spinners.succeed(f"Loaded {len(docs)} documents")
+    num_cpus = multiprocessing.cpu_count()
+    loaded_files = []
+    with multiprocessing.Pool(num_cpus) as pool:
+        futures = []
+        for file_path in glob.glob(os.path.join(root_dir, '**/*'), recursive=True):
+            if is_ignored(file_path, root_dir):
+                continue
+            if any(
+                    file_path.endswith(exclude_file) for exclude_file in EXCLUDE_FILES):
+                continue
+            for ext in LOADER_MAPPING:
+                if file_path.endswith(ext):
+                    loader = LOADER_MAPPING[ext]['loader']
+                    args = LOADER_MAPPING[ext]['args']
+                    load = loader(file_path, **args)
+                    futures.append(pool.apply_async(load.load_and_split))
+                    loaded_files.append(file_path)
+        docs = []
+        for future in futures:
+            docs.extend(future.get())
+
+    print('\n' + '\n'.join([f'📄 {os.path.abspath(file_path)}:' for file_path in loaded_files]))
     return docs
 
 
 def calculate_cost(texts, model_name):
     enc = tiktoken.encoding_for_model(model_name)
     all_text = ''.join([text.page_content for text in texts])
     tokens = enc.encode(all_text)
```

### Comparing `talk_codebase-0.1.25/PKG-INFO` & `talk_codebase-0.1.26/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.25
+Version: 0.1.26
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -16,61 +16,66 @@
 Requires-Dist: gpt4all (>=0.2.3,<0.3.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: langchain (>=0.0.181,<0.0.182)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: unstructured (>=0.6.10,<0.7.0)
 Requires-Dist: urllib3 (==1.26.6)
 Description-Content-Type: text/markdown
 
-# talk-codebase: A Tool for Chatting with Your Codebase
+## talk-codebase: Tool for chatting with your codebase and docs using OpenAI, LlamaCpp, and GPT-4-All
 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
 
 ## Description
 
-Talk-codebase is a powerful tool that allows you to converse with your codebase. It uses LLMs to answer your queries.
+Talk-codebase is a tool that allows you to converse with your codebase using LLMs to answer your queries. It supports
+offline code processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third
+parties, or you can use OpenAI if privacy is not a concern for you. It is only recommended for educational purposes and
+not for production use.
 
-You can use [GPT4All](https://github.com/nomic-ai/gpt4all) for offline code processing without sharing your code with
-third parties. Alternatively, you can use OpenAI if privacy is not a concern for you. You can switch between these two
-options quickly and easily.
+## Installation
 
-Project created for educational purposes. It is not recommended to use it in production.
+To install `talk-codebase`, you need to have Python 3.9 and an OpenAI API
+key [api-keys](https://platform.openai.com/account/api-keys).
+Additionally, if you want to use the GPT4All model, you need to download
+the [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) model and specify its
+path in the configuration. If you want some files to be ignored, add them to .gitignore.
 
-## Installation
+To install `talk-codebase`, run the following command in your terminal:
 
 ```bash
 pip install talk-codebase
 ```
 
-## Usage
-
-Talk-codebase works only with files of popular programming languages and .txt files. All other files will be ignored.
-If you want some files to be ignored, add them to .gitignore.
+Once `talk-codebase` is installed, you can use it to chat with your codebase by running the following command:
 
 ```bash
-# Start chatting with your codebase
-talk-codebase chat <directory>
+talk-codebase chat
+```
 
-# Configure or edit configuration ~/.config.yaml
-talk-codebase configure
+If you need to configure or edit the configuration, you can run:
 
-# Help
-talk-codebase --help
+```bash
+talk-codebase configure
 ```
 
-## Requirements
+## The supported extensions:
 
-- Python 3.9
-- OpenAI API key [api-keys](https://platform.openai.com/account/api-keys)
-- If you want to use GPT4All, you need to download the
-  model [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) and specify the path
-  to it in the configuration.
+- [x] `.csv`
+- [x] `.doc`
+- [x] `.docx`
+- [x] `.epub`
+- [x] `.md`
+- [x] `.pdf`
+- [x] `.txt`
+- [x] `popular programming languages`
 
 ## Contributing
 
 Contributions are always welcome!
```

