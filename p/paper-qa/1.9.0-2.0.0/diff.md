# Comparing `tmp/paper-qa-1.9.0.tar.gz` & `tmp/paper-qa-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-1.9.0.tar", last modified: Thu May 25 13:45:02 2023, max compression
+gzip compressed data, was "paper-qa-2.0.0.tar", last modified: Tue May 30 14:30:42 2023, max compression
```

## Comparing `paper-qa-1.9.0.tar` & `paper-qa-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:45:02.333935 paper-qa-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 13:44:23.000000 paper-qa-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-25 13:45:02.333935 paper-qa-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-25 13:44:23.000000 paper-qa-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:45:02.329935 paper-qa-1.9.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-25 13:45:02.000000 paper-qa-1.9.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-25 13:45:02.000000 paper-qa-1.9.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:45:02.000000 paper-qa-1.9.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 13:45:02.000000 paper-qa-1.9.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 13:45:02.000000 paper-qa-1.9.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:45:02.333935 paper-qa-1.9.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:45:02.333935 paper-qa-1.9.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    21407 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:45:02.333935 paper-qa-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-25 13:44:23.000000 paper-qa-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:45:02.333935 paper-qa-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-05-25 13:44:23.000000 paper-qa-1.9.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:30:42.065305 paper-qa-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 14:29:59.000000 paper-qa-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-05-30 14:30:42.065305 paper-qa-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-05-30 14:29:59.000000 paper-qa-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:30:42.061305 paper-qa-2.0.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-05-30 14:30:42.000000 paper-qa-2.0.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-30 14:30:42.000000 paper-qa-2.0.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:30:42.000000 paper-qa-2.0.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-30 14:30:42.000000 paper-qa-2.0.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 14:30:42.000000 paper-qa-2.0.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:30:42.065305 paper-qa-2.0.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 14:29:59.000000 paper-qa-2.0.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-30 14:29:59.000000 paper-qa-2.0.0/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:30:42.065305 paper-qa-2.0.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 14:29:59.000000 paper-qa-2.0.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-30 14:29:59.000000 paper-qa-2.0.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22193 2023-05-30 14:29:59.000000 paper-qa-2.0.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-30 14:29:59.000000 paper-qa-2.0.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-30 14:29:59.000000 paper-qa-2.0.0/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-05-30 14:29:59.000000 paper-qa-2.0.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-30 14:29:59.000000 paper-qa-2.0.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-30 14:29:59.000000 paper-qa-2.0.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 14:29:59.000000 paper-qa-2.0.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:30:42.065305 paper-qa-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-30 14:29:59.000000 paper-qa-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:30:42.065305 paper-qa-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-05-30 14:29:59.000000 paper-qa-2.0.0/tests/test_paperqa.py
```

### Comparing `paper-qa-1.9.0/LICENSE` & `paper-qa-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-1.9.0/PKG-INFO` & `paper-qa-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.9.0
+Version: 2.0.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -59,39 +59,50 @@
 pip install paper-qa
 ```
 
 ## Usage
 
 Make sure you have set your OPENAI_API_KEY environment variable to your [openai api key](https://platform.openai.com/account/api-keys)
 
-To use paper-qa, you need to have a list of paths (valid extensions include: .pdf, .txt) and a list of citations (strings) that correspond to the paths. You can then use the `Docs` class to add the documents and then query them.
+To use paper-qa, you need to have a list of paths (valid extensions include: .pdf, .txt) and a list of citations (strings) that correspond to the paths. You can then use the `Docs` class to add the documents and then query them. If you don't have citations, `Docs` will try to guess them from the first page of your docs.
 
 ```python
 
 from paperqa import Docs
 
 # get a list of paths
 
 docs = Docs()
 for d in my_docs:
     docs.add(d)
-    
+
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
 print(answer.formatted_answer)
 ```
 
 The answer object has the following attributes: `formatted_answer`, `answer` (answer alone), `question`, `context` (the summaries of passages found for answer), `references` (the docs from which the passages came), and `passages` which contain the raw text of the passages as a dictionary.
 
 ### Choosing Model
 
 By default, it uses a hybrid of `gpt-3.5-turbo` and `gpt-4`. If you don't have gpt-4 access or would like to save money, you can adjust:
 
 ```py
 docs = Docs(llm='gpt-3.5-turbo')
 ```
+
+or you can use any other model available in [langchain](https://github.com/hwchase17/langchain):
+
+```py
+from langchain.llms import Anthropic, OpenAIChat
+model = OpenAIChat(model='gpt-4')
+summary_model = Anthropic(model="claude-instant-v1-100k", anthropic_api_key="my-api-key")
+docs = Docs(llm=model, summary_llm=summary_model)
+```
+
+
 #### Locally Hosted
 
 You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
 
 ```py
 from paperqa import Docs
 from langchain.llms import LlamaCpp
