# Comparing `tmp/drakaina-0.7.0b0.tar.gz` & `tmp/drakaina-0.7.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drakaina-0.7.0b0.tar", max compression
+gzip compressed data, was "drakaina-0.7.0b3.tar", max compression
```

## Comparing `drakaina-0.7.0b0.tar` & `drakaina-0.7.0b3.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0     9580 2023-05-17 12:47:04.917328 drakaina-0.7.0b0/drakaina/__init__.py
--rw-r--r--   0        0        0    11634 2023-05-17 12:47:04.918340 drakaina-0.7.0b0/drakaina/_types.py
--rw-r--r--   0        0        0     1494 2023-01-27 12:48:38.216236 drakaina-0.7.0b0/drakaina/asgi.py
--rw-r--r--   0        0        0     3699 2023-02-13 13:22:12.183448 drakaina-0.7.0b0/drakaina/client/__init__.py
--rw-r--r--   0        0        0     6158 2022-07-08 05:47:38.000000 drakaina-0.7.0b0/drakaina/client/base.py
--rw-r--r--   0        0        0     1832 2022-07-08 05:47:38.000000 drakaina-0.7.0b0/drakaina/client/http.py
--rw-r--r--   0        0        0    11280 2023-01-27 12:55:37.114745 drakaina-0.7.0b0/drakaina/client/tcp.py
--rw-r--r--   0        0        0     8797 2022-07-08 05:47:38.000000 drakaina-0.7.0b0/drakaina/client/websocket.py
--rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.0b0/drakaina/contrib/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.0b0/drakaina/contrib/django/__init__.py
--rw-r--r--   0        0        0     6132 2023-04-11 08:46:20.669302 drakaina-0.7.0b0/drakaina/contrib/django/middleware.py
--rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.0b0/drakaina/contrib/django/views.py
--rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.0b0/drakaina/contrib/jwt/__init__.py
--rw-r--r--   0        0        0      348 2023-03-10 11:02:10.213372 drakaina-0.7.0b0/drakaina/contrib/jwt/errors.py
--rw-r--r--   0        0        0     9102 2023-05-17 12:47:04.918340 drakaina-0.7.0b0/drakaina/contrib/jwt/middleware.py
--rw-r--r--   0        0        0      913 2023-04-03 15:58:34.495338 drakaina-0.7.0b0/drakaina/contrib/jwt/types.py
--rw-r--r--   0        0        0    18791 2023-05-17 12:47:04.919340 drakaina-0.7.0b0/drakaina/contrib/jwt/utils.py
--rw-r--r--   0        0        0     1651 2023-05-05 11:41:17.675178 drakaina-0.7.0b0/drakaina/drakaina_openapi.py
--rw-r--r--   0        0        0     1327 2023-05-11 09:46:59.367413 drakaina-0.7.0b0/drakaina/exceptions.py
--rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.0b0/drakaina/middleware/__init__.py
--rw-r--r--   0        0        0     1378 2023-03-29 21:57:07.601330 drakaina-0.7.0b0/drakaina/middleware/base.py
--rw-r--r--   0        0        0     7586 2023-05-17 12:47:04.920325 drakaina-0.7.0b0/drakaina/middleware/cors.py
--rw-r--r--   0        0        0     2040 2023-05-17 12:47:04.920325 drakaina-0.7.0b0/drakaina/middleware/exception.py
--rw-r--r--   0        0        0      430 2023-04-13 16:28:59.822156 drakaina-0.7.0b0/drakaina/middleware/gzip.py
--rw-r--r--   0        0        0      983 2023-04-04 11:19:41.525282 drakaina-0.7.0b0/drakaina/middleware/logging.py
--rw-r--r--   0        0        0     1138 2023-01-18 00:52:37.644550 drakaina-0.7.0b0/drakaina/middleware/openapi/__init__.py
--rw-r--r--   0        0        0     1079 2023-04-04 11:19:41.580823 drakaina-0.7.0b0/drakaina/middleware/request_wrapper.py
--rw-r--r--   0        0        0    12639 2023-05-17 12:47:04.921327 drakaina-0.7.0b0/drakaina/registries.py
--rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.0b0/drakaina/rpc_protocols/__init__.py
--rw-r--r--   0        0        0    12567 2023-05-17 12:47:04.922328 drakaina-0.7.0b0/drakaina/rpc_protocols/base.py
--rw-r--r--   0        0        0    10527 2023-05-16 19:17:53.349082 drakaina-0.7.0b0/drakaina/rpc_protocols/jsonrpc20.py
--rw-r--r--   0        0        0      200 2023-01-09 10:12:10.047554 drakaina-0.7.0b0/drakaina/rsgi.py
--rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.0b0/drakaina/serializers.py
--rw-r--r--   0        0        0    11142 2023-01-27 12:51:42.029067 drakaina-0.7.0b0/drakaina/tcp.py
--rw-r--r--   0        0        0     3741 2023-05-17 12:47:04.922328 drakaina-0.7.0b0/drakaina/utils.py
--rw-r--r--   0        0        0      162 2023-01-25 16:44:10.299855 drakaina-0.7.0b0/drakaina/ws.py
--rw-r--r--   0        0        0     8181 2023-05-17 12:47:04.923326 drakaina-0.7.0b0/drakaina/wsgi.py
--rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.0b0/LICENSE
--rw-r--r--   0        0        0     2714 2023-05-17 12:47:04.923326 drakaina-0.7.0b0/pyproject.toml
--rw-r--r--   0        0        0     5416 2023-05-17 12:47:04.916302 drakaina-0.7.0b0/README.md
--rw-r--r--   0        0        0     6701 1970-01-01 00:00:00.000000 drakaina-0.7.0b0/setup.py
--rw-r--r--   0        0        0     6933 1970-01-01 00:00:00.000000 drakaina-0.7.0b0/PKG-INFO
+-rw-r--r--   0        0        0     9578 2023-05-30 12:08:58.530489 drakaina-0.7.0b3/drakaina/__init__.py
+-rw-r--r--   0        0        0     1494 2023-01-27 12:48:38.216236 drakaina-0.7.0b3/drakaina/asgi.py
+-rw-r--r--   0        0        0     3699 2023-02-13 13:22:12.183448 drakaina-0.7.0b3/drakaina/client/__init__.py
+-rw-r--r--   0        0        0     6158 2022-07-08 05:47:38.000000 drakaina-0.7.0b3/drakaina/client/base.py
+-rw-r--r--   0        0        0     1832 2022-07-08 05:47:38.000000 drakaina-0.7.0b3/drakaina/client/http.py
+-rw-r--r--   0        0        0    11280 2023-01-27 12:55:37.114745 drakaina-0.7.0b3/drakaina/client/tcp.py
+-rw-r--r--   0        0        0     8797 2022-07-08 05:47:38.000000 drakaina-0.7.0b3/drakaina/client/websocket.py
+-rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.0b3/drakaina/contrib/__init__.py
+-rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.0b3/drakaina/contrib/django/__init__.py
+-rw-r--r--   0        0        0     6132 2023-04-11 08:46:20.669302 drakaina-0.7.0b3/drakaina/contrib/django/middleware.py
+-rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.0b3/drakaina/contrib/django/views.py
+-rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.0b3/drakaina/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0      348 2023-03-10 11:02:10.213372 drakaina-0.7.0b3/drakaina/contrib/jwt/errors.py
+-rw-r--r--   0        0        0     9095 2023-05-30 12:08:58.531504 drakaina-0.7.0b3/drakaina/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0      911 2023-05-29 22:21:28.708378 drakaina-0.7.0b3/drakaina/contrib/jwt/types.py
+-rw-r--r--   0        0        0    18791 2023-05-30 12:08:58.532513 drakaina-0.7.0b3/drakaina/contrib/jwt/utils.py
+-rw-r--r--   0        0        0     4115 2023-05-28 21:21:43.059480 drakaina-0.7.0b3/drakaina/drakaina_openapi.py
+-rw-r--r--   0        0        0     1327 2023-05-11 09:46:59.367413 drakaina-0.7.0b3/drakaina/exceptions.py
+-rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.0b3/drakaina/middleware/__init__.py
+-rw-r--r--   0        0        0     1370 2023-05-29 22:21:28.722375 drakaina-0.7.0b3/drakaina/middleware/base.py
+-rw-r--r--   0        0        0     7579 2023-05-30 12:08:58.533488 drakaina-0.7.0b3/drakaina/middleware/cors.py
+-rw-r--r--   0        0        0     2032 2023-05-30 12:08:58.533488 drakaina-0.7.0b3/drakaina/middleware/exception.py
+-rw-r--r--   0        0        0      430 2023-04-13 16:28:59.822156 drakaina-0.7.0b3/drakaina/middleware/gzip.py
+-rw-r--r--   0        0        0      983 2023-04-04 11:19:41.525282 drakaina-0.7.0b3/drakaina/middleware/logging.py
+-rw-r--r--   0        0        0     1072 2023-05-29 22:42:27.401282 drakaina-0.7.0b3/drakaina/middleware/request_wrapper.py
+-rw-r--r--   0        0        0    12637 2023-05-30 12:08:58.534489 drakaina-0.7.0b3/drakaina/registries.py
+-rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.0b3/drakaina/rpc_protocols/__init__.py
+-rw-r--r--   0        0        0     7537 2023-05-30 12:08:58.535504 drakaina-0.7.0b3/drakaina/rpc_protocols/base.py
+-rw-r--r--   0        0        0    21236 2023-05-30 12:08:58.536491 drakaina-0.7.0b3/drakaina/rpc_protocols/jsonrpc20.py
+-rw-r--r--   0        0        0      200 2023-01-09 10:12:10.047554 drakaina-0.7.0b3/drakaina/rsgi.py
+-rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.0b3/drakaina/serializers.py
+-rw-r--r--   0        0        0    11142 2023-01-27 12:51:42.029067 drakaina-0.7.0b3/drakaina/tcp.py
+-rw-r--r--   0        0        0    21947 2023-05-30 12:08:58.536491 drakaina-0.7.0b3/drakaina/types.py
+-rw-r--r--   0        0        0     3746 2023-05-30 12:08:58.537488 drakaina-0.7.0b3/drakaina/utils.py
+-rw-r--r--   0        0        0      162 2023-01-25 16:44:10.299855 drakaina-0.7.0b3/drakaina/ws.py
+-rw-r--r--   0        0        0     8452 2023-05-30 12:08:58.538489 drakaina-0.7.0b3/drakaina/wsgi.py
+-rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.0b3/LICENSE
+-rw-r--r--   0        0        0     2685 2023-05-30 12:08:58.538489 drakaina-0.7.0b3/pyproject.toml
+-rw-r--r--   0        0        0     5416 2023-05-30 12:08:58.530489 drakaina-0.7.0b3/README.md
+-rw-r--r--   0        0        0     6671 1970-01-01 00:00:00.000000 drakaina-0.7.0b3/setup.py
+-rw-r--r--   0        0        0     6884 1970-01-01 00:00:00.000000 drakaina-0.7.0b3/PKG-INFO
```

### Comparing `drakaina-0.7.0b0/drakaina/__init__.py` & `drakaina-0.7.0b3/drakaina/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from typing import Any
 from typing import Callable
 from typing import Iterable
 from typing import MutableMapping
 from typing import Optional
 from typing import TypeVar
 
