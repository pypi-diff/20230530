# Comparing `tmp/optscale_arcee-0.1.30.tar.gz` & `tmp/optscale_arcee-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optscale_arcee-0.1.30.tar", last modified: Thu Apr 13 11:07:46 2023, max compression
+gzip compressed data, was "optscale_arcee-0.1.34.tar", last modified: Tue May 30 12:07:27 2023, max compression
```

## Comparing `optscale_arcee-0.1.30.tar` & `optscale_arcee-0.1.34.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/
--rw-rw-r--   0 am        (1000) am        (1000)    11304 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/LICENSE.txt
--rw-rw-r--   0 am        (1000) am        (1000)     2241 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/PKG-INFO
--rw-rw-r--   0 am        (1000) am        (1000)     1423 2023-04-07 12:57:57.000000 optscale_arcee-0.1.30/README.rst
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.407026 optscale_arcee-0.1.30/optscale_arcee/
--rw-rw-r--   0 am        (1000) am        (1000)       95 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)     3751 2023-04-07 12:57:57.000000 optscale_arcee-0.1.30/optscale_arcee/arcee.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/optscale_arcee/hw_stat_collector/
--rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/hw_stat_collector/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)     4098 2023-04-07 12:57:57.000000 optscale_arcee-0.1.30/optscale_arcee/hw_stat_collector/collector.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/optscale_arcee/module_collector/
--rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/module_collector/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)     2633 2023-04-07 12:57:57.000000 optscale_arcee-0.1.30/optscale_arcee/module_collector/collector.py
--rw-rw-r--   0 am        (1000) am        (1000)     6757 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/name_generator.py
--rw-rw-r--   0 am        (1000) am        (1000)     9821 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/platform.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/optscale_arcee/platforms_meta/
--rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/platforms_meta/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)     2469 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/platforms_meta/azure.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/optscale_arcee/sender/
--rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/optscale_arcee/sender/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)     4064 2023-04-07 12:57:57.000000 optscale_arcee-0.1.30/optscale_arcee/sender/sender.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/optscale_arcee.egg-info/
--rw-rw-r--   0 am        (1000) am        (1000)     2241 2023-04-13 11:07:46.000000 optscale_arcee-0.1.30/optscale_arcee.egg-info/PKG-INFO
--rw-rw-r--   0 am        (1000) am        (1000)      734 2023-04-13 11:07:46.000000 optscale_arcee-0.1.30/optscale_arcee.egg-info/SOURCES.txt
--rw-rw-r--   0 am        (1000) am        (1000)        1 2023-04-13 11:07:46.000000 optscale_arcee-0.1.30/optscale_arcee.egg-info/dependency_links.txt
--rw-rw-r--   0 am        (1000) am        (1000)       60 2023-04-13 11:07:46.000000 optscale_arcee-0.1.30/optscale_arcee.egg-info/requires.txt
--rw-rw-r--   0 am        (1000) am        (1000)       15 2023-04-13 11:07:46.000000 optscale_arcee-0.1.30/optscale_arcee.egg-info/top_level.txt
--rw-rw-r--   0 am        (1000) am        (1000)      524 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/setup.cfg
--rw-rw-r--   0 am        (1000) am        (1000)       69 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/setup.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-04-13 11:07:46.411026 optscale_arcee-0.1.30/tests/
--rw-rw-r--   0 am        (1000) am        (1000)     4593 2023-03-24 12:30:15.000000 optscale_arcee-0.1.30/tests/test_data.py
--rw-rw-r--   0 am        (1000) am        (1000)     3850 2023-04-07 12:57:57.000000 optscale_arcee-0.1.30/tests/test_platform.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/
+-rw-rw-r--   0 am        (1000) am        (1000)    11304 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/LICENSE.txt
+-rw-rw-r--   0 am        (1000) am        (1000)     2211 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/PKG-INFO
+-rw-rw-r--   0 am        (1000) am        (1000)     1393 2023-05-30 12:01:34.000000 optscale_arcee-0.1.34/README.rst
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/optscale_arcee/
+-rw-rw-r--   0 am        (1000) am        (1000)       95 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4021 2023-05-30 12:01:34.000000 optscale_arcee-0.1.34/optscale_arcee/arcee.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/optscale_arcee/hw_stat_collector/
+-rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/hw_stat_collector/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4103 2023-05-30 12:01:34.000000 optscale_arcee-0.1.34/optscale_arcee/hw_stat_collector/collector.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/optscale_arcee/module_collector/
+-rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/module_collector/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)     2633 2023-04-07 12:57:57.000000 optscale_arcee-0.1.34/optscale_arcee/module_collector/collector.py
+-rw-rw-r--   0 am        (1000) am        (1000)     6757 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/name_generator.py
+-rw-rw-r--   0 am        (1000) am        (1000)     9821 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/platform.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/optscale_arcee/platforms_meta/
+-rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/platforms_meta/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)     2469 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/platforms_meta/azure.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/optscale_arcee/sender/
+-rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/sender/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4567 2023-05-30 12:01:34.000000 optscale_arcee-0.1.34/optscale_arcee/sender/sender.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/optscale_arcee.egg-info/
+-rw-rw-r--   0 am        (1000) am        (1000)     2211 2023-05-30 12:07:27.000000 optscale_arcee-0.1.34/optscale_arcee.egg-info/PKG-INFO
+-rw-rw-r--   0 am        (1000) am        (1000)      734 2023-05-30 12:07:27.000000 optscale_arcee-0.1.34/optscale_arcee.egg-info/SOURCES.txt
+-rw-rw-r--   0 am        (1000) am        (1000)        1 2023-05-30 12:07:27.000000 optscale_arcee-0.1.34/optscale_arcee.egg-info/dependency_links.txt
+-rw-rw-r--   0 am        (1000) am        (1000)       60 2023-05-30 12:07:27.000000 optscale_arcee-0.1.34/optscale_arcee.egg-info/requires.txt
+-rw-rw-r--   0 am        (1000) am        (1000)       15 2023-05-30 12:07:27.000000 optscale_arcee-0.1.34/optscale_arcee.egg-info/top_level.txt
+-rw-rw-r--   0 am        (1000) am        (1000)      524 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/setup.cfg
+-rw-rw-r--   0 am        (1000) am        (1000)       69 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/setup.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/tests/
+-rw-rw-r--   0 am        (1000) am        (1000)     4593 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/tests/test_data.py
+-rw-rw-r--   0 am        (1000) am        (1000)     3850 2023-04-07 12:57:57.000000 optscale_arcee-0.1.34/tests/test_platform.py
```

### Comparing `optscale_arcee-0.1.30/LICENSE.txt` & `optscale_arcee-0.1.34/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.30/PKG-INFO` & `optscale_arcee-0.1.34/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optscale_arcee
-Version: 0.1.30
+Version: 0.1.34
 Summary: ML profiling tool for OptScale
 Home-page: https://my.optscale.com/
 Author: Hystax
 License: UNKNOWN
 Description: # Arcee
         ## *The OptScale ML profiling tool by Hystax*
         
