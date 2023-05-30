# Comparing `tmp/whochat-1.3.4.tar.gz` & `tmp/whochat-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whochat-1.3.4.tar", last modified: Mon May 29 15:57:29 2023, max compression
+gzip compressed data, was "whochat-1.3.5.tar", last modified: Tue May 30 08:28:15 2023, max compression
```

## Comparing `whochat-1.3.4.tar` & `whochat-1.3.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.773577 whochat-1.3.4/
--rw-r--r--   0 luming     (501) staff       (20)     1514 2023-01-29 06:35:29.000000 whochat-1.3.4/LICENSE
--rw-r--r--   0 luming     (501) staff       (20)       55 2023-01-29 06:35:29.000000 whochat-1.3.4/MANIFEST.in
--rw-r--r--   0 luming     (501) staff       (20)     7644 2023-05-29 15:57:29.773753 whochat-1.3.4/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)     6991 2023-05-29 15:57:17.000000 whochat-1.3.4/README.md
--rw-r--r--   0 luming     (501) staff       (20)     1292 2023-05-29 15:57:29.774164 whochat-1.3.4/setup.cfg
--rw-r--r--   0 luming     (501) staff       (20)       38 2023-03-09 09:22:00.000000 whochat-1.3.4/setup.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.766218 whochat-1.3.4/whochat/
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.768285 whochat-1.3.4/whochat/ComWeChatRobot/
--rw-r--r--   0 luming     (501) staff       (20)   165376 2023-02-13 09:38:48.000000 whochat-1.3.4/whochat/ComWeChatRobot/CWeChatRobot.exe
--rw-r--r--   0 luming     (501) staff       (20)   293888 2023-02-13 09:38:48.000000 whochat-1.3.4/whochat/ComWeChatRobot/DWeChatRobot.dll
--rw-r--r--   0 luming     (501) staff       (20)      472 2023-02-13 09:38:48.000000 whochat-1.3.4/whochat/ComWeChatRobot/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)       65 2023-05-29 15:50:44.000000 whochat-1.3.4/whochat/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)      107 2023-01-29 06:35:29.000000 whochat-1.3.4/whochat/__main__.py
--rw-r--r--   0 luming     (501) staff       (20)      608 2023-02-13 09:38:48.000000 whochat-1.3.4/whochat/_comtypes.py
--rw-r--r--   0 luming     (501) staff       (20)     6413 2023-02-13 09:38:48.000000 whochat-1.3.4/whochat/abc.py
--rw-r--r--   0 luming     (501) staff       (20)    22043 2023-05-26 16:24:36.000000 whochat-1.3.4/whochat/bot.py
--rw-r--r--   0 luming     (501) staff       (20)     4952 2023-05-11 01:43:21.000000 whochat-1.3.4/whochat/cli.py
--rw-r--r--   0 luming     (501) staff       (20)      762 2023-05-11 01:43:21.000000 whochat-1.3.4/whochat/logger.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.771566 whochat-1.3.4/whochat/messages/
--rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.4/whochat/messages/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)      447 2023-03-09 10:27:55.000000 whochat-1.3.4/whochat/messages/constants.py
--rw-r--r--   0 luming     (501) staff       (20)     6875 2023-01-29 06:35:29.000000 whochat-1.3.4/whochat/messages/tcp.py
--rw-r--r--   0 luming     (501) staff       (20)     7210 2023-05-26 16:02:21.000000 whochat-1.3.4/whochat/messages/websocket.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.772353 whochat-1.3.4/whochat/rpc/
--rw-r--r--   0 luming     (501) staff       (20)       22 2023-01-29 06:35:29.000000 whochat-1.3.4/whochat/rpc/__init__.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.772696 whochat-1.3.4/whochat/rpc/clients/
--rw-r--r--   0 luming     (501) staff       (20)        0 2023-03-09 10:27:55.000000 whochat-1.3.4/whochat/rpc/clients/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)     4824 2023-05-29 14:29:26.000000 whochat-1.3.4/whochat/rpc/clients/websocket.py
--rw-r--r--   0 luming     (501) staff       (20)     1823 2023-03-09 10:27:55.000000 whochat-1.3.4/whochat/rpc/docs.py
--rw-r--r--   0 luming     (501) staff       (20)    10159 2023-05-26 15:23:50.000000 whochat-1.3.4/whochat/rpc/handlers.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.773251 whochat-1.3.4/whochat/rpc/servers/
--rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.4/whochat/rpc/servers/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)      930 2023-01-29 06:35:29.000000 whochat-1.3.4/whochat/rpc/servers/http.py
--rw-r--r--   0 luming     (501) staff       (20)     1138 2023-05-26 10:13:13.000000 whochat-1.3.4/whochat/rpc/servers/websocket.py
--rw-r--r--   0 luming     (501) staff       (20)      315 2023-05-11 01:43:21.000000 whochat-1.3.4/whochat/settings.py
--rw-r--r--   0 luming     (501) staff       (20)     1108 2023-05-29 10:26:50.000000 whochat-1.3.4/whochat/signals.py
--rw-r--r--   0 luming     (501) staff       (20)     3091 2023-03-09 10:27:55.000000 whochat-1.3.4/whochat/utils.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.767129 whochat-1.3.4/whochat.egg-info/
--rw-r--r--   0 luming     (501) staff       (20)     7644 2023-05-29 15:57:29.000000 whochat-1.3.4/whochat.egg-info/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)      870 2023-05-29 15:57:29.000000 whochat-1.3.4/whochat.egg-info/SOURCES.txt
--rw-r--r--   0 luming     (501) staff       (20)        1 2023-05-29 15:57:29.000000 whochat-1.3.4/whochat.egg-info/dependency_links.txt
--rw-r--r--   0 luming     (501) staff       (20)       50 2023-05-29 15:57:29.000000 whochat-1.3.4/whochat.egg-info/entry_points.txt
--rw-r--r--   0 luming     (501) staff       (20)      115 2023-05-29 15:57:29.000000 whochat-1.3.4/whochat.egg-info/requires.txt
--rw-r--r--   0 luming     (501) staff       (20)        8 2023-05-29 15:57:29.000000 whochat-1.3.4/whochat.egg-info/top_level.txt
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-30 08:28:15.334673 whochat-1.3.5/
+-rw-r--r--   0 luming     (501) staff       (20)     1514 2023-01-29 06:35:29.000000 whochat-1.3.5/LICENSE
+-rw-r--r--   0 luming     (501) staff       (20)       55 2023-01-29 06:35:29.000000 whochat-1.3.5/MANIFEST.in
+-rw-r--r--   0 luming     (501) staff       (20)     7727 2023-05-30 08:28:15.334789 whochat-1.3.5/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)     7074 2023-05-30 08:27:58.000000 whochat-1.3.5/README.md
+-rw-r--r--   0 luming     (501) staff       (20)     1292 2023-05-30 08:28:15.335376 whochat-1.3.5/setup.cfg
+-rw-r--r--   0 luming     (501) staff       (20)       38 2023-03-09 09:22:00.000000 whochat-1.3.5/setup.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-30 08:28:15.319872 whochat-1.3.5/whochat/
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-30 08:28:15.322931 whochat-1.3.5/whochat/ComWeChatRobot/
+-rw-r--r--   0 luming     (501) staff       (20)   165376 2023-02-13 09:38:48.000000 whochat-1.3.5/whochat/ComWeChatRobot/CWeChatRobot.exe
+-rw-r--r--   0 luming     (501) staff       (20)   293888 2023-02-13 09:38:48.000000 whochat-1.3.5/whochat/ComWeChatRobot/DWeChatRobot.dll
+-rw-r--r--   0 luming     (501) staff       (20)      472 2023-02-13 09:38:48.000000 whochat-1.3.5/whochat/ComWeChatRobot/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)       65 2023-05-30 08:26:27.000000 whochat-1.3.5/whochat/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)      107 2023-01-29 06:35:29.000000 whochat-1.3.5/whochat/__main__.py
+-rw-r--r--   0 luming     (501) staff       (20)      608 2023-02-13 09:38:48.000000 whochat-1.3.5/whochat/_comtypes.py
+-rw-r--r--   0 luming     (501) staff       (20)     6413 2023-02-13 09:38:48.000000 whochat-1.3.5/whochat/abc.py
+-rw-r--r--   0 luming     (501) staff       (20)    22043 2023-05-26 16:24:36.000000 whochat-1.3.5/whochat/bot.py
+-rw-r--r--   0 luming     (501) staff       (20)     4952 2023-05-11 01:43:21.000000 whochat-1.3.5/whochat/cli.py
+-rw-r--r--   0 luming     (501) staff       (20)      762 2023-05-11 01:43:21.000000 whochat-1.3.5/whochat/logger.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-30 08:28:15.332038 whochat-1.3.5/whochat/messages/
+-rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.5/whochat/messages/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)      447 2023-03-09 10:27:55.000000 whochat-1.3.5/whochat/messages/constants.py
+-rw-r--r--   0 luming     (501) staff       (20)     6875 2023-01-29 06:35:29.000000 whochat-1.3.5/whochat/messages/tcp.py
+-rw-r--r--   0 luming     (501) staff       (20)     8543 2023-05-30 07:41:31.000000 whochat-1.3.5/whochat/messages/websocket.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-30 08:28:15.332927 whochat-1.3.5/whochat/rpc/
+-rw-r--r--   0 luming     (501) staff       (20)       22 2023-01-29 06:35:29.000000 whochat-1.3.5/whochat/rpc/__init__.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-30 08:28:15.333416 whochat-1.3.5/whochat/rpc/clients/
+-rw-r--r--   0 luming     (501) staff       (20)        0 2023-03-09 10:27:55.000000 whochat-1.3.5/whochat/rpc/clients/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)     4824 2023-05-29 14:29:26.000000 whochat-1.3.5/whochat/rpc/clients/websocket.py
+-rw-r--r--   0 luming     (501) staff       (20)     1823 2023-03-09 10:27:55.000000 whochat-1.3.5/whochat/rpc/docs.py
+-rw-r--r--   0 luming     (501) staff       (20)    10159 2023-05-26 15:23:50.000000 whochat-1.3.5/whochat/rpc/handlers.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-30 08:28:15.334282 whochat-1.3.5/whochat/rpc/servers/
+-rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.5/whochat/rpc/servers/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)      930 2023-01-29 06:35:29.000000 whochat-1.3.5/whochat/rpc/servers/http.py
+-rw-r--r--   0 luming     (501) staff       (20)     1138 2023-05-26 10:13:13.000000 whochat-1.3.5/whochat/rpc/servers/websocket.py
+-rw-r--r--   0 luming     (501) staff       (20)      315 2023-05-11 01:43:21.000000 whochat-1.3.5/whochat/settings.py
+-rw-r--r--   0 luming     (501) staff       (20)     1108 2023-05-29 10:26:50.000000 whochat-1.3.5/whochat/signals.py
+-rw-r--r--   0 luming     (501) staff       (20)     3091 2023-03-09 10:27:55.000000 whochat-1.3.5/whochat/utils.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-30 08:28:15.321704 whochat-1.3.5/whochat.egg-info/
+-rw-r--r--   0 luming     (501) staff       (20)     7727 2023-05-30 08:28:15.000000 whochat-1.3.5/whochat.egg-info/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)      870 2023-05-30 08:28:15.000000 whochat-1.3.5/whochat.egg-info/SOURCES.txt
+-rw-r--r--   0 luming     (501) staff       (20)        1 2023-05-30 08:28:15.000000 whochat-1.3.5/whochat.egg-info/dependency_links.txt
+-rw-r--r--   0 luming     (501) staff       (20)       50 2023-05-30 08:28:15.000000 whochat-1.3.5/whochat.egg-info/entry_points.txt
+-rw-r--r--   0 luming     (501) staff       (20)      115 2023-05-30 08:28:15.000000 whochat-1.3.5/whochat.egg-info/requires.txt
+-rw-r--r--   0 luming     (501) staff       (20)        8 2023-05-30 08:28:15.000000 whochat-1.3.5/whochat.egg-info/top_level.txt
```

### Comparing `whochat-1.3.4/LICENSE` & `whochat-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/PKG-INFO` & `whochat-1.3.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whochat
-Version: 1.3.4
+Version: 1.3.5
 Summary: 一个命令就可启用的微信机器人
 Home-page: https://github.com/amchii/whochat
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/whochat
 Classifier: Intended Audience :: Developers
