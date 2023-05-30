# Comparing `tmp/tiny_proxy-0.1.1.tar.gz` & `tmp/tiny_proxy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tiny_proxy-0.1.1.tar", last modified: Sun Jul 24 09:08:52 2022, max compression
+gzip compressed data, was "dist/tiny_proxy-0.2.0.tar", last modified: Tue May 30 10:31:23 2023, max compression
```

## Comparing `tiny_proxy-0.1.1.tar` & `tiny_proxy-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2022-07-24 09:08:52.000000 tiny_proxy-0.1.1/
--rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2021-02-13 05:38:25.000000 tiny_proxy-0.1.1/LICENSE.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       47 2021-02-11 14:12:33.000000 tiny_proxy-0.1.1/MANIFEST.in
--rw-rw-r--   0 roman     (1000) roman     (1000)     1575 2022-07-24 09:08:52.000000 tiny_proxy-0.1.1/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)     1176 2022-07-24 08:39:11.000000 tiny_proxy-0.1.1/README.md
--rw-rw-r--   0 roman     (1000) roman     (1000)      225 2022-07-24 06:17:16.000000 tiny_proxy-0.1.1/pyproject.toml
--rw-rw-r--   0 roman     (1000) roman     (1000)       38 2022-07-24 09:08:52.000000 tiny_proxy-0.1.1/setup.cfg
--rw-rw-r--   0 roman     (1000) roman     (1000)     1181 2022-07-24 07:15:32.000000 tiny_proxy-0.1.1/setup.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2022-07-24 09:08:52.000000 tiny_proxy-0.1.1/tiny_proxy/
--rw-rw-r--   0 roman     (1000) roman     (1000)      646 2022-07-24 08:39:31.000000 tiny_proxy-0.1.1/tiny_proxy/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)       38 2022-06-29 04:36:07.000000 tiny_proxy-0.1.1/tiny_proxy/_errors.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2022-07-24 09:08:52.000000 tiny_proxy-0.1.1/tiny_proxy/_handlers/
--rw-rw-r--   0 roman     (1000) roman     (1000)        0 2022-07-10 03:37:09.000000 tiny_proxy-0.1.1/tiny_proxy/_handlers/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1303 2022-07-21 10:18:13.000000 tiny_proxy-0.1.1/tiny_proxy/_handlers/base.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      623 2022-07-10 04:59:52.000000 tiny_proxy-0.1.1/tiny_proxy/_handlers/http.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      474 2022-07-10 04:55:30.000000 tiny_proxy-0.1.1/tiny_proxy/_handlers/socks4.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      631 2022-07-10 04:05:04.000000 tiny_proxy-0.1.1/tiny_proxy/_handlers/socks5.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2022-07-24 09:08:52.000000 tiny_proxy-0.1.1/tiny_proxy/_proxy/
--rw-rw-r--   0 roman     (1000) roman     (1000)        0 2022-07-10 03:36:46.000000 tiny_proxy-0.1.1/tiny_proxy/_proxy/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      149 2022-07-10 03:46:01.000000 tiny_proxy-0.1.1/tiny_proxy/_proxy/abc.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     5489 2022-07-24 08:28:57.000000 tiny_proxy-0.1.1/tiny_proxy/_proxy/http.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     3725 2022-07-12 06:03:44.000000 tiny_proxy-0.1.1/tiny_proxy/_proxy/socks4.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6834 2022-07-13 08:00:49.000000 tiny_proxy-0.1.1/tiny_proxy/_proxy/socks5.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1212 2022-07-10 04:31:14.000000 tiny_proxy-0.1.1/tiny_proxy/_stream.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      913 2022-07-10 04:00:42.000000 tiny_proxy-0.1.1/tiny_proxy/_tunnel.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2022-07-24 09:08:52.000000 tiny_proxy-0.1.1/tiny_proxy.egg-info/
--rw-rw-r--   0 roman     (1000) roman     (1000)     1575 2022-07-24 09:08:52.000000 tiny_proxy-0.1.1/tiny_proxy.egg-info/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)      605 2022-07-24 09:08:52.000000 tiny_proxy-0.1.1/tiny_proxy.egg-info/SOURCES.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        1 2022-07-24 09:08:52.000000 tiny_proxy-0.1.1/tiny_proxy.egg-info/dependency_links.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       20 2022-07-24 09:08:52.000000 tiny_proxy-0.1.1/tiny_proxy.egg-info/requires.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       11 2022-07-24 09:08:52.000000 tiny_proxy-0.1.1/tiny_proxy.egg-info/top_level.txt
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-30 10:31:23.000000 tiny_proxy-0.2.0/
+-rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2021-02-13 05:38:25.000000 tiny_proxy-0.2.0/LICENSE.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       47 2021-02-11 14:12:33.000000 tiny_proxy-0.2.0/MANIFEST.in
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1575 2023-05-30 10:31:23.000000 tiny_proxy-0.2.0/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1176 2022-07-24 08:39:11.000000 tiny_proxy-0.2.0/README.md
+-rw-rw-r--   0 roman     (1000) roman     (1000)      225 2022-07-24 06:17:16.000000 tiny_proxy-0.2.0/pyproject.toml
+-rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-05-30 10:31:23.000000 tiny_proxy-0.2.0/setup.cfg
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1181 2022-07-24 07:15:32.000000 tiny_proxy-0.2.0/setup.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-30 10:31:23.000000 tiny_proxy-0.2.0/tests/
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3427 2022-07-21 10:17:03.000000 tiny_proxy-0.2.0/tests/test_proxy.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-30 10:31:23.000000 tiny_proxy-0.2.0/tiny_proxy/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      646 2023-05-30 10:27:47.000000 tiny_proxy-0.2.0/tiny_proxy/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)       38 2022-06-29 04:36:07.000000 tiny_proxy-0.2.0/tiny_proxy/_errors.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-30 10:31:23.000000 tiny_proxy-0.2.0/tiny_proxy/_handlers/
+-rw-rw-r--   0 roman     (1000) roman     (1000)        0 2022-07-10 03:37:09.000000 tiny_proxy-0.2.0/tiny_proxy/_handlers/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1303 2022-07-21 10:18:13.000000 tiny_proxy-0.2.0/tiny_proxy/_handlers/base.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      623 2022-07-10 04:59:52.000000 tiny_proxy-0.2.0/tiny_proxy/_handlers/http.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      474 2022-07-10 04:55:30.000000 tiny_proxy-0.2.0/tiny_proxy/_handlers/socks4.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      631 2022-07-10 04:05:04.000000 tiny_proxy-0.2.0/tiny_proxy/_handlers/socks5.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-30 10:31:23.000000 tiny_proxy-0.2.0/tiny_proxy/_proxy/
+-rw-rw-r--   0 roman     (1000) roman     (1000)        0 2022-07-10 03:36:46.000000 tiny_proxy-0.2.0/tiny_proxy/_proxy/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      149 2022-07-10 03:46:01.000000 tiny_proxy-0.2.0/tiny_proxy/_proxy/abc.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     5587 2023-02-15 09:59:19.000000 tiny_proxy-0.2.0/tiny_proxy/_proxy/http.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3823 2023-02-15 09:59:05.000000 tiny_proxy-0.2.0/tiny_proxy/_proxy/socks4.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     6932 2023-02-15 09:56:36.000000 tiny_proxy-0.2.0/tiny_proxy/_proxy/socks5.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1397 2022-10-01 12:59:26.000000 tiny_proxy-0.2.0/tiny_proxy/_stream.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      972 2022-10-01 12:16:22.000000 tiny_proxy-0.2.0/tiny_proxy/_tunnel.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-30 10:31:23.000000 tiny_proxy-0.2.0/tiny_proxy.egg-info/
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1575 2023-05-30 10:31:23.000000 tiny_proxy-0.2.0/tiny_proxy.egg-info/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)      625 2023-05-30 10:31:23.000000 tiny_proxy-0.2.0/tiny_proxy.egg-info/SOURCES.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-05-30 10:31:23.000000 tiny_proxy-0.2.0/tiny_proxy.egg-info/dependency_links.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       20 2023-05-30 10:31:23.000000 tiny_proxy-0.2.0/tiny_proxy.egg-info/requires.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       11 2023-05-30 10:31:23.000000 tiny_proxy-0.2.0/tiny_proxy.egg-info/top_level.txt
```

### Comparing `tiny_proxy-0.1.1/LICENSE.txt` & `tiny_proxy-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiny_proxy-0.1.1/PKG-INFO` & `tiny_proxy-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny_proxy
-Version: 0.1.1
+Version: 0.2.0
 Summary: Simple proxy server (SOCKS4(a), SOCKS5(h), HTTP tunnel)
 Home-page: https://github.com/romis2012/tiny-proxy
 Author: Roman Snegirev
 Author-email: snegiryev@gmail.com
 License: Apache 2
 Keywords: socks socks5 socks4 http proxy server asyncio trio anyio
 Platform: UNKNOWN
