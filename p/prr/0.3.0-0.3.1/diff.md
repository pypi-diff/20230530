# Comparing `tmp/prr-0.3.0.tar.gz` & `tmp/prr-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prr-0.3.0.tar", max compression
+gzip compressed data, was "prr-0.3.1.tar", max compression
```

## Comparing `prr-0.3.0.tar` & `prr-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0     1074 2023-05-07 19:46:47.449469 prr-0.3.0/LICENSE
--rw-r--r--   0        0        0    19636 2023-05-19 16:31:19.212738 prr-0.3.0/README.md
--rwxr-xr-x   0        0        0        0 2023-05-13 08:47:25.401520 prr-0.3.0/prr/__init__.py
--rwxr-xr-x   0        0        0     2596 2023-05-15 09:36:57.102458 prr-0.3.0/prr/__main__.py
--rw-r--r--   0        0        0      143 2023-05-12 09:06:58.755478 prr-0.3.0/prr/config.py
--rw-r--r--   0        0        0      931 2023-05-12 09:06:58.755747 prr-0.3.0/prr/options.py
--rw-r--r--   0        0        0     7489 2023-05-12 09:06:58.755911 prr-0.3.0/prr/prompt.py
--rw-r--r--   0        0        0      644 2023-05-12 09:06:58.756020 prr-0.3.0/prr/prompt_run.py
--rw-r--r--   0        0        0      954 2023-05-12 09:06:58.756155 prr-0.3.0/prr/prompt_run_result.py
--rw-r--r--   0        0        0      886 2023-05-12 09:06:58.756267 prr-0.3.0/prr/request.py
--rw-r--r--   0        0        0      810 2023-05-12 09:06:58.756379 prr-0.3.0/prr/response.py
--rw-r--r--   0        0        0     1086 2023-05-12 09:06:58.756486 prr-0.3.0/prr/runner.py
--rw-r--r--   0        0        0     2797 2023-05-12 09:06:58.756591 prr-0.3.0/prr/saver.py
--rw-r--r--   0        0        0      486 2023-05-12 09:06:58.756697 prr-0.3.0/prr/service_config.py
--rw-r--r--   0        0        0      858 2023-05-19 16:31:19.214514 prr-0.3.0/prr/service_registry.py
--rw-r--r--   0        0        0     2353 2023-05-19 16:31:19.214883 prr-0.3.0/prr/services/providers/anthropic/complete.py
--rw-r--r--   0        0        0     2921 2023-05-19 16:31:19.215004 prr-0.3.0/prr/services/providers/google/chat.py
--rw-r--r--   0        0        0     1931 2023-05-19 16:31:19.215259 prr-0.3.0/prr/services/providers/google/complete.py
--rw-r--r--   0        0        0     1736 2023-05-19 16:31:19.215507 prr-0.3.0/prr/services/providers/openai/chat.py
--rwxr-xr-x   0        0        0     4293 2023-05-12 09:06:58.758300 prr-0.3.0/prr/utils/run.py
--rwxr-xr-x   0        0        0     2333 2023-05-12 09:06:58.758555 prr-0.3.0/prr/utils/watch.py
--rw-r--r--   0        0        0      852 2023-05-19 16:31:29.568859 prr-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    20428 1970-01-01 00:00:00.000000 prr-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-07 19:46:47.449469 prr-0.3.1/LICENSE
+-rw-r--r--   0        0        0    20237 2023-05-30 10:52:02.806517 prr-0.3.1/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-13 08:47:25.401520 prr-0.3.1/prr/__init__.py
+-rwxr-xr-x   0        0        0     3697 2023-05-23 10:57:14.414579 prr-0.3.1/prr/__main__.py
+-rwxr-xr-x   0        0        0     4385 2023-05-23 10:57:14.414734 prr-0.3.1/prr/commands/run.py
+-rwxr-xr-x   0        0        0     2395 2023-05-23 10:57:14.414830 prr-0.3.1/prr/commands/watch.py
+-rw-r--r--   0        0        0      376 2023-05-23 10:57:14.415002 prr-0.3.1/prr/prompt/__init__.py
+-rw-r--r--   0        0        0     1744 2023-05-23 10:57:14.415110 prr-0.3.1/prr/prompt/model_options.py
+-rw-r--r--   0        0        0     6538 2023-05-23 10:57:14.415244 prr-0.3.1/prr/prompt/prompt_config.py
+-rw-r--r--   0        0        0     1980 2023-05-23 10:57:14.415364 prr-0.3.1/prr/prompt/prompt_loader.py
+-rw-r--r--   0        0        0     3165 2023-05-23 10:57:14.415488 prr-0.3.1/prr/prompt/prompt_template.py
+-rw-r--r--   0        0        0      834 2023-05-23 10:57:14.415581 prr-0.3.1/prr/prompt/service_config.py
+-rw-r--r--   0        0        0     1393 2023-05-23 10:57:14.415747 prr-0.3.1/prr/runner/__init__.py
+-rw-r--r--   0        0        0      654 2023-05-23 10:57:14.415829 prr-0.3.1/prr/runner/prompt_run.py
+-rw-r--r--   0        0        0      954 2023-05-23 10:57:14.416098 prr-0.3.1/prr/runner/prompt_run_result.py
+-rw-r--r--   0        0        0      767 2023-05-23 10:57:14.416178 prr-0.3.1/prr/runner/request.py
+-rw-r--r--   0        0        0      810 2023-05-23 10:57:14.416439 prr-0.3.1/prr/runner/response.py
+-rw-r--r--   0        0        0     2874 2023-05-23 10:57:14.416540 prr-0.3.1/prr/runner/saver.py
+-rw-r--r--   0        0        0     2436 2023-05-23 10:57:14.416727 prr-0.3.1/prr/services/providers/anthropic/complete.py
+-rw-r--r--   0        0        0     1507 2023-05-30 10:52:02.808566 prr-0.3.1/prr/services/providers/bigcode/starcoder.py
+-rw-r--r--   0        0        0     2941 2023-05-23 10:57:14.416885 prr-0.3.1/prr/services/providers/google/chat.py
+-rw-r--r--   0        0        0     1951 2023-05-23 10:57:14.417015 prr-0.3.1/prr/services/providers/google/complete.py
+-rw-r--r--   0        0        0     1429 2023-05-23 10:57:14.417158 prr-0.3.1/prr/services/providers/openai/chat.py
+-rw-r--r--   0        0        0     1073 2023-05-30 10:52:02.808827 prr-0.3.1/prr/services/service_registry.py
+-rw-r--r--   0        0        0      143 2023-05-23 10:57:14.417498 prr-0.3.1/prr/utils/config.py
+-rw-r--r--   0        0        0      907 2023-05-30 10:52:39.886565 prr-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    21127 1970-01-01 00:00:00.000000 prr-0.3.1/PKG-INFO
```

### Comparing `prr-0.3.0/LICENSE` & `prr-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prr-0.3.0/README.md` & `prr-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 - Each prompt run is recorded in detail for later analysis including raw rendered prompt and raw completion
 
 ## TODO
 
 As this is early stage work, there's lots improvements that can be done in the future and you're welcome to contribute!
 
 - [x] Get rix of Python 3.10 dependency
