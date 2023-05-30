# Comparing `tmp/playmolecule-1.8.3.tar.gz` & `tmp/playmolecule-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.8.3.tar", last modified: Fri May 26 09:55:41 2023, max compression
+gzip compressed data, was "playmolecule-1.8.4.tar", last modified: Tue May 30 13:06:54 2023, max compression
```

## Comparing `playmolecule-1.8.3.tar` & `playmolecule-1.8.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:55:41.419762 playmolecule-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-26 09:55:19.000000 playmolecule-1.8.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 09:55:19.000000 playmolecule-1.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-26 09:55:41.419762 playmolecule-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 09:55:19.000000 playmolecule-1.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:55:41.419762 playmolecule-1.8.3/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-26 09:55:41.419762 playmolecule-1.8.3/playmolecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32601 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:55:41.419762 playmolecule-1.8.3/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-26 09:55:41.000000 playmolecule-1.8.3/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-26 09:55:41.000000 playmolecule-1.8.3/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:55:41.000000 playmolecule-1.8.3/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:55:41.000000 playmolecule-1.8.3/playmolecule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 09:55:41.000000 playmolecule-1.8.3/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 09:55:41.000000 playmolecule-1.8.3/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-26 09:55:19.000000 playmolecule-1.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 09:55:41.419762 playmolecule-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 09:55:19.000000 playmolecule-1.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:55:41.419762 playmolecule-1.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 09:55:19.000000 playmolecule-1.8.3/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-26 09:55:19.000000 playmolecule-1.8.3/tests/test_app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-26 09:55:19.000000 playmolecule-1.8.3/tests/test_datacenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:06:54.148855 playmolecule-1.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-30 13:06:29.000000 playmolecule-1.8.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 13:06:29.000000 playmolecule-1.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-30 13:06:54.144854 playmolecule-1.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-30 13:06:29.000000 playmolecule-1.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:06:54.148855 playmolecule-1.8.4/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-30 13:06:29.000000 playmolecule-1.8.4/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-30 13:06:29.000000 playmolecule-1.8.4/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 13:06:54.148855 playmolecule-1.8.4/playmolecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-30 13:06:29.000000 playmolecule-1.8.4/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-30 13:06:29.000000 playmolecule-1.8.4/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-30 13:06:29.000000 playmolecule-1.8.4/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33358 2023-05-30 13:06:29.000000 playmolecule-1.8.4/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-30 13:06:29.000000 playmolecule-1.8.4/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-30 13:06:29.000000 playmolecule-1.8.4/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-30 13:06:29.000000 playmolecule-1.8.4/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-30 13:06:29.000000 playmolecule-1.8.4/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-30 13:06:29.000000 playmolecule-1.8.4/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-30 13:06:29.000000 playmolecule-1.8.4/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-30 13:06:29.000000 playmolecule-1.8.4/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:06:54.144854 playmolecule-1.8.4/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-30 13:06:54.000000 playmolecule-1.8.4/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 13:06:54.000000 playmolecule-1.8.4/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:06:54.000000 playmolecule-1.8.4/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:06:53.000000 playmolecule-1.8.4/playmolecule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 13:06:54.000000 playmolecule-1.8.4/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 13:06:54.000000 playmolecule-1.8.4/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-30 13:06:29.000000 playmolecule-1.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:06:54.148855 playmolecule-1.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 13:06:29.000000 playmolecule-1.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:06:54.144854 playmolecule-1.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-30 13:06:29.000000 playmolecule-1.8.4/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-30 13:06:29.000000 playmolecule-1.8.4/tests/test_app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-30 13:06:29.000000 playmolecule-1.8.4/tests/test_datacenter.py
```

### Comparing `playmolecule-1.8.3/LICENSE.md` & `playmolecule-1.8.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/PKG-INFO` & `playmolecule-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.8.3
+Version: 1.8.4
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.8.3/playmolecule/__init__.py` & `playmolecule-1.8.4/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/playmolecule/_test_funcs.py` & `playmolecule-1.8.4/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/playmolecule/config.py` & `playmolecule-1.8.4/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/playmolecule/datacenter.py` & `playmolecule-1.8.4/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/playmolecule/devutils.py` & `playmolecule-1.8.4/playmolecule/devutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -518,34 +518,44 @@
         if len(newvals) == 1:
             newvals = newvals[0]
         input_args[name] = newvals
 
     return input_args
 
 
