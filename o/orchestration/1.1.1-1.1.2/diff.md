# Comparing `tmp/orchestration-1.1.1.tar.gz` & `tmp/orchestration-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orchestration-1.1.1.tar", last modified: Thu May 25 19:50:34 2023, max compression
+gzip compressed data, was "dist/orchestration-1.1.2.tar", last modified: Tue May 30 16:50:31 2023, max compression
```

## Comparing `orchestration-1.1.1.tar` & `orchestration-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:50:34.000000 orchestration-1.1.1/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     4426 2023-05-25 19:50:34.000000 orchestration-1.1.1/PKG-INFO
--rw-r--r--   0 henrytazewell   (501) staff       (20)     3303 2023-05-25 19:47:12.000000 orchestration-1.1.1/README.md
--rw-r--r--   0 henrytazewell   (501) staff       (20)      653 2023-05-25 19:50:21.000000 orchestration-1.1.1/setup.py
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration.egg-info/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     4426 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration.egg-info/PKG-INFO
--rw-r--r--   0 henrytazewell   (501) staff       (20)      280 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration.egg-info/SOURCES.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration.egg-info/requires.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration.egg-info/top_level.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)        1 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration.egg-info/dependency_links.txt
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-25 19:50:34.000000 orchestration-1.1.1/orchestration/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     3082 2023-05-25 19:40:08.000000 orchestration-1.1.1/orchestration/task.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)       51 2023-05-25 19:23:22.000000 orchestration-1.1.1/orchestration/__init__.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)     1138 2023-05-25 19:46:26.000000 orchestration-1.1.1/orchestration/orchestrator.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)       38 2023-05-25 19:50:34.000000 orchestration-1.1.1/setup.cfg
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-30 16:50:31.000000 orchestration-1.1.2/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     4426 2023-05-30 16:50:31.000000 orchestration-1.1.2/PKG-INFO
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     3303 2023-05-25 19:47:12.000000 orchestration-1.1.2/README.md
+-rw-r--r--   0 henrytazewell   (501) staff       (20)      653 2023-05-26 14:17:52.000000 orchestration-1.1.2/setup.py
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration.egg-info/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     4426 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration.egg-info/PKG-INFO
+-rw-r--r--   0 henrytazewell   (501) staff       (20)      280 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration.egg-info/SOURCES.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration.egg-info/requires.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration.egg-info/top_level.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)        1 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration.egg-info/dependency_links.txt
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     3081 2023-05-26 15:06:37.000000 orchestration-1.1.2/orchestration/task.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       51 2023-05-26 14:18:32.000000 orchestration-1.1.2/orchestration/__init__.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)      977 2023-05-30 16:49:16.000000 orchestration-1.1.2/orchestration/orchestrator.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       38 2023-05-30 16:50:31.000000 orchestration-1.1.2/setup.cfg
```

### Comparing `orchestration-1.1.1/PKG-INFO` & `orchestration-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestration
-Version: 1.1.1
+Version: 1.1.2
 Summary: This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.
 Home-page: https://github.com/htazewell/orchestration
 Author: Henry Tazewell
 Author-email: htazewell@gmail.com
 License: UNKNOWN
 Description: # Orchestration
```

### Comparing `orchestration-1.1.1/README.md` & `orchestration-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `orchestration-1.1.1/setup.py` & `orchestration-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='orchestration',
-    version='1.1.1',
+    version='1.1.2',
     description='This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Henry Tazewell',
     author_email='htazewell@gmail.com',
     url='https://github.com/htazewell/orchestration',
     packages=find_packages(),
```

### Comparing `orchestration-1.1.1/orchestration.egg-info/PKG-INFO` & `orchestration-1.1.2/orchestration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestration
-Version: 1.1.1
+Version: 1.1.2
 Summary: This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.
 Home-page: https://github.com/htazewell/orchestration
 Author: Henry Tazewell
 Author-email: htazewell@gmail.com
 License: UNKNOWN
 Description: # Orchestration
```

### Comparing `orchestration-1.1.1/orchestration/task.py` & `orchestration-1.1.2/orchestration/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
             if self.script_type == 'bash':
                 process = subprocess.Popen(['bash', script_path] + script_args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
             elif self.script_type == 'python':
                 process = subprocess.Popen(['python', script_path] + script_args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
             else:
                 logging.error(f"Unsupported script type: {self.script_type}")
                 return
-
             stdout, stderr = process.communicate(timeout=60)
 
             if process.returncode != 0:
                 logging.error(f"Error executing script: {script_path}")
                 logging.error(stderr)
             else:
                 logging.info(f"Script output: {stdout}")
```

### Comparing `orchestration-1.1.1/orchestration/orchestrator.py` & `orchestration-1.1.2/orchestration/orchestrator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import logging
 import time
+import datetime
 from orchestration.task import Task
 
 
 class Orchestrator:
     def __init__(self):
         self.tasks = []
 
     def add_task(self, cron_expression, script_type):
         task = Task(cron_expression, script_type)
         self.tasks.append(task)
         return task
 
     def execute_tasks(self):
-        while True:
-            for task in self.tasks:
-                # Check if the task should be skipped
-                if any(skip_condition for skip_condition in task.skips):
-                    logging.info(f"Skipping task execution due to skip conditions: {task.cron_expression}")
-                    continue
-
-                if task.should_execute():
-                    for script in task.scripts:
-                        if isinstance(script, tuple) and len(script) == 2:
-                            script_path, parameters_list = script
-                            task.repeat(script_path, parameters_list)
-                        else:
-                            task.execute_script(script)
-                        time.sleep(task.interval)
-
-            time.sleep(task.interval)  # Sleep for 1 second
+        for task in self.tasks:
+            # Check if the task should be skipped
+            if any(skip_condition for skip_condition in task.skips):
+                logging.info(f"Skipping task execution...")
+                continue
+
+            if task.should_execute():
+                for script in task.scripts:
+                    if isinstance(script, tuple) and len(script) == 2:
+                        script_path, parameters_list = script
+                        task.repeat(script_path, parameters_list)
+                    else:
+                        task.execute_script(script)
+                    time.sleep(task.interval)
```

