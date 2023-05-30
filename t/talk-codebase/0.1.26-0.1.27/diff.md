# Comparing `tmp/talk_codebase-0.1.26.tar.gz` & `tmp/talk_codebase-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.26.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.27.tar", max compression
```

## Comparing `talk_codebase-0.1.26.tar` & `talk_codebase-0.1.27.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1845 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/README.md
--rw-r--r--   0        0        0      888 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/pyproject.toml
--rw-r--r--   0        0        0     4442 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/talk_codebase/LLM.py
--rw-r--r--   0        0        0        0 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/talk_codebase/__init__.py
--rw-r--r--   0        0        0     3009 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/talk_codebase/cli.py
--rw-r--r--   0        0        0     1717 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/talk_codebase/consts.py
--rw-r--r--   0        0        0     2403 2023-05-30 07:23:49.083089 talk_codebase-0.1.26/talk_codebase/utils.py
--rw-r--r--   0        0        0     2847 1970-01-01 00:00:00.000000 talk_codebase-0.1.26/PKG-INFO
+-rw-r--r--   0        0        0     2866 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/README.md
+-rw-r--r--   0        0        0      888 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/pyproject.toml
+-rw-r--r--   0        0        0     4442 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/talk_codebase/LLM.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     2880 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/talk_codebase/cli.py
+-rw-r--r--   0        0        0     1717 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2403 2023-05-30 10:52:44.164284 talk_codebase-0.1.27/talk_codebase/utils.py
+-rw-r--r--   0        0        0     3868 1970-01-01 00:00:00.000000 talk_codebase-0.1.27/PKG-INFO
```

### Comparing `talk_codebase-0.1.26/pyproject.toml` & `talk_codebase-0.1.27/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.26"
+version = "0.1.27"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.26/talk_codebase/LLM.py` & `talk_codebase-0.1.27/talk_codebase/LLM.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.26/talk_codebase/cli.py` & `talk_codebase-0.1.27/talk_codebase/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 import fire
 import questionary
 import yaml
 
 from talk_codebase.LLM import factory_llm
 from talk_codebase.consts import DEFAULT_CONFIG
 
+config_path = os.path.join(os.path.expanduser("~"), ".talk_codebase_config.yaml")
+
 
 def get_config():
-    home_dir = os.path.expanduser("~")
-    config_path = os.path.join(home_dir, ".config.yaml")
     print(f"🤖 Loading config from {config_path}:")
     if os.path.exists(config_path):
         with open(config_path, "r") as f:
             config = yaml.safe_load(f)
     else:
         config = {}
     return config
 
 
 def save_config(config):
     home_dir = os.path.expanduser("~")
-    config_path = os.path.join(home_dir, ".config.yaml")
     with open(config_path, "w") as f:
         yaml.dump(config, f)
 
 
 def configure():
     config = get_config()
     model_type = questionary.select(
@@ -63,20 +62,20 @@
 def validate_config(config):
     for key, value in DEFAULT_CONFIG.items():
         if key not in config:
             config[key] = value
     if config.get("model_type") == "openai":
         api_key = config.get("api_key")
         if not api_key:
-            print("🤖 Please configure your API key. Use talk-codebase configure --model_type=openai")
+            print("🤖 Please configure your API key. Use talk-codebase configure")
             exit(0)
     elif config.get("model_type") == "local":
         model_path = config.get("model_path")
         if not model_path:
-            print("🤖 Please configure your model path. Use talk-codebase configure --model_type=local")
+            print("🤖 Please configure your model path. Use talk-codebase configure")
             exit(0)
     save_config(config)
     return config
 
 
 def chat(root_dir):
     config = validate_config(get_config())
@@ -90,14 +89,14 @@
             "chat": chat,
             "configure": configure
         })
     except KeyboardInterrupt:
         print("\n🤖 Bye!")
     except Exception as e:
         if str(e) == "<empty message>":
-            print("🤖 Please configure your API key. Use talk-codebase configure --model_type=openai")
+            print("🤖 Please configure your API key. Use talk-codebase configure")
         else:
             raise e
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `talk_codebase-0.1.26/talk_codebase/consts.py` & `talk_codebase-0.1.27/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.26/talk_codebase/utils.py` & `talk_codebase-0.1.27/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.26/PKG-INFO` & `talk_codebase-0.1.27/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: talk-codebase
-Version: 0.1.26
-Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
-Keywords: chatgpt,openai,cli
-Author: Saryev Rustam
-Author-email: rustam1997@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
-Requires-Dist: fire (>=0.5.0,<0.6.0)
-Requires-Dist: gitpython (>=3.1.31,<4.0.0)
-Requires-Dist: gpt4all (>=0.2.3,<0.3.0)
-Requires-Dist: halo (>=0.0.31,<0.0.32)
-Requires-Dist: langchain (>=0.0.181,<0.0.182)
-Requires-Dist: openai (>=0.27.7,<0.28.0)
-Requires-Dist: questionary (>=1.10.0,<2.0.0)
-Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
-Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
-Requires-Dist: unstructured (>=0.6.10,<0.7.0)
-Requires-Dist: urllib3 (==1.26.6)
-Description-Content-Type: text/markdown
-
 ## talk-codebase: Tool for chatting with your codebase and docs using OpenAI, LlamaCpp, and GPT-4-All
 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
@@ -40,42 +14,68 @@
 not for production use.
 
 ## Installation
 
 To install `talk-codebase`, you need to have Python 3.9 and an OpenAI API
 key [api-keys](https://platform.openai.com/account/api-keys).
 Additionally, if you want to use the GPT4All model, you need to download
-the [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) model and specify its
+the [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) model. If you prefer a
+different model, you can download it from [GPT4All](https://gpt4all.io) and configure path to it in the configuration
+and specify its
 path in the configuration. If you want some files to be ignored, add them to .gitignore.
 
 To install `talk-codebase`, run the following command in your terminal:
 
 ```bash
 pip install talk-codebase
 ```
 
 Once `talk-codebase` is installed, you can use it to chat with your codebase by running the following command:
 
 ```bash
-talk-codebase chat
+talk-codebase chat <path-to-your-codebase>
 ```
 
 If you need to configure or edit the configuration, you can run:
 
 ```bash
 talk-codebase configure
 ```
 
+You can also edit the configuration manually by editing the `~/.config.yaml` file.
+If for some reason you cannot find the configuration file, just run the tool and at the very beginning it will output
+the path to the configuration file.
+
+```yaml
+# The OpenAI API key. You can get it from https://beta.openai.com/account/api-keys
+api_key: sk-xxx
+# maximum overlap between chunks. It can be nice to have some overlap to maintain some continuity between chunks
+chunk_overlap: '50'
+# maximum size of a chunk
+chunk_size: '500'
+# number of samples to generate for each prompt.
+k: '4'
+# maximum tokens for the LLMs
+max_tokens: '1048'
+# token limit for the LLM model only OpenAI
+model_name: gpt-3.5-turbo
+# path to the llm file on disk.
+model_path: models/ggml-gpt4all-j-v1.3-groovy.bin
+# type of the LLM model. It can be either local or openai
+model_type: openai
+
+```
+
 ## The supported extensions:
 
 - [x] `.csv`
 - [x] `.doc`
 - [x] `.docx`
 - [x] `.epub`
 - [x] `.md`
 - [x] `.pdf`
 - [x] `.txt`
 - [x] `popular programming languages`
 
 ## Contributing
 
-Contributions are always welcome!
+Contributions are always welcome!
```

