# Comparing `tmp/talk_codebase-0.1.22.tar.gz` & `tmp/talk_codebase-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.22.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.23.tar", max compression
```

## Comparing `talk_codebase-0.1.22.tar` & `talk_codebase-0.1.23.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      866 2023-05-29 12:31:03.637641 talk_codebase-0.1.22/README.md
--rw-r--r--   0        0        0      811 2023-05-29 12:31:03.637641 talk_codebase-0.1.22/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 12:31:03.641641 talk_codebase-0.1.22/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1974 2023-05-29 12:31:03.641641 talk_codebase-0.1.22/talk_codebase/cli.py
--rw-r--r--   0        0        0      518 2023-05-29 12:31:03.641641 talk_codebase-0.1.22/talk_codebase/consts.py
--rw-r--r--   0        0        0     2872 2023-05-29 12:31:03.641641 talk_codebase-0.1.22/talk_codebase/llm.py
--rw-r--r--   0        0        0     1568 2023-05-29 12:31:03.641641 talk_codebase-0.1.22/talk_codebase/utils.py
--rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 talk_codebase-0.1.22/PKG-INFO
+-rw-r--r--   0        0        0     1480 2023-05-29 22:14:20.629669 talk_codebase-0.1.23/README.md
+-rw-r--r--   0        0        0      863 2023-05-29 22:14:20.633669 talk_codebase-0.1.23/pyproject.toml
+-rw-r--r--   0        0        0     4362 2023-05-29 22:14:20.633669 talk_codebase-0.1.23/talk_codebase/LLM.py
+-rw-r--r--   0        0        0        0 2023-05-29 22:14:20.633669 talk_codebase-0.1.23/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     3028 2023-05-29 22:14:20.633669 talk_codebase-0.1.23/talk_codebase/cli.py
+-rw-r--r--   0        0        0      814 2023-05-29 22:14:20.633669 talk_codebase-0.1.23/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2025 2023-05-29 22:14:20.633669 talk_codebase-0.1.23/talk_codebase/utils.py
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 talk_codebase-0.1.23/PKG-INFO
```

### Comparing `talk_codebase-0.1.22/pyproject.toml` & `talk_codebase-0.1.23/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.22"
+version = "0.1.23"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
@@ -14,14 +14,16 @@
 openai = "^0.27.7"
 tiktoken = "^0.4.0"
 faiss-cpu = "^1.7.4"
 halo = "^0.0.31"
 urllib3 = "1.26.6"
 gitpython = "^3.1.31"
 questionary = "^1.10.0"
+gpt4all = "^0.2.3"
+sentence-transformers = "^2.2.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project.urls]
```

### Comparing `talk_codebase-0.1.22/talk_codebase/cli.py` & `talk_codebase-0.1.23/talk_codebase/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import os
 
 import fire
+import questionary
 import yaml
 
-from talk_codebase.llm import create_vector_store, send_question
+from talk_codebase.LLM import factory_llm
+from talk_codebase.consts import DEFAULT_CONFIG
 
 
 def get_config():
     home_dir = os.path.expanduser("~")
     config_path = os.path.join(home_dir, ".config.yaml")
+    print(f"🤖 Loading config from {config_path}:")
     if os.path.exists(config_path):
         with open(config_path, "r") as f:
             config = yaml.safe_load(f)
     else:
         config = {}
     return config
 
@@ -22,55 +25,79 @@
     config_path = os.path.join(home_dir, ".config.yaml")
     with open(config_path, "w") as f:
         yaml.dump(config, f)
 
 
 def configure():
     config = get_config()
-    api_key = input("🤖 Enter your OpenAI API key: ")
-    model_name = input("🤖 Enter your model name (default: gpt-3.5-turbo): ") or "gpt-3.5-turbo"
-    config["api_key"] = api_key
-    config["model_name"] = model_name
+    model_type = questionary.select(
+        "🤖 Select model type:",
+        choices=[
+            {"name": "OpenAI", "value": "openai"},
+            {"name": "Local", "value": "local"},
+        ]
+    ).ask()
+    config["model_type"] = model_type
+    if model_type == "openai":
+        api_key = input("🤖 Enter your OpenAI API key: ")
+        model_name = input("🤖 Enter your model name (default: gpt-3.5-turbo): ")
+        config["model_name"] = model_name if model_name else DEFAULT_CONFIG["model_name"]
+        config["api_key"] = api_key
+    elif model_type == "local":
+        model_path = input(f"🤖 Enter your model path: (default: {DEFAULT_CONFIG['model_path']}) ")
+        config["model_path"] = model_path if model_path else DEFAULT_CONFIG["model_path"]
     save_config(config)
+    print("🤖 Configuration saved!")
 
 
-def loop(vector_store, api_key, model_name):
+def loop(llm):
     while True:
-        question = input("👉 ")
+        question = input("👉 ").lower().strip()
         if not question:
             print("🤖 Please enter a question.")
             continue
