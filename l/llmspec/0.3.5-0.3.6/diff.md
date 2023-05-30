# Comparing `tmp/llmspec-0.3.5.tar.gz` & `tmp/llmspec-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmspec-0.3.5.tar", last modified: Sat May 27 03:52:30 2023, max compression
+gzip compressed data, was "llmspec-0.3.6.tar", last modified: Tue May 30 03:30:26 2023, max compression
```

## Comparing `llmspec-0.3.5.tar` & `llmspec-0.3.6.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    11098 2023-05-27 03:52:21.586964 llmspec-0.3.5/LICENSE
--rw-r--r--   0        0        0       33 2023-05-27 03:52:21.586964 llmspec-0.3.5/README.md
--rw-r--r--   0        0        0      687 2023-05-27 03:52:21.586964 llmspec-0.3.5/llmspec/__init__.py
--rw-r--r--   0        0        0    12393 2023-05-27 03:52:21.586964 llmspec-0.3.5/llmspec/llmspec.py
--rw-r--r--   0        0        0      215 2023-05-27 03:52:21.586964 llmspec-0.3.5/llmspec/mixins.py
--rw-r--r--   0        0        0       54 2023-05-27 03:52:21.586964 llmspec-0.3.5/llmspec/types.py
--rw-r--r--   0        0        0     1130 2023-05-27 03:52:30.735068 llmspec-0.3.5/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-27 03:52:21.590964 llmspec-0.3.5/tests/dummy_test.py
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11098 2023-05-30 03:30:13.033159 llmspec-0.3.6/LICENSE
+-rw-r--r--   0        0        0       33 2023-05-30 03:30:13.033159 llmspec-0.3.6/README.md
+-rw-r--r--   0        0        0      659 2023-05-30 03:30:13.033159 llmspec-0.3.6/llmspec/__init__.py
+-rw-r--r--   0        0        0     9640 2023-05-30 03:30:13.033159 llmspec-0.3.6/llmspec/llmspec.py
+-rw-r--r--   0        0        0      215 2023-05-30 03:30:13.033159 llmspec-0.3.6/llmspec/mixins.py
+-rw-r--r--   0        0        0     1130 2023-05-30 03:30:26.501390 llmspec-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-30 03:30:13.033159 llmspec-0.3.6/tests/dummy_test.py
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.6/PKG-INFO
```

### Comparing `llmspec-0.3.5/LICENSE` & `llmspec-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llmspec-0.3.5/llmspec/__init__.py` & `llmspec-0.3.6/llmspec/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,21 @@
     CompletionChoice,
     CompletionResponse,
     EmbeddingData,
     EmbeddingRequest,
     EmbeddingResponse,
     ErrorResponse,
     LanguageModels,
-    LLMSpec,
     PromptCompletionRequest,
     Role,
     TokenUsage,
 )
 
 __all__ = [
     "LanguageModels",
-    "LLMSpec",
     "ChatMessage",
     "ChatResponse",
     "ChatCompletionRequest",
     "ChatChoice",
     "CompletionResponse",
     "CompletionChoice",
     "PromptCompletionRequest",
```

### Comparing `llmspec-0.3.5/pyproject.toml` & `llmspec-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "msgspec>=0.15.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.3.5"
+version = "0.3.6"
 
 [project.license]
 text = "Apache-2.0"
 
 [build-system]
 requires = [
     "pdm-backend",
```

