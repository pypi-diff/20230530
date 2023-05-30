# Comparing `tmp/loggingx-1.0.0.tar.gz` & `tmp/loggingx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggingx-1.0.0.tar", last modified: Tue May 23 08:20:22 2023, max compression
+gzip compressed data, was "loggingx-1.0.1.tar", last modified: Tue May 30 07:59:48 2023, max compression
```

## Comparing `loggingx-1.0.0.tar` & `loggingx-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 xingweidong   (501) staff       (20)        0 2023-05-23 08:20:22.732349 loggingx-1.0.0/
--rw-r--r--   0 xingweidong   (501) staff       (20)     1068 2023-05-23 02:50:57.000000 loggingx-1.0.0/LICENSE
--rw-r--r--   0 xingweidong   (501) staff       (20)     2389 2023-05-23 08:20:22.732172 loggingx-1.0.0/PKG-INFO
--rw-r--r--   0 xingweidong   (501) staff       (20)     1705 2023-05-23 08:15:45.000000 loggingx-1.0.0/README.md
--rw-r--r--   0 xingweidong   (501) staff       (20)      817 2023-05-23 08:11:13.000000 loggingx-1.0.0/pyproject.toml
--rw-r--r--   0 xingweidong   (501) staff       (20)       38 2023-05-23 08:20:22.732392 loggingx-1.0.0/setup.cfg
-drwxr-xr-x   0 xingweidong   (501) staff       (20)        0 2023-05-23 08:20:22.729883 loggingx-1.0.0/src/
-drwxr-xr-x   0 xingweidong   (501) staff       (20)        0 2023-05-23 08:20:22.730995 loggingx-1.0.0/src/loggingx/
--rw-r--r--   0 xingweidong   (501) staff       (20)        0 2023-05-23 03:05:46.000000 loggingx-1.0.0/src/loggingx/__init__.py
--rw-r--r--   0 xingweidong   (501) staff       (20)     6030 2023-05-23 07:13:03.000000 loggingx-1.0.0/src/loggingx/handlers.py
-drwxr-xr-x   0 xingweidong   (501) staff       (20)        0 2023-05-23 08:20:22.731861 loggingx-1.0.0/src/loggingx.egg-info/
--rw-r--r--   0 xingweidong   (501) staff       (20)     2389 2023-05-23 08:20:22.000000 loggingx-1.0.0/src/loggingx.egg-info/PKG-INFO
--rw-r--r--   0 xingweidong   (501) staff       (20)      261 2023-05-23 08:20:22.000000 loggingx-1.0.0/src/loggingx.egg-info/SOURCES.txt
--rw-r--r--   0 xingweidong   (501) staff       (20)        1 2023-05-23 08:20:22.000000 loggingx-1.0.0/src/loggingx.egg-info/dependency_links.txt
--rw-r--r--   0 xingweidong   (501) staff       (20)       22 2023-05-23 08:20:22.000000 loggingx-1.0.0/src/loggingx.egg-info/requires.txt
--rw-r--r--   0 xingweidong   (501) staff       (20)        9 2023-05-23 08:20:22.000000 loggingx-1.0.0/src/loggingx.egg-info/top_level.txt
+drwxr-xr-x   0 xingweidong   (501) staff       (20)        0 2023-05-30 07:59:48.254975 loggingx-1.0.1/
+-rw-r--r--   0 xingweidong   (501) staff       (20)     1068 2023-05-23 02:50:57.000000 loggingx-1.0.1/LICENSE
+-rw-r--r--   0 xingweidong   (501) staff       (20)     3489 2023-05-30 07:59:48.254848 loggingx-1.0.1/PKG-INFO
+-rw-r--r--   0 xingweidong   (501) staff       (20)     2805 2023-05-30 07:37:24.000000 loggingx-1.0.1/README.md
+-rw-r--r--   0 xingweidong   (501) staff       (20)      817 2023-05-30 07:04:48.000000 loggingx-1.0.1/pyproject.toml
+-rw-r--r--   0 xingweidong   (501) staff       (20)       38 2023-05-30 07:59:48.255023 loggingx-1.0.1/setup.cfg
+drwxr-xr-x   0 xingweidong   (501) staff       (20)        0 2023-05-30 07:59:48.253029 loggingx-1.0.1/src/
+drwxr-xr-x   0 xingweidong   (501) staff       (20)        0 2023-05-30 07:59:48.253829 loggingx-1.0.1/src/loggingx/
+-rw-r--r--   0 xingweidong   (501) staff       (20)        0 2023-05-30 06:33:51.000000 loggingx-1.0.1/src/loggingx/__init__.py
+-rw-r--r--   0 xingweidong   (501) staff       (20)     5861 2023-05-30 06:56:25.000000 loggingx-1.0.1/src/loggingx/handlers.py
+drwxr-xr-x   0 xingweidong   (501) staff       (20)        0 2023-05-30 07:59:48.254658 loggingx-1.0.1/src/loggingx.egg-info/
+-rw-r--r--   0 xingweidong   (501) staff       (20)     3489 2023-05-30 07:59:48.000000 loggingx-1.0.1/src/loggingx.egg-info/PKG-INFO
+-rw-r--r--   0 xingweidong   (501) staff       (20)      261 2023-05-30 07:59:48.000000 loggingx-1.0.1/src/loggingx.egg-info/SOURCES.txt
+-rw-r--r--   0 xingweidong   (501) staff       (20)        1 2023-05-30 07:59:48.000000 loggingx-1.0.1/src/loggingx.egg-info/dependency_links.txt
+-rw-r--r--   0 xingweidong   (501) staff       (20)       22 2023-05-30 07:59:48.000000 loggingx-1.0.1/src/loggingx.egg-info/requires.txt
+-rw-r--r--   0 xingweidong   (501) staff       (20)        9 2023-05-30 07:59:48.000000 loggingx-1.0.1/src/loggingx.egg-info/top_level.txt
```

### Comparing `loggingx-1.0.0/LICENSE` & `loggingx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loggingx-1.0.0/pyproject.toml` & `loggingx-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "loggingx"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="xingweidong", email="614968414@qq.com" },
 ]
 maintainers = [
   { name="xingweidong", email="614968414@qq.com" },
 ]
 description = "logging拓展功能模块"
