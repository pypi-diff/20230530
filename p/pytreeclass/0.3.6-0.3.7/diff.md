# Comparing `tmp/pytreeclass-0.3.6.tar.gz` & `tmp/pytreeclass-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.3.6.tar", last modified: Thu May 18 18:30:40 2023, max compression
+gzip compressed data, was "pytreeclass-0.3.7.tar", last modified: Tue May 30 07:07:32 2023, max compression
```

## Comparing `pytreeclass-0.3.6.tar` & `pytreeclass-0.3.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:40.929109 pytreeclass-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-18 18:30:40.929109 pytreeclass-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:40.925109 pytreeclass-0.3.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:40.925109 pytreeclass-0.3.6/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:40.925109 pytreeclass-0.3.6/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/pytreeclass/_src/code_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    19804 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/pytreeclass/_src/tree_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28722 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/pytreeclass/_src/tree_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:40.925109 pytreeclass-0.3.6/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-18 18:30:40.000000 pytreeclass-0.3.6/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-18 18:30:40.000000 pytreeclass-0.3.6/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:30:40.000000 pytreeclass-0.3.6/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:30:40.000000 pytreeclass-0.3.6/pytreeclass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 18:30:40.000000 pytreeclass-0.3.6/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 18:30:40.000000 pytreeclass-0.3.6/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 18:30:40.929109 pytreeclass-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:40.929109 pytreeclass-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:32.940313 pytreeclass-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-30 07:07:32.940313 pytreeclass-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:32.936313 pytreeclass-0.3.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:32.936313 pytreeclass-0.3.7/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:32.940313 pytreeclass-0.3.7/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/pytreeclass/_src/code_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19808 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/pytreeclass/_src/tree_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26343 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27290 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/pytreeclass/_src/tree_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:32.936313 pytreeclass-0.3.7/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-30 07:07:32.000000 pytreeclass-0.3.7/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-30 07:07:32.000000 pytreeclass-0.3.7/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 07:07:32.000000 pytreeclass-0.3.7/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 07:07:32.000000 pytreeclass-0.3.7/pytreeclass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 07:07:32.000000 pytreeclass-0.3.7/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 07:07:32.000000 pytreeclass-0.3.7/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 07:07:32.940313 pytreeclass-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:32.940313 pytreeclass-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17765 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.3.6/LICENSE` & `pytreeclass-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.6/PKG-INFO` & `pytreeclass-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.3.6
+Version: 0.3.7
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytreeclass-0.3.6/README.md` & `pytreeclass-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.6/docs/conf.py` & `pytreeclass-0.3.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.6/pytreeclass/__init__.py` & `pytreeclass-0.3.7/pytreeclass/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,8 +46,12 @@
     "tree_map_with_trace",
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
     "Partial",
 )
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
+
+AtIndexer.__module__ = "pytreeclass"
+TreeClass.__module__ = "pytreeclass"
+Partial.__module__ = "pytreeclass"
```

### Comparing `pytreeclass-0.3.6/pytreeclass/_src/__init__.py` & `pytreeclass-0.3.7/pytreeclass/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.6/pytreeclass/_src/code_build.py` & `pytreeclass-0.3.7/pytreeclass/_src/code_build.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.6/pytreeclass/_src/tree_base.py` & `pytreeclass-0.3.7/pytreeclass/_src/tree_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             return AtIndexer(self.tree, (*self.where, where))
 
         raise NotImplementedError(
             f"Indexing with {type(where).__name__} is not implemented.\n"
             "Example of supported indexing:\n\n"
             ">>> import jax\n"
             ">>> import pytreeclass as pytc\n"
-            f"class {type(self.tree).__name__}:(pytc.TreeClass)\n"
+            f"class {type(self.tree).__name__}(pytc.TreeClass):\n"
             "    ...\n\n"
             f">>> tree = {type(self.tree).__name__}(...)\n"
             ">>> # indexing by boolean pytree\n"
             ">>> mask = jax.tree_map(lambda x: x > 0, tree)\n"
             ">>> tree.at[mask].get()\n\n"
             ">>> # indexing by attribute name\n"
             ">>> tree.at[`attribute_name`].get()\n\n"
@@ -482,16 +482,16 @@
             Set the `value` and return a new instance with the updated value.
         - `.at[***].apply(func)`:
             Apply a `func` and return a new instance with the updated value.
         - `.at['method'](*a, **k)`:
             Call a `method` and return a (return value, new instance) tuple.
 
         `***` acceptable index types are `str` for mapping keys or
-        class attributes, `int` for positional indexing, `...` for all leaves,
-        and a boolean mask of the same structure as the tree.
+        class attributes, `int` for positional indexing, `...` to select all leaves,
+        , a boolean mask of the same structure as the tree.
 
         Example:
             >>> import pytreeclass as pytc
             >>> class Tree(pytc.TreeClass):
             ...     a:int = 1
             ...     b:float = 2.0
             ...     def add(self, x:int) -> int:
```

### Comparing `pytreeclass-0.3.6/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.3.7/pytreeclass/_src/tree_pprint.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,135 +14,135 @@
 
 from __future__ import annotations
 
 import dataclasses as dc
 import functools as ft
 import inspect
 import math
+from collections.abc import MutableMapping, MutableSequence
 from itertools import chain
 from types import FunctionType
-from typing import Any, Callable, Literal
+from typing import Any, Callable, Iterable, Literal
 
 import jax
 import jax.tree_util as jtu
 import numpy as np
 from jax import custom_jvp
 from jax.util import unzip2
-from jaxlib.xla_extension import PjitFunction
+from typing_extensions import TypedDict, Unpack
 
 from pytreeclass._src.tree_util import (
     IsLeafType,
     Node,
     construct_tree,
     tree_leaves_with_trace,
     tree_map_with_trace,
 )
 
+
+class PPSpec(TypedDict):
+    indent: int
+    kind: Literal["REPR", "STR"]
+    width: int
+    depth: int | float
+
+
 PyTree = Any
-PrintKind = Literal["repr", "str"]
+PP = Callable[[Any, Unpack[PPSpec]], str]
+ORDER_KEY = ["B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB"]
 from_iterable = chain.from_iterable
 
 
-def _node_pprint(
-    node: Any,
-    *,
-    indent: int,
-    kind: PrintKind,
-    width: int,
-    depth: int | float,
-) -> str:
-    if depth < 0:
+def pp(node: Any, **spec: Unpack[PPSpec]) -> str:
+    if spec["depth"] < 0:
         return "..."
 
-    # avoid circular import by importing Partial here
+    # avoid circular import by importing
     from pytreeclass import TreeClass
 
-    spec = dict(indent=indent, kind=kind, width=width, depth=depth)
-
     if isinstance(node, ft.partial):
-        text = f"Partial({_func_pprint(node.func, **spec)})"
+        text = f"Partial({func_pp(node.func, **spec)})"
     elif isinstance(node, (FunctionType, custom_jvp)):
-        text = _func_pprint(node, **spec)
-    elif isinstance(node, PjitFunction):
-        text = f"jit({_func_pprint(node, **spec)})"
+        text = func_pp(node, **spec)
     elif isinstance(node, jax.ShapeDtypeStruct):
-        text = _shape_dtype_pprint(node, **spec)
+        text = shape_dtype_pp(node, **spec)
     elif isinstance(node, tuple) and hasattr(node, "_fields"):
-        text = _namedtuple_pprint(node, **spec)
-    elif isinstance(node, list):
-        text = _list_pprint(node, **spec)
+        text = namedtuple_pp(node, **spec)
+    elif isinstance(node, MutableSequence):
+        text = list_pp(node, **spec)
     elif isinstance(node, tuple):
-        text = _tuple_pprint(node, **spec)
+        text = tuple_pp(node, **spec)
     elif isinstance(node, set):
-        text = _set_pprint(node, **spec)
-    elif isinstance(node, dict):
-        text = _dict_pprint(node, **spec)
+        text = set_pp(node, **spec)
+    elif isinstance(node, MutableMapping):
+        text = dict_pp(node, **spec)
     elif dc.is_dataclass(node):
-        text = _dataclass_pprint(node, **spec)
+        text = dataclass_pp(node, **spec)
     elif isinstance(node, TreeClass):
-        text = _treeclass_pprint(node, **spec)
-    elif isinstance(node, (np.ndarray, jax.Array)) and kind == "repr":
-        text = _numpy_pprint(node, **spec)
+        text = treeclass_pp(node, **spec)
+    elif isinstance(node, (np.ndarray, jax.Array)) and spec["kind"] == "REPR":
+        text = numpy_pp(node, **spec)
     else:
-        text = _general_pprint(node, **spec)
+        text = general_pp(node, **spec)
 
-    return _format_width(text, width)
+    return format_width(text, width=spec["width"])
 
 
-def _general_pprint(
-    node: Any,
-    *,
-    indent: int,
-    kind: PrintKind,
-    width: int,
-    depth: int,
-) -> str:
-    del depth, width
+def pps(xs: Iterable[Any], pp: PP, **spec: Unpack[PPSpec]) -> str:
+    if spec["depth"] == 0:
+        return "..."
 
-    text = f"{node!r}" if kind == "repr" else f"{node!s}"
-    is_mutltiline = "\n" in text
-    indent = (indent + 1) if is_mutltiline else indent
-    text = ("\n" + "\t" * indent).join(text.split("\n"))
-    text = ("\n" + "\t" * (indent) + text) if is_mutltiline else text
-    return text
+    spec["indent"] += 1
+    spec["depth"] -= 1
 
+    text = (
+        "\n"
+        + "\t" * spec["indent"]
+        + (", \n" + "\t" * spec["indent"]).join(pp(x, **spec) for x in xs)
+        + "\n"
+        + "\t" * (spec["indent"] - 1)
+    )
+
+    return format_width(text, width=spec["width"])
+
+
+def key_value_pp(x: tuple[str, Any], **spec: Unpack[PPSpec]) -> str:
+    return f"{x[0]}:{pp(x[1], **spec)}"
 
-def _shape_dtype_pprint(
-    node: Any,
-    *,
-    indent: int,
-    kind: PrintKind,
-    width: int,
-    depth: int,
-) -> str:
-    """Pretty print a node with dtype and shape"""
-    del indent, kind, depth, width
 
+def attr_value_pp(x: tuple[str, Any], **spec: Unpack[PPSpec]) -> str:
+    return f"{x[0]}={pp(x[1], **spec)}"
+
+
+def general_pp(node: Any, **spec: Unpack[PPSpec]) -> str:
+    text = f"{node!r}" if spec["kind"] == "REPR" else f"{node!s}"
+
+    if "\n" not in text:
+        return text
+
+    indent = spec["indent"] + 1
+    return "\n" + "\t" * indent + ("\n" + "\t" * indent).join(text.split("\n"))
+
+
+def shape_dtype_pp(node: Any, **spec: Unpack[PPSpec]) -> str:
+    """Pretty print a node with dtype and shape"""
     shape = f"{node.shape}".replace(",", "")
     shape = shape.replace("(", "[")
     shape = shape.replace(")", "]")
     shape = shape.replace(" ", ",")
     dtype = f"{node.dtype}".replace("int", "i")
     dtype = dtype.replace("float", "f")
     dtype = dtype.replace("complex", "c")
     return dtype + shape
 
 
-def _numpy_pprint(
-    node: np.ndarray | jax.Array,
-    *,
-    indent: int,
-    kind: PrintKind,
-    width: int,
-    depth: int,
-) -> str:
+def numpy_pp(node: np.ndarray | jax.Array, **spec: Unpack[PPSpec]) -> str:
     """Replace np.ndarray repr with short hand notation for type and shape"""
-    spec = dict(indent=indent, kind=kind, width=width, depth=depth)
 
-    base = _shape_dtype_pprint(node, **spec)
+    base = shape_dtype_pp(node, **spec)
 
     if not issubclass(node.dtype.type, (np.integer, np.floating)) or node.size == 0:
         return base
 
     # Extended repr for numpy array, with extended information
     # this part of the function is inspired by
     # lovely-jax https://github.com/xl0/lovely-jax
@@ -150,199 +150,90 @@
     # handle interval
     low, high = np.min(node), np.max(node)
     interval = "(" if math.isinf(low) else "["
     is_integer = issubclass(node.dtype.type, np.integer)
     interval += f"{low},{high}" if is_integer else f"{low:.2f},{high:.2f}"
     interval += ")" if math.isinf(high) else "]"  # resolve closed/open interval
     interval = interval.replace("inf", "∞")  # replace inf with infinity symbol
-
     # handle mean and std
     mean, std = f"{np.mean(node):.2f}", f"{np.std(node):.2f}"
 
     return f"{base}(μ={mean}, σ={std}, ∈{interval})"
 
 
-def _func_pprint(
-    func: Callable,
-    *,
-    indent: int,
-    kind: PrintKind,
-    width: int,
-    depth: int,
-) -> str:
+def func_pp(func: Callable, **spec: Unpack[PPSpec]) -> str:
     # Pretty print function
     # Example:
     #     >>> def example(a: int, b=1, *c, d, e=2, **f) -> str:
     #         ...
-    #     >>> _func_pprint(example)
+    #     >>> func_pp(example)
     #     "example(a, b, *c, d, e, **f)"
-    del indent, kind, depth, width
+    del spec
     args, varargs, varkw, _, kwonlyargs, _, _ = inspect.getfullargspec(func)
     args = (", ".join(args)) if len(args) > 0 else ""
     varargs = ("*" + varargs) if varargs is not None else ""
     kwonlyargs = (", ".join(kwonlyargs)) if len(kwonlyargs) > 0 else ""
     varkw = ("**" + varkw) if varkw is not None else ""
-    name = "Lambda" if (func.__name__ == "<lambda>") else func.__name__
+    name = getattr(func, "__name__", "")
     text = f"{name}("
     text += ", ".join(item for item in [args, varargs, kwonlyargs, varkw] if item != "")
     text += ")"
     return text
 
 
-def _list_pprint(
-    node: list,
-    *,
-    indent: int,
-    kind: PrintKind,
-    width: int,
-    depth: int,
-) -> str:
-    if depth == 0:
-        return "[...]"
-    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
-    text = (f"{(_node_pprint(v,**spec))}" for v in node)
-    text = (", \n" + "\t" * (indent + 1)).join(text)
-    text = "[\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + "]"
-    return text
+def list_pp(node: list, **spec: Unpack[PPSpec]) -> str:
+    return "[" + pps(node, pp=pp, **spec) + "]"
 
 
-def _tuple_pprint(
-    node: tuple,
-    *,
-    indent: int,
-    kind: PrintKind,
-    width: int,
-    depth: int,
-) -> str:
-    if depth == 0:
-        return "(...)"
-    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
-    text = (f"{(_node_pprint(v,**spec))}" for v in node)
-    text = (", \n" + "\t" * (indent + 1)).join(text)
-    text = "(\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + ")"
-    return text
+def tuple_pp(node: tuple, **spec) -> str:
+    return "(" + pps(node, pp=pp, **spec) + ")"
 
 
-def _set_pprint(
-    node: set,
-    *,
-    indent: int,
-    kind: PrintKind,
-    width: int,
-    depth: int,
-) -> str:
-    if depth == 0:
-        return "{...}"
-    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
-    text = (f"{(_node_pprint(v,**spec))}" for v in node)
-    text = (", \n" + "\t" * (indent + 1)).join(text)
-    text = "{\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + "}"
-    return text
+def set_pp(node: set, **spec: Unpack[PPSpec]) -> str:
+    return "{" + pps(node, pp=pp, **spec) + "}"
 
 
-def _dict_pprint(
-    node: dict,
-    *,
-    indent: int,
-    kind: PrintKind,
-    width: int,
-    depth: int,
-) -> str:
-    if depth == 0:
-        return "{...}"
-    kvs = node.items()
-    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
-    text = (f"{k}:{_node_pprint(v,**spec)}" for k, v in kvs)
-    text = (", \n" + "\t" * (indent + 1)).join(text)
-    text = "{\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + "}"
-    return text
+def dict_pp(node: dict, **spec: Unpack[PPSpec]) -> str:
+    return "{" + pps(node.items(), pp=key_value_pp, **spec) + "}"
 
 
-def _namedtuple_pprint(
-    node: Any,
-    *,
-    indent: int,
-    kind: PrintKind,
-    width: int,
-    depth: int,
-) -> str:
+def namedtuple_pp(node: Any, **spec: Unpack[PPSpec]) -> str:
     name = type(node).__name__
