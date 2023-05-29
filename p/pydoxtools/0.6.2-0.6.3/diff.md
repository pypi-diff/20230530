# Comparing `tmp/pydoxtools-0.6.2.tar.gz` & `tmp/pydoxtools-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoxtools-0.6.2.tar", max compression
+gzip compressed data, was "pydoxtools-0.6.3.tar", max compression
```

## Comparing `pydoxtools-0.6.2.tar` & `pydoxtools-0.6.3.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0     1072 2023-01-19 05:32:50.265107 pydoxtools-0.6.2/LICENSE
--rw-r--r--   0        0        0     8260 2023-05-25 01:08:00.818589 pydoxtools-0.6.2/README.md
--rw-r--r--   0        0        0      258 2023-05-25 06:20:55.635381 pydoxtools-0.6.2/pydoxtools/__init__.py
--rw-r--r--   0        0        0    11157 2023-05-26 18:46:19.000755 pydoxtools-0.6.2/pydoxtools/agent.py
--rw-r--r--   0        0        0     2508 2022-02-09 15:52:43.898218 pydoxtools-0.6.2/pydoxtools/class_utils.py
--rwxr-xr-x   0        0        0    30541 2023-05-09 05:49:37.140825 pydoxtools-0.6.2/pydoxtools/classifier.py
--rw-r--r--   0        0        0    29431 2022-11-12 20:39:33.790453 pydoxtools-0.6.2/pydoxtools/cluster_utils.py
--rw-r--r--   0        0        0     6047 2023-05-25 01:00:13.344389 pydoxtools-0.6.2/pydoxtools/dask_operators.py
--rw-r--r--   0        0        0    53220 2023-05-24 17:14:40.070633 pydoxtools-0.6.2/pydoxtools/document.py
--rw-r--r--   0        0        0    35071 2023-05-24 00:02:05.489329 pydoxtools-0.6.2/pydoxtools/document_base.py
--rw-r--r--   0        0        0     1673 2023-05-09 23:54:11.246379 pydoxtools-0.6.2/pydoxtools/extract_classes.py
--rw-r--r--   0        0        0        3 2023-05-02 20:33:41.756428 pydoxtools-0.6.2/pydoxtools/extract_db.py
--rw-r--r--   0        0        0     3978 2023-05-23 19:28:54.538602 pydoxtools-0.6.2/pydoxtools/extract_filesystem.py
--rw-r--r--   0        0        0    13329 2023-05-09 23:54:11.178377 pydoxtools-0.6.2/pydoxtools/extract_html.py
--rw-r--r--   0        0        0    12566 2023-05-26 18:48:24.639525 pydoxtools-0.6.2/pydoxtools/extract_index.py
--rw-r--r--   0        0        0     3177 2023-05-20 06:10:12.179526 pydoxtools-0.6.2/pydoxtools/extract_nlpchat.py
--rw-r--r--   0        0        0     2469 2023-05-09 23:54:11.186378 pydoxtools-0.6.2/pydoxtools/extract_objects.py
--rw-r--r--   0        0        0     1656 2023-05-10 07:01:17.768739 pydoxtools-0.6.2/pydoxtools/extract_ocr.py
--rw-r--r--   0        0        0     6469 2023-05-23 19:52:11.543694 pydoxtools-0.6.2/pydoxtools/extract_pandoc.py
--rw-r--r--   0        0        0     5544 2023-05-09 23:54:11.270379 pydoxtools-0.6.2/pydoxtools/extract_spacy.py
--rw-r--r--   0        0        0    43269 2023-05-20 05:43:43.697769 pydoxtools-0.6.2/pydoxtools/extract_tables.py
--rw-r--r--   0        0        0     8139 2023-05-09 23:54:11.150377 pydoxtools-0.6.2/pydoxtools/extract_textstructure.py
--rw-r--r--   0        0        0     1232 2023-04-26 22:02:00.116297 pydoxtools-0.6.2/pydoxtools/file_utils.py
--rwxr-xr-x   0        0        0     6143 2022-11-12 20:39:33.794453 pydoxtools-0.6.2/pydoxtools/html_utils.py
--rw-r--r--   0        0        0      150 2022-02-09 15:52:43.898218 pydoxtools-0.6.2/pydoxtools/initialize_library.py
--rw-r--r--   0        0        0     7077 2022-11-12 20:39:33.794453 pydoxtools-0.6.2/pydoxtools/labeling.py
--rw-r--r--   0        0        0     7364 2023-05-18 23:05:10.290935 pydoxtools-0.6.2/pydoxtools/list_utils.py
--rw-r--r--   0        0        0      371 2022-11-12 20:39:33.794453 pydoxtools-0.6.2/pydoxtools/math_utils.py
--rw-r--r--   0        0        0     2431 2022-11-12 20:39:33.794453 pydoxtools-0.6.2/pydoxtools/models.py
--rwxr-xr-x   0        0        0    18776 2023-05-06 19:40:13.998671 pydoxtools-0.6.2/pydoxtools/nlp_utils.py
--rw-r--r--   0        0        0     2502 2022-03-30 10:01:09.241031 pydoxtools-0.6.2/pydoxtools/ocr_language_mappings.py
--rw-r--r--   0        0        0     8897 2023-05-09 23:54:11.158377 pydoxtools-0.6.2/pydoxtools/operator_huggingface.py
--rw-r--r--   0        0        0     1137 2023-05-14 18:22:46.918667 pydoxtools-0.6.2/pydoxtools/operators.py
--rw-r--r--   0        0        0     7856 2023-05-22 06:53:09.989310 pydoxtools-0.6.2/pydoxtools/operators_base.py
--rwxr-xr-x   0        0        0    12146 2023-05-09 23:54:11.106376 pydoxtools-0.6.2/pydoxtools/pdf_utils.py
--rw-r--r--   0        0        0    34126 2023-03-28 06:51:36.920970 pydoxtools-0.6.2/pydoxtools/random_data_generators.py
--rwxr-xr-x   0        0        0     1332 2023-05-11 04:47:15.118352 pydoxtools-0.6.2/pydoxtools/settings.py
--rw-r--r--   0        0        0    17693 2023-05-09 05:49:37.108824 pydoxtools-0.6.2/pydoxtools/training.py
--rw-r--r--   0        0        0     3898 2022-02-09 15:52:43.898218 pydoxtools-0.6.2/pydoxtools/visual_document_analysis.py
--rw-r--r--   0        0        0     3209 2023-01-19 05:32:50.269106 pydoxtools-0.6.2/pydoxtools/webdav_utils.py
--rw-r--r--   0        0        0     5950 2023-05-26 19:02:02.709630 pydoxtools-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    11122 1970-01-01 00:00:00.000000 pydoxtools-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-29 07:08:59.780129 pydoxtools-0.6.3/LICENSE
+-rw-r--r--   0        0        0     8260 2023-05-25 18:58:37.513803 pydoxtools-0.6.3/README.md
+-rw-r--r--   0        0        0      261 2023-05-29 20:02:49.181016 pydoxtools-0.6.3/pydoxtools/__init__.py
+-rw-r--r--   0        0        0    12096 2023-05-29 21:07:28.688538 pydoxtools-0.6.3/pydoxtools/agent.py
+-rw-r--r--   0        0        0     2508 2022-02-03 10:08:19.000000 pydoxtools-0.6.3/pydoxtools/class_utils.py
+-rwxr-xr-x   0        0        0    30541 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/classifier.py
+-rw-r--r--   0        0        0    29431 2022-09-09 18:06:03.434226 pydoxtools-0.6.3/pydoxtools/cluster_utils.py
+-rw-r--r--   0        0        0     6047 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/dask_operators.py
+-rw-r--r--   0        0        0    54044 2023-05-29 18:22:59.945511 pydoxtools-0.6.3/pydoxtools/document.py
+-rw-r--r--   0        0        0    35071 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/document_base.py
+-rw-r--r--   0        0        0     1673 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_classes.py
+-rw-r--r--   0        0        0     3978 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_filesystem.py
+-rw-r--r--   0        0        0    13329 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_html.py
+-rw-r--r--   0        0        0    12566 2023-05-27 05:02:18.158595 pydoxtools-0.6.3/pydoxtools/extract_index.py
+-rw-r--r--   0        0        0     5965 2023-05-29 18:22:59.945511 pydoxtools-0.6.3/pydoxtools/extract_nlpchat.py
+-rw-r--r--   0        0        0     2469 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_objects.py
+-rw-r--r--   0        0        0     1656 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_ocr.py
+-rw-r--r--   0        0        0     6469 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_pandoc.py
+-rw-r--r--   0        0        0     5544 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_spacy.py
+-rw-r--r--   0        0        0    43269 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_tables.py
+-rw-r--r--   0        0        0     8139 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/extract_textstructure.py
+-rw-r--r--   0        0        0     1232 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/file_utils.py
+-rwxr-xr-x   0        0        0     6143 2022-09-14 22:13:53.783991 pydoxtools-0.6.3/pydoxtools/html_utils.py
+-rw-r--r--   0        0        0      150 2022-02-03 10:08:19.000000 pydoxtools-0.6.3/pydoxtools/initialize_library.py
+-rw-r--r--   0        0        0     7077 2022-09-09 18:06:03.434226 pydoxtools-0.6.3/pydoxtools/labeling.py
+-rw-r--r--   0        0        0     7364 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/list_utils.py
+-rw-r--r--   0        0        0      371 2022-09-09 18:06:03.434226 pydoxtools-0.6.3/pydoxtools/math_utils.py
+-rw-r--r--   0        0        0     2431 2022-09-13 15:47:40.161989 pydoxtools-0.6.3/pydoxtools/models.py
+-rwxr-xr-x   0        0        0    18776 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/nlp_utils.py
+-rw-r--r--   0        0        0     2502 2022-03-25 12:06:42.174796 pydoxtools-0.6.3/pydoxtools/ocr_language_mappings.py
+-rw-r--r--   0        0        0     8897 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/operator_huggingface.py
+-rw-r--r--   0        0        0     1134 2023-05-29 18:22:59.945511 pydoxtools-0.6.3/pydoxtools/operators.py
+-rw-r--r--   0        0        0     7856 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/operators_base.py
+-rwxr-xr-x   0        0        0    12146 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/pdf_utils.py
+-rw-r--r--   0        0        0    34126 2023-03-29 07:08:59.788125 pydoxtools-0.6.3/pydoxtools/random_data_generators.py
+-rwxr-xr-x   0        0        0     1332 2023-05-25 18:58:37.521804 pydoxtools-0.6.3/pydoxtools/settings.py
+-rw-r--r--   0        0        0    17693 2023-05-25 18:58:37.525804 pydoxtools-0.6.3/pydoxtools/training.py
+-rw-r--r--   0        0        0     3898 2022-02-03 10:08:19.000000 pydoxtools-0.6.3/pydoxtools/visual_document_analysis.py
+-rw-r--r--   0        0        0     3209 2023-03-29 07:08:59.788125 pydoxtools-0.6.3/pydoxtools/webdav_utils.py
+-rw-r--r--   0        0        0     5930 2023-05-29 21:49:19.710912 pydoxtools-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    11084 1970-01-01 00:00:00.000000 pydoxtools-0.6.3/PKG-INFO
```

### Comparing `pydoxtools-0.6.2/LICENSE` & `pydoxtools-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/README.md` & `pydoxtools-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/agent.py` & `pydoxtools-0.6.3/pydoxtools/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 def where_or(x):
     if len(x) > 1:
         return {"$or": x}
     elif len(x) == 1:
         return x[0]
 
 