```

### Comparing `loggingx-1.0.0/src/loggingx/handlers.py` & `loggingx-1.0.1/src/loggingx/handlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import redis
-from typing import Union
-from logging import LogRecord, makeLogRecord
+from logging import makeLogRecord
 from logging.handlers import QueueHandler, QueueListener
 
 
 DEFAULT_REDIS_STREAM_KEY = 'log'  # Redis stream消息队列默认key
 
 
 class RedisStreamHandler(QueueHandler):
     """
     Redis stream处理器，发布logging日志到redis stream消息队列。
     """
 
     def __init__(
         self,
-        redis_url: str,
-        redis_stream_key: str = DEFAULT_REDIS_STREAM_KEY,
+        redis_url,
+        redis_stream_key = DEFAULT_REDIS_STREAM_KEY,
         **redis_kwargs
     ):
         """
         初始化一个实例。
 
         Args:
             redis_url (str): Redis URL，redis的连接字符串。
@@ -29,15 +28,15 @@
 
         self.redis_stream_key = redis_stream_key
 
         r = redis.Redis.from_url(redis_url, **redis_kwargs)
 
         super().__init__(r)
 
-    def enqueue(self, record: LogRecord):
+    def enqueue(self, record):
         """
         Override QueueHandler.enqueue(self, record)方法。
         发布日志消息到redis stream消息队列。
 
         Args:
             record (LogRecord): LogRecord实例。
         """
@@ -49,18 +48,18 @@
 class RedisStreamListener(QueueListener):
     """
     RedisStreamHandler的侦听器，消费redis stream消息队列的日志消息，转发到下游handlers。
     """
 
     def __init__(
         self,
-        redis_url: str,
+        redis_url,
         *handlers,
-        respect_handler_level: bool = False,
-        redis_stream_key: str = DEFAULT_REDIS_STREAM_KEY,
+        respect_handler_level = False,
+        redis_stream_key = DEFAULT_REDIS_STREAM_KEY,
         **redis_kwargs
     ):
         """
         初始化一个实例。
 
         Args:
             redis_url (str): Redis URL，redis的连接字符串。
@@ -81,15 +80,15 @@
 
         r = redis.Redis.from_url(redis_url, **redis_kwargs)
         self.redis_encoding = r.get_encoder().encoding
         self.redis_encoding_errors = r.get_encoder().encoding_errors
 
         super().__init__(r, *handlers, respect_handler_level=respect_handler_level)
 
-    def dequeue(self, block) -> Union[dict[bytes, bytes], None]:
+    def dequeue(self, block):
         """
         Override QueueHandler.dequeue(self, block)方法。
         消费redis stream消息队列的日志消息。
 
         Args:
             block (bool): 是否阻塞。
 
@@ -112,41 +111,41 @@
                 # 判断哨兵消息
                 if msg.get(self.redis_encode(self.stop_sentinel_key)) != self.redis_encode(self.stop_sentinel_value):
                     record = msg
                 # 删除已消费的数据
                 self.queue.xdel(self.redis_stream_key, id)
         return record
 
-    def redis_encode(self, value: str) -> bytes:
+    def redis_encode(self, value):
         """
         使用redis连接实例的编码参数进行编码。
 
         Args:
             value (str): 需要编码的字符串。
 
         Returns:
             bytes: 编码结果。
         """
 
         return value.encode(self.redis_encoding, self.redis_encoding_errors)
 
-    def redis_decode(self, value: bytes) -> str:
+    def redis_decode(self, value):
         """
         使用redis连接实例的编码参数进行解码。
 
         Args:
             value (bytes): 需要解码的bytes字符串。
 
         Returns:
             str: 解码结果。
         """
 
         return value.decode(self.redis_encoding, self.redis_encoding_errors)
 
-    def prepare(self, record: dict[bytes, bytes]) -> LogRecord:
+    def prepare(self, record):
         """
         Override QueueHandler.prepare(self, record)方法。
         准备日志消息，将从redis stream消息队列消费的消息转换成LogRecord实例。
 
         Args:
             record (dict[bytes, bytes]): 从redis stream消息队列消费的消息。
```