```

### Comparing `tiny_proxy-0.1.1/README.md` & `tiny_proxy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tiny_proxy-0.1.1/setup.py` & `tiny_proxy-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tiny_proxy-0.1.1/tiny_proxy/__init__.py` & `tiny_proxy-0.2.0/tiny_proxy/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ._proxy.socks4 import Socks4Proxy
 from ._proxy.http import HttpProxy
 
 from ._handlers.http import HttpProxyHandler
 from ._handlers.socks4 import Socks4ProxyHandler
 from ._handlers.socks5 import Socks5ProxyHandler
 
-__version__ = '0.1.1'
+__version__ = '0.2.0'
 
 __all__ = (
     'ProxyError',
     'SocketStream',
     'create_tunnel',
     'AbstractProxy',
     'Socks5Proxy',
```

### Comparing `tiny_proxy-0.1.1/tiny_proxy/_handlers/base.py` & `tiny_proxy-0.2.0/tiny_proxy/_handlers/base.py`

 * *Files identical despite different names*

### Comparing `tiny_proxy-0.1.1/tiny_proxy/_handlers/http.py` & `tiny_proxy-0.2.0/tiny_proxy/_handlers/http.py`

 * *Files identical despite different names*

### Comparing `tiny_proxy-0.1.1/tiny_proxy/_handlers/socks5.py` & `tiny_proxy-0.2.0/tiny_proxy/_handlers/socks5.py`

 * *Files identical despite different names*

### Comparing `tiny_proxy-0.1.1/tiny_proxy/_proxy/http.py` & `tiny_proxy-0.2.0/tiny_proxy/_proxy/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,17 @@
             anyio.ClosedResourceError,
             anyio.BrokenResourceError,
         ) as e:
             raise ConnectionResetError(
                 f'Connection reset by peer {self.stream.getpeername()}'
             ) from e
 
