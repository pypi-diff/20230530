# Comparing `tmp/configzen-0.1.47.tar.gz` & `tmp/configzen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.47.tar", max compression
+gzip compressed data, was "configzen-0.2.0.tar", max compression
```

## Comparing `configzen-0.1.47.tar` & `configzen-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.47/configzen/__init__.py
--rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.1.47/configzen/__main__.py
--rw-r--r--   0        0        0    59205 2023-05-30 02:08:56.017181 configzen-0.1.47/configzen/config.py
--rw-r--r--   0        0        0     2553 2023-05-30 00:29:12.193684 configzen-0.1.47/configzen/errors.py
--rw-r--r--   0        0        0    20820 2023-05-30 00:45:02.555346 configzen-0.1.47/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.47/configzen/py.typed
--rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.1.47/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.47/LICENSE
--rw-r--r--   0        0        0     1155 2023-05-30 02:09:14.792016 configzen-0.1.47/pyproject.toml
--rw-r--r--   0        0        0     7326 2023-05-30 00:29:12.142683 configzen-0.1.47/README.md
--rw-r--r--   0        0        0     7852 1970-01-01 00:00:00.000000 configzen-0.1.47/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.0/configzen/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.0/configzen/__main__.py
+-rw-r--r--   0        0        0    60597 2023-05-30 13:45:42.424136 configzen-0.2.0/configzen/config.py
+-rw-r--r--   0        0        0     2553 2023-05-30 00:29:12.193684 configzen-0.2.0/configzen/errors.py
+-rw-r--r--   0        0        0    20820 2023-05-30 00:45:02.555346 configzen-0.2.0/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.0/configzen/py.typed
+-rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.2.0/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1154 2023-05-30 13:46:45.360908 configzen-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7326 2023-05-30 00:29:12.142683 configzen-0.2.0/README.md
+-rw-r--r--   0        0        0     7851 1970-01-01 00:00:00.000000 configzen-0.2.0/PKG-INFO
```

### Comparing `configzen-0.1.47/configzen/__main__.py` & `configzen-0.2.0/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.47/configzen/config.py` & `configzen-0.2.0/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,16 @@
 import pydantic
 from anyconfig.utils import filter_options, is_dict_like, is_list_like
 from pydantic.fields import (  # type: ignore[attr-defined]
     ModelField,
     make_generic_validator,
 )
 from pydantic.json import ENCODERS_BY_TYPE
-from pydantic.main import ModelMetaclass
+from pydantic.main import ModelMetaclass, BaseModel
+from pydantic.utils import ROOT_KEY
 
 from configzen.errors import (
     ConfigAccessError,
     InternalConfigError,
     ResourceLookupError,
     UnspecifiedParserError,
     pretty_syntax_error,
@@ -139,14 +140,18 @@
 TOKEN: str = "__context_token__"
 LOCAL: str = "__local__"
 
 current_context: contextvars.ContextVar[
     BaseContext[Any] | None
 ] = contextvars.ContextVar("current_context", default=None)
 
+_exporting: contextvars.ContextVar[bool] = contextvars.ContextVar(
+    "_exporting", default=False
+)
+
 
 def _get_defaults_from_model_class(
     model: type[pydantic.BaseModel],
 ) -> dict[str, Any]:
     defaults = {}
     for field in model.__fields__.values():
         default = field.default
@@ -293,25 +298,27 @@
         return functools.partial(with_post_deserialize, func)
 
     post_deserialize.register(cls, func)
     return cls
 
 
 @functools.singledispatch
-def export(obj: ConfigModelT) -> dict[str, Any]:
+def export(obj: Any, **kwargs: Any) -> dict[str, Any]:
     """
     Export a ConfigModel to a safely-serializable format.
     Register a custom exporter for a type using the `with_exporter` decorator,
     which can help to exclude particular values from the export if needed.
 
     Parameters
     ----------
     obj
     """
-    return obj.dict()
+    if isinstance(obj, ConfigModel) and not _exporting.get():
+        return obj.export(**kwargs)
+    return cast(dict[str, Any], obj.dict(**kwargs))
 
 
 def with_exporter(
     func: Callable[[ConfigModelT], dict[str, Any]],
     cls: type[ConfigModelT] | None = None,
 ) -> type[ConfigModelT] | Any:
     """
@@ -1680,29 +1687,64 @@
         super()._init_private_attributes()
         local = contextvars.copy_context()
         setattr(self, LOCAL, local)
         tok = getattr(self, TOKEN, None)
         if tok:
             current_context.reset(tok)
 
+    def export(self, **kwargs: Any) -> dict[str, Any]:
+        """
+        Export the configuration model.
+
+        Returns
+        -------
+        The exported configuration model.
+        """
+        tok = _exporting.set(True)  # noqa: FBT003
+        ctx = contextvars.copy_context()
+        _exporting.reset(tok)
+        return ctx.run(self.dict, **kwargs)
+
+
     @no_type_check
     def _iter(self, **kwargs: Any) -> Generator[tuple[str, Any], None, None]:
-        if kwargs.get("to_dict", False):  # and kwargs.get("preprocessing", True):
+        if kwargs.get("to_dict", False) and _exporting.get():
             state = {}
             for key, value in super()._iter(**kwargs):
                 state[key] = value
             metadata = getattr(self, EXPORT, None)
             if metadata:
                 context = get_context(self)
                 context.manager.processor_class.export(state, metadata=metadata)
             yield from state.items()
         else:
             yield from super()._iter(**kwargs)
 
     @classmethod
+    @no_type_check
+    def _get_value(
+        cls,
+        value: Any,
+        *,
+        to_dict: bool,
+        **kwds: Any
+    ) -> Any:
+        if _exporting.get():
+            exporter = export.dispatch(type(value))
+            if (
+                isinstance(value, BaseModel)
+                or exporter != export.dispatch(object)
+            ) and to_dict:
+                value_dict = export(value, **kwds)
+                if ROOT_KEY in value_dict:
+                    return value_dict[ROOT_KEY]
+                return value_dict
+        return super()._get_value(value, to_dict=to_dict, **kwds)
+
+    @classmethod
     def _resolve_manager(
         cls,
         resource: ConfigManager[ConfigModelT] | RawResourceT | None = None,
         *,
         create_if_missing: bool | None = None,
     ) -> ConfigManager[ConfigModelT]:
         if resource is None:
@@ -1978,15 +2020,18 @@
         -------
         The number of bytes written.
         """
         context = get_context(self)
         if context.owner is self:
             if write_kwargs is None:
                 write_kwargs = {}
-            blob = context.manager.dump_config(self, **kwargs)
+            tok = _exporting.set(True)  # noqa: FBT003
+            ctx = contextvars.copy_context()
+            _exporting.reset(tok)
+            blob = ctx.run(context.manager.dump_config, self, **kwargs)
             result = await self.write_async(blob, **write_kwargs)
             context.initial_state = self.__dict__
             return result
         return await save_async(
             cast(ConfigAt[ConfigModelT], context.at),
             write_kwargs=write_kwargs,
             **kwargs,
```

### Comparing `configzen-0.1.47/configzen/errors.py` & `configzen-0.2.0/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.47/configzen/processor.py` & `configzen-0.2.0/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.47/configzen/typedefs.py` & `configzen-0.2.0/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.47/LICENSE` & `configzen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.47/pyproject.toml` & `configzen-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.47"
+version = "0.2.0"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.1.47/README.md` & `configzen-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.47/PKG-INFO` & `configzen-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.47
+Version: 0.2.0
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