@@ -220,15 +231,15 @@
 them to the `Docs` object.
 
 We can also do specific queries of our Zotero library and iterate over the results:
 
 ```py
 for item in zotero.iterate(
         q="large language models",
-        qmode="everything", 
+        qmode="everything",
         sort="date",
         direction="desc",
         limit=100,
 ):
     print("Adding", item.title)
     docs.add(item.pdf, key=item.key)
 ```
@@ -288,10 +299,18 @@
     pickle.dump(docs, f)
 
 # load
 with open("my_docs.pkl", "rb") as f:
     docs = pickle.load(f)
 ```
 
+### PDF Reading Options
+
+By default [PyPDF](https://pypi.org/project/pypdf/) is used since it's pure python and easy to install. For faster PDF reading, paper-qa will detect and use [PymuPDF (fitz)](https://pymupdf.readthedocs.io/en/latest/):
+
+```sh
+pip install pymupdf
+```
+
 ### Callbacks
 
 TODO
```

### Comparing `paper-qa-1.9.0/README.md` & `paper-qa-2.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -45,39 +45,50 @@
 pip install paper-qa
 ```
 
 ## Usage
 
 Make sure you have set your OPENAI_API_KEY environment variable to your [openai api key](https://platform.openai.com/account/api-keys)
 
-To use paper-qa, you need to have a list of paths (valid extensions include: .pdf, .txt) and a list of citations (strings) that correspond to the paths. You can then use the `Docs` class to add the documents and then query them.
+To use paper-qa, you need to have a list of paths (valid extensions include: .pdf, .txt) and a list of citations (strings) that correspond to the paths. You can then use the `Docs` class to add the documents and then query them. If you don't have citations, `Docs` will try to guess them from the first page of your docs.
 
 ```python
 
 from paperqa import Docs
 
 # get a list of paths
 
 docs = Docs()
 for d in my_docs:
     docs.add(d)
-    
+
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
 print(answer.formatted_answer)
 ```
 
 The answer object has the following attributes: `formatted_answer`, `answer` (answer alone), `question`, `context` (the summaries of passages found for answer), `references` (the docs from which the passages came), and `passages` which contain the raw text of the passages as a dictionary.
 
 ### Choosing Model
 
 By default, it uses a hybrid of `gpt-3.5-turbo` and `gpt-4`. If you don't have gpt-4 access or would like to save money, you can adjust:
 
 ```py
 docs = Docs(llm='gpt-3.5-turbo')
 ```
+
+or you can use any other model available in [langchain](https://github.com/hwchase17/langchain):
+
+```py
+from langchain.llms import Anthropic, OpenAIChat
+model = OpenAIChat(model='gpt-4')
+summary_model = Anthropic(model="claude-instant-v1-100k", anthropic_api_key="my-api-key")
+docs = Docs(llm=model, summary_llm=summary_model)
+```
+
+
 #### Locally Hosted
 
 You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
 
 ```py
 from paperqa import Docs
 from langchain.llms import LlamaCpp
@@ -206,15 +217,15 @@
 them to the `Docs` object.
 
 We can also do specific queries of our Zotero library and iterate over the results:
 
 ```py
 for item in zotero.iterate(
         q="large language models",
-        qmode="everything", 
+        qmode="everything",
         sort="date",
         direction="desc",
         limit=100,
 ):
     print("Adding", item.title)
     docs.add(item.pdf, key=item.key)
 ```
@@ -274,10 +285,18 @@
     pickle.dump(docs, f)
 
 # load
 with open("my_docs.pkl", "rb") as f:
     docs = pickle.load(f)
 ```
 
+### PDF Reading Options
+
+By default [PyPDF](https://pypi.org/project/pypdf/) is used since it's pure python and easy to install. For faster PDF reading, paper-qa will detect and use [PymuPDF (fitz)](https://pymupdf.readthedocs.io/en/latest/):
+
+```sh
+pip install pymupdf
+```
+
 ### Callbacks
 
 TODO
```

### Comparing `paper-qa-1.9.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-2.0.0/paper_qa.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.9.0
+Version: 2.0.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -59,39 +59,50 @@
 pip install paper-qa
 ```
 
 ## Usage
 
 Make sure you have set your OPENAI_API_KEY environment variable to your [openai api key](https://platform.openai.com/account/api-keys)
 
-To use paper-qa, you need to have a list of paths (valid extensions include: .pdf, .txt) and a list of citations (strings) that correspond to the paths. You can then use the `Docs` class to add the documents and then query them.
+To use paper-qa, you need to have a list of paths (valid extensions include: .pdf, .txt) and a list of citations (strings) that correspond to the paths. You can then use the `Docs` class to add the documents and then query them. If you don't have citations, `Docs` will try to guess them from the first page of your docs.
 
 ```python
 
 from paperqa import Docs
 
 # get a list of paths
 
 docs = Docs()
 for d in my_docs:
     docs.add(d)