-- [ ] Clean basic code smells
+- [x] Clean basic code smells
 - [ ] Improve support for OpenAI and Anthropic
-- [ ] Add support for other LLM providers
+- [x] Add support for other LLM providers
 - [ ] Add support for locally hosted models
 - [ ] Pass model-related options to templating engine to allow for model-specific prompts
 - [ ] Add support for testing against expectations (elapsed_time, tokens_used)
 - [ ] Build interface to extract stats from subsequent runs for later analysis
 - [x] Add support for chat structure in prompts using YAML
 - [x] Integrate Jinja as templating language for prompts
 - [x] Make dependency files for Jinja subtemplates are tracked in watch command
@@ -118,14 +118,22 @@
 gcloud config set project <your-project-id>
 ```
 
 ```sh
 gcloud auth application-default login
 ```
 
+
+### Code completion
+Using Starcoder model you can get code completion for a variety of languages. Here's a quick example of how to use it (check out the content of `examples/code/completion.yaml`):
+
+```sh
+$ prr run ./examples/code/completion.yaml
+```
+
 ### Run a prompt from a simple text file containing just a prompt
 
 Let's create a simple text file and call it `dingo` with the following content:
 
 ```text
 What are key traits of a Dingo dog?
 ```
@@ -177,15 +185,15 @@
 If you refer to another template within your template, changes to that file will automatically be tracked too.
 
 ### Watch - cooldown mode
 
 If your prompt is often saved and you're worried of running it too often, you can use `-c` option that's specific to `watch` command which enables defined number of seconds cooldown after every run, before it proceeds to execute on your changes again.
 
 ```
-$ ./prr watch -c 15 ./subconcepts-of-buddhism
+$ prr watch -c 15 ./subconcepts-of-buddhism
 ```
 
 
 ### Prompt Scripts
 
 You can run prompts directly by setting the right first shebang line, pointing to your prr installation and using the `script` command.
 
@@ -414,14 +422,16 @@
 
 ## Available models
 
 ### Current integrations
 
 * OpenAI/chat - https://platform.openai.com/docs/guides/chat
 * Anthropic/complete - https://console.anthropic.com/docs/api
+* Google Vertex AI PaLM - https://cloud.google.com/vertex-ai/docs/generative-ai/learn/overview
+* Starcoder - https://huggingface.co/bigcode/starcoder
 
 ## Development
 
 1. Clone the repo
 
 ```sh
 $ git clone https://github.com/Forward-Operators/prr.git
@@ -446,14 +456,19 @@
 # https://platform.openai.com/account/api-keys
 OPENAI_API_KEY="sk-..."
 
 # https://console.anthropic.com/account/keys
 ANTHROPIC_API_KEY="sk-ant-..."
 
 DEFAULT_SERVICE="openai/chat/gpt-3.5-turbo"
+# https://console.cloud.google.com
+GOOGLE_PROJECT="gcp-project-id"
+GOOGLE_LOCATION="us-central1"
+# https://huggingface.co/settings/tokens
+HF_TOKEN="hf_..."
 ```
 
 You can also use DEFAULT_SERVICE to specify the model you want to use by default, but otherwise you're good to go!
 
 If you'd like to run this code during developmnent, you can use `python -m prr` to load the module.
 
 
@@ -464,10 +479,16 @@
 1. Fork the repo
 2. Create a new branch
 3. Install pre-commit - `pre-commit install`
 4. Commit your changes
 5. Push the branch to your fork
 6. Create a new Pull Request
 
+### Running unit tests
+
+```sh
+$ pytest
+```
+
 ## License
 
 **prr** - Prompt Runner is released under the [MIT License](/LICENSE).
```

#### html2text {}

