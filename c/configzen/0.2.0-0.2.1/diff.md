# Comparing `tmp/configzen-0.2.0.tar.gz` & `tmp/configzen-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.2.0.tar", max compression
+gzip compressed data, was "configzen-0.2.1.tar", max compression
```

## Comparing `configzen-0.2.0.tar` & `configzen-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.0/configzen/__init__.py
--rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.0/configzen/__main__.py
--rw-r--r--   0        0        0    60597 2023-05-30 13:45:42.424136 configzen-0.2.0/configzen/config.py
--rw-r--r--   0        0        0     2553 2023-05-30 00:29:12.193684 configzen-0.2.0/configzen/errors.py
--rw-r--r--   0        0        0    20820 2023-05-30 00:45:02.555346 configzen-0.2.0/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.0/configzen/py.typed
--rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.2.0/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.0/LICENSE
--rw-r--r--   0        0        0     1154 2023-05-30 13:46:45.360908 configzen-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7326 2023-05-30 00:29:12.142683 configzen-0.2.0/README.md
--rw-r--r--   0        0        0     7851 1970-01-01 00:00:00.000000 configzen-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.1/configzen/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.1/configzen/__main__.py
+-rw-r--r--   0        0        0    60674 2023-05-30 13:51:47.402579 configzen-0.2.1/configzen/config.py
+-rw-r--r--   0        0        0     2553 2023-05-30 00:29:12.193684 configzen-0.2.1/configzen/errors.py
+-rw-r--r--   0        0        0    20820 2023-05-30 00:45:02.555346 configzen-0.2.1/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.1/configzen/py.typed
+-rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.2.1/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1154 2023-05-30 13:52:50.177583 configzen-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7326 2023-05-30 00:29:12.142683 configzen-0.2.1/README.md
+-rw-r--r--   0        0        0     7851 1970-01-01 00:00:00.000000 configzen-0.2.1/PKG-INFO
```

### Comparing `configzen-0.2.0/configzen/__main__.py` & `configzen-0.2.1/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.0/configzen/config.py` & `configzen-0.2.1/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 import dataclasses
 import functools
 import io
 import os
 import pathlib
 import urllib.parse
 import urllib.request
-from collections.abc import Callable, Generator
 from typing import (
     Any,
     ClassVar,
     Generic,
     Literal,
     Optional,
     cast,
@@ -204,15 +203,15 @@
 
 
 for obj_type, encoder in ENCODERS_BY_TYPE.items():
     pre_serialize.register(obj_type, encoder)
 
 
 def with_pre_serialize(
-    func: Callable[[T], Any], cls: type[T] | None = None
+    func: collections.abc.Callable[[T], Any], cls: type[T] | None = None
 ) -> type[T] | Any:
     """
     Register a pre-serialization converter function for a type.
 
     Parameters
     ----------
     func
@@ -238,15 +237,17 @@
     if cls is None:
         return functools.partial(with_pre_serialize, func)
 
     pre_serialize.register(cls, func)
 
     if not hasattr(cls, "__get_validators__"):
 
-        def validator_gen() -> Generator[Callable[[Any], Any], None, None]:
+        def validator_gen() -> (
+            collections.abc.Generator[collections.abc.Callable[[Any], Any], None, None]
+        ):
             yield lambda value: post_deserialize.dispatch(cls)(cls, value)
 
         cls.__get_validators__ = validator_gen  # type: ignore[attr-defined]
 
     return cls
 
 
@@ -273,15 +274,15 @@
     """
     if isinstance(value, cls):
         return value
     return cls(value)
 
 
 def with_post_deserialize(
-    func: Callable[[Any], T], cls: type[T] | None = None
+    func: collections.abc.Callable[[Any], T], cls: type[T] | None = None
 ) -> type[T] | Any:
     """
     Register a loader function for a type.
 
     Parameters
     ----------
     func
@@ -314,15 +315,15 @@
     """
     if isinstance(obj, ConfigModel) and not _exporting.get():
         return obj.export(**kwargs)
     return cast(dict[str, Any], obj.dict(**kwargs))
 
 
 def with_exporter(
-    func: Callable[[ConfigModelT], dict[str, Any]],
+    func: collections.abc.Callable[[ConfigModelT], dict[str, Any]],
     cls: type[ConfigModelT] | None = None,
 ) -> type[ConfigModelT] | Any:
     """
     Register a custom exporter for a type.
 
     Parameters
     ----------
@@ -1088,22 +1089,22 @@
         if isinstance(other, list):
             return self.list_route == other
         return NotImplemented
 
     def __str__(self) -> str:
         return self.compose()
 
-    def __iter__(self) -> Generator[str, None, None]:
+    def __iter__(self) -> collections.abc.Generator[str, None, None]:
         yield from self.list_route
 
 
 def at(
     mapping: Any,
     route: SupportsRoute,
-    converter_func: Callable[[Any], dict[str, Any]] = _vars,
+    converter_func: collections.abc.Callable[[Any], dict[str, Any]] = _vars,
     manager: ConfigManager[ConfigModelT] | None = None,
 ) -> Any:
     """
     Get an item at a route.
 
     Parameters
     ----------
@@ -1616,15 +1617,17 @@
     The context of the configuration model.
     """
     return cast(
         Optional[BaseContext[ConfigModelT]], getattr(config, LOCAL).get(current_context)
     )
 
 
-def _json_encoder(model_encoder: Callable[..., Any], value: Any, **kwargs: Any) -> Any:
+def _json_encoder(
+    model_encoder: collections.abc.Callable[..., Any], value: Any, **kwargs: Any
+) -> Any:
     initial_state_type = type(value)
     converted_value = pre_serialize(value)
     if isinstance(converted_value, initial_state_type):
         return model_encoder(value, **kwargs)
     return converted_value
 
 
@@ -1700,43 +1703,37 @@
         The exported configuration model.
         """
         tok = _exporting.set(True)  # noqa: FBT003
         ctx = contextvars.copy_context()
         _exporting.reset(tok)
         return ctx.run(self.dict, **kwargs)
 
-
     @no_type_check
-    def _iter(self, **kwargs: Any) -> Generator[tuple[str, Any], None, None]:
+    def _iter(
+        self, **kwargs: Any
+    ) -> collections.abc.Generator[tuple[str, Any], None, None]:
         if kwargs.get("to_dict", False) and _exporting.get():
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
     @no_type_check
-    def _get_value(
-        cls,
-        value: Any,
-        *,
-        to_dict: bool,
-        **kwds: Any
-    ) -> Any:
+    def _get_value(cls, value: Any, *, to_dict: bool, **kwds: Any) -> Any:
         if _exporting.get():
             exporter = export.dispatch(type(value))
             if (
-                isinstance(value, BaseModel)
-                or exporter != export.dispatch(object)
+                isinstance(value, BaseModel) or exporter != export.dispatch(object)
             ) and to_dict:
                 value_dict = export(value, **kwds)
                 if ROOT_KEY in value_dict:
                     return value_dict[ROOT_KEY]
                 return value_dict
         return super()._get_value(value, to_dict=to_dict, **kwds)
```

### Comparing `configzen-0.2.0/configzen/errors.py` & `configzen-0.2.1/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.0/configzen/processor.py` & `configzen-0.2.1/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.0/configzen/typedefs.py` & `configzen-0.2.1/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.0/LICENSE` & `configzen-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.2.0/pyproject.toml` & `configzen-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.2.0"
+version = "0.2.1"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.2.0/README.md` & `configzen-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.2.0/PKG-INFO` & `configzen-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.2.0
+Version: 0.2.1
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