-    
+
 answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
 print(answer.formatted_answer)
 ```
 
 The answer object has the following attributes: `formatted_answer`, `answer` (answer alone), `question`, `context` (the summaries of passages found for answer), `references` (the docs from which the passages came), and `passages` which contain the raw text of the passages as a dictionary.
 
 ### Choosing Model
 
 By default, it uses a hybrid of `gpt-3.5-turbo` and `gpt-4`. If you don't have gpt-4 access or would like to save money, you can adjust:
 
 ```py
 docs = Docs(llm='gpt-3.5-turbo')
 ```
+
+or you can use any other model available in [langchain](https://github.com/hwchase17/langchain):
+
+```py
+from langchain.llms import Anthropic, OpenAIChat
+model = OpenAIChat(model='gpt-4')
+summary_model = Anthropic(model="claude-instant-v1-100k", anthropic_api_key="my-api-key")
+docs = Docs(llm=model, summary_llm=summary_model)
+```
+
+
 #### Locally Hosted
 
 You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
 
 ```py
 from paperqa import Docs
 from langchain.llms import LlamaCpp
@@ -220,15 +231,15 @@
 them to the `Docs` object.
 
 We can also do specific queries of our Zotero library and iterate over the results:
 
 ```py
 for item in zotero.iterate(
         q="large language models",
-        qmode="everything", 
+        qmode="everything",
         sort="date",
         direction="desc",
         limit=100,
 ):
     print("Adding", item.title)
     docs.add(item.pdf, key=item.key)
 ```
@@ -288,10 +299,18 @@
     pickle.dump(docs, f)
 
 # load
 with open("my_docs.pkl", "rb") as f:
     docs = pickle.load(f)
 ```
 
+### PDF Reading Options
+
+By default [PyPDF](https://pypi.org/project/pypdf/) is used since it's pure python and easy to install. For faster PDF reading, paper-qa will detect and use [PymuPDF (fitz)](https://pymupdf.readthedocs.io/en/latest/):
+
+```sh
+pip install pymupdf
+```
+
 ### Callbacks
 
 TODO
```

### Comparing `paper-qa-1.9.0/paperqa/agent.py` & `paper-qa-2.0.0/paperqa/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def status(answer: Answer, docs: Docs):
     return f" Status: Current Papers: {len(docs.doc_previews())} Current Evidence: {len(answer.contexts)} Current Cost: ${answer.cost:.2f}"
 
 
 class PaperSelection(BaseTool):
     name = "Select Papers"
-    description = "Select from current papers. Provide instructions as a string to use for choosing papers."
+    description = "Select from current papers. Provide a desired question to answer as a string to use for choosing papers."
     docs: Docs = None
     answer: Answer = None
     chain: LLMChain = None
 
     def __init__(self, docs, answer):
         # call the parent class constructor
         super(PaperSelection, self).__init__()
```

### Comparing `paper-qa-1.9.0/paperqa/contrib/zotero.py` & `paper-qa-2.0.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.9.0/paperqa/docs.py` & `paper-qa-2.0.0/paperqa/docs.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,18 +23,19 @@
 from .qaprompts import (
     citation_prompt,
     make_chain,
     qa_prompt,
     search_prompt,
     select_paper_prompt,
     summary_prompt,
+    get_score,
 )
 from .readers import read_doc
 from .types import Answer, Context
-from .utils import maybe_is_text, md5sum
+from .utils import maybe_is_text, md5sum, gather_with_concurrency, guess_is_4xx
 
 os.makedirs(os.path.dirname(CACHE_PATH), exist_ok=True)
 langchain.llm_cache = SQLiteCache(CACHE_PATH)
 
 
 class Docs:
     """A collection of documents to be used for answering questions."""
@@ -43,38 +44,41 @@
         self,
         chunk_size_limit: int = 3000,
         llm: Optional[Union[LLM, str]] = None,
         summary_llm: Optional[Union[LLM, str]] = None,
         name: str = "default",
         index_path: Optional[Path] = None,
         embeddings: Optional[Embeddings] = None,