-        if question.lower() in ('exit', 'quit'):
+        if question in ('exit', 'quit'):
             break
-        send_question(question, vector_store, api_key, model_name)
+        llm.send_question(question)
+
+
+def validate_config(config):
+    for key, value in DEFAULT_CONFIG.items():
+        if key not in config:
+            config[key] = value
+    if config.get("model_type") == "openai":
+        api_key = config.get("api_key")
+        if not api_key:
+            print("🤖 Please configure your API key. Use talk-codebase configure --model_type=openai")
+            exit(0)
+    elif config.get("model_type") == "local":
+        model_path = config.get("model_path")
+        if not model_path:
+            print("🤖 Please configure your model path. Use talk-codebase configure --model_type=local")
+            exit(0)
+    save_config(config)
+    return config
 
 
 def chat(root_dir):
+    config = validate_config(get_config())
+    llm = factory_llm(root_dir, config)
+    loop(llm)
+
+
+def main():
     try:
-        config = get_config()
-        api_key = config.get("api_key")
-        model_name = config.get("model_name")
-        if not (api_key and model_name):
-            configure()
-            chat(root_dir)
-        vector_store = create_vector_store(root_dir, api_key, model_name)
-        loop(vector_store, api_key, model_name)
+        fire.Fire({
+            "chat": chat,
+            "configure": configure
+        })
     except KeyboardInterrupt:
         print("\n🤖 Bye!")
     except Exception as e:
         if str(e) == "<empty message>":
-            print("🤖 Please configure your API key.")
-            configure()
-            chat(root_dir)
+            print("🤖 Please configure your API key. Use talk-codebase configure --model_type=openai")
         else:
-            print(f"\n🤖 Error: {e}")
-
-
-def main():
-    fire.Fire({
-        "chat": chat,
-        "configure": configure,
-    })
+            raise e
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `talk_codebase-0.1.22/talk_codebase/consts.py` & `talk_codebase-0.1.23/talk_codebase/consts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,6 +1,16 @@
 EXCLUDE_DIRS = ['__pycache__', '.venv', '.git', '.idea', 'venv', 'env', 'node_modules', 'dist', 'build', '.vscode',
                 '.github', '.gitlab']
 ALLOW_FILES = ['.txt', '.js', '.mjs', '.ts', '.tsx', '.css', '.scss', '.less', '.html', '.htm', '.json', '.py',
                '.java', '.c', '.cpp', '.cs', '.go', '.php', '.rb', '.rs', '.swift', '.kt', '.scala', '.m', '.h',
                '.sh', '.pl', '.pm', '.lua', '.sql']
 EXCLUDE_FILES = ['requirements.txt', 'package.json', 'package-lock.json', 'yarn.lock']
+DEFAULT_MODEL_PATH = "models/ggml-gpt4all-j-v1.3-groovy.bin"
+DEFAULT_CONFIG = {
+    "max_tokens": "1048",
+    "chunk_size": "500",
+    "chunk_overlap": "50",
+    "k": "4",
+    "model_name": "gpt-3.5-turbo",
+    "model_path": "models/ggml-gpt4all-j-v1.3-groovy.bin",
+    "model_type": "openai",
+}
```

### Comparing `talk_codebase-0.1.22/PKG-INFO` & `talk_codebase-0.1.23/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.22
+Version: 0.1.23
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
+Requires-Dist: gpt4all (>=0.2.3,<0.3.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: langchain (>=0.0.181,<0.0.182)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
+Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: urllib3 (==1.26.6)
 Description-Content-Type: text/markdown
 
-# talk-codebase is a powerful tool for chatting with your codebase
+# talk-codebase: A Tool for Chatting with Your Codebase
 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
 
+## Description
+
+Talk-codebase is a powerful tool that allows you to converse with your codebase. It uses LLMs to answer your queries.
+
+You can use [GPT4All](https://github.com/nomic-ai/gpt4all) for offline code processing without sharing your code with
+third parties. Alternatively, you can use OpenAI if privacy is not a concern for you. You can switch between these two
+options quickly and easily.
+
 ## Installation
 
 ```bash
 pip install talk-codebase
 ```
 
 ## Usage
 
-talk-codebase works only with files of popular programming languages and additionally with .txt files. All other files
-will be ignored.
+Talk-codebase works only with files of popular programming languages and .txt files. All other files will be ignored.
 
 ```bash
 # Start chatting with your codebase
 talk-codebase chat <directory>
 
-# Configure
+# Configure or edit configuration ~/.config.yaml
 talk-codebase configure
 
 # Help
 talk-codebase --help
 ```
 
 ## Requirements
 
 - Python 3.9
 - OpenAI API key [api-keys](https://platform.openai.com/account/api-keys)
+- If you want to use GPT4All, you need to download the
+  model [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) and specify the path
+  to it in the configuration.
```

