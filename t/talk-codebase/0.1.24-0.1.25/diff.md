# Comparing `tmp/talk_codebase-0.1.24.tar.gz` & `tmp/talk_codebase-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.24.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.25.tar", max compression
```

## Comparing `talk_codebase-0.1.24.tar` & `talk_codebase-0.1.25.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1684 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/README.md
--rw-r--r--   0        0        0      863 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/pyproject.toml
--rw-r--r--   0        0        0     4359 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/talk_codebase/LLM.py
--rw-r--r--   0        0        0        0 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/talk_codebase/__init__.py
--rw-r--r--   0        0        0     3009 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/talk_codebase/cli.py
--rw-r--r--   0        0        0      814 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/talk_codebase/consts.py
--rw-r--r--   0        0        0     2025 2023-05-29 23:00:29.955920 talk_codebase-0.1.24/talk_codebase/utils.py
--rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 talk_codebase-0.1.24/PKG-INFO
+-rw-r--r--   0        0        0     1684 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/README.md
+-rw-r--r--   0        0        0      863 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/pyproject.toml
+-rw-r--r--   0        0        0     4442 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/talk_codebase/LLM.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     3009 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/talk_codebase/cli.py
+-rw-r--r--   0        0        0      891 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2025 2023-05-29 23:10:00.995816 talk_codebase-0.1.25/talk_codebase/utils.py
+-rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 talk_codebase-0.1.25/PKG-INFO
```

### Comparing `talk_codebase-0.1.24/README.md` & `talk_codebase-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.24/pyproject.toml` & `talk_codebase-0.1.25/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.24"
+version = "0.1.25"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.24/talk_codebase/LLM.py` & `talk_codebase-0.1.25/talk_codebase/LLM.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from langchain.callbacks.manager import CallbackManager
 from langchain.chains import RetrievalQA
 from langchain.chat_models import ChatOpenAI
 from langchain.embeddings import HuggingFaceEmbeddings, OpenAIEmbeddings
 from langchain.llms import GPT4All
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 
+from talk_codebase.consts import MODEL_TYPES
 from talk_codebase.utils import load_files, get_local_vector_store, calculate_cost, StreamStdOut
 
 
 class BaseLLM:
 
     def __init__(self, root_dir, config):
         self.config = config
@@ -53,16 +54,15 @@
         docs = load_files(root_dir)
         if len(docs) == 0:
             print("✘ No documents found")
             exit(0)
         text_splitter = RecursiveCharacterTextSplitter(chunk_size=int(self.config.get("chunk_size")),
                                                        chunk_overlap=int(self.config.get("chunk_overlap")))
         texts = text_splitter.split_documents(docs)
-
-        if index == "openai":
+        if index == MODEL_TYPES["OPENAI"]:
             cost = calculate_cost(docs, self.config.get("model_name"))
             approve = questionary.select(
                 f"Creating a vector store for {len(docs)} documents will cost ~${cost:.5f}. Do you want to continue?",
                 choices=[
                     {"name": "Yes", "value": True},
                     {"name": "No", "value": False},
                 ]
@@ -78,25 +78,25 @@
         return db
 
 
 class LocalLLM(BaseLLM):
 
     def _create_store(self, root_dir: str) -> Optional[FAISS]:
         embeddings = HuggingFaceEmbeddings(model_name='all-MiniLM-L6-v2')
-        return self._create_vector_store(embeddings, "local", root_dir)
+        return self._create_vector_store(embeddings, MODEL_TYPES["LOCAL"], root_dir)
 
     def _create_model(self):
         llm = GPT4All(model=self.config.get("model_path"), n_ctx=int(self.config.get("max_tokens")), streaming=True)
         return llm
 
 
 class OpenAILLM(BaseLLM):
     def _create_store(self, root_dir: str) -> Optional[FAISS]:
         embeddings = OpenAIEmbeddings(openai_api_key=self.config.get("api_key"))
-        return self._create_vector_store(embeddings, "openai", root_dir)
+        return self._create_vector_store(embeddings, MODEL_TYPES["OPENAI"], root_dir)
 
     def _create_model(self):
         return ChatOpenAI(model_name=self.config.get("model_name"), openai_api_key=self.config.get("api_key"),
                           streaming=True,
                           max_tokens=int(self.config.get("max_tokens")),
                           callback_manager=CallbackManager([StreamStdOut()]))
```

### Comparing `talk_codebase-0.1.24/talk_codebase/cli.py` & `talk_codebase-0.1.25/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.24/talk_codebase/consts.py` & `talk_codebase-0.1.25/talk_codebase/consts.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 EXCLUDE_DIRS = ['__pycache__', '.venv', '.git', '.idea', 'venv', 'env', 'node_modules', 'dist', 'build', '.vscode',
                 '.github', '.gitlab']
 ALLOW_FILES = ['.txt', '.js', '.mjs', '.ts', '.tsx', '.css', '.scss', '.less', '.html', '.htm', '.json', '.py',
                '.java', '.c', '.cpp', '.cs', '.go', '.php', '.rb', '.rs', '.swift', '.kt', '.scala', '.m', '.h',
                '.sh', '.pl', '.pm', '.lua', '.sql']
 EXCLUDE_FILES = ['requirements.txt', 'package.json', 'package-lock.json', 'yarn.lock']
 DEFAULT_MODEL_PATH = "models/ggml-gpt4all-j-v1.3-groovy.bin"
+MODEL_TYPES = {
+    "OPENAI": "openai",
+    "LOCAL": "local",
+}
 DEFAULT_CONFIG = {
     "max_tokens": "1048",
     "chunk_size": "500",
     "chunk_overlap": "50",
     "k": "4",
     "model_name": "gpt-3.5-turbo",
     "model_path": "models/ggml-gpt4all-j-v1.3-groovy.bin",
-    "model_type": "openai",
+    "model_type": MODEL_TYPES["OPENAI"],
 }
```

### Comparing `talk_codebase-0.1.24/talk_codebase/utils.py` & `talk_codebase-0.1.25/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.24/PKG-INFO` & `talk_codebase-0.1.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.24
+Version: 0.1.25
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