@@ -21,45 +21,45 @@
         First of all you need to import and init arcee in your code:
         ```sh
         import optscale_arcee as arcee
         ```
         
         ```sh
         # init arcee using context manager syntax
-        with arcee.init('token', 'application_key'):
+        with arcee.init('token', 'model_key'):
             # some code
         ```
         
         To use custom endpoint and enable\disable ssl checks (supports using self-signed ssl certificates):
         ```sh
-        with arcee.init('token', 'application_key', endpoint_url='https://my.custom.endpoint:443/arcee/v2', ssl=False):
+        with arcee.init('token', 'model_key', endpoint_url='https://my.custom.endpoint:443/arcee/v2', ssl=False):
             # some code
         ```
         
         Alternatively arcee can be initialized via function call. However manual finish is required:
         ```sh
-        arcee.init('token', 'application_key')
+        arcee.init('token', 'model_key')
         # some code
         arcee.finish()
         ```
         
         Or in error case:
         ```sh
-        arcee.init('token', 'application_key')
+        arcee.init('token', 'model_key')
         # some code
         arcee.error()
         ```
         
         To send stats:
         ```sh
         arcee.send({"loss": 2.0012, "iter": 2, "epoch": 1})
         ```
         (key should be string, value - int or float, multiple values can be sent)
         
