# Comparing `tmp/tcp-over-websocket-1.0.4.tar.gz` & `tmp/tcp-over-websocket-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcp-over-websocket-1.0.4.tar", last modified: Wed Feb 15 05:53:46 2023, max compression
+gzip compressed data, was "tcp-over-websocket-1.0.5.tar", last modified: Tue May 30 02:50:19 2023, max compression
```

## Comparing `tcp-over-websocket-1.0.4.tar` & `tcp-over-websocket-1.0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-02-15 05:53:46.667005 tcp-over-websocket-1.0.4/
--rw-r--r--   0 jchesney   (501) staff       (20)     1057 2022-08-15 06:33:48.000000 tcp-over-websocket-1.0.4/LICENSE
--rw-r--r--   0 jchesney   (501) staff       (20)      383 2023-02-15 05:53:46.666499 tcp-over-websocket-1.0.4/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)     7280 2023-02-14 04:25:50.000000 tcp-over-websocket-1.0.4/README.md
--rw-r--r--   0 jchesney   (501) staff       (20)       38 2023-02-15 05:53:46.667143 tcp-over-websocket-1.0.4/setup.cfg
--rw-r--r--   0 jchesney   (501) staff       (20)     3019 2023-02-15 05:53:46.000000 tcp-over-websocket-1.0.4/setup.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-02-15 05:53:46.652833 tcp-over-websocket-1.0.4/tcp_over_websocket/
--rw-r--r--   0 jchesney   (501) staff       (20)     6148 2023-02-13 12:36:03.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/.DS_Store
--rw-r--r--   0 jchesney   (501) staff       (20)       45 2023-02-15 05:53:46.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-02-15 05:53:46.659888 tcp-over-websocket-1.0.4/tcp_over_websocket/config/
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2023-02-13 10:57:48.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/config/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1423 2023-02-13 13:56:02.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/config/file_config.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1676 2023-02-13 14:04:45.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/config/file_config_abc.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2685 2023-02-14 04:25:50.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/config/file_config_data_exchange.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1844 2023-02-13 14:28:20.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/config/file_config_service.py
--rw-r--r--   0 jchesney   (501) staff       (20)      464 2023-02-13 14:17:07.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/config/file_config_tcp_connect_tunnel.py
--rw-r--r--   0 jchesney   (501) staff       (20)      620 2023-02-13 14:17:07.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/config/file_config_tcp_listen_tunnel.py
--rw-r--r--   0 jchesney   (501) staff       (20)     7876 2023-02-15 05:52:47.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/run_tcp_over_websocket_service.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-02-15 05:53:46.663763 tcp-over-websocket-1.0.4/tcp_over_websocket/tcp_tunnel/
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2023-02-13 12:17:20.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/tcp_tunnel/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)     7451 2023-02-14 01:08:10.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/tcp_tunnel/tcp_tunnel_abc.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2111 2023-02-13 23:33:48.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/tcp_tunnel/tcp_tunnel_connect.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1586 2023-02-13 23:33:37.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/tcp_tunnel/tcp_tunnel_listen.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-02-15 05:53:46.666103 tcp-over-websocket-1.0.4/tcp_over_websocket/util/
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2023-02-13 11:51:55.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/util/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2276 2023-02-14 03:24:51.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/util/log_util.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1324 2023-02-13 12:39:31.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/util/restart_util.py
--rw-r--r--   0 jchesney   (501) staff       (20)       74 2023-02-13 12:37:58.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/util/vortex_util.py
--rw-r--r--   0 jchesney   (501) staff       (20)       60 2023-02-13 12:34:24.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/util/windows_util.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1419 2023-02-13 12:30:00.000000 tcp-over-websocket-1.0.4/tcp_over_websocket/winsvc_tcp_over_websocket_service.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-02-15 05:53:46.656253 tcp-over-websocket-1.0.4/tcp_over_websocket.egg-info/
--rw-r--r--   0 jchesney   (501) staff       (20)      383 2023-02-15 05:53:46.000000 tcp-over-websocket-1.0.4/tcp_over_websocket.egg-info/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)     1221 2023-02-15 05:53:46.000000 tcp-over-websocket-1.0.4/tcp_over_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-02-15 05:53:46.000000 tcp-over-websocket-1.0.4/tcp_over_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 jchesney   (501) staff       (20)      200 2023-02-15 05:53:46.000000 tcp-over-websocket-1.0.4/tcp_over_websocket.egg-info/entry_points.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-02-15 05:53:46.000000 tcp-over-websocket-1.0.4/tcp_over_websocket.egg-info/not-zip-safe
--rw-r--r--   0 jchesney   (501) staff       (20)       75 2023-02-15 05:53:46.000000 tcp-over-websocket-1.0.4/tcp_over_websocket.egg-info/requires.txt
--rw-r--r--   0 jchesney   (501) staff       (20)       19 2023-02-15 05:53:46.000000 tcp-over-websocket-1.0.4/tcp_over_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-30 02:50:19.995063 tcp-over-websocket-1.0.5/
+-rw-r--r--   0 jchesney   (501) staff       (20)     1057 2022-08-15 06:33:48.000000 tcp-over-websocket-1.0.5/LICENSE
+-rw-r--r--   0 jchesney   (501) staff       (20)      383 2023-05-30 02:50:19.994754 tcp-over-websocket-1.0.5/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)     7550 2023-05-30 02:46:36.000000 tcp-over-websocket-1.0.5/README.md
+-rw-r--r--   0 jchesney   (501) staff       (20)       38 2023-05-30 02:50:19.995151 tcp-over-websocket-1.0.5/setup.cfg
+-rw-r--r--   0 jchesney   (501) staff       (20)     3019 2023-05-30 02:50:19.000000 tcp-over-websocket-1.0.5/setup.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-30 02:50:19.986477 tcp-over-websocket-1.0.5/tcp_over_websocket/
+-rw-r--r--   0 jchesney   (501) staff       (20)     6148 2023-02-13 12:36:03.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/.DS_Store
+-rw-r--r--   0 jchesney   (501) staff       (20)       45 2023-05-30 02:50:19.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-30 02:50:19.991136 tcp-over-websocket-1.0.5/tcp_over_websocket/config/
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2023-02-13 10:57:48.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/config/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1423 2023-02-13 13:56:02.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/config/file_config.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1676 2023-02-13 14:04:45.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/config/file_config_abc.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2685 2023-02-14 04:25:50.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/config/file_config_data_exchange.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1844 2023-02-13 14:28:20.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/config/file_config_service.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      464 2023-02-13 14:17:07.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/config/file_config_tcp_connect_tunnel.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      521 2023-05-30 01:36:45.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/config/file_config_tcp_listen_tunnel.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     7876 2023-05-30 01:36:45.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/run_tcp_over_websocket_service.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-30 02:50:19.992490 tcp-over-websocket-1.0.5/tcp_over_websocket/tcp_tunnel/
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2023-02-13 12:17:20.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/tcp_tunnel/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     8123 2023-05-30 02:38:22.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/tcp_tunnel/tcp_tunnel_abc.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2461 2023-05-30 02:11:33.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/tcp_tunnel/tcp_tunnel_connect.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1934 2023-05-30 02:24:04.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/tcp_tunnel/tcp_tunnel_listen.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-30 02:50:19.994372 tcp-over-websocket-1.0.5/tcp_over_websocket/util/
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2023-02-13 11:51:55.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/util/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2250 2023-05-30 01:36:45.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/util/log_util.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1324 2023-02-13 12:39:31.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/util/restart_util.py
+-rw-r--r--   0 jchesney   (501) staff       (20)       74 2023-02-13 12:37:58.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/util/vortex_util.py
+-rw-r--r--   0 jchesney   (501) staff       (20)       60 2023-02-13 12:34:24.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/util/windows_util.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1419 2023-02-13 12:30:00.000000 tcp-over-websocket-1.0.5/tcp_over_websocket/winsvc_tcp_over_websocket_service.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-30 02:50:19.988635 tcp-over-websocket-1.0.5/tcp_over_websocket.egg-info/
+-rw-r--r--   0 jchesney   (501) staff       (20)      383 2023-05-30 02:50:19.000000 tcp-over-websocket-1.0.5/tcp_over_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)     1221 2023-05-30 02:50:19.000000 tcp-over-websocket-1.0.5/tcp_over_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-05-30 02:50:19.000000 tcp-over-websocket-1.0.5/tcp_over_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)      200 2023-05-30 02:50:19.000000 tcp-over-websocket-1.0.5/tcp_over_websocket.egg-info/entry_points.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-05-30 02:50:19.000000 tcp-over-websocket-1.0.5/tcp_over_websocket.egg-info/not-zip-safe
+-rw-r--r--   0 jchesney   (501) staff       (20)       75 2023-05-30 02:50:19.000000 tcp-over-websocket-1.0.5/tcp_over_websocket.egg-info/requires.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)       19 2023-05-30 02:50:19.000000 tcp-over-websocket-1.0.5/tcp_over_websocket.egg-info/top_level.txt
```

### Comparing `tcp-over-websocket-1.0.4/LICENSE` & `tcp-over-websocket-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tcp-over-websocket-1.0.4/README.md` & `tcp-over-websocket-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -80,25 +80,29 @@
         }
     },
     "tcpTunnelConnects": [
         {
             "connectToHost": "search.brave.com",
             "connectToPort": 80,
             "tunnelName": "brave"
+        },
+        {
+            "connectToHost": "127.0.0.1",
+            "connectToPort": 22,
+            "tunnelName": "test_ssh"
         }
     ],
     "tcpTunnelListens": [
         {
             "listenBindAddress": "127.0.0.1",
             "listenPort": 8091,
             "tunnelName": "duckduckgo"
         }],
     "weAreServer": false
 }
