# Comparing `tmp/Telegant-0.2.1.tar.gz` & `tmp/Telegant-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Telegant-0.2.1.tar", last modified: Wed Apr  5 23:06:59 2023, max compression
+gzip compressed data, was "Telegant-0.2.2.tar", last modified: Tue May 30 00:33:49 2023, max compression
```

## Comparing `Telegant-0.2.1.tar` & `Telegant-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 23:06:59.084687 Telegant-0.2.1/
--rw-rw-rw-   0        0        0     1086 2023-03-12 18:52:49.000000 Telegant-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     5049 2023-04-05 23:06:59.083685 Telegant-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4513 2023-04-05 23:02:47.000000 Telegant-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 23:06:59.068853 Telegant-0.2.1/Telegant.egg-info/
--rw-rw-rw-   0        0        0     5049 2023-04-05 23:06:58.000000 Telegant-0.2.1/Telegant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-04-05 23:06:58.000000 Telegant-0.2.1/Telegant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 23:06:58.000000 Telegant-0.2.1/Telegant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-05 23:06:58.000000 Telegant-0.2.1/Telegant.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-05 23:06:58.000000 Telegant-0.2.1/Telegant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 23:06:59.084687 Telegant-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      699 2023-04-03 04:31:03.000000 Telegant-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-05 23:06:59.072672 Telegant-0.2.1/telegant/
--rw-rw-rw-   0        0        0       26 2023-03-29 05:18:44.000000 Telegant-0.2.1/telegant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 23:06:59.082687 Telegant-0.2.1/telegant/handlers/
--rw-rw-rw-   0        0        0      818 2023-03-20 04:46:56.000000 Telegant-0.2.1/telegant/handlers/CallbackQueryHandler.py
--rw-rw-rw-   0        0        0      489 2023-03-20 04:46:56.000000 Telegant-0.2.1/telegant/handlers/CommandHandler.py
--rw-rw-rw-   0        0        0     1480 2023-04-05 22:59:54.000000 Telegant-0.2.1/telegant/handlers/EventHandler.py
--rw-rw-rw-   0        0        0      494 2023-03-28 00:59:15.000000 Telegant-0.2.1/telegant/handlers/TextHandler.py
--rw-rw-rw-   0        0        0      226 2023-03-20 04:46:56.000000 Telegant-0.2.1/telegant/handlers/UpdateHandler.py
--rw-rw-rw-   0        0        0      220 2023-03-20 04:46:56.000000 Telegant-0.2.1/telegant/handlers/__init__.py
--rw-rw-rw-   0        0        0     1224 2023-04-03 04:54:12.000000 Telegant-0.2.1/telegant/method.py
--rw-rw-rw-   0        0        0     4471 2023-03-29 05:18:44.000000 Telegant-0.2.1/telegant/telegant.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:33:49.113086 Telegant-0.2.2/
+-rw-rw-rw-   0        0        0     1086 2023-03-12 18:52:49.000000 Telegant-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     5067 2023-05-30 00:33:49.113086 Telegant-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4531 2023-04-05 23:12:27.000000 Telegant-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 00:33:49.092089 Telegant-0.2.2/Telegant.egg-info/
+-rw-rw-rw-   0        0        0     5067 2023-05-30 00:33:48.000000 Telegant-0.2.2/Telegant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-05-30 00:33:49.000000 Telegant-0.2.2/Telegant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 00:33:48.000000 Telegant-0.2.2/Telegant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 00:33:48.000000 Telegant-0.2.2/Telegant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 00:33:48.000000 Telegant-0.2.2/Telegant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 00:33:49.113086 Telegant-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      699 2023-05-30 00:31:07.000000 Telegant-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:33:49.098088 Telegant-0.2.2/telegant/
+-rw-rw-rw-   0        0        0       26 2023-03-29 05:18:44.000000 Telegant-0.2.2/telegant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:33:49.112085 Telegant-0.2.2/telegant/handlers/
+-rw-rw-rw-   0        0        0      818 2023-03-20 04:46:56.000000 Telegant-0.2.2/telegant/handlers/CallbackQueryHandler.py
+-rw-rw-rw-   0        0        0      623 2023-05-29 23:55:01.000000 Telegant-0.2.2/telegant/handlers/CommandHandler.py
+-rw-rw-rw-   0        0        0     1480 2023-04-05 22:59:54.000000 Telegant-0.2.2/telegant/handlers/EventHandler.py
+-rw-rw-rw-   0        0        0      634 2023-05-30 00:09:04.000000 Telegant-0.2.2/telegant/handlers/TextHandler.py
+-rw-rw-rw-   0        0        0      224 2023-05-30 00:30:38.000000 Telegant-0.2.2/telegant/handlers/UpdateHandler.py
+-rw-rw-rw-   0        0        0      220 2023-03-20 04:46:56.000000 Telegant-0.2.2/telegant/handlers/__init__.py
+-rw-rw-rw-   0        0        0     1224 2023-04-03 04:54:12.000000 Telegant-0.2.2/telegant/method.py
+-rw-rw-rw-   0        0        0     5092 2023-05-30 00:04:09.000000 Telegant-0.2.2/telegant/telegant.py
```

### Comparing `Telegant-0.2.1/LICENSE` & `Telegant-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.1/PKG-INFO` & `Telegant-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Telegant
-Version: 0.2.1
+Version: 0.2.2
 Summary: An Elegant Modern Bot Framework for Python
 Home-page: https://github.com/kotov584/Telegant
 Author: Kotov584
 License: MIT
 Keywords: python,telegram,bot,api,async,asynchronous,elegant,modern
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -122,15 +122,15 @@
 
 ### Inline buttons example
 ```python 
 @bot.hear("hello")
 async def say_hello(bot, update): 
     buttons = [
         [
-            {"text": "Option 1 (inline)", "data": "option1"},  
+            {"text": "Option 1 (inline)", "callback_data": "option1"},  
         ]
     ]
 
     #snake_case example
     await bot.send_message(text="What's up?", reply_markup=buttons)
 ```
 