+        max_concurrent: int = 5,
     ) -> None:
         """Initialize the collection of documents.
 
         Args:
             chunk_size_limit: The maximum number of characters to use for a single chunk of text.
             llm: The language model to use for answering questions. Default - OpenAI chat-gpt-turbo
             summary_llm: The language model to use for summarizing documents. If None, llm is used.
             name: The name of the collection.
             index_path: The path to the index file IF pickled. If None, defaults to using name in $HOME/.paperqa/name
             embeddings: The embeddings to use for indexing documents. Default - OpenAI embeddings
+            max_concurrent: Number of concurrent LLM model calls to make
         """
         self.docs = []
         self.chunk_size_limit = chunk_size_limit
         self.keys = set()
         self._faiss_index = None
         self._doc_index = None
         self.update_llm(llm, summary_llm)
         if index_path is None:
             index_path = Path.home() / ".paperqa" / name
         self.index_path = index_path
         self.name = name
         if embeddings is None:
             embeddings = OpenAIEmbeddings()
         self.embeddings = embeddings
+        self.max_concurrent = max_concurrent
         self._deleted_keys = set()
 
     def update_llm(
         self,
         llm: Optional[Union[LLM, str]] = None,
         summary_llm: Optional[Union[LLM, str]] = None,
     ) -> None:
@@ -105,31 +109,29 @@
     def add(
         self,
         path: str,
         citation: Optional[str] = None,
         key: Optional[str] = None,
         disable_check: bool = False,
         chunk_chars: Optional[int] = 3000,
-    ) -> None:
+    ) -> str:
         """Add a document to the collection."""
 
         # first check to see if we already have this document
         # this way we don't make api call to create citation on file we already have
         hash = md5sum(path)
         if hash in [d["hash"] for d in self.docs]:
             raise ValueError(f"Document {path} already in collection.")
 
         if citation is None:
-            cite_chain = make_chain(
-                prompt=citation_prompt, llm=self.summary_llm)
+            cite_chain = make_chain(prompt=citation_prompt, llm=self.summary_llm)
             # peak first chunk
             texts, _ = read_doc(path, "", "", chunk_chars=chunk_chars)
             if len(texts) == 0:
-                raise ValueError(
-                    f"Could not read document {path}. Is it empty?")
+                raise ValueError(f"Could not read document {path}. Is it empty?")
             citation = cite_chain.run(texts[0])
             if len(citation) < 3 or "Unknown" in citation or "insufficient" in citation:
                 citation = f"Unknown, {os.path.basename(path)}, {datetime.now().year}"
 
         if key is None:
             # get first name and year from citation
             try:
@@ -141,25 +143,25 @@
                 )
             try:
                 year = re.search(r"(\d{4})", citation).group(1)
             except AttributeError:
                 year = ""
             key = f"{author}{year}"
         key = self.get_unique_key(key)
-        texts, metadata = read_doc(
-            path, citation, key, chunk_chars=chunk_chars)
+        texts, metadata = read_doc(path, citation, key, chunk_chars=chunk_chars)
         # loose check to see if document was loaded
         #
         if len("".join(texts)) < 10 or (
             not disable_check and not maybe_is_text("".join(texts))
         ):
             raise ValueError(
                 f"This does not look like a text document: {path}. Path disable_check to ignore this error."
             )
         self.add_texts(texts, metadata, hash)
+        return key
 
     def add_texts(
         self,
         texts: List[str],
         metadatas: List[dict],
         hash: str,
         text_embeddings: Optional[List[List[float]]] = None,
@@ -235,86 +237,81 @@
         self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []
     ) -> List[str]:
         """Return a list of documents that match the query."""
         if len(self.docs) == 0:
             return ""
         if self._doc_index is None:
             texts = [doc["metadata"][0]["citation"] for doc in self.docs]
-            metadatas = [{"key": doc["metadata"][0]["dockey"]}
-                         for doc in self.docs]
+            metadatas = [{"key": doc["metadata"][0]["dockey"]} for doc in self.docs]
             self._doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
         docs = self._doc_index.max_marginal_relevance_search(
             query, k=k + len(self._deleted_keys)
         )
-        docs = [doc for doc in docs if doc.metadata["key"]
-                not in self._deleted_keys]
+        docs = [doc for doc in docs if doc.metadata["key"] not in self._deleted_keys]
         chain = make_chain(select_paper_prompt, self.summary_llm)
         papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
         result = await chain.arun(
-            instructions=query, papers="\n".join(papers), callbacks=callbacks
+            question=query, papers="\n".join(papers), callbacks=callbacks
         )
         return result
 
     def doc_match(
         self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []
     ) -> List[str]:
         """Return a list of documents that match the query."""
         if len(self.docs) == 0:
             return ""
         if self._doc_index is None:
             texts = [doc["metadata"][0]["citation"] for doc in self.docs]
-            metadatas = [{"key": doc["metadata"][0]["dockey"]}
-                         for doc in self.docs]
+            metadatas = [{"key": doc["metadata"][0]["dockey"]} for doc in self.docs]
             self._doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
         docs = self._doc_index.max_marginal_relevance_search(
             query, k=k + len(self._deleted_keys)
         )
