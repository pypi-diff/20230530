# Comparing `tmp/sockettools-1.0.0.tar.gz` & `tmp/sockettools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockettools-1.0.0.tar", last modified: Mon May 22 18:13:35 2023, max compression
+gzip compressed data, was "sockettools-1.0.1.tar", last modified: Tue May 30 16:41:12 2023, max compression
```

## Comparing `sockettools-1.0.0.tar` & `sockettools-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:13:35.887437 sockettools-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-22 18:13:18.000000 sockettools-1.0.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-22 18:13:35.887437 sockettools-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-22 18:13:18.000000 sockettools-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-22 18:13:18.000000 sockettools-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 18:13:35.887437 sockettools-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:13:35.883437 sockettools-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:13:35.887437 sockettools-1.0.0/src/sockettools/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 18:13:18.000000 sockettools-1.0.0/src/sockettools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-22 18:13:18.000000 sockettools-1.0.0/src/sockettools/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-22 18:13:18.000000 sockettools-1.0.0/src/sockettools/clienthandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-22 18:13:18.000000 sockettools-1.0.0/src/sockettools/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-22 18:13:18.000000 sockettools-1.0.0/src/sockettools/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-22 18:13:18.000000 sockettools-1.0.0/src/sockettools/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-22 18:13:18.000000 sockettools-1.0.0/src/sockettools/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:13:35.887437 sockettools-1.0.0/src/sockettools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-22 18:13:35.000000 sockettools-1.0.0/src/sockettools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-22 18:13:35.000000 sockettools-1.0.0/src/sockettools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:13:35.000000 sockettools-1.0.0/src/sockettools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 18:13:35.000000 sockettools-1.0.0/src/sockettools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:41:12.204817 sockettools-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-30 16:41:00.000000 sockettools-1.0.1/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-30 16:41:12.204817 sockettools-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-30 16:41:00.000000 sockettools-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-30 16:41:00.000000 sockettools-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:41:12.204817 sockettools-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:41:12.204817 sockettools-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:41:12.204817 sockettools-1.0.1/src/sockettools/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-30 16:41:00.000000 sockettools-1.0.1/src/sockettools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-30 16:41:00.000000 sockettools-1.0.1/src/sockettools/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-30 16:41:00.000000 sockettools-1.0.1/src/sockettools/clienthandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-30 16:41:00.000000 sockettools-1.0.1/src/sockettools/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-30 16:41:00.000000 sockettools-1.0.1/src/sockettools/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-30 16:41:00.000000 sockettools-1.0.1/src/sockettools/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-30 16:41:00.000000 sockettools-1.0.1/src/sockettools/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:41:12.204817 sockettools-1.0.1/src/sockettools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-30 16:41:12.000000 sockettools-1.0.1/src/sockettools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-30 16:41:12.000000 sockettools-1.0.1/src/sockettools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:41:12.000000 sockettools-1.0.1/src/sockettools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 16:41:12.000000 sockettools-1.0.1/src/sockettools.egg-info/top_level.txt
```

### Comparing `sockettools-1.0.0/LICENCE.md` & `sockettools-1.0.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `sockettools-1.0.0/PKG-INFO` & `sockettools-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,42 @@
 Metadata-Version: 2.1
 Name: sockettools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wrapper around built-in python sockets library
 Author-email: Highghlow <highghlow@proton.me>
 Project-URL: Homepage, https://github.com/highghlow/SocketTools
 Project-URL: Bug Tracker, https://github.com/highghlow/SocketTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 
 # Socket Server Tools
 Use sockets easily
+## Installation
+To install the latest version run
+Unix/macOS:
+```
+python3 -m pip install sockettools
+```
+Windows:
+```
+py -m pip install sockettools
+```
+To install a specified release run
+Unix/maxOS
+```
+python3 -m pip install sockettools=[version]
+```
+Windows:
+```
+py -m pip install sockettools=[version]
+```
 ## Quickstart
 server.py:
 ```python
 import network
 
 class TransferProtocol(network.Protocol):
     @classmethod
```

### Comparing `sockettools-1.0.0/pyproject.toml` & `sockettools-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "sockettools"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Highghlow", email="highghlow@proton.me" },
 ]
 description = "Wrapper around built-in python sockets library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sockettools-1.0.0/src/sockettools/client.py` & `sockettools-1.0.1/src/sockettools/client.py`

 * *Files identical despite different names*

### Comparing `sockettools-1.0.0/src/sockettools/clienthandler.py` & `sockettools-1.0.1/src/sockettools/clienthandler.py`

 * *Files identical despite different names*

### Comparing `sockettools-1.0.0/src/sockettools/events.py` & `sockettools-1.0.1/src/sockettools/events.py`

 * *Files identical despite different names*

### Comparing `sockettools-1.0.0/src/sockettools/server.py` & `sockettools-1.0.1/src/sockettools/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,19 +36,21 @@
         alf += alf.upper()
         alf += "1234567890"
         p = ""
         for _ in range(length):
             p += _random.choice(alf)
         return p
     
-    def _handle(self, conn, addr, handler):
+    def _handle(self, conn, addr, handler, hid):
         try:
             handler.serve()
         except Exception as e:
             handler.event._fire(_events.EXCEPTION, e)
+            if handler.event.registered.get(_events.EXCEPTION, []) == []:
+                raise
 
     def _serve_forever(self, host, port, stop_event=None):
         '''Internal. Does not perform prerun check'''
         self.socket = _socket.socket()
         self.socket.bind((host, port))
         self.socket.listen()
         self.socket.setblocking(0)
@@ -56,15 +58,15 @@
             try:
                 connection, addr = self.socket.accept()
                 new_handler = self.handler(connection, addr, self)
                 while True:
                     handler_id = self._generate_hid()
                     if handler_id not in self.handlers.keys():
                         break
-                thread = _threading.Thread(target=self._handle, name=handler_id, args=(connection, addr, new_handler))
+                thread = _threading.Thread(target=self._handle, name=handler_id, args=(connection, addr, new_handler, handler_id))
                 self.handlers[handler_id] = _active_handler(new_handler, thread)
                 thread.start()
             except BlockingIOError:
                 pass
             if stop_event is not None and stop_event.isSet():
                 break
```

### Comparing `sockettools-1.0.0/src/sockettools/transport.py` & `sockettools-1.0.1/src/sockettools/transport.py`

 * *Files identical despite different names*

### Comparing `sockettools-1.0.0/src/sockettools.egg-info/PKG-INFO` & `sockettools-1.0.1/src/sockettools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,42 @@
 Metadata-Version: 2.1
 Name: sockettools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wrapper around built-in python sockets library
 Author-email: Highghlow <highghlow@proton.me>
 Project-URL: Homepage, https://github.com/highghlow/SocketTools
 Project-URL: Bug Tracker, https://github.com/highghlow/SocketTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 
 # Socket Server Tools
 Use sockets easily
+## Installation
+To install the latest version run
+Unix/macOS:
+```
+python3 -m pip install sockettools
+```
+Windows:
+```
+py -m pip install sockettools
+```
+To install a specified release run
+Unix/maxOS
+```
+python3 -m pip install sockettools=[version]
+```
+Windows:
+```
+py -m pip install sockettools=[version]
+```
 ## Quickstart
 server.py:
 ```python
 import network
 
 class TransferProtocol(network.Protocol):
     @classmethod
```