-class Agent:
+class LLMAgent:
     # TODO: define BlogWritingAgent as a pipeline as well?
     #       not sure, yet, if we would benefit from this here...
     #       might make sense in the future, if we have multiple
     #       agents for different tasks...
 
     _context_where_all = where_or([{"information_type": "question"},
                                    {"information_type": "task"},
@@ -63,19 +63,19 @@
     def __init__(
             self,
             objective: str,
             # TODO: support multiple datasources
             data_source: pdx.DocumentBag,
             vector_store: chromadb.config.Settings,
             startfresh: bool = True,
-            privacy_mode="non_proviate_llm_queries"
+            privacy_mode="non_private_llm_queries"
     ):
         if not isinstance(vector_store, chromadb.config.Settings):
             raise NotImplementedError("Other vectorstores besides chromadb are WIP!")
-        if privacy_mode != "non_proviate_llm_queries":
+        if privacy_mode != "non_private_llm_queries":
             raise RuntimeError("You have to have 'Alpaca' model installed in order"
                                "to run other privacy modes...")
         self.vector_store = vector_store
         self._objective = objective
         self._debug_queue = []
         self._final_result = ""
         self._data_source: pdx.DocumentBag | None = data_source
@@ -128,42 +128,59 @@
 
     def add_data(self, key, data):
         doc = self.documents.Document(f"{key.strip()}: {data.strip()}")
         add_info_to_collection(
             self.chromadb_collection, doc,
             [{"information_type": "data", "key": key.strip(), "info": data.strip()}])
 
-    def task_chat(self, task, context=None, previous_tasks=None, format="yaml"):
+    def task_chat(self, task, context=None, previous_tasks=None, format="yaml", method="prompt"):
         msgs = []
         msgs.append({"role": "system",
                      "content": "You are a helpful assistant that aims to complete one task."})
-        msgs.append({"role": "user",
-                     "content": f"# Overall objective: \n{self._objective}\n\n"}),
-        if previous_tasks:
+        if method == "chat":
             msgs.append({"role": "user",
-                         "content": f"# Take into account these previously completed tasks"
-                                    f"\n\n{previous_tasks} \n\n"}),
-        if context:
-            msgs.append({"role": "user",
-                         "content": f"# Take into account this context"
-                                    f"\n\n{context} \n\n"}),
-        msgs.append(
-            {"role": "user", "content": f"# Complete the following task: \n{task} \n\n"
-                                        f"Provide only the precise information requested without context, "
-                                        f"make sure we can parse the response as {format}. RESULT:\n"})
+                         "content": f"# Overall objective: \n{self._objective}\n\n"}),
+            if previous_tasks:
+                msgs.append({"role": "user",
+                             "content": f"# Take into account these previously completed tasks"
+                                        f"\n\n{previous_tasks} \n\n"}),
+            if context:
+                msgs.append({"role": "user",
+                             "content": f"# Take into account this context"
+                                        f"\n\n{context} \n\n"}),
+            msgs.append(
+                {"role": "user", "content": f"# Complete the following task: \n{task} \n\n"
+                                            f"Provide only the precise information requested without context, "
+                                            f"make sure we can parse the response as {format}. RESULT:\n"})
+        else:
+            msg = f"# Considering the overall objective: \n{self._objective}\n\n"
+            if previous_tasks:
+                msg += f"# Take into account these previously completed tasks:\n\n{previous_tasks} \n\n"
+            if context:
+                msg += f"# Take into account this context:\n\n{context} \n\n"
+            msg += f"# Complete the following task: \n{task} \n\n" \
+                   f"Provide only the precise information requested without context, " \
+                   f"make sure we can parse the response as {format}. RESULT:\n"
+            msgs.append(
+                {"role": "user", "content": msg})
         return msgs
 
     def get_context(self, task: str, n_results: int = 5, where_clause=None):
         where_clause = where_clause or self._context_where_all
         context = self.chromadb_collection.query(
             query_embeddings=[self.vectorize(task).tolist()],
             where=where_clause,
             n_results=n_results)["documents"]
         return context
 