-        To add tags to application run (key, value):
+        To add tags to model run (key, value):
         ```sh
         arcee.tag("project", "torchvision demo")
         ```
         
         To add milestones:
         ```sh
         arcee.milestone("Download test data")
```

### Comparing `optscale_arcee-0.1.30/README.rst` & `optscale_arcee-0.1.34/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -14,45 +14,45 @@
 First of all you need to import and init arcee in your code:
 ```sh
 import optscale_arcee as arcee
 ```
 
 ```sh
 # init arcee using context manager syntax
-with arcee.init('token', 'application_key'):
+with arcee.init('token', 'model_key'):
     # some code
 ```
 
 To use custom endpoint and enable\disable ssl checks (supports using self-signed ssl certificates):
 ```sh
-with arcee.init('token', 'application_key', endpoint_url='https://my.custom.endpoint:443/arcee/v2', ssl=False):
+with arcee.init('token', 'model_key', endpoint_url='https://my.custom.endpoint:443/arcee/v2', ssl=False):
     # some code
 ```
 
 Alternatively arcee can be initialized via function call. However manual finish is required:
 ```sh
-arcee.init('token', 'application_key')
+arcee.init('token', 'model_key')
 # some code
 arcee.finish()
 ```
 
 Or in error case:
 ```sh
-arcee.init('token', 'application_key')
+arcee.init('token', 'model_key')
 # some code
 arcee.error()
 ```
 
 To send stats:
 ```sh
 arcee.send({"loss": 2.0012, "iter": 2, "epoch": 1})
 ```
 (key should be string, value - int or float, multiple values can be sent)
 
-To add tags to application run (key, value):
+To add tags to model run (key, value):
 ```sh
 arcee.tag("project", "torchvision demo")
 ```
 
 To add milestones:
 ```sh
 arcee.milestone("Download test data")
```

### Comparing `optscale_arcee-0.1.30/optscale_arcee/arcee.py` & `optscale_arcee-0.1.34/optscale_arcee/arcee.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import time
 import threading
+
 from optscale_arcee.sender.sender import Sender
 from optscale_arcee.name_generator import NameGenerator
 
 
 def single(class_):
     instances = {}
 
@@ -13,43 +14,46 @@
             instances[class_] = class_(*args, **kwargs)
         return instances[class_]
 
     return get_instance
 
 
 class Job(threading.Thread):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, shutdown_flag, *args, **kwargs):
         # TODO: typing
         threading.Thread.__init__(self)
-        self.shutdown_flag = threading.Event()
+        self.__shutdown_flag = shutdown_flag
         self.__kw = kwargs
 
     def s_noblock(self, sender, run, token):
         return asyncio.run(sender.send_proc_data(run, token))
 
     def job(self):
         args = self.__kw.get("meth_args", list())
         self.s_noblock(*args)
 
     def run(self):
         sleep = self.__kw.get("sleep")
         if not sleep or not isinstance(sleep, int):
             # 1 second by default
             sleep = 1
-        while not self.shutdown_flag.is_set():
+        while not self.__shutdown_flag.is_set():
             self.job()
             time.sleep(sleep)
 
 
 @single
 class Arcee:
-    def __init__(self, token=None, application_key=None, endpoint_url=None, ssl=True):
+    def __init__(
+            self, token=None, model_key=None, endpoint_url=None, ssl=True
+    ):
+        self.shutdown_flag = threading.Event()
         self.token = token
