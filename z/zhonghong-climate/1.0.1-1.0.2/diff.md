# Comparing `tmp/zhonghong_climate-1.0.1.tar.gz` & `tmp/zhonghong_climate-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhonghong_climate-1.0.1.tar", last modified: Wed Jul 13 08:13:11 2022, max compression
+gzip compressed data, was "zhonghong_climate-1.0.2.tar", last modified: Tue May 30 07:35:50 2023, max compression
```

## Comparing `zhonghong_climate-1.0.1.tar` & `zhonghong_climate-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-07-13 08:13:11.770108 zhonghong_climate-1.0.1/
--rw-rw-rw-   0        0        0      773 2022-07-13 08:13:11.770108 zhonghong_climate-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       62 2022-07-13 08:06:16.000000 zhonghong_climate-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2022-07-13 08:13:11.770108 zhonghong_climate-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1051 2022-07-13 08:12:08.000000 zhonghong_climate-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-13 08:13:11.754518 zhonghong_climate-1.0.1/zhonghong_climate/
--rw-rw-rw-   0        0        0        0 2022-07-13 08:06:16.000000 zhonghong_climate-1.0.1/zhonghong_climate/__init__.py
--rw-rw-rw-   0        0        0     3500 2022-07-13 08:06:16.000000 zhonghong_climate-1.0.1/zhonghong_climate/helper.py
--rw-rw-rw-   0        0        0     8166 2022-07-13 08:06:16.000000 zhonghong_climate-1.0.1/zhonghong_climate/hub.py
--rw-rw-rw-   0        0        0     4865 2022-07-13 08:06:16.000000 zhonghong_climate-1.0.1/zhonghong_climate/hvac.py
--rw-rw-rw-   0        0        0     8297 2022-07-13 08:06:16.000000 zhonghong_climate-1.0.1/zhonghong_climate/protocol.py
--rw-rw-rw-   0        0        0       23 2022-07-13 08:06:16.000000 zhonghong_climate-1.0.1/zhonghong_climate/version.py
-drwxrwxrwx   0        0        0        0 2022-07-13 08:13:11.770108 zhonghong_climate-1.0.1/zhonghong_climate.egg-info/
--rw-rw-rw-   0        0        0      773 2022-07-13 08:13:11.000000 zhonghong_climate-1.0.1/zhonghong_climate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2022-07-13 08:13:11.000000 zhonghong_climate-1.0.1/zhonghong_climate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-13 08:13:11.000000 zhonghong_climate-1.0.1/zhonghong_climate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-07-13 08:13:11.000000 zhonghong_climate-1.0.1/zhonghong_climate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-07-13 08:13:11.000000 zhonghong_climate-1.0.1/zhonghong_climate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 07:35:50.603321 zhonghong_climate-1.0.2/
+-rw-rw-rw-   0        0        0      752 2023-05-30 07:35:50.603321 zhonghong_climate-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       62 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 07:35:50.608339 zhonghong_climate-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1051 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:35:50.568614 zhonghong_climate-1.0.2/zhonghong_climate/
+-rw-rw-rw-   0        0        0       31 2023-05-30 07:22:47.000000 zhonghong_climate-1.0.2/zhonghong_climate/__init__.py
+-rw-rw-rw-   0        0        0     3485 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.2/zhonghong_climate/helper.py
+-rw-rw-rw-   0        0        0     8456 2023-05-30 07:24:22.000000 zhonghong_climate-1.0.2/zhonghong_climate/hub.py
+-rw-rw-rw-   0        0        0     4850 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.2/zhonghong_climate/hvac.py
+-rw-rw-rw-   0        0        0     8297 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.2/zhonghong_climate/protocol.py
+-rw-rw-rw-   0        0        0       23 2023-05-30 07:25:48.000000 zhonghong_climate-1.0.2/zhonghong_climate/version.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:35:50.603321 zhonghong_climate-1.0.2/zhonghong_climate.egg-info/
+-rw-rw-rw-   0        0        0      752 2023-05-30 07:35:50.000000 zhonghong_climate-1.0.2/zhonghong_climate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-05-30 07:35:50.000000 zhonghong_climate-1.0.2/zhonghong_climate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 07:35:50.000000 zhonghong_climate-1.0.2/zhonghong_climate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 07:35:50.000000 zhonghong_climate-1.0.2/zhonghong_climate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-30 07:35:50.000000 zhonghong_climate-1.0.2/zhonghong_climate.egg-info/top_level.txt
```

### Comparing `zhonghong_climate-1.0.1/PKG-INFO` & `zhonghong_climate-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: zhonghong_climate
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python library for interfacing with ZhongHong HVAC controller
 Home-page: https://github.com/heculess/zhonghong_hvac
 Author: heculess lau
 Author-email: heculess@hotmail.com
 License: Apache
 Keywords: zhonghong climate hvac
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.5
 
 Python library for interfacing with ZhongHong HVAC controller
