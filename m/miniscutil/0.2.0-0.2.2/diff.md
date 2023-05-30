# Comparing `tmp/miniscutil-0.2.0.tar.gz` & `tmp/miniscutil-0.2.2.tar.gz`

## Comparing `miniscutil-0.2.0.tar` & `miniscutil-0.2.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/__about__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/__init__.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/adapt.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/asyncio_helpers.py
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/config.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/current.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/deep.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/deepeq.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/dictdiff.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/dispatch.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/misc.py
--rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/ofdict.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/sum.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/type_util.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/lsp/README.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/lsp/__init__.py
--rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/lsp/document.py
--rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/lsp/server.py
--rw-r--r--   0        0        0    12543 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/lsp/types.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/__init__.py
--rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/extrarpc.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/io_transport.py
--rw-r--r--   0        0        0    19393 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/jsonrpc.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/starlette_ws_transport.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/transport.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/websocket_transport.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_classdispatch.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_config.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_current.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_deepeq.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_humansize.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_lsp.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_ofdict.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_typing.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/snapshots/test_humansize/test_human_size/bytes
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.2.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.2.0/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/__about__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/__init__.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/adapt.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/asyncio_helpers.py
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/config.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/current.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/deep.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/deepeq.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/dictdiff.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/dispatch.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/misc.py
+-rw-r--r--   0        0        0    13847 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/ofdict.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/sum.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/type_util.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/lsp/README.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/lsp/__init__.py
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/lsp/document.py
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/lsp/server.py
+-rw-r--r--   0        0        0    12751 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/lsp/types.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/__init__.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/extrarpc.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/io_transport.py
+-rw-r--r--   0        0        0    19268 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/jsonrpc.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/starlette_ws_transport.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/transport.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.2.2/miniscutil/rpc/websocket_transport.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_classdispatch.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_config.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_current.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_deepeq.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_humansize.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_lsp.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_ofdict.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_typing.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/test_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.2.2/tests/snapshots/test_humansize/test_human_size/bytes
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.2.2/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.2.2/PKG-INFO
```

### Comparing `miniscutil-0.2.0/miniscutil/__init__.py` & `miniscutil-0.2.2/miniscutil/__init__.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/adapt.py` & `miniscutil-0.2.2/miniscutil/adapt.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/asyncio_helpers.py` & `miniscutil-0.2.2/miniscutil/asyncio_helpers.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/config.py` & `miniscutil-0.2.2/miniscutil/config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/current.py` & `miniscutil-0.2.2/miniscutil/current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/deep.py` & `miniscutil-0.2.2/miniscutil/deep.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/deepeq.py` & `miniscutil-0.2.2/miniscutil/deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/dispatch.py` & `miniscutil-0.2.2/miniscutil/dispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/misc.py` & `miniscutil-0.2.2/miniscutil/misc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/ofdict.py` & `miniscutil-0.2.2/miniscutil/ofdict.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,16 @@
 @contextmanager
 def dpath(coord: str):
     with map_ctx(ofdict_context, lambda x: x + [coord]) as p:
         yield p
 
 
 class OfDictError(TypeError):
+    """Error caused by a failure to convert a dictionary-like object to a type using ofdict."""
+
     def __init__(self, msg: str):
         super().__init__(msg + atstr())
 
 
 @classdispatch
 def ofdict(A: Type[T], a: JsonLike) -> T:
     """Converts an ``a`` to an instance of ``A``, calling recursively if necessary.
@@ -108,14 +110,15 @@
 
     [todo] I am hoping to retire this in favour of Pydantic.
     """
     if isinstance(A, str):
         raise TypeError(
             f"please make sure your class {A} is referred using types and not string-escaped types"
         )
+        # [todo] also https://docs.python.org/3/library/typing.html#typing.ForwardRef
     S = as_newtype(A)
     if S is not None:
         return A(ofdict(S, a))
     if inspect.isclass(A) and issubclass(A, OfDictUnion):
         class_key = getattr(A, "_class_key", "__class__")
         ct = getattr(A, "_class_table", None)
         if ct is None:
@@ -141,15 +144,16 @@
         else:
             logger.warning(f"Expected one of {values}, got {a}")
     if get_origin(A) is Union:
         es = []
         for X in get_args(A):
             try:
                 return ofdict(X, a)
