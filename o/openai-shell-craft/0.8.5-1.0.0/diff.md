# Comparing `tmp/openai_shell_craft-0.8.5.tar.gz` & `tmp/openai_shell_craft-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_shell_craft-0.8.5.tar", last modified: Thu May 25 00:57:00 2023, max compression
+gzip compressed data, was "openai_shell_craft-1.0.0.tar", last modified: Mon May 29 23:07:52 2023, max compression
```

## Comparing `openai_shell_craft-0.8.5.tar` & `openai_shell_craft-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:57:00.417746 openai_shell_craft-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-05-25 00:57:00.417746 openai_shell_craft-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:57:00.413746 openai_shell_craft-0.8.5/openai_shell_craft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-05-25 00:57:00.000000 openai_shell_craft-0.8.5/openai_shell_craft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-25 00:57:00.000000 openai_shell_craft-0.8.5/openai_shell_craft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 00:57:00.000000 openai_shell_craft-0.8.5/openai_shell_craft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-25 00:57:00.000000 openai_shell_craft-0.8.5/openai_shell_craft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 00:57:00.000000 openai_shell_craft-0.8.5/openai_shell_craft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 00:57:00.000000 openai_shell_craft-0.8.5/openai_shell_craft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 00:57:00.417746 openai_shell_craft-0.8.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:57:00.413746 openai_shell_craft-0.8.5/shell_craft/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:57:00.413746 openai_shell_craft-0.8.5/shell_craft/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/cli/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/cli/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/cli/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/cli/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/cli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/cli/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/cli/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/cli/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:57:00.413746 openai_shell_craft-0.8.5/shell_craft/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/factories/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:57:00.417746 openai_shell_craft-0.8.5/shell_craft/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/prompts/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/prompts/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/prompts/templates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3388 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/shell_craft/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:57:00.417746 openai_shell_craft-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-25 00:56:50.000000 openai_shell_craft-0.8.5/tests/test_factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.030892 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-29 23:07:52.000000 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-29 23:07:52.000000 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:07:52.000000 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-29 23:07:52.000000 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 23:07:52.000000 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 23:07:52.000000 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.030892 openai_shell_craft-1.0.0/shell_craft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.030892 openai_shell_craft-1.0.0/shell_craft/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/shell_craft/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/factories/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/shell_craft/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/prompts/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/prompts/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/prompts/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/shell_craft/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/shell_craft/services/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/services/openai/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2310 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/services/openai/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/services/openai/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/services/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/tests/test_cli_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/tests/test_factories.py
```

### Comparing `openai_shell_craft-0.8.5/LICENSE` & `openai_shell_craft-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.5/PKG-INFO` & `openai_shell_craft-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: openai_shell_craft
-Version: 0.8.5
-Summary: Generating shell commands and code using natural language models (OpenAI ChatGPT).
-Author-email: Johnathan Irvin <irvinjohnathan@gmail.com>
-Project-URL: Homepage, https://github.com/JohnnyIrvin/shell-craft
-Project-URL: Bug Tracker, https://github.com/JohnnyIrvin/shell-craft/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Shell Craft
 
 [![PyPI version](https://img.shields.io/pypi/v/openai-shell-craft?color=green&label=PyPI)](https://pypi.org/project/openai-shell-craft/) [![codecov](https://codecov.io/gh/JohnnyIrvin/shell-craft/branch/trunk/graph/badge.svg?token=MKYZOJR8SQ)](https://codecov.io/gh/JohnnyIrvin/shell-craft)
 
 Generating shell commands and code using natural language models (OpenAI ChatGPT). 
 
 Shell Craft can:
@@ -57,23 +43,30 @@
 ## Python API
 
 The following example shows how to use Shell Craft inside of your own Python code. The example loads your api key from an environment variable, uses the Bash prompt, and gets input from the user.
 
 ```python
 import os
 
-from shell_craft import Service
+from shell_craft.services import OpenAIService, OpenAISettings
 from shell_craft.prompts import BASH_PROMPT
 
-Service(
-    api_key = os.environ.get("OPENAI_API_KEY"),
-    prompt = BASH_PROMPT,
+results = OpenAIService(
+    OpenAISettings(
+        api_key = os.environ.get("OPENAI_API_KEY"),
+        model='gpt-3.5-turbo',
+        count=1,
+        temperature=0.0,
+        messages=BASH_PROMPT.messages,
+    )
 ).query(
     message = input("Enter your request: ")
 )
+
+print(results)
 ```
 
 ## API Key
 
 Shell Craft uses the OpenAI API to generate the shell commands, requiring an API key to give it access to an account with OpenAI.
 
 _Warning! **API keys are sensitive information** and should be kept confidential. Don't share your API key with anyone who shouldn't have access to it. Failure to do so may result in charges on your OpenAI account. Shell Craft never transmits this key to any service other than the official OpenAI API. **Your API key** is **your responsibility**._
```

### Comparing `openai_shell_craft-0.8.5/README.md` & `openai_shell_craft-1.0.0/openai_shell_craft.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: openai-shell-craft
+Version: 1.0.0
+Summary: Generating shell commands and code using natural language models (OpenAI ChatGPT).
+Author-email: Johnathan Irvin <irvinjohnathan@gmail.com>
+Project-URL: Homepage, https://github.com/JohnnyIrvin/shell-craft
+Project-URL: Bug Tracker, https://github.com/JohnnyIrvin/shell-craft/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Shell Craft
 
 [![PyPI version](https://img.shields.io/pypi/v/openai-shell-craft?color=green&label=PyPI)](https://pypi.org/project/openai-shell-craft/) [![codecov](https://codecov.io/gh/JohnnyIrvin/shell-craft/branch/trunk/graph/badge.svg?token=MKYZOJR8SQ)](https://codecov.io/gh/JohnnyIrvin/shell-craft)
 
 Generating shell commands and code using natural language models (OpenAI ChatGPT). 
 
 Shell Craft can:
@@ -43,23 +57,30 @@
 ## Python API
 
 The following example shows how to use Shell Craft inside of your own Python code. The example loads your api key from an environment variable, uses the Bash prompt, and gets input from the user.
 
 ```python
 import os
 
-from shell_craft import Service
+from shell_craft.services import OpenAIService, OpenAISettings
 from shell_craft.prompts import BASH_PROMPT
 
-Service(
-    api_key = os.environ.get("OPENAI_API_KEY"),
-    prompt = BASH_PROMPT,
+results = OpenAIService(
+    OpenAISettings(
+        api_key = os.environ.get("OPENAI_API_KEY"),
+        model='gpt-3.5-turbo',
+        count=1,
+        temperature=0.0,
+        messages=BASH_PROMPT.messages,
+    )
 ).query(
     message = input("Enter your request: ")
 )
+
+print(results)
 ```
 
 ## API Key
 
 Shell Craft uses the OpenAI API to generate the shell commands, requiring an API key to give it access to an account with OpenAI.
 
 _Warning! **API keys are sensitive information** and should be kept confidential. Don't share your API key with anyone who shouldn't have access to it. Failure to do so may result in charges on your OpenAI account. Shell Craft never transmits this key to any service other than the official OpenAI API. **Your API key** is **your responsibility**._
```

### Comparing `openai_shell_craft-0.8.5/openai_shell_craft.egg-info/PKG-INFO` & `openai_shell_craft-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openai-shell-craft
-Version: 0.8.5
+Name: openai_shell_craft
+Version: 1.0.0
 Summary: Generating shell commands and code using natural language models (OpenAI ChatGPT).
 Author-email: Johnathan Irvin <irvinjohnathan@gmail.com>
 Project-URL: Homepage, https://github.com/JohnnyIrvin/shell-craft
 Project-URL: Bug Tracker, https://github.com/JohnnyIrvin/shell-craft/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -57,23 +57,30 @@
 ## Python API
 
 The following example shows how to use Shell Craft inside of your own Python code. The example loads your api key from an environment variable, uses the Bash prompt, and gets input from the user.
 
 ```python
 import os
 
-from shell_craft import Service
+from shell_craft.services import OpenAIService, OpenAISettings
 from shell_craft.prompts import BASH_PROMPT
 
-Service(
-    api_key = os.environ.get("OPENAI_API_KEY"),
-    prompt = BASH_PROMPT,
+results = OpenAIService(
+    OpenAISettings(
+        api_key = os.environ.get("OPENAI_API_KEY"),
+        model='gpt-3.5-turbo',
+        count=1,
+        temperature=0.0,
+        messages=BASH_PROMPT.messages,
+    )
 ).query(
     message = input("Enter your request: ")
 )
+
+print(results)
 ```
 
 ## API Key
 
 Shell Craft uses the OpenAI API to generate the shell commands, requiring an API key to give it access to an account with OpenAI.
 
 _Warning! **API keys are sensitive information** and should be kept confidential. Don't share your API key with anyone who shouldn't have access to it. Failure to do so may result in charges on your OpenAI account. Shell Craft never transmits this key to any service other than the official OpenAI API. **Your API key** is **your responsibility**._
```

### Comparing `openai_shell_craft-0.8.5/pyproject.toml` & `openai_shell_craft-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openai_shell_craft"
-version = "0.8.5"
+version = "1.0.0"
 authors = [
   { name="Johnathan Irvin", email="irvinjohnathan@gmail.com" },
 ]
 description = "Generating shell commands and code using natural language models (OpenAI ChatGPT)."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `openai_shell_craft-0.8.5/shell_craft/__init__.py` & `openai_shell_craft-1.0.0/shell_craft/factories/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 Johnathan P. Irvin
+# Copyright (c) 2023 Johnathan P. Irvin and contributors
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -14,10 +14,10 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-from .service import Service
+from .prompt import PromptFactory
 
-__all__ = ["Service"]
+__all__ = ["PromptFactory"]
```

### Comparing `openai_shell_craft-0.8.5/shell_craft/__main__.py` & `openai_shell_craft-1.0.0/shell_craft/__main__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.5/shell_craft/cli/__init__.py` & `openai_shell_craft-1.0.0/shell_craft/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.5/shell_craft/cli/language.py` & `openai_shell_craft-1.0.0/shell_craft/factories/prompt.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,40 +14,42 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-from argparse import ArgumentParser
-from shell_craft.factories import PromptFactory
-from shell_craft.prompts import languages
-
-ARGUMENTS = {
-    'prompt': lambda x: PromptFactory.get_prompt(x) in languages.get_prompts()
-}
-
-def add_arguments(parser: ArgumentParser):
-    """
-    Adds 'request' argument to the parser. This argument is used to
-    specify the input to prompt the API with. This argument is required,
-    however, it can be piped in from another command or from a file.
-
-    Args:
-        parser (ArgumentParser): The parser to add the argument to.
-    """
-    group = parser.add_mutually_exclusive_group(required=False)
-    group.add_argument(
-        '--refactor',
-        action='store_true',
-        help='Refactor the code.'
-    )
-    group.add_argument(
-        '--document',
-        action='store_true',
-        help='Document the code.'
-    )
-    group.add_argument(
-        '--test',
-        action='store_true',
-        help='Test the code.'
-    )
+from shell_craft.prompts import Prompt
+
+
+class PromptFactory:
+    @staticmethod
+    def get_prompt(prompt: str) -> Prompt:
+        """
+        Generates a new prompt object based on the prompt type. If the prompt
+        type is not supported, a ValueError is raised.
+
+        Args:
+            prompt (str): A string representing the prompt type.
+
+        Raises:
+            ValueError: If the prompt type is not supported.
+
+        Returns:
+            Prompt: A new prompt object.
+        """        
+        import shell_craft.prompts as prompts
+
+        if not prompt:
+            return None
+
+        available_prompts = [
+            prompt.removesuffix('_PROMPT').casefold()
+            for prompt in dir(prompts)
+            if prompt.endswith("_PROMPT")
+        ]
+
+        if prompt.casefold() in available_prompts:
+            return getattr(prompts, f"{prompt.upper()}_PROMPT")
+
+
+        raise ValueError(f"Unknown prompt type: {prompt}")
```

### Comparing `openai_shell_craft-0.8.5/shell_craft/cli/models.py` & `openai_shell_craft-1.0.0/shell_craft/services/service.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 Johnathan P. Irvin and contributors
+# Copyright (c) 2023 Johnathan P. Irvin
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -14,35 +14,23 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-from argparse import ArgumentParser
+from typing import Protocol
 
 
-def add_arguments(parser: ArgumentParser):
-    """
-    Adds '--model' argument to the parser. This argument is used to specify
-    openai's model to use. The default is 'gpt-3.5-turbo'. This argument is
-    optional. The models are provided by the OpenAI API but not all models
-    are available to all users. Nor are all models implemented in the
-    shell_craft library.
+class Service(Protocol):
+    def query(self, message: str) -> list[str]:
+        """
+        Querys the foreign service with the given message and returns the
+        results.
 
-    Args:
-        parser (ArgumentParser): The parser to add the argument to.
-    """    
-    parser.add_argument(
-        "--model",
-        type=str,
-        default="gpt-3.5-turbo",
-        help="The input to prompt the API with.",
-        choices=[
-            "gpt-4",
-            "gpt-4-0314",
-            "gpt-4-32k",
-            "gpt-4-32k-0314",
-            "gpt-3.5-turbo",
-            "gpt-3.5-turbo-0301",
-        ]
-    )
+        Args:
+            message (str): The message to query the foreign service with.
+
+        Returns:
+            list[str]: The results of the query.
+        """        
+        ...
```

### Comparing `openai_shell_craft-0.8.5/shell_craft/cli/prompt.py` & `openai_shell_craft-1.0.0/shell_craft/cli/prompt.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,21 +14,18 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-from argparse import ArgumentParser
 from os import getppid
 
 from psutil import NoSuchProcess, Process
 
-import shell_craft.prompts as prompts
-
 
 def get_calling_shell() -> str:
     """
     Get the name of the shell that called this script. This is used to determine
     the default prompt type. If the calling shell is PowerShell or pwsh, it is converted
     to "powershell" to match the prompt type. If the calling shell is not recognized,
     the default prompt type is "bash".
@@ -42,30 +39,7 @@
         return (
             "powershell" 
             if Process(getppid()).name() in 
             ["pwsh", "powershell"] else "bash"
         )
     except NoSuchProcess:
         return "bash"
-
-
-def add_arguments(parser: ArgumentParser):
-    """
-    Adds '--prompt' as an argument to the parser. The choices are the names of
-    the prompts in the prompts module, without the '_PROMPT' suffix, and converted to
-    lowercase. The default is the name of the shell that called this script.
-
-    Args:
-        parser (ArgumentParser): The parser to add the argument to.
-    """    
-    parser.add_argument(
-        "--prompt",
-        type=str,
-        choices=[
-            prompt.removesuffix('_PROMPT').lower()
-            for prompt in dir(prompts)
-            if prompt.endswith("PROMPT")
-        ],
-        help="The type of prompt to use.",
-        nargs='?',
-        default=get_calling_shell()
-    )
```

### Comparing `openai_shell_craft-0.8.5/shell_craft/cli/request.py` & `openai_shell_craft-1.0.0/shell_craft/cli/types.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,24 +14,40 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-from argparse import ArgumentParser
+from argparse import ArgumentTypeError
+from typing import Callable
 
 
-def add_arguments(parser: ArgumentParser):
+def limited_float(min: float, max: float) -> Callable:
     """
-    Adds 'request' argument to the parser. This argument is used to
-    specify the input to prompt the API with. This argument is required,
-    however, it can be piped in from another command or from a file.
+    Create a function that will validate a float is between the given min and
+    max values for use with argparse.
 
     Args:
-        parser (ArgumentParser): The parser to add the argument to.
+        min (float): The minimum value for the float.
+        max (float): The maximum value for the float.
+
+    Returns:
+        Callable: A function that will validate a float is between the given min
     """    
-    parser.add_argument(
-        "request",
-        type=str,
-        nargs="*",
-    )
+    def _ret_func(arg: str) -> float:
+        if arg is None or not str(arg).isdecimal:
+            raise ArgumentTypeError(f"{arg} is not a decimal")
+        
+        f = float(arg)
+        if f in [float("inf"), float("-inf")]:
+            raise ArgumentTypeError(f"{arg} is not a decimal")
+        
+        if f != f:
+            raise ArgumentTypeError(f"{arg} is not a decimal")
+
+        if f < min or f > max:
+            raise ArgumentTypeError(f"{arg} is not between {min} and {max}")
+        
+        return f
+    
+    return _ret_func
```

### Comparing `openai_shell_craft-0.8.5/shell_craft/factories/__init__.py` & `openai_shell_craft-1.0.0/shell_craft/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 Johnathan P. Irvin and contributors
+# Copyright (c) 2023 Johnathan P. Irvin
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -14,10 +14,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-from .prompt import PromptFactory
-
-__all__ = ["PromptFactory"]
```

### Comparing `openai_shell_craft-0.8.5/shell_craft/factories/prompt.py` & `openai_shell_craft-1.0.0/tests/test_factories.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,42 +14,28 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-from shell_craft.prompts import Prompt
+import pytest
 
+import shell_craft.prompts as prompts
+from shell_craft.factories import PromptFactory
 
-class PromptFactory:
-    @staticmethod
-    def get_prompt(prompt: str) -> Prompt:
-        """
-        Generates a new prompt object based on the prompt type. If the prompt
-        type is not supported, a ValueError is raised.
-
-        Args:
-            prompt (str): A string representing the prompt type.
-
-        Raises:
-            ValueError: If the prompt type is not supported.
-
-        Returns:
-            Prompt: A new prompt object.
-        """        
-        import shell_craft.prompts as prompts
-
-        if not prompt:
-            return None
-
-        available_prompts = [
-            prompt.removesuffix('_PROMPT').casefold()
-            for prompt in dir(prompts)
-            if prompt.endswith("_PROMPT")
-        ]
-
-        if prompt.casefold() in available_prompts:
-            return getattr(prompts, f"{prompt.upper()}_PROMPT")
-
-
-        raise ValueError(f"Unknown prompt type: {prompt}")
+PROMPTS = [
+    prompt
+    for prompt in dir(prompts)
+    if prompt.endswith("_PROMPT")
+    and not prompt.startswith("_")
+]
+
+@pytest.mark.parametrize("prompt", PROMPTS)
+def test_prompt_factory(prompt: str):
+    """
+    Test that the prompt factory returns the correct prompt.
+
+    Args:
+        prompt (str): The prompt to test.
+    """    
+    assert PromptFactory.get_prompt(prompt.removesuffix("_PROMPT")) == getattr(prompts, prompt)
```

### Comparing `openai_shell_craft-0.8.5/shell_craft/prompts/__init__.py` & `openai_shell_craft-1.0.0/shell_craft/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.5/shell_craft/prompts/languages.py` & `openai_shell_craft-1.0.0/shell_craft/prompts/languages.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.5/shell_craft/prompts/prompt.py` & `openai_shell_craft-1.0.0/shell_craft/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.5/shell_craft/prompts/templates.py` & `openai_shell_craft-1.0.0/shell_craft/prompts/templates.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.8.5/tests/test_factories.py` & `openai_shell_craft-1.0.0/shell_craft/services/openai/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 Johnathan P. Irvin and contributors
+# Copyright (c) 2023 Johnathan P. Irvin
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -14,28 +14,13 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-import pytest
+from .service import OpenAIService, OpenAISettings
 
-import shell_craft.prompts as prompts
-from shell_craft.factories import PromptFactory
-
-PROMPTS = [
-    prompt
-    for prompt in dir(prompts)
-    if prompt.endswith("_PROMPT")
-    and not prompt.startswith("_")
+__all__ = [
+    'OpenAIService',
+    'OpenAISettings',
 ]
-
-@pytest.mark.parametrize("prompt", PROMPTS)
-def test_prompt_factory(prompt: str):
-    """
-    Test that the prompt factory returns the correct prompt.
-
-    Args:
-        prompt (str): The prompt to test.
-    """    
-    assert PromptFactory.get_prompt(prompt.removesuffix("_PROMPT")) == getattr(prompts, prompt)
```