-
 ```
 
 ## Example Server Configuration
 
 ```
 {
     "dataExchange": {
@@ -114,26 +118,32 @@
         "logToStdout": true,
         "syslog": {
             "logToSysloyHost": null
         }
     },
     "tcpTunnelConnects": [
         {
-            "connectToHost": "search.brave.com",
+            "connectToHost": "duckduckgo.com",
             "connectToPort": 80,
-            "tunnelName": "brave"
+            "tunnelName": "duckduckgo"
         }
     ],
     "tcpTunnelListens": [
         {
             "listenBindAddress": "127.0.0.1",
-            "listenPort": 8091,
-            "tunnelName": "duckduckgo"
-        }],
-    "weAreServer": false
+            "listenPort": 8092,
+            "tunnelName": "brave"
+        },
+        {
+            "listenBindAddress": "127.0.0.1",
+            "listenPort": 8022,
+            "tunnelName": "test_ssh"
+        }
+    ],
+    "weAreServer": true
 }
 ```
 
 ## Windows Services
 
 To install tcp-over-websocket, open a command prompt as administrator, and run 
 the following command.
```

### Comparing `tcp-over-websocket-1.0.4/setup.py` & `tcp-over-websocket-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "tcp_over_websocket"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "1.0.4"
+package_version = "1.0.5"
 description = "TCP over HTTPS Upgraded Websocket with Mutual TLS"
 
 download_url = (
     "https://codeload.github.com/Synerty/tcp-over-websocket"
     "/zip/refs/heads/master"
 )
 url = "https://github.com/Synerty/tcp-over-websocket"