-        self.application_key = application_key
-        self.sender = Sender(endpoint_url, ssl)
+        self.model_key = model_key
+        self.sender = Sender(endpoint_url, ssl, self.shutdown_flag)
         self.hb = None
         self._run = None
         self._tags = {}
         self._name = None
 
     @property
     def run(self):
@@ -83,22 +87,29 @@
         if exc_type is None:
             finish()
         else:
             error()
         return exc_type is None
 
 
-def init(token, application_key, run_name=None, endpoint_url=None, ssl=True, period=1):
-    arcee = Arcee(token, application_key, endpoint_url, ssl)
+def init(token, model_key, run_name=None, endpoint_url=None, ssl=True, period=1):
+    arcee = Arcee(token, model_key, endpoint_url, ssl)
     name = run_name if run_name is not None else NameGenerator.get_random_name()
-    run_id = asyncio.run(arcee.sender.get_run_id(application_key, token, name))["id"]
+    run_id = asyncio.run(arcee.sender.get_run_id(model_key, token, name))["id"]
     arcee.run = run_id
     arcee.name = name
-    arcee.hb = Job(meth_args=(arcee.sender, run_id, token), sleep=period)
+    arcee.hb = Job(meth_args=(arcee.sender, run_id, token), sleep=period,
+                   shutdown_flag=arcee.shutdown_flag)
     arcee.hb.start()
+    asyncio.run(
+        arcee.sender.send_stats(
+            arcee.token,
+            {"project": arcee.model_key, "run": arcee.run, "data": {}},
+        )
+    )
     return arcee
 
 
 def tag(key, value):
     arcee = Arcee()
     arcee.tags = (key, value)
     asyncio.run(arcee.sender.add_tags(arcee.run, arcee.token, arcee.tags))
@@ -122,15 +133,15 @@
                 arcee.run,
                 arcee.token,
                 2,
                 True,
             )
         )
     finally:
-        arcee.hb.shutdown_flag.set()
+        arcee.shutdown_flag.set()
         arcee.hb.join()
 
 
 def error():
     arcee = Arcee()
     try:
         asyncio.run(
@@ -138,24 +149,24 @@
                 arcee.run,
                 arcee.token,
                 3,
                 True,
             )
         )
     finally:
-        arcee.hb.shutdown_flag.set()
+        arcee.shutdown_flag.set()
         arcee.hb.join()
 
 
 def info():
     arcee = Arcee()
     return arcee.__dict__
 
 
 def send(data):
     arcee = Arcee()
     asyncio.run(
         arcee.sender.send_stats(
             arcee.token,
-            {"project": arcee.application_key, "run": arcee.run, "data": data},
+            {"project": arcee.model_key, "run": arcee.run, "data": data},
         )
     )
```

### Comparing `optscale_arcee-0.1.30/optscale_arcee/hw_stat_collector/collector.py` & `optscale_arcee-0.1.34/optscale_arcee/hw_stat_collector/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         stats = {
             "avg_gpu_memory_free": avg_gpu_memory_free,
             "avg_gpu_memory_total": avg_gpu_memory_total,
             "avg_gpu_memory_used": avg_gpu_memory_used,
         }
         # get rid of devices with limited support
         if not math.isnan(avg_gpu_load):
-            stats["avg_gpu_load"] = avg_gpu_load * 100,
+            stats["avg_gpu_load"] = avg_gpu_load * 100
         return stats
 
     @staticmethod
     def _ps_stats(cpu_interval=0.5, proc_interval=0.5):
         load1, load5, load15 = psutil.getloadavg()
         cpu_load = psutil.cpu_percent(interval=cpu_interval, percpu=True)
         cpu_percent = round(sum(cpu_load) / psutil.cpu_count(), 2)