+    def get_data(self, where_clause):
+        context = self.chromadb_collection.get(
+            where=where_clause)
+        return context
+
     def execute_task(
             self,
             task,
             context_size: int = 5,
             previous_task_size=0,
             max_tokens=256,
             formatting="yaml",
@@ -175,15 +192,15 @@
                                        n_results=context_size)[0]
         else:
             context = ""
         # TODO: if we had this exact task in an earlier iteration..
         #       evaluate if we have to do it again or already have our answer...
         if previous_task_size:
             previous_tasks = self.get_context(
-                task, where_clause=self._context_where_info,
+                task, where_clause=self._context_where_tasks,
                 n_results=previous_task_size)[0]
         else:
             previous_tasks = ""
         msgs = self.task_chat(previous_tasks=previous_tasks,
                               context="\n---\n".join(context), task=task,
                               format=formatting)
         msg = '\n'.join(m['content'] for m in msgs)
@@ -236,14 +253,15 @@
         # TODO: try to formulate questions in a way that we can answer them with
         #       only a single word...
         #       also, try this "local" strategy to answer questions...
         # anslist = pd.DataFrame(Document(txt).answers(question)[0])
         # if not anslist.empty:
         #    ans = anslist.groupby(0).sum().sort_values(by=1, ascending=False).index[0]
         # else:
+        # TODO: should we save the question?
         res = self.execute_task(task=f"answer the following question: '{question}' "
                                      f"using this text as input: {txt}", formatting="txt")
         ans = res
         # TODO: ask questions like "is this correct?" or can you provide the name?
         # ans_parsed = yaml.unsafe_load(ans)
         self.add_question(question, ans)
         return ans
```

### Comparing `pydoxtools-0.6.2/pydoxtools/class_utils.py` & `pydoxtools-0.6.3/pydoxtools/class_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/classifier.py` & `pydoxtools-0.6.3/pydoxtools/classifier.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/cluster_utils.py` & `pydoxtools-0.6.3/pydoxtools/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/dask_operators.py` & `pydoxtools-0.6.3/pydoxtools/dask_operators.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/document.py` & `pydoxtools-0.6.3/pydoxtools/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from .document_base import Pipeline, ElementType
 from .extract_classes import LanguageExtractor, TextBlockClassifier
 from .extract_filesystem import PathLoader
 from .extract_filesystem import force_decode, load_raw_file_content
 from .extract_html import HtmlExtractor
 from .extract_index import IndexExtractor, KnnQuery, \
     SimilarityGraph, TextrankOperator, TextPieceSplitter, ChromaIndexFromBag
-from .extract_nlpchat import OpenAIChat
+from .extract_nlpchat import LLMChat
 from .extract_objects import EntityExtractor
 from .extract_ocr import OCRExtractor
 from .extract_pandoc import PandocLoader, PandocOperator, PandocConverter, PandocBlocks, PandocToPdxConverter
 from .extract_spacy import SpacyOperator, extract_spacy_token_vecs, get_spacy_embeddings, extract_noun_chunks
 from .extract_tables import ListExtractor, TableCandidateAreasExtractor
 from .extract_textstructure import DocumentElementFilter, TextBoxElementExtractor, TitleExtractor, SectionsExtractor
 from .html_utils import get_text_only_blocks