```

### Comparing `tcp-over-websocket-1.0.4/tcp_over_websocket/.DS_Store` & `tcp-over-websocket-1.0.5/tcp_over_websocket/.DS_Store`

 * *Files identical despite different names*

### Comparing `tcp-over-websocket-1.0.4/tcp_over_websocket/config/file_config.py` & `tcp-over-websocket-1.0.5/tcp_over_websocket/config/file_config.py`

 * *Files identical despite different names*

### Comparing `tcp-over-websocket-1.0.4/tcp_over_websocket/config/file_config_abc.py` & `tcp-over-websocket-1.0.5/tcp_over_websocket/config/file_config_abc.py`

 * *Files identical despite different names*

### Comparing `tcp-over-websocket-1.0.4/tcp_over_websocket/config/file_config_data_exchange.py` & `tcp-over-websocket-1.0.5/tcp_over_websocket/config/file_config_data_exchange.py`

 * *Files identical despite different names*

### Comparing `tcp-over-websocket-1.0.4/tcp_over_websocket/config/file_config_service.py` & `tcp-over-websocket-1.0.5/tcp_over_websocket/config/file_config_service.py`

 * *Files identical despite different names*

### Comparing `tcp-over-websocket-1.0.4/tcp_over_websocket/run_tcp_over_websocket_service.py` & `tcp-over-websocket-1.0.5/tcp_over_websocket/run_tcp_over_websocket_service.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 from txhttputil.site.BasicResource import BasicResource
 from txhttputil.site.SiteUtil import setupSite
 from txhttputil.util.PemUtil import generateDiffieHellmanParameterBytes
 from vortex.DeferUtil import isMainThread
 from vortex.DeferUtil import vortexLogFailure
 from vortex.VortexFactory import VortexFactory
 
