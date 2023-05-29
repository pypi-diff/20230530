# Comparing `tmp/vscode_task_runner-0.1.3.tar.gz` & `tmp/vscode_task_runner-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vscode_task_runner-0.1.3.tar", max compression
+gzip compressed data, was "vscode_task_runner-0.1.4.tar", max compression
```

## Comparing `vscode_task_runner-0.1.3.tar` & `vscode_task_runner-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-05-29 18:39:14.578192 vscode_task_runner-0.1.3/LICENSE
--rw-r--r--   0        0        0     7591 2023-05-29 18:39:14.578192 vscode_task_runner-0.1.3/README.md
--rw-r--r--   0        0        0     1273 2023-05-29 18:39:14.578192 vscode_task_runner-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/__init__.py
--rw-r--r--   0        0        0       39 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/__main__.py
--rw-r--r--   0        0        0     2745 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/console.py
--rw-r--r--   0        0        0     1551 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/constants.py
--rw-r--r--   0        0        0     1193 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/executor.py
--rw-r--r--   0        0        0     3740 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/helpers.py
--rw-r--r--   0        0        0     1835 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/json_parser.py
--rw-r--r--   0        0        0     1464 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/models.py
--rw-r--r--   0        0        0     9296 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/task.py
--rw-r--r--   0        0        0     7497 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/terminal_task_system.py
--rw-r--r--   0        0        0     8561 1970-01-01 00:00:00.000000 vscode_task_runner-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/LICENSE
+-rw-r--r--   0        0        0     7680 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/README.md
+-rw-r--r--   0        0        0     1332 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/__main__.py
+-rw-r--r--   0        0        0     2756 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/console.py
+-rw-r--r--   0        0        0     1551 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/constants.py
+-rw-r--r--   0        0        0     1193 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/executor.py
+-rw-r--r--   0        0        0     3740 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/helpers.py
+-rw-r--r--   0        0        0     1835 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/json_parser.py
+-rw-r--r--   0        0        0     1464 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/models.py
+-rw-r--r--   0        0        0     9296 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/task.py
+-rw-r--r--   0        0        0     7497 2023-05-29 22:52:17.610664 vscode_task_runner-0.1.4/vtr/terminal_task_system.py
+-rw-r--r--   0        0        0     8651 1970-01-01 00:00:00.000000 vscode_task_runner-0.1.4/PKG-INFO
```

### Comparing `vscode_task_runner-0.1.3/LICENSE` & `vscode_task_runner-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.3/README.md` & `vscode_task_runner-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 
 ```bash
 pip install vscode-task-runner
 ```
 
 Use the command `vtr` on the command line and provide the label of the task(s).
 There must be a `.vscode/tasks.json` file in the working directory you run the
-command in.
+command in. (You can also use the `vscode-task-runner` command instead
+if it makes you feel better).
 
 ## Examples
 
 ```json
 {
   "version": "2.0.0",
   "tasks": [
@@ -134,15 +135,15 @@
 ```
 
 You can also use it as a [pre-commit](https://pre-commit.com) hook if desired:
 
 ```yaml
 repos:
   - repo: https://github.com/NathanVaughn/vscode-task-runner
-    rev: v0.1.2
+    rev: v0.1.3
     hooks:
       - id: vtr
         # Optionally override the hook name here
         # name: Build & Test
         args:
           - build # put the tasks you want to run here
           - test
```

### Comparing `vscode_task_runner-0.1.3/pyproject.toml` & `vscode_task_runner-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
     name = "vscode-task-runner"
-    version = "0.1.3"
-    description = "Task runner for VSCode tasks.json"
+    version = "0.1.4"
+    description = "Task runner for VS Code tasks.json"
     license = "MIT"
     readme = "README.md"
     homepage = "https://github.com/NathanVaughn/vscode-task-runner"
     repository = "https://github.com/NathanVaughn/vscode-task-runner.git"
     authors = ["Nathan Vaughn <nvaughn51@gmail.com>"]
     classifiers = [
         "Intended Audience :: Developers",
@@ -26,15 +26,16 @@
 [tool.poetry.group.dev.dependencies]
     pre-commit  = "^3.2.0"
     pytest      = "^7.3.1"
     pytest-mock = "^3.10.0"
     pytest-cov  = "^4.1.0"
 
 [tool.poetry.scripts]
-    vtr = "vtr.console:run"
+    vtr                = "vtr.console:run"
+    vscode-task-runner = "vtr.console:run"
 
 [tool.pyright]
     typeCheckingMode = "basic"
     venvPath         = "."
     venv             = ".venv"
 
 [tool.ruff]
```

### Comparing `vscode_task_runner-0.1.3/vtr/console.py` & `vscode_task_runner-0.1.4/vtr/console.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # parse the tasks.json
     try:
         all_tasks_data, tasks_json = vtr.json_parser.load_vscode_tasks_data()
         # build task objects
         all_tasks: dict[str, Task] = {
             t["label"]: Task(all_tasks_data, t["label"])
             for t in all_tasks_data["tasks"]
-            if t.get("type") in ["process", "shell"]
+            if t.get("type", "process") in ["process", "shell"]
         }
     except FileNotFoundError:
         all_tasks = {}
         task_label_help_text += (
             " Invoke this command inside a directory with a"
             + f" {os.path.join('.vscode', 'tasks.json')} file to see and run tasks."
         )
```

### Comparing `vscode_task_runner-0.1.3/vtr/constants.py` & `vscode_task_runner-0.1.4/vtr/constants.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.3/vtr/executor.py` & `vscode_task_runner-0.1.4/vtr/executor.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.3/vtr/helpers.py` & `vscode_task_runner-0.1.4/vtr/helpers.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.3/vtr/json_parser.py` & `vscode_task_runner-0.1.4/vtr/json_parser.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.3/vtr/models.py` & `vscode_task_runner-0.1.4/vtr/models.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.3/vtr/task.py` & `vscode_task_runner-0.1.4/vtr/task.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.3/vtr/terminal_task_system.py` & `vscode_task_runner-0.1.4/vtr/terminal_task_system.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.3/PKG-INFO` & `vscode_task_runner-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vscode-task-runner
-Version: 0.1.3
-Summary: Task runner for VSCode tasks.json
+Version: 0.1.4
+Summary: Task runner for VS Code tasks.json
 Home-page: https://github.com/NathanVaughn/vscode-task-runner
 License: MIT
 Author: Nathan Vaughn
 Author-email: nvaughn51@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -52,15 +52,16 @@
 
 ```bash
 pip install vscode-task-runner
 ```
 
 Use the command `vtr` on the command line and provide the label of the task(s).
 There must be a `.vscode/tasks.json` file in the working directory you run the
-command in.
+command in. (You can also use the `vscode-task-runner` command instead
+if it makes you feel better).
 
 ## Examples
 
 ```json
 {
   "version": "2.0.0",
   "tasks": [
@@ -157,15 +158,15 @@
 ```
 
 You can also use it as a [pre-commit](https://pre-commit.com) hook if desired:
 
 ```yaml
 repos:
   - repo: https://github.com/NathanVaughn/vscode-task-runner
-    rev: v0.1.2
+    rev: v0.1.3
     hooks:
       - id: vtr
         # Optionally override the hook name here
         # name: Build & Test
         args:
           - build # put the tasks you want to run here
           - test
```