@@ -615,16 +615,26 @@
             ########### QaM machine #############
             # TODO: make sure we can set the model that we want to use dynamically!
             Configuration(qam_model_id='deepset/minilm-uncased-squad2'),
             QamExtractor()
             .pipe(property_dict="to_dict", trf_model_id="qam_model_id").out("answers").cache(),
 
             ########### Chat AI ##################
-            Configuration(openai_chat_model_id="gpt-3.5-turbo"),
-            OpenAIChat().pipe(property_dict="to_dict", model_id="openai_chat_model_id")
+            Configuration(chat_model_id="gpt-3.5-turbo").docs(
+                "In order to use openai-chatgpt, you can use 'gpt-3.5-turbo'."
+                "The standard model that can be used right now is 'ggml-mpt-7b-chat' "
+                "which runs locally and can be used for commercial purposes"
+                "Additionally, we support gpt4all models. Currently available"
+                "models are: ggml-gpt4all-j-v1.3-groovy.bin, ggml-gpt4all-l13b-snoozy.bin, "
+                "ggml-mpt-7b-chat.bin, ggml-gpt4all-j-v1.2-jazzy.bin, ggml-gpt4all-j-v1.1-breezy.bin, "
+                "ggml-gpt4all-j.bin, ggml-vicuna-7b-1.1-q4_2.bin, ggml-vicuna-13b-1.1-q4_2.bin, "
+                "ggml-wizardLM-7B.q4_2.bin, ggml-stable-vicuna-13B.q4_2.bin, ggml-mpt-7b-base.bin, "
+                "ggml-nous-gpt4-vicuna-13b.bin, ggml-mpt-7b-instruct.bin, ggml-wizard-13b-uncensored.bin"
+            ),
+            LLMChat().pipe(property_dict="to_dict", model_id="chat_model_id")
             .out("chat_answers").cache()
         ]
     }
 
     def __init__(
             self,
             fobj: str | bytes | Path | IO | dict | list | set = None,
```

### Comparing `pydoxtools-0.6.2/pydoxtools/document_base.py` & `pydoxtools-0.6.3/pydoxtools/document_base.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/extract_classes.py` & `pydoxtools-0.6.3/pydoxtools/extract_classes.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/extract_filesystem.py` & `pydoxtools-0.6.3/pydoxtools/extract_filesystem.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/extract_html.py` & `pydoxtools-0.6.3/pydoxtools/extract_html.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/extract_index.py` & `pydoxtools-0.6.3/pydoxtools/extract_index.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/extract_objects.py` & `pydoxtools-0.6.3/pydoxtools/extract_objects.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/extract_ocr.py` & `pydoxtools-0.6.3/pydoxtools/extract_ocr.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/extract_pandoc.py` & `pydoxtools-0.6.3/pydoxtools/extract_pandoc.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/extract_spacy.py` & `pydoxtools-0.6.3/pydoxtools/extract_spacy.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/extract_tables.py` & `pydoxtools-0.6.3/pydoxtools/extract_tables.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/extract_textstructure.py` & `pydoxtools-0.6.3/pydoxtools/extract_textstructure.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/file_utils.py` & `pydoxtools-0.6.3/pydoxtools/file_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/html_utils.py` & `pydoxtools-0.6.3/pydoxtools/html_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/labeling.py` & `pydoxtools-0.6.3/pydoxtools/labeling.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/list_utils.py` & `pydoxtools-0.6.3/pydoxtools/list_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/models.py` & `pydoxtools-0.6.3/pydoxtools/models.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/nlp_utils.py` & `pydoxtools-0.6.3/pydoxtools/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/ocr_language_mappings.py` & `pydoxtools-0.6.3/pydoxtools/ocr_language_mappings.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/operator_huggingface.py` & `pydoxtools-0.6.3/pydoxtools/operator_huggingface.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/operators.py` & `pydoxtools-0.6.3/pydoxtools/operators.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 from pydoxtools.operators_base import Operator, Configuration
 from operators_base import FunctionOperator, ElementWiseOperator, Alias, ForgivingExtractIterator,DataMerger
 from operator_huggingface import HuggingfacePipeline, QamExtractor
 from extract_filesystem import FileLoader, PathLoader, Path
 from extract_ocr import OCRExtractor
-from extract_nlpchat import OpenAIChat
+from extract_nlpchat import LLMChat
 from extract_pandoc import PandocLoader, PandocOperator, PandocConverter, PandocBlocks
 from extract_html import HtmlExtractor
 from extract_classes import LanguageExtractor, TextBlockClassifier
 from extract_index import IndexExtractor, KnnQuery, TextPieceSplitter, HuggingfaceVectorizer,\
     SimilarityGraph, TextrankOperator
 from extract_objects import EntityExtractor
 from extract_spacy import SpacyOperator
```

### Comparing `pydoxtools-0.6.2/pydoxtools/operators_base.py` & `pydoxtools-0.6.3/pydoxtools/operators_base.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/pdf_utils.py` & `pydoxtools-0.6.3/pydoxtools/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/random_data_generators.py` & `pydoxtools-0.6.3/pydoxtools/random_data_generators.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/settings.py` & `pydoxtools-0.6.3/pydoxtools/settings.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/training.py` & `pydoxtools-0.6.3/pydoxtools/training.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/visual_document_analysis.py` & `pydoxtools-0.6.3/pydoxtools/visual_document_analysis.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pydoxtools/webdav_utils.py` & `pydoxtools-0.6.3/pydoxtools/webdav_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.2/pyproject.toml` & `pydoxtools-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydoxtools"
-version = "0.6.2"
+version = "0.6.3"
 description = "This library contains a set of tools in order to extract and synthesize structured information from documents"
 authors = ["thomas meschede <yeusblender@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pydoxtools.xyntopia.com"
 repository = "https://github.com/xyntopia/pydoxtools"
 documentation = "https://pydoxtools.xyntopia.com"
@@ -66,16 +66,14 @@
     "quantities", "readability-lxml", "pandas", "beautifulsoup4", "hnswlib",
     "networkx", "openai", "textract", "pandoc", "python-pptx", "dask", "pytesseract"
 ]
 # TODO: rename & regroups extras (e.g. light, medium average or something like that...)
 inference = ["transformers", "scikit-learn", "tqdm", "torch", "pytorch-lightning", "spacy",
     "beautifulsoup4", "pandas", "urlextract", "hnswlib", "chromadb"]
 
-all = ["chromadb"]
-
 [tool.poetry.group.colab]
 optional = true
 
 [tool.poetry.group.colab.dependencies]
 pytest = ">=6.0.1"
 yattag = ">=1.13.2" #for html text coloring
 pigeonXT-jupyter = "^0.6.1" # for labeling purposes...
```

### Comparing `pydoxtools-0.6.2/PKG-INFO` & `pydoxtools-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: pydoxtools
-Version: 0.6.2
+Version: 0.6.3
 Summary: This library contains a set of tools in order to extract and synthesize structured information from documents
 Home-page: https://pydoxtools.xyntopia.com
 License: MIT
 Keywords: AI,document-analysis,LLM,NLP,ML
 Author: thomas meschede
 Author-email: yeusblender@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: all
 Provides-Extra: etl
 Provides-Extra: inference
 Requires-Dist: Pint (>=0.16.1)
 Requires-Dist: Shapely (>=1.8.0,<2.0.0)
 Requires-Dist: appdirs (>=1.4.4)
 Requires-Dist: beautifulsoup4 (>=4.8.0) ; extra == "etl" or extra == "inference"
 Requires-Dist: chardet (>=5.1.0,<6.0.0)
-Requires-Dist: chromadb (>=0.3.23,<0.4.0) ; extra == "inference" or extra == "all"
+Requires-Dist: chromadb (>=0.3.23,<0.4.0) ; extra == "inference"
 Requires-Dist: dask[complete] (>=2023.4.1,<2024.0.0) ; extra == "etl"
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: extruct (>=0.9.0) ; extra == "etl"
 Requires-Dist: goose3 (>=3.1.6) ; extra == "etl"
 Requires-Dist: hnswlib (>=0.6.2) ; extra == "etl" or extra == "inference"
 Requires-Dist: langdetect (>=1.0.8) ; extra == "etl"
 Requires-Dist: lxml (>=4.6.2)
```

