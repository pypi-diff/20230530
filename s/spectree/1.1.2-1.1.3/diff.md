# Comparing `tmp/spectree-1.1.2.tar.gz` & `tmp/spectree-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectree-1.1.2.tar", last modified: Mon Apr 24 13:26:47 2023, max compression
+gzip compressed data, was "spectree-1.1.3.tar", last modified: Tue May 30 09:31:32 2023, max compression
```

## Comparing `spectree-1.1.2.tar` & `spectree-1.1.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:26:47.396857 spectree-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-24 13:26:32.000000 spectree-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 13:26:32.000000 spectree-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-04-24 13:26:47.396857 spectree-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-04-24 13:26:32.000000 spectree-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-24 13:26:32.000000 spectree-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:26:47.396857 spectree-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 13:26:32.000000 spectree-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:26:47.392857 spectree-1.1.2/spectree/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:26:47.392857 spectree-1.1.2/spectree/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/plugins/falcon_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/plugins/flask_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/plugins/quart_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/plugins/starlette_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:26:47.392857 spectree-1.1.2/spectree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-04-24 13:26:47.000000 spectree-1.1.2/spectree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-24 13:26:47.000000 spectree-1.1.2/spectree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:26:47.000000 spectree-1.1.2/spectree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 13:26:47.000000 spectree-1.1.2/spectree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 13:26:47.000000 spectree-1.1.2/spectree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:26:47.396857 spectree-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_falcon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_falcon_asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_flask_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_flask_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_quart.py
--rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:31:32.521828 spectree-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-30 09:31:18.000000 spectree-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 09:31:18.000000 spectree-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18665 2023-05-30 09:31:32.521828 spectree-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-05-30 09:31:18.000000 spectree-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-30 09:31:18.000000 spectree-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 09:31:32.521828 spectree-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-30 09:31:18.000000 spectree-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:31:32.517828 spectree-1.1.3/spectree/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:31:32.517828 spectree-1.1.3/spectree/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/plugins/falcon_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/plugins/flask_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/plugins/quart_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/plugins/starlette_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13804 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:31:32.517828 spectree-1.1.3/spectree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18665 2023-05-30 09:31:32.000000 spectree-1.1.3/spectree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-30 09:31:32.000000 spectree-1.1.3/spectree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:31:32.000000 spectree-1.1.3/spectree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-30 09:31:32.000000 spectree-1.1.3/spectree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 09:31:32.000000 spectree-1.1.3/spectree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:31:32.521828 spectree-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_falcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_falcon_asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_flask_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_flask_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_quart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_utils.py
```

### Comparing `spectree-1.1.2/LICENSE` & `spectree-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/PKG-INFO` & `spectree-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: spectree
-Version: 1.1.2
+Version: 1.1.3
 Summary: generate OpenAPI document and validate request&response with Python annotations.
 Author-email: Keming Yang <kemingy94@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/0b01001001/spectree
 Project-URL: documentation, https://0b01001001.github.io/spectree/
 Project-URL: repository, https://github.com/0b01001001/spectree
 Project-URL: changelog, https://github.com/0b01001001/spectree/releases
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: email
 Provides-Extra: flask
 Provides-Extra: quart
 Provides-Extra: falcon
 Provides-Extra: starlette
 Provides-Extra: dev
```

### Comparing `spectree-1.1.2/README.md` & `spectree-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/pyproject.toml` & `spectree-1.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 [project]
 name = "spectree"