-
-    if depth == 0:
-        return f"{name}(...)"
-
     kvs = node._asdict().items()
-    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
-    text = (f"{k}={_node_pprint(v,**spec)}" for k, v in kvs)
-    text = (", \n" + "\t" * (indent + 1)).join(text)
-    name = type(node).__name__
-    text = f"{name}(\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + ")"
-    return text
+    return name + "(" + pps(kvs, pp=attr_value_pp, **spec) + ")"
 
 
-def _dataclass_pprint(
-    node: Any,
-    *,
-    indent: int,
-    kind: PrintKind,
-    width: int,
-    depth: int,
-) -> str:
+def dataclass_pp(node: Any, **spec: Unpack[PPSpec]) -> str:
     name = type(node).__name__
-
-    if depth == 0:
-        return f"{name}(...)"
-
     kvs = ((f.name, vars(node)[f.name]) for f in dc.fields(node) if f.repr)
-    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
-    text = (f"{k}={_node_pprint(v,**spec)}" for k, v in kvs)
-    text = (", \n" + "\t" * (indent + 1)).join(text)
-    text = f"{name}(\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + ")"
-    return text
+    return name + "(" + pps(kvs, pp=attr_value_pp, **spec) + ")"
 
 
-def _treeclass_pprint(
-    node: Any,
-    *,
-    indent: int,
-    kind: PrintKind,
-    width: int,
-    depth: int,
-) -> str:
-    name = type(node).__name__
-    if depth == 0:
-        return f"{name}(...)"
-
+def treeclass_pp(node: Any, **spec: Unpack[PPSpec]) -> str:
     # avoid circular import by importing here
     from pytreeclass import fields
 