-            except Exception as e:
+            except OfDictError as e:
+                # [note] python 3.11 has exception groups instead
                 es.append(e)
         # [todo] raise everything?
         raise es[-1]
     od = getattr(A, "__ofdict__", None)
     if od is not None:
         return od(a)
     adapt = getattr(A, "__adapt__", None)
@@ -432,14 +436,33 @@
     _class_table: ClassVar[dict[str, type]]
     _root_class: ClassVar[type["OfDictUnion"]]
     """ Use this when you have a class hierarchy of types that you want
     to be able to serialize using todict.
 
     It works by also storing a  `"__class__": cls.__name__` entry on a class table.
     When the dict is deserialised, it will look up this class name to find the subclass.
+
+
+    Example usage:
+    ```
+    class Base(OfDictUnion):
+      pass
+
+    @dataclass
+    class X(Base):
+      x : str
+
+    @dataclass
+    class Y(Base):
+      y : int
+
+    assert todict(X(x="hello")) == {"__class__": "X", "x": "hello"}
+    assert todict(Y(y=42)) == {"__class__": "Y", "y": 42}
+    assert ofdict(Base, {"__class__": "X", "x": "hello"}) == X(x="hello")
+    ```
     """
 
     def __init_subclass__(cls, **kwargs):
         if not hasattr(cls, "_class_table"):
             # first time
             cls._class_table = dict()
             cls._root_class = cls
@@ -457,12 +480,12 @@
         return x.dict()
 
     @ofdict.register(BaseModel)
     def _ofdict_model(ModelCls: type[BaseModel], item):
         try:
             return ModelCls.parse_obj(item)
         except ValidationError as e:
-            raise TypeError(f"Model {ModelCls.__name__} is invalid: {e}") from e
+            raise OfDictError(f"Model {ModelCls.__name__} is invalid: {e}") from e
 
     # [todo] pydantic validation types like EmailStr, SecretStr etc
 except ImportError:
     pass
```

### Comparing `miniscutil-0.2.0/miniscutil/sum.py` & `miniscutil-0.2.2/miniscutil/sum.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/type_util.py` & `miniscutil-0.2.2/miniscutil/type_util.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/lsp/document.py` & `miniscutil-0.2.2/miniscutil/lsp/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import bisect
 import contextlib
 from contextvars import ContextVar
 from dataclasses import dataclass, replace
 from enum import Enum
 import functools
 import itertools
-from typing import Iterable, Optional, TypeAlias, Union
-
+from typing import Iterable, Optional, Union
+try:
+    from typing import TypeAlias, TypeVar
+except:
+    from typing_extensions import TypeAlias, TypeVar
 from miniscutil.misc import set_ctx
 
 
 class PositionEncodingKind(Enum):
     UTF8 = "utf-8"
     UTF16 = "utf-16"
     UTF32 = "utf-32"
```

### Comparing `miniscutil-0.2.0/miniscutil/lsp/server.py` & `miniscutil-0.2.2/miniscutil/lsp/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,7 +120,12 @@
     @rpc_method("textDocument/didSave")
     def on_did_save(self, params: lsp.DidSaveTextDocumentParams):
         pass
 
     @rpc_method("textDocument/didClose")
     def on_did_close(self, params: lsp.DidCloseTextDocumentParams):
         pass
+
+    @rpc_method("$/setTrace")
+    def on_set_trace(self, params: lsp.SetTraceParams):
+        # [todo] logging stuff.
+        pass
```

### Comparing `miniscutil-0.2.0/miniscutil/lsp/types.py` & `miniscutil-0.2.2/miniscutil/lsp/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from dataclasses import dataclass, field, replace
 from enum import Enum
 from pathlib import Path
-from typing import Any, Generic, Literal, Optional, TypeAlias, TypeVar, Union
+from typing import Any, Generic, Literal, Optional, Union
 from typing import Optional as opt
 import urllib.parse
 from .document import *