@@ -144,15 +144,15 @@
             {"text": "Option 1 (reply)"},  
         ]
     ]
 
     await bot.send_message(text="What's up?", reply_markup=buttons)
 ```
 
-Bot always detects your buttons type automatically by data key. 
+Bot always detects your buttons type automatically by callback_data key. 
 If you want to use inline buttons you have to write text and data values for each button.
 As it is detects your inline button when you have "data" key in your button.
 Otherwise, it will detect as reply keyboard.
 
 ## Commands
 
 You can assign to one function one command or many commands as needed.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Telegant Version: 0.2.1 Summary: An Elegant Modern
+Metadata-Version: 2.1 Name: Telegant Version: 0.2.2 Summary: An Elegant Modern
 Bot Framework for Python Home-page: https://github.com/kotov584/Telegant
 Author: Kotov584 License: MIT Keywords:
 python,telegram,bot,api,async,asynchronous,elegant,modern Requires-Python:
 >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
                             ****** Telegant ******
        [Code_style:_black] [https://img.shields.io/badge/Telegram-Group-
     blue.svg?logo=telegram] [https://img.shields.io/badge/Telegram-Channel-
@@ -28,23 +28,23 @@
 case styles ### snake_case ```python @bot.hear("hello") async def say_hello
 (bot, update): await bot.send_message(text="What's up?") ``` ### camelCase
 ```python @bot.hear("hello") async def say_hello(bot, update): await
 bot.sendMessage(text="What's up?") ``` ### PascalCase ```python @bot.hear
 ("hello") async def say_hello(bot, update): await bot.SendMessage(text="What's
 up?") ``` ## Sending bot with buttons ### Inline buttons example ```python
 @bot.hear("hello") async def say_hello(bot, update): buttons = [ [ {"text":
-"Option 1 (inline)", "data": "option1"}, ] ] #snake_case example await
+"Option 1 (inline)", "callback_data": "option1"}, ] ] #snake_case example await
 bot.send_message(text="What's up?", reply_markup=buttons) ``` ### Reply buttons
 example ```python @bot.hear("hello") async def say_hello(bot, update): buttons
 = [ [ {"text": "Option 1 (reply)"}, ] ] await bot.send_message(text="What's
 up?", reply_markup=buttons) ``` Bot always detects your buttons type
-automatically by data key. If you want to use inline buttons you have to write
-text and data values for each button. As it is detects your inline button when
-you have "data" key in your button. Otherwise, it will detect as reply
-keyboard. ## Commands You can assign to one function one command or many
+automatically by callback_data key. If you want to use inline buttons you have
+to write text and data values for each button. As it is detects your inline
+button when you have "data" key in your button. Otherwise, it will detect as
+reply keyboard. ## Commands You can assign to one function one command or many
 commands as needed. For single command use @bot.command() decorator. ```python
 @bot.command("start") async def say_hello(bot, update): await bot.send_message
 (text="Sup I'm start") ``` For several commands use @bot.commands() decorator.
 ```python @bot.commands(['help', 'ask']) async def say_hello(bot, update):
 await bot.send_message(text="You've reached for help") ``` Export data after
 command by your keys ```python @bot.commands(['usernameandage']) @bot.with_args
 (['username', 'age']) async def handler(bot, update, data): await
```

### Comparing `Telegant-0.2.1/README.md` & `Telegant-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
 ### Inline buttons example
 ```python 
 @bot.hear("hello")
 async def say_hello(bot, update): 
     buttons = [
         [
-            {"text": "Option 1 (inline)", "data": "option1"},  
+            {"text": "Option 1 (inline)", "callback_data": "option1"},  
         ]
     ]
 
     #snake_case example
     await bot.send_message(text="What's up?", reply_markup=buttons)
 ```
 
@@ -132,15 +132,15 @@
             {"text": "Option 1 (reply)"},  
         ]
     ]
 
     await bot.send_message(text="What's up?", reply_markup=buttons)
 ```
 
-Bot always detects your buttons type automatically by data key. 
+Bot always detects your buttons type automatically by callback_data key. 
 If you want to use inline buttons you have to write text and data values for each button.
 As it is detects your inline button when you have "data" key in your button.
 Otherwise, it will detect as reply keyboard.
 
 ## Commands
 
 You can assign to one function one command or many commands as needed.
```