+    name = type(node).__name__
     skip = [f.name for f in fields(node) if not f.repr]
     kvs = ((k, v) for k, v in vars(node).items() if k not in skip)
-    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
-    text = (f"{k}={_node_pprint(v,**spec)}" for k, v in kvs)
-    text = (", \n" + "\t" * (indent + 1)).join(text)
-    text = f"{name}(\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + ")"
-    return text
+    return name + "(" + pps(kvs, pp=attr_value_pp, **spec) + ")"
 
 
-def _node_type_pprint(
-    node: jax.Array | np.ndarray,
-    *,
-    indent: int,
-    kind: PrintKind,
-    width: int,
-    depth: int,
-) -> str:
-    if isinstance(node, (jax.Array, np.ndarray)):
-        shape_dype = node.shape, node.dtype
-        spec = dict(indent=indent, kind=kind, width=width, depth=depth)
-        text = _node_pprint(jax.ShapeDtypeStruct(*shape_dype), **spec)
-    else:
-        text = f"{type(node).__name__}"
-    return text
+def type_pp(node: Any, **spec: Unpack[PPSpec]) -> str:
+    if not isinstance(node, (jax.Array, np.ndarray)):
+        return f"{type(node).__name__}"
+
+    shape_dype = node.shape, node.dtype
+    return pp(jax.ShapeDtypeStruct(*shape_dype), **spec)
+
+
+def size_pp(size: int, **spec: Unpack[PPSpec]):
+    size_order = int(math.log(size, 1024)) if size > 0 else 0
+    text = f"{(size)/(1024**size_order):.2f}{ORDER_KEY[size_order]}"
+    return pp(text, **spec)
 
 
 def tree_repr(
     tree: PyTree,
     *,
     width: int = 80,
     tabwidth: int = 2,
@@ -366,15 +257,15 @@
 
         >>> print(pytc.tree_repr(tree, depth=1))
         {a:1, b:[...], c:{...}, f:i32[2](μ=6.50, σ=0.50, ∈[6,7])}
 
         >>> print(pytc.tree_repr(tree, depth=2))
         {a:1, b:[2, 3], c:{d:4, e:5}, f:i32[2](μ=6.50, σ=0.50, ∈[6,7])}
     """
-    text = _node_pprint(tree, indent=0, kind="repr", width=width, depth=depth)
+    text = pp(tree, indent=0, kind="REPR", width=width, depth=depth)
     return text.expandtabs(tabwidth)
 
 
 def tree_str(
     tree: PyTree,
     *,
     width: int = 80,
@@ -395,15 +286,15 @@
 
         >>> print(pytc.tree_str(tree, depth=1))
         {a:1, b:[...], c:{...}, f:[6 7]}
 
         >>> print(pytc.tree_str(tree, depth=2))
         {a:1, b:[2, 3], c:{d:4, e:5}, f:[6 7]}
     """
-    text = _node_pprint(tree, indent=0, kind="str", width=width, depth=depth)
+    text = pp(tree, indent=0, kind="STR", width=width, depth=depth)
     return text.expandtabs(tabwidth)
 
 
 def _is_trace_leaf_depth_factory(depth: int | float):
     # generate `is_trace_leaf` function to stop tracing at a certain `depth`
     # in essence, depth is the length of the trace entry
     def is_trace_leaf(trace) -> bool:
@@ -425,15 +316,16 @@
 ):
     """Returns a string representation of the tree with indentation.
 
     Args:
         tree: The tree to be printed.
         depth: The maximum depth of the tree to be printed.
         is_leaf: A function that takes a node and returns True if it is a leaf node.
-        tabwidth: The number of spaces per indentation level. if `None` then tabs are not expanded.
+        tabwidth: The number of spaces per indentation level. if `None`
+            then tabs are not expanded.
 
     Example:
         >>> import pytreeclass as pytc
         >>> tree = [1, [2, 3], [4, [5, 6]]]
         >>> print(pytc.tree_indent(tree))
         list
             [0]=1
@@ -449,19 +341,19 @@
     """
     smark = (" \t")[:tabwidth]  # space mark
 
     def step(node: Node, depth: int = 0) -> str:
         indent = smark * depth
 
         if (len(node.children)) == 0:
-            ppspec = dict(indent=0, kind="repr", width=80, depth=0)
+            ppspec = dict(indent=0, kind="REPR", width=80, depth=0)
             text = f"{indent}"
             (key, _), value = node.data
             text += f"{key}=" if key is not None else ""
-            text += _node_pprint(value, **ppspec)
+            text += pp(value, **ppspec)
             return text + "\n"
 
         (key, type), _ = node.data
         text = f"{indent}"
         text += f"{key}:" if key is not None else ""
         text += f"{type.__name__}\n"
 
@@ -531,19 +423,19 @@
         is_last: bool = False,
         is_lasts: tuple[bool, ...] = (),
     ) -> str:
         indent = "".join(smark if is_last else vmark for is_last in is_lasts[:-1])
         branch = (lmark if is_last else cmark) if depth > 0 else ""
 
         if (child_count := len(node.children)) == 0:
-            ppspec = dict(indent=0, kind="repr", width=80, depth=0)
+            ppspec = dict(indent=0, kind="REPR", width=80, depth=0)
             (key, _), value = node.data
             text = f"{indent}"
             text += f"{branch}{key}=" if key is not None else ""
-            text += _node_pprint(value, **ppspec)
+            text += pp(value, **ppspec)
             return text + "\n"
 
         (key, type), _ = node.data
 
         text = f"{indent}{branch}"
         text += f"{key}:" if key is not None else ""
         text += f"{type.__name__}\n"
