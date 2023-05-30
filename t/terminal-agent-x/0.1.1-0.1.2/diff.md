# Comparing `tmp/terminal-agent-x-0.1.1.tar.gz` & `tmp/terminal-agent-x-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal-agent-x-0.1.1.tar", last modified: Wed May 24 17:23:40 2023, max compression
+gzip compressed data, was "terminal-agent-x-0.1.2.tar", last modified: Tue May 30 03:21:18 2023, max compression
```

## Comparing `terminal-agent-x-0.1.1.tar` & `terminal-agent-x-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-24 17:23:40.149061 terminal-agent-x-0.1.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-05-08 10:01:27.000000 terminal-agent-x-0.1.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2602 2023-05-24 17:23:40.149061 terminal-agent-x-0.1.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1840 2023-05-24 17:23:29.000000 terminal-agent-x-0.1.1/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      869 2023-05-24 17:08:45.000000 terminal-agent-x-0.1.1/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-24 17:23:40.149061 terminal-agent-x-0.1.1/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-24 17:23:40.145061 terminal-agent-x-0.1.1/terminal_agent_x/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-09 00:14:06.000000 terminal-agent-x-0.1.1/terminal_agent_x/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4359 2023-05-24 17:07:28.000000 terminal-agent-x-0.1.1/terminal_agent_x/tax.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-24 17:23:40.149061 terminal-agent-x-0.1.1/terminal_agent_x.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2602 2023-05-24 17:23:40.000000 terminal-agent-x-0.1.1/terminal_agent_x.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      288 2023-05-24 17:23:40.000000 terminal-agent-x-0.1.1/terminal_agent_x.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-24 17:23:40.000000 terminal-agent-x-0.1.1/terminal_agent_x.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-05-24 17:23:40.000000 terminal-agent-x-0.1.1/terminal_agent_x.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-05-24 17:23:40.000000 terminal-agent-x-0.1.1/terminal_agent_x.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-30 03:21:18.426922 terminal-agent-x-0.1.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-05-08 10:01:27.000000 terminal-agent-x-0.1.2/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3394 2023-05-30 03:21:18.426922 terminal-agent-x-0.1.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2582 2023-05-30 03:17:04.000000 terminal-agent-x-0.1.2/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      914 2023-05-30 03:16:22.000000 terminal-agent-x-0.1.2/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-30 03:21:18.426922 terminal-agent-x-0.1.2/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-30 03:21:18.426922 terminal-agent-x-0.1.2/terminal_agent_x/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-09 00:14:06.000000 terminal-agent-x-0.1.2/terminal_agent_x/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5940 2023-05-30 03:06:35.000000 terminal-agent-x-0.1.2/terminal_agent_x/tax.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-30 03:21:18.426922 terminal-agent-x-0.1.2/terminal_agent_x.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3394 2023-05-30 03:21:18.000000 terminal-agent-x-0.1.2/terminal_agent_x.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      288 2023-05-30 03:21:18.000000 terminal-agent-x-0.1.2/terminal_agent_x.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-30 03:21:18.000000 terminal-agent-x-0.1.2/terminal_agent_x.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-05-30 03:21:18.000000 terminal-agent-x-0.1.2/terminal_agent_x.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-05-30 03:21:18.000000 terminal-agent-x-0.1.2/terminal_agent_x.egg-info/top_level.txt
```

### Comparing `terminal-agent-x-0.1.1/LICENSE` & `terminal-agent-x-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal-agent-x-0.1.1/PKG-INFO` & `terminal-agent-x-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: terminal-agent-x
-Version: 0.1.1
+Version: 0.1.2
 Summary: A terminal agent for terminal users.
 Author-email: LyuLumos <lyujiuyang0@gmail.com>
 Project-URL: Homepage, https://github.com/LyuLumos/Terminal-Agent-X
 Project-URL: Bug Tracker, https://github.com/LyuLumos/Terminal-Agent-X/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -52,15 +53,31 @@
 
 ```
 tax write a python code for fibonacci
 ```
 
 Use `tax -h` to get more information.
 ```bash
-usage: tax.py [-h] [--openai_key OPENAI_KEY] [--model MODEL] [--file FILE] [--url URL] [--show_all] prompt [prompt ...]
+usage: tax.py [-h] [--openai_key OPENAI_KEY] [--model MODEL] [--file FILE] [--url URL] [--default_url] [--claude] [--show_all] prompt [prompt ...]
+
+Description of your program
+
+positional arguments:
+  prompt                Prompt
+
+options:
+  -h, --help            show this help message and exit
+  --openai_key OPENAI_KEY
+                        Your key for OpenAI, only for one-time request
+  --model MODEL         Model name. You can use all OpenAI models.
+  --file FILE           Output file. If specified, the output will be written to this file. Tax will act like ChatGPT
+  --url URL             URL for API request which can be accessd under GFW. When your network environment is NOT under GFW, you can use OpenAI API directly.
+  --default_url         Use default OpenAI API URL for request.
+  --claude              Use Claude API for request.
+  --show_all            Show all contents in the response
 ```
 
 ## Support
 
 I have tested on Windows 10/11(cmd) and Ubuntu 22.04, it should work on other platforms.
 
 ## Attention