+from tcp_over_websocket.config import file_config
 from tcp_over_websocket.tcp_tunnel.tcp_tunnel_connect import TcpTunnelConnect
 from tcp_over_websocket.tcp_tunnel.tcp_tunnel_listen import TcpTunnelListen
 from tcp_over_websocket.util.log_util import setupLogger
 from tcp_over_websocket.util.vortex_util import CLIENT_VORTEX_NAME
 from tcp_over_websocket.util.vortex_util import SERVER_VORTEX_NAME
-from tcp_over_websocket.config import file_config
 
 # Setup the logger to catch the startup.
 setupLogger()
 
 from twisted.internet import reactor, defer
 
 import logging
```

### Comparing `tcp-over-websocket-1.0.4/tcp_over_websocket/tcp_tunnel/tcp_tunnel_abc.py` & `tcp-over-websocket-1.0.5/tcp_over_websocket/tcp_tunnel/tcp_tunnel_abc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import logging
 from abc import ABCMeta
-from abc import abstractmethod
 from collections import deque
 
 from twisted.internet import protocol
 from twisted.internet import reactor
-from twisted.internet.defer import Deferred
 from twisted.internet.defer import inlineCallbacks
 from twisted.internet.protocol import connectionDone
-from twisted.internet.task import deferLater
 from twisted.python.failure import Failure
-from vortex.DeferUtil import vortexLogFailure
 from vortex.PayloadEndpoint import PayloadEndpoint
 from vortex.PayloadEnvelope import PayloadEnvelope
 from vortex.VortexFactory import VortexFactory
 
 
 logger = logging.getLogger(__name__)
 
@@ -41,14 +37,15 @@
         self._sendControlFilt = {FILT_IS_CONTROL_KEY: True}
         self._sendControlFilt.update(self._listenFilt)
 
         self._factory = _ABCFactory(
             self._processFromTcp,
             self._localConnectionMade,
             self._localConnectionLost,
+            self._tunnelName,
         )
         self._tcpServer = None
         self._endpoint = None
 
         self._isLocalConnected = False
         self._dataBuffer: deque[bytes] = deque()
 
@@ -164,18 +161,20 @@
 
 class _ABCProtocol(protocol.Protocol):
     def __init__(
         self,
         dataReceivedCallable,
         connectionMadeCallable,
         connectionLostCallable,
+        tunnelName,
     ):
         self._dataReceivedCallable = dataReceivedCallable
         self._connectionMadeCallable = connectionMadeCallable
         self._connectionLostCallable = connectionLostCallable
+        self._tunnelName = tunnelName
 
     def connectionMade(self):
         try:
             self._connectionMadeCallable()
         except Exception as e:
             logger.exception(e)
 