-        docs = [doc for doc in docs if doc.metadata["key"]
-                not in self._deleted_keys]
+        docs = [doc for doc in docs if doc.metadata["key"] not in self._deleted_keys]
         chain = make_chain(select_paper_prompt, self.summary_llm)
         papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
         result = chain.run(
-            instructions=query, papers="\n".join(papers), callbacks=callbacks
+            question=query, papers="\n".join(papers), callbacks=callbacks
         )
         return result
 
     def __getstate__(self):
         state = self.__dict__.copy()
         if self._faiss_index is not None:
             state["_faiss_index"].save_local(self.index_path)
         del state["_faiss_index"]
         del state["_doc_index"]
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         try:
-            self._faiss_index = FAISS.load_local(
-                self.index_path, self.embeddings)
+            self._faiss_index = FAISS.load_local(self.index_path, self.embeddings)
         except:
             # they use some special exception type, but I don't want to import it
             self._faiss_index = None
         if not hasattr(self, "_doc_index"):
             self._doc_index = None
         # must be a better way to have backwards compatibility
         if not hasattr(self, "_deleted_keys"):
             self._deleted_keys = set()
+        if not hasattr(self, "max_concurrent"):
+            self.max_concurrent = 5
         self.update_llm(None, None)
 
     def _build_faiss_index(self):
         if self._faiss_index is None:
-            texts = reduce(lambda x, y: x + y,
-                           [doc["texts"] for doc in self.docs], [])
+            texts = reduce(lambda x, y: x + y, [doc["texts"] for doc in self.docs], [])
             text_embeddings = reduce(
-                lambda x, y: x + y, [doc["text_embeddings"]
-                                     for doc in self.docs], []
+                lambda x, y: x + y, [doc["text_embeddings"] for doc in self.docs], []
             )
             metadatas = reduce(
                 lambda x, y: x + y, [doc["metadata"] for doc in self.docs], []
             )
             self._faiss_index = FAISS.from_embeddings(
                 # wow adding list to the zip was tricky
                 text_embeddings=list(zip(texts, text_embeddings)),
@@ -373,51 +370,68 @@
             docs = self._faiss_index.max_marginal_relevance_search(
                 answer.question, k=_k, fetch_k=5 * _k
             )
         else:
             docs = self._faiss_index.similarity_search(
                 answer.question, k=_k, fetch_k=5 * _k
             )
+        # ok now filter
+        if key_filter is not None:
+            docs = [doc for doc in docs if doc.metadata["dockey"] in key_filter][:k]
 
         async def process(doc):
             if doc.metadata["dockey"] in self._deleted_keys:
                 return None, None
-            if key_filter is not None and doc.metadata["dockey"] not in key_filter:
-                return None, None
             # check if it is already in answer (possible in agent setting)
             if doc.metadata["key"] in [c.key for c in answer.contexts]:
                 return None, None
             callbacks = [OpenAICallbackHandler()] + get_callbacks(
                 "evidence:" + doc.metadata["key"]
             )
             summary_chain = make_chain(summary_prompt, self.summary_llm)
-            c = Context(
-                key=doc.metadata["key"],
-                citation=doc.metadata["citation"],
-                context=await summary_chain.arun(
+            # This is dangerous because it
+            # could mask errors that are important
+            # I also cannot know what the exception
+            # type is because any model could be used
+            # my best idea is see if there is a 4XX
+            # http code in the exception
+            try:
+                context = await summary_chain.arun(
                     question=answer.question,
                     context_str=doc.page_content,
                     citation=doc.metadata["citation"],
                     callbacks=callbacks,
-                ),
+                )
+            except Exception as e:
+                if guess_is_4xx(e):
+                    return None, None
+                raise e
+            c = Context(
+                key=doc.metadata["key"],
+                citation=doc.metadata["citation"],
+                context=context,
                 text=doc.page_content,
+                score=get_score(context),
             )
             if "not applicable" not in c.context.casefold():
+                print(c.score)
                 return c, callbacks[0]
             return None, None
 
-        results = await asyncio.gather(*[process(doc) for doc in docs])
+        results = await gather_with_concurrency(
+            self.max_concurrent, *[process(doc) for doc in docs]
+        )
         # filter out failures
         results = [r for r in results if r[0] is not None]
         answer.tokens += sum([cb.total_tokens for _, cb in results])
         answer.cost += sum([cb.total_cost for _, cb in results])
         contexts = [c for c, _ in results if c is not None]
         if len(contexts) == 0:
             return answer
-        contexts = sorted(contexts, key=lambda x: len(x.context), reverse=True)
+        contexts = sorted(contexts, key=lambda x: x.score, reverse=True)
         contexts = contexts[:max_sources]
         # add to answer (if not already there)
         keys = [c.key for c in answer.contexts]
         for c in contexts:
             if c.key not in keys:
                 answer.contexts.append(c)
 
@@ -497,19 +511,20 @@
         get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
     ) -> Answer:
         if k < max_sources:
             raise ValueError("k should be greater than max_sources")
         if answer is None:
             answer = Answer(query)
         if len(answer.contexts) == 0:
-            if key_filter or (key_filter is None and len(self.docs) > 5):
+            if key_filter or (key_filter is None and len(self.docs) > max_sources):
                 callbacks = [OpenAICallbackHandler()] + get_callbacks("filter")
                 keys = await self.adoc_match(answer.question, callbacks=callbacks)
                 answer.tokens += callbacks[0].total_tokens
                 answer.cost += callbacks[0].total_cost
+                key_filter = True if len(keys) > 0 else False
             answer = await self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
                 key_filter=keys if key_filter else None,
                 get_callbacks=get_callbacks,
@@ -530,16 +545,16 @@
                 context_str=context_str,
                 length=length_prompt,
                 callbacks=callbacks,
             )
             answer.tokens += cb.total_tokens
             answer.cost += cb.total_cost
         # it still happens lol