@@ -578,18 +470,18 @@
         tree: PyTree
         depth: depth of the tree to print. default is max depth
         is_leaf: function to determine if a node is a leaf. default is None
     """
 
     def step(node: Node, depth: int = 0) -> str:
         if len(node.children) == 0:
-            ppspec = dict(indent=0, kind="repr", width=80, depth=0)
+            ppspec = dict(indent=0, kind="REPR", width=80, depth=0)
             key, _, value = node.data
             text = f"{key}=" if key is not None else ""
-            text += _node_pprint(value, **ppspec)
+            text += pp(value, **ppspec)
             text = "<b>" + text + "</b>"
             return f'\tid{id(node.parent)} --- id{id(node)}("{text}")\n'
 
         key, type, _ = node.data
         text = f"{key}:" if key is not None else ""
         text += f"{type.__name__}"
         text = "<b>" + text + "</b>"
@@ -609,15 +501,15 @@
         is_trace_leaf=_is_trace_leaf_depth_factory(depth),
     )
     text = "flowchart LR\n" + step(root)
 
     return (text.expandtabs(tabwidth) if tabwidth is not None else text).rstrip()
 
 
-def _format_width(string, width=60):
+def format_width(string, width=60):
     """strip newline/tab characters if less than max width"""
     children_length = len(string) - string.count("\n") - string.count("\t")
     if children_length > width:
         return string
     return string.replace("\n", "").replace("\t", "")
 
 
@@ -850,23 +742,22 @@
 
         if trace == ((), ()):
             # avoid printing the leaf trace (which is the root of the tree)
             # twice, once as a leaf and once as the root at the end
             continue
 
         paths = jtu.keystr(trace[0])
-        types = _node_type_pprint(leaf, indent=0, kind="str", width=60, depth=depth)
+        types = type_pp(leaf, indent=0, kind="STR", width=60, depth=depth)
         counts = f"{count:,}"
         ROWS += [[paths, types, counts]]
 
     paths = "Σ"
-    types = _node_type_pprint(tree, indent=0, kind="str", width=60, depth=depth)
+    types = type_pp(tree, indent=0, kind="STR", width=60, depth=depth)
     counts = f"{COUNT:,}"
     ROWS += [[paths, types, counts]]
-
     return _table(ROWS)
 
 
 def tree_repr_with_trace(
     tree: PyTree,
     is_leaf: IsLeafType = None,
     transpose: bool = False,
```

### Comparing `pytreeclass-0.3.6/pytreeclass/_src/tree_util.py` & `pytreeclass-0.3.7/pytreeclass/_src/tree_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import dataclasses as dc
 import functools as ft
-import hashlib
 import operator as op
 from collections import defaultdict
 from math import ceil, floor, trunc
-from typing import Any, Callable, Hashable, Iterator, Sequence, Tuple, TypeVar, Union
+from typing import (
+    Any,
+    Callable,
+    Generic,
+    Hashable,
+    Iterator,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
 from jax._src.tree_util import _registry, _registry_with_keypaths
 from jax.util import unzip2
@@ -37,79 +46,52 @@
 TraceEntry = Tuple[KeyEntry, TypeEntry]
 KeyPath = Tuple[KeyEntry, ...]
 TypePath = Tuple[TypeEntry, ...]
 TraceType = Tuple[KeyPath, TypePath]
 IsLeafType = Union[type(None), Callable[[Any], bool]]
 
 
-def _hash_node(node: Any) -> int:
-    if isinstance(node, (jax.Array, np.ndarray)):
-        return int(hashlib.sha256(np.array(node).tobytes()).hexdigest(), 16)
-    if isinstance(node, set):
-        return hash(frozenset(node))
-    if isinstance(node, dict):
-        return hash(frozenset(node.items()))
-    if isinstance(node, list):
-        return hash(tuple(node))
-    return hash(node)
-
-
 def tree_hash(*trees: PyTree) -> int:
-    hashed = jtu.tree_map(_hash_node, jtu.tree_leaves(trees))
-    return hash((*hashed, jtu.tree_structure(trees)))
-
-
-class _ImmutableWrapper:
-    __slots__ = ("__wrapped__", "__weakref__")
-
-    def __init__(self, x: Any) -> None:
-        object.__setattr__(self, "__wrapped__", getattr(x, "__wrapped__", x))
-
-    def unwrap(self) -> Any:
-        return getattr(self, "__wrapped__")
-
-    def __setattr__(self, _, __) -> None:
-        raise AttributeError("Cannot assign to frozen instance.")
-
-    def __delattr__(self, _: str) -> None:
-        raise AttributeError("Cannot delete from frozen instance.")
-
-
-class _HashableWrapper(_ImmutableWrapper):
-    def __eq__(self, rhs: Any) -> bool:
-        if not isinstance(rhs, _HashableWrapper):
-            return False
-        return tree_hash(self.unwrap()) == tree_hash(rhs.unwrap())
-
-    def __hash__(self) -> int:
-        return tree_hash(self.unwrap())
+    leaves, treedef = jtu.tree_flatten(trees)
+    return hash((*leaves, treedef))
 
 
 def _frozen_error(opname: str, tree):
     raise NotImplementedError(
         f"Cannot apply `{opname}` operation to a frozen object `{tree!r}`.\n"
         "Unfreeze the object first to apply operations to it\n"
         "Example:\n"
         ">>> import jax\n"
         ">>> import pytreeclass as pytc\n"
         ">>> tree = jax.tree_map(pytc.unfreeze, tree, is_leaf=pytc.is_frozen)"
     )
 
 
-class _FrozenWrapper(_ImmutableWrapper):
+class _FrozenWrapper(Generic[T]):
+    __slots__ = ("__wrapped__", "__weakref__")
+
+    def __init__(self, x: T) -> None:
+        object.__setattr__(self, "__wrapped__", x)
+
+    def __setattr__(self, _, __) -> None:
+        raise AttributeError("Cannot assign to frozen instance.")
+
+    def __delattr__(self, _: str) -> None:
+        raise AttributeError("Cannot delete from frozen instance.")
+
     def __repr__(self):
-        return f"#{self.unwrap()!r}"
+        return f"#{self.__wrapped__!r}"
 
-    def __eq__(self, rhs: Any) -> bool:
+    def __eq__(self, rhs: Any) -> bool | jax.Array:
         if not isinstance(rhs, _FrozenWrapper):
             return False
-        return self.unwrap() == rhs.unwrap()
+        return is_tree_equal(self.__wrapped__, rhs.__wrapped__)
 
     def __hash__(self) -> int:
-        return tree_hash(self.unwrap())
+        return tree_hash(self.__wrapped__)
 
     # raise helpful error message when trying to interact with frozen object
     __add__ = __radd__ = __iadd__ = lambda x, _: _frozen_error("+", x)
     __sub__ = __rsub__ = __isub__ = lambda x, _: _frozen_error("-", x)
     __mul__ = __rmul__ = __imul__ = lambda x, _: _frozen_error("*", x)
     __matmul__ = __rmatmul__ = __imatmul__ = lambda x, _: _frozen_error("@", x)
     __truediv__ = __rtruediv__ = __itruediv__ = lambda x, _: _frozen_error("/", x)
@@ -123,21 +105,21 @@
     __or__ = __ror__ = __ior__ = lambda x, _: _frozen_error("or", x)
     __neg__ = __pos__ = __abs__ = __invert__ = lambda x: _frozen_error("unary op", x)
     __call__ = lambda x, *_, **__: _frozen_error("call", x)
 
 
 jtu.register_pytree_node(
     nodetype=_FrozenWrapper,
-    flatten_func=lambda tree: ((), _HashableWrapper(tree.unwrap())),
-    unflatten_func=lambda treedef, _: _FrozenWrapper(treedef.unwrap()),
+    flatten_func=lambda tree: ((), tree),
+    unflatten_func=lambda treedef, _: treedef,
 )
 
 
 def freeze(wrapped: Any) -> _FrozenWrapper:
-    r"""Freeze a value to avoid updating it by `jax` transformations.
+    """Freeze a value to avoid updating it by `jax` transformations.
 
     Example:
         >>> import jax
         >>> import pytreeclass as pytc
         >>> import jax.tree_util as jtu
         >>> # Usage with `jax.tree_util.tree_leaves`
         >>> # no leaves for a wrapped value
@@ -149,47 +131,24 @@
         [#2.0]
 
         >>> # Usage with `jax.tree_util.tree_map`
         >>> a= [1,2,3]
         >>> a[1] = pytc.freeze(a[1])
         >>> jtu.tree_map(lambda x:x+100, a)
         [101, #2, 103]
-
-        >>> class Test(pytc.TreeClass):
-        ...     a: float
-        ...     @jax.value_and_grad
-        ...     def __call__(self, x):
-        ...         # unfreeze `a` to update it
-        ...         self = jax.tree_map(pytc.unfreeze, self, is_leaf=pytc.is_frozen)
-        ...         return x ** self.a
-
-        >>> # without `freeze` wrapping `a`, `a` will be updated
-        >>> value, grad = Test(a = 2.)(2.)
-        >>> print(f"value: {value}\ngrad: {grad}")
-        value: 4.0
-        grad: Test(a=2.7725887)
-
-        >>> # with `freeze` wrapping `a`, `a` will NOT be updated
-        >>> value, grad = Test(a=pytc.freeze(2.))(2.)
-        >>> print(f"value: {value}\ngrad: {grad}")
-        value: 4.0
-        grad: Test(a=#2.0)
-
-        >>> # usage with `jax.tree_map` to freeze a tree
-        >>> tree = Test(a = 2.)
-        >>> frozen_tree = jax.tree_map(pytc.freeze, tree)
-        >>> value, grad = frozen_tree(2.)
-        >>> print(f"value: {value}\ngrad: {grad}")
-        value: 4.0
-        grad: Test(a=#2.0)
     """