@@ -74,27 +91,22 @@
 ## License
 
 [GNU General Public License v3.0](LICENSE)
 
 ## Development Logs
 
 <details>
-<summary>Contents</summary>
-
-<details>
 <summary>0.1.0</summary>
 
 - Implement basic functions
 - Support for Windows cmd and Linux shell
 - Add `--file` option for saving the response to a file
 </details>
 
 <details>
 <summary>0.1.1</summary>
 
 - Add `--show_all` option for showing all contents of the response.
 - Add `--url` option for users not under GFW.
-- support for Windows Powershell
+- Add support for Windows Powershell
 </details>
 
-
-</details>
```

### Comparing `terminal-agent-x-0.1.1/pyproject.toml` & `terminal-agent-x-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal-agent-x"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="LyuLumos", email="lyujiuyang0@gmail.com" },
 ]
 description = "A terminal agent for terminal users."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
```

### Comparing `terminal-agent-x-0.1.1/terminal_agent_x/tax.py` & `terminal-agent-x-0.1.2/terminal_agent_x/tax.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import signal
+import subprocess
 import os
 import argparse
 import psutil
 import re
 import json
 
 
@@ -10,88 +12,118 @@
     parent_process_name = psutil.Process(os.getppid()).name()
     if parent_process_name in ['pwsh', 'powershell', 'powershell.exe']:
         return 'powershell'
     elif parent_process_name in ['cmd', 'cmd.exe']:
         return 'cmd'
 
 
-def fetch_code(openai_key, model, prompt):
-    command = "curl -s"
-    url = "https://api.lyulumos.space/v1/chat/completions"
+def run_command_with_timeout(command, timeout):
+    p = subprocess.Popen(command, stdout=subprocess.PIPE,
+                         stderr=subprocess.PIPE, shell=True)
+    try:
+        stdout, stderr = p.communicate(timeout=timeout)
+        return stdout.decode('utf-8', 'ignore'), stderr.decode('utf-8', 'ignore')
+    except subprocess.TimeoutExpired as timeout_e:
+        p.terminate()
+        if os.name == 'nt':
+            kill_process_tree(p.pid)
+        else:
+            os.killpg(os.getpgid(p.pid), signal.SIGTERM)
+        raise subprocess.TimeoutExpired(
+            p.args, timeout, output=stdout, stderr=stderr) from timeout_e
+
+
+def kill_process_tree(pid):
+    try:
+        parent = psutil.Process(pid)
+        children = parent.children(recursive=True)
+        for child in children:
+            child.kill()
+        parent.kill()
+    except psutil.NoSuchProcess:
+        pass
+
+
+def fetch_code(openai_key, model, prompt, args):
+    url = "https://api.lyulumos.space/v1/chat/completions" if not args.default_url else "https://api.openai.com/v1/chat/completions"
+    url = "https://claude-api.lyulumos.space/v1/chat/completions" if args.claude else url
     headers = [
         f"Authorization: Bearer {openai_key}",
         "Content-Type: application/json"
     ]
     terminal_headers = [
         f"Authorization='Bearer {openai_key}'",
         "'Content-Type'='application/json'"
     ]
     data = f'{{"model": "{model}","messages": [{{"role": "user", "content": "{prompt}"}}]}}'
 
     if os.name == 'nt':  # Windows
         if check_terminal() == 'powershell':
