# Comparing `tmp/configzen-0.1.46.tar.gz` & `tmp/configzen-0.1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.46.tar", max compression
+gzip compressed data, was "configzen-0.1.47.tar", max compression
```

## Comparing `configzen-0.1.46.tar` & `configzen-0.1.47.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.46/configzen/__init__.py
--rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.1.46/configzen/__main__.py
--rw-r--r--   0        0        0    59167 2023-05-30 01:58:49.826473 configzen-0.1.46/configzen/config.py
--rw-r--r--   0        0        0     2553 2023-05-30 00:29:12.193684 configzen-0.1.46/configzen/errors.py
--rw-r--r--   0        0        0    20820 2023-05-30 00:45:02.555346 configzen-0.1.46/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.46/configzen/py.typed
--rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.1.46/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.46/LICENSE
--rw-r--r--   0        0        0     1155 2023-05-30 01:59:16.842583 configzen-0.1.46/pyproject.toml
--rw-r--r--   0        0        0     7326 2023-05-30 00:29:12.142683 configzen-0.1.46/README.md
--rw-r--r--   0        0        0     7852 1970-01-01 00:00:00.000000 configzen-0.1.46/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.47/configzen/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.1.47/configzen/__main__.py
+-rw-r--r--   0        0        0    59205 2023-05-30 02:08:56.017181 configzen-0.1.47/configzen/config.py
+-rw-r--r--   0        0        0     2553 2023-05-30 00:29:12.193684 configzen-0.1.47/configzen/errors.py
+-rw-r--r--   0        0        0    20820 2023-05-30 00:45:02.555346 configzen-0.1.47/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.47/configzen/py.typed
+-rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.1.47/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.47/LICENSE
+-rw-r--r--   0        0        0     1155 2023-05-30 02:09:14.792016 configzen-0.1.47/pyproject.toml
+-rw-r--r--   0        0        0     7326 2023-05-30 00:29:12.142683 configzen-0.1.47/README.md
+-rw-r--r--   0        0        0     7852 1970-01-01 00:00:00.000000 configzen-0.1.47/PKG-INFO
```

### Comparing `configzen-0.1.46/configzen/__main__.py` & `configzen-0.1.47/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.46/configzen/config.py` & `configzen-0.1.47/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1831,15 +1831,15 @@
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
         context = get_context(self)
-        tok = current_context.set(context)
+        tok = current_context.set(get_context(context.owner))
         if context.owner is self:
             changed = context.manager.read(config_class=type(self), **kwargs)
         else:
             changed = reload(cast(ConfigAt[ConfigModelT], context.at), **kwargs)
         current_context.reset(tok)
         state = changed.__dict__
         context.initial_state = state
@@ -1942,15 +1942,15 @@
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
         context = get_context(self)
-        tok = current_context.set(context)
+        tok = current_context.set(get_context(context.owner))
         if context.owner is self:
             changed = await context.manager.read_async(
                 config_class=type(self), **kwargs
             )
         else:
             changed = await reload_async(
                 cast(ConfigAt[ConfigModelT], context.at), **kwargs
```

### Comparing `configzen-0.1.46/configzen/errors.py` & `configzen-0.1.47/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.46/configzen/processor.py` & `configzen-0.1.47/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.46/configzen/typedefs.py` & `configzen-0.1.47/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.46/LICENSE` & `configzen-0.1.47/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.46/pyproject.toml` & `configzen-0.1.47/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.46"
+version = "0.1.47"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.1.46/README.md` & `configzen-0.1.47/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.46/PKG-INFO` & `configzen-0.1.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.46
+Version: 0.1.47
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