-
```

### Comparing `zhonghong_climate-1.0.1/setup.py` & `zhonghong_climate-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `zhonghong_climate-1.0.1/zhonghong_climate/helper.py` & `zhonghong_climate-1.0.2/zhonghong_climate/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import copy
 import logging
-import socket
 import struct
 
 from .protocol import (AcData, AcOnline, AcStatus, ChecksumError, CtlStatus,
                        FuncCode, Header, AcAddr)
 
 logger = logging.getLogger(__name__)
```

### Comparing `zhonghong_climate-1.0.1/zhonghong_climate/hub.py` & `zhonghong_climate-1.0.2/zhonghong_climate/hub.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 
 class ZhongHongGateway:
     def __init__(self, ip_addr: str, port: int, gw_addr: int):
         self.gw_addr = gw_addr
         self.ip_addr = ip_addr
         self.port = port
+        self.available = True
         self.sock = None
         self.ac_callbacks = defaultdict(
             list)  # type DefaultDict[protocol.AcAddr, List[Callable]]
         self.devices = {}
         self._listening = False
         self._threads = []
         self.max_retry = 5
@@ -77,23 +78,25 @@
                 logger.debug("send >> %s", ac_data.hex())
                 self.sock.send(ac_data.encode())
                 self.sock.settimeout(None)
 
             except socket.timeout:
                 logger.error("Connot connect to gateway %s:%s", self.ip_addr,
                              self.port)
+                self.available = False
                 return
 
             except OSError as e:
                 if e.errno == 32:  # Broken pipe
                     logger.error("OSError 32 raise, Broken pipe", exc_info=e)
                 if retry_count < self.max_retry:
                     retry_count += 1
                     self.open_socket()
                     _send(retry_count)
+                self.available = False
 
         _send(0)
 
     def _validate_data(self, data):
         if data is None:
             logger.error('No data in response from hub %s', data)
             return False
@@ -106,38 +109,43 @@
 
         try:
             return self.sock.recv(SOCKET_BUFSIZE)
 
         except ConnectionResetError:
             logger.debug("Connection reset by peer")
             self.open_socket()
+            self.available = False
 
         except socket.timeout as e:
             logger.error("timeout error", exc_info=e)
+            self.available = False
 
         except OSError as e:
             if e.errno == 9:  # when socket close, errorno 9 will raise
                 logger.debug("OSError 9 raise, socket is closed")
 
             else:
                 logger.error("unknown error when recv", exc_info=e)
+            self.available = False
 
         except Exception as e:
             logger.error("unknown error when recv", exc_info=e)
+            self.available = False
 
         return None
 
     def _listen_to_msg(self):
         while self._listening:
             data = self._get_data()
 
             if not data:
                 continue
 
             logger.debug("recv data << %s", protocol.bytes_debug_str(data))
+            self.available = True
 
             for ac_data in helper.get_ac_data(data):
                 logger.debug("get ac_data << %s", ac_data)
 
                 if ac_data.func_code == protocol.FuncCode.STATUS:
                     for payload in ac_data:
                         if not isinstance(payload, protocol.AcStatus):
```

### Comparing `zhonghong_climate-1.0.1/zhonghong_climate/hvac.py` & `zhonghong_climate-1.0.2/zhonghong_climate/hvac.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import enum
 import json
 import logging
-import socket
 from typing import Callable, List
 
 from . import hub, protocol
 
 logger = logging.getLogger(__name__)
```

### Comparing `zhonghong_climate-1.0.1/zhonghong_climate/protocol.py` & `zhonghong_climate-1.0.2/zhonghong_climate/protocol.py`

 * *Files identical despite different names*

### Comparing `zhonghong_climate-1.0.1/zhonghong_climate.egg-info/PKG-INFO` & `zhonghong_climate-1.0.2/zhonghong_climate.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: zhonghong-climate
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python library for interfacing with ZhongHong HVAC controller
 Home-page: https://github.com/heculess/zhonghong_hvac
 Author: heculess lau
 Author-email: heculess@hotmail.com
 License: Apache
 Keywords: zhonghong climate hvac
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.5
 
 Python library for interfacing with ZhongHong HVAC controller
-
```

