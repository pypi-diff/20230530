# Comparing `tmp/promptlayer-0.1.83.tar.gz` & `tmp/promptlayer-0.1.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/promptlayer-0.1.83.tar", last modified: Sun May 28 18:41:21 2023, max compression
+gzip compressed data, was "dist/promptlayer-0.1.84.tar", last modified: Tue May 30 03:06:09 2023, max compression
```

## Comparing `promptlayer-0.1.83.tar` & `promptlayer-0.1.84.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.419518 promptlayer-0.1.83/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.83/LICENSE
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-28 18:41:21.419171 promptlayer-0.1.83/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.83/README.md
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.410863 promptlayer-0.1.83/promptlayer/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      496 2023-05-24 19:31:54.000000 promptlayer-0.1.83/promptlayer/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.414068 promptlayer-0.1.83/promptlayer/langchain/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.83/promptlayer/langchain/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.415305 promptlayer-0.1.83/promptlayer/langchain/llms/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.83/promptlayer/langchain/llms/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.83/promptlayer/langchain/llms/openai.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2689 2023-03-27 21:24:30.000000 promptlayer-0.1.83/promptlayer/promptlayer.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.416686 promptlayer-0.1.83/promptlayer/prompts/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.83/promptlayer/prompts/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1285 2023-03-31 18:02:42.000000 promptlayer-0.1.83/promptlayer/prompts/prompts.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.418259 promptlayer-0.1.83/promptlayer/track/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.83/promptlayer/track/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.83/promptlayer/track/track.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13445 2023-05-24 19:31:54.000000 promptlayer-0.1.83/promptlayer/utils.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-28 18:41:21.413598 promptlayer-0.1.83/promptlayer.egg-info/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-28 18:41:21.000000 promptlayer-0.1.83/promptlayer.egg-info/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      502 2023-05-28 18:41:21.000000 promptlayer-0.1.83/promptlayer.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-05-28 18:41:21.000000 promptlayer-0.1.83/promptlayer.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       36 2023-05-28 18:41:21.000000 promptlayer-0.1.83/promptlayer.egg-info/requires.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-05-28 18:41:21.000000 promptlayer-0.1.83/promptlayer.egg-info/top_level.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-05-28 18:41:21.419626 promptlayer-0.1.83/setup.cfg
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      860 2023-05-28 18:40:49.000000 promptlayer-0.1.83/setup.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.097950 promptlayer-0.1.84/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.84/LICENSE
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-30 03:06:09.097504 promptlayer-0.1.84/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.84/README.md
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.084355 promptlayer-0.1.84/promptlayer/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      888 2023-05-30 02:39:06.000000 promptlayer-0.1.84/promptlayer/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.093012 promptlayer-0.1.84/promptlayer/langchain/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.84/promptlayer/langchain/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.094205 promptlayer-0.1.84/promptlayer/langchain/llms/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.84/promptlayer/langchain/llms/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.84/promptlayer/langchain/llms/openai.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3141 2023-05-30 02:39:06.000000 promptlayer-0.1.84/promptlayer/promptlayer.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.095447 promptlayer-0.1.84/promptlayer/prompts/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.84/promptlayer/prompts/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1285 2023-03-31 18:02:42.000000 promptlayer-0.1.84/promptlayer/prompts/prompts.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.096711 promptlayer-0.1.84/promptlayer/track/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.84/promptlayer/track/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.84/promptlayer/track/track.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13445 2023-05-24 19:31:54.000000 promptlayer-0.1.84/promptlayer/utils.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-30 03:06:09.091879 promptlayer-0.1.84/promptlayer.egg-info/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-30 03:06:09.000000 promptlayer-0.1.84/promptlayer.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      502 2023-05-30 03:06:09.000000 promptlayer-0.1.84/promptlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-05-30 03:06:09.000000 promptlayer-0.1.84/promptlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       19 2023-05-30 03:06:09.000000 promptlayer-0.1.84/promptlayer.egg-info/requires.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-05-30 03:06:09.000000 promptlayer-0.1.84/promptlayer.egg-info/top_level.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-05-30 03:06:09.098099 promptlayer-0.1.84/setup.cfg
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      837 2023-05-30 03:05:33.000000 promptlayer-0.1.84/setup.py
```

### Comparing `promptlayer-0.1.83/LICENSE` & `promptlayer-0.1.84/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.83/PKG-INFO` & `promptlayer-0.1.84/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.83
+Version: 0.1.84
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.83 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.84 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.83/README.md` & `promptlayer-0.1.84/README.md`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.83/promptlayer/langchain/llms/openai.py` & `promptlayer-0.1.84/promptlayer/langchain/llms/openai.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.83/promptlayer/promptlayer.py` & `promptlayer-0.1.84/promptlayer/promptlayer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import inspect
+
 from promptlayer.utils import (
     get_api_key,
     promptlayer_api_handler,
     promptlayer_api_handler_async,
 )
 
 
@@ -12,33 +13,42 @@
 
     def __init__(self, obj, function_name="", provider_type="openai"):
         object.__setattr__(self, "_obj", obj)
         object.__setattr__(self, "_function_name", function_name)
         object.__setattr__(self, "_provider_type", provider_type)
 
     def __getattr__(self, name):
-        return PromptLayerBase(
-            getattr(object.__getattribute__(self, "_obj"), name),
-            function_name=f'{object.__getattribute__(self, "_function_name")}.{name}',
-            provider_type=object.__getattribute__(self, "_provider_type"),
-        )
+        attr = getattr(object.__getattribute__(self, "_obj"), name)
+        if inspect.isclass(attr) or inspect.isfunction(attr) or inspect.ismethod(attr):
+            return PromptLayerBase(
+                attr,
+                function_name=f'{object.__getattribute__(self, "_function_name")}.{name}',
+                provider_type=object.__getattribute__(self, "_provider_type"),
+            )
+        return attr
 
     def __delattr__(self, name):
         delattr(object.__getattribute__(self, "_obj"), name)
 
     def __setattr__(self, name, value):
         setattr(object.__getattribute__(self, "_obj"), name, value)
 
     def __call__(self, *args, **kwargs):
         tags = kwargs.pop("pl_tags", None)
         if tags is not None and not isinstance(tags, list):
             raise Exception("pl_tags must be a list of strings.")
         return_pl_id = kwargs.pop("return_pl_id", False)
         request_start_time = datetime.datetime.now().timestamp()
         function_object = object.__getattribute__(self, "_obj")
+        if inspect.isclass(function_object):
+            return PromptLayerBase(
+                function_object(*args, **kwargs),
+                function_name=object.__getattribute__(self, "_function_name"),
+                provider_type=object.__getattribute__(self, "_provider_type"),
+            )
         if inspect.iscoroutinefunction(function_object):
 
             async def async_wrapper(*args, **kwargs):
                 response = await function_object(*args, **kwargs)
                 request_end_time = datetime.datetime.now().timestamp()
                 return await promptlayer_api_handler_async(
                     object.__getattribute__(self, "_function_name"),
```

### Comparing `promptlayer-0.1.83/promptlayer/prompts/prompts.py` & `promptlayer-0.1.84/promptlayer/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.83/promptlayer/track/track.py` & `promptlayer-0.1.84/promptlayer/track/track.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.83/promptlayer/utils.py` & `promptlayer-0.1.84/promptlayer/utils.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.83/promptlayer.egg-info/PKG-INFO` & `promptlayer-0.1.84/promptlayer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.83
+Version: 0.1.84
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.83 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.84 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.83/setup.py` & `promptlayer-0.1.84/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,12 +16,12 @@
     long_description_content_type="text/markdown",
     author="Magniv",
     author_email="hello@magniv.io",
     url="https://www.promptlayer.com",
     project_urls={
         "Documentation": "https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629",
     },
-    version="0.1.83",
+    version="0.1.84",
     py_modules=["promptlayer"],
     packages=find_packages(),
-    install_requires=["requests", "openai", "langchain", "anthropic"],
+    install_requires=["requests", "langchain"],
 )
```

