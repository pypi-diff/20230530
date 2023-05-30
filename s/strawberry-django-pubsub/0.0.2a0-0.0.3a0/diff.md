# Comparing `tmp/strawberry_django_pubsub-0.0.2a0.tar.gz` & `tmp/strawberry_django_pubsub-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_pubsub-0.0.2a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "strawberry_django_pubsub-0.0.3a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `strawberry_django_pubsub-0.0.2a0.tar` & `strawberry_django_pubsub-0.0.3a0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090251 strawberry_django_pubsub-0.0.2a0/.flake8
--rw-r--r--   0        0        0     3187 2023-05-22 12:10:46.979031 strawberry_django_pubsub-0.0.2a0/.gitignore
--rw-r--r--   0        0        0      264 2023-05-25 12:49:21.090454 strawberry_django_pubsub-0.0.2a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1058 2023-05-26 06:42:27.160926 strawberry_django_pubsub-0.0.2a0/LICENSE
--rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090542 strawberry_django_pubsub-0.0.2a0/Makefile
--rw-r--r--   0        0        0       29 2023-04-26 10:05:26.787023 strawberry_django_pubsub-0.0.2a0/README.md
--rw-r--r--   0        0        0     1690 2023-05-25 12:50:39.844857 strawberry_django_pubsub-0.0.2a0/pyproject.toml
--rw-r--r--   0        0        0     1959 2023-05-25 12:49:21.090815 strawberry_django_pubsub-0.0.2a0/requirements/compile.py
--rw-r--r--   0        0        0     3938 2023-05-25 12:49:21.090957 strawberry_django_pubsub-0.0.2a0/requirements/py310-django41.txt
--rw-r--r--   0        0        0     3936 2023-05-25 12:49:21.091083 strawberry_django_pubsub-0.0.2a0/requirements/py310-django42.txt
--rw-r--r--   0        0        0     3529 2023-05-25 12:49:21.091198 strawberry_django_pubsub-0.0.2a0/requirements/py311-django41.txt
--rw-r--r--   0        0        0     3527 2023-05-25 12:49:21.091307 strawberry_django_pubsub-0.0.2a0/requirements/py311-django42.txt
--rw-r--r--   0        0        0     3937 2023-05-25 12:49:21.091429 strawberry_django_pubsub-0.0.2a0/requirements/py39-django41.txt
--rw-r--r--   0        0        0     3935 2023-05-25 12:49:21.091548 strawberry_django_pubsub-0.0.2a0/requirements/py39-django42.txt
--rw-r--r--   0        0        0       68 2023-05-25 12:49:21.091644 strawberry_django_pubsub-0.0.2a0/requirements/requirements.in
--rw-r--r--   0        0        0       61 2023-05-26 09:07:05.164020 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/__init__.py
--rw-r--r--   0        0        0     5812 2023-05-26 09:06:21.618698 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/asgi.py
--rw-r--r--   0        0        0      521 2023-05-25 12:49:21.091987 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/context.py
--rw-r--r--   0        0        0     1435 2023-05-25 12:49:21.092317 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/debug.py
--rw-r--r--   0        0        0      484 2023-05-25 12:49:21.092418 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/event.py
--rw-r--r--   0        0        0      700 2023-05-25 12:49:21.092518 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/exceptions.py
--rw-r--r--   0        0        0     1992 2023-05-25 12:49:21.092654 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py
--rw-r--r--   0        0        0     4157 2023-05-25 12:49:21.092782 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/queue.py
--rw-r--r--   0        0        0      264 2023-05-25 12:49:21.092910 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/types.py
--rw-r--r--   0        0        0      507 2023-05-25 12:49:21.093182 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/utils.py
--rw-r--r--   0        0        0      324 2023-05-25 12:49:21.093287 strawberry_django_pubsub-0.0.2a0/tox.ini
--rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 strawberry_django_pubsub-0.0.2a0/PKG-INFO
+-rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090251 strawberry_django_pubsub-0.0.3a0/.flake8
+-rw-r--r--   0        0        0     3187 2023-05-22 12:10:46.979031 strawberry_django_pubsub-0.0.3a0/.gitignore
+-rw-r--r--   0        0        0      264 2023-05-25 12:49:21.090454 strawberry_django_pubsub-0.0.3a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1058 2023-05-26 06:42:27.160926 strawberry_django_pubsub-0.0.3a0/LICENSE
+-rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090542 strawberry_django_pubsub-0.0.3a0/Makefile
+-rw-r--r--   0        0        0       29 2023-04-26 10:05:26.787023 strawberry_django_pubsub-0.0.3a0/README.md
+-rw-r--r--   0        0        0     1690 2023-05-25 12:50:39.844857 strawberry_django_pubsub-0.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0     1959 2023-05-25 12:49:21.090815 strawberry_django_pubsub-0.0.3a0/requirements/compile.py
+-rw-r--r--   0        0        0     3938 2023-05-25 12:49:21.090957 strawberry_django_pubsub-0.0.3a0/requirements/py310-django41.txt
+-rw-r--r--   0        0        0     3936 2023-05-25 12:49:21.091083 strawberry_django_pubsub-0.0.3a0/requirements/py310-django42.txt
+-rw-r--r--   0        0        0     3529 2023-05-25 12:49:21.091198 strawberry_django_pubsub-0.0.3a0/requirements/py311-django41.txt
+-rw-r--r--   0        0        0     3527 2023-05-25 12:49:21.091307 strawberry_django_pubsub-0.0.3a0/requirements/py311-django42.txt
+-rw-r--r--   0        0        0     3937 2023-05-25 12:49:21.091429 strawberry_django_pubsub-0.0.3a0/requirements/py39-django41.txt
+-rw-r--r--   0        0        0     3935 2023-05-25 12:49:21.091548 strawberry_django_pubsub-0.0.3a0/requirements/py39-django42.txt
+-rw-r--r--   0        0        0       68 2023-05-25 12:49:21.091644 strawberry_django_pubsub-0.0.3a0/requirements/requirements.in
+-rw-r--r--   0        0        0       61 2023-05-30 10:33:19.968979 strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/__init__.py
+-rw-r--r--   0        0        0     6498 2023-05-30 10:32:16.257207 strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/asgi.py
+-rw-r--r--   0        0        0      521 2023-05-25 12:49:21.091987 strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/context.py
+-rw-r--r--   0        0        0     1435 2023-05-25 12:49:21.092317 strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/debug.py
+-rw-r--r--   0        0        0      484 2023-05-25 12:49:21.092418 strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/event.py
+-rw-r--r--   0        0        0      841 2023-05-30 10:26:07.846938 strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/exceptions.py
+-rw-r--r--   0        0        0     1993 2023-05-30 09:31:17.846212 strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py
+-rw-r--r--   0        0        0     4157 2023-05-25 12:49:21.092782 strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/queue.py
+-rw-r--r--   0        0        0      264 2023-05-25 12:49:21.092910 strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/types.py
+-rw-r--r--   0        0        0      507 2023-05-25 12:49:21.093182 strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/utils.py
+-rw-r--r--   0        0        0      324 2023-05-25 12:49:21.093287 strawberry_django_pubsub-0.0.3a0/tox.ini
+-rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 strawberry_django_pubsub-0.0.3a0/PKG-INFO
```

### Comparing `strawberry_django_pubsub-0.0.2a0/.gitignore` & `strawberry_django_pubsub-0.0.3a0/.gitignore`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.2a0/LICENSE` & `strawberry_django_pubsub-0.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.2a0/pyproject.toml` & `strawberry_django_pubsub-0.0.3a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.2a0/requirements/compile.py` & `strawberry_django_pubsub-0.0.3a0/requirements/compile.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.2a0/requirements/py310-django41.txt` & `strawberry_django_pubsub-0.0.3a0/requirements/py310-django41.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.2a0/requirements/py310-django42.txt` & `strawberry_django_pubsub-0.0.3a0/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.2a0/requirements/py311-django41.txt` & `strawberry_django_pubsub-0.0.3a0/requirements/py311-django41.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.2a0/requirements/py311-django42.txt` & `strawberry_django_pubsub-0.0.3a0/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.2a0/requirements/py39-django41.txt` & `strawberry_django_pubsub-0.0.3a0/requirements/py39-django41.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.2a0/requirements/py39-django42.txt` & `strawberry_django_pubsub-0.0.3a0/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/asgi.py` & `strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/asgi.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from asgiref.typing import ASGIReceiveCallable, ASGISendCallable, Scope
 from strawberry.schema import BaseSchema
 
 from strawberry_django_pubsub.context import StrawberryDjangoWsContext
 from strawberry_django_pubsub.debug import pretty_print_event
 from strawberry_django_pubsub.exceptions import (
+    StopConsumer,
     WebSocketAcceptConnection,
     WebSocketDenyConnection,
 )
 from strawberry_django_pubsub.handlers.graphql_transport_ws_handler import (
     GraphQLTransportWSHandler,
 )
 from strawberry_django_pubsub.utils import get_handler_name
@@ -54,18 +55,23 @@
         # ensure where mounted on a websocket
         if not self.scope["type"] == WEBSOCKET_TYPE:
             pretty_print_event(
                 "Connection denied", context=self.scope, debug=self.debug
             )
             raise WebSocketDenyConnection()
 
-        # dispatch websocket protocol
-        while True:
-            message = await receive()
-            await self.dispatch(message)
+        try:
+            # dispatch websocket protocol
+            while True:
+                message = await receive()
+                await self.dispatch(message)
+
+        except StopConsumer:
+            # Exit cleanly
+            pass
 
     async def dispatch(self, message):
         """
         Works out what to do with a message.
         """
 
         pretty_print_event("dispatch", context=message, debug=self.debug)
@@ -145,25 +151,44 @@
             await self.receive_json(await self.decode_json(text_data), **kwargs)
         else:
             raise ValueError("No text section for incoming WebSocket frame!")
 
     async def receive_json(self, content, **kwargs):
         await self._handler.handle_message(content)
 
+    async def close(self, code=None):
+        """
+        Closes the WebSocket from the server end
+        """
+        if code is not None and code is not True:
+            await self.send({"type": "websocket.close", "code": code})
+        else:
+            await self.send({"type": "websocket.close"})
+
     async def send_json(self, content, close=False) -> None:
         """
         Encode the given content as JSON and send it to the client.
         """
         pretty_print_event("send_json", context=content, debug=self.debug)
 
         await self.send(
             {"type": "websocket.send", "text": await self.encode_json(content)},
             close=close,
         )
 
+        if close:
+            await self.close(close)
+
+    async def websocket_disconnect(self, message):
+        """
+        Called when a WebSocket connection is closed.
+        """
+        await self.disconnect(message["code"])
+        raise StopConsumer()
+
     async def disconnect(self, code) -> None:
         await self._handler.handle_disconnect(code)
 
     @classmethod
     async def decode_json(cls, text_data):
         return json.loads(text_data)
```

