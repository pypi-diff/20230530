# Comparing `tmp/latch_asgi-0.1.2.tar.gz` & `tmp/latch_asgi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_asgi-0.1.2.tar", max compression
+gzip compressed data, was "latch_asgi-0.1.3.tar", max compression
```

## Comparing `latch_asgi-0.1.2.tar` & `latch_asgi-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       14 2023-05-29 19:32:41.850558 latch_asgi-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-29 19:37:32.876999 latch_asgi-0.1.2/latch_asgi/__init__.py
--rw-r--r--   0        0        0     5002 2023-05-29 19:42:37.064349 latch_asgi-0.1.2/latch_asgi/asgi_iface.py
--rw-r--r--   0        0        0     4999 2023-05-29 20:11:30.512830 latch_asgi-0.1.2/latch_asgi/auth.py
--rw-r--r--   0        0        0      241 2023-05-29 22:40:28.861103 latch_asgi-0.1.2/latch_asgi/config.py
--rw-r--r--   0        0        0     2802 2023-05-29 20:13:46.441816 latch_asgi-0.1.2/latch_asgi/context.py
--rw-r--r--   0        0        0     3306 2023-05-29 20:18:25.688320 latch_asgi-0.1.2/latch_asgi/datadog_propagator.py
--rw-r--r--   0        0        0     5261 2023-05-29 20:03:21.571328 latch_asgi-0.1.2/latch_asgi/framework.py
--rw-r--r--   0        0        0        0 2023-05-29 20:46:30.864706 latch_asgi-0.1.2/latch_asgi/py.typed
--rw-r--r--   0        0        0     8364 2023-05-29 22:41:13.000935 latch_asgi-0.1.2/latch_asgi/server.py
--rw-r--r--   0        0        0     1388 2023-05-29 22:40:47.473863 latch_asgi-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 latch_asgi-0.1.2/setup.py
--rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 latch_asgi-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       14 2023-05-29 19:32:41.850558 latch_asgi-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 19:37:32.876999 latch_asgi-0.1.3/latch_asgi/__init__.py
+-rw-r--r--   0        0        0     5002 2023-05-29 19:42:37.064349 latch_asgi-0.1.3/latch_asgi/asgi_iface.py
+-rw-r--r--   0        0        0     4999 2023-05-29 20:11:30.512830 latch_asgi-0.1.3/latch_asgi/auth.py
+-rw-r--r--   0        0        0      241 2023-05-29 22:40:28.861103 latch_asgi-0.1.3/latch_asgi/config.py
+-rw-r--r--   0        0        0     2802 2023-05-29 20:13:46.441816 latch_asgi-0.1.3/latch_asgi/context.py
+-rw-r--r--   0        0        0     3306 2023-05-29 20:18:25.688320 latch_asgi-0.1.3/latch_asgi/datadog_propagator.py
+-rw-r--r--   0        0        0     5261 2023-05-29 20:03:21.571328 latch_asgi-0.1.3/latch_asgi/framework.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:46:30.864706 latch_asgi-0.1.3/latch_asgi/py.typed
+-rw-r--r--   0        0        0     8366 2023-05-29 22:51:16.303612 latch_asgi-0.1.3/latch_asgi/server.py
+-rw-r--r--   0        0        0     1388 2023-05-29 22:53:37.196720 latch_asgi-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 latch_asgi-0.1.3/setup.py
+-rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 latch_asgi-0.1.3/PKG-INFO
```

### Comparing `latch_asgi-0.1.2/latch_asgi/asgi_iface.py` & `latch_asgi-0.1.3/latch_asgi/asgi_iface.py`

 * *Files identical despite different names*

### Comparing `latch_asgi-0.1.2/latch_asgi/auth.py` & `latch_asgi-0.1.3/latch_asgi/auth.py`

 * *Files identical despite different names*

### Comparing `latch_asgi-0.1.2/latch_asgi/context.py` & `latch_asgi-0.1.3/latch_asgi/context.py`

 * *Files identical despite different names*

### Comparing `latch_asgi-0.1.2/latch_asgi/datadog_propagator.py` & `latch_asgi-0.1.3/latch_asgi/datadog_propagator.py`

 * *Files identical despite different names*

### Comparing `latch_asgi-0.1.2/latch_asgi/framework.py` & `latch_asgi-0.1.3/latch_asgi/framework.py`

 * *Files identical despite different names*

### Comparing `latch_asgi-0.1.2/latch_asgi/server.py` & `latch_asgi-0.1.3/latch_asgi/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         while True:
             message = await receive()
             await log.info(repr(message.type))
 
             if isinstance(message, LifespanStartupEvent):
                 with tracer.start_as_current_span("startup"):
                     try:
-                        await log.info("Connecting to Vacuole")
+                        await log.info("Executing startup tasks")
                         # todo(maximsmol): debug clock skew on connection reset
                         await asyncio.gather(*self.startup_tasks)
 
                         with tracer.start_as_current_span("send completion event"):
                             await send(
                                 LifespanStartupCompleteEvent("lifespan.startup.complete")
                             )
```

### Comparing `latch_asgi-0.1.2/pyproject.toml` & `latch_asgi-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-asgi"
-version = "0.1.2"
+version = "0.1.3"
 description = "ASGI python server"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_asgi"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_asgi-0.1.2/setup.py` & `latch_asgi-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'opentelemetry-instrumentation-asgi>=0.36b0,<0.37',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'orjson>=3.8.5,<4.0.0',
  'pysimdjson>=5.0.2,<6.0.0']
 
 setup_kwargs = {
     'name': 'latch-asgi',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'ASGI python server',
     'long_description': '# python-asgi\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `latch_asgi-0.1.2/PKG-INFO` & `latch_asgi-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latch-asgi
-Version: 0.1.2
+Version: 0.1.3
 Summary: ASGI python server
 License: CC0 1.0
 Author: Max Smolin
 Author-email: max@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