-        if "(Foo2012)" in answer_text:
-            answer_text = answer_text.replace("(Foo2012)", "")
+        if "(Example2012)" in answer_text:
+            answer_text = answer_text.replace("(Example2012)", "")
         for c in contexts:
             key = c.key
             text = c.context
             citation = c.citation
             # do check for whole key (so we don't catch Callahan2019a with Callahan2019)
             skey = key.split(" ")[0]
             if skey + " " in answer_text or skey + ")" or skey + "," in answer_text:
```

### Comparing `paper-qa-1.9.0/paperqa/qaprompts.py` & `paper-qa-2.0.0/paperqa/qaprompts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import copy
 from datetime import datetime
 from typing import Any, Dict, List, Optional
+import re
 
 import langchain.prompts as prompts
 from langchain.callbacks.manager import AsyncCallbackManagerForChainRun
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
 from langchain.prompts.chat import ChatPromptTemplate, HumanMessagePromptTemplate
 from langchain.schema import LLMResult, SystemMessage
 
 summary_prompt = prompts.PromptTemplate(
     input_variables=["question", "context_str", "citation"],
-    template="Summarize and provide direct quotes from the text below to help answer a question. "
-    "Do not directly answer the question, instead summarize and "
-    "quote to give evidence to help answer the question. "
-    "Do not use outside sources. "
-    'Reply with "Not applicable" if the text is unrelated to the question. '
-    "Use 150 or less words."
+    template="Summarize the text below to help answer a question. "
+    "Do not directly answer the question, instead summarize "
+    "to give evidence to help answer the question. Include direct quotes. "
+    'Reply "Not applicable" if text is irrelevant. '
+    "Use around 100 words. At the end of your response, provide a score from 1-10 on a newline "
+    "indicating relevance to question. Do not explain your score. "
     "\n\n"
     "{context_str}\n"
     "Extracted from {citation}\n"
     "Question: {question}\n"
     "Relevant Information Summary:",
 )
 
-
 qa_prompt = prompts.PromptTemplate(
     input_variables=["question", "context_str", "length"],
     template="Write an answer ({length}) "
     "for the question below based on the provided context. "
     "If the context provides insufficient information, "
     'reply "I cannot answer". '
-    "For each sentence in your answer, indicate which sources most support it "
+    "For each part of your answer, indicate which sources most support it "
     "via valid citation markers at the end of sentences, like (Example2012). "
     "Answer in an unbiased, comprehensive, and scholarly tone. "
     "If the question is subjective, provide an opinionated answer in the concluding 1-2 sentences. "
     "Use Markdown for formatting code or text, and try to use direct quotes to support arguments.\n\n"
     "{context_str}\n"
     "Question: {question}\n"
     "Answer: ",
@@ -50,33 +50,34 @@
     "Provide some broad and some specific searches. "
     "Recent years are 2021, 2022, 2023.\n\n"
     "1.",
 )
 
 
 select_paper_prompt = prompts.PromptTemplate(
-    input_variables=["instructions", "papers"],
-    template="Select papers according to instructions below. "
+    input_variables=["question", "papers"],
+    template="Select papers to help answer the question below. "
     "Papers are listed as $KEY: $PAPER_INFO. "
     "Return a list of keys, separated by commas. "
-    'Return "None", if no papers are applicable. \n\n'
-    "Instructions: {instructions}\n\n"
+    'Return "None", if no papers are applicable. '
+    "Choose papers that are relevant, from reputable sources, and timely. \n\n"
+    "Question: {question}\n\n"
     "{papers}\n\n"
     "Selected keys:",
 )
 
 
 def _get_datetime():
     now = datetime.now()
     return now.strftime("%m/%d/%Y")
 
 
 citation_prompt = prompts.PromptTemplate(
     input_variables=["text"],
-    template="Provide a possible citation for the following text in MLA Format. Today's date is {date}\n"
+    template="Provide a citation for the following text in MLA Format. You must answer. Today's date is {date}\n"
     "{text}\n\n"
     "Citation:",
     partial_variables={"date": _get_datetime},
 )
 
 
 class FallbackLLMChain(LLMChain):