@@ -193,43 +192,64 @@
 
     def write(self, data: bytes):
         try:
             self.transport.write(data)
         except Exception as e:
             logger.exception(e)
 
+    @inlineCallbacks
     def close(self):
         try:
-            self.transport.loseConnection()
+            logger.debug(f"Closing tcp connect for [{self._tunnelName}]")
+            yield self.transport.loseConnection()
+            logger.debug(f"Closed tcp connect for [{self._tunnelName}]")
         except Exception as e:
             logger.exception(e)
 
 
 class _ABCFactory(protocol.Factory):
     def __init__(
         self,
         dataReceivedCallable,
         connectionMadeCallable,
         connectionLostCallable,
+        tunnelName,
     ):
         self._dataReceivedCallable = dataReceivedCallable
         self._connectionMadeCallable = connectionMadeCallable
         self._connectionLostCallable = connectionLostCallable
+        self._tunnelName = tunnelName
         self._lastProtocol = None
 
     def buildProtocol(self, addr):
-        self.closeLastConnection()
+        if self._lastProtocol:
+            reactor.callLater(0, self._closeProtocol, self._lastProtocol)
         self._lastProtocol = _ABCProtocol(
             self._dataReceivedCallable,
             self._connectionMadeCallable,
             self._connectionLostCallable,
+            self._tunnelName,
         )
         return self._lastProtocol
 
     def write(self, data: bytes):
         assert self._lastProtocol, "We have no last protocol"
         self._lastProtocol.write(data)
 
+    @inlineCallbacks
     def closeLastConnection(self):
         if self._lastProtocol:
-            self._lastProtocol.close()
+            protocol = self._lastProtocol
             self._lastProtocol = None
+            yield self._closeProtocol(protocol)
+
+    @inlineCallbacks
+    def _closeProtocol(self, protocol):
+        logger.debug(
+            f"Disconnecting existing tcp connections"
+            f" for [{self._tunnelName}]"
+        )
+        yield protocol.close()
+        logger.debug(
+            f"Disconnected existing tcp connections"
+            f" for [{self._tunnelName}]"
+        )
```

### Comparing `tcp-over-websocket-1.0.4/tcp_over_websocket/tcp_tunnel/tcp_tunnel_connect.py` & `tcp-over-websocket-1.0.5/tcp_over_websocket/tcp_tunnel/tcp_tunnel_connect.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 
 from twisted.internet import reactor
 from twisted.internet.defer import inlineCallbacks
 from twisted.internet.endpoints import TCP4ClientEndpoint
 from twisted.python.failure import Failure
-from vortex.PayloadEndpoint import PayloadEndpoint
 
 from tcp_over_websocket.config.file_config_tcp_connect_tunnel import (
     FileConfigTcpConnectTunnel,
 )
 from tcp_over_websocket.tcp_tunnel.tcp_tunnel_abc import TcpTunnelABC
 
 logger = logging.getLogger(__name__)
@@ -22,33 +21,43 @@
     ):
         TcpTunnelABC.__init__(self, config.tunnelName, otherVortexName)
         self._config = config
         self._tcpClient = None
 
     def start(self):
         self._start()
+        logger.debug(f"Started tcp connect for [{self._tunnelName}]")
 
+    @inlineCallbacks
     def shutdown(self):
         self._shutdown()
-        self._closeClient()
+        yield self._closeClient()
 
     @inlineCallbacks
     def _remoteConnectionMade(self):
-        TcpTunnelABC._remoteConnectionMade(self)
+        yield TcpTunnelABC._remoteConnectionMade(self)
         yield self._connectClient()
 
+    @inlineCallbacks
     def _remoteConnectionLost(self, cleanly: bool):
-        TcpTunnelABC._remoteConnectionLost(self, cleanly)
-        self._closeClient()
+        yield TcpTunnelABC._remoteConnectionLost(self, cleanly)
+        yield self._closeClient()
 