+def report_alive(outdir):
+    from datetime import datetime
+
+    while True:
+        current_date = datetime.now()
+        with open(os.path.join(outdir, ".pm.alive"), "w") as f:
+            f.write(current_date.isoformat())
+
+
 def app_wrapper2(
     func,
     cli_arg_str=None,
     token=None,
     execid=None,
     dump_argparser=None,
     dump_manifest=None,
     input_json=None,
 ):
     from contextlib import redirect_stdout, redirect_stderr
-    from func2argparse import func_to_argparser
+    from func2argparse import func_to_argparser, write_argparser_json
     import importlib
     import datetime
     import shutil
     from unittest import mock
     import json
     import yaml
     import traceback
     import logging
     from shlex import split
+    import threading
 
     # Import the module/function of the app to call
     pieces = func.split(".")
     top_module = pieces[0]
     module_name = ".".join(pieces[:-1])
     module = importlib.import_module(module_name)
     func = getattr(module, pieces[-1])
@@ -588,15 +598,27 @@
                 params[arg] = str(value)
             if isinstance(value, list) or isinstance(value, tuple):
                 params[arg] = [str(x) if isinstance(x, Path) else x for x in value]
 
         os.makedirs(params["outdir"], exist_ok=True)
         if "scratchdir" in params and params["scratchdir"] is not None:
             os.makedirs(params["scratchdir"], exist_ok=True)
-        func(**params)
+
+        thread = threading.Thread(target=report_alive, args=(params["outdir"],), daemon=True)
+        thread.start()
+
+        try:
+            func(**params)
+        except Exception as e:
+            with open(os.path.join(outdir,".pm.err"), "w") as f:
+                f.write("")
+            raise e
+        else:
+            with open(os.path.join(outdir,".pm.done"), "w") as f:
+                f.write("")
         return
 
     try:
         SESSION, JOB, EXECID = _get_session(token, execid)
         indir = "/data/in"
         os.makedirs(indir, exist_ok=True)
 
@@ -628,14 +650,16 @@
         _handle_error(
             f"Failed at initializing wrapper with error:\n{traceback.format_exc()}",
             JOB,
             None,
         )
         return
 
+    thread = threading.Thread(target=report_alive, args=(outdir,), daemon=True)
+    thread.start()
     try:
         # Download app inputs and input arguments from backend
         JOB._download("input", indir)
         JOB._download("output", outdir)
 
         sessionargs = {}
         sig = inspect.signature(func)
```

### Comparing `playmolecule-1.8.3/playmolecule/job.py` & `playmolecule-1.8.4/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/playmolecule/jsonlogger.py` & `playmolecule-1.8.4/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/playmolecule/local.py` & `playmolecule-1.8.4/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/playmolecule/playqueue.py` & `playmolecule-1.8.4/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/playmolecule/session.py` & `playmolecule-1.8.4/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/playmolecule/utils.py` & `playmolecule-1.8.4/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.8.4/playmolecule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.8.3
+Version: 1.8.4
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.8.3/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.8.4/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/pyproject.toml` & `playmolecule-1.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/tests/test.py` & `playmolecule-1.8.4/tests/test.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/tests/test_app_wrapper.py` & `playmolecule-1.8.4/tests/test_app_wrapper.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.3/tests/test_datacenter.py` & `playmolecule-1.8.4/tests/test_datacenter.py`

 * *Files identical despite different names*