@@ -93,16 +94,25 @@
         except NotImplementedError as e:
             return self.generate(input_list, run_manager=run_manager)
 
 
 def make_chain(prompt, llm):
     if type(llm) == ChatOpenAI:
         system_message_prompt = SystemMessage(
-            content="You are a scholarly researcher that answers in an unbiased, concise, scholarly tone. "
-            "You sometimes refuse to answer if there is insufficient information. "
-            "If there are potentially ambiguous terms or acronyms, first define them. ",
+            content="Answer in an unbiased, concise, scholarly tone. "
+            "You may refuse to answer if there is insufficient information. "
+            "If there are ambiguous terms or acronyms, first define them. ",
         )
         human_message_prompt = HumanMessagePromptTemplate(prompt=prompt)
         prompt = ChatPromptTemplate.from_messages(
             [system_message_prompt, human_message_prompt]
         )
     return FallbackLLMChain(prompt=prompt, llm=llm)
+
+
+def get_score(text):
+    score = re.search(r"[sS]core[:is\s]+([0-9]+)", text)
+    if score:
+        return int(score.group(1))
+    if len(text) < 100:
+        return 1
+    return 5
```

### Comparing `paper-qa-1.9.0/paperqa/readers.py` & `paper-qa-2.0.0/paperqa/readers.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,14 +23,65 @@
         OCR_CACHE = SQLiteCache(OCR_CACHE_PATH)
     return OCR_CACHE
 
 
 TextSplitter = TokenTextSplitter
 
 
+def clear_cache():
+    """Clear the OCR cache."""
+    # TODO: upstream broken
+    # _get_ocr_cache().clear()
+    global OCR_CACHE
+    OCR_CACHE = None
+    os.unlink(OCR_CACHE_PATH)
+
+
+def parse_pdf_fitz(path, citation, key, chunk_chars, overlap):
+    import fitz
+
+    doc = fitz.open(path)
+    splits = []
+    split = ""
+    pages = []
+    metadatas = []
+    for i in range(doc.page_count):
+        page = doc.load_page(i)
+        split += page.get_text("text", sort=True)
+        pages.append(str(i + 1))
+        # split could be so long it needs to be split
+        # into multiple chunks. Or it could be so short
+        # that it needs to be combined with the next chunk.
+        while len(split) > chunk_chars:
+            splits.append(split[:chunk_chars])
+            # pretty formatting of pages (e.g. 1-3, 4, 5-7)
+            pg = "-".join([pages[0], pages[-1]])
+            metadatas.append(
+                dict(
+                    citation=citation,
+                    dockey=key,
+                    key=f"{key} pages {pg}",
+                )
+            )
+            split = split[chunk_chars - overlap :]
+            pages = [str(i + 1)]
+    if len(split) > overlap:
+        splits.append(split[:chunk_chars])
+        pg = "-".join([pages[0], pages[-1]])
+        metadatas.append(
+            dict(
+                citation=citation,
+                dockey=key,
+                key=f"{key} pages {pg}",
+            )
+        )
+    doc.close()
+    return splits, metadatas
+
+
 def parse_pdf(path, citation, key, chunk_chars=2000, overlap=50):
     import pypdf
 
     pdfFileObj = open(path, "rb")
     pdfReader = pypdf.PdfReader(pdfFileObj)
     splits = []
     split = ""
@@ -207,19 +258,34 @@
             prompt=cache_key,
             llm_string="",
             return_val=_serialize(out),
         )
     return out
 
 
-def _read_doc(path, citation, key, chunk_chars=3000, overlap=100, disable_check=False):
+def _read_doc(
+    path,
+    citation,
+    key,
+    chunk_chars=3000,
+    overlap=100,
+    disable_check=False,
+    force_pypdf=False,
+):
     """Parse a document into chunks."""
     if isinstance(path, Path):
         path = str(path)
     if path.endswith(".pdf"):