-    return _FrozenWrapper(wrapped)
+    return wrapped if is_frozen(wrapped) else _FrozenWrapper(wrapped)
+
+
+def is_frozen(wrapped: Any) -> bool:
+    """Returns True if the value is a frozen wrapper."""
+    return isinstance(wrapped, _FrozenWrapper)
 
 
-def unfreeze(x: Any) -> Any:
+def unfreeze(wrapped: Any) -> Any:
     """Unfreeze `frozen` value, otherwise return the value itself.
 
     - use `is_leaf=pytc.is_frozen` with `jax.tree_map` to unfreeze a tree.**
 
     Example:
         >>> import pytreeclass as pytc
         >>> import jax
@@ -198,23 +157,18 @@
         1
         >>> # usage with `jax.tree_map`
         >>> frozen_tree = jax.tree_map(pytc.freeze, {"a": 1, "b": 2})
         >>> unfrozen_tree = jax.tree_map(pytc.unfreeze, frozen_tree, is_leaf=pytc.is_frozen)
         >>> unfrozen_tree
         {'a': 1, 'b': 2}
     """
-    return x.unwrap() if isinstance(x, _FrozenWrapper) else x
-
-
-def is_frozen(wrapped: Any) -> bool:
-    """Returns True if the value is a frozen wrapper."""
-    return isinstance(wrapped, _FrozenWrapper)
+    return getattr(wrapped, "__wrapped__") if is_frozen(wrapped) else wrapped
 
 
-def is_nondiff(x: Any) -> bool:
+def is_nondiff(wrapped: Any) -> bool:
     """
     Returns True if the node is a non-differentiable node, and False for if the
     node is of type float, complex number, or a numpy array of floats or
     complex numbers.
 
     Example:
         >>> import pytreeclass as pytc
@@ -230,17 +184,17 @@
 
     Note:
         This function is meant to be used with `jax.tree_map` to
         create a mask for non-differentiable nodes in a tree, that can be used
         to freeze the non-differentiable nodes before passing the tree to a
         `jax` transformation.
     """
-    if hasattr(x, "dtype") and np.issubdtype(x.dtype, np.inexact):
+    if hasattr(wrapped, "dtype") and np.issubdtype(wrapped.dtype, np.inexact):
         return False
-    if isinstance(x, (float, complex)):
+    if isinstance(wrapped, (float, complex)):
         return False
     return True
 
 
 def tree_copy(tree: T) -> T:
     """Return a copy of the tree."""
     leaves, treedef = jtu.tree_flatten(tree)
@@ -502,30 +456,31 @@
             setattr(klass, key, method)
     return klass
 
 
 def _is_leaf_rhs_equal(leaf, rhs) -> bool | jax.Array:
     if hasattr(leaf, "shape") and hasattr(leaf, "dtype"):
         if hasattr(rhs, "shape") and hasattr(rhs, "dtype"):
-            verdict = jnp.array_equal(leaf, rhs)
+            if leaf.shape != rhs.shape:
+                return False
+            if leaf.dtype != rhs.dtype:
+                return False
             try:
-                return bool(verdict)
+                return bool(verdict := jnp.all(leaf == rhs))
             except Exception:
                 return verdict  # fail under `jit`
         return False
     return leaf == rhs
 
 
 def is_tree_equal(*trees: Any) -> bool | jax.Array:
     """Return `True` if all pytrees are equal.
 
     Note:
         trees are compared using their leaves and treedefs.
-        For `array` leaves `jnp.array_equal` is used, for other leaves
-        method `__eq__` is used.
 
     Note:
         Under `jit` the return type is boolean `jax.Array` instead of `bool`.
     """
 
     tree0, *rest = trees
     leaves0, treedef0 = jtu.tree_flatten(tree0)
@@ -536,31 +491,31 @@
         if (treedef != treedef0) or verdict is False:
             return False
         verdict = ft.reduce(op.and_, map(_is_leaf_rhs_equal, leaves0, leaves), verdict)
     return verdict
 
 
 @dc.dataclass(frozen=True)
-class NamedSequenceKey:
-    idx: int
-    key: Hashable
-
+class NamedSequenceKey(jtu.GetAttrKey, jtu.SequenceKey):
+    # inherit from both `jtu.GetAttrKey` and `jtu.SequenceKey`
+    # in case the user perform isinstance check to unpack the name/index
+    # `TreeClass` is modeled as a `NamedTuple`` with both `name` and `idx` identifiers
     def __str__(self):
-        return f".{self.key}"
+        return f".{self.name}"
 
 
 # indexing matching registry
 # define rule for indexing matching through `at` property
 # for example, `jax` internals uses `jtu.GetAttrKey` to index an attribute,
 # however its not ergonomic to use `tree.at[jtu.GetAttrKey("attr")]`
 # to index an attribute instead `tree.at['attr']` is more ergonomic
 match_registry: dict[type, Callable] = defaultdict(lambda entry: (entry,))
 match_registry[jtu.GetAttrKey] = lambda entry: (entry.name,)
 match_registry[jtu.SequenceKey] = lambda entry: (entry.idx,)
