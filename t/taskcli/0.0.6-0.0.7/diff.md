# Comparing `tmp/taskcli-0.0.6.tar.gz` & `tmp/taskcli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcli-0.0.6.tar", last modified: Mon May 29 15:06:47 2023, max compression
+gzip compressed data, was "taskcli-0.0.7.tar", last modified: Tue May 30 17:09:07 2023, max compression
```

## Comparing `taskcli-0.0.6.tar` & `taskcli-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:06:47.801714 taskcli-0.0.6/
--rw-r--r--   0 p          (501) staff       (20)     1062 2022-11-19 23:50:29.000000 taskcli-0.0.6/LICENSE
--rw-r--r--   0 p          (501) staff       (20)      219 2023-05-29 15:06:47.801781 taskcli-0.0.6/PKG-INFO
--rw-r--r--   0 p          (501) staff       (20)     1781 2023-05-29 14:52:00.000000 taskcli-0.0.6/README.md
--rw-r--r--   0 p          (501) staff       (20)       86 2022-11-19 23:50:29.000000 taskcli-0.0.6/pyproject.toml
--rw-r--r--   0 p          (501) staff       (20)      405 2023-05-29 15:06:47.802058 taskcli-0.0.6/setup.cfg
-drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:06:47.798726 taskcli-0.0.6/src/
-drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:06:47.800525 taskcli-0.0.6/src/taskcli/
--rw-r--r--   0 p          (501) staff       (20)      144 2023-05-29 14:27:39.000000 taskcli-0.0.6/src/taskcli/__init__.py
--rw-r--r--   0 p          (501) staff       (20)     8253 2023-05-29 14:25:30.000000 taskcli-0.0.6/src/taskcli/old.py
--rw-r--r--   0 p          (501) staff       (20)    18634 2023-05-29 15:06:23.000000 taskcli-0.0.6/src/taskcli/taskcli.py
-drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:06:47.801613 taskcli-0.0.6/src/taskcli.egg-info/
--rw-r--r--   0 p          (501) staff       (20)      219 2023-05-29 15:06:47.000000 taskcli-0.0.6/src/taskcli.egg-info/PKG-INFO
--rw-r--r--   0 p          (501) staff       (20)      248 2023-05-29 15:06:47.000000 taskcli-0.0.6/src/taskcli.egg-info/SOURCES.txt
--rw-r--r--   0 p          (501) staff       (20)        1 2023-05-29 15:06:47.000000 taskcli-0.0.6/src/taskcli.egg-info/dependency_links.txt
--rw-r--r--   0 p          (501) staff       (20)        8 2023-05-29 15:06:47.000000 taskcli-0.0.6/src/taskcli.egg-info/top_level.txt
+drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-30 17:09:07.992735 taskcli-0.0.7/
+-rw-r--r--   0 p          (501) staff       (20)     1062 2022-11-19 23:50:29.000000 taskcli-0.0.7/LICENSE
+-rw-r--r--   0 p          (501) staff       (20)      219 2023-05-30 17:09:07.992812 taskcli-0.0.7/PKG-INFO
+-rw-r--r--   0 p          (501) staff       (20)     1781 2023-05-29 14:52:00.000000 taskcli-0.0.7/README.md
+-rw-r--r--   0 p          (501) staff       (20)       86 2022-11-19 23:50:29.000000 taskcli-0.0.7/pyproject.toml
+-rw-r--r--   0 p          (501) staff       (20)      405 2023-05-30 17:09:07.993114 taskcli-0.0.7/setup.cfg
+drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-30 17:09:07.990115 taskcli-0.0.7/src/
+drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-30 17:09:07.991900 taskcli-0.0.7/src/taskcli/
+-rw-r--r--   0 p          (501) staff       (20)      144 2023-05-29 14:27:39.000000 taskcli-0.0.7/src/taskcli/__init__.py
+-rw-r--r--   0 p          (501) staff       (20)     8253 2023-05-29 14:25:30.000000 taskcli-0.0.7/src/taskcli/old.py
+-rw-r--r--   0 p          (501) staff       (20)    18635 2023-05-30 17:07:54.000000 taskcli-0.0.7/src/taskcli/taskcli.py
+drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-30 17:09:07.992620 taskcli-0.0.7/src/taskcli.egg-info/
+-rw-r--r--   0 p          (501) staff       (20)      219 2023-05-30 17:09:07.000000 taskcli-0.0.7/src/taskcli.egg-info/PKG-INFO
+-rw-r--r--   0 p          (501) staff       (20)      248 2023-05-30 17:09:07.000000 taskcli-0.0.7/src/taskcli.egg-info/SOURCES.txt
+-rw-r--r--   0 p          (501) staff       (20)        1 2023-05-30 17:09:07.000000 taskcli-0.0.7/src/taskcli.egg-info/dependency_links.txt
+-rw-r--r--   0 p          (501) staff       (20)        8 2023-05-30 17:09:07.000000 taskcli-0.0.7/src/taskcli.egg-info/top_level.txt
```

### Comparing `taskcli-0.0.6/LICENSE` & `taskcli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcli-0.0.6/README.md` & `taskcli-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `taskcli-0.0.6/src/taskcli/old.py` & `taskcli-0.0.7/src/taskcli/old.py`

 * *Files identical despite different names*

### Comparing `taskcli-0.0.6/src/taskcli/taskcli.py` & `taskcli-0.0.7/src/taskcli/taskcli.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,14 @@
 
 #     def processing_arg(self, func_name):
 #         self.current_task = func_name
 #         if self.previous_task != self.current_task:
 #             for k,v in task_data.items():
 
 
-
 def arg(
     *names,
     type=None,
     default=EMPTY,
     choices=None,
     required=EMPTY,
     help="",
@@ -494,16 +493,16 @@
         argv = sys.argv
 
     # Detect if we're running as a script or not
     frame = inspect.currentframe()
     assert frame is not None
     module = inspect.getmodule(frame.f_back)
     assert module is not None
-    if (module.__name__ != "__main__") and not force:
-        return
+    # if (module.__name__ != "__main__") and not force:
+    #     return
 
     ns = Namespace(tasks)
     if ns.has_default_task():
         dt = ns.get_default_task()
         if dt.has_positional_args() and len(ns.tasks) > 1:
             raise Exception(
                 f"The default task {dt.name} has positional arguments as they can be confused with \
@@ -541,21 +540,19 @@
                 raise Exception("No tasks were defined. Use @task decorator to define tasks.")
             elif len(tasks) == 1 and not explicit_default_task:
                 task_name = list(tasks.keys())[0]
             else:
                 raise Exception("No task name provided, and there's no default task defined.")
     else:
         if argv[1].startswith("-") and ns.has_default_task():
-
             assert len(argv) >= 2
             task_name = ns.get_default_task().name
         elif argv[1].startswith("-") and not ns.get_default_task():
             raise Exception("No task name provided, and there's no default task defined.")
         else:
-
             assert len(argv) >= 2
             task_name = argv[1].replace("-", "_")
             argv = [argv[0]] + argv[2:]  # remove task name from argv
 
     argv = argv[1:]
     assert isinstance(task_name, str), f"task name must be a string, got {type(task_name)}, {task_name}"
     parser = build_parser_for_task(task_name)
```