-
+try:
+    from typing import TypeAlias, TypeVar
+except:
+    from typing_extensions import TypeAlias, TypeVar
 T = TypeVar("T")
 
 DocumentUri = str
 
 # [todo] use TypedDict or BaseModel instead?
 
 """ This file contains a Python implementation of the Language Server Protocol datatypes.
@@ -459,7 +462,15 @@
     ] = field(default=None)
 
 
 @dataclass
 class ApplyWorkspaceEditParams:
     edit: WorkspaceEdit
     label: Optional[str] = field(default=None)
+
+
+TraceValue: TypeAlias = Literal["off", "messages", "verbose"]
+
+
+@dataclass
+class SetTraceParams:
+    value: TraceValue
```

### Comparing `miniscutil-0.2.0/miniscutil/rpc/extrarpc.py` & `miniscutil-0.2.2/miniscutil/rpc/extrarpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 from typing import (
     Any,
     AsyncGenerator,
     AsyncIterator,
     Callable,
     Generic,
     Optional,
-    TypeAlias,
-    TypeVar,
     Union,
 )
 from uuid import uuid4
 
+try:
+    from typing import TypeAlias, TypeVar
+except:
+    from typing_extensions import TypeAlias, TypeVar
 from .transport import Transport
 from .jsonrpc import InitializationMode, RpcServer, rpc_method
 
 ProgressToken: TypeAlias = Union[str, int]
 
 logger = logging.getLogger(__name__)
 
@@ -39,15 +41,15 @@
     value: Q
 
 
 class RequestFutureWithProgress(Generic[Q, R]):
     """A future for an RPC request that also has a 'progress()' field."""
 
     token: ProgressToken
-    _q: asyncio.Queue[Q | StopAsyncIteration]
+    _q: asyncio.Queue[Union[Q, StopAsyncIteration]]
     _r: asyncio.Future[R]
     _callbacks: set[Callable[[Q], None]]
 
     def __init__(self, token: ProgressToken, result_fut: asyncio.Future[R]):
         # [todo] use a deque and Event instead so that it can be iterated multiple times.
         self.token = token
         self._q = asyncio.Queue()
```

### Comparing `miniscutil-0.2.0/miniscutil/rpc/io_transport.py` & `miniscutil-0.2.2/miniscutil/rpc/io_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/rpc/jsonrpc.py` & `miniscutil-0.2.2/miniscutil/rpc/jsonrpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -519,28 +519,25 @@
             if req.method == "shutdown":
                 if "shutdown" in self.dispatcher:
                     return await self.dispatcher.dispatch("shutdown", None)
                 else:
                     return None
             raise invalid_request("server has shut down")
 
-        logger.debug(f"{self.name} ← {req.id} {req.method}")
-
         if req.method == "$/cancelRequest":
             if not req.is_notification:
                 raise invalid_request("cancel request must be a notification")
             if not isinstance(req.params, dict) or not "id" in req.params:
                 raise invalid_params('params must be a dict with "id" key')
             t = self.their_requests.get(req.params["id"], None)
             if t is not None:
                 t.cancel("requested by peer")
             return None
 
         if req.method not in self.dispatcher:
-            logger.error(f'method "{req.method}" not found')
             raise method_not_found(req.method)
 
         T = self.dispatcher.param_type(req.method)
         try:
             params = ofdict(T, req.params)
         except TypeError as e:
             message = (
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `miniscutil-0.2.0/miniscutil/rpc/starlette_ws_transport.py` & `miniscutil-0.2.2/miniscutil/rpc/starlette_ws_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/rpc/transport.py` & `miniscutil-0.2.2/miniscutil/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/miniscutil/rpc/websocket_transport.py` & `miniscutil-0.2.2/miniscutil/rpc/websocket_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/tests/test_classdispatch.py` & `miniscutil-0.2.2/tests/test_classdispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/tests/test_config.py` & `miniscutil-0.2.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/tests/test_current.py` & `miniscutil-0.2.2/tests/test_current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/tests/test_deepeq.py` & `miniscutil-0.2.2/tests/test_deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/tests/test_lsp.py` & `miniscutil-0.2.2/tests/test_lsp.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/tests/test_ofdict.py` & `miniscutil-0.2.2/tests/test_ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/tests/test_typing.py` & `miniscutil-0.2.2/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/.gitignore` & `miniscutil-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/LICENSE.txt` & `miniscutil-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/README.md` & `miniscutil-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/pyproject.toml` & `miniscutil-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.0/PKG-INFO` & `miniscutil-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniscutil
-Version: 0.2.0
+Version: 0.2.2
 Project-URL: Documentation, https://github.com/EdAyers/sss/miniscutil#readme
 Project-URL: Issues, https://github.com/EdAyers/sss/miniscutil/issues
 Project-URL: Source, https://github.com/EdAyers/sss/miniscutil
 Author-email: "E.W.Ayers" <contact@edayers.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