-        self.logger.info('CONNECT {}:{}'.format(remote_host, remote_port))
+        local_addr = self.stream.getsockname()
+        remote_addr = (remote_host, remote_port)
+        self.logger.info('CONNECT {} -> {}'.format(local_addr, remote_addr))
 
         try:
             stream = await anyio.connect_tcp(remote_host=remote_host, remote_port=remote_port)
             remote = SocketStream(stream)
         except OSError as e:
             self.logger.error(e)
             await self.respond(502, 'Bad Gateway', raise_exc=False)
```

### Comparing `tiny_proxy-0.1.1/tiny_proxy/_proxy/socks4.py` & `tiny_proxy-0.2.0/tiny_proxy/_proxy/socks4.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,17 @@
             anyio.ClosedResourceError,
             anyio.BrokenResourceError,
         ) as e:
             raise ConnectionResetError(
                 f'Connection reset by peer {self.stream.getpeername()}'
             ) from e
 
-        self.logger.info('CONNECT {}:{}'.format(remote_host, remote_port))
+        local_addr = self.stream.getsockname()
+        remote_addr = (remote_host, remote_port)
+        self.logger.info('CONNECT {} -> {}'.format(local_addr, remote_addr))
 
         try:
             stream = await anyio.connect_tcp(remote_host=remote_host, remote_port=remote_port)
             remote = SocketStream(stream)
         except OSError as e:
             await self.respond(ReplyCode.CONNECTION_FAILED)
             raise ProxyError(f"Couldn't connect to host {remote_host}:{remote_port}") from e