-            webrequest_pwsh = f'Invoke-WebRequest -Uri "{url}" -Method POST -Headers '
-            f'@{{{terminal_headers[0]};{terminal_headers[1]}}} -Body \'{data}\' -UseBasicParsing | '
-            'Select-Object -ExpandProperty Content | ConvertFrom-Json | Select-Object -ExpandProperty '
-            'choices | Select-Object -First 1 | Select-Object -ExpandProperty message | Select-Object '
-            '-ExpandProperty content'
-            print(webrequest_pwsh)
-
+            wt_command = f'Invoke-WebRequest -Uri "{url}" -Method POST -Headers @{{{terminal_headers[0]};{terminal_headers[1]}}} -Body \'{data}\' -UseBasicParsing | Select-Object -ExpandProperty Content | ConvertFrom-Json | Select-Object -ExpandProperty choices | Select-Object -First 1 | Select-Object -ExpandProperty message | Select-Object -ExpandProperty content'
+            print(
+                f'Current version does not fully support Windows PowerShell. Please copy command below and paste:\n\n{wt_command}')
+            return ''
         else:  # Windows cmd
             headers = [h.replace('"', '\\"') for h in headers]
             data = data.replace('"', '\\"')
-            command += f' "{url}" -H "{headers[0]}" -H "{headers[1]}" -d "{data}"'
+            command = f'curl -s "{url}" -H "{headers[0]}" -H "{headers[1]}" -d "{data}"'
     else:  # Linux
-        command += f" --location '{url}' --header '{headers[0]}' --header '{headers[1]}' --data '{data}'"
+        command = f"curl -s --location '{url}' --header '{headers[0]}' --header '{headers[1]}' --data '{data}'"
     # print(command)
 
     try:
-        res = json.loads(os.popen(command).read())[
-            'choices'][0]['message']['content']
+        res, err = run_command_with_timeout(command, 60)
+        # print(res, err)
+        # res = os.popen(command).read().encode('utf-8').decode('utf-8', 'ignore')
+        return json.loads(res)['choices'][0]['message']['content']
     except KeyError:
         assert False, 'This is most likely due to poor internet. Please retry.'
-    return str(res)
 
 
 def find_code(text):
     pattern = r"```(.*?)```"
     match = re.search(pattern, text, re.DOTALL)
     if match:
         return delete_prefix(match.group(0))  # with ``` pairs
     return None
 
 
 def delete_prefix(text):
     # text: ```python\nprint('Hello, world!')\n``` or ```\nprint('Hello, world!')\n```
