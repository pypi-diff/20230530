# Comparing `tmp/lanarky-0.7.3.tar.gz` & `tmp/lanarky-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanarky-0.7.3.tar", max compression
+gzip compressed data, was "lanarky-0.7.4.tar", max compression
```

## Comparing `lanarky-0.7.3.tar` & `lanarky-0.7.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1073 2023-05-29 18:18:26.617325 lanarky-0.7.3/LICENSE
--rw-r--r--   0        0        0     4348 2023-05-29 18:18:26.617325 lanarky-0.7.3/README.md
--rw-r--r--   0        0        0        0 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/__init__.py
--rw-r--r--   0        0        0     2874 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/callbacks/__init__.py
--rw-r--r--   0        0        0     3023 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/callbacks/agents.py
--rw-r--r--   0        0        0     2200 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/callbacks/base.py
--rw-r--r--   0        0        0     1685 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/callbacks/llm.py
--rw-r--r--   0        0        0     3461 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0      422 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/register/__init__.py
--rw-r--r--   0        0        0     1047 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/register/base.py
--rw-r--r--   0        0        0     1014 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/register/callbacks.py
--rw-r--r--   0        0        0       74 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/responses/__init__.py
--rw-r--r--   0        0        0     2926 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/responses/streaming.py
--rw-r--r--   0        0        0      150 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/routing/__init__.py
--rw-r--r--   0        0        0     5266 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/routing/langchain.py
--rw-r--r--   0        0        0     4299 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/routing/utils.py
--rw-r--r--   0        0        0      715 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/schemas.py
--rw-r--r--   0        0        0       69 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/testing/__init__.py
--rw-r--r--   0        0        0     3212 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/testing/settings.py
--rw-r--r--   0        0        0       73 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/websockets/__init__.py
--rw-r--r--   0        0        0     3844 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/websockets/base.py
--rw-r--r--   0        0        0     1270 2023-05-29 18:18:26.813325 lanarky-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     5337 1970-01-01 00:00:00.000000 lanarky-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-30 19:46:58.936897 lanarky-0.7.4/LICENSE
+-rw-r--r--   0        0        0     4340 2023-05-30 19:46:58.936897 lanarky-0.7.4/README.md
+-rw-r--r--   0        0        0       68 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/__init__.py
+-rw-r--r--   0        0        0     2874 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/callbacks/__init__.py
+-rw-r--r--   0        0        0     3023 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/callbacks/agents.py
+-rw-r--r--   0        0        0     2200 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/callbacks/base.py
+-rw-r--r--   0        0        0     1685 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/callbacks/llm.py
+-rw-r--r--   0        0        0     3461 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0      422 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/register/__init__.py
+-rw-r--r--   0        0        0     1171 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/register/base.py
+-rw-r--r--   0        0        0     1074 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/register/callbacks.py
+-rw-r--r--   0        0        0       74 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/responses/__init__.py
+-rw-r--r--   0        0        0     2926 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/responses/streaming.py
+-rw-r--r--   0        0        0      150 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/routing/__init__.py
+-rw-r--r--   0        0        0     5266 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/routing/langchain.py
+-rw-r--r--   0        0        0     4299 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/routing/utils.py
+-rw-r--r--   0        0        0      715 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/testing/__init__.py
+-rw-r--r--   0        0        0     3212 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/websockets/__init__.py
+-rw-r--r--   0        0        0     3844 2023-05-30 19:46:59.116901 lanarky-0.7.4/lanarky/websockets/base.py
+-rw-r--r--   0        0        0     1270 2023-05-30 19:46:59.116901 lanarky-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 lanarky-0.7.4/PKG-INFO
```

### Comparing `lanarky-0.7.3/LICENSE` & `lanarky-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.3/README.md` & `lanarky-0.7.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 ```python
 from dotenv import load_dotenv
 from fastapi import FastAPI
 from langchain import ConversationChain
 from langchain.chat_models import ChatOpenAI
 
-from lanarky.routing import LangchainRouter
+from lanarky import LangchainRouter
 
 load_dotenv()
 app = FastAPI()
 
 langchain_router = LangchainRouter(
     langchain_url="/chat",
     langchain_object=ConversationChain(
```

#### html2text {}

```diff
@@ -21,15 +21,15 @@
 agnostic solution which can be easily integrated into existing backend
 infrastructures. ## ð¾ Installation The library is available on PyPI and can
 be installed via `pip`. ```bash pip install lanarky ``` You can find the full
 documentation at [https://lanarky.readthedocs.io/en/latest/](https://
 lanarky.readthedocs.io/en/latest/). ## ð¥ Build your first Langchain app
 ```python from dotenv import load_dotenv from fastapi import FastAPI from
 langchain import ConversationChain from langchain.chat_models import ChatOpenAI
-from lanarky.routing import LangchainRouter load_dotenv() app = FastAPI()
+from lanarky import LangchainRouter load_dotenv() app = FastAPI()
 langchain_router = LangchainRouter( langchain_url="/chat",
 langchain_object=ConversationChain( llm=ChatOpenAI(temperature=0), verbose=True
 ), streaming_mode=0 ) app.include_router(langchain_router) ``` See [`examples/
 `](https://github.com/ajndkr/lanarky/blob/main/examples/README.md) for list of
 available demo examples. Create a `.env` file using `.env.sample` and add your
 OpenAI API key to it before running the examples. ![demo](https://
 raw.githubusercontent.com/ajndkr/lanarky/main/assets/demo.gif) ## ð Roadmap
```