```diff
@@ -17,16 +17,16 @@
 against the same prompt - Expandable to other LLM providers (current
 integrations are <100 lines of code each) - Each prompt run across models gives
 you stats on model response times and token counts used to work across
 performance, quality and cost factors - Each prompt run is recorded in detail
 for later analysis including raw rendered prompt and raw completion ## TODO As
 this is early stage work, there's lots improvements that can be done in the
 future and you're welcome to contribute! - [x] Get rix of Python 3.10
-dependency - [ ] Clean basic code smells - [ ] Improve support for OpenAI and
-Anthropic - [ ] Add support for other LLM providers - [ ] Add support for
+dependency - [x] Clean basic code smells - [ ] Improve support for OpenAI and
+Anthropic - [x] Add support for other LLM providers - [ ] Add support for
 locally hosted models - [ ] Pass model-related options to templating engine to
 allow for model-specific prompts - [ ] Add support for testing against
 expectations (elapsed_time, tokens_used) - [ ] Build interface to extract stats
 from subsequent runs for later analysis - [x] Add support for chat structure in
 prompts using YAML - [x] Integrate Jinja as templating language for prompts -
 [x] Make dependency files for Jinja subtemplates are tracked in watch command -
 [x] #!/usr/bin/prr shebang support for executable prompts - [ ] More output
@@ -53,31 +53,34 @@
 console.anthropic.com/account/keys ANTHROPIC_API_KEY="sk-ant-..."
 DEFAULT_SERVICE="openai/chat/gpt-3.5-turbo" ``` #### For Google PaLM, you need
 to install the following dependencies: You need to install [Google Cloud SDK]
 (https://cloud.google.com/sdk/docs/install) and you need to have access to a
 Vertex AI with Generative AI enabled. `prr` assumes you're logged in into your
 Google Cloud account and have access to the project you want to use. ```sh
 gcloud auth login ``` ```sh gcloud config set project  ``` ```sh gcloud auth
-application-default login ``` ### Run a prompt from a simple text file
-containing just a prompt Let's create a simple text file and call it `dingo`
-with the following content: ```text What are key traits of a Dingo dog? ``` Now
-start prr's `run` command providing path to your prompt file as argument. Let's
-use `--abbrev` option to skip showing the full prompt and completion for now.
-```sh $ prr run --abbrev ./dingo ð Reading ./dingo ð Running service
-openai/chat/gpt-3.5-turbo with default options. ð¤ openai/chat/gpt-3.5-turbo
-temperature=1.0 top_k=-1 top_p=-1 max_tokens=32 Prompt: What are key traits of
-a ... (35 chars) Completion: Here are some key traits ... (133 chars)
-Completion length: 133 bytes Tokens used: 50 Elapsed time: 2.74s ``` Your
-prompt was ran against default model with default configuration and you can see
-the execution time as well as how much tokens were used. ### Run a prompt
-against specific service With `--service` parameter, you can use any model the
-`prr` currently supports (see below) that you have configured with the API key.
-Here's how to use it against **Anthropic's Claude v1**. ```sh $ prr run --
-service anthropic/complete/claude-v1 ./subconcepts-of-buddhism ``` ###
-Templating with Jinja All prompts (whenever defined in separate files or as
+application-default login ``` ### Code completion Using Starcoder model you can
+get code completion for a variety of languages. Here's a quick example of how
+to use it (check out the content of `examples/code/completion.yaml`): ```sh $
+prr run ./examples/code/completion.yaml ``` ### Run a prompt from a simple text
+file containing just a prompt Let's create a simple text file and call it
+`dingo` with the following content: ```text What are key traits of a Dingo dog?
+``` Now start prr's `run` command providing path to your prompt file as
+argument. Let's use `--abbrev` option to skip showing the full prompt and
+completion for now. ```sh $ prr run --abbrev ./dingo ð Reading ./dingo ð
+Running service openai/chat/gpt-3.5-turbo with default options. ð¤ openai/
+chat/gpt-3.5-turbo temperature=1.0 top_k=-1 top_p=-1 max_tokens=32 Prompt: What
+are key traits of a ... (35 chars) Completion: Here are some key traits ...
+(133 chars) Completion length: 133 bytes Tokens used: 50 Elapsed time: 2.74s
+``` Your prompt was ran against default model with default configuration and
+you can see the execution time as well as how much tokens were used. ### Run a
+prompt against specific service With `--service` parameter, you can use any
+model the `prr` currently supports (see below) that you have configured with
+the API key. Here's how to use it against **Anthropic's Claude v1**. ```sh $
+prr run --service anthropic/complete/claude-v1 ./subconcepts-of-buddhism ```
+### Templating with Jinja All prompts (whenever defined in separate files or as
 values in configuration) use [Jinja](https://jinja.palletsprojects.com/en/
 3.1.x/) for templating. With that, you can easily create complex prompts with
 flow control, including other templates for easy management of larger prompts,
 and introduce variations to prompt text based on specific models (soon), among
 other things. Basic example of including external file to prompt with
 templating language: ``` Tell me all about {% include '_current_topic' %},
 please. ``` ### Watch prompt for changes to re-run it then when occur (after
@@ -86,15 +89,15 @@
 command. It allows for the same options as `run` and is able to follow changes
 to your prompt and re-execute all defined models when you save your work. ```sh
 $ prr watch ./subconcepts-of-buddhism ``` If you refer to another template
 within your template, changes to that file will automatically be tracked too.
 ### Watch - cooldown mode If your prompt is often saved and you're worried of
 running it too often, you can use `-c` option that's specific to `watch`
 command which enables defined number of seconds cooldown after every run,
-before it proceeds to execute on your changes again. ``` $ ./prr watch -c 15 ./
+before it proceeds to execute on your changes again. ``` $ prr watch -c 15 ./
 subconcepts-of-buddhism ``` ### Prompt Scripts You can run prompts directly by
 setting the right first shebang line, pointing to your prr installation and
 using the `script` command. ``` #!prr script Write a nerdcore rap song about an
 AI from the projects who reaches unbelievable levels of success, but has to
 sacrifice a lot of tokens along the way. ``` ### Prompt Scripts arguments In
 the below example, you are reading the file (let's say csv, but try other
 formats too!) passed in argument to your prompt script and including its
@@ -193,27 +196,31 @@
 ```yaml request: model: anthropic/complete/claude-v1 options: max_tokens: 64
 temperature: 0 top_k: -1 top_p: -1 response: completion_tokens: 28 log_id:
 e4ec82a710f780100ccf671f85254bcf prompt_tokens: 43 stop_reason: stop_sequence
 tokens_used: 71 total_tokens: 71 truncated: false stats: elapsed_time:
 1.1589760780334473 end_time: 1683471638.6106346 start_time: 1683471637.4516585
 ``` ## Available models ### Current integrations * OpenAI/chat - https://
 platform.openai.com/docs/guides/chat * Anthropic/complete - https://
-console.anthropic.com/docs/api ## Development 1. Clone the repo ```sh $ git
-clone https://github.com/Forward-Operators/prr.git ``` 2. Make sure you have
-Python 3.9 or 3.10 installed. If you need to have multiple Python versions in
-your system, consider using [asdf](https://github.com/asdf-vm/asdf). 3. Install
-the required packages: This project uses Poetry. See [how to install](https://
-python-poetry.org/docs/#installation) it. ```sh poetry shell poetry install ```
-It will install `prr` executable file in your active python environment. 4.
-Setup your API keys Copy `.env.example` - and save it as `~/.prr_rc`. Fill in
-your API keys for OpenAI, Anthropic and others: ```bash # https://
-platform.openai.com/account/api-keys OPENAI_API_KEY="sk-..." # https://
+console.anthropic.com/docs/api * Google Vertex AI PaLM - https://
+cloud.google.com/vertex-ai/docs/generative-ai/learn/overview * Starcoder -
+https://huggingface.co/bigcode/starcoder ## Development 1. Clone the repo ```sh
+$ git clone https://github.com/Forward-Operators/prr.git ``` 2. Make sure you
+have Python 3.9 or 3.10 installed. If you need to have multiple Python versions
+in your system, consider using [asdf](https://github.com/asdf-vm/asdf). 3.
+Install the required packages: This project uses Poetry. See [how to install]
+(https://python-poetry.org/docs/#installation) it. ```sh poetry shell poetry
+install ``` It will install `prr` executable file in your active python
+environment. 4. Setup your API keys Copy `.env.example` - and save it as
+`~/.prr_rc`. Fill in your API keys for OpenAI, Anthropic and others: ```bash #
+https://platform.openai.com/account/api-keys OPENAI_API_KEY="sk-..." # https://
 console.anthropic.com/account/keys ANTHROPIC_API_KEY="sk-ant-..."
-DEFAULT_SERVICE="openai/chat/gpt-3.5-turbo" ``` You can also use
+DEFAULT_SERVICE="openai/chat/gpt-3.5-turbo" # https://console.cloud.google.com
+GOOGLE_PROJECT="gcp-project-id" GOOGLE_LOCATION="us-central1" # https://
+huggingface.co/settings/tokens HF_TOKEN="hf_..." ``` You can also use
 DEFAULT_SERVICE to specify the model you want to use by default, but otherwise
 you're good to go! If you'd like to run this code during developmnent, you can
 use `python -m prr` to load the module. ## Contributing We'd love your help in
 making Prr even better! To contribute, please follow these steps: 1. Fork the
 repo 2. Create a new branch 3. Install pre-commit - `pre-commit install` 4.
 Commit your changes 5. Push the branch to your fork 6. Create a new Pull
-Request ## License **prr** - Prompt Runner is released under the [MIT License]
-(/LICENSE).
+Request ### Running unit tests ```sh $ pytest ``` ## License **prr** - Prompt
+Runner is released under the [MIT License](/LICENSE).
```

### Comparing `prr-0.3.0/prr/__main__.py` & `prr-0.3.1/prr/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 import argparse
 import os
 import sys
 
-from prr.config import load_config
-
-from .utils.run import RunPromptCommand
-from .utils.watch import WatchPromptCommand
+from prr.commands.run import RunPromptCommand
+from prr.commands.watch import WatchPromptCommand
+from prr.prompt.model_options import ModelOptions
+from prr.utils.config import load_config
 
 config = load_config()
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Run a prompt against configured models.",
@@ -34,21 +34,51 @@
     def add_common_args(_parser):
         _parser.add_argument(
             "--abbrev",
             help="Abbreviate prompts and completions",
             action="store_true",
             default=False,
         )
+
         _parser.add_argument(
             "--service",
             "-s",
-            help="Service to use if none is configured (defaults to DEFAULT_SERVICE environment variable)",
-            default=config["DEFAULT_SERVICE"],
+            help="Service to use if none is configured (defaults to DEFAULT_SERVICE)",
+            default=config.get("DEFAULT_SERVICE"),
             type=str,
         )
+
+        _parser.add_argument(
+            "--temperature",
+            "-t",
+            help="Temperature (defaults to DEFAULT_TEMPERATURE)",
+            type=float,
+        )
+
+        _parser.add_argument(
+            "--max_tokens",
+            "-mt",
+            help="Max tokens to use (defaults to DEFAULT_MAX_TOKENS)",
+            type=int,
+        )
+
+        _parser.add_argument(
+            "--top_p",
+            "-tp",
+            help="Sets a cumulative probability threshold for selecting candidate tokens, where only tokens with a cumulative probability higher than the threshold are considered, allowing for flexible control over the diversity of the generated output (defaults to DEFAULT_TOP_P).",
+            type=int,
+        )
+
+        _parser.add_argument(
+            "--top_k",
+            "-tk",
+            help="Determines the number of top-scoring candidate tokens to consider at each decoding step, effectively limiting the diversity of the generated output (defaults to DEFAULT_TOP_K)",
+            type=int,
+        )
+
         _parser.add_argument(
             "--quiet",
             "-q",
             help="Quiet mode, just outputs the completion",
             action="store_true",
             default=False,
         )
```

### Comparing `prr-0.3.0/prr/prompt_run.py` & `prr-0.3.1/prr/runner/prompt_run.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 
-from .prompt_run_result import PromptRunResult
+from prr.runner.prompt_run_result import PromptRunResult
 
 
 # takes prompt and model config, finds provider, runs the prompt
 class PromptRun:
     def __init__(self, prompt, service, service_config):
         self.prompt = prompt
         self.service = service
```

### Comparing `prr-0.3.0/prr/prompt_run_result.py` & `prr-0.3.1/prr/runner/prompt_run_result.py`

 * *Files identical despite different names*

### Comparing `prr-0.3.0/prr/request.py` & `prr-0.3.1/prr/runner/request.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 class ServiceRequest:
     def __init__(self, service_config, rendered_prompt_content):
         self.service_config = service_config
         self.prompt_content = rendered_prompt_content
 
     def to_dict(self):
         return {
-            "model": self.service_config.config_name(),
+            "model": self.service_config.model,
             "options": self.service_config.options.to_dict(),
-            # rendered prompt is saved to a separate file
-            # 'prompt_content': self.prompt_content,
         }
 
     def prompt_text(self, max_len=0):
         if isinstance(self.prompt_content, str):
             text = self.prompt_content
         else:
             text = yaml.dump(self.prompt_content)
```

### Comparing `prr-0.3.0/prr/response.py` & `prr-0.3.1/prr/runner/response.py`

 * *Files identical despite different names*

### Comparing `prr-0.3.0/prr/saver.py` & `prr-0.3.1/prr/runner/saver.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from datetime import datetime
 
 import yaml
 
 
 class PromptRunSaver:
-    def __init__(self, prompt):
-        self.prompt_path = prompt.path
+    def __init__(self, prompt_config):
+        self.prompt_config = prompt_config
         self.run_time = datetime.now()
         self.runs_subdir = self.run_root_directory_path()
 
     def run_root_directory_path_for_runs_dir(self, runs_dir):
         try:
             previous_runs = os.listdir(runs_dir)
         except FileNotFoundError:
@@ -22,33 +22,37 @@
 
             if not os.path.exists(run_dir):
                 return run_dir
 
             run_id += 1
 
     def run_root_directory_path(self):
-        dirname = os.path.dirname(self.prompt_path)
-        basename = os.path.basename(self.prompt_path)
+        dirname = self.prompt_config.search_path
+
+        if self.prompt_config.filename:
+            basename = os.path.basename(self.prompt_config.filename)
+        else:
+            basename = "prr"
 
         root, extension = os.path.splitext(basename)
 
         if extension == ".yaml":
             basename = root
 
         runs_dir = os.path.join(dirname, f"{basename}.runs")
 
         return self.run_root_directory_path_for_runs_dir(runs_dir)
 
-    def run_directory_path(self, model_or_model_config_name):
-        model_name_part = model_or_model_config_name.replace("/", "-")
+    def run_directory_path(self, service_or_model_name):
+        model_name_part = service_or_model_name.replace("/", "-")
 
         return os.path.join(self.runs_subdir, model_name_part)
 
-    def prepare_run_directory(self, model_or_model_config_name):
-        run_dir = self.run_directory_path(model_or_model_config_name)
+    def prepare_run_directory(self, service_or_model_name):
+        run_dir = self.run_directory_path(service_or_model_name)
 
         os.makedirs(run_dir, exist_ok=True)
 
         return run_dir
 
     def save_prompt(self, run_directory, request):
         prompt_content = request.prompt_content
@@ -74,15 +78,15 @@
     def save_run(self, run_directory, result):
         run_file = os.path.join(run_directory, f"run.yaml")
         run_data = result.metrics()
 
         with open(run_file, "w") as f:
             yaml.dump(run_data, f, default_flow_style=False)
 
-    def save(self, model_or_model_config_name, result):
-        run_directory = self.prepare_run_directory(model_or_model_config_name)
+    def save(self, service_or_model_name, result):
+        run_directory = self.prepare_run_directory(service_or_model_name)
 
         self.save_prompt(run_directory, result.request)
         self.save_completion(run_directory, result.response)
         self.save_run(run_directory, result)
 
         return run_directory
```

### Comparing `prr-0.3.0/prr/service_registry.py` & `prr-0.3.1/prr/services/service_registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from prr.services.providers.anthropic.complete import ServiceAnthropicComplete
+from prr.services.providers.bigcode.starcoder import ServiceBigcodeStarcoder
 from prr.services.providers.google.chat import ServiceGoogleChat
 from prr.services.providers.google.complete import ServiceGoogleComplete
 from prr.services.providers.openai.chat import ServiceOpenAIChat
 
 
+# main registry, where services are being... registered
+# and looked up for upon execution
 class ServiceRegistry:
     def __init__(self):
         self.services = {}
 
     def register(self, service_class):
         key = f"{service_class.provider}/{service_class.service}"
         self.services[key] = service_class()
 
     def register_all_services(self):
         self.register(ServiceOpenAIChat)
         self.register(ServiceAnthropicComplete)
+        self.register(ServiceBigcodeStarcoder)
         self.register(ServiceGoogleComplete)
         self.register(ServiceGoogleChat)
 
     def service_for_service_config(self, service_config):
         key = service_config.service_key()
         return self.services[key]
```

### Comparing `prr-0.3.0/prr/services/providers/anthropic/complete.py` & `prr-0.3.1/prr/services/providers/anthropic/complete.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # https://console.anthropic.com/docs/api/reference
 # https://github.com/anthropics/anthropic-sdk-python/tree/main/examples
 
 import os
 
 import anthropic
 
-from prr.config import load_config
-from prr.request import ServiceRequest
-from prr.response import ServiceResponse
+from prr.runner.request import ServiceRequest
+from prr.runner.response import ServiceResponse
+from prr.utils.config import load_config
 
 config = load_config()
 
-# https://console.anthropic.com/docs/api/reference
-
 
 # Anthropic model provider class
 class ServiceAnthropicComplete:
     provider = "anthropic"
     service = "complete"
 
     def run(self, prompt, service_config):
@@ -24,15 +22,19 @@
         options = self.service_config.options
         self.prompt = prompt
 
         prompt_text = self.prompt_text()
 
         client = anthropic.Client(config.get("ANTHROPIC_API_KEY", None))
 
-        service_request = ServiceRequest(self.service_config, prompt_text)
+        options = service_config.options
+
+        prompt_text = self.prompt_text_from_template(prompt.template)
+
+        service_request = ServiceRequest(service_config, prompt_text)
 
         response = client.completion(
             prompt=prompt_text,
             stop_sequences=[anthropic.HUMAN_PROMPT],
             model=service_config.model_name(),
             max_tokens_to_sample=options.max_tokens,
             temperature=options.temperature,
@@ -55,22 +57,20 @@
                 "stop_reason": response["stop_reason"],
                 "log_id": response["log_id"],
             },
         )
 
         return service_request, service_response
 
-    def prompt_text(self):
-        messages = self.prompt.messages
-
+    def prompt_text_from_template(self, template):
         prompt_text = ""
 
-        # prefer messages from prompt if they exist
-        if messages:
-            for message in messages:
-                if message["role"] != "assistant":
-                    prompt_text += " " + message["content"]
+        # prefer messages from template if they exist
+        if template.messages:
+            for message in template.messages:
+                if message.role != "assistant":
+                    prompt_text += " " + message.render_text()
 
         else:
-            prompt_text = self.prompt.text()
+            prompt_text = template.render_text()
 
         return f"{anthropic.HUMAN_PROMPT} {prompt_text}{anthropic.AI_PROMPT}"
```

### Comparing `prr-0.3.0/prr/services/providers/google/chat.py` & `prr-0.3.1/prr/services/providers/google/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from google.cloud import aiplatform
 from vertexai.preview.language_models import ChatModel, InputOutputTextPair
 
-from prr.config import load_config
-from prr.request import ServiceRequest
-from prr.response import ServiceResponse
+from prr.runner.request import ServiceRequest
+from prr.runner.response import ServiceResponse
+from prr.utils.config import load_config
 
 config = load_config()
 
 aiplatform.init(
     # your Google Cloud Project ID or number
     # environment default used is not set
     project=config.get("GOOGLE_PROJECT"),
```

### Comparing `prr-0.3.0/prr/services/providers/google/complete.py` & `prr-0.3.1/prr/services/providers/google/complete.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from google.cloud import aiplatform
 from vertexai.preview.language_models import TextGenerationModel
 
-from prr.config import load_config
-from prr.request import ServiceRequest
-from prr.response import ServiceResponse
+from prr.runner.request import ServiceRequest
+from prr.runner.response import ServiceResponse
+from prr.utils.config import load_config
 
 config = load_config()
 
 aiplatform.init(
     # your Google Cloud Project ID or number
     # environment default used is not set
     project=config.get("GOOGLE_PROJECT", None),
```

### Comparing `prr-0.3.0/prr/services/providers/openai/chat.py` & `prr-0.3.1/prr/services/providers/openai/chat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 import openai
 
-from prr.config import load_config
-from prr.request import ServiceRequest
-from prr.response import ServiceResponse
+from prr.runner.request import ServiceRequest
+from prr.runner.response import ServiceResponse
+from prr.utils.config import load_config
 
 config = load_config()
 openai.api_key = config.get("OPENAI_API_KEY", None)
 
 
 # OpenAI model provider class
 class ServiceOpenAIChat:
     provider = "openai"
     service = "chat"
 
     def run(self, prompt, service_config):
-        self.prompt = prompt
-        self.service_config = service_config
+        messages = prompt.template.render_messages()
 
-        messages = self.messages_from_prompt()
+        service_request = ServiceRequest(service_config, {"messages": messages})
 
-        service_request = ServiceRequest(self.service_config, {"messages": messages})
-
-        options = self.service_config.options
+        options = service_config.options
 
         completion = openai.ChatCompletion.create(
-            model=self.service_config.model_name(),
+            model=service_config.model_name(),
             messages=messages,
             temperature=options.temperature,
             max_tokens=options.max_tokens,
         )
 
         usage = completion.usage
 
@@ -46,16 +43,7 @@
                 "prompt_tokens": usage.prompt_tokens,
                 "total_tokens": usage.total_tokens,
                 "finish_reason": first_choice.finish_reason,
             },
         )
 
         return service_request, service_response
-
-    def messages_from_prompt(self):
-        messages = self.prompt.messages
-
-        # prefer messages in prompt if they exist
-        if messages:
-            return messages
-
-        return [{"role": "user", "content": self.prompt.text()}]
```

### Comparing `prr-0.3.0/prr/utils/run.py` & `prr-0.3.1/prr/commands/run.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 import sys
 from io import StringIO
 
 from rich import print
 from rich.console import Console
 from rich.panel import Panel
 
-# from prr.config import config
 from prr.prompt import Prompt
+from prr.prompt.prompt_loader import PromptConfigLoader
 from prr.runner import Runner
 
 console = Console(log_time=False, log_path=False)
 
 
 class RunPromptCommand:
     def __init__(self, args, prompt_args=None):
         self.args = args
         self.prompt_args = prompt_args
-        self.prompt = None
+        self.prompt_config = None
 
         if self.args["quiet"]:
             self.console = Console(file=StringIO())
         else:
             self.console = Console(log_time=False, log_path=False)
 
         self.load_prompt_for_path()
-        self.runner = Runner(self.prompt)
+        self.runner = Runner(self.prompt_config)
 
     def print_run_results(self, result, run_save_directory):
         request = result.request
         response = result.response
 
         if self.args["quiet"]:
             print(response.response_content)
@@ -53,70 +53,71 @@
                 self.console.log(
                     Panel("[yellow]" + request.prompt_text().strip() + "[/yellow]")
                 )
                 self.console.log(
                     Panel("[green]" + response.response_content.strip() + "[/green]")
                 )
 
-                completion = f"[blue]Completion length[/blue]: {len(response.response_content)} bytes"
-                tokens_used = f"[blue]Tokens used[/blue]: {response.tokens_used()}"
-                elapsed_time = (
-                    f"[blue]Elapsed time[/blue]: {round(result.elapsed_time, 2)}s"
-                )
+            completion = f"[blue]Completion length[/blue]: {len(response.response_content)} bytes"
+            tokens_used = f"[blue]Tokens used[/blue]: {response.tokens_used()}"
+            elapsed_time = (
+                f"[blue]Elapsed time[/blue]: {round(result.elapsed_time, 2)}s"
+            )
 
             self.console.log(f"{completion} {tokens_used} {elapsed_time}")
 
             if run_save_directory:
                 self.console.log(f"💾 {run_save_directory}")
 
     def run_prompt_on_service(self, service_name, save=False):
-        service_config = self.prompt.config_for_service(service_name)
+        # TODO/FIXME: doing all this here just to get the actual options
+        #             calculated after command line, defaults, config, etc
+        service_config = self.prompt_config.service_with_name(service_name)
+        service_config.process_option_overrides(self.args)
         options = service_config.options
 
         with self.console.status(
             f":robot: [bold green]{service_name}[/bold green]"
         ) as status:
             self.console.log(
                 f"\n🤖 [bold]{service_name}[/bold] {options.description()}",
                 style="frame",
             )
 
             status.update(status="running model", spinner="dots8Bit")
 
-            result, run_save_directory = self.runner.run_service(service_name, save)
+            result, run_save_directory = self.runner.run_service(
+                service_name, self.args, save
+            )
 
             self.print_run_results(result, run_save_directory)
 
     def load_prompt_for_path(self):
         prompt_path = self.args["prompt_path"]
 
-        if not os.path.exists(prompt_path) or not os.access(prompt_path, os.R_OK):
-            self.console.log(
-                f":x: Prompt file {prompt_path} is not accessible, giving up."
-            )
-            exit(-1)
-
         self.console.log(f":magnifying_glass_tilted_left: Reading {prompt_path}")
-        self.prompt = Prompt(prompt_path, self.prompt_args)
+
+        loader = PromptConfigLoader()
+        self.prompt_config = loader.load_from_path(prompt_path)
 
     def run_prompt(self):
-        services_to_run = self.prompt.configured_service_names()
+        services_to_run = self.prompt_config.configured_services()
 
         if services_to_run == []:
             if self.args["service"]:
                 services_to_run = [self.args["service"]]
                 self.console.log(
                     f":racing_car:  Running service {self.args['service']} with default options."
                 )
             else:
                 self.console.log(
-                    f":x: No services configured for prompt {self.args['prompt_path']}, nor given in command-line. Not even in .env!"
+                    f":x: No services configured for prompt {self.args['prompt_path']}, in ~/.prr_rc nor given in command-line."
                 )
                 exit(-1)
         else:
             self.console.log(f":racing_car:  Running services: {services_to_run}")
 
         if not self.args["abbrev"]:
-            self.console.log(Panel(self.prompt.text()))
+            self.console.log(Panel(self.prompt_config.template_text()))
 
-            for service_name in services_to_run:
-                self.run_prompt_on_service(service_name, self.args["log"])
+        for service_name in services_to_run:
+            self.run_prompt_on_service(service_name, self.args["log"])
```

### Comparing `prr-0.3.0/prr/utils/watch.py` & `prr-0.3.1/prr/commands/watch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 
 import datetime
 import os
 import time
 
+from prr.commands.run import RunPromptCommand
 from prr.prompt import Prompt
-from prr.utils.run import RunPromptCommand
+from prr.prompt.prompt_loader import PromptConfigLoader
 
 
 def timestamp_for_file(path):
     if os.path.exists(path):
         return os.path.getmtime(path)
 
     return 0
@@ -30,17 +31,18 @@
     def update_timestamps(self, ready_timestamps=None):
         if ready_timestamps != None:
             self.file_timestamps = ready_timestamps
         else:
             self.file_timestamps = self.current_timestamps()
 
     def setup_files_to_monitor(self):
-        prompt = Prompt(self.args["prompt_path"], self.prompt_args)
-        self.files = [prompt.path]
-        self.files.extend(prompt.dependency_files)
+        loader = PromptConfigLoader()
+        prompt_config = loader.load_from_path(self.args["prompt_path"])
+
+        self.files = loader.file_dependencies
         self.update_timestamps()
 
     def files_changed(self):
         new_timestamps = self.current_timestamps()
 
         if new_timestamps != self.file_timestamps:
             self.update_timestamps(new_timestamps)
```

### Comparing `prr-0.3.0/pyproject.toml` & `prr-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "prr"
-version = "0.3.0"
+version = "0.3.1"
 description = "prr - command-line LLM prompt runner"
 authors = [ "Zbigniew Sobiecki <zbigniew@fwdoperators.com>" , "Mateusz Kozak <mateusz@fwdoperators.com>" ]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^0.27.6"
 python-dotenv = "^1.0.0"
 anthropic = "^0.2.7"
 rich = "^13.3.5"
 Jinja2 = "^3.1.2"
 pyyaml = "^6.0"
 google-cloud-aiplatform = "^1.25.0"
+huggingface-hub = "^0.14.1"
+text-generation = "^0.5.2"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.12.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 
 [tool.poetry.scripts]
```

### Comparing `prr-0.3.0/PKG-INFO` & `prr-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: prr
-Version: 0.3.0
+Version: 0.3.1
 Summary: prr - command-line LLM prompt runner
 License: MIT
 Author: Zbigniew Sobiecki
 Author-email: zbigniew@fwdoperators.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: anthropic (>=0.2.7,<0.3.0)
 Requires-Dist: google-cloud-aiplatform (>=1.25.0,<2.0.0)
+Requires-Dist: huggingface-hub (>=0.14.1,<0.15.0)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: text-generation (>=0.5.2,<0.6.0)
 Description-Content-Type: text/markdown
 
 # prr - The Prompt Runner
 
 Welcome to **prr - The Prompt Runner**!
 
 **prr** is a simple toolchain designed to help you run prompts across multiple Large Language Models (LLMs), whether they are hosted locally or accessible through APIs. Easily refine your parameters, prompts and model choices to achieve the best results while iterating smoothly with a quick feedback loop.
@@ -49,17 +51,17 @@
 - Each prompt run is recorded in detail for later analysis including raw rendered prompt and raw completion
 
 ## TODO
 
 As this is early stage work, there's lots improvements that can be done in the future and you're welcome to contribute!
 
 - [x] Get rix of Python 3.10 dependency
-- [ ] Clean basic code smells
+- [x] Clean basic code smells
 - [ ] Improve support for OpenAI and Anthropic
-- [ ] Add support for other LLM providers
+- [x] Add support for other LLM providers
 - [ ] Add support for locally hosted models
 - [ ] Pass model-related options to templating engine to allow for model-specific prompts
 - [ ] Add support for testing against expectations (elapsed_time, tokens_used)
 - [ ] Build interface to extract stats from subsequent runs for later analysis
 - [x] Add support for chat structure in prompts using YAML
 - [x] Integrate Jinja as templating language for prompts
 - [x] Make dependency files for Jinja subtemplates are tracked in watch command
@@ -140,14 +142,22 @@
 gcloud config set project <your-project-id>
 ```
 
 ```sh
 gcloud auth application-default login
 ```
 
+
+### Code completion
+Using Starcoder model you can get code completion for a variety of languages. Here's a quick example of how to use it (check out the content of `examples/code/completion.yaml`):
+
+```sh
+$ prr run ./examples/code/completion.yaml
+```
+
 ### Run a prompt from a simple text file containing just a prompt
 
 Let's create a simple text file and call it `dingo` with the following content:
 
 ```text
 What are key traits of a Dingo dog?
 ```
@@ -199,15 +209,15 @@
 If you refer to another template within your template, changes to that file will automatically be tracked too.
 
 ### Watch - cooldown mode
 
 If your prompt is often saved and you're worried of running it too often, you can use `-c` option that's specific to `watch` command which enables defined number of seconds cooldown after every run, before it proceeds to execute on your changes again.
 
 ```
-$ ./prr watch -c 15 ./subconcepts-of-buddhism
+$ prr watch -c 15 ./subconcepts-of-buddhism
 ```
 
 
 ### Prompt Scripts
 
 You can run prompts directly by setting the right first shebang line, pointing to your prr installation and using the `script` command.
 
@@ -436,14 +446,16 @@
 
 ## Available models
 
 ### Current integrations
 
 * OpenAI/chat - https://platform.openai.com/docs/guides/chat
 * Anthropic/complete - https://console.anthropic.com/docs/api
+* Google Vertex AI PaLM - https://cloud.google.com/vertex-ai/docs/generative-ai/learn/overview
+* Starcoder - https://huggingface.co/bigcode/starcoder
 
 ## Development
 
 1. Clone the repo
 
 ```sh
 $ git clone https://github.com/Forward-Operators/prr.git
@@ -468,14 +480,19 @@
 # https://platform.openai.com/account/api-keys
 OPENAI_API_KEY="sk-..."
 
 # https://console.anthropic.com/account/keys
 ANTHROPIC_API_KEY="sk-ant-..."
 
 DEFAULT_SERVICE="openai/chat/gpt-3.5-turbo"
+# https://console.cloud.google.com
+GOOGLE_PROJECT="gcp-project-id"
+GOOGLE_LOCATION="us-central1"
+# https://huggingface.co/settings/tokens
+HF_TOKEN="hf_..."
 ```
 
 You can also use DEFAULT_SERVICE to specify the model you want to use by default, but otherwise you're good to go!
 
 If you'd like to run this code during developmnent, you can use `python -m prr` to load the module.
 
 
@@ -486,11 +503,17 @@
 1. Fork the repo
 2. Create a new branch
 3. Install pre-commit - `pre-commit install`
 4. Commit your changes
 5. Push the branch to your fork
 6. Create a new Pull Request
 
+### Running unit tests
+
+```sh
+$ pytest
+```
+
 ## License
 
 **prr** - Prompt Runner is released under the [MIT License](/LICENSE).
```