@@ -189,14 +189,18 @@
     "id": 4
 }
 ```
 
 [CHANGELOG](https://github.com/amchii/whochat/blob/main/CHANGELOG.md)
 
 [Tags](https://github.com/amchii/whochat/tags)
+## v1.3.5
+* 解析最新微信版本`extra_info`
+* Log raw message at debug level
+
 ## v1.3.4
 * 自动设置微信版本号避免更新
 * 增加环境变量`WHOCHAT_WECHAT_VERSION`自定义微信版本号
 * 尝试使`BotWebsocketRPCClient.rpc_call`更正确地运行
 
 ## v1.3.3
 * 增加获取微信最新版本号的方法
```

### Comparing `whochat-1.3.4/README.md` & `whochat-1.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,18 @@
     "id": 4
 }
 ```
 
 [CHANGELOG](https://github.com/amchii/whochat/blob/main/CHANGELOG.md)
 
 [Tags](https://github.com/amchii/whochat/tags)
+## v1.3.5
+* 解析最新微信版本`extra_info`
+* Log raw message at debug level
+
 ## v1.3.4
 * 自动设置微信版本号避免更新
 * 增加环境变量`WHOCHAT_WECHAT_VERSION`自定义微信版本号
 * 尝试使`BotWebsocketRPCClient.rpc_call`更正确地运行
 
 ## v1.3.3
 * 增加获取微信最新版本号的方法
```

