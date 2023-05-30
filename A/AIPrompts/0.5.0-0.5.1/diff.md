# Comparing `tmp/AIPrompts-0.5.0.tar.gz` & `tmp/AIPrompts-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIPrompts-0.5.0.tar", last modified: Sun May 21 00:58:49 2023, max compression
+gzip compressed data, was "AIPrompts-0.5.1.tar", last modified: Tue May 30 19:16:06 2023, max compression
```

## Comparing `AIPrompts-0.5.0.tar` & `AIPrompts-0.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:58:49.847573 AIPrompts-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:58:49.843572 AIPrompts-0.5.0/AIPrompts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-21 00:58:49.000000 AIPrompts-0.5.0/AIPrompts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-21 00:58:49.000000 AIPrompts-0.5.0/AIPrompts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:58:49.000000 AIPrompts-0.5.0/AIPrompts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-21 00:58:49.000000 AIPrompts-0.5.0/AIPrompts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 00:58:49.000000 AIPrompts-0.5.0/AIPrompts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-21 00:58:49.847573 AIPrompts-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:58:49.847573 AIPrompts-0.5.0/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/turbo.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:58:49.847573 AIPrompts-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:58:49.847573 AIPrompts-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/tests/test_turbo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:16:06.479989 AIPrompts-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:16:06.475989 AIPrompts-0.5.1/AIPrompts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-30 19:16:06.000000 AIPrompts-0.5.1/AIPrompts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-30 19:16:06.000000 AIPrompts-0.5.1/AIPrompts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:16:06.000000 AIPrompts-0.5.1/AIPrompts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 19:16:06.000000 AIPrompts-0.5.1/AIPrompts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 19:16:06.000000 AIPrompts-0.5.1/AIPrompts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-30 19:16:06.479989 AIPrompts-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:16:06.479989 AIPrompts-0.5.1/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:16:06.479989 AIPrompts-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:16:06.479989 AIPrompts-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/tests/test_turbo.py
```

### Comparing `AIPrompts-0.5.0/AIPrompts.egg-info/PKG-INFO` & `AIPrompts-0.5.1/AIPrompts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPrompts
-Version: 0.5.0
+Version: 0.5.1
 Summary: Create and parse prompts for large language models.
 Home-page: https://github.com/TeiaLabs/prompts
 Author: Teialabs
 Author-email: jonatas@teialabs.com
 Keywords: prompt openai teialabs gpt3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `AIPrompts-0.5.0/PKG-INFO` & `AIPrompts-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPrompts
-Version: 0.5.0
+Version: 0.5.1
 Summary: Create and parse prompts for large language models.
 Home-page: https://github.com/TeiaLabs/prompts
 Author: Teialabs
 Author-email: jonatas@teialabs.com
 Keywords: prompt openai teialabs gpt3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `AIPrompts-0.5.0/README.md` & `AIPrompts-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.0/prompts/dynamic.py` & `AIPrompts-0.5.1/prompts/dynamic.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.0/prompts/ensemble.py` & `AIPrompts-0.5.1/prompts/ensemble.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.0/prompts/exceptions.py` & `AIPrompts-0.5.1/prompts/exceptions.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.0/prompts/schemas.py` & `AIPrompts-0.5.1/prompts/schemas.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,41 +37,35 @@
 
 class PromptRole(str, Enum):
     USER = "user"
     SYSTEM = "system"
     ASSISTANT = "assistant"
 
 
-class TemplateData(BaseModel):
-    # Openai inputs
+class TemplateInputs(BaseModel):
     inputs: dict[str, str]
     name: str | None = None
     role: PromptRole
-
-    # Prompts template management
+    # advanced usage: select sub-templates
     template_name: str = "default"
 
 
-class TemplateContent(BaseModel):
-    # Openai inputs
+class ChatMLMessage(BaseModel):
     content: str
     name: str | None = None
     role: PromptRole
 
-    # Prompts template management
-    template_name: str = "default"
-
 
 class TurboSchema(BaseModel):
     # Prompt identification
     name: str
     description: str = ""
     # Engine settings
     settings: OpenAIModelSettings
     # Prompt templates
     system_templates: list[Template] | str
     user_templates: list[Template] | str
     assistant_templates: list[Template] | str
     # Prompt initial config
-    initial_template_data: list[TemplateData | TemplateContent] = Field(
+    initial_template_data: list[TemplateInputs | ChatMLMessage] = Field(
         default_factory=list
     )
```

### Comparing `AIPrompts-0.5.0/prompts/turbo.py` & `AIPrompts-0.5.1/prompts/turbo.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import yaml
 
 from .dynamic import DynamicPrompt
 from .schemas import (
     OpenAIModelSettings,
     PromptRole,
     Template,
-    TemplateContent,
-    TemplateData,
+    ChatMLMessage,
+    TemplateInputs,
     TurboSchema,
 )
 
 TEMPLATE_TYPE = list[Template] | DynamicPrompt | str | None
 
 
 class TurboPrompt:
@@ -134,17 +134,17 @@
         if name is not None:
             prompt_message["name"] = name
         self.prompts.append(prompt_message)
 
     def build(self, **_) -> list[dict[str, str]]:
         return copy.deepcopy(self.prompts)
 
-    def add_raw_content(self, content_item: dict | TemplateContent):
+    def add_raw_content(self, content_item: dict | ChatMLMessage):
         if isinstance(content_item, dict):
-            content_item = TemplateContent(**content_item)
+            content_item = ChatMLMessage(**content_item)
 
         self._add_prompt(
             prompt_type=content_item.role,
             prompt=content_item.content,
             name=content_item.name,
         )
 
@@ -194,21 +194,21 @@
             raise ValueError(
                 f"{type}_prompt must be a string or a list of strings/prompts"
             )
 
     def add_initial_template_data(
         self,
         prompt: "TurboPrompt",
-        initial_template_data: list[TemplateData | TemplateContent] | None,
+        initial_template_data: list[TemplateInputs | ChatMLMessage] | None,
     ) -> None:
         if initial_template_data is None:
             return
 
         for hist in initial_template_data:
-            if isinstance(hist, TemplateContent):
+            if isinstance(hist, ChatMLMessage):
                 prompt.add_raw_content(hist)
                 continue
 
             if hist.role == PromptRole.SYSTEM:
                 prompt.add_system_message(
                     template_name=hist.template_name, **hist.inputs
                 )
@@ -231,15 +231,15 @@
 
     @classmethod
     def from_settings(
         cls,
         name: str,
         description: str,
         settings: OpenAIModelSettings,
-        initial_template_data: list[TemplateData | TemplateContent],
+        initial_template_data: list[TemplateInputs | ChatMLMessage],
         system_template: list[Template] | str = "",
         user_template: list[Template] | str = "",
         assistant_template: list[Template] | str = "",
     ):
         tbs = TurboSchema(
             name=name,
             description=description,
```

### Comparing `AIPrompts-0.5.0/setup.py` & `AIPrompts-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.0/tests/test_ensemble.py` & `AIPrompts-0.5.1/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.0/tests/test_prompt.py` & `AIPrompts-0.5.1/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.0/tests/test_turbo.py` & `AIPrompts-0.5.1/tests/test_turbo.py`

 * *Files identical despite different names*