```

### Comparing `tiny_proxy-0.1.1/tiny_proxy/_proxy/socks5.py` & `tiny_proxy-0.2.0/tiny_proxy/_proxy/socks5.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,17 @@
             anyio.ClosedResourceError,
             anyio.BrokenResourceError,
         ) as e:
             raise ConnectionResetError(
                 f'Connection reset by peer {self.stream.getpeername()}'
             ) from e
 
-        self.logger.info('CONNECT {}:{}'.format(remote_host, remote_port))
+        local_addr = self.stream.getsockname()
+        remote_addr = (remote_host, remote_port)
+        self.logger.info('CONNECT {} -> {}'.format(local_addr, remote_addr))
 
         try:
             # todo: add timeout?
             stream = await anyio.connect_tcp(remote_host=remote_host, remote_port=remote_port)
             remote = SocketStream(stream)
         except OSError as e:
             reply = bytes([SOCKS_VER5, ReplyCode.CONNECTION_REFUSED, NULL, NULL, NULL, NULL])
```

### Comparing `tiny_proxy-0.1.1/tiny_proxy/_stream.py` & `tiny_proxy-0.2.0/tiny_proxy/_stream.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 
     async def receive_until(self, delimiter: bytes, max_bytes: int) -> bytes:
         return await self._buffered.receive_until(delimiter, max_bytes)
 
     async def aclose(self):
         if not self._closing:
             self._closing = True
-            await self._buffered.aclose()
+            try:
+                # underlying TLSStream.aclose() -> TLSStream.unwrap()
+                await self._buffered.aclose()
+            except (anyio.BrokenResourceError, anyio.BusyResourceError):
+                pass
 
     def getpeername(self):
         return self._stream.extra(anyio.abc.SocketAttribute.remote_address, '')
 
     def getsockname(self):
         return self._stream.extra(anyio.abc.SocketAttribute.local_address, '')
```

### Comparing `tiny_proxy-0.1.1/tiny_proxy/_tunnel.py` & `tiny_proxy-0.2.0/tiny_proxy/_tunnel.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,18 @@
                     anyio.ClosedResourceError,
                     anyio.BrokenResourceError,
                 ):
                     break
 
                 try:
                     await writer.send(data)
-                except (anyio.ClosedResourceError, anyio.BrokenResourceError):
+                except (
+                    anyio.ClosedResourceError,
+                    anyio.BrokenResourceError,
+                ):
                     break
         finally:
             await writer.aclose()
 
     async with anyio.create_task_group() as tg:
         tg.start_soon(pipe, endpoint1, endpoint2)
         tg.start_soon(pipe, endpoint2, endpoint1)
```

### Comparing `tiny_proxy-0.1.1/tiny_proxy.egg-info/PKG-INFO` & `tiny_proxy-0.2.0/tiny_proxy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-proxy
-Version: 0.1.1
+Version: 0.2.0
 Summary: Simple proxy server (SOCKS4(a), SOCKS5(h), HTTP tunnel)
 Home-page: https://github.com/romis2012/tiny-proxy
 Author: Roman Snegirev
 Author-email: snegiryev@gmail.com
 License: Apache 2
 Keywords: socks socks5 socks4 http proxy server asyncio trio anyio
 Platform: UNKNOWN
```

### Comparing `tiny_proxy-0.1.1/tiny_proxy.egg-info/SOURCES.txt` & `tiny_proxy-0.2.0/tiny_proxy.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+tests/test_proxy.py
 tiny_proxy/__init__.py
 tiny_proxy/_errors.py
 tiny_proxy/_stream.py
 tiny_proxy/_tunnel.py
 tiny_proxy.egg-info/PKG-INFO
 tiny_proxy.egg-info/SOURCES.txt
 tiny_proxy.egg-info/dependency_links.txt
```

