# Comparing `tmp/configzen-0.1.44.tar.gz` & `tmp/configzen-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.44.tar", max compression
+gzip compressed data, was "configzen-0.1.45.tar", max compression
```

## Comparing `configzen-0.1.44.tar` & `configzen-0.1.45.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.44/configzen/__init__.py
--rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.1.44/configzen/__main__.py
--rw-r--r--   0        0        0    58999 2023-05-30 00:59:59.013627 configzen-0.1.44/configzen/config.py
--rw-r--r--   0        0        0     2553 2023-05-30 00:29:12.193684 configzen-0.1.44/configzen/errors.py
--rw-r--r--   0        0        0    20820 2023-05-30 00:45:02.555346 configzen-0.1.44/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.44/configzen/py.typed
--rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.1.44/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.44/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-30 01:00:43.050064 configzen-0.1.44/pyproject.toml
--rw-r--r--   0        0        0     7326 2023-05-30 00:29:12.142683 configzen-0.1.44/README.md
--rw-r--r--   0        0        0     7806 1970-01-01 00:00:00.000000 configzen-0.1.44/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.45/configzen/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.1.45/configzen/__main__.py
+-rw-r--r--   0        0        0    59025 2023-05-30 01:43:37.404238 configzen-0.1.45/configzen/config.py
+-rw-r--r--   0        0        0     2553 2023-05-30 00:29:12.193684 configzen-0.1.45/configzen/errors.py
+-rw-r--r--   0        0        0    20820 2023-05-30 00:45:02.555346 configzen-0.1.45/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.45/configzen/py.typed
+-rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.1.45/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.45/LICENSE
+-rw-r--r--   0        0        0     1155 2023-05-30 01:45:15.877969 configzen-0.1.45/pyproject.toml
+-rw-r--r--   0        0        0     7326 2023-05-30 00:29:12.142683 configzen-0.1.45/README.md
+-rw-r--r--   0        0        0     7852 1970-01-01 00:00:00.000000 configzen-0.1.45/PKG-INFO
```

### Comparing `configzen-0.1.44/configzen/__main__.py` & `configzen-0.1.45/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.44/configzen/config.py` & `configzen-0.1.45/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1775,15 +1775,18 @@
         """
         context = get_context(self)
         self.__dict__.update(context.initial_state)
 
     def __deepcopy__(
         self: ConfigModelT, memodict: dict[Any, Any] | None = None
     ) -> ConfigModelT:
-        return type(self)(**copy.deepcopy(dict(self._iter(to_dict=False))))
+        state = dict(self._iter(to_dict=False))
+        state.pop(LOCAL, None)
+        state.pop(TOKEN, None)
+        return type(self)(**copy.deepcopy(state))
 
     @classmethod
     def load(
         cls: type[ConfigModelT],
         resource: ConfigManager[ConfigModelT] | RawResourceT | None = None,
         create_if_missing: bool | None = None,
         **kwargs: Any,
@@ -1828,19 +1831,19 @@
         Returns
         -------
         self
         """
         context = get_context(self)
         if context.owner is self:
             current_context.set(context)
-            new_config = context.manager.read(config_class=type(self), **kwargs)
-            context.initial_state = new_config.__dict__
-            state = context.initial_state
+            changed = context.manager.read(config_class=type(self), **kwargs)
         else:
-            state = reload(cast(ConfigAt[ConfigModelT], context.at), **kwargs)
+            changed = reload(cast(ConfigAt[ConfigModelT], context.at), **kwargs)
+        state = changed.__dict__
+        context.initial_state = state
         self.update(**state)
         return self
 
     def save(
         self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
     ) -> int:
         """
@@ -1938,23 +1941,23 @@
         Returns
         -------
         self
         """
         context = get_context(self)
         if context.owner is self:
             current_context.set(context)
-            new_async_config = await context.manager.read_async(
+            changed = await context.manager.read_async(
                 config_class=type(self), **kwargs
             )
-            context.initial_state = new_async_config.__dict__
-            state = context.initial_state
         else:
-            state = await reload_async(
+            changed = await reload_async(
                 cast(ConfigAt[ConfigModelT], context.at), **kwargs
             )
+        state = changed.__dict__
+        context.initial_state = state
         self.update(**state)
         return self
 
     async def save_async(
         self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
     ) -> int:
         """
@@ -2008,16 +2011,17 @@
 
     @classmethod
     def __field_setup__(cls, value: Any, field: ModelField) -> Any:
         context = current_context.get()
         if context is not None:
             subcontext = context.enter(field.name)
             tok = current_context.set(subcontext)
-            _vars(value)[TOKEN] = tok
-            _vars(value)[LOCAL] = contextvars.copy_context()
+            vs = _vars(value)
+            vs[TOKEN] = tok
+            vs[LOCAL] = contextvars.copy_context()
         return value
 
 
 class ConfigMeta(pydantic.BaseSettings.Config):
     """
     Meta-configuration for the `ConfigModel` class.
```

### Comparing `configzen-0.1.44/configzen/errors.py` & `configzen-0.1.45/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.44/configzen/processor.py` & `configzen-0.1.45/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.44/configzen/typedefs.py` & `configzen-0.1.45/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.44/LICENSE` & `configzen-0.1.45/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.44/pyproject.toml` & `configzen-0.1.45/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.44"
+version = "0.1.45"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^1.10.7"
 anyconfig = "^0.13.0"
 typing-extensions = { version = "^4.5.0", python = ">=3.9,<3.11"}
 
@@ -23,39 +24,17 @@
 
 [tool.poetry.group.yaml.dependencies]
 pyyaml = "^6.0"
 
 [tool.poetry.group.toml.dependencies]
 toml = "^0.10.2"
 
-[tool.poetry.group.ion.dependencies]
-anyconfig-ion-backend = "^0.1.1"
-
-[tool.poetry.group.bson.dependencies]
-anyconfig-bson-backend = "^0.1.2"
-
-[tool.poetry.group.cbor.dependencies]
-anyconfig-cbor-backend = "^0.1.2"
-
-[tool.poetry.group.cbor2.dependencies]
-anyconfig-cbor2-backend = "^0.1.2"
-
-[tool.poetry.group.configobj.dependencies]
-anyconfig-configobj-backend = "^0.1.4"
-
-[tool.poetry.group.msgpack.dependencies]
-anyconfig-msgpack-backend = "^0.1.1"
-
 [tool.ruff]
 target-version = "py39"
 select = ["F","E","W","I","UP","N","S","C","B","A","T","Q","RUF","YTT","BLE","ANN","FBT","PL","TRY","RSE","SLF","DTZ","EXE","ISC","ICN","G","INP","PIE","RET","SIM","TID","TCH","ARG","PTH"]
 ignore = ["DTZ005","INP001","TCH003","ANN101","ANN102","ANN401","I001","TID252","T201","B905","S101","TRY003","PLR2004"]
 fix = true
 exclude = ["examples/"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
-[project.urls]
-"Homepage" = "https://github.com/bswck/configzen"
-"Bug Tracker" = "https://github.com/bswck/configzen/issues"
```

### Comparing `configzen-0.1.44/README.md` & `configzen-0.1.45/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.44/PKG-INFO` & `configzen-0.1.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.44
+Version: 0.1.45
 Summary: The easiest way to manage configuration files in Python
+Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