-match_registry[NamedSequenceKey] = lambda entry: (entry.idx, entry.key)
+match_registry[NamedSequenceKey] = lambda entry: (entry.idx, entry.name)
 match_registry[jtu.DictKey] = lambda entry: (entry.key,)
 match_registry[jtu.FlattenedIndexKey] = lambda entry: (entry.key,)
 
 
 def _generate_path_mask(
     tree: PyTree,
     where: tuple[int | str, ...],
@@ -568,35 +523,33 @@
 ) -> PyTree:
     # generate a mask for `where` path in `tree`
     # where path is a tuple of indices or keys, for example
     # where=("a",) wil set all leaves of `tree` with key "a" to True and
     # all other leaves to False
     match = False
 
-    def map_func(path: TraceType, _: Any):
-        keys, _ = path
-
-        if len(where) > len(keys):
+    def map_func(path, _: Any):
+        if len(where) > len(path):
             # path is shorter than `where` path. for example
             # where=("a", "b") and the current path is ("a",) then
             # the current path is not a match
             return False
 
-        for wi, key in zip(where, keys):
-            if wi not in (..., *match_registry[type(key)](key)):
+        for wi, ki in zip(where, path):
+            if wi not in (..., *match_registry[type(ki)](ki)):
                 return False
 
         nonlocal match
 
         return (match := True)
 
-    mask = tree_map_with_trace(map_func, tree, is_leaf=is_leaf)
+    mask = jtu.tree_map_with_path(map_func, tree, is_leaf=is_leaf)
 
     if not match:
-        raise LookupError(f"No leaf match is found for {where=} and {mask=}")
+        raise LookupError(f"No leaf match is found for {where=}.")
 
     return mask
 
 
 def _combine_maybe_bool_masks(*masks: PyTree) -> PyTree:
     # combine boolean masks with `&` operator if all masks are boolean
     # otherwise raise an error
@@ -729,15 +682,15 @@
     func: Callable[..., Any],
     tree: Any,
     *rest: Any,
     is_leaf: IsLeafType = None,
 ) -> Any:
     # the code style of `tree_{...} is heavilty influenced by `jax.tree_util`
     # https://github.com/google/jax/blob/main/jax/_src/tree_util.py
-    r"""
+    """
     Similar to `jax.tree_util.tree_map_with_path` that accept a function
     that takes a two-item tuple for key path and type path.
 
     Args:
         func: A function that takes a trace and a leaf and returns a new leaf.
         tree: The tree to be mapped over.
         rest: Additional trees to be mapped over.
```

### Comparing `pytreeclass-0.3.6/pytreeclass.egg-info/PKG-INFO` & `pytreeclass-0.3.7/pytreeclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.3.6
+Version: 0.3.7
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytreeclass-0.3.6/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.3.7/pytreeclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.6/setup.py` & `pytreeclass-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.6/tests/test_indexing.py` & `pytreeclass-0.3.7/tests/test_indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,31 +40,31 @@
         d=level1(a=1, b=10, c=jnp.array([1, 2, 3, 4, 5])),
         e=level1(a=2, b=20, c=jnp.array([-1, -2, -3, -4, -5])),
     )
 
     B = A.at[A > 0].get()
     C = level2(
         d=level1(a=1, b=10, c=jnp.array([1, 2, 3, 4, 5])),
-        e=level1(a=2, b=20, c=jnp.array([])),
+        e=level1(a=2, b=20, c=jnp.array([], dtype=int)),
     )
 
     assert pytc.is_tree_equal(B, C)
 
     B = A.at[(A > 0) & (A < 5)].get()
     C = level2(
         d=level1(a=1, b=None, c=jnp.array([1, 2, 3, 4])),
-        e=level1(a=2, b=None, c=jnp.array([])),
+        e=level1(a=2, b=None, c=jnp.array([], dtype=int)),
     )
 
     assert pytc.is_tree_equal(B, C)
 
     B = A.at[A == 0].get()
     C = level2(
-        d=level1(a=None, b=None, c=jnp.array([])),
-        e=level1(a=None, b=None, c=jnp.array([])),
+        d=level1(a=None, b=None, c=jnp.array([], dtype=int)),
+        e=level1(a=None, b=None, c=jnp.array([], dtype=int)),
     )
 
     assert pytc.is_tree_equal(B, C)
 
     with pytest.raises(TypeError):
         B = A.at[A].get()
 
@@ -584,15 +584,17 @@
         a: jnp.ndarray
 
         def __init__(self, a=jnp.array([1, 2, 3, 4, 5])) -> None:
             self.a = a
 
     t = Tree()
 
-    assert pytc.is_tree_equal(t.at[t > 0].at[t < 0].get(), Tree(jnp.array([])))
+    assert pytc.is_tree_equal(
+        t.at[t > 0].at[t < 0].get(), Tree(jnp.array([], dtype=int))
+    )
 
     with pytest.raises(AttributeError):
         t.at[t > 0].bet
 
     with pytest.raises(AttributeError):
         t.at["a"].bet
```

### Comparing `pytreeclass-0.3.6/tests/test_nn.py` & `pytreeclass-0.3.7/tests/test_nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,21 +145,21 @@
             self.count = 0
 
         def __call__(self, x):
             return x @ self.weight + self.bias
 
     class StackedLinear(pytc.TreeClass, leafwise=True):
         name: str
-        exact_array: jax.Array
-        bool_array: jax.Array
+        # exact_array: jax.Array
+        # bool_array: jax.Array
 
         def __init__(self, key, in_dim, out_dim, hidden_dim):
             self.name = "stack"
-            self.exact_array = jnp.array([1, 2, 3])
-            self.bool_array = jnp.array([True, True])
+            # self.exact_array = jnp.array([1, 2, 3])
+            # self.bool_array = jnp.array([True, True])
 
             keys = jr.split(key, 3)
 
             self.l1 = Linear(key=keys[0], in_dim=in_dim, out_dim=hidden_dim)
             self.l2 = Linear(key=keys[1], in_dim=hidden_dim, out_dim=hidden_dim)
             self.l3 = Linear(key=keys[2], in_dim=hidden_dim, out_dim=out_dim)
```

### Comparing `pytreeclass-0.3.6/tests/test_tree_freeze.py` & `pytreeclass-0.3.7/tests/test_tree_freeze.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import pytest
 
 import pytreeclass as pytc
-from pytreeclass._src.tree_util import _HashableWrapper, tree_hash
+from pytreeclass._src.tree_util import tree_hash
 
 
 def test_freeze_unfreeze():
     class A(pytc.TreeClass, leafwise=True):
         a: int
         b: int
 
