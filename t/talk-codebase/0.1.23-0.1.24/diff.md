# Comparing `tmp/talk_codebase-0.1.23.tar.gz` & `tmp/talk_codebase-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.23.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.24.tar", max compression
```

## Comparing `talk_codebase-0.1.23.tar` & `talk_codebase-0.1.24.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1480 2023-05-29 22:14:20.629669 talk_codebase-0.1.23/README.md
--rw-r--r--   0        0        0      863 2023-05-29 22:14:20.633669 talk_codebase-0.1.23/pyproject.toml
--rw-r--r--   0        0        0     4362 2023-05-29 22:14:20.633669 talk_codebase-0.1.23/talk_codebase/LLM.py
--rw-r--r--   0        0        0        0 2023-05-29 22:14:20.633669 talk_codebase-0.1.23/talk_codebase/__init__.py
--rw-r--r--   0        0        0     3028 2023-05-29 22:14:20.633669 talk_codebase-0.1.23/talk_codebase/cli.py
--rw-r--r--   0        0        0      814 2023-05-29 22:14:20.633669 talk_codebase-0.1.23/talk_codebase/consts.py
--rw-r--r--   0        0        0     2025 2023-05-29 22:14:20.633669 talk_codebase-0.1.23/talk_codebase/utils.py
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 talk_codebase-0.1.23/PKG-INFO
+-rw-r--r--   0        0        0     1684 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/README.md
+-rw-r--r--   0        0        0      863 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/pyproject.toml
+-rw-r--r--   0        0        0     4359 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/talk_codebase/LLM.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     3009 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/talk_codebase/cli.py
+-rw-r--r--   0        0        0      814 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2025 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/talk_codebase/utils.py
+-rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 talk_codebase-0.1.24/PKG-INFO
```

### Comparing `talk_codebase-0.1.23/README.md` & `talk_codebase-0.1.24/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -10,23 +10,26 @@
 
 Talk-codebase is a powerful tool that allows you to converse with your codebase. It uses LLMs to answer your queries.
 
 You can use [GPT4All](https://github.com/nomic-ai/gpt4all) for offline code processing without sharing your code with
 third parties. Alternatively, you can use OpenAI if privacy is not a concern for you. You can switch between these two
 options quickly and easily.
 
+Project created for educational purposes. It is not recommended to use it in production.
+
 ## Installation
 
 ```bash
 pip install talk-codebase
 ```
 
 ## Usage
 
 Talk-codebase works only with files of popular programming languages and .txt files. All other files will be ignored.
+If you want some files to be ignored, add them to .gitignore.
 
 ```bash
 # Start chatting with your codebase
 talk-codebase chat <directory>
 
 # Configure or edit configuration ~/.config.yaml
 talk-codebase configure
@@ -37,8 +40,12 @@
 
 ## Requirements
 
 - Python 3.9
 - OpenAI API key [api-keys](https://platform.openai.com/account/api-keys)
 - If you want to use GPT4All, you need to download the
   model [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) and specify the path
-  to it in the configuration.
+  to it in the configuration.
+
+## Contributing
+
+Contributions are always welcome!
```

### Comparing `talk_codebase-0.1.23/pyproject.toml` & `talk_codebase-0.1.24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.23"
+version = "0.1.24"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.23/talk_codebase/LLM.py` & `talk_codebase-0.1.24/talk_codebase/LLM.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     def _create_store(self, root_dir):
         raise NotImplementedError("Subclasses must implement this method.")
 
     def _create_model(self):
         raise NotImplementedError("Subclasses must implement this method.")
 
-    def send_question(self, question):
+    def send_query(self, question):
         k = self.config.get("k")
         qa = RetrievalQA.from_chain_type(llm=self.llm, chain_type="stuff",
                                          retriever=self.vector_store.as_retriever(search_kwargs={"k": int(k)}),
                                          return_source_documents=True)
         answer = qa(question)
         print('\n' + '\n'.join([f'📄 {os.path.abspath(s.metadata["source"])}:' for s in answer["source_documents"]]))
```

### Comparing `talk_codebase-0.1.23/talk_codebase/cli.py` & `talk_codebase-0.1.24/talk_codebase/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,21 +47,21 @@
         config["model_path"] = model_path if model_path else DEFAULT_CONFIG["model_path"]
     save_config(config)
     print("🤖 Configuration saved!")
 
 
 def loop(llm):
     while True:
-        question = input("👉 ").lower().strip()
-        if not question:
-            print("🤖 Please enter a question.")
+        query = input("👉 ").lower().strip()
+        if not query:
+            print("🤖 Please enter a query")
             continue
-        if question in ('exit', 'quit'):
+        if query in ('exit', 'quit'):
             break
-        llm.send_question(question)
+        llm.send_query(query)
 
 
 def validate_config(config):
     for key, value in DEFAULT_CONFIG.items():
         if key not in config:
             config[key] = value
     if config.get("model_type") == "openai":
```

### Comparing `talk_codebase-0.1.23/talk_codebase/consts.py` & `talk_codebase-0.1.24/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.23/talk_codebase/utils.py` & `talk_codebase-0.1.24/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.23/PKG-INFO` & `talk_codebase-0.1.24/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.23
+Version: 0.1.24
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -35,23 +35,26 @@
 
 Talk-codebase is a powerful tool that allows you to converse with your codebase. It uses LLMs to answer your queries.
 
 You can use [GPT4All](https://github.com/nomic-ai/gpt4all) for offline code processing without sharing your code with
 third parties. Alternatively, you can use OpenAI if privacy is not a concern for you. You can switch between these two
 options quickly and easily.
 
+Project created for educational purposes. It is not recommended to use it in production.
+
 ## Installation
 
 ```bash
 pip install talk-codebase
 ```
 
 ## Usage
 
 Talk-codebase works only with files of popular programming languages and .txt files. All other files will be ignored.
+If you want some files to be ignored, add them to .gitignore.
 
 ```bash
 # Start chatting with your codebase
 talk-codebase chat <directory>
 
 # Configure or edit configuration ~/.config.yaml
 talk-codebase configure
@@ -63,7 +66,11 @@
 ## Requirements
 
 - Python 3.9
 - OpenAI API key [api-keys](https://platform.openai.com/account/api-keys)
 - If you want to use GPT4All, you need to download the
   model [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) and specify the path
   to it in the configuration.
+
+## Contributing
+
+Contributions are always welcome!
```