### Comparing `whochat-1.3.4/setup.cfg` & `whochat-1.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/ComWeChatRobot/CWeChatRobot.exe` & `whochat-1.3.5/whochat/ComWeChatRobot/CWeChatRobot.exe`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/ComWeChatRobot/DWeChatRobot.dll` & `whochat-1.3.5/whochat/ComWeChatRobot/DWeChatRobot.dll`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/_comtypes.py` & `whochat-1.3.5/whochat/_comtypes.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/abc.py` & `whochat-1.3.5/whochat/abc.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/bot.py` & `whochat-1.3.5/whochat/bot.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/cli.py` & `whochat-1.3.5/whochat/cli.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/logger.py` & `whochat-1.3.5/whochat/logger.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/messages/tcp.py` & `whochat-1.3.5/whochat/messages/tcp.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/rpc/clients/websocket.py` & `whochat-1.3.5/whochat/rpc/clients/websocket.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/rpc/docs.py` & `whochat-1.3.5/whochat/rpc/docs.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/rpc/handlers.py` & `whochat-1.3.5/whochat/rpc/handlers.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/rpc/servers/http.py` & `whochat-1.3.5/whochat/rpc/servers/http.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/rpc/servers/websocket.py` & `whochat-1.3.5/whochat/rpc/servers/websocket.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/signals.py` & `whochat-1.3.5/whochat/signals.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat/utils.py` & `whochat-1.3.5/whochat/utils.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.4/whochat.egg-info/PKG-INFO` & `whochat-1.3.5/whochat.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whochat
-Version: 1.3.4
+Version: 1.3.5
 Summary: 一个命令就可启用的微信机器人
 Home-page: https://github.com/amchii/whochat
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/whochat
 Classifier: Intended Audience :: Developers
@@ -189,14 +189,18 @@
     "id": 4
 }
 ```
 
 [CHANGELOG](https://github.com/amchii/whochat/blob/main/CHANGELOG.md)
 
 [Tags](https://github.com/amchii/whochat/tags)
+## v1.3.5
+* 解析最新微信版本`extra_info`
+* Log raw message at debug level
+
 ## v1.3.4
 * 自动设置微信版本号避免更新
 * 增加环境变量`WHOCHAT_WECHAT_VERSION`自定义微信版本号
 * 尝试使`BotWebsocketRPCClient.rpc_call`更正确地运行
 
 ## v1.3.3
 * 增加获取微信最新版本号的方法
```

### Comparing `whochat-1.3.4/whochat.egg-info/SOURCES.txt` & `whochat-1.3.5/whochat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