@@ -354,23 +354,23 @@
     assert model.a == pytest.approx(-0.45068058, 1e-5)
 
 
 def test_wrapper():
     # only apply last wrapper
     assert hash((pytc.freeze(1))) == tree_hash(1)
 
-    lhs = _HashableWrapper(1)
-    # test getter
-    assert lhs.__wrapped__ == 1
-    assert lhs.__wrapped__
-
-    # comparison with the wrapped object
-    assert lhs != 1
-    # hash of the wrapped object
-    assert hash(lhs) == tree_hash(1)
+    # lhs = _HashableWrapper(1)
+    # # test getter
+    # assert lhs.__wrapped__ == 1
+    # assert lhs.__wrapped__
+
+    # # comparison with the wrapped object
+    # assert lhs != 1
+    # # hash of the wrapped object
+    # assert hash(lhs) == tree_hash(1)
 
     # test immutability
     frozen_value = pytc.freeze(1)
 
     with pytest.raises(AttributeError):
         frozen_value.__wrapped__ = 2
```

### Comparing `pytreeclass-0.3.6/tests/test_tree_operator.py` & `pytreeclass-0.3.7/tests/test_tree_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import math
 
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import pytest
 
 import pytreeclass as pytc
-from pytreeclass._src.tree_util import _hash_node, bcmap
+from pytreeclass._src.tree_util import bcmap
 
 
 def test_bcmap():
     class Test(pytc.TreeClass, leafwise=True):
         a: tuple[int]
         b: tuple[int]
         c: jnp.ndarray
@@ -125,12 +125,12 @@
     with pytest.raises(TypeError):
         A + "s"
 
     with pytest.raises(TypeError):
         A == (1,)
 
 
-def test_hash_node():
-    assert _hash_node([1, 2, 3])
-    assert _hash_node(jnp.array([1, 2, 3]))
-    assert _hash_node({1, 2, 3})
-    assert _hash_node({"a": 1})
+# def test_hash_node():
+#     assert _hash_node([1, 2, 3])
+#     assert _hash_node(jnp.array([1, 2, 3]))
+#     assert _hash_node({1, 2, 3})
+#     assert _hash_node({"a": 1})
```

### Comparing `pytreeclass-0.3.6/tests/test_tree_pprint.py` & `pytreeclass-0.3.7/tests/test_tree_pprint.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.6/tests/test_tree_viz_util.py` & `pytreeclass-0.3.7/tests/test_tree_viz_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 from __future__ import annotations
 
 import jax
 import jax.nn.initializers as ji
 import jax.tree_util as jtu
 
-from pytreeclass._src.tree_pprint import (
-    _func_pprint,
-    _hbox,
-    _hstack,
-    _node_pprint,
-    _table,
-    _vbox,
-)
+from pytreeclass._src.tree_pprint import _hbox, _hstack, _table, _vbox, func_pp, pp
 
 
 def test_vbox():
     assert _vbox("a", " a", "a ") == "┌──┐\n│a │\n├──┤\n│ a│\n├──┤\n│a │\n└──┘"
     assert _vbox("a", "b") == "┌─┐\n│a│\n├─┤\n│b│\n└─┘"
 
 
@@ -33,40 +26,40 @@
     )
 
 
 def test_hstack():
     assert _hstack(_hbox("a"), _vbox("b", "c")) == "┌─┬─┐\n│a│b│\n└─┼─┤\n  │c│\n  └─┘"
 
 
-def test_func_pprint():
+def test_func_pp():
     def example(a: int, b=1, *c, d, e=2, **f) -> str:
         ...  # fmt: skip
 
     assert (
-        _func_pprint(example, indent=0, kind="str", width=60, depth=0)
+        func_pp(example, indent=0, kind="str", width=60, depth=0)
         == "example(a, b, *c, d, e, **f)"
     )
+    # assert (
+    #     func_pp(lambda x: x, indent=0, kind="str", width=60, depth=0)
+    #     == "Lambda(x)"
+    # )
     assert (
-        _func_pprint(lambda x: x, indent=0, kind="str", width=60, depth=0)
-        == "Lambda(x)"
-    )
-    assert (
-        _func_pprint(jax.nn.relu, indent=0, kind="str", width=60, depth=0)
+        func_pp(jax.nn.relu, indent=0, kind="str", width=60, depth=0)
         == "relu(*args, **kwargs)"
     )
     assert (
-        _node_pprint(jtu.Partial(jax.nn.relu), indent=0, kind="str", width=60, depth=0)
+        pp(jtu.Partial(jax.nn.relu), indent=0, kind="str", width=60, depth=0)
         == "Partial(relu(*args, **kwargs))"
     )
     assert (
-        _node_pprint(jtu.Partial(jax.nn.relu), indent=0, kind="str", width=60, depth=0)
+        pp(jtu.Partial(jax.nn.relu), indent=0, kind="str", width=60, depth=0)
         == "Partial(relu(*args, **kwargs))"
     )
     assert (
-        _func_pprint(ji.he_normal, indent=0, kind="str", width=60, depth=0)
+        func_pp(ji.he_normal, indent=0, kind="str", width=60, depth=0)
         == "he_normal(in_axis, out_axis, batch_axis, dtype)"
     )
 
-    assert (
-        _node_pprint(jax.jit(lambda x: x), indent=0, kind="repr", width=60, depth=0)
-        == "jit(Lambda(x))"
-    )
+    # assert (
+    #     _pprint(jax.jit(lambda x: x), indent=0, kind="repr", width=60, depth=0)
+    #     == "jit(Lambda(x))"
+    # )
```

### Comparing `pytreeclass-0.3.6/tests/test_treeclass.py` & `pytreeclass-0.3.7/tests/test_treeclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,20 +128,20 @@
             self.a = pytc.freeze(a)
             self.b = b
 
     test = Test()
     npt.assert_allclose(jtu.tree_leaves(test)[0], jnp.array([4, 5, 6]))
 
 
-def test_hash():
-    class T(pytc.TreeClass):
-        a: jax.Array
+# def test_hash():
+#     class T(pytc.TreeClass):
+#         a: jax.Array
 
-    # with pytest.raises(TypeError):
-    hash(T(jnp.array([1, 2, 3])))
+#     # with pytest.raises(TypeError):
+#     hash(T(jnp.array([1, 2, 3])))
 
 
 def test_post_init():
     class Test(pytc.TreeClass):
         a: int = 1
 
         def __post_init__(self):
```

