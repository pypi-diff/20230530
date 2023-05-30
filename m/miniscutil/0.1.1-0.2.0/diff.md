# Comparing `tmp/miniscutil-0.1.1.tar.gz` & `tmp/miniscutil-0.2.0.tar.gz`

## Comparing `miniscutil-0.1.1.tar` & `miniscutil-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/__about__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/__init__.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/adapt.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/asyncio_helpers.py
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/config.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/current.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/deep.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/deepeq.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/dictdiff.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/dispatch.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/misc.py
--rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/ofdict.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/sum.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/type_util.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/lsp/README.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/lsp/__init__.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/lsp/server.py
--rw-r--r--   0        0        0    12321 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/lsp/types.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/__init__.py
--rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/extrarpc.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/io_transport.py
--rw-r--r--   0        0        0    19393 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/jsonrpc.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/starlette_ws_transport.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/transport.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/websocket_transport.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_classdispatch.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_config.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_current.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_deepeq.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_humansize.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_ofdict.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_typing.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/snapshots/test_humansize/test_human_size/bytes
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.1.1/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.1.1/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/__about__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/__init__.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/adapt.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/asyncio_helpers.py
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/config.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/current.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/deep.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/deepeq.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/dictdiff.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/dispatch.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/misc.py
+-rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/ofdict.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/sum.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/type_util.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/lsp/README.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/lsp/__init__.py
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/lsp/document.py
+-rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/lsp/server.py
+-rw-r--r--   0        0        0    12543 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/lsp/types.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/__init__.py
+-rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/extrarpc.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/io_transport.py
+-rw-r--r--   0        0        0    19393 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/jsonrpc.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/starlette_ws_transport.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/transport.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.2.0/miniscutil/rpc/websocket_transport.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_classdispatch.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_config.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_current.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_deepeq.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_humansize.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_lsp.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_ofdict.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_typing.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/test_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.2.0/tests/snapshots/test_humansize/test_human_size/bytes
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.2.0/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.2.0/PKG-INFO
```

### Comparing `miniscutil-0.1.1/miniscutil/__init__.py` & `miniscutil-0.2.0/miniscutil/__init__.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/adapt.py` & `miniscutil-0.2.0/miniscutil/adapt.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/asyncio_helpers.py` & `miniscutil-0.2.0/miniscutil/asyncio_helpers.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/config.py` & `miniscutil-0.2.0/miniscutil/config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/current.py` & `miniscutil-0.2.0/miniscutil/current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/deep.py` & `miniscutil-0.2.0/miniscutil/deep.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/deepeq.py` & `miniscutil-0.2.0/miniscutil/deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/dispatch.py` & `miniscutil-0.2.0/miniscutil/dispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/misc.py` & `miniscutil-0.2.0/miniscutil/misc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/ofdict.py` & `miniscutil-0.2.0/miniscutil/ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/sum.py` & `miniscutil-0.2.0/miniscutil/sum.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/type_util.py` & `miniscutil-0.2.0/miniscutil/type_util.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/lsp/types.py` & `miniscutil-0.2.0/miniscutil/lsp/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, replace
 from enum import Enum
 from pathlib import Path
 from typing import Any, Generic, Literal, Optional, TypeAlias, TypeVar, Union
 from typing import Optional as opt
 import urllib.parse
+from .document import *
 
 T = TypeVar("T")
 
 DocumentUri = str
 
 # [todo] use TypedDict or BaseModel instead?
 