### Comparing `strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/context.py` & `strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/context.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/debug.py` & `strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/debug.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/exceptions.py` & `strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,7 +24,15 @@
     Raised when connection is dropped; this exception should only be called
     explicit in debug mode only.
     """
 
     def __init__(self, code: int = 1000, reason: Optional[str] = None) -> None:
         self.code = code
         self.reason = reason or ""
+
+
+class StopConsumer(Exception):
+    """
+    Raised when a consumer wants to stop and close down its application instance.
+    """
+
+    pass
```

### Comparing `strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py` & `strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
     async def send_json(self, data: dict) -> None:
         await self._ws.send_json(data)
 
     async def close(self, code: int = 1000, reason: Optional[str] = None) -> None:
         # FIXME: We are using `self._ws.base_send` directly instead of `self._ws.close`
         # because the later doesn't accept the `reason` argument.
+
         await self._ws._send(
             {
                 "type": "websocket.close",
                 "code": code,
                 "reason": reason or "",
             }
         )
```

### Comparing `strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/queue.py` & `strawberry_django_pubsub-0.0.3a0/strawberry_django_pubsub/queue.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.2a0/PKG-INFO` & `strawberry_django_pubsub-0.0.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-pubsub
-Version: 0.0.2a0
+Version: 0.0.3a0
 Summary: Strawberry Django PubSub 
 Author-email: DK <dk@terminalkitten.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
```