@@ -78,15 +78,15 @@
         ps_stats = {
             "cpu_count": psutil.cpu_count(),
             "cpu_percent": cpu_percent,
             "cpu_percent_percpu": cpu_load,
             "load_average": [load1, load5, load15],
             "cpu_usage": (load15 / psutil.cpu_count()) * 100,
             "used_ram_percent": psutil.virtual_memory()[2],
-            "used_ram_mb": psutil.virtual_memory()[3] / 1000000,
+            "used_ram_mb": psutil.virtual_memory()[3] / (1024 * 1024),
         }
 
         proc_stats = {
             # process cpu usage in % (per core)
             "cpu": cpu_proc,
             "mem": {
                 # process virtual memory usage, p - percent, t - value
```

### Comparing `optscale_arcee-0.1.30/optscale_arcee/module_collector/collector.py` & `optscale_arcee-0.1.34/optscale_arcee/module_collector/collector.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.30/optscale_arcee/name_generator.py` & `optscale_arcee-0.1.34/optscale_arcee/name_generator.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.30/optscale_arcee/platform.py` & `optscale_arcee-0.1.34/optscale_arcee/platform.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.30/optscale_arcee/platforms_meta/azure.py` & `optscale_arcee-0.1.34/optscale_arcee/platforms_meta/azure.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.30/optscale_arcee/sender/sender.py` & `optscale_arcee-0.1.34/optscale_arcee/sender/sender.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 import aiohttp
+import threading
 
 from optscale_arcee.platform import CollectorFactory
 from optscale_arcee.module_collector.collector import Collector as ImportsCollector
 from optscale_arcee.hw_stat_collector.collector import Collector as HwCollector
 
 
+def check_shutdown_flag_set(function):
+    async def inner(self, *args, **kwargs):
+        if not self.shutdown_flag.is_set():
+            return await function(self, *args, **kwargs)
+    return inner
+
+
 class Sender:
 
     # default OptScale url
     base_url = "https://my.optscale.com:443/arcee/v2"
 
-    def __init__(self, endpoint_url=None, ssl=True):
+    def __init__(self, endpoint_url=None, ssl=True, shutdown_flag=None):
         if endpoint_url is None:
             endpoint_url = self.base_url
         self.endpoint_url = endpoint_url
+        self.shutdown_flag = shutdown_flag or threading.Event()
         self.ssl = ssl
 
     @staticmethod
     async def m():
         platform = await CollectorFactory.get()
         return await platform().get_platform_meta()
 
@@ -46,50 +55,57 @@
     async def send_patch_request(self, url, headers=None, data=None) -> str:
         async with aiohttp.ClientSession(headers=headers) as session:
             async with session.patch(
                 url, json=data, raise_for_status=True, ssl=self.ssl
             ) as response:
                 return await response.json()
 
-    async def get_run_id(self, application, token, run_name):
-        uri = "%s/applications/%s/run" % (self.endpoint_url, application)
+    @check_shutdown_flag_set
+    async def get_run_id(self, model_key, token, run_name):
+        uri = "%s/applications/%s/run" % (self.endpoint_url, model_key)
         headers = {"x-api-key": token, "Content-Type": "application/json"}
         data = {"imports": await self._imports_data(), "name": run_name}
         return await self.send_post_request(uri, headers, data)
 
+    @check_shutdown_flag_set
     async def add_milestone(self, run_id, token, value):
         uri = "%s/run/%s/milestones" % (self.endpoint_url, run_id)
         headers = {"x-api-key": token, "Content-Type": "application/json"}
         return await self.send_post_request(uri, headers, {"milestone": value})
 
+    @check_shutdown_flag_set
     async def add_tags(self, run_id, token, tags):
         uri = "%s/run/%s" % (self.endpoint_url, run_id)
         headers = {"x-api-key": token, "Content-Type": "application/json"}
         return await self.send_patch_request(uri, headers, {"tags": tags})
 
+    @check_shutdown_flag_set
     async def change_state(self, run_id, token, state, finish=False):
         uri = "%s/run/%s" % (self.endpoint_url, run_id)
         headers = {"x-api-key": token, "Content-Type": "application/json"}
         return await self.send_patch_request(
             uri, headers, {"state": state, "finish": finish}
         )
 
+    @check_shutdown_flag_set
     async def create_stage(self, run_id, token, name):
         uri = "%s/run/%s/stages" % (self.endpoint_url, run_id)
         headers = {"x-api-key": token, "Content-Type": "application/json"}
         return await self.send_post_request(uri, headers, {"stage": name})
 
+    @check_shutdown_flag_set
     async def send_stats(self, token, data):
         headers = {"x-api-key": token, "Content-Type": "application/json"}
         meta = await self.m()
         data.update({"platform": meta.to_dict()})
         await self.send_post_request(
             "%s/%s" % (self.endpoint_url, "collect"), headers, data
         )
 
+    @check_shutdown_flag_set
     async def send_proc_data(self, run_id, token):
         uri = "%s/run/%s/proc" % (self.endpoint_url, run_id)
         headers = {"x-api-key": token, "Content-Type": "application/json"}
         data = dict()
         meta = await self.m()
         proc = await self._proc_data()
         data.update({"platform": meta.to_dict()})
```

### Comparing `optscale_arcee-0.1.30/optscale_arcee.egg-info/PKG-INFO` & `optscale_arcee-0.1.34/optscale_arcee.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optscale-arcee
-Version: 0.1.30
+Version: 0.1.34
 Summary: ML profiling tool for OptScale
 Home-page: https://my.optscale.com/
 Author: Hystax
 License: UNKNOWN
 Description: # Arcee
         ## *The OptScale ML profiling tool by Hystax*
         
@@ -21,45 +21,45 @@
         First of all you need to import and init arcee in your code:
         ```sh
         import optscale_arcee as arcee
         ```
         
         ```sh
         # init arcee using context manager syntax
-        with arcee.init('token', 'application_key'):
+        with arcee.init('token', 'model_key'):
             # some code
         ```
         
         To use custom endpoint and enable\disable ssl checks (supports using self-signed ssl certificates):
         ```sh
-        with arcee.init('token', 'application_key', endpoint_url='https://my.custom.endpoint:443/arcee/v2', ssl=False):
+        with arcee.init('token', 'model_key', endpoint_url='https://my.custom.endpoint:443/arcee/v2', ssl=False):
             # some code
         ```
         
         Alternatively arcee can be initialized via function call. However manual finish is required:
         ```sh
-        arcee.init('token', 'application_key')
+        arcee.init('token', 'model_key')
         # some code
         arcee.finish()
         ```
         
         Or in error case:
         ```sh
-        arcee.init('token', 'application_key')
+        arcee.init('token', 'model_key')
         # some code
         arcee.error()
         ```
         
         To send stats:
         ```sh
         arcee.send({"loss": 2.0012, "iter": 2, "epoch": 1})
         ```
         (key should be string, value - int or float, multiple values can be sent)
         
-        To add tags to application run (key, value):
+        To add tags to model run (key, value):
         ```sh
         arcee.tag("project", "torchvision demo")
         ```
         
         To add milestones:
         ```sh
         arcee.milestone("Download test data")
```

### Comparing `optscale_arcee-0.1.30/optscale_arcee.egg-info/SOURCES.txt` & `optscale_arcee-0.1.34/optscale_arcee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.30/setup.cfg` & `optscale_arcee-0.1.34/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = optscale_arcee
-version = 0.1.30
+version = 0.1.34
 author = Hystax
 description = ML profiling tool for OptScale
 long_description = file: README.rst
 long_description_content_type = text/markdown
 url = https://my.optscale.com/
 keywords = arcee, ml, optscale, finops, mlops
```

### Comparing `optscale_arcee-0.1.30/tests/test_data.py` & `optscale_arcee-0.1.34/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.30/tests/test_platform.py` & `optscale_arcee-0.1.34/tests/test_platform.py`

 * *Files identical despite different names*

