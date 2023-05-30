# Comparing `tmp/Telegant-0.2.3.tar.gz` & `tmp/Telegant-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Telegant-0.2.3.tar", last modified: Tue May 30 01:22:37 2023, max compression
+gzip compressed data, was "Telegant-0.2.4.tar", last modified: Tue May 30 05:36:13 2023, max compression
```

## Comparing `Telegant-0.2.3.tar` & `Telegant-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 01:22:37.593829 Telegant-0.2.3/
--rw-rw-rw-   0        0        0     1086 2023-03-12 18:52:49.000000 Telegant-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     5067 2023-05-30 01:22:37.593829 Telegant-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4531 2023-04-05 23:12:27.000000 Telegant-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 01:22:37.582826 Telegant-0.2.3/Telegant.egg-info/
--rw-rw-rw-   0        0        0     5067 2023-05-30 01:22:37.000000 Telegant-0.2.3/Telegant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-05-30 01:22:37.000000 Telegant-0.2.3/Telegant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 01:22:37.000000 Telegant-0.2.3/Telegant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 01:22:37.000000 Telegant-0.2.3/Telegant.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 01:22:37.000000 Telegant-0.2.3/Telegant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 01:22:37.593829 Telegant-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      699 2023-05-30 01:21:33.000000 Telegant-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 01:22:37.585825 Telegant-0.2.3/telegant/
--rw-rw-rw-   0        0        0       26 2023-03-29 05:18:44.000000 Telegant-0.2.3/telegant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 01:22:37.592825 Telegant-0.2.3/telegant/handlers/
--rw-rw-rw-   0        0        0      818 2023-03-20 04:46:56.000000 Telegant-0.2.3/telegant/handlers/CallbackQueryHandler.py
--rw-rw-rw-   0        0        0      623 2023-05-29 23:55:01.000000 Telegant-0.2.3/telegant/handlers/CommandHandler.py
--rw-rw-rw-   0        0        0     1480 2023-04-05 22:59:54.000000 Telegant-0.2.3/telegant/handlers/EventHandler.py
--rw-rw-rw-   0        0        0      634 2023-05-30 00:09:04.000000 Telegant-0.2.3/telegant/handlers/TextHandler.py
--rw-rw-rw-   0        0        0      300 2023-05-30 01:15:05.000000 Telegant-0.2.3/telegant/handlers/UpdateHandler.py
--rw-rw-rw-   0        0        0      220 2023-03-20 04:46:56.000000 Telegant-0.2.3/telegant/handlers/__init__.py
--rw-rw-rw-   0        0        0     1224 2023-04-03 04:54:12.000000 Telegant-0.2.3/telegant/method.py
--rw-rw-rw-   0        0        0     5256 2023-05-30 01:12:50.000000 Telegant-0.2.3/telegant/telegant.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:36:13.873923 Telegant-0.2.4/
+-rw-rw-rw-   0        0        0     1086 2023-03-12 18:52:49.000000 Telegant-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     5067 2023-05-30 05:36:13.873923 Telegant-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4531 2023-04-05 23:12:27.000000 Telegant-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 05:36:13.865739 Telegant-0.2.4/Telegant.egg-info/
+-rw-rw-rw-   0        0        0     5067 2023-05-30 05:36:13.000000 Telegant-0.2.4/Telegant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-05-30 05:36:13.000000 Telegant-0.2.4/Telegant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 05:36:13.000000 Telegant-0.2.4/Telegant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 05:36:13.000000 Telegant-0.2.4/Telegant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 05:36:13.000000 Telegant-0.2.4/Telegant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 05:36:13.875006 Telegant-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      699 2023-05-30 05:35:01.000000 Telegant-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:36:13.867736 Telegant-0.2.4/telegant/
+-rw-rw-rw-   0        0        0       26 2023-03-29 05:18:44.000000 Telegant-0.2.4/telegant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:36:13.872923 Telegant-0.2.4/telegant/handlers/
+-rw-rw-rw-   0        0        0      818 2023-03-20 04:46:56.000000 Telegant-0.2.4/telegant/handlers/CallbackQueryHandler.py
+-rw-rw-rw-   0        0        0      623 2023-05-29 23:55:01.000000 Telegant-0.2.4/telegant/handlers/CommandHandler.py
+-rw-rw-rw-   0        0        0     1480 2023-04-05 22:59:54.000000 Telegant-0.2.4/telegant/handlers/EventHandler.py
+-rw-rw-rw-   0        0        0      634 2023-05-30 00:09:04.000000 Telegant-0.2.4/telegant/handlers/TextHandler.py
+-rw-rw-rw-   0        0        0      300 2023-05-30 01:15:05.000000 Telegant-0.2.4/telegant/handlers/UpdateHandler.py
+-rw-rw-rw-   0        0        0      220 2023-03-20 04:46:56.000000 Telegant-0.2.4/telegant/handlers/__init__.py
+-rw-rw-rw-   0        0        0     1224 2023-04-03 04:54:12.000000 Telegant-0.2.4/telegant/method.py
+-rw-rw-rw-   0        0        0     6241 2023-05-30 05:33:04.000000 Telegant-0.2.4/telegant/telegant.py
```

### Comparing `Telegant-0.2.3/LICENSE` & `Telegant-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.3/PKG-INFO` & `Telegant-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Telegant
-Version: 0.2.3
+Version: 0.2.4
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
-Metadata-Version: 2.1 Name: Telegant Version: 0.2.3 Summary: An Elegant Modern
+Metadata-Version: 2.1 Name: Telegant Version: 0.2.4 Summary: An Elegant Modern
 Bot Framework for Python Home-page: https://github.com/kotov584/Telegant
 Author: Kotov584 License: MIT Keywords:
 python,telegram,bot,api,async,asynchronous,elegant,modern Requires-Python:
 >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
                             ****** Telegant ******
        [Code_style:_black] [https://img.shields.io/badge/Telegram-Group-
     blue.svg?logo=telegram] [https://img.shields.io/badge/Telegram-Channel-
```

### Comparing `Telegant-0.2.3/README.md` & `Telegant-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.3/Telegant.egg-info/PKG-INFO` & `Telegant-0.2.4/Telegant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Telegant
-Version: 0.2.3
+Version: 0.2.4
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
-Metadata-Version: 2.1 Name: Telegant Version: 0.2.3 Summary: An Elegant Modern
+Metadata-Version: 2.1 Name: Telegant Version: 0.2.4 Summary: An Elegant Modern
 Bot Framework for Python Home-page: https://github.com/kotov584/Telegant
 Author: Kotov584 License: MIT Keywords:
 python,telegram,bot,api,async,asynchronous,elegant,modern Requires-Python:
 >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
                             ****** Telegant ******
        [Code_style:_black] [https://img.shields.io/badge/Telegram-Group-
     blue.svg?logo=telegram] [https://img.shields.io/badge/Telegram-Channel-
```

### Comparing `Telegant-0.2.3/setup.py` & `Telegant-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup( 
     name='Telegant',
-    version='0.2.3',
+    version='0.2.4',
     description='An Elegant Modern Bot Framework for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kotov584/Telegant',
     author='Kotov584', 
     license='MIT', 
     keywords='python, telegram, bot, api, async, asynchronous, elegant, modern',
```

### Comparing `Telegant-0.2.3/telegant/handlers/CallbackQueryHandler.py` & `Telegant-0.2.4/telegant/handlers/CallbackQueryHandler.py`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.3/telegant/handlers/CommandHandler.py` & `Telegant-0.2.4/telegant/handlers/CommandHandler.py`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.3/telegant/handlers/EventHandler.py` & `Telegant-0.2.4/telegant/handlers/EventHandler.py`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.3/telegant/handlers/TextHandler.py` & `Telegant-0.2.4/telegant/handlers/TextHandler.py`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.3/telegant/method.py` & `Telegant-0.2.4/telegant/method.py`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.3/telegant/telegant.py` & `Telegant-0.2.4/telegant/telegant.py`

 * *Files 11% similar despite different names*

```diff
@@ -91,14 +91,19 @@
                         k: args[i] if i < len(args) else "" for i, k in enumerate(keys)
                     }
                     await handler_func(bot, update, data)
 
             return wrapper
 
         return decorator
+
+    def init(self):
+        def decorator(handler_func):
+            return handler_func(self.event_handler)
+        return decorator
         
     def on(self, value): 
         return self.process_event_handler(
             value, value, UpdateHandler(self.event_handler), "update_handlers"
         )
 
     def hear(self, value): 
@@ -151,7 +156,25 @@
     def step(self, value):
         def decorator(handler_func):
             async def wrapper(bot, update): 
                 print(f"Dialogue step {value} was detected.")      
                 return await handler_func(bot, update)
             return wrapper  
         return decorator
+
+    async def request(self, action, params=None):
+        async with aiohttp.ClientSession() as session:
+            try:
+                url = f"{self.base_url}{action}"
+                if not params.get("chat_id"):
+                    params["chat_id"] = self.chat_id
+                if params.get("reply_markup"):
+                    params["reply_markup"] = self.create_keyboard(params["reply_markup"])
+                response = await session.post(url, params=params)
+                return await response.json()
+            except Exception as e:
+                print(f"Error sending request: {e}")
+
+    def __getattr__(self, name):
+        async def wrapper(**params):
+            camel_case_name = re.sub(r"_([a-z])", lambda m: m.group(1).upper(), name)
+            return await self.request(camel_case_name, params)
```