#### html2text {}

```diff
@@ -23,23 +23,23 @@
 case styles ### snake_case ```python @bot.hear("hello") async def say_hello
 (bot, update): await bot.send_message(text="What's up?") ``` ### camelCase
 ```python @bot.hear("hello") async def say_hello(bot, update): await
 bot.sendMessage(text="What's up?") ``` ### PascalCase ```python @bot.hear
 ("hello") async def say_hello(bot, update): await bot.SendMessage(text="What's
 up?") ``` ## Sending bot with buttons ### Inline buttons example ```python
 @bot.hear("hello") async def say_hello(bot, update): buttons = [ [ {"text":
-"Option 1 (inline)", "data": "option1"}, ] ] #snake_case example await
+"Option 1 (inline)", "callback_data": "option1"}, ] ] #snake_case example await
 bot.send_message(text="What's up?", reply_markup=buttons) ``` ### Reply buttons
 example ```python @bot.hear("hello") async def say_hello(bot, update): buttons
 = [ [ {"text": "Option 1 (reply)"}, ] ] await bot.send_message(text="What's
 up?", reply_markup=buttons) ``` Bot always detects your buttons type
-automatically by data key. If you want to use inline buttons you have to write
-text and data values for each button. As it is detects your inline button when
-you have "data" key in your button. Otherwise, it will detect as reply
-keyboard. ## Commands You can assign to one function one command or many
+automatically by callback_data key. If you want to use inline buttons you have
+to write text and data values for each button. As it is detects your inline
+button when you have "data" key in your button. Otherwise, it will detect as
+reply keyboard. ## Commands You can assign to one function one command or many
 commands as needed. For single command use @bot.command() decorator. ```python
 @bot.command("start") async def say_hello(bot, update): await bot.send_message
 (text="Sup I'm start") ``` For several commands use @bot.commands() decorator.
 ```python @bot.commands(['help', 'ask']) async def say_hello(bot, update):
 await bot.send_message(text="You've reached for help") ``` Export data after
 command by your keys ```python @bot.commands(['usernameandage']) @bot.with_args
 (['username', 'age']) async def handler(bot, update, data): await
```

### Comparing `Telegant-0.2.1/Telegant.egg-info/PKG-INFO` & `Telegant-0.2.2/Telegant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Telegant
-Version: 0.2.1
+Version: 0.2.2
 Summary: An Elegant Modern Bot Framework for Python
 Home-page: https://github.com/kotov584/Telegant
 Author: Kotov584
 License: MIT
 Keywords: python,telegram,bot,api,async,asynchronous,elegant,modern
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -122,15 +122,15 @@
 
 ### Inline buttons example
 ```python 
 @bot.hear("hello")
 async def say_hello(bot, update): 
     buttons = [
         [
-            {"text": "Option 1 (inline)", "data": "option1"},  
+            {"text": "Option 1 (inline)", "callback_data": "option1"},  
         ]
     ]
 
     #snake_case example
     await bot.send_message(text="What's up?", reply_markup=buttons)
 ```
 
@@ -144,15 +144,15 @@
             {"text": "Option 1 (reply)"},  
         ]
     ]
 
     await bot.send_message(text="What's up?", reply_markup=buttons)
 ```
 
-Bot always detects your buttons type automatically by data key. 
+Bot always detects your buttons type automatically by callback_data key. 
 If you want to use inline buttons you have to write text and data values for each button.
 As it is detects your inline button when you have "data" key in your button.
 Otherwise, it will detect as reply keyboard.
 
 ## Commands
 
 You can assign to one function one command or many commands as needed.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Telegant Version: 0.2.1 Summary: An Elegant Modern
+Metadata-Version: 2.1 Name: Telegant Version: 0.2.2 Summary: An Elegant Modern
 Bot Framework for Python Home-page: https://github.com/kotov584/Telegant
 Author: Kotov584 License: MIT Keywords:
 python,telegram,bot,api,async,asynchronous,elegant,modern Requires-Python:
 >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
                             ****** Telegant ******
        [Code_style:_black] [https://img.shields.io/badge/Telegram-Group-
     blue.svg?logo=telegram] [https://img.shields.io/badge/Telegram-Channel-
@@ -28,23 +28,23 @@
 case styles ### snake_case ```python @bot.hear("hello") async def say_hello
 (bot, update): await bot.send_message(text="What's up?") ``` ### camelCase
 ```python @bot.hear("hello") async def say_hello(bot, update): await
 bot.sendMessage(text="What's up?") ``` ### PascalCase ```python @bot.hear
 ("hello") async def say_hello(bot, update): await bot.SendMessage(text="What's
 up?") ``` ## Sending bot with buttons ### Inline buttons example ```python
 @bot.hear("hello") async def say_hello(bot, update): buttons = [ [ {"text":
-"Option 1 (inline)", "data": "option1"}, ] ] #snake_case example await
+"Option 1 (inline)", "callback_data": "option1"}, ] ] #snake_case example await
 bot.send_message(text="What's up?", reply_markup=buttons) ``` ### Reply buttons
 example ```python @bot.hear("hello") async def say_hello(bot, update): buttons
 = [ [ {"text": "Option 1 (reply)"}, ] ] await bot.send_message(text="What's
 up?", reply_markup=buttons) ``` Bot always detects your buttons type
-automatically by data key. If you want to use inline buttons you have to write
-text and data values for each button. As it is detects your inline button when
-you have "data" key in your button. Otherwise, it will detect as reply
-keyboard. ## Commands You can assign to one function one command or many
+automatically by callback_data key. If you want to use inline buttons you have
+to write text and data values for each button. As it is detects your inline
+button when you have "data" key in your button. Otherwise, it will detect as
+reply keyboard. ## Commands You can assign to one function one command or many
 commands as needed. For single command use @bot.command() decorator. ```python
 @bot.command("start") async def say_hello(bot, update): await bot.send_message
 (text="Sup I'm start") ``` For several commands use @bot.commands() decorator.
 ```python @bot.commands(['help', 'ask']) async def say_hello(bot, update):
 await bot.send_message(text="You've reached for help") ``` Export data after
 command by your keys ```python @bot.commands(['usernameandage']) @bot.with_args
 (['username', 'age']) async def handler(bot, update, data): await
```

### Comparing `Telegant-0.2.1/setup.py` & `Telegant-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup( 
     name='Telegant',
-    version='0.2.1',
+    version='0.2.2',
     description='An Elegant Modern Bot Framework for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kotov584/Telegant',
     author='Kotov584', 
     license='MIT', 
     keywords='python, telegram, bot, api, async, asynchronous, elegant, modern',
```

### Comparing `Telegant-0.2.1/telegant/handlers/CallbackQueryHandler.py` & `Telegant-0.2.2/telegant/handlers/CallbackQueryHandler.py`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.1/telegant/handlers/EventHandler.py` & `Telegant-0.2.2/telegant/handlers/EventHandler.py`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.1/telegant/method.py` & `Telegant-0.2.2/telegant/method.py`

 * *Files identical despite different names*

### Comparing `Telegant-0.2.1/telegant/telegant.py` & `Telegant-0.2.2/telegant/telegant.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 class Bot:
     def __init__(self, token):
         self.token = token
         self.event_handler = EventHandler()
         self.event_handler.base_url = f"https://api.telegram.org/bot{self.token}/"
+        self.user_state = {}
 
     async def polling(self):
         last_update_id = 0
         async with aiohttp.ClientSession() as session:
             while True:
                 response_json, last_update_id = await self.get_updates(
                     session, last_update_id
@@ -90,21 +91,21 @@
                         k: args[i] if i < len(args) else "" for i, k in enumerate(keys)
                     }
                     await handler_func(bot, update, data)
 
             return wrapper
 
         return decorator
-
-    def hear(self, value):
+        
+    def hear(self, value): 
         return self.process_event_handler(
             value, "message", TextHandler(self.event_handler), "message_handlers"
         )
 
-    def hears(self, value):
+    def hears(self, value): 
         return self.process_many_events(
             value, "message", TextHandler(self.event_handler), "message_handlers"
         )
 
     def command(self, value):
         return self.process_event_handler(
             value, "message", CommandHandler(self.event_handler), "command_handlers"
@@ -129,7 +130,23 @@
     def callbacks(self, callbacks_list):
         return self.process_many_events(
             callbacks_list,
             "callback_query",
             CallbackQueryHandler(self.event_handler),
             "callback_handlers",
         )
+
+    def dialogue(self, value):
+        def decorator(handler_func):
+            async def wrapper(bot, update): 
+                print(f"Dialogue {value} was detected.")
+                return await handler_func(bot, update)
+            return wrapper
+        return decorator
+
+    def step(self, value):
+        def decorator(handler_func):
+            async def wrapper(bot, update): 
+                print(f"Dialogue step {value} was detected.")      
+                return await handler_func(bot, update)
+            return wrapper  
+        return decorator
```