-        return parse_pdf(path, citation, key, chunk_chars, overlap)
+        if force_pypdf:
+            return parse_pdf(path, citation, key, chunk_chars, overlap)
+        try:
+            import fitz
+
+            return parse_pdf_fitz(path, citation, key, chunk_chars, overlap)
+        except ImportError:
+            return parse_pdf(path, citation, key, chunk_chars, overlap)
     elif path.endswith(".txt"):
         return parse_txt(path, citation, key, chunk_chars, overlap)
     elif path.endswith(".html"):
         return parse_txt(path, citation, key, chunk_chars, overlap, html=True)
     else:
         return parse_code_txt(path, citation, key, chunk_chars, overlap)
```

### Comparing `paper-qa-1.9.0/paperqa/types.py` & `paper-qa-2.0.0/paperqa/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,21 +2,36 @@
 from pathlib import Path
 from typing import Any, Dict, List, Union
 
 StrPath = Union[str, Path]
 
 
 @dataclass
+class Context:
+    """A class to hold the context of a question."""
+
+    key: str
+    citation: str
+    context: str
+    text: str
+    score: int = 5
+
+    def __str__(self) -> str:
+        """Return the context as a string."""
+        return self.context
+
+
+@dataclass
 class Answer:
     """A class to hold the answer to a question."""
 
     question: str
     answer: str = ""
     context: str = ""
-    contexts: List[Any] = None
+    contexts: List[Context] = None
     references: str = ""
     formatted_answer: str = ""
     passages: Dict[str, str] = None
     tokens: int = 0
     cost: float = 0
 
     def __post_init__(self):
@@ -25,21 +40,7 @@
             self.contexts = []
         if self.passages is None:
             self.passages = {}
 
     def __str__(self) -> str:
         """Return the answer as a string."""
         return self.formatted_answer
-
-
-@dataclass
-class Context:
-    """A class to hold the context of a question."""
-
-    key: str
-    citation: str
-    context: str
-    text: str
-
-    def __str__(self) -> str:
-        """Return the context as a string."""
-        return self.context
```

### Comparing `paper-qa-1.9.0/setup.py` & `paper-qa-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.9.0/tests/test_paperqa.py` & `paper-qa-2.0.0/tests/test_paperqa.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import os
 import pickle
+import sys
 from typing import Any
 from unittest import IsolatedAsyncioTestCase
+from unittest import mock
+from importlib import reload
+from importlib import import_module
 
 import requests
 from langchain.callbacks.base import AsyncCallbackHandler
 from langchain.llms import OpenAI
 from langchain.llms.fake import FakeListLLM
 
 import paperqa
 from paperqa.utils import strings_similarity
+from paperqa.readers import clear_cache
 
 
 class TestHandler(AsyncCallbackHandler):
     async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         print(token)
 
 
@@ -237,22 +242,35 @@
     assert docs.docs[1]["key"] == "Wiki2023a"
 
     os.remove(doc_path)
     os.remove(doc_path2)
 
 
 def test_pdf_reader():
+    clear_cache()
     tests_dir = os.path.dirname(os.path.abspath(__file__))
     doc_path = os.path.join(tests_dir, "paper.pdf")
     docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-curie-001"))
     docs.add(doc_path, "Wellawatte et al, XAI Review, 2023")
     answer = docs.query("Are counterfactuals actionable?")
     assert "yes" in answer.answer or "Yes" in answer.answer
 
 
+def test_pdf_pypdf_reader():
+    tests_dir = os.path.dirname(os.path.abspath(__file__))
+    doc_path = os.path.join(tests_dir, "paper.pdf")
+    splits1, _ = paperqa.readers._read_doc(
+        doc_path, "foo te al", "bar", force_pypdf=True
+    )
+    splits2, _ = paperqa.readers._read_doc(
+        doc_path, "foo te al", "bar", force_pypdf=False
+    )
+    assert strings_similarity(splits1[0].casefold(), splits2[0].casefold()) > 0.85
+
+
 def test_prompt_length():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
@@ -387,7 +405,30 @@
 
     docs = paperqa.Docs()
     try:
         zotero = ZoteroDB(library_type="user")  # "group" if group library
     except ValueError:
         # close enough
         return
+
+
+def test_too_much_evidence():
+    doc_path = "example2.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Barack_Obama")
+        f.write(r.text)
+    docs = paperqa.Docs(llm="gpt-3.5-turbo", summary_llm="gpt-3.5-turbo")
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    # add with new dockey
+    with open("example.txt", "w", encoding="utf-8") as f:
+        f.write(r.text)
+        f.write("\n")  # so we don't have same hash
+    docs.add(
+        "example.txt",
+        "WikiMedia Foundation, 2023, Accessed now",
+        key="test",
+        chunk_chars=4000,
+    )
+    answer = docs.query(
+        "What is Barrack's greatest accomplishment?", max_sources=10, k=10
+    )
```

