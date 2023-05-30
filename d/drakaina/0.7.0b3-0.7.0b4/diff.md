# Comparing `tmp/drakaina-0.7.0b3.tar.gz` & `tmp/drakaina-0.7.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drakaina-0.7.0b3.tar", max compression
+gzip compressed data, was "drakaina-0.7.0b4.tar", max compression
```

## Comparing `drakaina-0.7.0b3.tar` & `drakaina-0.7.0b4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     9578 2023-05-30 12:08:58.530489 drakaina-0.7.0b3/drakaina/__init__.py
--rw-r--r--   0        0        0     1494 2023-01-27 12:48:38.216236 drakaina-0.7.0b3/drakaina/asgi.py
--rw-r--r--   0        0        0     3699 2023-02-13 13:22:12.183448 drakaina-0.7.0b3/drakaina/client/__init__.py
--rw-r--r--   0        0        0     6158 2022-07-08 05:47:38.000000 drakaina-0.7.0b3/drakaina/client/base.py
--rw-r--r--   0        0        0     1832 2022-07-08 05:47:38.000000 drakaina-0.7.0b3/drakaina/client/http.py
--rw-r--r--   0        0        0    11280 2023-01-27 12:55:37.114745 drakaina-0.7.0b3/drakaina/client/tcp.py
--rw-r--r--   0        0        0     8797 2022-07-08 05:47:38.000000 drakaina-0.7.0b3/drakaina/client/websocket.py
--rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.0b3/drakaina/contrib/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.0b3/drakaina/contrib/django/__init__.py
--rw-r--r--   0        0        0     6132 2023-04-11 08:46:20.669302 drakaina-0.7.0b3/drakaina/contrib/django/middleware.py
--rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.0b3/drakaina/contrib/django/views.py
--rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.0b3/drakaina/contrib/jwt/__init__.py
--rw-r--r--   0        0        0      348 2023-03-10 11:02:10.213372 drakaina-0.7.0b3/drakaina/contrib/jwt/errors.py
--rw-r--r--   0        0        0     9095 2023-05-30 12:08:58.531504 drakaina-0.7.0b3/drakaina/contrib/jwt/middleware.py
--rw-r--r--   0        0        0      911 2023-05-29 22:21:28.708378 drakaina-0.7.0b3/drakaina/contrib/jwt/types.py
--rw-r--r--   0        0        0    18791 2023-05-30 12:08:58.532513 drakaina-0.7.0b3/drakaina/contrib/jwt/utils.py
--rw-r--r--   0        0        0     4115 2023-05-28 21:21:43.059480 drakaina-0.7.0b3/drakaina/drakaina_openapi.py
--rw-r--r--   0        0        0     1327 2023-05-11 09:46:59.367413 drakaina-0.7.0b3/drakaina/exceptions.py
--rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.0b3/drakaina/middleware/__init__.py
--rw-r--r--   0        0        0     1370 2023-05-29 22:21:28.722375 drakaina-0.7.0b3/drakaina/middleware/base.py
--rw-r--r--   0        0        0     7579 2023-05-30 12:08:58.533488 drakaina-0.7.0b3/drakaina/middleware/cors.py
--rw-r--r--   0        0        0     2032 2023-05-30 12:08:58.533488 drakaina-0.7.0b3/drakaina/middleware/exception.py
--rw-r--r--   0        0        0      430 2023-04-13 16:28:59.822156 drakaina-0.7.0b3/drakaina/middleware/gzip.py
--rw-r--r--   0        0        0      983 2023-04-04 11:19:41.525282 drakaina-0.7.0b3/drakaina/middleware/logging.py
--rw-r--r--   0        0        0     1072 2023-05-29 22:42:27.401282 drakaina-0.7.0b3/drakaina/middleware/request_wrapper.py
--rw-r--r--   0        0        0    12637 2023-05-30 12:08:58.534489 drakaina-0.7.0b3/drakaina/registries.py
--rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.0b3/drakaina/rpc_protocols/__init__.py
--rw-r--r--   0        0        0     7537 2023-05-30 12:08:58.535504 drakaina-0.7.0b3/drakaina/rpc_protocols/base.py
--rw-r--r--   0        0        0    21236 2023-05-30 12:08:58.536491 drakaina-0.7.0b3/drakaina/rpc_protocols/jsonrpc20.py
--rw-r--r--   0        0        0      200 2023-01-09 10:12:10.047554 drakaina-0.7.0b3/drakaina/rsgi.py
--rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.0b3/drakaina/serializers.py
--rw-r--r--   0        0        0    11142 2023-01-27 12:51:42.029067 drakaina-0.7.0b3/drakaina/tcp.py
--rw-r--r--   0        0        0    21947 2023-05-30 12:08:58.536491 drakaina-0.7.0b3/drakaina/types.py
--rw-r--r--   0        0        0     3746 2023-05-30 12:08:58.537488 drakaina-0.7.0b3/drakaina/utils.py
--rw-r--r--   0        0        0      162 2023-01-25 16:44:10.299855 drakaina-0.7.0b3/drakaina/ws.py
--rw-r--r--   0        0        0     8452 2023-05-30 12:08:58.538489 drakaina-0.7.0b3/drakaina/wsgi.py
--rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.0b3/LICENSE
--rw-r--r--   0        0        0     2685 2023-05-30 12:08:58.538489 drakaina-0.7.0b3/pyproject.toml
--rw-r--r--   0        0        0     5416 2023-05-30 12:08:58.530489 drakaina-0.7.0b3/README.md
--rw-r--r--   0        0        0     6671 1970-01-01 00:00:00.000000 drakaina-0.7.0b3/setup.py
--rw-r--r--   0        0        0     6884 1970-01-01 00:00:00.000000 drakaina-0.7.0b3/PKG-INFO
+-rw-r--r--   0        0        0     9270 2023-05-30 13:55:11.975948 drakaina-0.7.0b4/drakaina/__init__.py
+-rw-r--r--   0        0        0     1494 2023-01-27 12:48:38.216236 drakaina-0.7.0b4/drakaina/asgi.py
+-rw-r--r--   0        0        0     3699 2023-02-13 13:22:12.183448 drakaina-0.7.0b4/drakaina/client/__init__.py
+-rw-r--r--   0        0        0     6158 2022-07-08 05:47:38.000000 drakaina-0.7.0b4/drakaina/client/base.py
+-rw-r--r--   0        0        0     1832 2022-07-08 05:47:38.000000 drakaina-0.7.0b4/drakaina/client/http.py
+-rw-r--r--   0        0        0    11280 2023-01-27 12:55:37.114745 drakaina-0.7.0b4/drakaina/client/tcp.py
+-rw-r--r--   0        0        0     8797 2022-07-08 05:47:38.000000 drakaina-0.7.0b4/drakaina/client/websocket.py
+-rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.0b4/drakaina/contrib/__init__.py
+-rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.0b4/drakaina/contrib/django/__init__.py
+-rw-r--r--   0        0        0     6132 2023-04-11 08:46:20.669302 drakaina-0.7.0b4/drakaina/contrib/django/middleware.py
+-rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.0b4/drakaina/contrib/django/views.py
+-rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.0b4/drakaina/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0      348 2023-03-10 11:02:10.213372 drakaina-0.7.0b4/drakaina/contrib/jwt/errors.py
+-rw-r--r--   0        0        0     8847 2023-05-30 13:55:11.976951 drakaina-0.7.0b4/drakaina/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0      911 2023-05-29 22:21:28.708378 drakaina-0.7.0b4/drakaina/contrib/jwt/types.py
+-rw-r--r--   0        0        0    18201 2023-05-30 13:55:11.977951 drakaina-0.7.0b4/drakaina/contrib/jwt/utils.py
+-rw-r--r--   0        0        0     4115 2023-05-28 21:21:43.059480 drakaina-0.7.0b4/drakaina/drakaina_openapi.py
+-rw-r--r--   0        0        0     1327 2023-05-11 09:46:59.367413 drakaina-0.7.0b4/drakaina/exceptions.py
+-rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.0b4/drakaina/middleware/__init__.py
+-rw-r--r--   0        0        0     1370 2023-05-29 22:21:28.722375 drakaina-0.7.0b4/drakaina/middleware/base.py
+-rw-r--r--   0        0        0     7364 2023-05-30 13:55:11.978951 drakaina-0.7.0b4/drakaina/middleware/cors.py
+-rw-r--r--   0        0        0     1967 2023-05-30 13:55:11.980056 drakaina-0.7.0b4/drakaina/middleware/exception.py
+-rw-r--r--   0        0        0      430 2023-04-13 16:28:59.822156 drakaina-0.7.0b4/drakaina/middleware/gzip.py
+-rw-r--r--   0        0        0      983 2023-04-04 11:19:41.525282 drakaina-0.7.0b4/drakaina/middleware/logging.py
+-rw-r--r--   0        0        0     1072 2023-05-29 22:42:27.401282 drakaina-0.7.0b4/drakaina/middleware/request_wrapper.py
+-rw-r--r--   0        0        0    12285 2023-05-30 13:55:11.980056 drakaina-0.7.0b4/drakaina/registries.py
+-rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.0b4/drakaina/rpc_protocols/__init__.py
+-rw-r--r--   0        0        0     7317 2023-05-30 13:55:11.981055 drakaina-0.7.0b4/drakaina/rpc_protocols/base.py
+-rw-r--r--   0        0        0    20624 2023-05-30 13:55:11.982509 drakaina-0.7.0b4/drakaina/rpc_protocols/jsonrpc20.py
+-rw-r--r--   0        0        0      200 2023-01-09 10:12:10.047554 drakaina-0.7.0b4/drakaina/rsgi.py
+-rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.0b4/drakaina/serializers.py
+-rw-r--r--   0        0        0    11142 2023-01-27 12:51:42.029067 drakaina-0.7.0b4/drakaina/tcp.py
+-rw-r--r--   0        0        0    22700 2023-05-30 13:55:11.982509 drakaina-0.7.0b4/drakaina/types.py
+-rw-r--r--   0        0        0     3625 2023-05-30 13:55:11.983500 drakaina-0.7.0b4/drakaina/utils.py
+-rw-r--r--   0        0        0      162 2023-01-25 16:44:10.299855 drakaina-0.7.0b4/drakaina/ws.py
+-rw-r--r--   0        0        0     8212 2023-05-30 13:55:11.984506 drakaina-0.7.0b4/drakaina/wsgi.py
+-rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.0b4/LICENSE
+-rw-r--r--   0        0        0     2595 2023-05-30 13:55:11.984506 drakaina-0.7.0b4/pyproject.toml
+-rw-r--r--   0        0        0     5200 2023-05-30 13:55:11.974952 drakaina-0.7.0b4/README.md
+-rw-r--r--   0        0        0     6671 1970-01-01 00:00:00.000000 drakaina-0.7.0b4/setup.py
+-rw-r--r--   0        0        0     6892 1970-01-01 00:00:00.000000 drakaina-0.7.0b4/PKG-INFO
```

### Comparing `drakaina-0.7.0b3/drakaina/__init__.py` & `drakaina-0.7.0b4/drakaina/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,308 +1,308 @@
-from __future__ import annotations
-
-from asyncio import iscoroutinefunction
-from functools import update_wrapper
-from typing import Any
-from typing import Callable
-from typing import Iterable
-from typing import MutableMapping
-from typing import Optional
-from typing import TypeVar
-
-from drakaina.exceptions import AuthenticationFailedError
-from drakaina.exceptions import ForbiddenError
-from drakaina.registries import RPC_REGISTRY
-from drakaina.registries import RPCRegistry
-from drakaina.types import AnyRequest
-from drakaina.types import Comparator
-from drakaina.utils import iterable_str_arg
-
-__all__ = (
-    "RPCRegistry",
-    "rpc_registry",
-    "remote_procedure",
-    "check_permissions",
-    "login_required",
-    "match_all",
-    "match_any",
-    "ENV_APP",
-    "ENV_IS_AUTHENTICATED",
-    "ENV_USER",
-    "ENV_USER_ID",
-    "ENV_AUTH_PAYLOAD",
-    "ENV_AUTH_SCOPES",
-)
-
-# General registry
-rpc_registry = RPCRegistry()
-
-# Environ (Request) context
-ENV_APP = "drakaina.app"
-ENV_IS_AUTHENTICATED = "auth.is_authenticated"
-ENV_USER = "user"
-ENV_USER_ID = "user_id"
-ENV_AUTH_PAYLOAD = "auth.payload"
-ENV_AUTH_SCOPES = "auth.scopes"
-
-T = TypeVar("T", bound=Callable)
-
-
-def remote_procedure(
-    name: Optional[str] = None,
-    registry: Optional[RPCRegistry] = None,
-    provide_request: Optional[bool] = None,
-    metadata: Optional[dict[str, Any]] = None,
-    **meta_options,
-) -> Callable:
-    """Decorator allow wrap function and define it as remote procedure.
-
-    :param name:
-        Procedure name. Default as function name.
-    :type name: str
-    :param registry:
-        Procedure registry custom object
-    :type registry: RPCRegistry
-    :param provide_request:
-        Provide a request object or context data (from the transport layer).
-        If `True`, then the request object or context can be supplied to
-        the procedure as a `request` argument.
-    :type provide_request: bool
-    :param metadata:
-        Metadata that can be processed by middleware.
-    :type metadata: dict[str, Any]
-    :param meta_options:
-        Metadata that can be processed by middleware.
-
-    """
-
-    def __decorator(
-        procedure: T,
-        _registry: RPCRegistry = None,
-        _name: str = None,
-        _provide_request: bool = None,
-        _metadata: dict | None = None,
-    ) -> T:
-        """Returns a registered procedure"""
-
-        if iscoroutinefunction(procedure):
-
-            async def wrapper(*args, **kwargs):
-                if not _provide_request:
-                    if len(args) == 0:
-                        kwargs.pop("request")
-                    else:
-                        scope, *args = args
-                return await procedure(*args, **kwargs)
-
-        else:
-
-            def wrapper(*args, **kwargs):
-                if not _provide_request:
-                    if len(args) == 0:
-                        kwargs.pop("request")
-                    else:
-                        environ, *args = args
-                return procedure(*args, **kwargs)
-
-        # Need to update the wrapper before registering in the registry
-        decorated_procedure = update_wrapper(wrapper, procedure)
-
-        if _registry is None:
-            _registry = rpc_registry
-        if _name is None:
-            _name = procedure.__name__
-        _registry.register_procedure(
-            decorated_procedure,
-            name=_name,
-            provide_request=_provide_request,
-            metadata=_metadata,
-        )
-
-        return decorated_procedure
-
-    if callable(name):
-        return __decorator(
-            procedure=name,
-            _registry=registry,
-            _name=None,
-            _provide_request=provide_request,
-            _metadata={**(metadata or {}), **meta_options},
-        )
-    elif not isinstance(name, (str, type(None))):
-        raise TypeError(
-            "Expected first argument to be an str, a callable, or None",
-        )
-
-    def decorator(procedure):
-        assert callable(procedure)
-        return __decorator(
-            procedure=procedure,
-            _registry=registry,
-            _name=name,
-            _provide_request=provide_request,
-            _metadata={**(metadata or {}), **meta_options},
-        )
-
-    return decorator
-
-
-def login_required(*_args) -> Callable:
-    """Requires login decorator.
-
-    Gives access to the procedure only to authenticated users.
-
-    """
-
-    def __decorator(procedure: T) -> T:
-        """Returns a registered procedure"""
-        registry: RPCRegistry = getattr(procedure, RPC_REGISTRY, None)
-        if registry is None:
-            raise TypeError(
-                "Incorrect usage of decorator. Please use "
-                "the `drakaina.remote_procedure` decorator first.",
-            )
-
-        if iscoroutinefunction(procedure):
-
-            async def wrapper(*args, **kwargs):
-                request = _get_request(*args, **kwargs)
-                if not _is_authenticated(request):
-                    raise ForbiddenError("Authentication required")
-
-                return await procedure(*args, **kwargs)
-
-        else:
-
-            def wrapper(*args, **kwargs):
-                request = _get_request(*args, **kwargs)
-                if not _is_authenticated(request):
-                    raise ForbiddenError("Authentication required")
-
-                return procedure(*args, **kwargs)
-
-        wrapper = update_wrapper(wrapper, procedure)
-        registry.replace(procedure, wrapper)
-        return wrapper
-
-    if len(_args) > 0:
-        if callable(_args[0]):
-            return __decorator(_args[0])
-        else:
-            raise TypeError("Expected first argument to be a callable")
-
-    def decorator(procedure):
-        assert callable(procedure)
-        return __decorator(procedure)
-
-    return decorator
-
-
-def match_any(required: Iterable[str], provided: str | Iterable[str]) -> bool:
-    return any((scope in provided for scope in required))
-
-
-def match_all(required: Iterable[str], provided: str | Iterable[str]) -> bool:
-    return set(required).issubset(set(provided))
-
-
-def check_permissions(
-    scopes: str | Iterable[str],
-    comparator: Comparator = match_all,
-) -> Callable:
-    """Permission decorator.
-
-    Gives access to the procedure only to authorized users.
-
-    """
-    if not (
-        isinstance(scopes, str)
-        or (
-            isinstance(scopes, Iterable)
-            and all((isinstance(scope, str) for scope in scopes))
-        )
-    ):
-        raise TypeError(
-            "The `scopes` argument must be a string or Iterable[string]",
-        )
-    if not callable(comparator):
-        raise TypeError(
-            "The `comparator` argument must be a function that implements "
-            "the Comparator interface",
-        )
-
-    procedure_scopes = iterable_str_arg(scopes)
-
-    def __decorator(procedure: T) -> T:
-        registry: RPCRegistry = getattr(procedure, RPC_REGISTRY, None)
-        if registry is None:
-            raise TypeError(
-                "Incorrect usage of decorator. Please use "
-                "the `drakaina.remote_procedure` decorator first.",
-            )
-
-        if iscoroutinefunction(procedure):
-
-            async def wrapper(*args, **kwargs):
-                request = _get_request(*args, **kwargs)  # noqa
-
-                if not _is_authenticated(request):
-                    raise ForbiddenError("Authentication required")
-
-                user_scopes = _get_scopes(request)
-                if not isinstance(user_scopes, Iterable):
-                    raise AuthenticationFailedError(
-                        "Invalid permissions format",
-                    )
-
-                if not comparator(procedure_scopes, user_scopes):
-                    raise ForbiddenError("Forbidden")
-
-                return await procedure(*args, **kwargs)
-
-        else:
-
-            def wrapper(*args, **kwargs):
-                request = _get_request(*args, **kwargs)  # noqa
-
-                if not _is_authenticated(request):
-                    raise ForbiddenError("Authentication required")
-
-                user_scopes = _get_scopes(request)
-                if not isinstance(user_scopes, Iterable):
-                    raise AuthenticationFailedError(
-                        "Invalid permissions format",
-                    )
-
-                if not comparator(procedure_scopes, user_scopes):
-                    raise ForbiddenError("Forbidden")
-
-                return procedure(*args, **kwargs)
-
-        wrapper = update_wrapper(wrapper, procedure)
-        registry.replace(procedure, wrapper)
-        return wrapper
-
-    return __decorator
-
-
-def _get_request(*args, **kwargs) -> Optional[AnyRequest]:
-    if len(args) == 0:
-        return kwargs.get("request")
-    else:
-        return args[0]
-
-
-def _is_authenticated(request: AnyRequest) -> bool:
-    if isinstance(request, (dict, MutableMapping)):
-        return request.get(ENV_IS_AUTHENTICATED, False)
-    else:
-        return getattr(request, ENV_IS_AUTHENTICATED, False)
-
-
-def _get_scopes(request: AnyRequest) -> Optional[Iterable[str]]:
-    if isinstance(request, (dict, MutableMapping)):
-        scopes = request.get(ENV_AUTH_SCOPES, None)
-    else:
-        scopes = getattr(request, ENV_AUTH_SCOPES, None)
-    if scopes is not None:
-        return iterable_str_arg(scopes)
+from __future__ import annotations
+
+from asyncio import iscoroutinefunction
+from functools import update_wrapper
+from typing import Any
+from typing import Callable
+from typing import Iterable
+from typing import MutableMapping
+from typing import Optional
+from typing import TypeVar
+
+from drakaina.exceptions import AuthenticationFailedError
+from drakaina.exceptions import ForbiddenError
+from drakaina.registries import RPC_REGISTRY
+from drakaina.registries import RPCRegistry
+from drakaina.types import AnyRequest
+from drakaina.types import Comparator
+from drakaina.utils import iterable_str_arg
+
+__all__ = (
+    "RPCRegistry",
+    "rpc_registry",
+    "remote_procedure",
+    "check_permissions",
+    "login_required",
+    "match_all",
+    "match_any",
+    "ENV_APP",
+    "ENV_IS_AUTHENTICATED",
+    "ENV_USER",
+    "ENV_USER_ID",
+    "ENV_AUTH_PAYLOAD",
+    "ENV_AUTH_SCOPES",
+)
+
+# General registry
+rpc_registry = RPCRegistry()
+
+# Environ (Request) context
+ENV_APP = "drakaina.app"
+ENV_IS_AUTHENTICATED = "auth.is_authenticated"
+ENV_USER = "user"
+ENV_USER_ID = "user_id"
+ENV_AUTH_PAYLOAD = "auth.payload"
+ENV_AUTH_SCOPES = "auth.scopes"
+
+T = TypeVar("T", bound=Callable)
+
+
+def remote_procedure(
+    name: Optional[str] = None,
+    registry: Optional[RPCRegistry] = None,
+    provide_request: Optional[bool] = None,
+    metadata: Optional[dict[str, Any]] = None,
+    **meta_options,
+) -> Callable:
+    """Decorator allow wrap function and define it as remote procedure.
+
+    :param name:
+        Procedure name. Default as function name.
+    :type name: str
+    :param registry:
+        Procedure registry custom object
+    :type registry: RPCRegistry
+    :param provide_request:
+        Provide a request object or context data (from the transport layer).
+        If `True`, then the request object or context can be supplied to
+        the procedure as a `request` argument.
+    :type provide_request: bool
+    :param metadata:
+        Metadata that can be processed by middleware.
+    :type metadata: dict[str, Any]
+    :param meta_options:
+        Metadata that can be processed by middleware.
+
+    """
+
+    def __decorator(
+        procedure: T,
+        _registry: RPCRegistry = None,
+        _name: str = None,
+        _provide_request: bool = None,
+        _metadata: dict | None = None,
+    ) -> T:
+        """Returns a registered procedure"""
+
+        if iscoroutinefunction(procedure):
+
+            async def wrapper(*args, **kwargs):
+                if not _provide_request:
+                    if len(args) == 0:
+                        kwargs.pop("request")
+                    else:
+                        scope, *args = args
+                return await procedure(*args, **kwargs)
+
+        else:
+
+            def wrapper(*args, **kwargs):
+                if not _provide_request:
+                    if len(args) == 0:
+                        kwargs.pop("request")
+                    else:
+                        environ, *args = args
+                return procedure(*args, **kwargs)
+
+        # Need to update the wrapper before registering in the registry
+        decorated_procedure = update_wrapper(wrapper, procedure)
+
+        if _registry is None:
+            _registry = rpc_registry
+        if _name is None:
+            _name = procedure.__name__
+        _registry.register_procedure(
+            decorated_procedure,
+            name=_name,
+            provide_request=_provide_request,
+            metadata=_metadata,
+        )
+
+        return decorated_procedure
+
+    if callable(name):
+        return __decorator(
+            procedure=name,
+            _registry=registry,
+            _name=None,
+            _provide_request=provide_request,
+            _metadata={**(metadata or {}), **meta_options},
+        )
+    elif not isinstance(name, (str, type(None))):
+        raise TypeError(
+            "Expected first argument to be an str, a callable, or None",
+        )
+
+    def decorator(procedure):
+        assert callable(procedure)
+        return __decorator(
+            procedure=procedure,
+            _registry=registry,
+            _name=name,
+            _provide_request=provide_request,
+            _metadata={**(metadata or {}), **meta_options},
+        )
+
+    return decorator
+
+
+def login_required(*_args) -> Callable:
+    """Requires login decorator.
+
+    Gives access to the procedure only to authenticated users.
+
+    """
+
+    def __decorator(procedure: T) -> T:
+        """Returns a registered procedure"""
+        registry: RPCRegistry = getattr(procedure, RPC_REGISTRY, None)
+        if registry is None:
+            raise TypeError(
+                "Incorrect usage of decorator. Please use "
+                "the `drakaina.remote_procedure` decorator first.",
+            )
+
+        if iscoroutinefunction(procedure):
+
+            async def wrapper(*args, **kwargs):
+                request = _get_request(*args, **kwargs)
+                if not _is_authenticated(request):
+                    raise ForbiddenError("Authentication required")
+
+                return await procedure(*args, **kwargs)
+
+        else:
+
+            def wrapper(*args, **kwargs):
+                request = _get_request(*args, **kwargs)
+                if not _is_authenticated(request):
+                    raise ForbiddenError("Authentication required")
+
+                return procedure(*args, **kwargs)
+
+        wrapper = update_wrapper(wrapper, procedure)
+        registry.replace(procedure, wrapper)
+        return wrapper
+
+    if len(_args) > 0:
+        if callable(_args[0]):
+            return __decorator(_args[0])
+        else:
+            raise TypeError("Expected first argument to be a callable")
+
+    def decorator(procedure):
+        assert callable(procedure)
+        return __decorator(procedure)
+
+    return decorator
+
+
+def match_any(required: Iterable[str], provided: str | Iterable[str]) -> bool:
+    return any((scope in provided for scope in required))
+
+
+def match_all(required: Iterable[str], provided: str | Iterable[str]) -> bool:
+    return set(required).issubset(set(provided))
+
+
+def check_permissions(
+    scopes: str | Iterable[str],
+    comparator: Comparator = match_all,
+) -> Callable:
+    """Permission decorator.
+
+    Gives access to the procedure only to authorized users.
+
+    """
+    if not (
+        isinstance(scopes, str)
+        or (
+            isinstance(scopes, Iterable)
+            and all((isinstance(scope, str) for scope in scopes))
+        )
+    ):
+        raise TypeError(
+            "The `scopes` argument must be a string or Iterable[string]",
+        )
+    if not callable(comparator):
+        raise TypeError(
+            "The `comparator` argument must be a function that implements "
+            "the Comparator interface",
+        )
+
+    procedure_scopes = iterable_str_arg(scopes)
+
+    def __decorator(procedure: T) -> T:
+        registry: RPCRegistry = getattr(procedure, RPC_REGISTRY, None)
+        if registry is None:
+            raise TypeError(
+                "Incorrect usage of decorator. Please use "
+                "the `drakaina.remote_procedure` decorator first.",
+            )
+
+        if iscoroutinefunction(procedure):
+
+            async def wrapper(*args, **kwargs):
+                request = _get_request(*args, **kwargs)  # noqa
+
+                if not _is_authenticated(request):
+                    raise ForbiddenError("Authentication required")
+
+                user_scopes = _get_scopes(request)
+                if not isinstance(user_scopes, Iterable):
+                    raise AuthenticationFailedError(
+                        "Invalid permissions format",
+                    )
+
+                if not comparator(procedure_scopes, user_scopes):
+                    raise ForbiddenError("Forbidden")
+
+                return await procedure(*args, **kwargs)
+
+        else:
+
+            def wrapper(*args, **kwargs):
+                request = _get_request(*args, **kwargs)  # noqa
+
+                if not _is_authenticated(request):
+                    raise ForbiddenError("Authentication required")
+
+                user_scopes = _get_scopes(request)
+                if not isinstance(user_scopes, Iterable):
+                    raise AuthenticationFailedError(
+                        "Invalid permissions format",
+                    )
+
+                if not comparator(procedure_scopes, user_scopes):
+                    raise ForbiddenError("Forbidden")
+
+                return procedure(*args, **kwargs)
+
+        wrapper = update_wrapper(wrapper, procedure)
+        registry.replace(procedure, wrapper)
+        return wrapper
+
+    return __decorator
+
+
+def _get_request(*args, **kwargs) -> Optional[AnyRequest]:
+    if len(args) == 0:
+        return kwargs.get("request")
+    else:
+        return args[0]
+
+
+def _is_authenticated(request: AnyRequest) -> bool:
+    if isinstance(request, (dict, MutableMapping)):
+        return request.get(ENV_IS_AUTHENTICATED, False)
+    else:
+        return getattr(request, ENV_IS_AUTHENTICATED, False)
+
+
+def _get_scopes(request: AnyRequest) -> Optional[Iterable[str]]:
+    if isinstance(request, (dict, MutableMapping)):
+        scopes = request.get(ENV_AUTH_SCOPES, None)
+    else:
+        scopes = getattr(request, ENV_AUTH_SCOPES, None)
+    if scopes is not None:
+        return iterable_str_arg(scopes)
```

### Comparing `drakaina-0.7.0b3/drakaina/asgi.py` & `drakaina-0.7.0b4/drakaina/asgi.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/client/__init__.py` & `drakaina-0.7.0b4/drakaina/client/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/client/base.py` & `drakaina-0.7.0b4/drakaina/client/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/client/http.py` & `drakaina-0.7.0b4/drakaina/client/http.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/client/tcp.py` & `drakaina-0.7.0b4/drakaina/client/tcp.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/client/websocket.py` & `drakaina-0.7.0b4/drakaina/client/websocket.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/contrib/django/__init__.py` & `drakaina-0.7.0b4/drakaina/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/contrib/django/middleware.py` & `drakaina-0.7.0b4/drakaina/contrib/django/middleware.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/contrib/django/views.py` & `drakaina-0.7.0b4/drakaina/contrib/django/views.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/contrib/jwt/types.py` & `drakaina-0.7.0b4/drakaina/contrib/jwt/types.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/drakaina_openapi.py` & `drakaina-0.7.0b4/drakaina/drakaina_openapi.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/exceptions.py` & `drakaina-0.7.0b4/drakaina/exceptions.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/middleware/base.py` & `drakaina-0.7.0b4/drakaina/middleware/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/middleware/cors.py` & `drakaina-0.7.0b4/drakaina/middleware/cors.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,215 +1,215 @@
-from __future__ import annotations
-
-from typing import Iterable
-from typing import Optional
-
-from drakaina.middleware.base import BaseMiddleware
-from drakaina.types import ASGIReceive
-from drakaina.types import ASGIScope
-from drakaina.types import ASGISend
-from drakaina.types import WSGIApplication
-from drakaina.types import WSGIEnvironment
-from drakaina.types import WSGIResponse
-from drakaina.types import WSGIStartResponse
-from drakaina.utils import iterable_str_arg
-
-__all__ = ("CORSMiddleware",)
-
-DEFAULT_HEADERS = (
-    "Accept, Accept-Encoding, Accept-Language, Authorization, "
-    "Content-Language, Content-Type, DNT, Origin, User-Agent, X-Requested-With"
-)
-ALL_METHODS = "DELETE, GET, HEAD, OPTIONS, PATCH, POST, PUT"
-DEFAULT_METHODS = "GET, POST, OPTIONS"
-
-
-class CORSMiddleware(BaseMiddleware):
-    """Middleware for providing CORS headers and handling preflight requests.
-
-    See: https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS
-
-    :param allow_origin:
-        The "Access-Control-Allow-Origin" header.
-    :type allow_origin: Union[str, Iterable[str]]
-    :param allow_methods:
-        The "Access-Control-Allow-Methods" header.
-        Default: "GET, POST, OPTIONS".
-    :type allow_methods: Union[str, Iterable[str]]
-    :param allow_headers:
-        The "Access-Control-Allow-Headers" header.
-        Default: "Accept, Accept-Encoding, Authorization,
-        Content-Type, DNT, Origin, User-Agent, X-Requested-With".
-    :type allow_headers: Union[str, Iterable[str]]
-    :param allow_credentials:
-        The "Access-Control-Allow-Credentials" header. Default: None.
-    :type allow_credentials: bool
-    :param expose_headers:
-        The "Access-Control-Expose-Headers" header. Default: None.
-    :type expose_headers: Union[str, Iterable[str]]
-    :param max_age:
-        The "Access-Control-Max-Age" header. Default: 3600 sec. (1 hour).
-    :type max_age: Union[int, str]
-
-    """
-
-    __slots__ = (
-        "_cors_headers",
-        "_preflight_cors_headers",
-        "_allow_origin",
-        "_allow_credentials",
-        "_allow_headers",
-    )
-
-    def __init__(
-        self,
-        app: WSGIApplication,
-        allow_origin: str | Iterable[str],
-        allow_methods: Optional[str | Iterable[str]] = None,
-        allow_headers: Optional[str | Iterable[str]] = None,
-        allow_credentials: Optional[bool] = None,
-        expose_headers: Optional[str | Iterable[str]] = None,
-        max_age: int = 3600,
-        **kwargs,
-    ):
-        super().__init__(app, **kwargs)
-
-        self._allow_origin = ", ".join(iterable_str_arg(allow_origin))
-
-        if allow_methods:
-            if "*" in allow_methods:
-                _allow_methods = ALL_METHODS
-            else:
-                _allow_methods = ", ".join(iterable_str_arg(allow_methods))
-        else:
-            _allow_methods = DEFAULT_METHODS
-
-        if allow_headers:
-            self._allow_headers = ", ".join(
-                sorted(
-                    set(iterable_str_arg(DEFAULT_HEADERS))
-                    | set(iterable_str_arg(allow_headers)),
-                ),
-            )
-        else:
-            self._allow_headers = DEFAULT_HEADERS
-
-        if expose_headers:
-            _expose_headers = ", ".join(iterable_str_arg(expose_headers))
-        else:
-            _expose_headers = None
-
-        self._allow_credentials = allow_credentials
-
-        # Prepare CORS response headers
-        self._cors_headers = []
-        if self._allow_credentials:
-            self._cors_headers.append(
-                ("Access-Control-Allow-Credentials", "true"),
-            )
-        if _expose_headers:
-            self._cors_headers.append(
-                ("Access-Control-Expose-Headers", _expose_headers),
-            )
-
-        # Prepare pre-flight CORS response headers
-        self._preflight_cors_headers = [
-            ("Access-Control-Allow-Methods", _allow_methods),
-            ("Access-Control-Max-Age", str(max_age)),
-            ("Content-Length", "0"),
-        ]
-        if "*" not in self._allow_origin or self._allow_credentials:
-            self._preflight_cors_headers.append(("Vary", "Origin"))
-
-        if self._allow_credentials:
-            self._preflight_cors_headers.append(
-                ("Access-Control-Allow-Credentials", "true"),
-            )
-
-    def __wsgi_call__(
-        self,
-        environ: WSGIEnvironment,
-        start_response: WSGIStartResponse,
-    ) -> WSGIResponse:
-        if environ.get("HTTP_ORIGIN"):
-            if environ.get("REQUEST_METHOD") == "OPTIONS":
-                return self.options(environ, start_response)
-            return self.app(
-                environ,
-                self._start_response_with_cors(environ, start_response),
-            )
-        else:
-            return self.app(environ, start_response)
-
-    async def __asgi_call__(
-        self,
-        scope: ASGIScope,
-        receive: ASGIReceive,
-        send: ASGISend,
-    ):
-        if scope["type"] != "http":
-            await self.app(scope, receive, send)
-        ...
-
-    def options(
-        self,
-        environ: WSGIEnvironment,
-        start_response: WSGIStartResponse,
-    ) -> WSGIResponse:
-        """Response for OPTIONS request"""
-        request_origin = environ["HTTP_ORIGIN"]
-        request_headers = environ.get("HTTP_ACCESS_CONTROL_REQUEST_HEADERS")
-
-        response_headers = self._preflight_cors_headers[:]
-
-        if "*" in self._allow_origin or request_origin in self._allow_origin:
-            if "*" not in self._allow_origin or self._allow_credentials:
-                response_headers.append(
-                    ("Access-Control-Allow-Origin", request_origin),
-                )
-            else:
-                response_headers.append(("Access-Control-Allow-Origin", "*"))
-
-        if "*" in self._allow_headers and request_headers is not None:
-            response_headers.append(
-                ("Access-Control-Allow-Headers", request_headers),
-            )
-        if "*" not in self._allow_headers:
-            response_headers.append(
-                ("Access-Control-Allow-Headers", self._allow_headers),
-            )
-
-        start_response("200 OK", response_headers)
-        yield b""
-
-    def _start_response_with_cors(
-        self,
-        environ: WSGIEnvironment,
-        start_response: WSGIStartResponse,
-    ) -> WSGIStartResponse:
-        """Wraps the start_response method, and includes the CORS header
-        for the specified origin.
-        """
-        request_origin = environ["HTTP_ORIGIN"]
-
-        cors_headers = self._cors_headers[:]
-
-        if "*" in self._allow_origin:
-            if "HTTP_COOKIE" in environ:
-                cors_headers.append(
-                    ("Access-Control-Allow-Origin", request_origin),
-                )
-                cors_headers.append(("Vary", "Origin"))
-            else:
-                cors_headers.append(("Access-Control-Allow-Origin", "*"))
-        elif (
-            "*" not in self._allow_origin
-            and request_origin in self._allow_origin
-        ):
-            cors_headers.append(("Access-Control-Allow-Origin", request_origin))
-            cors_headers.append(("Vary", "Origin"))
-
-        def response_with_cors(status, headers, exc_info=None):
-            headers.extend(cors_headers)
-            return start_response(status, headers, exc_info)
-
-        return response_with_cors
+from __future__ import annotations
+
+from typing import Iterable
+from typing import Optional
+
+from drakaina.middleware.base import BaseMiddleware
+from drakaina.types import ASGIReceive
+from drakaina.types import ASGIScope
+from drakaina.types import ASGISend
+from drakaina.types import WSGIApplication
+from drakaina.types import WSGIEnvironment
+from drakaina.types import WSGIResponse
+from drakaina.types import WSGIStartResponse
+from drakaina.utils import iterable_str_arg
+
+__all__ = ("CORSMiddleware",)
+
+DEFAULT_HEADERS = (
+    "Accept, Accept-Encoding, Accept-Language, Authorization, "
+    "Content-Language, Content-Type, DNT, Origin, User-Agent, X-Requested-With"
+)
+ALL_METHODS = "DELETE, GET, HEAD, OPTIONS, PATCH, POST, PUT"
+DEFAULT_METHODS = "GET, POST, OPTIONS"
+
+
+class CORSMiddleware(BaseMiddleware):
+    """Middleware for providing CORS headers and handling preflight requests.
+
+    See: https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS
+
+    :param allow_origin:
+        The "Access-Control-Allow-Origin" header.
+    :type allow_origin: Union[str, Iterable[str]]
+    :param allow_methods:
+        The "Access-Control-Allow-Methods" header.
+        Default: "GET, POST, OPTIONS".
+    :type allow_methods: Union[str, Iterable[str]]
+    :param allow_headers:
+        The "Access-Control-Allow-Headers" header.
+        Default: "Accept, Accept-Encoding, Authorization,
+        Content-Type, DNT, Origin, User-Agent, X-Requested-With".
+    :type allow_headers: Union[str, Iterable[str]]
+    :param allow_credentials:
+        The "Access-Control-Allow-Credentials" header. Default: None.
+    :type allow_credentials: bool
+    :param expose_headers:
+        The "Access-Control-Expose-Headers" header. Default: None.
+    :type expose_headers: Union[str, Iterable[str]]
+    :param max_age:
+        The "Access-Control-Max-Age" header. Default: 3600 sec. (1 hour).
+    :type max_age: Union[int, str]
+
+    """
+
+    __slots__ = (
+        "_cors_headers",
+        "_preflight_cors_headers",
+        "_allow_origin",
+        "_allow_credentials",
+        "_allow_headers",
+    )
+
+    def __init__(
+        self,
+        app: WSGIApplication,
+        allow_origin: str | Iterable[str],
+        allow_methods: Optional[str | Iterable[str]] = None,
+        allow_headers: Optional[str | Iterable[str]] = None,
+        allow_credentials: Optional[bool] = None,
+        expose_headers: Optional[str | Iterable[str]] = None,
+        max_age: int = 3600,
+        **kwargs,
+    ):
+        super().__init__(app, **kwargs)
+
+        self._allow_origin = ", ".join(iterable_str_arg(allow_origin))
+
+        if allow_methods:
+            if "*" in allow_methods:
+                _allow_methods = ALL_METHODS
+            else:
+                _allow_methods = ", ".join(iterable_str_arg(allow_methods))
+        else:
+            _allow_methods = DEFAULT_METHODS
+
+        if allow_headers:
+            self._allow_headers = ", ".join(
+                sorted(
+                    set(iterable_str_arg(DEFAULT_HEADERS))
+                    | set(iterable_str_arg(allow_headers)),
+                ),
+            )
+        else:
+            self._allow_headers = DEFAULT_HEADERS
+
+        if expose_headers:
+            _expose_headers = ", ".join(iterable_str_arg(expose_headers))
+        else:
+            _expose_headers = None
+
+        self._allow_credentials = allow_credentials
+
+        # Prepare CORS response headers
+        self._cors_headers = []
+        if self._allow_credentials:
+            self._cors_headers.append(
+                ("Access-Control-Allow-Credentials", "true"),
+            )
+        if _expose_headers:
+            self._cors_headers.append(
+                ("Access-Control-Expose-Headers", _expose_headers),
+            )
+
+        # Prepare pre-flight CORS response headers
+        self._preflight_cors_headers = [
+            ("Access-Control-Allow-Methods", _allow_methods),
+            ("Access-Control-Max-Age", str(max_age)),
+            ("Content-Length", "0"),
+        ]
+        if "*" not in self._allow_origin or self._allow_credentials:
+            self._preflight_cors_headers.append(("Vary", "Origin"))
+
+        if self._allow_credentials:
+            self._preflight_cors_headers.append(
+                ("Access-Control-Allow-Credentials", "true"),
+            )
+
+    def __wsgi_call__(
+        self,
+        environ: WSGIEnvironment,
+        start_response: WSGIStartResponse,
+    ) -> WSGIResponse:
+        if environ.get("HTTP_ORIGIN"):
+            if environ.get("REQUEST_METHOD") == "OPTIONS":
+                return self.options(environ, start_response)
+            return self.app(
+                environ,
+                self._start_response_with_cors(environ, start_response),
+            )
+        else:
+            return self.app(environ, start_response)
+
+    async def __asgi_call__(
+        self,
+        scope: ASGIScope,
+        receive: ASGIReceive,
+        send: ASGISend,
+    ):
+        if scope["type"] != "http":
+            await self.app(scope, receive, send)
+        ...
+
+    def options(
+        self,
+        environ: WSGIEnvironment,
+        start_response: WSGIStartResponse,
+    ) -> WSGIResponse:
+        """Response for OPTIONS request"""
+        request_origin = environ["HTTP_ORIGIN"]
+        request_headers = environ.get("HTTP_ACCESS_CONTROL_REQUEST_HEADERS")
+
+        response_headers = self._preflight_cors_headers[:]
+
+        if "*" in self._allow_origin or request_origin in self._allow_origin:
+            if "*" not in self._allow_origin or self._allow_credentials:
+                response_headers.append(
+                    ("Access-Control-Allow-Origin", request_origin),
+                )
+            else:
+                response_headers.append(("Access-Control-Allow-Origin", "*"))
+
+        if "*" in self._allow_headers and request_headers is not None:
+            response_headers.append(
+                ("Access-Control-Allow-Headers", request_headers),
+            )
+        if "*" not in self._allow_headers:
+            response_headers.append(
+                ("Access-Control-Allow-Headers", self._allow_headers),
+            )
+
+        start_response("200 OK", response_headers)
+        yield b""
+
+    def _start_response_with_cors(
+        self,
+        environ: WSGIEnvironment,
+        start_response: WSGIStartResponse,
+    ) -> WSGIStartResponse:
+        """Wraps the start_response method, and includes the CORS header
+        for the specified origin.
+        """
+        request_origin = environ["HTTP_ORIGIN"]
+
+        cors_headers = self._cors_headers[:]
+
+        if "*" in self._allow_origin:
+            if "HTTP_COOKIE" in environ:
+                cors_headers.append(
+                    ("Access-Control-Allow-Origin", request_origin),
+                )
+                cors_headers.append(("Vary", "Origin"))
+            else:
+                cors_headers.append(("Access-Control-Allow-Origin", "*"))
+        elif (
+            "*" not in self._allow_origin
+            and request_origin in self._allow_origin
+        ):
+            cors_headers.append(("Access-Control-Allow-Origin", request_origin))
+            cors_headers.append(("Vary", "Origin"))
+
+        def response_with_cors(status, headers, exc_info=None):
+            headers.extend(cors_headers)
+            return start_response(status, headers, exc_info)
+
+        return response_with_cors
```

### Comparing `drakaina-0.7.0b3/drakaina/middleware/logging.py` & `drakaina-0.7.0b4/drakaina/middleware/logging.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/middleware/request_wrapper.py` & `drakaina-0.7.0b4/drakaina/middleware/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/rpc_protocols/jsonrpc20.py` & `drakaina-0.7.0b4/drakaina/rpc_protocols/jsonrpc20.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,612 +1,612 @@
-from __future__ import annotations
-
-from copy import deepcopy
-from typing import Any
-from typing import ClassVar
-
-from drakaina.exceptions import AuthenticationFailedError
-from drakaina.exceptions import BadRequestError
-from drakaina.exceptions import DeserializationError
-from drakaina.exceptions import ForbiddenError
-from drakaina.exceptions import InternalServerError
-from drakaina.exceptions import InvalidParametersError
-from drakaina.exceptions import InvalidPermissionsError
-from drakaina.exceptions import InvalidTokenError
-from drakaina.exceptions import NotFoundError
-from drakaina.exceptions import RPCError
-from drakaina.exceptions import SerializationError
-from drakaina.registries import RPC_SCHEMA
-from drakaina.registries import RPCRegistry
-from drakaina.rpc_protocols.base import BaseRPCProtocol
-from drakaina.serializers import BaseSerializer
-from drakaina.serializers import JsonSerializer
-from drakaina.types import JSONRPCRequest
-from drakaina.types import JSONRPCRequestObject
-from drakaina.types import JSONRPCResponse
-from drakaina.types import JSONRPCResponseObject
-from drakaina.types import MethodSchema
-from drakaina.types import OAPI
-from drakaina.types import ORPC
-from drakaina.utils import unwrap_func
-
-__all__ = ("JsonRPCv2",)
-
-DEFAULT_OPENRPC_SCHEMA = ORPC.OpenRPC(
-    openrpc=ORPC.SUPPORTED_VERSION,
-    info=ORPC.Info(version="1.0.0", title="JSON-RPC 2.0 service"),
-    servers=[ORPC.Server(name="main", url="/")],
-    methods=[],
-)
-"""This is the default OpenRPC schema.
-
-Specify an explicit schema template
-'openrpc_schema_template' to control it.
-"""
-
-DEFAULT_OPENAPI_SCHEMA = OAPI.OpenAPI(
-    openapi=OAPI.SUPPORTED_VERSION,
-    info=OAPI.Info(version="1.0.0", title="JSON-RPC 2.0 service"),
-    servers=[OAPI.Server(url="/")],
-    paths=OAPI.Paths(),
-)
-"""This is the default OpenAPI schema.
-
-Specify an explicit schema template
-'openapi_schema_template' to control it.
-"""
-
-
-# JSON-RPC Error classes
-
-
-class JsonRPCError(RPCError):
-    """JSON-RPC Common error
-
-    Reserved for implementation-defined server-errors.
-    Codes -32000 to -32099.
-
-    """
-
-    code: int = -32000
-    default_message: str = "Server error"
-    id: int | str = None
-    data: Any = None
-
-    def __init__(
-        self,
-        *args,
-        message: str = None,
-        id: int | str = None,
-        data: Any | None = None,
-    ):
-        super().__init__(*args)
-
-        self.id = id
-        if message:
-            self.message = message
-
-        if self.message and data:
-            self.data = {"text": self.message.strip(), "details": data}
-        elif self.message:
-            self.data = self.message.strip()
-        elif data:
-            self.data = data
-
-    def __str__(self) -> str:
-        return f"{self.__class__.__name__} ({self.code} {self.default_message})"
-
-    def __repr__(self) -> str:
-        return (
-            f"<{self.__class__.__name__} ({self.code} {self.default_message})>"
-        )
-
-    def as_dict(self) -> JSONRPCResponseObject:
-        error = dict(
-            jsonrpc="2.0",
-            error={"code": self.code, "message": self.default_message},
-            id=self.id,
-        )
-
-        if self.data:
-            error["error"]["data"] = self.data
-
-        return error
-
-
-class InvalidRequestError(JsonRPCError):
-    """Invalid Request
-
-    The JSON sent is not a valid Request object.
-
-    """
-
-    code = -32600
-    default_message = "Invalid Request"
-
-
-class MethodNotFoundError(JsonRPCError):
-    """Method not found
-
-    The method does not exist / is not available.
-
-    """
-
-    code = -32601
-    default_message = "Method not found"
-
-
-class InvalidParamsError(JsonRPCError):
-    """Invalid params
-
-    Invalid method parameter(s).
-
-    """
-
-    code = -32602
-    default_message = "Invalid params"
-
-
-class InternalError(JsonRPCError):
-    """Internal error
-
-    Internal JSON-RPC error.
-
-    """
-
-    code = -32603
-    default_message = "Internal error"
-
-
-class ParseError(JsonRPCError):
-    """Parse error
-
-    Invalid JSON was received by the server.
-    An error occurred on the server while parsing the JSON text.
-
-    """
-
-    code = -32700
-    default_message = "Parse error"
-
-
-# Implementation of Drakaina errors
-
-
-class AuthenticationFailedJRPCError(JsonRPCError):
-    """Authentication failed"""
-
-    code = -32010
-    default_message = "Authentication failed"
-
-
-class InvalidTokenJRPCError(AuthenticationFailedJRPCError):
-    """Invalid token error"""
-
-    code = -32011
-    default_message = "Invalid token"
-
-
-class ForbiddenJRPCError(AuthenticationFailedJRPCError):
-    """Forbidden error"""
-
-    code = -32012
-    default_message = "Forbidden"
-
-
-class InvalidPermissionsJRPCError(ForbiddenJRPCError):
-    """Invalid permissions error"""
-
-    code = -32013
-    default_message = "Invalid permissions"
-
-
-# JSON-RPC v2.0 implementation
-
-
-class JsonRPCv2(BaseRPCProtocol):
-    """JSON-RPC 2.0 implementation.
-
-    :param registry:
-        Registry of remote procedures.
-        Default: `drakaina.registries.rpc_registry` (generic module instance)
-    :param serializer:
-        Serializer object. Default: `JsonSerializer` (stdlib.json)
-    :param schema_serializer:
-        The serializer object to serialize the schema.
-        Default: `JsonSerializer` (stdlib.json)
-    :param openrpc:
-        An object (TypedDict) of OpenRPC containing general information,
-        information about the server(s). It must not contain a method schema.
-    :param openapi:
-        An object (TypedDict) of OpenAPI containing general information,
-        information about the server(s). It must not contain a paths schema.
-
-    """
-
-    __slots__ = (
-        "allow_service_discovery",
-        "schema_url",
-        "openrpc_schema_template",
-        "openapi_schema_template",
-        "__openrpc_schema",
-        "__openapi_schema",
-    )
-
-    base_error_class: ClassVar = JsonRPCError
-    """Base class for JSON-RPC 2.0 protocol implementation."""
-
-    default_error_class: ClassVar = InternalError
-    """Default JSON-RPC 2.0 error class to represent internal exceptions."""
-
-    _errors_map: ClassVar = {
-        Exception: JsonRPCError,
-        RPCError: JsonRPCError,
-        BadRequestError: InvalidRequestError,
-        NotFoundError: MethodNotFoundError,
-        InvalidParametersError: InvalidParamsError,
-        InternalServerError: InternalError,
-        SerializationError: InternalError,
-        DeserializationError: ParseError,
-        AuthenticationFailedError: AuthenticationFailedJRPCError,
-        InvalidTokenError: InvalidTokenJRPCError,
-        ForbiddenError: ForbiddenJRPCError,
-        InvalidPermissionsError: InvalidPermissionsJRPCError,
-    }
-
-    def __init__(
-        self,
-        registry: RPCRegistry | None = None,
-        serializer: BaseSerializer | None = None,
-        schema_serializer: BaseSerializer | None = None,
-        openrpc: ORPC.OpenRPC | None = None,
-        openapi: OAPI.OpenAPI | None = None,
-        allow_service_discovery: bool | None = None,
-        schema_url: str | None = None,
-    ):
-        if serializer is None:
-            serializer = JsonSerializer()
-
-        super().__init__(
-            registry=registry,
-            serializer=serializer,
-            schema_serializer=schema_serializer,
-        )
-        self.allow_service_discovery = allow_service_discovery
-        self.schema_url = schema_url
-
-        # Schemas
-        self.openrpc_schema_template = (
-            openrpc if openrpc is not None else DEFAULT_OPENRPC_SCHEMA
-        )
-        self.__openrpc_schema = None
-        self.openapi_schema_template = (
-            openapi if openapi is not None else DEFAULT_OPENAPI_SCHEMA
-        )
-        self.__openapi_schema = None
-
-        if allow_service_discovery:
-            self.registry.register_rpc_extension(
-                extension_procedure=self.rpc_discover,
-                extension_name="rpc.discover",
-            )
-
-    def handle(
-        self,
-        rpc_request: JSONRPCRequest,
-        request: Any | None = None,
-    ) -> JSONRPCResponse | None:
-        """Handles a procedure call or batch of procedure call
-
-        :param rpc_request:
-            RPC request in protocol format.
-        :type rpc_request: JSONRPCRequest
-        :param request:
-            Optional parameter that can be passed as an
-            argument to the procedure.
-        :type request: Any
-        :return:
-            Returns the result in protocol format.
-        :rtype: JSONRPCResponse
-
-        """
-        # Check bad request
-        if not (isinstance(rpc_request, (dict, list)) and len(rpc_request) > 0):
-            return InvalidRequestError().as_dict()
-
-        # Handle batch request
-        if isinstance(rpc_request, list):
-            batch_result = []
-            for request_object in rpc_request:
-                result = self.execute(request_object, request=request)
-                if result is not None:
-                    batch_result.append(result)
-            if len(batch_result) == 0:
-                return None
-            return batch_result
-
-        # Handle single request
-        return self.execute(rpc_request, request=request)
-
-    def execute(
-        self,
-        procedure_call: JSONRPCRequestObject,
-        request: Any | None = None,
-    ) -> JSONRPCResponseObject | None:
-        """Execute a remote procedure call.
-
-        :param procedure_call:
-            RPC request object in protocol format.
-        :type procedure_call: JSONRPCRequestObject
-        :param request:
-            Optional parameter that can be passed as an
-            argument to the procedure. By default, None will be passed.
-        :type request: Any
-        :return:
-            Returns a result object in protocol format.
-        :rtype: JSONRPCResponseObject
-
-        """
-        if not isinstance(procedure_call, dict):
-            return InvalidRequestError().as_dict()
-        method: str = procedure_call.get("method")
-        params: list | dict | None = procedure_call.get("params")
-        request_id: int | str | None = procedure_call.get("id")
-
-        # Validate protocol
-        if (
-            procedure_call.get("jsonrpc") != "2.0"
-            or not isinstance(method, str)
-            or not (params is None or isinstance(params, (list, dict)))
-            or not (request_id is None or isinstance(request_id, (int, str)))
-        ):
-            return InvalidRequestError(id=request_id).as_dict()
-
-        # Getting procedure
-        procedure = self.registry[method]
-        if procedure is None:
-            if request_id is None:
-                return None
-            return MethodNotFoundError(id=request_id).as_dict()
-
-        # Prepare parameters
-        args, kwargs = (), {}
-        if params is not None:
-            if isinstance(params, list):
-                args = (request, *params)
-            elif isinstance(params, dict):
-                kwargs = dict(request=request, **params)
-        else:
-            kwargs = dict(request=request)
-
-        # Execute RPC method
-        try:
-            result = procedure(*args, **kwargs)
-        except RPCError as err:
-            error = self.handle_error(err)
-            error.id = request_id
-            return error.as_dict()
-        except Exception as err:
-            return InternalError(message=str(err), id=request_id).as_dict()
-
-        if request_id is None:
-            return None
-
-        return dict(jsonrpc="2.0", result=result, id=request_id)
-
-    def rpc_discover(self) -> dict[str, Any]:
-        """Returns an OpenRPC schema as a description of this service.
-
-        :return:
-
-        """
-        if self.schema_url is not None:
-            self._validate_rpc_url()
-            schema = {"$ref": self.schema_url}
-        else:
-            schema = self.openrpc_schema()
-
-        return {"name": "OpenRPC Schema", "schema": schema}
-
-    def openrpc_schema(self) -> ORPC.OpenRPC:
-        """Implementation of OpenRPC specification.
-
-        https://spec.open-rpc.org/
-
-        """
-        if not self.__openrpc_schema:
-            openrpc: ORPC.OpenRPC = deepcopy(self.openrpc_schema_template)
-
-            for method_name, procedure_ in self.registry.items():
-                procedure = unwrap_func(procedure_)
-                try:
-                    method_schema: MethodSchema = getattr(procedure, RPC_SCHEMA)
-                except AttributeError:
-                    break
-
-                method = ORPC.Method(
-                    name=method_name,
-                    params=[],
-                    result={},
-                    deprecated=method_schema.get("deprecated", False),
-                )
-                if "short_description" in method_schema:
-                    method["summary"] = method_schema["short_description"]
-                if "description" in method_schema:
-                    method["description"] = method_schema["description"]
-
-                # Fill parameters schema
-                parameters = method_schema.get("parameters", {})
-                for param_name, parameter in parameters.items():
-                    cd_param = ORPC.ContentDescriptor(
-                        name=parameter.get("name", param_name),
-                        schema=ORPC.Schema(),
-                        required=parameter.get("required", False),
-                        deprecated=parameter.get("deprecated", False),
-                    )
-                    if "type" in parameter:
-                        cd_param["schema"]["type"] = ORPC.type_mapping(
-                            parameter["type"],
-                        )
-                    if "default" in parameter:
-                        cd_param["schema"]["default"] = parameter["default"]
-                    if "description" in parameter:
-                        cd_param["summary"] = parameter["description"]
-                        cd_param["description"] = parameter["description"]
-
-                    method["params"].append(cd_param)
-
-                # Fill result schema
-                if "result" in method_schema:
-                    result_schema = method_schema["result"]
-                    cd_result = ORPC.ContentDescriptor(
-                        name=result_schema.get("name", "result"),
-                        schema=ORPC.Schema(),
-                    )
-                    if "type" in result_schema:
-                        cd_result["schema"]["type"] = ORPC.type_mapping(
-                            result_schema.get("type"),
-                        )
-                    if "description" in result_schema:
-                        cd_result["summary"] = result_schema["description"]
-                        cd_result["description"] = result_schema["description"]
-
-                    method["result"] = cd_result
-
-                openrpc["methods"].append(method)
-
-            self.__openrpc_schema = openrpc
-        return self.__openrpc_schema
-
-    def openapi_schema(self) -> dict:
-        """Implementation of OpenAPI specification.
-
-        https://spec.openapis.org/oas/latest.html
-
-        """
-        if not self.__openapi_schema:
-            openapi: OAPI.OpenAPI = deepcopy(self.openapi_schema_template)
-
-            for method_name, procedure_ in self.registry.items():
-                procedure = unwrap_func(procedure_)
-                try:
-                    method_schema: MethodSchema = getattr(procedure, RPC_SCHEMA)
-                except AttributeError:
-                    break
-
-                path_name = self.schema_url + "#" + method_name
-                operation = OAPI.Operation(
-                    operationId=method_name,
-                    parameters=[],
-                    deprecated=method_schema.get("deprecated", False),
-                )
-                if "short_description" in method_schema:
-                    operation["summary"] = method_schema["short_description"]
-                if "description" in method_schema:
-                    operation["description"] = method_schema["description"]
-
-                # Fill request body
-                parameters = method_schema.get("parameters", {}).items()
-                media = OAPI.MediaType(
-                    schema=OAPI.Schema(
-                        type="object",
-                        properties={
-                            "jsonrpc": {
-                                "type": "string",
-                                "description": "Protocol version",
-                            },
-                            "method": {
-                                "type": "string",
-                                "description": "Procedure (method) name",
-                            },
-                            "params": {
-                                "type": "object",
-                                "properties": {
-                                    param_name: {
-                                        "default": parameter.get("default", ""),
-                                        "description": parameter.get(
-                                            "description",
-                                            "",
-                                        ),
-                                        "deprecated": parameter.get(
-                                            "deprecated",
-                                            False,
-                                        ),
-                                    }
-                                    for param_name, parameter in parameters
-                                },
-                            },
-                            "id": {
-                                "type": "string",
-                            },
-                        },
-                        required=["jsonrpc", "method"],
-                    ),
-                )
-                if "example" in method_schema:
-                    media["example"] = method_schema["example"]
-                if "examples" in method_schema:
-                    media["examples"] = method_schema["examples"]
-                operation["requestBody"] = OAPI.RequestBody(
-                    content={"application/json": media},
-                    description="JSON-RPC 2.0 Request Object",
-                    required=True,
-                )
-
-                # Fill result schema
-                if "result" in method_schema:
-                    result_schema = method_schema["result"]
-
-                    media = OAPI.MediaType(
-                        schema=OAPI.Schema(
-                            type="object",
-                            properties=dict(
-                                jsonrpc=dict(type="string", default="2.0"),
-                                result=dict(),
-                                id=dict(type="string"),
-                            ),
-                        ),
-                    )
-                    if "type" in result_schema:
-                        media["schema"]["type"] = OAPI.type_mapping(
-                            result_schema.get("type"),
-                        )
-                    if "description" in result_schema:
-                        media["schema"]["description"] = result_schema[
-                            "description"
-                        ]
-                    if "example" in result_schema:
-                        media["example"] = result_schema["example"]
-                    if "examples" in result_schema:
-                        media["examples"] = result_schema["examples"]
-                else:
-                    # If returns type is NoneType
-                    media = OAPI.MediaType(
-                        schema=OAPI.Schema(
-                            type="object",
-                            properties=dict(
-                                jsonrpc=dict(type="string", default="2.0"),
-                                result=dict(type="null"),
-                                id=dict(type="string"),
-                            ),
-                        ),
-                    )
-                operation["responses"] = OAPI.Responses(
-                    **{
-                        "200": OAPI.Response(
-                            description="JSON-RPC 2.0 Response Object",
-                            content={"application/json": media},
-                        ),
-                    },
-                )
-
-                openapi["paths"][path_name] = OAPI.PathItem(post=operation)
-
-            self.__openapi_schema = openapi
-        return self.__openapi_schema
-
-    def _validate_rpc_url(self):
-        assert bool(self.schema_url), (
-            "To use service description schemes, "
-            "you must specify the URL responsible for processing "
-            "RPC requests."
-        )
+from __future__ import annotations
+
+from copy import deepcopy
+from typing import Any
+from typing import ClassVar
+
+from drakaina.exceptions import AuthenticationFailedError
+from drakaina.exceptions import BadRequestError
+from drakaina.exceptions import DeserializationError
+from drakaina.exceptions import ForbiddenError
+from drakaina.exceptions import InternalServerError
+from drakaina.exceptions import InvalidParametersError
+from drakaina.exceptions import InvalidPermissionsError
+from drakaina.exceptions import InvalidTokenError
+from drakaina.exceptions import NotFoundError
+from drakaina.exceptions import RPCError
+from drakaina.exceptions import SerializationError
+from drakaina.registries import RPC_SCHEMA
+from drakaina.registries import RPCRegistry
+from drakaina.rpc_protocols.base import BaseRPCProtocol
+from drakaina.serializers import BaseSerializer
+from drakaina.serializers import JsonSerializer
+from drakaina.types import JSONRPCRequest
+from drakaina.types import JSONRPCRequestObject
+from drakaina.types import JSONRPCResponse
+from drakaina.types import JSONRPCResponseObject
+from drakaina.types import MethodSchema
+from drakaina.types import OAPI
+from drakaina.types import ORPC
+from drakaina.utils import unwrap_func
+
+__all__ = ("JsonRPCv2",)
+
+DEFAULT_OPENRPC_SCHEMA = ORPC.OpenRPC(
+    openrpc=ORPC.SUPPORTED_VERSION,
+    info=ORPC.Info(version="1.0.0", title="JSON-RPC 2.0 service"),
+    servers=[ORPC.Server(name="main", url="/")],
+    methods=[],
+)
+"""This is the default OpenRPC schema.
+
+Specify an explicit schema template
+'openrpc_schema_template' to control it.
+"""
+
+DEFAULT_OPENAPI_SCHEMA = OAPI.OpenAPI(
+    openapi=OAPI.SUPPORTED_VERSION,
+    info=OAPI.Info(version="1.0.0", title="JSON-RPC 2.0 service"),
+    servers=[OAPI.Server(url="/")],
+    paths=OAPI.Paths(),
+)
+"""This is the default OpenAPI schema.
+
+Specify an explicit schema template
+'openapi_schema_template' to control it.
+"""
+
+
+# JSON-RPC Error classes
+
+
+class JsonRPCError(RPCError):
+    """JSON-RPC Common error
+
+    Reserved for implementation-defined server-errors.
+    Codes -32000 to -32099.
+
+    """
+
+    code: int = -32000
+    default_message: str = "Server error"
+    id: int | str = None
+    data: Any = None
+
+    def __init__(
+        self,
+        *args,
+        message: str = None,
+        id: int | str = None,
+        data: Any | None = None,
+    ):
+        super().__init__(*args)
+
+        self.id = id
+        if message:
+            self.message = message
+
+        if self.message and data:
+            self.data = {"text": self.message.strip(), "details": data}
+        elif self.message:
+            self.data = self.message.strip()
+        elif data:
+            self.data = data
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__} ({self.code} {self.default_message})"
+
+    def __repr__(self) -> str:
+        return (
+            f"<{self.__class__.__name__} ({self.code} {self.default_message})>"
+        )
+
+    def as_dict(self) -> JSONRPCResponseObject:
+        error = dict(
+            jsonrpc="2.0",
+            error={"code": self.code, "message": self.default_message},
+            id=self.id,
+        )
+
+        if self.data:
+            error["error"]["data"] = self.data
+
+        return error
+
+
+class InvalidRequestError(JsonRPCError):
+    """Invalid Request
+
+    The JSON sent is not a valid Request object.
+
+    """
+
+    code = -32600
+    default_message = "Invalid Request"
+
+
+class MethodNotFoundError(JsonRPCError):
+    """Method not found
+
+    The method does not exist / is not available.
+
+    """
+
+    code = -32601
+    default_message = "Method not found"
+
+
+class InvalidParamsError(JsonRPCError):
+    """Invalid params
+
+    Invalid method parameter(s).
+
+    """
+
+    code = -32602
+    default_message = "Invalid params"
+
+
+class InternalError(JsonRPCError):
+    """Internal error
+
+    Internal JSON-RPC error.
+
+    """
+
+    code = -32603
+    default_message = "Internal error"
+
+
+class ParseError(JsonRPCError):
+    """Parse error
+
+    Invalid JSON was received by the server.
+    An error occurred on the server while parsing the JSON text.
+
+    """
+
+    code = -32700
+    default_message = "Parse error"
+
+
+# Implementation of Drakaina errors
+
+
+class AuthenticationFailedJRPCError(JsonRPCError):
+    """Authentication failed"""
+
+    code = -32010
+    default_message = "Authentication failed"
+
+
+class InvalidTokenJRPCError(AuthenticationFailedJRPCError):
+    """Invalid token error"""
+
+    code = -32011
+    default_message = "Invalid token"
+
+
+class ForbiddenJRPCError(AuthenticationFailedJRPCError):
+    """Forbidden error"""
+
+    code = -32012
+    default_message = "Forbidden"
+
+
+class InvalidPermissionsJRPCError(ForbiddenJRPCError):
+    """Invalid permissions error"""
+
+    code = -32013
+    default_message = "Invalid permissions"
+
+
+# JSON-RPC v2.0 implementation
+
+
+class JsonRPCv2(BaseRPCProtocol):
+    """JSON-RPC 2.0 implementation.
+
+    :param registry:
+        Registry of remote procedures.
+        Default: `drakaina.registries.rpc_registry` (generic module instance)
+    :param serializer:
+        Serializer object. Default: `JsonSerializer` (stdlib.json)
+    :param schema_serializer:
+        The serializer object to serialize the schema.
+        Default: `JsonSerializer` (stdlib.json)
+    :param openrpc:
+        An object (TypedDict) of OpenRPC containing general information,
+        information about the server(s). It must not contain a method schema.
+    :param openapi:
+        An object (TypedDict) of OpenAPI containing general information,
+        information about the server(s). It must not contain a paths schema.
+
+    """
+
+    __slots__ = (
+        "allow_service_discovery",
+        "schema_url",
+        "openrpc_schema_template",
+        "openapi_schema_template",
+        "__openrpc_schema",
+        "__openapi_schema",
+    )
+
+    base_error_class: ClassVar = JsonRPCError
+    """Base class for JSON-RPC 2.0 protocol implementation."""
+
+    default_error_class: ClassVar = InternalError
+    """Default JSON-RPC 2.0 error class to represent internal exceptions."""
+
+    _errors_map: ClassVar = {
+        Exception: JsonRPCError,
+        RPCError: JsonRPCError,
+        BadRequestError: InvalidRequestError,
+        NotFoundError: MethodNotFoundError,
+        InvalidParametersError: InvalidParamsError,
+        InternalServerError: InternalError,
+        SerializationError: InternalError,
+        DeserializationError: ParseError,
+        AuthenticationFailedError: AuthenticationFailedJRPCError,
+        InvalidTokenError: InvalidTokenJRPCError,
+        ForbiddenError: ForbiddenJRPCError,
+        InvalidPermissionsError: InvalidPermissionsJRPCError,
+    }
+
+    def __init__(
+        self,
+        registry: RPCRegistry | None = None,
+        serializer: BaseSerializer | None = None,
+        schema_serializer: BaseSerializer | None = None,
+        openrpc: ORPC.OpenRPC | None = None,
+        openapi: OAPI.OpenAPI | None = None,
+        allow_service_discovery: bool | None = None,
+        schema_url: str | None = None,
+    ):
+        if serializer is None:
+            serializer = JsonSerializer()
+
+        super().__init__(
+            registry=registry,
+            serializer=serializer,
+            schema_serializer=schema_serializer,
+        )
+        self.allow_service_discovery = allow_service_discovery
+        self.schema_url = schema_url
+
+        # Schemas
+        self.openrpc_schema_template = (
+            openrpc if openrpc is not None else DEFAULT_OPENRPC_SCHEMA
+        )
+        self.__openrpc_schema = None
+        self.openapi_schema_template = (
+            openapi if openapi is not None else DEFAULT_OPENAPI_SCHEMA
+        )
+        self.__openapi_schema = None
+
+        if allow_service_discovery:
+            self.registry.register_rpc_extension(
+                extension_procedure=self.rpc_discover,
+                extension_name="rpc.discover",
+            )
+
+    def handle(
+        self,
+        rpc_request: JSONRPCRequest,
+        request: Any | None = None,
+    ) -> JSONRPCResponse | None:
+        """Handles a procedure call or batch of procedure call
+
+        :param rpc_request:
+            RPC request in protocol format.
+        :type rpc_request: JSONRPCRequest
+        :param request:
+            Optional parameter that can be passed as an
+            argument to the procedure.
+        :type request: Any
+        :return:
+            Returns the result in protocol format.
+        :rtype: JSONRPCResponse
+
+        """
+        # Check bad request
+        if not (isinstance(rpc_request, (dict, list)) and len(rpc_request) > 0):
+            return InvalidRequestError().as_dict()
+
+        # Handle batch request
+        if isinstance(rpc_request, list):
+            batch_result = []
+            for request_object in rpc_request:
+                result = self.execute(request_object, request=request)
+                if result is not None:
+                    batch_result.append(result)
+            if len(batch_result) == 0:
+                return None
+            return batch_result
+
+        # Handle single request
+        return self.execute(rpc_request, request=request)
+
+    def execute(
+        self,
+        procedure_call: JSONRPCRequestObject,
+        request: Any | None = None,
+    ) -> JSONRPCResponseObject | None:
+        """Execute a remote procedure call.
+
+        :param procedure_call:
+            RPC request object in protocol format.
+        :type procedure_call: JSONRPCRequestObject
+        :param request:
+            Optional parameter that can be passed as an
+            argument to the procedure. By default, None will be passed.
+        :type request: Any
+        :return:
+            Returns a result object in protocol format.
+        :rtype: JSONRPCResponseObject
+
+        """
+        if not isinstance(procedure_call, dict):
+            return InvalidRequestError().as_dict()
+        method: str = procedure_call.get("method")
+        params: list | dict | None = procedure_call.get("params")
+        request_id: int | str | None = procedure_call.get("id")
+
+        # Validate protocol
+        if (
+            procedure_call.get("jsonrpc") != "2.0"
+            or not isinstance(method, str)
+            or not (params is None or isinstance(params, (list, dict)))
+            or not (request_id is None or isinstance(request_id, (int, str)))
+        ):
+            return InvalidRequestError(id=request_id).as_dict()
+
+        # Getting procedure
+        procedure = self.registry[method]
+        if procedure is None:
+            if request_id is None:
+                return None
+            return MethodNotFoundError(id=request_id).as_dict()
+
+        # Prepare parameters
+        args, kwargs = (), {}
+        if params is not None:
+            if isinstance(params, list):
+                args = (request, *params)
+            elif isinstance(params, dict):
+                kwargs = dict(request=request, **params)
+        else:
+            kwargs = dict(request=request)
+
+        # Execute RPC method
+        try:
+            result = procedure(*args, **kwargs)
+        except RPCError as err:
+            error = self.handle_error(err)
+            error.id = request_id
+            return error.as_dict()
+        except Exception as err:
+            return InternalError(message=str(err), id=request_id).as_dict()
+
+        if request_id is None:
+            return None
+
+        return dict(jsonrpc="2.0", result=result, id=request_id)
+
+    def rpc_discover(self) -> dict[str, Any]:
+        """Returns an OpenRPC schema as a description of this service.
+
+        :return:
+
+        """
+        if self.schema_url is not None:
+            self._validate_rpc_url()
+            schema = {"$ref": self.schema_url}
+        else:
+            schema = self.openrpc_schema()
+
+        return {"name": "OpenRPC Schema", "schema": schema}
+
+    def openrpc_schema(self) -> ORPC.OpenRPC:
+        """Implementation of OpenRPC specification.
+
+        https://spec.open-rpc.org/
+
+        """
+        if not self.__openrpc_schema:
+            openrpc: ORPC.OpenRPC = deepcopy(self.openrpc_schema_template)
+
+            for method_name, procedure_ in self.registry.items():
+                procedure = unwrap_func(procedure_)
+                try:
+                    method_schema: MethodSchema = getattr(procedure, RPC_SCHEMA)
+                except AttributeError:
+                    break
+
+                method = ORPC.Method(
+                    name=method_name,
+                    params=[],
+                    result={},
+                    deprecated=method_schema.get("deprecated", False),
+                )
+                if "short_description" in method_schema:
+                    method["summary"] = method_schema["short_description"]
+                if "description" in method_schema:
+                    method["description"] = method_schema["description"]
+
+                # Fill parameters schema
+                parameters = method_schema.get("parameters", {})
+                for param_name, parameter in parameters.items():
+                    cd_param = ORPC.ContentDescriptor(
+                        name=parameter.get("name", param_name),
+                        schema=ORPC.Schema(),
+                        required=parameter.get("required", False),
+                        deprecated=parameter.get("deprecated", False),
+                    )
+                    if "type" in parameter:
+                        cd_param["schema"]["type"] = ORPC.type_mapping(
+                            parameter["type"],
+                        )
+                    if "default" in parameter:
+                        cd_param["schema"]["default"] = parameter["default"]
+                    if "description" in parameter:
+                        cd_param["summary"] = parameter["description"]
+                        cd_param["description"] = parameter["description"]
+
+                    method["params"].append(cd_param)
+
+                # Fill result schema
+                if "result" in method_schema:
+                    result_schema = method_schema["result"]
+                    cd_result = ORPC.ContentDescriptor(
+                        name=result_schema.get("name", "result"),
+                        schema=ORPC.Schema(),
+                    )
+                    if "type" in result_schema:
+                        cd_result["schema"]["type"] = ORPC.type_mapping(
+                            result_schema.get("type"),
+                        )
+                    if "description" in result_schema:
+                        cd_result["summary"] = result_schema["description"]
+                        cd_result["description"] = result_schema["description"]
+
+                    method["result"] = cd_result
+
+                openrpc["methods"].append(method)
+
+            self.__openrpc_schema = openrpc
+        return self.__openrpc_schema
+
+    def openapi_schema(self) -> dict:
+        """Implementation of OpenAPI specification.
+
+        https://spec.openapis.org/oas/latest.html
+
+        """
+        if not self.__openapi_schema:
+            openapi: OAPI.OpenAPI = deepcopy(self.openapi_schema_template)
+
+            for method_name, procedure_ in self.registry.items():
+                procedure = unwrap_func(procedure_)
+                try:
+                    method_schema: MethodSchema = getattr(procedure, RPC_SCHEMA)
+                except AttributeError:
+                    break
+
+                path_name = self.schema_url + "#" + method_name
+                operation = OAPI.Operation(
+                    operationId=method_name,
+                    parameters=[],
+                    deprecated=method_schema.get("deprecated", False),
+                )
+                if "short_description" in method_schema:
+                    operation["summary"] = method_schema["short_description"]
+                if "description" in method_schema:
+                    operation["description"] = method_schema["description"]
+
+                # Fill request body
+                parameters = method_schema.get("parameters", {}).items()
+                media = OAPI.MediaType(
+                    schema=OAPI.Schema(
+                        type="object",
+                        properties={
+                            "jsonrpc": {
+                                "type": "string",
+                                "description": "Protocol version",
+                            },
+                            "method": {
+                                "type": "string",
+                                "description": "Procedure (method) name",
+                            },
+                            "params": {
+                                "type": "object",
+                                "properties": {
+                                    param_name: {
+                                        "default": parameter.get("default", ""),
+                                        "description": parameter.get(
+                                            "description",
+                                            "",
+                                        ),
+                                        "deprecated": parameter.get(
+                                            "deprecated",
+                                            False,
+                                        ),
+                                    }
+                                    for param_name, parameter in parameters
+                                },
+                            },
+                            "id": {
+                                "type": "string",
+                            },
+                        },
+                        required=["jsonrpc", "method"],
+                    ),
+                )
+                if "example" in method_schema:
+                    media["example"] = method_schema["example"]
+                if "examples" in method_schema:
+                    media["examples"] = method_schema["examples"]
+                operation["requestBody"] = OAPI.RequestBody(
+                    content={"application/json": media},
+                    description="JSON-RPC 2.0 Request Object",
+                    required=True,
+                )
+
+                # Fill result schema
+                if "result" in method_schema:
+                    result_schema = method_schema["result"]
+
+                    media = OAPI.MediaType(
+                        schema=OAPI.Schema(
+                            type="object",
+                            properties=dict(
+                                jsonrpc=dict(type="string", default="2.0"),
+                                result=dict(),
+                                id=dict(type="string"),
+                            ),
+                        ),
+                    )
+                    if "type" in result_schema:
+                        media["schema"]["type"] = OAPI.type_mapping(
+                            result_schema.get("type"),
+                        )
+                    if "description" in result_schema:
+                        media["schema"]["description"] = result_schema[
+                            "description"
+                        ]
+                    if "example" in result_schema:
+                        media["example"] = result_schema["example"]
+                    if "examples" in result_schema:
+                        media["examples"] = result_schema["examples"]
+                else:
+                    # If returns type is NoneType
+                    media = OAPI.MediaType(
+                        schema=OAPI.Schema(
+                            type="object",
+                            properties=dict(
+                                jsonrpc=dict(type="string", default="2.0"),
+                                result=dict(type="null"),
+                                id=dict(type="string"),
+                            ),
+                        ),
+                    )
+                operation["responses"] = OAPI.Responses(
+                    **{
+                        "200": OAPI.Response(
+                            description="JSON-RPC 2.0 Response Object",
+                            content={"application/json": media},
+                        ),
+                    },
+                )
+
+                openapi["paths"][path_name] = OAPI.PathItem(post=operation)
+
+            self.__openapi_schema = openapi
+        return self.__openapi_schema
+
+    def _validate_rpc_url(self):
+        assert bool(self.schema_url), (
+            "To use service description schemes, "
+            "you must specify the URL responsible for processing "
+            "RPC requests."
+        )
```

### Comparing `drakaina-0.7.0b3/drakaina/serializers.py` & `drakaina-0.7.0b4/drakaina/serializers.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/tcp.py` & `drakaina-0.7.0b4/drakaina/tcp.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/drakaina/types.py` & `drakaina-0.7.0b4/drakaina/types.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,847 +1,893 @@
-from __future__ import annotations
-
-from collections import OrderedDict
-from collections.abc import Awaitable
-from collections.abc import Callable
-from collections.abc import Mapping
-from collections.abc import MutableMapping
-from collections.abc import MutableSequence
-from collections.abc import Sequence
-from enum import StrEnum
-from sys import version_info
-from typing import Any
-from typing import Dict
-from typing import Iterable
-from typing import Literal
-from typing import Protocol
-from typing import Tuple
-from typing import Type
-from typing import TypedDict
-from typing import Union
-
-if version_info < (3, 10):
-    from typing_extensions import TypeAlias
-else:
-    from typing import TypeAlias
-
-if version_info < (3, 11):
-    from typing_extensions import NotRequired
-else:
-    from typing import NotRequired
-
-
-"""
-JSON-RPC types definitions
-"""
-
-JSONSimpleTypes: TypeAlias = Union[str, int, float, bool, None]
-JSONTypes: TypeAlias = Union[
-    JSONSimpleTypes,
-    Mapping[str, JSONSimpleTypes],
-    Sequence[JSONSimpleTypes],
-]
-
-
-class JSONRPCRequestObject(TypedDict):
-    jsonrpc: Literal["2.0"]
-    method: str
-    params: NotRequired[list[JSONTypes] | dict[str, JSONTypes]]
-    id: NotRequired[str | int | None]
-
-
-class JSONRPCErrorObject(TypedDict):
-    code: int
-    message: str
-    data: NotRequired[JSONTypes]
-
-
-class JSONRPCResponseObject(TypedDict):
-    jsonrpc: Literal["2.0"]
-    result: NotRequired[JSONTypes]
-    error: NotRequired[JSONRPCErrorObject]
-    id: str | int | None
-
-
-JSONRPCBatchRequestObject: TypeAlias = Sequence[JSONRPCRequestObject]
-JSONRPCRequest: TypeAlias = Union[
-    JSONRPCRequestObject,
-    JSONRPCBatchRequestObject,
-]
-JSONRPCBatchResponseObject: TypeAlias = Sequence[JSONRPCResponseObject]
-JSONRPCResponse: TypeAlias = Union[
-    JSONRPCResponseObject,
-    JSONRPCBatchResponseObject,
-]
-
-
-"""
-Schema types
-"""
-
-json_schema_type_mapping = {
-    None: "null",
-    type(None): "null",
-    "None": "null",
-    "NoneType": "null",
-    bool: "boolean",
-    "bool": "boolean",
-    int: "integer",  # number?
-    "int": "integer",
-    float: "number",
-    "float": "number",
-    str: "string",
-    "str": "string",
-    list: "array",
-    "list": "array",
-    dict: "object",
-    "dict": "object",
-}
-
-
-def get_json_schema_type(t: type | str) -> str:
-    result = json_schema_type_mapping.get(t)
-    if result is None:
-        result = str(t)
-    return result
-    # if isinstance(t, type):
-    #     result = json_schema_type_mapping.get(t)
-    #     if result is None:
-    #         result = str(t)
-    #     return result
-
-
-_JSONSchema = TypedDict(
-    "_JSONSchema",
-    {
-        "$id": NotRequired[str],
-        "$ref": NotRequired[str],
-        "$dynamicRef": NotRequired[str],
-        "$dynamicAnchor": NotRequired[str],
-        "$schema": NotRequired[str],
-    },
-)
-
-
-class JSONSchema(_JSONSchema):
-    """JSON schema.
-
-    https://datatracker.ietf.org/doc/html/draft-bhutton-json-schema-00
-
-    """
-
-    base: NotRequired[str]
-    type: NotRequired[str | Sequence[str]]
-    description: NotRequired[str]
-    format: NotRequired[str]
-    required: NotRequired[list[str]]
-
-
-Reference = TypedDict(
-    "Reference",
-    {
-        "$ref": str,  # noqa
-        "summary": NotRequired[str],
-        "description": NotRequired[str],
-    },
-)
-
-
-class ParameterSchema(TypedDict):
-    name: NotRequired[str]
-    short_description: NotRequired[str]
-    description: NotRequired[str]
-    type: NotRequired[str]
-    default: NotRequired[Any]
-    required: NotRequired[bool]
-    """Default: False"""
-    deprecated: NotRequired[bool]
-    """Default: False"""
-
-
-class MethodSchema(TypedDict):
-    name: NotRequired[str]
-    short_description: NotRequired[str]
-    description: NotRequired[str]
-    parameters: NotRequired[OrderedDict[str, ParameterSchema]]
-    result: NotRequired[ParameterSchema]
-    notification: NotRequired[bool]
-    deprecated: NotRequired[bool]
-    errors: NotRequired[dict[str, str]]
-    example: NotRequired[Any]
-    examples: NotRequired[Sequence[Any]]
-    # tags: NotRequired[list[ORPCTag | Reference]]
-    # paramStructure: NotRequired[Literal["by-name", "by-position", "either"]]
-    # TODO: **MethodSchema(errors, examples, tags, )
-
-
-"""
-Schema types - OpenRPC
-https://spec.open-rpc.org/
-"""
-
-SUPPORTED_OPENRPC_VERSION = "1.2.1"
-
-
-class OpenRPC(TypedDict):
-    openrpc: Literal["1.2.1"]
-    info: ORPCInfo
-    methods: list[ORPCMethod | Reference]
-    servers: NotRequired[list[ORPCServer]]
-    components: NotRequired[ORPCComponents]
-    externalDocs: NotRequired[ORPCExtDoc]
-
-
-class ORPCInfo(TypedDict):
-    title: str
-    version: str
-    description: NotRequired[str]
-    termsOfService: NotRequired[str]
-    contact: NotRequired[ORPCContact]
-    license: NotRequired[ORPCLicense]
-
-
-class ORPCContact(TypedDict):
-    name: NotRequired[str]
-    url: NotRequired[str]
-    email: NotRequired[str]
-
-
-class ORPCLicense(TypedDict):
-    name: str
-    url: NotRequired[str]
-
-
-class ORPCServer(TypedDict):
-    name: str
-    url: str
-    """Runtime Expression"""
-    summary: NotRequired[str]
-    description: NotRequired[str]
-    variables: NotRequired[Mapping[str, ORPCServerVar]]
-
-
-class ORPCServerVar(TypedDict):
-    default: str
-    enum: NotRequired[list[str]]
-    description: NotRequired[str]
-
-
-class ORPCMethod(TypedDict):
-    name: str
-    params: list[ORPCContentDescriptor | Reference]
-    result: NotRequired[ORPCContentDescriptor | Reference]
-    tags: NotRequired[list[ORPCTag | Reference]]
-    summary: NotRequired[str]
-    description: NotRequired[str]
-    externalDocs: NotRequired[ORPCExtDoc]
-    deprecated: NotRequired[bool]
-    """Default: False"""
-    servers: NotRequired[list[ORPCServer]]
-    errors: NotRequired[list[JSONRPCErrorObject | Reference]]
-    links: NotRequired[list[ORPCLink | Reference]]
-    paramStructure: NotRequired[Literal["by-name", "by-position", "either"]]
-    examples: NotRequired[list[ORPCExamplePairing]]
-
-
-class ORPCContentDescriptor(TypedDict):
-    name: str
-    schema: JSONSchema
-    summary: NotRequired[str]
-    description: NotRequired[str]
-    required: NotRequired[bool]
-    """Default: False"""
-    deprecated: NotRequired[bool]
-    """Default: False"""
-
-
-class ORPCExamplePairing(TypedDict):
-    name: NotRequired[str]
-    summary: NotRequired[str]
-    description: NotRequired[str]
-    params: NotRequired[list[ORPCExample | Reference]]
-    result: NotRequired[ORPCExample | Reference]
-
-
-class ORPCExample(TypedDict):
-    name: NotRequired[str]
-    summary: NotRequired[str]
-    description: NotRequired[str]
-    value: NotRequired[Any]
-    externalValue: NotRequired[str]
-
-
-class ORPCLink(TypedDict):
-    name: str
-    summary: NotRequired[str]
-    description: NotRequired[str]
-    method: NotRequired[str]
-    params: NotRequired[Mapping[str, Any | str]]
-    """Mapping[str, Any | 'Runtime Expression']"""
-    server: NotRequired[ORPCServer]
-
-
-class ORPCComponents(TypedDict):
-    contentDescriptors: NotRequired[Mapping[str, ORPCContentDescriptor]]
-    schemas: NotRequired[Mapping[str, JSONSchema]]
-    examples: NotRequired[Mapping[str, ORPCExample]]
-    links: NotRequired[Mapping[str, ORPCLink]]
-    errors: NotRequired[Mapping[str, JSONRPCErrorObject]]
-    examplePairingObjects: NotRequired[Mapping[str, ORPCExamplePairing]]
-    tags: NotRequired[Mapping[str, ORPCTag]]
-
-
-class ORPCTag(TypedDict):
-    name: str
-    summary: NotRequired[str]
-    description: NotRequired[str]
-    externalDocs: NotRequired[ORPCExtDoc]
-
-
-class ORPCExtDoc(TypedDict):
-    url: str
-    description: NotRequired[str]
-
-
-class ORPC:
-    SUPPORTED_VERSION = SUPPORTED_OPENRPC_VERSION
-    OpenRPC = OpenRPC
-    Info = ORPCInfo
-    Contact = ORPCContact
-    License = ORPCLicense
-    Server = ORPCServer
-    ServerVar = ORPCServerVar
-    Method = ORPCMethod
-    ContentDescriptor = ORPCContentDescriptor
-    Schema = JSONSchema
-    ExamplePairing = ORPCExamplePairing
-    Example = ORPCExample
-    Link = ORPCLink
-    Components = ORPCComponents
-    Tag = ORPCTag
-    ExtDoc = ORPCExtDoc
-    Reference = Reference
-
-    type_mapping = get_json_schema_type
-
-
-"""
-Schema types - OpenAPI
-https://github.com/OAI/OpenAPI-Specification
-"""
-
-SUPPORTED_OPENAPI_VERSION = "3.0.0"
-
-
-class OpenAPI(TypedDict):
-    openapi: Literal["3.1.0"]
-    info: OASInfo
-    jsonSchemaDialect: NotRequired[str]
-    """URI"""
-    servers: NotRequired[list[OASServer]]
-    paths: NotRequired[OASPaths]
-    """OASPaths["/{path}", OASPathItem]"""
-    webhooks: NotRequired[Mapping[str, OASPathItem | Reference]]
-    components: NotRequired[OASComponents]
-    security: NotRequired[list[OASSecurityRequirement]]
-    tags: NotRequired[list[OASTag]]
-    externalDocs: NotRequired[OASExtDoc]
-
-
-class OASInfo(TypedDict):
-    title: str
-    version: str
-    summary: NotRequired[str]
-    description: NotRequired[str]
-    termsOfService: NotRequired[str]
-    contact: NotRequired[OASContact]
-    license: NotRequired[OASLicense]
-
-
-class OASContact(TypedDict):
-    name: NotRequired[str]
-    url: NotRequired[str]
-    email: NotRequired[str]
-
-
-class OASLicense(TypedDict):
-    name: str
-    identifier: NotRequired[str]
-    url: NotRequired[str]
-
-
-class OASServer(TypedDict):
-    url: str
-    description: NotRequired[str]
-    variables: NotRequired[Mapping[str, OASServerVar]]
-
-
-class OASServerVar(TypedDict):
-    default: str
-    enum: NotRequired[list[str]]
-    description: NotRequired[str]
-
-
-class OASComponents(TypedDict):
-    schemas: NotRequired[Mapping[str, OASSchema]]
-    responses: NotRequired[Mapping[str, OASResponse | Reference]]
-    parameters: NotRequired[Mapping[str, OASParameter | Reference]]
-    examples: NotRequired[Mapping[str, OASExample | Reference]]
-    requestBodies: NotRequired[Mapping[str, OASRequestBody | Reference]]
-    headers: NotRequired[Mapping[str, OASHeader | Reference]]
-    securitySchemes: NotRequired[Mapping[str, OASSecurityScheme | Reference]]
-    links: NotRequired[Mapping[str, OASLink | Reference]]
-    callbacks: NotRequired[Mapping[str, OASCallback | Reference]]
-    pathItems: NotRequired[Mapping[str, OASPathItem | Reference]]
-
-
-OASPathItemRef = TypedDict(
-    "OASPathItemRef",
-    {"$ref": NotRequired[str]},
-)
-
-
-class OASPathItem(OASPathItemRef):
-    summary: NotRequired[str]
-    description: NotRequired[str]
-    get: NotRequired[OASOperation]
-    put: NotRequired[OASOperation]
-    post: NotRequired[OASOperation]
-    delete: NotRequired[OASOperation]
-    options: NotRequired[OASOperation]
-    head: NotRequired[OASOperation]
-    patch: NotRequired[OASOperation]
-    trace: NotRequired[OASOperation]
-    servers: NotRequired[OASServer]
-    parameters: NotRequired[OASParameter | Reference]
-
-
-OASPaths = TypedDict("OASPaths", {"/{path}": OASPathItem})
-
-
-class OASOperation(TypedDict):
-    tags: NotRequired[list[str]]
-    summary: NotRequired[str]
-    description: NotRequired[str]
-    externalDocs: NotRequired[OASExtDoc]
-    operationId: NotRequired[str]
-    parameters: NotRequired[Sequence[OASParameter | Reference]]
-    requestBody: NotRequired[OASRequestBody | Reference]
-    responses: NotRequired[OASResponses]
-    callbacks: NotRequired[Mapping[str, OASCallback | Reference]]
-    deprecated: NotRequired[bool]
-    security: NotRequired[Sequence[OASSecurityRequirement]]
-    servers: NotRequired[Sequence[OASServer]]
-
-
-class OASExtDoc(TypedDict):
-    url: str
-    description: NotRequired[str]
-
-
-class OASParameterLocation(StrEnum):
-    PATH = "path"
-    QUERY = "query"
-    HEADER = "header"
-    COOKIE = "cookie"
-
-
-OASParameterIn = TypedDict(
-    "OASParameterIn",
-    {"in": OASParameterLocation},
-)
-
-
-class OASParameter(OASParameterIn):
-    name: str
-    # in: str
-    description: NotRequired[str]
-    required: NotRequired[bool]
-    """required = True if `in` == 'path'"""
-    deprecated: NotRequired[bool]
-    allowEmptyValue: NotRequired[bool]
-    style: NotRequired[str]
-    explode: NotRequired[bool]
-    allowReserved: NotRequired[bool]
-    schema: NotRequired[OASSchema]
-    example: NotRequired[Any]
-    examples: NotRequired[Mapping[str, OASExample | Reference]]
-    content: NotRequired[Mapping[str, OASMediaType]]
-    """A parameter MUST contain either a schema property, or
-    a content property, but not both."""
-
-
-class OASRequestBody(TypedDict):
-    content: Mapping[str, OASMediaType]
-    description: NotRequired[str]
-    required: NotRequired[bool]
-
-
-class OASMediaType(TypedDict):
-    schema: NotRequired[OASSchema]
-    example: NotRequired[Any]
-    examples: NotRequired[Mapping[str, OASExample | Reference]]
-    encoding: NotRequired[Mapping[str, OASEncoding]]
-
-
-class OASEncoding(TypedDict):
-    contentType: NotRequired[str]
-    headers: NotRequired[Mapping[str, OASHeader | Reference]]
-    style: NotRequired[str]
-    explode: NotRequired[bool]
-    allowReserved: NotRequired[bool]
-
-
-class OASResponse(TypedDict):
-    description: str
-    headers: NotRequired[Mapping[str, OASHeader | Reference]]
-    content: NotRequired[Mapping[str, OASMediaType]]
-    links: NotRequired[Mapping[str, OASLink | Reference]]
-
-
-OASResponses = TypedDict(
-    "OASResponses",
-    {
-        "{status_code}": NotRequired[Union[OASResponse, Reference]],
-        "default": NotRequired[Union[OASResponse, Reference]],
-    },
-)
-
-
-OASCallback = Dict[str, Union[OASPathItem, Reference]]
-
-
-class OASExample(TypedDict):
-    summary: NotRequired[str]
-    description: NotRequired[str]
-    value: NotRequired[Any]
-    externalValue: NotRequired[str]
-
-
-class OASLink(TypedDict):
-    operationRef: NotRequired[str]
-    operationId: NotRequired[str]
-    parameters: NotRequired[Mapping[str, Any | str]]
-    """NotRequired[Mapping[str, Any | {expression}]]"""
-    description: NotRequired[str]
-    server: NotRequired[OASServer]
-
-
-class OASHeader(TypedDict):
-    description: NotRequired[str]
-    required: NotRequired[bool]
-    deprecated: NotRequired[bool]
-    allowEmptyValue: NotRequired[bool]
-    style: NotRequired[str]
-    explode: NotRequired[bool]
-    allowReserved: NotRequired[bool]
-    schema: NotRequired[OASSchema]
-    example: NotRequired[Any]
-    examples: NotRequired[Mapping[str, OASExample | Reference]]
-    content: NotRequired[Mapping[str, OASMediaType]]
-    """A parameter MUST contain either a schema property, or
-    a content property, but not both."""
-
-
-class OASTag(TypedDict):
-    name: str
-    description: NotRequired[str]
-    externalDocs: NotRequired[OASExtDoc]
-
-
-class OASSchema(JSONSchema):
-    discriminator: NotRequired[OASDiscriminator]
-    xml: NotRequired[OASXML]
-    externalDocs: NotRequired[OASExtDoc]
-    example: NotRequired[Any]
-
-
-class OASDiscriminator(TypedDict):
-    propertyName: str
-    mapping: NotRequired[Mapping[str, str]]
-
-
-class OASXML(TypedDict):
-    name: NotRequired[str]
-    namespace: NotRequired[str]
-    prefix: NotRequired[str]
-    attribute: NotRequired[bool]
-    wrapped: NotRequired[bool]
-
-
-class OASSecuritySchemeType(StrEnum):
-    API_KEY = "apiKey"
-
-
-class OASSecuritySchemeLocation(StrEnum):
-    QUERY = "query"
-    HEADER = "header"
-    COOKIE = "cookie"
-
-
-OASSecuritySchemeIn = TypedDict(
-    "OASSecuritySchemeIn",
-    {"in": OASSecuritySchemeLocation},
-)
-
-
-class OASSecurityScheme(OASSecuritySchemeIn):
-    type: OASSecuritySchemeType
-    name: str
-    scheme: str
-    flows: OASOAuthFlows
-    openIdConnectUrl: str
-    description: NotRequired[str]
-    bearerFormat: NotRequired[str]
-
-
-class OASOAuthFlows(TypedDict):
-    implicit: NotRequired[OASOAuthFlow]
-    password: NotRequired[OASOAuthFlow]
-    clientCredentials: NotRequired[OASOAuthFlow]
-    authorizationCode: NotRequired[OASOAuthFlow]
-
-
-class OASOAuthFlow(TypedDict):
-    authorizationUrl: str
-    tokenUrl: str
-    scopes: str
-    refreshUrl: NotRequired[str]
-
-
-OASSecurityRequirement = Dict[str, list[str]]
-
-
-class OAPI:
-    SUPPORTED_VERSION = SUPPORTED_OPENAPI_VERSION
-    OpenAPI = OpenAPI
-    Info = OASInfo
-    Contact = OASContact
-    License = OASLicense
-    Server = OASServer
-    ServerVar = OASServerVar
-    Components = OASComponents
-    Paths = OASPaths
-    PathItem = OASPathItem
-    Operation = OASOperation
-    ExtDoc = OASExtDoc
-    ParameterLocation = OASParameterLocation
-    Parameter = OASParameter
-    RequestBody = OASRequestBody
-    MediaType = OASMediaType
-    Encoding = OASEncoding
-    Responses = OASResponses
-    Response = OASResponse
-    Callback = OASCallback
-    Example = OASExample
-    Link = OASLink
-    Header = OASHeader
-    Tag = OASTag
-    Reference = Reference
-    Schema = OASSchema
-    Discriminator = OASDiscriminator
-    XML = OASXML
-    SecurityScheme = OASSecurityScheme
-    OAuthFlows = OASOAuthFlows
-    OAuthFlow = OASOAuthFlow
-    SecurityRequirement = OASSecurityRequirement
-
-    type_mapping = get_json_schema_type
-
-
-"""
-WSGI types definitions
-PEP 3333 – Python Web Server Gateway Interface
-https://peps.python.org/pep-3333/
-"""
-
-WSGIEnvironmentKeys: TypeAlias = Literal[
-    # for CGI
-    # https://datatracker.ietf.org/doc/html/draft-coar-cgi-v11-03
-    "AUTH_TYPE",
-    "CONTENT_LENGTH",
-    "CONTENT_TYPE",
-    "GATEWAY_INTERFACE",
-    "PATH_INFO",
-    "PATH_TRANSLATED",
-    "QUERY_STRING",
-    "REMOTE_ADDR",
-    "REMOTE_HOST",
-    "REMOTE_IDENT",
-    "REMOTE_USER",
-    "REQUEST_METHOD",
-    "SCRIPT_NAME",
-    "SERVER_NAME",
-    "SERVER_PORT",
-    "SERVER_PROTOCOL",
-    "SERVER_SOFTWARE",
-    # for WSGI
-    "wsgi.errors",
-    "wsgi.input",
-    "wsgi.multiprocess",
-    "wsgi.multithread",
-    "wsgi.run_once",
-    "wsgi.url_scheme",
-    "wsgi.version",
-]
-# for framework needs
-WSGIDrakainaKeys: TypeAlias = Literal[
-    "drakaina.app",
-    "drakaina.is_authenticated",
-]
-WSGIEnvironment: TypeAlias = MutableMapping[str, Any]
-WSGIExceptionInfo: TypeAlias = Tuple[Type[BaseException], BaseException, Any]
-
-
-class WSGIStartResponse(Protocol):
-    def __call__(
-        self,
-        status: str,
-        headers: MutableSequence[tuple[str, str]],
-        exc_info: WSGIExceptionInfo | None = ...,
-    ) -> Callable[[bytes], Any]:
-        ...
-
-
-WSGIResponse: TypeAlias = Iterable[bytes]
-WSGIApplication: TypeAlias = Callable[
-    [WSGIEnvironment, WSGIStartResponse],
-    WSGIResponse,
-]
-
-
-class WSGIInputStream(Protocol):
-    def read(self, size: int | None = None) -> bytes:
-        ...
-
-    def readline(self) -> bytes:
-        ...
-
-    def readlines(self, hint: Any | None) -> Iterable[bytes]:
-        ...
-
-    def __iter__(self) -> bytes:
-        ...
-
-
-class WSGIErrorsStream(Protocol):
-    def flush(self) -> None:
-        ...
-
-    def write(self, s: str) -> None:
-        ...
-
-    def writelines(self, seq: Sequence[str]) -> None:
-        ...
-
-
-"""
-ASGI types definitions
-https://asgi.readthedocs.io/en/latest/
-"""
-
-ASGIScope: TypeAlias = MutableMapping[str, Any]
-ASGIMessage: TypeAlias = MutableMapping[str, Any]
-
-ASGIReceive: TypeAlias = Callable[[], Awaitable[ASGIMessage]]
-ASGISend: TypeAlias = Callable[[ASGIMessage], Awaitable[None]]
-
-ASGIApplication: TypeAlias = Callable[
-    [ASGIScope, ASGIReceive, ASGISend],
-    Awaitable[None],
-]
-
-
-"""
-Helpful types
-"""
-
-
-class Comparator(Protocol):
-    def __call__(
-        self,
-        required: Iterable[str],
-        provided: str | Iterable[str],
-    ) -> bool:
-        ...
-
-
-class ProxyRequest(MutableMapping):
-    """A wrapper class for environment mapping.
-
-    :param environment:
-
-    """
-
-    __slots__ = ("__environment",)
-
-    def __init__(self, environment: ASGIScope | WSGIEnvironment):
-        self.__environment = environment
-
-    def __getitem__(self, item):
-        return self.__environment[item]
-
-    def __setitem__(self, key, value):
-        self.__environment[key] = value
-
-    def __delitem__(self, key):
-        del self.__environment[key]
-
-    def __iter__(self):
-        return iter(self.__environment.keys())
-
-    def __contains__(self, item):
-        return item in self.__environment.keys()
-
-    def __len__(self):
-        return len(self.__environment)
-
-    def keys(self):
-        return self.__environment.keys()
-
-    def values(self):
-        return self.__environment.values()
-
-    def items(self):
-        return self.__environment.items()
-
-    def get(self, key, default=None):
-        return self.__environment.get(key, default)
-
-    def clear(self):
-        self.__environment.clear()
-
-    def setdefault(self, key, default=None):
-        self.__environment.setdefault(key, default)
-
-    def pop(self, key, default=None):
-        return self.__environment.pop(key, default)
-
-    def popitem(self):
-        return self.__environment.popitem()
-
-    def copy(self):
-        return self.__class__(self.__environment.copy())
-
-    def update(self, *args, **kwargs):
-        return self.__environment.update(*args, **kwargs)
-
-    def __getattr__(self, item):
-        if item in ("__environment", "_ProxyRequest__environment"):
-            super().__getattribute__(item)
-        return self.__environment[item]
-
-    def __setattr__(self, key, value):
-        if key in ("__environment", "_ProxyRequest__environment"):
-            super().__setattr__(key, value)
-        else:
-            self.__environment[key] = value
-
-    def __delattr__(self, item):
-        del self.__environment[item]
-
-
-AnyRequest: TypeAlias = Union[
-    ASGIScope,
-    WSGIEnvironment,
-    ProxyRequest,
-]
+from __future__ import annotations
+
+from collections import OrderedDict
+from collections.abc import Awaitable
+from collections.abc import Callable
+from collections.abc import Mapping
+from collections.abc import MutableMapping
+from collections.abc import MutableSequence
+from collections.abc import Sequence
+from sys import version_info
+from typing import Any
+from typing import Dict
+from typing import Iterable
+from typing import Literal
+from typing import Protocol
+from typing import Tuple
+from typing import Type
+from typing import TypedDict
+from typing import Union
+
+if version_info < (3, 10):
+    from typing_extensions import TypeAlias
+else:
+    from typing import TypeAlias
+
+if version_info < (3, 11):
+    from enum import Enum
+    from typing_extensions import NotRequired
+
+    # Copied from python 3.11
+
+    class ReprEnum(Enum):
+        """
+        Only changes the repr(), leaving str() and format()
+        to the mixed-in type.
+        """
+
+    class StrEnum(str, ReprEnum):
+        """
+        Enum where members are also (and must be) strings
+        """
+
+        def __new__(cls, *values):
+            "values must already be of type `str`"
+            if len(values) > 3:
+                raise TypeError("too many arguments for str(): %r" % (values,))
+            if len(values) == 1:
+                # it must be a string
+                if not isinstance(values[0], str):
+                    raise TypeError("%r is not a string" % (values[0],))
+            if len(values) >= 2:
+                # check that encoding argument is a string
+                if not isinstance(values[1], str):
+                    raise TypeError(
+                        "encoding must be a string, not %r" % (values[1],),
+                    )
+            if len(values) == 3:
+                # check that errors argument is a string
+                if not isinstance(values[2], str):
+                    raise TypeError(
+                        "errors must be a string, not %r" % (values[2]),
+                    )
+            value = str(*values)
+            member = str.__new__(cls, value)
+            member._value_ = value
+            return member
+
+        def _generate_next_value_(name, start, count, last_values):
+            """
+            Return the lower-cased version of the member name.
+            """
+            return name.lower()
+
+else:
+    from enum import StrEnum
+    from typing import NotRequired
+
+
+"""
+JSON-RPC types definitions
+"""
+
+JSONSimpleTypes: TypeAlias = Union[str, int, float, bool, None]
+JSONTypes: TypeAlias = Union[
+    JSONSimpleTypes,
+    Mapping[str, JSONSimpleTypes],
+    Sequence[JSONSimpleTypes],
+]
+
+
+class JSONRPCRequestObject(TypedDict):
+    jsonrpc: Literal["2.0"]
+    method: str
+    params: NotRequired[list[JSONTypes] | dict[str, JSONTypes]]
+    id: NotRequired[str | int | None]
+
+
+class JSONRPCErrorObject(TypedDict):
+    code: int
+    message: str
+    data: NotRequired[JSONTypes]
+
+
+class JSONRPCResponseObject(TypedDict):
+    jsonrpc: Literal["2.0"]
+    result: NotRequired[JSONTypes]
+    error: NotRequired[JSONRPCErrorObject]
+    id: str | int | None
+
+
+JSONRPCBatchRequestObject: TypeAlias = Sequence[JSONRPCRequestObject]
+JSONRPCRequest: TypeAlias = Union[
+    JSONRPCRequestObject,
+    JSONRPCBatchRequestObject,
+]
+JSONRPCBatchResponseObject: TypeAlias = Sequence[JSONRPCResponseObject]
+JSONRPCResponse: TypeAlias = Union[
+    JSONRPCResponseObject,
+    JSONRPCBatchResponseObject,
+]
+
+
+"""
+Schema types
+"""
+
+json_schema_type_mapping = {
+    None: "null",
+    type(None): "null",
+    "None": "null",
+    "NoneType": "null",
+    bool: "boolean",
+    "bool": "boolean",
+    int: "integer",  # number?
+    "int": "integer",
+    float: "number",
+    "float": "number",
+    str: "string",
+    "str": "string",
+    list: "array",
+    "list": "array",
+    dict: "object",
+    "dict": "object",
+}
+
+
+def get_json_schema_type(t: type | str) -> str:
+    result = json_schema_type_mapping.get(t)
+    if result is None:
+        result = str(t)
+    return result
+    # if isinstance(t, type):
+    #     result = json_schema_type_mapping.get(t)
+    #     if result is None:
+    #         result = str(t)
+    #     return result
+
+
+_JSONSchema = TypedDict(
+    "_JSONSchema",
+    {
+        "$id": NotRequired[str],
+        "$ref": NotRequired[str],
+        "$dynamicRef": NotRequired[str],
+        "$dynamicAnchor": NotRequired[str],
+        "$schema": NotRequired[str],
+    },
+)
+
+
+class JSONSchema(_JSONSchema):
+    """JSON schema.
+
+    https://datatracker.ietf.org/doc/html/draft-bhutton-json-schema-00
+
+    """
+
+    base: NotRequired[str]
+    type: NotRequired[str | Sequence[str]]
+    description: NotRequired[str]
+    format: NotRequired[str]
+    required: NotRequired[list[str]]
+
+
+Reference = TypedDict(
+    "Reference",
+    {
+        "$ref": str,  # noqa
+        "summary": NotRequired[str],
+        "description": NotRequired[str],
+    },
+)
+
+
+class ParameterSchema(TypedDict):
+    name: NotRequired[str]
+    short_description: NotRequired[str]
+    description: NotRequired[str]
+    type: NotRequired[str]
+    default: NotRequired[Any]
+    required: NotRequired[bool]
+    """Default: False"""
+    deprecated: NotRequired[bool]
+    """Default: False"""
+
+
+class MethodSchema(TypedDict):
+    name: NotRequired[str]
+    short_description: NotRequired[str]
+    description: NotRequired[str]
+    parameters: NotRequired[OrderedDict[str, ParameterSchema]]
+    result: NotRequired[ParameterSchema]
+    notification: NotRequired[bool]
+    deprecated: NotRequired[bool]
+    errors: NotRequired[dict[str, str]]
+    example: NotRequired[Any]
+    examples: NotRequired[Sequence[Any]]
+    # tags: NotRequired[list[ORPCTag | Reference]]
+    # paramStructure: NotRequired[Literal["by-name", "by-position", "either"]]
+    # TODO: **MethodSchema(errors, examples, tags, )
+
+
+"""
+Schema types - OpenRPC
+https://spec.open-rpc.org/
+"""
+
+SUPPORTED_OPENRPC_VERSION = "1.2.1"
+
+
+class OpenRPC(TypedDict):
+    openrpc: Literal["1.2.1"]
+    info: ORPCInfo
+    methods: list[ORPCMethod | Reference]
+    servers: NotRequired[list[ORPCServer]]
+    components: NotRequired[ORPCComponents]
+    externalDocs: NotRequired[ORPCExtDoc]
+
+
+class ORPCInfo(TypedDict):
+    title: str
+    version: str
+    description: NotRequired[str]
+    termsOfService: NotRequired[str]
+    contact: NotRequired[ORPCContact]
+    license: NotRequired[ORPCLicense]
+
+
+class ORPCContact(TypedDict):
+    name: NotRequired[str]
+    url: NotRequired[str]
+    email: NotRequired[str]
+
+
+class ORPCLicense(TypedDict):
+    name: str
+    url: NotRequired[str]
+
+
+class ORPCServer(TypedDict):
+    name: str
+    url: str
+    """Runtime Expression"""
+    summary: NotRequired[str]
+    description: NotRequired[str]
+    variables: NotRequired[Mapping[str, ORPCServerVar]]
+
+
+class ORPCServerVar(TypedDict):
+    default: str
+    enum: NotRequired[list[str]]
+    description: NotRequired[str]
+
+
+class ORPCMethod(TypedDict):
+    name: str
+    params: list[ORPCContentDescriptor | Reference]
+    result: NotRequired[ORPCContentDescriptor | Reference]
+    tags: NotRequired[list[ORPCTag | Reference]]
+    summary: NotRequired[str]
+    description: NotRequired[str]
+    externalDocs: NotRequired[ORPCExtDoc]
+    deprecated: NotRequired[bool]
+    """Default: False"""
+    servers: NotRequired[list[ORPCServer]]
+    errors: NotRequired[list[JSONRPCErrorObject | Reference]]
+    links: NotRequired[list[ORPCLink | Reference]]
+    paramStructure: NotRequired[Literal["by-name", "by-position", "either"]]
+    examples: NotRequired[list[ORPCExamplePairing]]
+
+
+class ORPCContentDescriptor(TypedDict):
+    name: str
+    schema: JSONSchema
+    summary: NotRequired[str]
+    description: NotRequired[str]
+    required: NotRequired[bool]
+    """Default: False"""
+    deprecated: NotRequired[bool]
+    """Default: False"""
+
+
+class ORPCExamplePairing(TypedDict):
+    name: NotRequired[str]
+    summary: NotRequired[str]
+    description: NotRequired[str]
+    params: NotRequired[list[ORPCExample | Reference]]
+    result: NotRequired[ORPCExample | Reference]
+
+
+class ORPCExample(TypedDict):
+    name: NotRequired[str]
+    summary: NotRequired[str]
+    description: NotRequired[str]
+    value: NotRequired[Any]
+    externalValue: NotRequired[str]
+
+
+class ORPCLink(TypedDict):
+    name: str
+    summary: NotRequired[str]
+    description: NotRequired[str]
+    method: NotRequired[str]
+    params: NotRequired[Mapping[str, Any | str]]
+    """Mapping[str, Any | 'Runtime Expression']"""
+    server: NotRequired[ORPCServer]
+
+
+class ORPCComponents(TypedDict):
+    contentDescriptors: NotRequired[Mapping[str, ORPCContentDescriptor]]
+    schemas: NotRequired[Mapping[str, JSONSchema]]
+    examples: NotRequired[Mapping[str, ORPCExample]]
+    links: NotRequired[Mapping[str, ORPCLink]]
+    errors: NotRequired[Mapping[str, JSONRPCErrorObject]]
+    examplePairingObjects: NotRequired[Mapping[str, ORPCExamplePairing]]
+    tags: NotRequired[Mapping[str, ORPCTag]]
+
+
+class ORPCTag(TypedDict):
+    name: str
+    summary: NotRequired[str]
+    description: NotRequired[str]
+    externalDocs: NotRequired[ORPCExtDoc]
+
+
+class ORPCExtDoc(TypedDict):
+    url: str
+    description: NotRequired[str]
+
+
+class ORPC:
+    SUPPORTED_VERSION = SUPPORTED_OPENRPC_VERSION
+    OpenRPC = OpenRPC
+    Info = ORPCInfo
+    Contact = ORPCContact
+    License = ORPCLicense
+    Server = ORPCServer
+    ServerVar = ORPCServerVar
+    Method = ORPCMethod
+    ContentDescriptor = ORPCContentDescriptor
+    Schema = JSONSchema
+    ExamplePairing = ORPCExamplePairing
+    Example = ORPCExample
+    Link = ORPCLink
+    Components = ORPCComponents
+    Tag = ORPCTag
+    ExtDoc = ORPCExtDoc
+    Reference = Reference
+
+    type_mapping = get_json_schema_type
+
+
+"""
+Schema types - OpenAPI
+https://github.com/OAI/OpenAPI-Specification
+"""
+
+SUPPORTED_OPENAPI_VERSION = "3.0.0"
+
+
+class OpenAPI(TypedDict):
+    openapi: Literal["3.1.0"]
+    info: OASInfo
+    jsonSchemaDialect: NotRequired[str]
+    """URI"""
+    servers: NotRequired[list[OASServer]]
+    paths: NotRequired[OASPaths]
+    """OASPaths["/{path}", OASPathItem]"""
+    webhooks: NotRequired[Mapping[str, OASPathItem | Reference]]
+    components: NotRequired[OASComponents]
+    security: NotRequired[list[OASSecurityRequirement]]
+    tags: NotRequired[list[OASTag]]
+    externalDocs: NotRequired[OASExtDoc]
+
+
+class OASInfo(TypedDict):
+    title: str
+    version: str
+    summary: NotRequired[str]
+    description: NotRequired[str]
+    termsOfService: NotRequired[str]
+    contact: NotRequired[OASContact]
+    license: NotRequired[OASLicense]
+
+
+class OASContact(TypedDict):
+    name: NotRequired[str]
+    url: NotRequired[str]
+    email: NotRequired[str]
+
+
+class OASLicense(TypedDict):
+    name: str
+    identifier: NotRequired[str]
+    url: NotRequired[str]
+
+
+class OASServer(TypedDict):
+    url: str
+    description: NotRequired[str]
+    variables: NotRequired[Mapping[str, OASServerVar]]
+
+
+class OASServerVar(TypedDict):
+    default: str
+    enum: NotRequired[list[str]]
+    description: NotRequired[str]
+
+
+class OASComponents(TypedDict):
+    schemas: NotRequired[Mapping[str, OASSchema]]
+    responses: NotRequired[Mapping[str, OASResponse | Reference]]
+    parameters: NotRequired[Mapping[str, OASParameter | Reference]]
+    examples: NotRequired[Mapping[str, OASExample | Reference]]
+    requestBodies: NotRequired[Mapping[str, OASRequestBody | Reference]]
+    headers: NotRequired[Mapping[str, OASHeader | Reference]]
+    securitySchemes: NotRequired[Mapping[str, OASSecurityScheme | Reference]]
+    links: NotRequired[Mapping[str, OASLink | Reference]]
+    callbacks: NotRequired[Mapping[str, OASCallback | Reference]]
+    pathItems: NotRequired[Mapping[str, OASPathItem | Reference]]
+
+
+OASPathItemRef = TypedDict(
+    "OASPathItemRef",
+    {"$ref": NotRequired[str]},
+)
+
+
+class OASPathItem(OASPathItemRef):
+    summary: NotRequired[str]
+    description: NotRequired[str]
+    get: NotRequired[OASOperation]
+    put: NotRequired[OASOperation]
+    post: NotRequired[OASOperation]
+    delete: NotRequired[OASOperation]
+    options: NotRequired[OASOperation]
+    head: NotRequired[OASOperation]
+    patch: NotRequired[OASOperation]
+    trace: NotRequired[OASOperation]
+    servers: NotRequired[OASServer]
+    parameters: NotRequired[OASParameter | Reference]
+
+
+OASPaths = TypedDict("OASPaths", {"/{path}": OASPathItem})
+
+
+class OASOperation(TypedDict):
+    tags: NotRequired[list[str]]
+    summary: NotRequired[str]
+    description: NotRequired[str]
+    externalDocs: NotRequired[OASExtDoc]
+    operationId: NotRequired[str]
+    parameters: NotRequired[Sequence[OASParameter | Reference]]
+    requestBody: NotRequired[OASRequestBody | Reference]
+    responses: NotRequired[OASResponses]
+    callbacks: NotRequired[Mapping[str, OASCallback | Reference]]
+    deprecated: NotRequired[bool]
+    security: NotRequired[Sequence[OASSecurityRequirement]]
+    servers: NotRequired[Sequence[OASServer]]
+
+
+class OASExtDoc(TypedDict):
+    url: str
+    description: NotRequired[str]
+
+
+class OASParameterLocation(StrEnum):
+    PATH = "path"
+    QUERY = "query"
+    HEADER = "header"
+    COOKIE = "cookie"
+
+
+OASParameterIn = TypedDict(
+    "OASParameterIn",
+    {"in": OASParameterLocation},
+)
+
+
+class OASParameter(OASParameterIn):
+    name: str
+    # in: str
+    description: NotRequired[str]
+    required: NotRequired[bool]
+    """required = True if `in` == 'path'"""
+    deprecated: NotRequired[bool]
+    allowEmptyValue: NotRequired[bool]
+    style: NotRequired[str]
+    explode: NotRequired[bool]
+    allowReserved: NotRequired[bool]
+    schema: NotRequired[OASSchema]
+    example: NotRequired[Any]
+    examples: NotRequired[Mapping[str, OASExample | Reference]]
+    content: NotRequired[Mapping[str, OASMediaType]]
+    """A parameter MUST contain either a schema property, or
+    a content property, but not both."""
+
+
+class OASRequestBody(TypedDict):
+    content: Mapping[str, OASMediaType]
+    description: NotRequired[str]
+    required: NotRequired[bool]
+
+
+class OASMediaType(TypedDict):
+    schema: NotRequired[OASSchema]
+    example: NotRequired[Any]
+    examples: NotRequired[Mapping[str, OASExample | Reference]]
+    encoding: NotRequired[Mapping[str, OASEncoding]]
+
+
+class OASEncoding(TypedDict):
+    contentType: NotRequired[str]
+    headers: NotRequired[Mapping[str, OASHeader | Reference]]
+    style: NotRequired[str]
+    explode: NotRequired[bool]
+    allowReserved: NotRequired[bool]
+
+
+class OASResponse(TypedDict):
+    description: str
+    headers: NotRequired[Mapping[str, OASHeader | Reference]]
+    content: NotRequired[Mapping[str, OASMediaType]]
+    links: NotRequired[Mapping[str, OASLink | Reference]]
+
+
+OASResponses = TypedDict(
+    "OASResponses",
+    {
+        "{status_code}": NotRequired[Union[OASResponse, Reference]],
+        "default": NotRequired[Union[OASResponse, Reference]],
+    },
+)
+
+
+OASCallback = Dict[str, Union[OASPathItem, Reference]]
+
+
+class OASExample(TypedDict):
+    summary: NotRequired[str]
+    description: NotRequired[str]
+    value: NotRequired[Any]
+    externalValue: NotRequired[str]
+
+
+class OASLink(TypedDict):
+    operationRef: NotRequired[str]
+    operationId: NotRequired[str]
+    parameters: NotRequired[Mapping[str, Any | str]]
+    """NotRequired[Mapping[str, Any | {expression}]]"""
+    description: NotRequired[str]
+    server: NotRequired[OASServer]
+
+
+class OASHeader(TypedDict):
+    description: NotRequired[str]
+    required: NotRequired[bool]
+    deprecated: NotRequired[bool]
+    allowEmptyValue: NotRequired[bool]
+    style: NotRequired[str]
+    explode: NotRequired[bool]
+    allowReserved: NotRequired[bool]
+    schema: NotRequired[OASSchema]
+    example: NotRequired[Any]
+    examples: NotRequired[Mapping[str, OASExample | Reference]]
+    content: NotRequired[Mapping[str, OASMediaType]]
+    """A parameter MUST contain either a schema property, or
+    a content property, but not both."""
+
+
+class OASTag(TypedDict):
+    name: str
+    description: NotRequired[str]
+    externalDocs: NotRequired[OASExtDoc]
+
+
+class OASSchema(JSONSchema):
+    discriminator: NotRequired[OASDiscriminator]
+    xml: NotRequired[OASXML]
+    externalDocs: NotRequired[OASExtDoc]
+    example: NotRequired[Any]
+
+
+class OASDiscriminator(TypedDict):
+    propertyName: str
+    mapping: NotRequired[Mapping[str, str]]
+
+
+class OASXML(TypedDict):
+    name: NotRequired[str]
+    namespace: NotRequired[str]
+    prefix: NotRequired[str]
+    attribute: NotRequired[bool]
+    wrapped: NotRequired[bool]
+
+
+class OASSecuritySchemeType(StrEnum):
+    API_KEY = "apiKey"
+
+
+class OASSecuritySchemeLocation(StrEnum):
+    QUERY = "query"
+    HEADER = "header"
+    COOKIE = "cookie"
+
+
+OASSecuritySchemeIn = TypedDict(
+    "OASSecuritySchemeIn",
+    {"in": OASSecuritySchemeLocation},
+)
+
+
+class OASSecurityScheme(OASSecuritySchemeIn):
+    type: OASSecuritySchemeType
+    name: str
+    scheme: str
+    flows: OASOAuthFlows
+    openIdConnectUrl: str
+    description: NotRequired[str]
+    bearerFormat: NotRequired[str]
+
+
+class OASOAuthFlows(TypedDict):
+    implicit: NotRequired[OASOAuthFlow]
+    password: NotRequired[OASOAuthFlow]
+    clientCredentials: NotRequired[OASOAuthFlow]
+    authorizationCode: NotRequired[OASOAuthFlow]
+
+
+class OASOAuthFlow(TypedDict):
+    authorizationUrl: str
+    tokenUrl: str
+    scopes: str
+    refreshUrl: NotRequired[str]
+
+
+OASSecurityRequirement = Dict[str, list[str]]
+
+
+class OAPI:
+    SUPPORTED_VERSION = SUPPORTED_OPENAPI_VERSION
+    OpenAPI = OpenAPI
+    Info = OASInfo
+    Contact = OASContact
+    License = OASLicense
+    Server = OASServer
+    ServerVar = OASServerVar
+    Components = OASComponents
+    Paths = OASPaths
+    PathItem = OASPathItem
+    Operation = OASOperation
+    ExtDoc = OASExtDoc
+    ParameterLocation = OASParameterLocation
+    Parameter = OASParameter
+    RequestBody = OASRequestBody
+    MediaType = OASMediaType
+    Encoding = OASEncoding
+    Responses = OASResponses
+    Response = OASResponse
+    Callback = OASCallback
+    Example = OASExample
+    Link = OASLink
+    Header = OASHeader
+    Tag = OASTag
+    Reference = Reference
+    Schema = OASSchema
+    Discriminator = OASDiscriminator
+    XML = OASXML
+    SecurityScheme = OASSecurityScheme
+    OAuthFlows = OASOAuthFlows
+    OAuthFlow = OASOAuthFlow
+    SecurityRequirement = OASSecurityRequirement
+
+    type_mapping = get_json_schema_type
+
+
+"""
+WSGI types definitions
+PEP 3333 – Python Web Server Gateway Interface
+https://peps.python.org/pep-3333/
+"""
+
+WSGIEnvironmentKeys: TypeAlias = Literal[
+    # for CGI
+    # https://datatracker.ietf.org/doc/html/draft-coar-cgi-v11-03
+    "AUTH_TYPE",
+    "CONTENT_LENGTH",
+    "CONTENT_TYPE",
+    "GATEWAY_INTERFACE",
+    "PATH_INFO",
+    "PATH_TRANSLATED",
+    "QUERY_STRING",
+    "REMOTE_ADDR",
+    "REMOTE_HOST",
+    "REMOTE_IDENT",
+    "REMOTE_USER",
+    "REQUEST_METHOD",
+    "SCRIPT_NAME",
+    "SERVER_NAME",
+    "SERVER_PORT",
+    "SERVER_PROTOCOL",
+    "SERVER_SOFTWARE",
+    # for WSGI
+    "wsgi.errors",
+    "wsgi.input",
+    "wsgi.multiprocess",
+    "wsgi.multithread",
+    "wsgi.run_once",
+    "wsgi.url_scheme",
+    "wsgi.version",
+]
+# for framework needs
+WSGIDrakainaKeys: TypeAlias = Literal[
+    "drakaina.app",
+    "drakaina.is_authenticated",
+]
+WSGIEnvironment: TypeAlias = MutableMapping[str, Any]
+WSGIExceptionInfo: TypeAlias = Tuple[Type[BaseException], BaseException, Any]
+
+
+class WSGIStartResponse(Protocol):
+    def __call__(
+        self,
+        status: str,
+        headers: MutableSequence[tuple[str, str]],
+        exc_info: WSGIExceptionInfo | None = ...,
+    ) -> Callable[[bytes], Any]:
+        ...
+
+
+WSGIResponse: TypeAlias = Iterable[bytes]
+WSGIApplication: TypeAlias = Callable[
+    [WSGIEnvironment, WSGIStartResponse],
+    WSGIResponse,
+]
+
+
+class WSGIInputStream(Protocol):
+    def read(self, size: int | None = None) -> bytes:
+        ...
+
+    def readline(self) -> bytes:
+        ...
+
+    def readlines(self, hint: Any | None) -> Iterable[bytes]:
+        ...
+
+    def __iter__(self) -> bytes:
+        ...
+
+
+class WSGIErrorsStream(Protocol):
+    def flush(self) -> None:
+        ...
+
+    def write(self, s: str) -> None:
+        ...
+
+    def writelines(self, seq: Sequence[str]) -> None:
+        ...
+
+
+"""
+ASGI types definitions
+https://asgi.readthedocs.io/en/latest/
+"""
+
+ASGIScope: TypeAlias = MutableMapping[str, Any]
+ASGIMessage: TypeAlias = MutableMapping[str, Any]
+
+ASGIReceive: TypeAlias = Callable[[], Awaitable[ASGIMessage]]
+ASGISend: TypeAlias = Callable[[ASGIMessage], Awaitable[None]]
+
+ASGIApplication: TypeAlias = Callable[
+    [ASGIScope, ASGIReceive, ASGISend],
+    Awaitable[None],
+]
+
+
+"""
+Helpful types
+"""
+
+
+class Comparator(Protocol):
+    def __call__(
+        self,
+        required: Iterable[str],
+        provided: str | Iterable[str],
+    ) -> bool:
+        ...
+
+
+class ProxyRequest(MutableMapping):
+    """A wrapper class for environment mapping.
+
+    :param environment:
+
+    """
+
+    __slots__ = ("__environment",)
+
+    def __init__(self, environment: ASGIScope | WSGIEnvironment):
+        self.__environment = environment
+
+    def __getitem__(self, item):
+        return self.__environment[item]
+
+    def __setitem__(self, key, value):
+        self.__environment[key] = value
+
+    def __delitem__(self, key):
+        del self.__environment[key]
+
+    def __iter__(self):
+        return iter(self.__environment.keys())
+
+    def __contains__(self, item):
+        return item in self.__environment.keys()
+
+    def __len__(self):
+        return len(self.__environment)
+
+    def keys(self):
+        return self.__environment.keys()
+
+    def values(self):
+        return self.__environment.values()
+
+    def items(self):
+        return self.__environment.items()
+
+    def get(self, key, default=None):
+        return self.__environment.get(key, default)
+
+    def clear(self):
+        self.__environment.clear()
+
+    def setdefault(self, key, default=None):
+        self.__environment.setdefault(key, default)
+
+    def pop(self, key, default=None):
+        return self.__environment.pop(key, default)
+
+    def popitem(self):
+        return self.__environment.popitem()
+
+    def copy(self):
+        return self.__class__(self.__environment.copy())
+
+    def update(self, *args, **kwargs):
+        return self.__environment.update(*args, **kwargs)
+
+    def __getattr__(self, item):
+        if item in ("__environment", "_ProxyRequest__environment"):
+            super().__getattribute__(item)
+        return self.__environment[item]
+
+    def __setattr__(self, key, value):
+        if key in ("__environment", "_ProxyRequest__environment"):
+            super().__setattr__(key, value)
+        else:
+            self.__environment[key] = value
+
+    def __delattr__(self, item):
+        del self.__environment[item]
+
+
+AnyRequest: TypeAlias = Union[
+    ASGIScope,
+    WSGIEnvironment,
+    ProxyRequest,
+]
```

### Comparing `drakaina-0.7.0b3/drakaina/utils.py` & `drakaina-0.7.0b4/drakaina/utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-""" Utility functions for package."""
-from __future__ import annotations
-
-import re
-from datetime import datetime
-from datetime import timedelta
-from functools import partial
-from typing import Callable
-from typing import Iterable
-from typing import Literal
-
-
-def iterable_str_arg(s: str | Iterable[str]) -> list[str]:
-    if isinstance(s, str):
-        s = s.replace(",", " ").strip().replace("  ", " ").split()
-    return list(map(str, s))
-
-
-def unwrap_func(func: Callable) -> Callable:
-    _func = func
-    while hasattr(_func, "__wrapped__") or isinstance(_func, partial):
-        _func = getattr(_func, "__wrapped__", None) or _func.func
-    return _func
-
-
-def short_description_by_name(s: str) -> str:
-    if isinstance(s, str):
-        return re.sub(r"[\.-_]", " ", s).capitalize()
-
-
-def get_cookies(cookie_str: str) -> dict[str, str]:
-    if cookie_str is None:
-        return {}
-
-    _cookies = {}
-    for cookie_item in cookie_str.split(";"):
-        if "=" not in cookie_item or "DELETED" in cookie_item:
-            continue
-        name, value = cookie_item.strip().split("=", 1)
-        _cookies[name] = value
-
-    return _cookies
-
-
-def set_cookie(
-    name: str,
-    value: str,
-    expires: datetime | int | str | None = None,
-    max_age: timedelta | int | None = None,
-    domain: str | None = None,
-    path: str | None = None,
-    secure: bool | None = None,
-    http_only: bool | None = None,
-    same_site: Literal["Strict", "Lax", "None"] | None = None,
-    flags: Iterable[str] | None = None,
-) -> tuple[str, str]:
-    """Returns tuple with cookie values prepared for ASGI/WSGI interface.
-
-    RFC6265: https://datatracker.ietf.org/doc/html/rfc6265
-
-    """
-    if "__Secure" in name:
-        secure = True
-    if "__Host" in name:
-        secure = True
-        domain = None
-        path = "/"
-    value = value.replace(";", "")
-    if expires:
-        if isinstance(expires, int):
-            expires = datetime.fromtimestamp(expires)
-        if isinstance(expires, datetime):
-            expires = expires.strftime("%a, %d %b %Y %H:%M:%S %Z")
-        assert isinstance(expires, str)
-        value += f"; Expires={expires}"
-    if max_age:
-        if isinstance(max_age, timedelta):
-            max_age = max_age.days * 24 * 3600 + max_age.seconds
-        assert isinstance(max_age, int) and max_age > 0
-        value += f"; Max-Age={max_age}"
-    if isinstance(domain, str):
-        value += f"; Domain={domain}"
-    if isinstance(path, str):
-        value += f"; Path={path}"
-    if secure:
-        value += "; Secure"
-    if http_only:
-        value += "; HttpOnly"
-    if same_site:
-        assert same_site in ("Strict", "Lax", "None")
-        if same_site == "None":
-            assert secure is True
-        value += f"; SameSite={same_site}"
-    if flags:
-        value += "; " + "; ".join(flags)
-
-    return "Set-Cookie", f"{name}={value}".strip()
-
-
-def mark_cookie_as_deleted(name: str) -> tuple[str, str]:
-    expiry_string = "Thu, 01 Jan 1970 00:00:00 GMT"
-    value = "DELETED"
-    return "Set-Cookie", f"{name}={value}; Expires={expiry_string}"
-
-
-def match_path(item_path: str | re.Pattern[str], path_info: str) -> bool:
-    """Check if the `path_info` (CGI) is equal to the given `item_path`
-    of the element being checked.
-
-    :param item_path: URL or regex pattern to match against the request path.
-    :param path_info: Request path string.
-    """
-
-    if item_path is None:
-        return True
-    if isinstance(item_path, str):
-        return path_info == item_path
-    if isinstance(item_path, re.Pattern):
-        return bool(item_path.match(path_info))
-
-    return False
+""" Utility functions for package."""
+from __future__ import annotations
+
+import re
+from datetime import datetime
+from datetime import timedelta
+from functools import partial
+from typing import Callable
+from typing import Iterable
+from typing import Literal
+
+
+def iterable_str_arg(s: str | Iterable[str]) -> list[str]:
+    if isinstance(s, str):
+        s = s.replace(",", " ").strip().replace("  ", " ").split()
+    return list(map(str, s))
+
+
+def unwrap_func(func: Callable) -> Callable:
+    _func = func
+    while hasattr(_func, "__wrapped__") or isinstance(_func, partial):
+        _func = getattr(_func, "__wrapped__", None) or _func.func
+    return _func
+
+
+def short_description_by_name(s: str) -> str:
+    if isinstance(s, str):
+        return re.sub(r"[\.-_]", " ", s).capitalize()
+
+
+def get_cookies(cookie_str: str) -> dict[str, str]:
+    if cookie_str is None:
+        return {}
+
+    _cookies = {}
+    for cookie_item in cookie_str.split(";"):
+        if "=" not in cookie_item or "DELETED" in cookie_item:
+            continue
+        name, value = cookie_item.strip().split("=", 1)
+        _cookies[name] = value
+
+    return _cookies
+
+
+def set_cookie(
+    name: str,
+    value: str,
+    expires: datetime | int | str | None = None,
+    max_age: timedelta | int | None = None,
+    domain: str | None = None,
+    path: str | None = None,
+    secure: bool | None = None,
+    http_only: bool | None = None,
+    same_site: Literal["Strict", "Lax", "None"] | None = None,
+    flags: Iterable[str] | None = None,
+) -> tuple[str, str]:
+    """Returns tuple with cookie values prepared for ASGI/WSGI interface.
+
+    RFC6265: https://datatracker.ietf.org/doc/html/rfc6265
+
+    """
+    if "__Secure" in name:
+        secure = True
+    if "__Host" in name:
+        secure = True
+        domain = None
+        path = "/"
+    value = value.replace(";", "")
+    if expires:
+        if isinstance(expires, int):
+            expires = datetime.fromtimestamp(expires)
+        if isinstance(expires, datetime):
+            expires = expires.strftime("%a, %d %b %Y %H:%M:%S %Z")
+        assert isinstance(expires, str)
+        value += f"; Expires={expires}"
+    if max_age:
+        if isinstance(max_age, timedelta):
+            max_age = max_age.days * 24 * 3600 + max_age.seconds
+        assert isinstance(max_age, int) and max_age > 0
+        value += f"; Max-Age={max_age}"
+    if isinstance(domain, str):
+        value += f"; Domain={domain}"
+    if isinstance(path, str):
+        value += f"; Path={path}"
+    if secure:
+        value += "; Secure"
+    if http_only:
+        value += "; HttpOnly"
+    if same_site:
+        assert same_site in ("Strict", "Lax", "None")
+        if same_site == "None":
+            assert secure is True
+        value += f"; SameSite={same_site}"
+    if flags:
+        value += "; " + "; ".join(flags)
+
+    return "Set-Cookie", f"{name}={value}".strip()
+
+
+def mark_cookie_as_deleted(name: str) -> tuple[str, str]:
+    expiry_string = "Thu, 01 Jan 1970 00:00:00 GMT"
+    value = "DELETED"
+    return "Set-Cookie", f"{name}={value}; Expires={expiry_string}"
+
+
+def match_path(item_path: str | re.Pattern[str], path_info: str) -> bool:
+    """Check if the `path_info` (CGI) is equal to the given `item_path`
+    of the element being checked.
+
+    :param item_path: URL or regex pattern to match against the request path.
+    :param path_info: Request path string.
+    """
+
+    if item_path is None:
+        return True
+    if isinstance(item_path, str):
+        return path_info == item_path
+    if isinstance(item_path, re.Pattern):
+        return bool(item_path.match(path_info))
+
+    return False
```

### Comparing `drakaina-0.7.0b3/LICENSE` & `drakaina-0.7.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b3/pyproject.toml` & `drakaina-0.7.0b4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-[tool.poetry]
-name = "drakaina"
-version = "0.7.0-beta.3"
-description = "Module for simple RPC service implementation"
-authors = ["Aleksey Terentyev <terentyev.a@pm.me>"]
-license = "Apache License 2.0"
-readme = "README.md"
-classifiers = [
-    "Development Status :: 4 - Beta",
-    "Environment :: Web Environment",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Topic :: System :: Networking",
-    "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
-]
-keywords = ["rpc", "jsonrpc"]
-homepage  = "https://gitlab.com/tau_lex/drakaina"
-repository = "https://gitlab.com/tau_lex/drakaina"
-
-[project.urls]
-"Bug Tracker" = "https://gitlab.com/tau_lex/drakaina/-/issues"
-
-[tool.poetry.dependencies]
-python = "^3.8"
-typing-extensions = "^4.6.2"
-msgpack = { version = "^1.0.5", optional = true }
-orjson = { version = "^3.8.14", optional = true }
-ujson = { version = "^5.7.0", optional = true }
-pyjwt = { version = "^2.7.0", optional = true }
-docstring-parser = { version = "^0.15", optional = true }
-
-[tool.poetry.extras]
-jwt = ["PyJWT"]
-ujson = ["ujson"]
-orjson = ["orjson"]
-msgpack = ["msgpack"]
-docs = ["docstring-parser"]
-tests = ["pytest", "httpx", "ujson", "orjson", "msgpack", "pyjwt", "django", "docstring-parser"]
-
-[tool.poetry.group.dev.dependencies]
-black = {extras = ["d"], version = "^22.12.0"}
-pre-commit = "^3.3.2"
-ruff = "^0.0.269"
-msgpack = "^1.0.4"
-orjson = "^3.8.6"
-pytest = "^7.3.1"
-ujson = "^5.7.0"
-pyjwt = "^2.7.0"
-django = ">=3.2"
-
-[tool.poetry.group.tests.dependencies]
-pytest = "^7.2.1"
-httpx = "^0.23.3"
-
-[tool.pytest.ini_options]
-cache_dir = ".pytest_cache"
-testpaths = "tests"
-
-[tool.ruff]
-# Enable Pyflakes `E` and `F` codes by default.
-select = ["E", "F"]
-ignore = []
-
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F"]
-unfixable = []
-
-exclude = [
-    ".git",
-    ".idea",
-    ".pytest_cache",
-    ".ruff_cache",
-    ".venv",
-    "content",
-    "dist",
-    "venv",
-]
-per-file-ignores = {}
-
-# Same as Black.
-line-length = 80
-
-# Allow unused variables when underscore-prefixed.
-dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
-
-target-version = "py38"
-
-[tool.ruff.mccabe]
-# Unlike Flake8, default to a complexity level of 10.
-max-complexity = 10
-
-[tool.black]
-target-version = ["py38"]
-line-length = 80
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "drakaina"
+version = "0.7.0-beta.4"
+description = "Module for simple RPC service implementation"
+authors = ["Aleksey Terentyev <terentyev.a@pm.me>"]
+license = "Apache License 2.0"
+readme = "README.md"
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Environment :: Web Environment",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: System :: Networking",
+    "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
+]
+keywords = ["rpc", "jsonrpc", "openrpc"]
+homepage  = "https://gitlab.com/tau_lex/drakaina"
+repository = "https://gitlab.com/tau_lex/drakaina"
+
+[project.urls]
+"Bug Tracker" = "https://gitlab.com/tau_lex/drakaina/-/issues"
+
+[tool.poetry.dependencies]
+python = "^3.8"
+typing-extensions = "^4.6.2"
+msgpack = { version = "^1.0.5", optional = true }
+orjson = { version = "^3.8.14", optional = true }
+ujson = { version = "^5.7.0", optional = true }
+pyjwt = { version = "^2.7.0", optional = true }
+docstring-parser = { version = "^0.15", optional = true }
+
+[tool.poetry.extras]
+jwt = ["PyJWT"]
+ujson = ["ujson"]
+orjson = ["orjson"]
+msgpack = ["msgpack"]
+docs = ["docstring-parser"]
+tests = ["pytest", "httpx", "ujson", "orjson", "msgpack", "pyjwt", "django", "docstring-parser"]
+
+[tool.poetry.group.dev.dependencies]
+black = {extras = ["d"], version = "^22.12.0"}
+pre-commit = "^3.3.2"
+ruff = "^0.0.269"
+msgpack = "^1.0.4"
+orjson = "^3.8.6"
+pytest = "^7.3.1"
+ujson = "^5.7.0"
+pyjwt = "^2.7.0"
+django = ">=3.2"
+
+[tool.poetry.group.tests.dependencies]
+pytest = "^7.2.1"
+httpx = "^0.23.3"
+
+[tool.pytest.ini_options]
+cache_dir = ".pytest_cache"
+testpaths = "tests"
+
+[tool.ruff]
+# Enable Pyflakes `E` and `F` codes by default.
+select = ["E", "F"]
+ignore = []
+
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = ["A", "B", "C", "D", "E", "F"]
+unfixable = []
+
+exclude = [
+    ".git",
+    ".idea",
+    ".pytest_cache",
+    ".ruff_cache",
+    ".venv",
+    "content",
+    "dist",
+    "venv",
+]
+per-file-ignores = {}
+
+# Same as Black.
+line-length = 80
+
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+target-version = "py38"
+
+[tool.ruff.mccabe]
+# Unlike Flake8, default to a complexity level of 10.
+max-complexity = 10
+
+[tool.black]
+target-version = ["py38"]
+line-length = 80
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `drakaina-0.7.0b3/README.md` & `drakaina-0.7.0b4/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,216 +1,216 @@
-# drakaina
-
-![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}
-
-[![image](https://img.shields.io/pypi/v/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
-[![image](https://img.shields.io/pypi/l/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
-[![image](https://img.shields.io/pypi/pyversions/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
-[![libera manifesto](https://img.shields.io/badge/libera-manifesto-lightgrey.svg)](https://liberamanifesto.com)
-
-❗ WIP ❗
-
-Framework for simple RPC service implementation.
-
-
-## Quickstart
-
-Drakaina may be installed via `pip` and requires Python 3.7 or higher :
-
-```shell
-pip install drakaina
-```
-
-A minimal Drakaina example is:
-
-```python
-from drakaina import remote_procedure
-from drakaina.wsgi import WSGIHandler
-
-@remote_procedure("hello")
-def hello_method(name):
-    return f"Hello, {name}!"
-
-"""
->>> from drakaina.rpc_protocols import JsonRPCv2
->>> JsonRPCv2().handle({"jsonrpc": "2.0", "method": "hello", "params": ["🐍 Python"] "id": 1})
-{"jsonrpc": "2.0", "result": "Hello, 🐍 Python!", "id": 1}
-"""
-
-# Or define WSGI application
-app = WSGIHandler(route="/jrpc")
-
-```
-
-
-## Features
-
-- Serializers layer.
-  - `json`, `orjson`, `ujson` and `msgpack` serializers.
-- Generates schemas for documentation in OpenRPC format.
-- WSGI protocol implementation
-  - CORS middleware
-  - JWT Authorization middleware.
-  - Compatible with middlewares for others wsgi-frameworks,
-    like as [Werkzeug](https://palletsprojects.com/p/werkzeug/),
-    [Flask](https://palletsprojects.com/p/flask/)
-- `login_required` and `check_permissions` decorators.
-
-
-# Documentation
-
-
-## Installation
-
-```shell
-pip install drakaina
-```
-
-
-## Middlewares
-
-
-### CORS
-
-
-### JWT
-
-Drakaina may be installed via `pip` and requires Python 3.7 or higher :
-
-```shell
-pip install drakaina[jwt]
-```
-
-Example of using Drakaina:
-
-```python
-from functools import partial
-from drakaina import check_permissions
-from drakaina import ENV_IS_AUTHENTICATED
-from drakaina import ENV_USER_ID
-from drakaina import login_required
-from drakaina import match_any
-from drakaina import remote_procedure
-from drakaina.contrib.jwt.middleware import JWTAuthenticationMiddleware
-from drakaina.wsgi import WSGIHandler
-
-import user_store
-
-
-@login_required
-@remote_procedure(provide_request=True)
-def my_method(request):
-    assert request[ENV_IS_AUTHENTICATED]
-    return f"Hello Bro ✋! Your ID={request[ENV_USER_ID]}"
-
-
-@check_permissions(["user_read", "user:admin", "username:johndoe"], match_any)
-@remote_procedure
-def my_method():
-    return "Hello Bro! ✋️"
-
-
-def get_user(request, payload):
-    user_id = request[ENV_USER_ID] or payload["user_id"]
-    return user_store.get(id=user_id)
-
-
-def get_jwt_scopes(request, payload):
-    # here `scp` is the key for the scopes value in the token payload
-    return payload.get("scp")
-
-
-app = WSGIHandler(
-    middlewares=[
-        partial(
-            JWTAuthenticationMiddleware,
-            secret_phrase="_secret_",
-            credentials_required=True,
-            auth_scheme="Bearer",
-            # token_getter=custom_implementation_get_token,
-            user_getter=get_user,
-            scopes_getter=get_jwt_scopes,
-            # revoke_checker=is_revoked,
-        )
-    ]
-)
-```
-
-Drakaina may be ran with any WSGI-compliant server,
-such as [Gunicorn](http://gunicorn.org).
-
-```shell
-gunicorn main:app
-```
-
-or ran with any ASGI-compliant server
-
-```shell
-uvicorn main:app2
-```
-
-
-### Using with Django
-
-Create file `rpc_views.py` in your django application.
-Define function and wrap it `remote_procedure` decorator:
-
-```python
-from drakaina import remote_procedure
-
-@remote_procedure
-def my_method():
-    return "Hello, Django Bro! ✋"
-```
-
-Add `RPCView` class to urlpatterns. The `as_view` method
-must accept the `autodiscover` argument as the name of
-the remote procedure files.
-
-```python
-from django.urls import path
-from drakaina.contrib.django.views import RPCView
-
-urlpatterns = [
-    ...,
-    path("api/", RPCView.as_view(autodiscover="rpc_views")),
-]
-```
-
-
-### JWT Authentication in your Django project
-
-Wrap an instance of `RPCView` with the `JWTAuthenticationMiddleware`.
-
-```python
-from django.urls import path
-from drakaina.contrib.django import RPCView, JWTAuthenticationMiddleware
-
-urlpatterns = [
-    ...,
-    path("api/", JWTAuthenticationMiddleware(
-        RPCView.as_view(autodiscover="rpc_views")
-    )),
-]
-```
-
-Define the parameters in the `settings.py` file.
-
-```python
-...
-
-DRAKAINA_JWT_SECRET_KEY = "__SECRET_KEY__"
-
-...
-```
-
-
-## License
-
-Apache License 2.0
-
-## Artwork
-
-"[drakaina.png](content/drakaina.png)" by Korolko Anastasia is licensed under
-<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="License Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a> ([CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)).
+# drakaina
+
+![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}
+
+[![image](https://img.shields.io/pypi/v/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
+[![image](https://img.shields.io/pypi/l/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
+[![image](https://img.shields.io/pypi/pyversions/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
+[![libera manifesto](https://img.shields.io/badge/libera-manifesto-lightgrey.svg)](https://liberamanifesto.com)
+
+❗ WIP ❗
+
+Framework for simple RPC service implementation.
+
+
+## Quickstart
+
+Drakaina may be installed via `pip` and requires Python 3.7 or higher :
+
+```shell
+pip install drakaina
+```
+
+A minimal Drakaina example is:
+
+```python
+from drakaina import remote_procedure
+from drakaina.wsgi import WSGIHandler
+
+@remote_procedure("hello")
+def hello_method(name):
+    return f"Hello, {name}!"
+
+"""
+>>> from drakaina.rpc_protocols import JsonRPCv2
+>>> JsonRPCv2().handle({"jsonrpc": "2.0", "method": "hello", "params": ["🐍 Python"] "id": 1})
+{"jsonrpc": "2.0", "result": "Hello, 🐍 Python!", "id": 1}
+"""
+
+# Or define WSGI application
+app = WSGIHandler(route="/jrpc")
+
+```
+
+
+## Features
+
+- Serializers layer.
+  - `json`, `orjson`, `ujson` and `msgpack` serializers.
+- Generates schemas for documentation in OpenRPC format.
+- WSGI protocol implementation
+  - CORS middleware
+  - JWT Authorization middleware.
+  - Compatible with middlewares for others wsgi-frameworks,
+    like as [Werkzeug](https://palletsprojects.com/p/werkzeug/),
+    [Flask](https://palletsprojects.com/p/flask/)
+- `login_required` and `check_permissions` decorators.
+
+
+# Documentation
+
+
+## Installation
+
+```shell
+pip install drakaina
+```
+
+
+## Middlewares
+
+
+### CORS
+
+
+### JWT
+
+Drakaina may be installed via `pip` and requires Python 3.7 or higher :
+
+```shell
+pip install drakaina[jwt]
+```
+
+Example of using Drakaina:
+
+```python
+from functools import partial
+from drakaina import check_permissions
+from drakaina import ENV_IS_AUTHENTICATED
+from drakaina import ENV_USER_ID
+from drakaina import login_required
+from drakaina import match_any
+from drakaina import remote_procedure
+from drakaina.contrib.jwt.middleware import JWTAuthenticationMiddleware
+from drakaina.wsgi import WSGIHandler
+
+import user_store
+
+
+@login_required
+@remote_procedure(provide_request=True)
+def my_method(request):
+    assert request[ENV_IS_AUTHENTICATED]
+    return f"Hello Bro ✋! Your ID={request[ENV_USER_ID]}"
+
+
+@check_permissions(["user_read", "user:admin", "username:johndoe"], match_any)
+@remote_procedure
+def my_method():
+    return "Hello Bro! ✋️"
+
+
+def get_user(request, payload):
+    user_id = request[ENV_USER_ID] or payload["user_id"]
+    return user_store.get(id=user_id)
+
+
+def get_jwt_scopes(request, payload):
+    # here `scp` is the key for the scopes value in the token payload
+    return payload.get("scp")
+
+
+app = WSGIHandler(
+    middlewares=[
+        partial(
+            JWTAuthenticationMiddleware,
+            secret_phrase="_secret_",
+            credentials_required=True,
+            auth_scheme="Bearer",
+            # token_getter=custom_implementation_get_token,
+            user_getter=get_user,
+            scopes_getter=get_jwt_scopes,
+            # revoke_checker=is_revoked,
+        )
+    ]
+)
+```
+
+Drakaina may be ran with any WSGI-compliant server,
+such as [Gunicorn](http://gunicorn.org).
+
+```shell
+gunicorn main:app
+```
+
+or ran with any ASGI-compliant server
+
+```shell
+uvicorn main:app2
+```
+
+
+### Using with Django
+
+Create file `rpc_views.py` in your django application.
+Define function and wrap it `remote_procedure` decorator:
+
+```python
+from drakaina import remote_procedure
+
+@remote_procedure
+def my_method():
+    return "Hello, Django Bro! ✋"
+```
+
+Add `RPCView` class to urlpatterns. The `as_view` method
+must accept the `autodiscover` argument as the name of
+the remote procedure files.
+
+```python
+from django.urls import path
+from drakaina.contrib.django.views import RPCView
+
+urlpatterns = [
+    ...,
+    path("api/", RPCView.as_view(autodiscover="rpc_views")),
+]
+```
+
+
+### JWT Authentication in your Django project
+
+Wrap an instance of `RPCView` with the `JWTAuthenticationMiddleware`.
+
+```python
+from django.urls import path
+from drakaina.contrib.django import RPCView, JWTAuthenticationMiddleware
+
+urlpatterns = [
+    ...,
+    path("api/", JWTAuthenticationMiddleware(
+        RPCView.as_view(autodiscover="rpc_views")
+    )),
+]
+```
+
+Define the parameters in the `settings.py` file.
+
+```python
+...
+
+DRAKAINA_JWT_SECRET_KEY = "__SECRET_KEY__"
+
+...
+```
+
+
+## License
+
+Apache License 2.0
+
+## Artwork
+
+"[drakaina.png](content/drakaina.png)" by Korolko Anastasia is licensed under
+<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="License Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a> ([CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)).
```

