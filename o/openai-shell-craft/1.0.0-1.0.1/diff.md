# Comparing `tmp/openai_shell_craft-1.0.0.tar.gz` & `tmp/openai_shell_craft-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_shell_craft-1.0.0.tar", last modified: Mon May 29 23:07:52 2023, max compression
+gzip compressed data, was "openai_shell_craft-1.0.1.tar", last modified: Mon May 29 23:10:53 2023, max compression
```

## Comparing `openai_shell_craft-1.0.0.tar` & `openai_shell_craft-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.030892 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-29 23:07:52.000000 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-29 23:07:52.000000 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:07:52.000000 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-29 23:07:52.000000 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 23:07:52.000000 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 23:07:52.000000 openai_shell_craft-1.0.0/openai_shell_craft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.030892 openai_shell_craft-1.0.0/shell_craft/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.030892 openai_shell_craft-1.0.0/shell_craft/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/shell_craft/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/factories/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/shell_craft/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/prompts/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/prompts/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/prompts/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/shell_craft/services/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/shell_craft/services/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/services/openai/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2310 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/services/openai/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/services/openai/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/shell_craft/services/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:07:52.034892 openai_shell_craft-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/tests/test_cli_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-29 23:07:41.000000 openai_shell_craft-1.0.0/tests/test_factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:10:53.751129 openai_shell_craft-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-29 23:10:53.751129 openai_shell_craft-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:10:53.747129 openai_shell_craft-1.0.1/openai_shell_craft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-29 23:10:53.000000 openai_shell_craft-1.0.1/openai_shell_craft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-29 23:10:53.000000 openai_shell_craft-1.0.1/openai_shell_craft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:10:53.000000 openai_shell_craft-1.0.1/openai_shell_craft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-29 23:10:53.000000 openai_shell_craft-1.0.1/openai_shell_craft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 23:10:53.000000 openai_shell_craft-1.0.1/openai_shell_craft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 23:10:53.000000 openai_shell_craft-1.0.1/openai_shell_craft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:10:53.751129 openai_shell_craft-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:10:53.747129 openai_shell_craft-1.0.1/shell_craft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:10:53.751129 openai_shell_craft-1.0.1/shell_craft/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/cli/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/cli/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:10:53.751129 openai_shell_craft-1.0.1/shell_craft/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/factories/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:10:53.751129 openai_shell_craft-1.0.1/shell_craft/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/prompts/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/prompts/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/prompts/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:10:53.751129 openai_shell_craft-1.0.1/shell_craft/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:10:53.751129 openai_shell_craft-1.0.1/shell_craft/services/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/services/openai/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2310 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/services/openai/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/services/openai/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/shell_craft/services/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:10:53.751129 openai_shell_craft-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/tests/test_cli_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-29 23:10:44.000000 openai_shell_craft-1.0.1/tests/test_factories.py
```

### Comparing `openai_shell_craft-1.0.0/LICENSE` & `openai_shell_craft-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/PKG-INFO` & `openai_shell_craft-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_shell_craft
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generating shell commands and code using natural language models (OpenAI ChatGPT).
 Author-email: Johnathan Irvin <irvinjohnathan@gmail.com>
 Project-URL: Homepage, https://github.com/JohnnyIrvin/shell-craft
 Project-URL: Bug Tracker, https://github.com/JohnnyIrvin/shell-craft/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_shell_craft-1.0.0/README.md` & `openai_shell_craft-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/openai_shell_craft.egg-info/PKG-INFO` & `openai_shell_craft-1.0.1/openai_shell_craft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-shell-craft
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generating shell commands and code using natural language models (OpenAI ChatGPT).
 Author-email: Johnathan Irvin <irvinjohnathan@gmail.com>
 Project-URL: Homepage, https://github.com/JohnnyIrvin/shell-craft
 Project-URL: Bug Tracker, https://github.com/JohnnyIrvin/shell-craft/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_shell_craft-1.0.0/openai_shell_craft.egg-info/SOURCES.txt` & `openai_shell_craft-1.0.1/openai_shell_craft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/pyproject.toml` & `openai_shell_craft-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openai_shell_craft"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Johnathan Irvin", email="irvinjohnathan@gmail.com" },
 ]
 description = "Generating shell commands and code using natural language models (OpenAI ChatGPT)."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `openai_shell_craft-1.0.0/shell_craft/__init__.py` & `openai_shell_craft-1.0.1/shell_craft/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/__main__.py` & `openai_shell_craft-1.0.1/shell_craft/__main__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/cli/__init__.py` & `openai_shell_craft-1.0.1/shell_craft/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/cli/commands.py` & `openai_shell_craft-1.0.1/shell_craft/cli/commands.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/cli/github.py` & `openai_shell_craft-1.0.1/shell_craft/cli/github.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/cli/main.py` & `openai_shell_craft-1.0.1/shell_craft/cli/main.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/cli/parser.py` & `openai_shell_craft-1.0.1/shell_craft/cli/parser.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/cli/prompt.py` & `openai_shell_craft-1.0.1/shell_craft/cli/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/cli/types.py` & `openai_shell_craft-1.0.1/shell_craft/cli/types.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/configuration.py` & `openai_shell_craft-1.0.1/shell_craft/configuration.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/factories/__init__.py` & `openai_shell_craft-1.0.1/shell_craft/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/factories/prompt.py` & `openai_shell_craft-1.0.1/shell_craft/factories/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/prompts/__init__.py` & `openai_shell_craft-1.0.1/shell_craft/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/prompts/languages.py` & `openai_shell_craft-1.0.1/shell_craft/prompts/languages.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/prompts/prompt.py` & `openai_shell_craft-1.0.1/shell_craft/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/prompts/templates.py` & `openai_shell_craft-1.0.1/shell_craft/prompts/templates.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/services/__init__.py` & `openai_shell_craft-1.0.1/shell_craft/services/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/services/openai/__init__.py` & `openai_shell_craft-1.0.1/shell_craft/services/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/services/openai/service.py` & `openai_shell_craft-1.0.1/shell_craft/services/openai/service.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/services/openai/settings.py` & `openai_shell_craft-1.0.1/shell_craft/services/openai/settings.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/shell_craft/services/service.py` & `openai_shell_craft-1.0.1/shell_craft/services/service.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/tests/test_cli_types.py` & `openai_shell_craft-1.0.1/tests/test_cli_types.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/tests/test_configuration.py` & `openai_shell_craft-1.0.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-1.0.0/tests/test_factories.py` & `openai_shell_craft-1.0.1/tests/test_factories.py`

 * *Files identical despite different names*

