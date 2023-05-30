# Comparing `tmp/pdocr-rpc-1.0.1.tar.gz` & `tmp/pdocr-rpc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/uos/github/pdocr-rpc/dist/.tmp-33hxrb6y/pdocr-rpc-1.0.1.tar", last modified: Fri May 26 10:32:41 2023, max compression
+gzip compressed data, was "/home/uos/github/pdocr-rpc/dist/.tmp-vxzn6xlk/pdocr-rpc-1.1.0.tar", last modified: Tue May 30 02:19:53 2023, max compression
```

## Comparing `pdocr-rpc-1.0.1.tar` & `pdocr-rpc-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-26 10:32:41.000000 pdocr-rpc-1.0.1/
--rw-r--r--   0 uos       (1000) uos       (1000)    11357 2023-05-26 08:16:45.000000 pdocr-rpc-1.0.1/LICENSE
--rw-r--r--   0 uos       (1000) uos       (1000)     3608 2023-05-26 10:32:41.000000 pdocr-rpc-1.0.1/PKG-INFO
--rw-r--r--   0 uos       (1000) uos       (1000)     3111 2023-05-26 10:31:47.000000 pdocr-rpc-1.0.1/README.md
-drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-26 10:32:41.000000 pdocr-rpc-1.0.1/pdocr_rpc/
--rw-r--r--   0 uos       (1000) uos       (1000)        0 2023-05-26 09:13:53.000000 pdocr-rpc-1.0.1/pdocr_rpc/__init__.py
--rw-r--r--   0 uos       (1000) uos       (1000)     5752 2023-05-26 10:18:48.000000 pdocr-rpc-1.0.1/pdocr_rpc/ocr.py
--rw-r--r--   0 uos       (1000) uos       (1000)     1423 2023-05-26 10:17:38.000000 pdocr-rpc-1.0.1/pdocr_rpc/ocr_server.py
--rw-r--r--   0 uos       (1000) uos       (1000)      904 2023-05-26 10:18:24.000000 pdocr-rpc-1.0.1/pdocr_rpc/setting.py
-drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-26 10:32:41.000000 pdocr-rpc-1.0.1/pdocr_rpc.egg-info/
--rw-r--r--   0 uos       (1000) uos       (1000)     3608 2023-05-26 10:32:40.000000 pdocr-rpc-1.0.1/pdocr_rpc.egg-info/PKG-INFO
--rw-r--r--   0 uos       (1000) uos       (1000)      248 2023-05-26 10:32:40.000000 pdocr-rpc-1.0.1/pdocr_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 uos       (1000) uos       (1000)        1 2023-05-26 10:32:40.000000 pdocr-rpc-1.0.1/pdocr_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 uos       (1000) uos       (1000)       10 2023-05-26 10:32:40.000000 pdocr-rpc-1.0.1/pdocr_rpc.egg-info/top_level.txt
--rw-r--r--   0 uos       (1000) uos       (1000)      482 2023-05-26 10:32:09.000000 pdocr-rpc-1.0.1/pyproject.toml
--rw-r--r--   0 uos       (1000) uos       (1000)       38 2023-05-26 10:32:41.000000 pdocr-rpc-1.0.1/setup.cfg
+drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/
+-rw-r--r--   0 uos       (1000) uos       (1000)    11357 2023-05-26 08:16:45.000000 pdocr-rpc-1.1.0/LICENSE
+-rw-r--r--   0 uos       (1000) uos       (1000)     3200 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/PKG-INFO
+-rw-r--r--   0 uos       (1000) uos       (1000)     2702 2023-05-30 02:15:13.000000 pdocr-rpc-1.1.0/README.md
+drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/pdocr_rpc/
+-rw-r--r--   0 uos       (1000) uos       (1000)        0 2023-05-26 09:13:53.000000 pdocr-rpc-1.1.0/pdocr_rpc/__init__.py
+-rw-r--r--   0 uos       (1000) uos       (1000)     5752 2023-05-26 10:18:48.000000 pdocr-rpc-1.1.0/pdocr_rpc/ocr.py
+-rw-r--r--   0 uos       (1000) uos       (1000)     1474 2023-05-30 02:02:07.000000 pdocr-rpc-1.1.0/pdocr_rpc/ocr_server.py
+-rw-r--r--   0 uos       (1000) uos       (1000)      904 2023-05-26 10:18:24.000000 pdocr-rpc-1.1.0/pdocr_rpc/setting.py
+drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/pdocr_rpc.egg-info/
+-rw-r--r--   0 uos       (1000) uos       (1000)     3200 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/pdocr_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 uos       (1000) uos       (1000)      265 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/pdocr_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 uos       (1000) uos       (1000)        1 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/pdocr_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 uos       (1000) uos       (1000)       10 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/pdocr_rpc.egg-info/top_level.txt
+-rw-r--r--   0 uos       (1000) uos       (1000)      482 2023-05-30 02:16:10.000000 pdocr-rpc-1.1.0/pyproject.toml
+-rw-r--r--   0 uos       (1000) uos       (1000)       38 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/setup.cfg
+drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/test/
+-rw-r--r--   0 uos       (1000) uos       (1000)      169 2023-05-30 02:02:07.000000 pdocr-rpc-1.1.0/test/test_ocr.py
```

### Comparing `pdocr-rpc-1.0.1/LICENSE` & `pdocr-rpc-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdocr-rpc-1.0.1/pdocr_rpc/ocr.py` & `pdocr-rpc-1.1.0/pdocr_rpc/ocr.py`

 * *Files identical despite different names*

### Comparing `pdocr-rpc-1.0.1/pdocr_rpc/ocr_server.py` & `pdocr-rpc-1.1.0/pdocr_rpc/ocr_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
 """
 :Author: Mikigo
 :Date: 2022/5/25 0:02
 """
-from time import time
-from os.path import join, dirname, abspath, exists
 from os import makedirs
+from os.path import join, dirname, abspath, exists
 from socketserver import ThreadingMixIn
+from time import time
 from typing import TYPE_CHECKING
 from xmlrpc.server import SimpleXMLRPCServer
+
 from pdocr_rpc.setting import setting
 
 if not TYPE_CHECKING:
     from paddleocr import PaddleOCR
 
 
 class ThreadXMLRPCServer(ThreadingMixIn, SimpleXMLRPCServer):
@@ -48,9 +49,10 @@
     return result
 
 
 if __name__ == "__main__":
     server = ThreadXMLRPCServer(("0.0.0.0", setting.PORT), allow_none=True)
     server.register_function(image_put, "image_put")
     server.register_function(paddle_ocr, "paddle_ocr")
-    print("监听客户端请求。。")
+    print("Listen to client requests ...")
+    print(f"Client request: IP:{setting.PORT}")
     server.serve_forever()
```

### Comparing `pdocr-rpc-1.0.1/pdocr_rpc/setting.py` & `pdocr-rpc-1.1.0/pdocr_rpc/setting.py`

 * *Files identical despite different names*