-from drakaina._types import AnyRequest
-from drakaina._types import Comparator
 from drakaina.exceptions import AuthenticationFailedError
 from drakaina.exceptions import ForbiddenError
 from drakaina.registries import RPC_REGISTRY
 from drakaina.registries import RPCRegistry
+from drakaina.types import AnyRequest
+from drakaina.types import Comparator
 from drakaina.utils import iterable_str_arg
 
 __all__ = (
     "RPCRegistry",
     "rpc_registry",
     "remote_procedure",
     "check_permissions",
```

### Comparing `drakaina-0.7.0b0/drakaina/asgi.py` & `drakaina-0.7.0b3/drakaina/asgi.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/client/__init__.py` & `drakaina-0.7.0b3/drakaina/client/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/client/base.py` & `drakaina-0.7.0b3/drakaina/client/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/client/http.py` & `drakaina-0.7.0b3/drakaina/client/http.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/client/tcp.py` & `drakaina-0.7.0b3/drakaina/client/tcp.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/client/websocket.py` & `drakaina-0.7.0b3/drakaina/client/websocket.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/contrib/django/__init__.py` & `drakaina-0.7.0b3/drakaina/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/contrib/django/middleware.py` & `drakaina-0.7.0b3/drakaina/contrib/django/middleware.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/contrib/django/views.py` & `drakaina-0.7.0b3/drakaina/contrib/django/views.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/contrib/jwt/middleware.py` & `drakaina-0.7.0b3/drakaina/contrib/jwt/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 from typing import Iterable
 
 from drakaina import ENV_AUTH_PAYLOAD
 from drakaina import ENV_AUTH_SCOPES
 from drakaina import ENV_IS_AUTHENTICATED
 from drakaina import ENV_USER
 from drakaina import ENV_USER_ID
-from drakaina._types import ASGIReceive
-from drakaina._types import ASGIScope
-from drakaina._types import ASGISend
-from drakaina._types import WSGIApplication
-from drakaina._types import WSGIEnvironment
-from drakaina._types import WSGIResponse
-from drakaina._types import WSGIStartResponse
 from drakaina.contrib.jwt import SUPPORTED_ALGORITHMS
 from drakaina.contrib.jwt.errors import InvalidJWTTokenError
 from drakaina.contrib.jwt.types import RevokeChecker
 from drakaina.contrib.jwt.types import ScopesGetter
 from drakaina.contrib.jwt.types import TokenGetter
 from drakaina.contrib.jwt.types import UserGetter
 from drakaina.contrib.jwt.utils import decode_jwt_token
 from drakaina.exceptions import AuthenticationFailedError
 from drakaina.exceptions import ForbiddenError
 from drakaina.middleware.base import BaseMiddleware
+from drakaina.types import ASGIReceive
+from drakaina.types import ASGIScope
+from drakaina.types import ASGISend
+from drakaina.types import WSGIApplication
+from drakaina.types import WSGIEnvironment
+from drakaina.types import WSGIResponse
+from drakaina.types import WSGIStartResponse
 from drakaina.utils import get_cookies
 from drakaina.utils import iterable_str_arg
 
 
 class JWTAuthenticationMiddleware(BaseMiddleware):
     """The middleware supporting JWT tokens.
```

### Comparing `drakaina-0.7.0b0/drakaina/contrib/jwt/types.py` & `drakaina-0.7.0b3/drakaina/contrib/jwt/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import Any
 from typing import Iterable
 from typing import Optional
 from typing import Protocol
 
-from drakaina._types import ASGIScope
-from drakaina._types import WSGIEnvironment
+from drakaina.types import ASGIScope
+from drakaina.types import WSGIEnvironment
 
 
 class TokenGetter(Protocol):
     def __call__(
         self,
         request: ASGIScope | WSGIEnvironment,
     ) -> Optional[str]:
```

### Comparing `drakaina-0.7.0b0/drakaina/contrib/jwt/utils.py` & `drakaina-0.7.0b3/drakaina/contrib/jwt/utils.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/exceptions.py` & `drakaina-0.7.0b3/drakaina/exceptions.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/middleware/base.py` & `drakaina-0.7.0b3/drakaina/middleware/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
-from drakaina._types import ASGIApplication
-from drakaina._types import ASGIReceive
-from drakaina._types import ASGIScope
-from drakaina._types import ASGISend
-from drakaina._types import WSGIApplication
-from drakaina._types import WSGIEnvironment
-from drakaina._types import WSGIResponse
-from drakaina._types import WSGIStartResponse
+from drakaina.types import ASGIApplication
+from drakaina.types import ASGIReceive
+from drakaina.types import ASGIScope
+from drakaina.types import ASGISend
+from drakaina.types import WSGIApplication
+from drakaina.types import WSGIEnvironment
+from drakaina.types import WSGIResponse
+from drakaina.types import WSGIStartResponse
 
 
 __all__ = ("BaseMiddleware",)
 
 
 class BaseMiddleware:
     """Base class for middleware.
```

### Comparing `drakaina-0.7.0b0/drakaina/middleware/cors.py` & `drakaina-0.7.0b3/drakaina/middleware/cors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 from typing import Iterable
 from typing import Optional
 
-from drakaina._types import ASGIReceive
-from drakaina._types import ASGIScope
-from drakaina._types import ASGISend
-from drakaina._types import WSGIApplication
-from drakaina._types import WSGIEnvironment
-from drakaina._types import WSGIResponse
-from drakaina._types import WSGIStartResponse
 from drakaina.middleware.base import BaseMiddleware
+from drakaina.types import ASGIReceive
+from drakaina.types import ASGIScope
+from drakaina.types import ASGISend
+from drakaina.types import WSGIApplication
+from drakaina.types import WSGIEnvironment
+from drakaina.types import WSGIResponse
+from drakaina.types import WSGIStartResponse
 from drakaina.utils import iterable_str_arg
 
 __all__ = ("CORSMiddleware",)
 
 DEFAULT_HEADERS = (
     "Accept, Accept-Encoding, Accept-Language, Authorization, "
     "Content-Language, Content-Type, DNT, Origin, User-Agent, X-Requested-With"
```

### Comparing `drakaina-0.7.0b0/drakaina/middleware/exception.py` & `drakaina-0.7.0b3/drakaina/middleware/exception.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from logging import Logger
 
-from drakaina._types import ASGIApplication
-from drakaina._types import ASGIReceive
-from drakaina._types import ASGIScope
-from drakaina._types import ASGISend
-from drakaina._types import WSGIApplication
-from drakaina._types import WSGIEnvironment
-from drakaina._types import WSGIResponse
-from drakaina._types import WSGIStartResponse
 from drakaina.middleware.base import BaseMiddleware
 from drakaina.rpc_protocols import BaseRPCProtocol
+from drakaina.types import ASGIApplication
+from drakaina.types import ASGIReceive
+from drakaina.types import ASGIScope
+from drakaina.types import ASGISend
+from drakaina.types import WSGIApplication
+from drakaina.types import WSGIEnvironment
+from drakaina.types import WSGIResponse
+from drakaina.types import WSGIStartResponse
 
 
 class ExceptionMiddleware(BaseMiddleware):
     """The middleware for handling unhandled exceptions in the application
     according to the RPC protocol.
 
     """
```

### Comparing `drakaina-0.7.0b0/drakaina/middleware/logging.py` & `drakaina-0.7.0b3/drakaina/middleware/logging.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/middleware/request_wrapper.py` & `drakaina-0.7.0b3/drakaina/middleware/request_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from drakaina._types import ASGIReceive
-from drakaina._types import ASGIScope
-from drakaina._types import ASGISend
-from drakaina._types import ProxyRequest
-from drakaina._types import WSGIEnvironment
-from drakaina._types import WSGIResponse
-from drakaina._types import WSGIStartResponse
 from drakaina.middleware.base import BaseMiddleware
+from drakaina.types import ASGIReceive
+from drakaina.types import ASGIScope
+from drakaina.types import ASGISend
+from drakaina.types import ProxyRequest
+from drakaina.types import WSGIEnvironment
+from drakaina.types import WSGIResponse
+from drakaina.types import WSGIStartResponse
 
 
 class RequestWrapperMiddleware(BaseMiddleware):
     """The middleware for wrapping the request object.
 
     Provides access to the mapping environment object through
     the attribute access interface. This is needed for some
```

### Comparing `drakaina-0.7.0b0/drakaina/registries.py` & `drakaina-0.7.0b3/drakaina/registries.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from typing import Any
 from typing import Iterable
 from typing import Iterator
 from typing import KeysView
 from typing import Mapping
 from typing import ValuesView
 
-from drakaina._types import MethodSchema
-from drakaina._types import ParameterSchema
+from drakaina.types import MethodSchema
+from drakaina.types import ParameterSchema
 from drakaina.utils import short_description_by_name
 from drakaina.utils import unwrap_func
 
 try:
     from docstring_parser import parse as parse_doc
 except ImportError:
     parse_doc = None
```

### Comparing `drakaina-0.7.0b0/drakaina/serializers.py` & `drakaina-0.7.0b3/drakaina/serializers.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/tcp.py` & `drakaina-0.7.0b3/drakaina/tcp.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/drakaina/utils.py` & `drakaina-0.7.0b3/drakaina/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     while hasattr(_func, "__wrapped__") or isinstance(_func, partial):
         _func = getattr(_func, "__wrapped__", None) or _func.func
     return _func
 
 
 def short_description_by_name(s: str) -> str:
     if isinstance(s, str):
-        return re.sub(r"[\.-_]", " ", s).title()
+        return re.sub(r"[\.-_]", " ", s).capitalize()
 
 
 def get_cookies(cookie_str: str) -> dict[str, str]:
     if cookie_str is None:
         return {}
 
     _cookies = {}
```

### Comparing `drakaina-0.7.0b0/drakaina/wsgi.py` & `drakaina-0.7.0b3/drakaina/wsgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 import re
 from functools import partial
 from logging import Logger
 from sys import version_info
 from typing import Iterable
 
 from drakaina import ENV_APP
-from drakaina._types import WSGIApplication
-from drakaina._types import WSGIEnvironment
-from drakaina._types import WSGIInputStream
-from drakaina._types import WSGIResponse
-from drakaina._types import WSGIStartResponse
 from drakaina.exceptions import BadRequestError
 from drakaina.middleware.base import BaseMiddleware
 from drakaina.middleware.exception import ExceptionMiddleware
 from drakaina.middleware.request_wrapper import RequestWrapperMiddleware
 from drakaina.rpc_protocols import BaseRPCProtocol
 from drakaina.rpc_protocols import JsonRPCv2
+from drakaina.types import WSGIApplication
+from drakaina.types import WSGIEnvironment
+from drakaina.types import WSGIInputStream
+from drakaina.types import WSGIResponse
+from drakaina.types import WSGIStartResponse
 from drakaina.utils import match_path
 
 if version_info < (3, 9):
     from typing import Type
     from typing import Union
     from typing_extensions import TypeAlias
 
@@ -99,14 +99,21 @@
     ):
         self.handler = handler if handler is not None else JsonRPCv2()
         self._rpc_content_type = self.handler.content_type
 
         self.route = route
         if isinstance(self.route, str) and not self.route.startswith("/"):
             self.route = "/" + self.route
+        schema_url = getattr(self.handler, "schema_url", None)
+        if (
+            self.route is not None
+            and hasattr(self.handler, "schema_url")
+            and schema_url is None
+        ):
+            setattr(self.handler, "schema_url", self.route)
 
         self.logger = logger
         self.max_content_size = int(max_content_size)
         self.openrpc_url = openrpc_url
         self.openapi_url = openapi_url
 
         if openrpc_url or openapi_url:
```

### Comparing `drakaina-0.7.0b0/LICENSE` & `drakaina-0.7.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/pyproject.toml` & `drakaina-0.7.0b3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drakaina"
-version = "0.7.0-beta.0"
+version = "0.7.0-beta.3"
 description = "Module for simple RPC service implementation"
 authors = ["Aleksey Terentyev <terentyev.a@pm.me>"]
 license = "Apache License 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
@@ -20,39 +20,39 @@
 homepage  = "https://gitlab.com/tau_lex/drakaina"
 repository = "https://gitlab.com/tau_lex/drakaina"
 
 [project.urls]
 "Bug Tracker" = "https://gitlab.com/tau_lex/drakaina/-/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-typing-extensions = "^4.5.0"
-msgpack = { version = "^1.0.4", optional = true }
-orjson = { version = "^3.8.5", optional = true }
+python = "^3.8"
+typing-extensions = "^4.6.2"
+msgpack = { version = "^1.0.5", optional = true }
+orjson = { version = "^3.8.14", optional = true }
 ujson = { version = "^5.7.0", optional = true }
-pyjwt = { version = "^2.6.0", optional = true }
+pyjwt = { version = "^2.7.0", optional = true }
 docstring-parser = { version = "^0.15", optional = true }
 
 [tool.poetry.extras]
 jwt = ["PyJWT"]
 ujson = ["ujson"]
 orjson = ["orjson"]
 msgpack = ["msgpack"]
 docs = ["docstring-parser"]
 tests = ["pytest", "httpx", "ujson", "orjson", "msgpack", "pyjwt", "django", "docstring-parser"]
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["d"], version = "^22.12.0"}
-pre-commit = {version = "^3.0.0", python = ">=3.8"}
-ruff = "^0.0.236"
+pre-commit = "^3.3.2"
+ruff = "^0.0.269"
 msgpack = "^1.0.4"
 orjson = "^3.8.6"
-pytest = "^7.2.1"
+pytest = "^7.3.1"
 ujson = "^5.7.0"
-pyjwt = "^2.6.0"
+pyjwt = "^2.7.0"
 django = ">=3.2"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.2.1"
 httpx = "^0.23.3"
 
 [tool.pytest.ini_options]
@@ -82,20 +82,20 @@
 
 # Same as Black.
 line-length = 80
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-target-version = "py37"
+target-version = "py38"
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 80
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `drakaina-0.7.0b0/README.md` & `drakaina-0.7.0b3/README.md`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b0/setup.py` & `drakaina-0.7.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,47 +4,46 @@
 packages = \
 ['drakaina',
  'drakaina.client',
  'drakaina.contrib',
  'drakaina.contrib.django',
  'drakaina.contrib.jwt',
  'drakaina.middleware',
- 'drakaina.middleware.openapi',
  'drakaina.rpc_protocols']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['typing-extensions>=4.5.0,<5.0.0']
+['typing-extensions>=4.6.2,<5.0.0']
 
 extras_require = \
 {'docs': ['docstring-parser>=0.15,<0.16'],
- 'jwt': ['pyjwt>=2.6.0,<3.0.0'],
- 'msgpack': ['msgpack>=1.0.4,<2.0.0'],
- 'orjson': ['orjson>=3.8.5,<4.0.0'],
- 'tests': ['msgpack>=1.0.4,<2.0.0',
-           'orjson>=3.8.5,<4.0.0',
+ 'jwt': ['pyjwt>=2.7.0,<3.0.0'],
+ 'msgpack': ['msgpack>=1.0.5,<2.0.0'],
+ 'orjson': ['orjson>=3.8.14,<4.0.0'],
+ 'tests': ['msgpack>=1.0.5,<2.0.0',
+           'orjson>=3.8.14,<4.0.0',
            'ujson>=5.7.0,<6.0.0',
-           'pyjwt>=2.6.0,<3.0.0',
+           'pyjwt>=2.7.0,<3.0.0',
            'docstring-parser>=0.15,<0.16'],
  'ujson': ['ujson>=5.7.0,<6.0.0']}
 
 setup_kwargs = {
     'name': 'drakaina',
-    'version': '0.7.0b0',
+    'version': '0.7.0b3',
     'description': 'Module for simple RPC service implementation',
     'long_description': '# drakaina\n\n![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}\n\n[![image](https://img.shields.io/pypi/v/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![image](https://img.shields.io/pypi/l/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![image](https://img.shields.io/pypi/pyversions/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n[![libera manifesto](https://img.shields.io/badge/libera-manifesto-lightgrey.svg)](https://liberamanifesto.com)\n\n❗ WIP ❗\n\nFramework for simple RPC service implementation.\n\n\n## Quickstart\n\nDrakaina may be installed via `pip` and requires Python 3.7 or higher :\n\n```shell\npip install drakaina\n```\n\nA minimal Drakaina example is:\n\n```python\nfrom drakaina import remote_procedure\nfrom drakaina.wsgi import WSGIHandler\n\n@remote_procedure("hello")\ndef hello_method(name):\n    return f"Hello, {name}!"\n\n"""\n>>> from drakaina.rpc_protocols import JsonRPCv2\n>>> JsonRPCv2().handle({"jsonrpc": "2.0", "method": "hello", "params": ["🐍 Python"] "id": 1})\n{"jsonrpc": "2.0", "result": "Hello, 🐍 Python!", "id": 1}\n"""\n\n# Or define WSGI application\napp = WSGIHandler(route="/jrpc")\n\n```\n\n\n## Features\n\n- Serializers layer.\n  - `json`, `orjson`, `ujson` and `msgpack` serializers.\n- Generates schemas for documentation in OpenRPC format.\n- WSGI protocol implementation\n  - CORS middleware\n  - JWT Authorization middleware.\n  - Compatible with middlewares for others wsgi-frameworks,\n    like as [Werkzeug](https://palletsprojects.com/p/werkzeug/),\n    [Flask](https://palletsprojects.com/p/flask/)\n- `login_required` and `check_permissions` decorators.\n\n\n# Documentation\n\n\n## Installation\n\n```shell\npip install drakaina\n```\n\n\n## Middlewares\n\n\n### CORS\n\n\n### JWT\n\nDrakaina may be installed via `pip` and requires Python 3.7 or higher :\n\n```shell\npip install drakaina[jwt]\n```\n\nExample of using Drakaina:\n\n```python\nfrom functools import partial\nfrom drakaina import check_permissions\nfrom drakaina import ENV_IS_AUTHENTICATED\nfrom drakaina import ENV_USER_ID\nfrom drakaina import login_required\nfrom drakaina import match_any\nfrom drakaina import remote_procedure\nfrom drakaina.contrib.jwt.middleware import JWTAuthenticationMiddleware\nfrom drakaina.wsgi import WSGIHandler\n\nimport user_store\n\n\n@login_required\n@remote_procedure(provide_request=True)\ndef my_method(request):\n    assert request[ENV_IS_AUTHENTICATED]\n    return f"Hello Bro ✋! Your ID={request[ENV_USER_ID]}"\n\n\n@check_permissions(["user_read", "user:admin", "username:johndoe"], match_any)\n@remote_procedure\ndef my_method():\n    return "Hello Bro! ✋️"\n\n\ndef get_user(request, payload):\n    user_id = request[ENV_USER_ID] or payload["user_id"]\n    return user_store.get(id=user_id)\n\n\ndef get_jwt_scopes(request, payload):\n    # here `scp` is the key for the scopes value in the token payload\n    return payload.get("scp")\n\n\napp = WSGIHandler(\n    middlewares=[\n        partial(\n            JWTAuthenticationMiddleware,\n            secret_phrase="_secret_",\n            credentials_required=True,\n            auth_scheme="Bearer",\n            # token_getter=custom_implementation_get_token,\n            user_getter=get_user,\n            scopes_getter=get_jwt_scopes,\n            # revoke_checker=is_revoked,\n        )\n    ]\n)\n```\n\nDrakaina may be ran with any WSGI-compliant server,\nsuch as [Gunicorn](http://gunicorn.org).\n\n```shell\ngunicorn main:app\n```\n\nor ran with any ASGI-compliant server\n\n```shell\nuvicorn main:app2\n```\n\n\n### Using with Django\n\nCreate file `rpc_views.py` in your django application.\nDefine function and wrap it `remote_procedure` decorator:\n\n```python\nfrom drakaina import remote_procedure\n\n@remote_procedure\ndef my_method():\n    return "Hello, Django Bro! ✋"\n```\n\nAdd `RPCView` class to urlpatterns. The `as_view` method\nmust accept the `autodiscover` argument as the name of\nthe remote procedure files.\n\n```python\nfrom django.urls import path\nfrom drakaina.contrib.django.views import RPCView\n\nurlpatterns = [\n    ...,\n    path("api/", RPCView.as_view(autodiscover="rpc_views")),\n]\n```\n\n\n### JWT Authentication in your Django project\n\nWrap an instance of `RPCView` with the `JWTAuthenticationMiddleware`.\n\n```python\nfrom django.urls import path\nfrom drakaina.contrib.django import RPCView, JWTAuthenticationMiddleware\n\nurlpatterns = [\n    ...,\n    path("api/", JWTAuthenticationMiddleware(\n        RPCView.as_view(autodiscover="rpc_views")\n    )),\n]\n```\n\nDefine the parameters in the `settings.py` file.\n\n```python\n...\n\nDRAKAINA_JWT_SECRET_KEY = "__SECRET_KEY__"\n\n...\n```\n\n\n## License\n\nApache License 2.0\n\n## Artwork\n\n"[drakaina.png](content/drakaina.png)" by Korolko Anastasia is licensed under\n<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="License Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a> ([CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)).\n',
     'author': 'Aleksey Terentyev',
     'author_email': 'terentyev.a@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/tau_lex/drakaina',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `drakaina-0.7.0b0/PKG-INFO` & `drakaina-0.7.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: drakaina
-Version: 0.7.0b0
+Version: 0.7.0b3
 Summary: Module for simple RPC service implementation
 Home-page: https://gitlab.com/tau_lex/drakaina
 License: Apache-2.0
 Keywords: rpc,jsonrpc
 Author: Aleksey Terentyev
 Author-email: terentyev.a@pm.me
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -26,18 +25,18 @@
 Provides-Extra: docs
 Provides-Extra: jwt
 Provides-Extra: msgpack
 Provides-Extra: orjson
 Provides-Extra: tests
 Provides-Extra: ujson
 Requires-Dist: docstring-parser (>=0.15,<0.16) ; extra == "docs" or extra == "tests"
-Requires-Dist: msgpack (>=1.0.4,<2.0.0) ; extra == "msgpack" or extra == "tests"
-Requires-Dist: orjson (>=3.8.5,<4.0.0) ; extra == "orjson" or extra == "tests"
-Requires-Dist: pyjwt (>=2.6.0,<3.0.0) ; extra == "jwt" or extra == "tests"
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Requires-Dist: msgpack (>=1.0.5,<2.0.0) ; extra == "msgpack" or extra == "tests"
+Requires-Dist: orjson (>=3.8.14,<4.0.0) ; extra == "orjson" or extra == "tests"
+Requires-Dist: pyjwt (>=2.7.0,<3.0.0) ; extra == "jwt" or extra == "tests"
+Requires-Dist: typing-extensions (>=4.6.2,<5.0.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0) ; extra == "ujson" or extra == "tests"
 Project-URL: Repository, https://gitlab.com/tau_lex/drakaina
 Description-Content-Type: text/markdown
 
 # drakaina
 
 ![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}
```