-version = "1.1.2"
+version = "1.1.3"
 dynamic = []
 description = "generate OpenAPI document and validate request&response with Python annotations."
 readme = "README.md"
 license = {text = "Apache-2.0"}
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 authors = [
     { name = "Keming Yang", email = "kemingy94@gmail.com" },
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
```

### Comparing `spectree-1.1.2/setup.py` & `spectree-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/spectree/_types.py` & `spectree-1.1.3/spectree/_types.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/spectree/config.py` & `spectree-1.1.3/spectree/config.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/spectree/models.py` & `spectree-1.1.3/spectree/models.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/spectree/page.py` & `spectree-1.1.3/spectree/page.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/spectree/plugins/__init__.py` & `spectree-1.1.3/spectree/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/spectree/plugins/base.py` & `spectree-1.1.3/spectree/plugins/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -105,7 +105,20 @@
     def parse_func(self, route: BackendRoute):
         """
         :param route: API routes
 
         get the endpoint function from routes
         """
         raise NotImplementedError
+
+    def get_func_operation_id(self, func: Callable, path: str, method: str):
+        """
+        :param func: route function (endpoint)
+        :param method: URI path for this route function
+        :param method: HTTP method for this route function
+
+        get the operation_id value for the endpoint
+        """
+        operation_id = getattr(func, "operation_id", None)
+        if not operation_id:
+            operation_id = f"{method.lower()}_{path.replace('/', '_')}"
+        return operation_id
```

### Comparing `spectree-1.1.2/spectree/plugins/falcon_plugin.py` & `spectree-1.1.3/spectree/plugins/falcon_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/spectree/plugins/flask_plugin.py` & `spectree-1.1.3/spectree/plugins/flask_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/spectree/plugins/quart_plugin.py` & `spectree-1.1.3/spectree/plugins/quart_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/spectree/plugins/starlette_plugin.py` & `spectree-1.1.3/spectree/plugins/starlette_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/spectree/response.py` & `spectree-1.1.3/spectree/response.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/spectree/spec.py` & `spectree-1.1.3/spectree/spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -296,21 +296,19 @@
                 func_tags = getattr(func, "tags", ())
                 for tag in func_tags:
                     if str(tag) not in tags:
                         tags[str(tag)] = (
                             tag.dict() if isinstance(tag, Tag) else {"name": tag}
                         )
 
-                operation_id = getattr(func, "operation_id", None)
-                if not operation_id:
-                    operation_id = f"{method.lower()}_{path.replace('/', '_')}"
-
                 routes[path][method.lower()] = {
                     "summary": summary or f"{name} <{method}>",
-                    "operationId": operation_id,
+                    "operationId": self.backend.get_func_operation_id(
+                        func, path, method
+                    ),
                     "description": desc or "",
                     "tags": [str(x) for x in getattr(func, "tags", ())],
                     "parameters": parse_params(func, parameters[:], self.models),
                     "responses": parse_resp(func, self.naming_strategy),
                 }
 
                 security = getattr(func, "security", None)
```

### Comparing `spectree-1.1.2/spectree/utils.py` & `spectree-1.1.3/spectree/utils.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/spectree.egg-info/PKG-INFO` & `spectree-1.1.3/spectree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: spectree
-Version: 1.1.2
+Version: 1.1.3
 Summary: generate OpenAPI document and validate request&response with Python annotations.
 Author-email: Keming Yang <kemingy94@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/0b01001001/spectree
 Project-URL: documentation, https://0b01001001.github.io/spectree/
 Project-URL: repository, https://github.com/0b01001001/spectree
 Project-URL: changelog, https://github.com/0b01001001/spectree/releases
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: email
 Provides-Extra: flask
 Provides-Extra: quart
 Provides-Extra: falcon
 Provides-Extra: starlette
 Provides-Extra: dev
```

### Comparing `spectree-1.1.2/spectree.egg-info/SOURCES.txt` & `spectree-1.1.3/spectree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/tests/test_config.py` & `spectree-1.1.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/tests/test_plugin.py` & `spectree-1.1.3/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/tests/test_plugin_falcon.py` & `spectree-1.1.3/tests/test_plugin_falcon.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/tests/test_plugin_falcon_asgi.py` & `spectree-1.1.3/tests/test_plugin_falcon_asgi.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/tests/test_plugin_flask.py` & `spectree-1.1.3/tests/test_plugin_flask.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/tests/test_plugin_flask_blueprint.py` & `spectree-1.1.3/tests/test_plugin_flask_blueprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,14 @@
     api.register(app)
 
     flask_app = Flask(__name__)
     flask_app.register_blueprint(app, **register_blueprint_kwargs)
 
     with flask_app.app_context():
         api.spec
-    api.register(app)
 
     with flask_app.test_client() as test_client:
         yield test_client, api
 
 
 @pytest.mark.parametrize(
     ("test_client_and_api", "prefix"),
```

### Comparing `spectree-1.1.2/tests/test_plugin_flask_view.py` & `spectree-1.1.3/tests/test_plugin_flask_view.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/tests/test_plugin_quart.py` & `spectree-1.1.3/tests/test_plugin_quart.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/tests/test_plugin_starlette.py` & `spectree-1.1.3/tests/test_plugin_starlette.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,25 +179,26 @@
         ),
         Mount("/static", app=StaticFiles(directory="docs"), name="static"),
     ]
 )
 
 
 def inner_register_func():
-    @app.route("/api/user/{name}/address/{address_id}")
     @api.validate(
         query=Query,
         path_parameter_descriptions={
             "name": "The name that uniquely identifies the user.",
             "non-existent-param": "description",
         },
     )
     def user_address(request):
         return None
 
+    app.routes.append(Route("/api/user/{name}/address/{address_id}", user_address))
+
 
 inner_register_func()
 api.register(app)
 
 
 @pytest.fixture
 def client():
```

### Comparing `spectree-1.1.2/tests/test_response.py` & `spectree-1.1.3/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/tests/test_spec.py` & `spectree-1.1.3/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.2/tests/test_utils.py` & `spectree-1.1.3/tests/test_utils.py`

 * *Files identical despite different names*