@@ -16,14 +17,16 @@
 It is not an exhaustive set of types, I add to it as needed.
 
 All docstrings are copied verbatim from the specification.
 
 https://microsoft.github.io/language-server-protocol/specifications/lsp/3.17/specification
 """
 
+EOL = ["\n", "\r\n", "\r"]
+
 
 def path_of_uri(uri: DocumentUri):
     x = urllib.parse.urlparse(uri)
     assert x.netloc == ""
     assert x.scheme == "file"
     return Path(x.path)
 
@@ -45,34 +48,14 @@
 
     def __fspath__(self):
         # https://docs.python.org/3/library/os.html#os.PathLike.__fspath__
         return str(path_of_uri(self.uri))
 
 
 @dataclass
-class Position:
-    line: int
-    character: int
-
-
-@dataclass
-class Range:
-    start: Position
-    end: Position
-
-    @classmethod
-    def mk(cls, l0: int, c0: int, l1: int, c1: int):
-        return cls(Position(l0, c0), Position(l1, c1))
-
-    @classmethod
-    def of_pos(cls, pos: Position):
-        return cls(pos, pos)
-
-
-@dataclass
 class TextDocumentParams:
     textDocument: TextDocumentIdentifier
 
     def __fspath__(self):
         return self.textDocument.__fspath__()
 
 
@@ -125,40 +108,60 @@
 @dataclass
 class ClientWorkspaceCapabilities:
     applyEdit: opt[bool] = field(default=None)
     # workspaceEdit: opt[WorkspaceEditClientCapabilities] = field(default=None)
 
 
 @dataclass
+class GeneralClientCapabilities:
+    # staleRequestSupport
+    # regularExpressions
+    # markdown
+    positionEncodings: opt[list[PositionEncodingKind]] = field(
+        default_factory=lambda: [PositionEncodingKind.UTF16]
+    )
+    """ The position encodings supported by the client. Client and server
+    have to agree on the same position encoding to ensure that offsets
+    (e.g. character position in a line) are interpreted the same on both
+    side.
+
+    To keep the protocol backwards compatible the following applies: if
+    the value 'utf-16' is missing from the array of position encodings
+    servers can assume that the client supports UTF-16. UTF-16 is
+    therefore a mandatory encoding.
+
+    If omitted it defaults to ['utf-16'].
+
+    Implementation considerations: since the conversion from one encoding
+    into another requires the content of the file / line the conversion
+    is best done where the file is read which is usually on the server
+    side."""
+
+
+@dataclass
 class ClientCapabilities:
     textDocument: opt[TextDocumentClientCapabilities] = field(default=None)
     workspace: opt[ClientWorkspaceCapabilities] = field(default=None)
     # notebookDocument
     # window
-    # general
+    general: opt[GeneralClientCapabilities] = field(default=None)
     # experimental
 
 
 @dataclass
 class InitializeParams:
     processId: Optional[int] = field(default=None)
     locale: Optional[str] = field(default=None)
     workspaceFolders: Optional[list[WorkspaceFolder]] = field(default=None)
     clientInfo: Optional[PeerInfo] = field(default=None)
     initializationOptions: Optional[Any] = field(default=None)
     capabilities: Optional[ClientCapabilities] = field(default=None)
     trace: Optional[Literal["off", "messages", "verbose"]] = field(default=None)
 
 
-class PositionEncodingKind(Enum):
-    UTF8 = "utf-8"
-    UTF16 = "utf-16"
-    UTF32 = "utf-32"
-
-
 class TextDocumentSyncKind(Enum):
     none = 0
     full = 1
     incremental = 2
 
 
 @dataclass
@@ -172,31 +175,14 @@
     change: Optional[TextDocumentSyncKind] = field(default=None)
     willChange: Optional[bool] = field(default=None)
     willSaveWaitUntil: Optional[bool] = field(default=None)
     save: Optional[Union[bool, SaveOptions]] = field(default=None)
 
 
 @dataclass
-class TextDocumentItem:
-    uri: DocumentUri
-    languageId: str
-    version: int
-    text: str
-    """ Content of the opened text document. """
-
-    def __fspath__(self):
-        return self.uri
-
-
-@dataclass
-class DidOpenTextDocumentParams:
-    textDocument: TextDocumentItem
-
-
-@dataclass
 class DocumentFilter:
     language: Optional[str]
     """ A language id, like `typescript`. """
     scheme: Optional[str]
     """ A Uri scheme, like `file` or `untitled`. """
     pattern: Optional[str]
     """ A glob pattern, like `*.{ts,js}`. """
@@ -212,19 +198,16 @@
 
 @dataclass
 class TextDocumentChangeRegistrationOptions:
     syncKind: TextDocumentSyncKind
 
 
 @dataclass
-class TextDocumentContentChangeEvent:
-    range: Optional[Range]
-    rangeLength: Optional[int]
-    text: str
-    """ The new text of the whole document, or the replacement text for the range if the range field is provided. """
+class DidOpenTextDocumentParams:
+    textDocument: TextDocumentItem
 
 
 @dataclass
 class DidCloseTextDocumentParams:
     textDocument: TextDocumentIdentifier
```

### Comparing `miniscutil-0.1.1/miniscutil/rpc/extrarpc.py` & `miniscutil-0.2.0/miniscutil/rpc/extrarpc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/rpc/io_transport.py` & `miniscutil-0.2.0/miniscutil/rpc/io_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/rpc/jsonrpc.py` & `miniscutil-0.2.0/miniscutil/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/rpc/starlette_ws_transport.py` & `miniscutil-0.2.0/miniscutil/rpc/starlette_ws_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/rpc/transport.py` & `miniscutil-0.2.0/miniscutil/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/miniscutil/rpc/websocket_transport.py` & `miniscutil-0.2.0/miniscutil/rpc/websocket_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/tests/test_classdispatch.py` & `miniscutil-0.2.0/tests/test_classdispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/tests/test_config.py` & `miniscutil-0.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/tests/test_current.py` & `miniscutil-0.2.0/tests/test_current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/tests/test_deepeq.py` & `miniscutil-0.2.0/tests/test_deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/tests/test_ofdict.py` & `miniscutil-0.2.0/tests/test_ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/tests/test_typing.py` & `miniscutil-0.2.0/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/.gitignore` & `miniscutil-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/LICENSE.txt` & `miniscutil-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/README.md` & `miniscutil-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/pyproject.toml` & `miniscutil-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.1/PKG-INFO` & `miniscutil-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniscutil
-Version: 0.1.1
+Version: 0.2.0
 Project-URL: Documentation, https://github.com/EdAyers/sss/miniscutil#readme
 Project-URL: Issues, https://github.com/EdAyers/sss/miniscutil/issues
 Project-URL: Source, https://github.com/EdAyers/sss/miniscutil
 Author-email: "E.W.Ayers" <contact@edayers.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