+    @inlineCallbacks
     def _closeClient(self):
         if self._tcpClient:
-            self._tcpClient.close()
+            logger.debug(f"Stopping tcp connect for [{self._tunnelName}]")
+            yield self._tcpClient.close()
             self._tcpClient = None
 
+        else:
+            logger.debug(f"No tcp connect to stop for [{self._tunnelName}]")
+
+        logger.debug(f"Stopped tcp connect for [{self._tunnelName}]")
+
     @inlineCallbacks
     def _connectClient(self):
         logger.debug(f"Connecting tcp for [{self._tunnelName}]")
 
         # Give it a timeout of 3 seconds, if it can't accept a TCP connection
         # in that time, it's not operationally capable
         endpoint = TCP4ClientEndpoint(
```

### Comparing `tcp-over-websocket-1.0.4/tcp_over_websocket/tcp_tunnel/tcp_tunnel_listen.py` & `tcp-over-websocket-1.0.5/tcp_over_websocket/tcp_tunnel/tcp_tunnel_listen.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,28 +26,38 @@
 
         endpoint = TCP4ServerEndpoint(
             reactor,
             port=self._config.listenPort,
             interface=self._config.listenBindAddress,
         )
 
-        logger.debug(f"Started tcp listen for [{self._tunnelName}]")
         self._tcpServer = yield endpoint.listen(self._factory)
+        logger.debug(f"Started tcp listen for [{self._tunnelName}]")
 
+    @inlineCallbacks
     def shutdown(self):
         self._shutdown()
 
         if self._tcpServer:
-            self._tcpServer.stopListening()
+            logger.debug(f"Stopping tcp listen for [{self._tunnelName}]")
+            yield self._tcpServer.stopListening()
             self._tcpServer = None
 
+            # Close existing connections
+            yield self._factory.closeLastConnection()
+
+        else:
+            logger.debug(f"No tcp listen to stop for [{self._tunnelName}]")
+
         logger.debug(f"Stopped tcp listen for [{self._tunnelName}]")
 
+    @inlineCallbacks
     def _remoteConnectionMade(self):
-        TcpTunnelABC._remoteConnectionMade(self)
+        yield TcpTunnelABC._remoteConnectionMade(self)
         # Do nothing, all is good
 
+    @inlineCallbacks
     def _remoteConnectionLost(self, cleanly: bool):
-        TcpTunnelABC._remoteConnectionLost(self, cleanly)
+        yield TcpTunnelABC._remoteConnectionLost(self, cleanly)
 
         # If the remote end can't connect, then drop the connection
-        self._factory.closeLastConnection()
+        yield self._factory.closeLastConnection()
```

### Comparing `tcp-over-websocket-1.0.4/tcp_over_websocket/util/log_util.py` & `tcp-over-websocket-1.0.5/tcp_over_websocket/util/log_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import gzip
 import logging
 import os
 import sys
 from logging.handlers import SysLogHandler
 from logging.handlers import TimedRotatingFileHandler
 
-from pathlib import Path
-
 LOG_FORMAT = "%(asctime)s %(levelname)s %(name)s:%(message)s"
 DATE_FORMAT = "%d-%b-%Y %H:%M:%S"
 
 logger = logging.getLogger(__name__)
 
 
 def setupLogger():
```

### Comparing `tcp-over-websocket-1.0.4/tcp_over_websocket/util/restart_util.py` & `tcp-over-websocket-1.0.5/tcp_over_websocket/util/restart_util.py`

 * *Files identical despite different names*

### Comparing `tcp-over-websocket-1.0.4/tcp_over_websocket/winsvc_tcp_over_websocket_service.py` & `tcp-over-websocket-1.0.5/tcp_over_websocket/winsvc_tcp_over_websocket_service.py`

 * *Files identical despite different names*

### Comparing `tcp-over-websocket-1.0.4/tcp_over_websocket.egg-info/SOURCES.txt` & `tcp-over-websocket-1.0.5/tcp_over_websocket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