-    s_new = re.sub(r'```[\w-]*\n', '```', text)
+    s_new = re.sub(r'```[\w-]*[+]*\n', '```', text)
     return s_new.strip('`').strip()
 
 
 def main():
     parser = argparse.ArgumentParser(description='Description of your program')
     parser.add_argument("prompt", nargs='+', type=str, help="Prompt")
     parser.add_argument('--openai_key', type=str,
                         help='Your key for OpenAI, only for one-time request')
     parser.add_argument('--model', type=str,
                         default='gpt-3.5-turbo', help='Model name. You can use all OpenAI models.')
     parser.add_argument(
         '--file', type=str, help='Output file. If specified, the output will be written to this file. Tax will act like ChatGPT')
     parser.add_argument('--url', type=str, default='https://api.lyulumos.space/v1/chat/completions',
-                        help='URL for API request. When your network environment is NOT under GFW, you can use OpenAI API directly.')
-    parser.add_argument('--show_all', action='store_true', help='Show all contents in the response')
+                        help='URL for API request which can be accessd under GFW. When your network environment is NOT under GFW, you can use OpenAI API directly.')
+    parser.add_argument('--default_url', action='store_true',
+                        help='Use default OpenAI API URL for request.')
+    parser.add_argument('--claude', action='store_true',
+                        help='Use Claude API for request.')
+    parser.add_argument('--show_all', action='store_true',
+                        help='Show all contents in the response')
     args = parser.parse_args()
 
     prompt = ' '.join(args.prompt)
     prompt = f'{prompt}. Answer me with markdown'
     openai_key = args.openai_key or os.environ.get('OpenAI_KEY')
     if not openai_key:
         assert False, 'Error: OpenAI key not found. Please specify it in system environment variables or pass it as an argument.'
 
     # res = get_model_response(openai_key, args.model, prompt)
-    res = fetch_code(openai_key, args.model, prompt)
+    res = fetch_code(openai_key, args.model, prompt, args)
 
     if args.file:
         with open(args.file, 'w', encoding='utf-8') as f:
             f.write(res)
         f.close()
     elif args.show_all:
         print(res)
```

### Comparing `terminal-agent-x-0.1.1/terminal_agent_x.egg-info/PKG-INFO` & `terminal-agent-x-0.1.2/terminal_agent_x.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: terminal-agent-x
-Version: 0.1.1
+Version: 0.1.2
 Summary: A terminal agent for terminal users.
 Author-email: LyuLumos <lyujiuyang0@gmail.com>
 Project-URL: Homepage, https://github.com/LyuLumos/Terminal-Agent-X
 Project-URL: Bug Tracker, https://github.com/LyuLumos/Terminal-Agent-X/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -52,15 +53,31 @@
 
 ```
 tax write a python code for fibonacci
 ```
 
 Use `tax -h` to get more information.
 ```bash
-usage: tax.py [-h] [--openai_key OPENAI_KEY] [--model MODEL] [--file FILE] [--url URL] [--show_all] prompt [prompt ...]
+usage: tax.py [-h] [--openai_key OPENAI_KEY] [--model MODEL] [--file FILE] [--url URL] [--default_url] [--claude] [--show_all] prompt [prompt ...]
+
+Description of your program
+
+positional arguments:
+  prompt                Prompt
+
+options:
+  -h, --help            show this help message and exit
+  --openai_key OPENAI_KEY
+                        Your key for OpenAI, only for one-time request
+  --model MODEL         Model name. You can use all OpenAI models.
+  --file FILE           Output file. If specified, the output will be written to this file. Tax will act like ChatGPT
+  --url URL             URL for API request which can be accessd under GFW. When your network environment is NOT under GFW, you can use OpenAI API directly.
+  --default_url         Use default OpenAI API URL for request.
+  --claude              Use Claude API for request.
+  --show_all            Show all contents in the response
 ```
 
 ## Support
 
 I have tested on Windows 10/11(cmd) and Ubuntu 22.04, it should work on other platforms.
 
 ## Attention
@@ -74,27 +91,22 @@
 ## License
 
 [GNU General Public License v3.0](LICENSE)
 
 ## Development Logs
 
 <details>
-<summary>Contents</summary>
-
-<details>
 <summary>0.1.0</summary>
 
 - Implement basic functions
 - Support for Windows cmd and Linux shell
 - Add `--file` option for saving the response to a file
 </details>
 
 <details>
 <summary>0.1.1</summary>
 
 - Add `--show_all` option for showing all contents of the response.
 - Add `--url` option for users not under GFW.
-- support for Windows Powershell
+- Add support for Windows Powershell
 </details>
 
-
-</details>
```

