# Comparing `tmp/orchestration-1.1.2.tar.gz` & `tmp/orchestration-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orchestration-1.1.2.tar", last modified: Tue May 30 16:50:31 2023, max compression
+gzip compressed data, was "dist/orchestration-1.1.3.tar", last modified: Tue May 30 16:55:40 2023, max compression
```

## Comparing `orchestration-1.1.2.tar` & `orchestration-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-30 16:50:31.000000 orchestration-1.1.2/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     4426 2023-05-30 16:50:31.000000 orchestration-1.1.2/PKG-INFO
--rw-r--r--   0 henrytazewell   (501) staff       (20)     3303 2023-05-25 19:47:12.000000 orchestration-1.1.2/README.md
--rw-r--r--   0 henrytazewell   (501) staff       (20)      653 2023-05-26 14:17:52.000000 orchestration-1.1.2/setup.py
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration.egg-info/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     4426 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration.egg-info/PKG-INFO
--rw-r--r--   0 henrytazewell   (501) staff       (20)      280 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration.egg-info/SOURCES.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration.egg-info/requires.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration.egg-info/top_level.txt
--rw-r--r--   0 henrytazewell   (501) staff       (20)        1 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration.egg-info/dependency_links.txt
-drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-30 16:50:31.000000 orchestration-1.1.2/orchestration/
--rw-r--r--   0 henrytazewell   (501) staff       (20)     3081 2023-05-26 15:06:37.000000 orchestration-1.1.2/orchestration/task.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)       51 2023-05-26 14:18:32.000000 orchestration-1.1.2/orchestration/__init__.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)      977 2023-05-30 16:49:16.000000 orchestration-1.1.2/orchestration/orchestrator.py
--rw-r--r--   0 henrytazewell   (501) staff       (20)       38 2023-05-30 16:50:31.000000 orchestration-1.1.2/setup.cfg
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-30 16:55:40.000000 orchestration-1.1.3/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     4426 2023-05-30 16:55:40.000000 orchestration-1.1.3/PKG-INFO
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     3303 2023-05-25 19:47:12.000000 orchestration-1.1.3/README.md
+-rw-r--r--   0 henrytazewell   (501) staff       (20)      653 2023-05-30 16:55:38.000000 orchestration-1.1.3/setup.py
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-30 16:55:40.000000 orchestration-1.1.3/orchestration.egg-info/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     4426 2023-05-30 16:55:40.000000 orchestration-1.1.3/orchestration.egg-info/PKG-INFO
+-rw-r--r--   0 henrytazewell   (501) staff       (20)      280 2023-05-30 16:55:40.000000 orchestration-1.1.3/orchestration.egg-info/SOURCES.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-30 16:55:40.000000 orchestration-1.1.3/orchestration.egg-info/requires.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       14 2023-05-30 16:55:40.000000 orchestration-1.1.3/orchestration.egg-info/top_level.txt
+-rw-r--r--   0 henrytazewell   (501) staff       (20)        1 2023-05-30 16:55:40.000000 orchestration-1.1.3/orchestration.egg-info/dependency_links.txt
+drwxr-xr-x   0 henrytazewell   (501) staff       (20)        0 2023-05-30 16:55:40.000000 orchestration-1.1.3/orchestration/
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     3081 2023-05-26 15:06:37.000000 orchestration-1.1.3/orchestration/task.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       51 2023-05-26 14:18:32.000000 orchestration-1.1.3/orchestration/__init__.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)     1063 2023-05-30 16:54:57.000000 orchestration-1.1.3/orchestration/orchestrator.py
+-rw-r--r--   0 henrytazewell   (501) staff       (20)       38 2023-05-30 16:55:40.000000 orchestration-1.1.3/setup.cfg
```

### Comparing `orchestration-1.1.2/PKG-INFO` & `orchestration-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestration
-Version: 1.1.2
+Version: 1.1.3
 Summary: This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.
 Home-page: https://github.com/htazewell/orchestration
 Author: Henry Tazewell
 Author-email: htazewell@gmail.com
 License: UNKNOWN
 Description: # Orchestration
```

### Comparing `orchestration-1.1.2/README.md` & `orchestration-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `orchestration-1.1.2/setup.py` & `orchestration-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='orchestration',
-    version='1.1.2',
+    version='1.1.3',
     description='This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Henry Tazewell',
     author_email='htazewell@gmail.com',
     url='https://github.com/htazewell/orchestration',
     packages=find_packages(),
```

### Comparing `orchestration-1.1.2/orchestration.egg-info/PKG-INFO` & `orchestration-1.1.3/orchestration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestration
-Version: 1.1.2
+Version: 1.1.3
 Summary: This Python script provides functionality to schedule and execute scripts based on cron expressions. It allows executing both bash and Python scripts and provides options to add script parameters and skip conditions.
 Home-page: https://github.com/htazewell/orchestration
 Author: Henry Tazewell
 Author-email: htazewell@gmail.com
 License: UNKNOWN
 Description: # Orchestration
```

### Comparing `orchestration-1.1.2/orchestration/task.py` & `orchestration-1.1.3/orchestration/task.py`

 * *Files identical despite different names*

### Comparing `orchestration-1.1.2/orchestration/orchestrator.py` & `orchestration-1.1.3/orchestration/orchestrator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import time
-import datetime
 from orchestration.task import Task
 
 
 class Orchestrator:
     def __init__(self):
         self.tasks = []
 
@@ -14,17 +13,20 @@
         return task
 
     def execute_tasks(self):
         for task in self.tasks:
             # Check if the task should be skipped
             if any(skip_condition for skip_condition in task.skips):
                 logging.info(f"Skipping task execution...")
+                time.sleep(task.interval)
                 continue
 
             if task.should_execute():
                 for script in task.scripts:
                     if isinstance(script, tuple) and len(script) == 2:
                         script_path, parameters_list = script
                         task.repeat(script_path, parameters_list)
                     else:
                         task.execute_script(script)
-                    time.sleep(task.interval)
+                    time.sleep(task.interval)
+            else:
+                time.sleep(task.interval)
```