### Comparing `lanarky-0.7.3/lanarky/callbacks/__init__.py` & `lanarky-0.7.4/lanarky/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.3/lanarky/callbacks/agents.py` & `lanarky-0.7.4/lanarky/callbacks/agents.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.3/lanarky/callbacks/base.py` & `lanarky-0.7.4/lanarky/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.3/lanarky/callbacks/llm.py` & `lanarky-0.7.4/lanarky/callbacks/llm.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.3/lanarky/callbacks/retrieval_qa.py` & `lanarky-0.7.4/lanarky/callbacks/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.3/lanarky/register/base.py` & `lanarky-0.7.4/lanarky/register/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from typing import Any, Optional, Union
 
 
 def register(
-    key: Union[list[str], str], _registry: dict[str, tuple[Any, list[str]]]
+    key: Union[list[str], str],
+    _registry: dict[str, tuple[Any, list[str]]],
+    *,
+    override: bool = False,
 ) -> Any:
     """Add a class/function to a registry with required keyword arguments.
 
     ``_registry`` is a dictionary mapping from a key to a tuple of the class/function
     and a list of required keyword arguments, if keyword arguments are passed. Otherwise
     it is a dictionary mapping from a key to the class/function.
 
     Args:
         key: key or list of keys to register the class/function under.
         _registry: registry to add the class/function to.
+        override: if True, override existing keys in the registry.
     """
 
     def _register_cls(cls: Any, required_kwargs: Optional[list] = None) -> Any:
         if isinstance(key, str):
             keys = [key]
         else:
             keys = key
 
         for _key in keys:
-            if _key in _registry:
+            if _key in _registry and not override:
                 raise KeyError(f"{cls} already registered as {_key}")
             _registry[_key] = cls if required_kwargs is None else (cls, required_kwargs)
         return cls
 
     return _register_cls
```

### Comparing `lanarky-0.7.3/lanarky/register/callbacks.py` & `lanarky-0.7.4/lanarky/register/callbacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 from .base import register
 
 STREAMING_CALLBACKS: dict[str, Any] = {}
 WEBSOCKET_CALLBACKS: dict[str, Any] = {}
 STREAMING_JSON_CALLBACKS: dict[str, Any] = {}
 
 
-def register_streaming_callback(key: Union[list[str], str]) -> Callable:
+def register_streaming_callback(key: Union[list[str], str], **kwargs) -> Callable:
     """Register a streaming callback handler."""
 
     def _register_cls(cls: Any) -> Callable:
-        register(key, STREAMING_CALLBACKS)(cls=cls)
+        register(key, STREAMING_CALLBACKS, **kwargs)(cls=cls)
         return cls
 
     return _register_cls
 
 
-def register_websocket_callback(key: Union[list[str], str]) -> Callable:
+def register_websocket_callback(key: Union[list[str], str], **kwargs) -> Callable:
     """Register a websocket callback handler."""
 
     def _register_cls(cls: Any) -> Callable:
-        register(key, WEBSOCKET_CALLBACKS)(cls=cls)
+        register(key, WEBSOCKET_CALLBACKS, **kwargs)(cls=cls)
         return cls
 
     return _register_cls
 
 
-def register_streaming_json_callback(key: Union[list[str], str]) -> Callable:
+def register_streaming_json_callback(key: Union[list[str], str], **kwargs) -> Callable:
     """Register an streaming json callback handler."""
 
     def _register_cls(cls: Any) -> Callable:
-        register(key, STREAMING_JSON_CALLBACKS)(cls=cls)
+        register(key, STREAMING_JSON_CALLBACKS, **kwargs)(cls=cls)
         return cls
 
     return _register_cls
```

### Comparing `lanarky-0.7.3/lanarky/responses/streaming.py` & `lanarky-0.7.4/lanarky/responses/streaming.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.3/lanarky/routing/langchain.py` & `lanarky-0.7.4/lanarky/routing/langchain.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.3/lanarky/routing/utils.py` & `lanarky-0.7.4/lanarky/routing/utils.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.3/lanarky/schemas.py` & `lanarky-0.7.4/lanarky/schemas.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.3/lanarky/testing/gradio.py` & `lanarky-0.7.4/lanarky/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.3/lanarky/websockets/base.py` & `lanarky-0.7.4/lanarky/websockets/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.3/pyproject.toml` & `lanarky-0.7.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lanarky"
-version = "0.7.3"
+version = "0.7.4"
 description = "Ship production-ready LLM projects with FastAPI"
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ajndkr/lanarky"
 repository = "https://github.com/ajndkr/lanarky"
 license = "MIT"
 packages = [{include = "lanarky"}]
```

### Comparing `lanarky-0.7.3/PKG-INFO` & `lanarky-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanarky
-Version: 0.7.3
+Version: 0.7.4
 Summary: Ship production-ready LLM projects with FastAPI
 Home-page: https://github.com/ajndkr/lanarky
 License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -70,15 +70,15 @@
 
 ```python
 from dotenv import load_dotenv
 from fastapi import FastAPI
 from langchain import ConversationChain
 from langchain.chat_models import ChatOpenAI
 
-from lanarky.routing import LangchainRouter
+from lanarky import LangchainRouter
 
 load_dotenv()
 app = FastAPI()
 
 langchain_router = LangchainRouter(
     langchain_url="/chat",
     langchain_object=ConversationChain(
```