### Comparing `drakaina-0.7.0b3/setup.py` & `drakaina-0.7.0b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
            'ujson>=5.7.0,<6.0.0',
            'pyjwt>=2.7.0,<3.0.0',
            'docstring-parser>=0.15,<0.16'],
  'ujson': ['ujson>=5.7.0,<6.0.0']}
 
 setup_kwargs = {
     'name': 'drakaina',
-    'version': '0.7.0b3',
+    'version': '0.7.0b4',
     'description': 'Module for simple RPC service implementation',
     'long_description': '# drakaina\n\n![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}\n\n[![image](https://img.shields.io/pypi/v/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![image](https://img.shields.io/pypi/l/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![image](https://img.shields.io/pypi/pyversions/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n[![libera manifesto](https://img.shields.io/badge/libera-manifesto-lightgrey.svg)](https://liberamanifesto.com)\n\n❗ WIP ❗\n\nFramework for simple RPC service implementation.\n\n\n## Quickstart\n\nDrakaina may be installed via `pip` and requires Python 3.7 or higher :\n\n```shell\npip install drakaina\n```\n\nA minimal Drakaina example is:\n\n```python\nfrom drakaina import remote_procedure\nfrom drakaina.wsgi import WSGIHandler\n\n@remote_procedure("hello")\ndef hello_method(name):\n    return f"Hello, {name}!"\n\n"""\n>>> from drakaina.rpc_protocols import JsonRPCv2\n>>> JsonRPCv2().handle({"jsonrpc": "2.0", "method": "hello", "params": ["🐍 Python"] "id": 1})\n{"jsonrpc": "2.0", "result": "Hello, 🐍 Python!", "id": 1}\n"""\n\n# Or define WSGI application\napp = WSGIHandler(route="/jrpc")\n\n```\n\n\n## Features\n\n- Serializers layer.\n  - `json`, `orjson`, `ujson` and `msgpack` serializers.\n- Generates schemas for documentation in OpenRPC format.\n- WSGI protocol implementation\n  - CORS middleware\n  - JWT Authorization middleware.\n  - Compatible with middlewares for others wsgi-frameworks,\n    like as [Werkzeug](https://palletsprojects.com/p/werkzeug/),\n    [Flask](https://palletsprojects.com/p/flask/)\n- `login_required` and `check_permissions` decorators.\n\n\n# Documentation\n\n\n## Installation\n\n```shell\npip install drakaina\n```\n\n\n## Middlewares\n\n\n### CORS\n\n\n### JWT\n\nDrakaina may be installed via `pip` and requires Python 3.7 or higher :\n\n```shell\npip install drakaina[jwt]\n```\n\nExample of using Drakaina:\n\n```python\nfrom functools import partial\nfrom drakaina import check_permissions\nfrom drakaina import ENV_IS_AUTHENTICATED\nfrom drakaina import ENV_USER_ID\nfrom drakaina import login_required\nfrom drakaina import match_any\nfrom drakaina import remote_procedure\nfrom drakaina.contrib.jwt.middleware import JWTAuthenticationMiddleware\nfrom drakaina.wsgi import WSGIHandler\n\nimport user_store\n\n\n@login_required\n@remote_procedure(provide_request=True)\ndef my_method(request):\n    assert request[ENV_IS_AUTHENTICATED]\n    return f"Hello Bro ✋! Your ID={request[ENV_USER_ID]}"\n\n\n@check_permissions(["user_read", "user:admin", "username:johndoe"], match_any)\n@remote_procedure\ndef my_method():\n    return "Hello Bro! ✋️"\n\n\ndef get_user(request, payload):\n    user_id = request[ENV_USER_ID] or payload["user_id"]\n    return user_store.get(id=user_id)\n\n\ndef get_jwt_scopes(request, payload):\n    # here `scp` is the key for the scopes value in the token payload\n    return payload.get("scp")\n\n\napp = WSGIHandler(\n    middlewares=[\n        partial(\n            JWTAuthenticationMiddleware,\n            secret_phrase="_secret_",\n            credentials_required=True,\n            auth_scheme="Bearer",\n            # token_getter=custom_implementation_get_token,\n            user_getter=get_user,\n            scopes_getter=get_jwt_scopes,\n            # revoke_checker=is_revoked,\n        )\n    ]\n)\n```\n\nDrakaina may be ran with any WSGI-compliant server,\nsuch as [Gunicorn](http://gunicorn.org).\n\n```shell\ngunicorn main:app\n```\n\nor ran with any ASGI-compliant server\n\n```shell\nuvicorn main:app2\n```\n\n\n### Using with Django\n\nCreate file `rpc_views.py` in your django application.\nDefine function and wrap it `remote_procedure` decorator:\n\n```python\nfrom drakaina import remote_procedure\n\n@remote_procedure\ndef my_method():\n    return "Hello, Django Bro! ✋"\n```\n\nAdd `RPCView` class to urlpatterns. The `as_view` method\nmust accept the `autodiscover` argument as the name of\nthe remote procedure files.\n\n```python\nfrom django.urls import path\nfrom drakaina.contrib.django.views import RPCView\n\nurlpatterns = [\n    ...,\n    path("api/", RPCView.as_view(autodiscover="rpc_views")),\n]\n```\n\n\n### JWT Authentication in your Django project\n\nWrap an instance of `RPCView` with the `JWTAuthenticationMiddleware`.\n\n```python\nfrom django.urls import path\nfrom drakaina.contrib.django import RPCView, JWTAuthenticationMiddleware\n\nurlpatterns = [\n    ...,\n    path("api/", JWTAuthenticationMiddleware(\n        RPCView.as_view(autodiscover="rpc_views")\n    )),\n]\n```\n\nDefine the parameters in the `settings.py` file.\n\n```python\n...\n\nDRAKAINA_JWT_SECRET_KEY = "__SECRET_KEY__"\n\n...\n```\n\n\n## License\n\nApache License 2.0\n\n## Artwork\n\n"[drakaina.png](content/drakaina.png)" by Korolko Anastasia is licensed under\n<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="License Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a> ([CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)).\n',
     'author': 'Aleksey Terentyev',
     'author_email': 'terentyev.a@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/tau_lex/drakaina',
```

### Comparing `drakaina-0.7.0b3/PKG-INFO` & `drakaina-0.7.0b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: drakaina
-Version: 0.7.0b3
+Version: 0.7.0b4
 Summary: Module for simple RPC service implementation
 Home-page: https://gitlab.com/tau_lex/drakaina
 License: Apache-2.0
-Keywords: rpc,jsonrpc
+Keywords: rpc,jsonrpc,openrpc
 Author: Aleksey Terentyev
 Author-email: terentyev.a@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

