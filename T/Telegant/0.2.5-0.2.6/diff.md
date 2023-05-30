# Comparing `tmp/Telegant-0.2.5.tar.gz` & `tmp/Telegant-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Telegant-0.2.5.tar", last modified: Tue May 30 06:30:58 2023, max compression
+gzip compressed data, was "Telegant-0.2.6.tar", last modified: Tue May 30 13:58:58 2023, max compression
```

## Comparing `Telegant-0.2.5.tar` & `Telegant-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 06:30:58.447877 Telegant-0.2.5/
--rw-rw-rw-   0        0        0     1086 2023-03-12 18:52:49.000000 Telegant-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     5067 2023-05-30 06:30:58.447877 Telegant-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4531 2023-04-05 23:12:27.000000 Telegant-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 06:30:58.432257 Telegant-0.2.5/Telegant.egg-info/
--rw-rw-rw-   0        0        0     5067 2023-05-30 06:30:58.000000 Telegant-0.2.5/Telegant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-05-30 06:30:58.000000 Telegant-0.2.5/Telegant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 06:30:58.000000 Telegant-0.2.5/Telegant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 06:30:58.000000 Telegant-0.2.5/Telegant.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 06:30:58.000000 Telegant-0.2.5/Telegant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 06:30:58.447877 Telegant-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      699 2023-05-30 06:30:32.000000 Telegant-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 06:30:58.432257 Telegant-0.2.5/telegant/
--rw-rw-rw-   0        0        0       26 2023-03-29 05:18:44.000000 Telegant-0.2.5/telegant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 06:30:58.447877 Telegant-0.2.5/telegant/handlers/
--rw-rw-rw-   0        0        0      818 2023-03-20 04:46:56.000000 Telegant-0.2.5/telegant/handlers/CallbackQueryHandler.py
--rw-rw-rw-   0        0        0      623 2023-05-29 23:55:01.000000 Telegant-0.2.5/telegant/handlers/CommandHandler.py
--rw-rw-rw-   0        0        0     1480 2023-04-05 22:59:54.000000 Telegant-0.2.5/telegant/handlers/EventHandler.py
--rw-rw-rw-   0        0        0      634 2023-05-30 00:09:04.000000 Telegant-0.2.5/telegant/handlers/TextHandler.py
--rw-rw-rw-   0        0        0      300 2023-05-30 01:15:05.000000 Telegant-0.2.5/telegant/handlers/UpdateHandler.py
--rw-rw-rw-   0        0        0      220 2023-03-20 04:46:56.000000 Telegant-0.2.5/telegant/handlers/__init__.py
--rw-rw-rw-   0        0        0     1224 2023-04-03 04:54:12.000000 Telegant-0.2.5/telegant/method.py
--rw-rw-rw-   0        0        0     6308 2023-05-30 06:28:49.000000 Telegant-0.2.5/telegant/telegant.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:58:58.167859 Telegant-0.2.6/
+-rw-rw-rw-   0        0        0     1086 2023-03-12 18:52:49.000000 Telegant-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     5067 2023-05-30 13:58:58.167859 Telegant-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4531 2023-04-05 23:12:27.000000 Telegant-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 13:58:58.152237 Telegant-0.2.6/Telegant.egg-info/
+-rw-rw-rw-   0        0        0     5067 2023-05-30 13:58:58.000000 Telegant-0.2.6/Telegant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-05-30 13:58:58.000000 Telegant-0.2.6/Telegant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 13:58:58.000000 Telegant-0.2.6/Telegant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 13:58:58.000000 Telegant-0.2.6/Telegant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 13:58:58.000000 Telegant-0.2.6/Telegant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 13:58:58.167859 Telegant-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      699 2023-05-30 13:42:30.000000 Telegant-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:58:58.152237 Telegant-0.2.6/telegant/
+-rw-rw-rw-   0        0        0       26 2023-03-29 05:18:44.000000 Telegant-0.2.6/telegant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:58:58.167859 Telegant-0.2.6/telegant/handlers/
+-rw-rw-rw-   0        0        0      818 2023-03-20 04:46:56.000000 Telegant-0.2.6/telegant/handlers/CallbackQueryHandler.py
+-rw-rw-rw-   0        0        0      623 2023-05-29 23:55:01.000000 Telegant-0.2.6/telegant/handlers/CommandHandler.py
+-rw-rw-rw-   0        0        0     1480 2023-04-05 22:59:54.000000 Telegant-0.2.6/telegant/handlers/EventHandler.py
+-rw-rw-rw-   0        0        0      634 2023-05-30 00:09:04.000000 Telegant-0.2.6/telegant/handlers/TextHandler.py
+-rw-rw-rw-   0        0        0      300 2023-05-30 01:15:05.000000 Telegant-0.2.6/telegant/handlers/UpdateHandler.py
+-rw-rw-rw-   0        0        0      220 2023-03-20 04:46:56.000000 Telegant-0.2.6/telegant/handlers/__init__.py
+-rw-rw-rw-   0        0        0     1224 2023-04-03 04:54:12.000000 Telegant-0.2.6/telegant/method.py
+-rw-rw-rw-   0        0        0     6436 2023-05-30 13:43:05.000000 Telegant-0.2.6/telegant/telegant.py
```

### Comparing `Telegant-0.2.5/LICENSE` & `Telegant-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.5/PKG-INFO` & `Telegant-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Telegant
-Version: 0.2.5
+Version: 0.2.6
 Summary: An Elegant Modern Bot Framework for Python
 Home-page: https://github.com/kotov584/Telegant
 Author: Kotov584
 License: MIT
 Keywords: python,telegram,bot,api,async,asynchronous,elegant,modern
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Telegant Version: 0.2.5 Summary: An Elegant Modern
+Metadata-Version: 2.1 Name: Telegant Version: 0.2.6 Summary: An Elegant Modern
 Bot Framework for Python Home-page: https://github.com/kotov584/Telegant
 Author: Kotov584 License: MIT Keywords:
 python,telegram,bot,api,async,asynchronous,elegant,modern Requires-Python:
 >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
                             ****** Telegant ******
        [Code_style:_black] [https://img.shields.io/badge/Telegram-Group-
     blue.svg?logo=telegram] [https://img.shields.io/badge/Telegram-Channel-
```

### Comparing `Telegant-0.2.5/README.md` & `Telegant-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.5/Telegant.egg-info/PKG-INFO` & `Telegant-0.2.6/Telegant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Telegant
-Version: 0.2.5
+Version: 0.2.6
 Summary: An Elegant Modern Bot Framework for Python
 Home-page: https://github.com/kotov584/Telegant
 Author: Kotov584
 License: MIT
 Keywords: python,telegram,bot,api,async,asynchronous,elegant,modern
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Telegant Version: 0.2.5 Summary: An Elegant Modern
+Metadata-Version: 2.1 Name: Telegant Version: 0.2.6 Summary: An Elegant Modern
 Bot Framework for Python Home-page: https://github.com/kotov584/Telegant
 Author: Kotov584 License: MIT Keywords:
 python,telegram,bot,api,async,asynchronous,elegant,modern Requires-Python:
 >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
                             ****** Telegant ******
        [Code_style:_black] [https://img.shields.io/badge/Telegram-Group-
     blue.svg?logo=telegram] [https://img.shields.io/badge/Telegram-Channel-
```

### Comparing `Telegant-0.2.5/setup.py` & `Telegant-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup( 
     name='Telegant',
-    version='0.2.5',
+    version='0.2.6',
     description='An Elegant Modern Bot Framework for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kotov584/Telegant',
     author='Kotov584', 
     license='MIT', 
     keywords='python, telegram, bot, api, async, asynchronous, elegant, modern',
```

### Comparing `Telegant-0.2.5/telegant/handlers/CallbackQueryHandler.py` & `Telegant-0.2.6/telegant/handlers/CallbackQueryHandler.py`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.5/telegant/handlers/CommandHandler.py` & `Telegant-0.2.6/telegant/handlers/CommandHandler.py`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.5/telegant/handlers/EventHandler.py` & `Telegant-0.2.6/telegant/handlers/EventHandler.py`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.5/telegant/handlers/TextHandler.py` & `Telegant-0.2.6/telegant/handlers/TextHandler.py`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.5/telegant/method.py` & `Telegant-0.2.6/telegant/method.py`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.5/telegant/telegant.py` & `Telegant-0.2.6/telegant/telegant.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,26 @@
     EventHandler,
     TextHandler,
     CommandHandler,
     CallbackQueryHandler,
     UpdateHandler,
 )
 
+from .method import *
 import re
 import aiohttp
 import asyncio
 
 
 class Bot:
     def __init__(self, token):
-        self.token = token
+        self.token = "6107480665:AAGV5JNUnh6ALI53-JZpjkft-7g2cL1BSGA"
         self.event_handler = EventHandler()
-        self.event_handler.base_url = f"https://api.telegram.org/bot{self.token}/"
+        self.base_url = f"https://api.telegram.org/bot{self.token}/"
+        self.event_handler.base_url = self.base_url 
         self.user_state = {}  
 
     async def polling(self):
         last_update_id = 0
         async with aiohttp.ClientSession() as session:
             while True:
                 response_json, last_update_id = await self.get_updates(
@@ -175,7 +177,8 @@
             except Exception as e:
                 print(f"Error sending request: {e}")
 
     def __getattr__(self, name):
         async def wrapper(**params):
             camel_case_name = re.sub(r"_([a-z])", lambda m: m.group(1).upper(), name)
             return await self.request(camel_case_name, params)
+        return wrapper
```

