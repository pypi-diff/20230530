# Comparing `tmp/chatgpt-mixin-0.1.7.tar.gz` & `tmp/chatgpt-mixin-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-mixin-0.1.7.tar", last modified: Mon May 29 12:27:12 2023, max compression
+gzip compressed data, was "chatgpt-mixin-0.1.8.tar", last modified: Tue May 30 07:00:34 2023, max compression
```

## Comparing `chatgpt-mixin-0.1.7.tar` & `chatgpt-mixin-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 12:27:12.928991 chatgpt-mixin-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-05-29 12:27:12.928991 chatgpt-mixin-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 12:27:12.928991 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-05-29 12:27:12.000000 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-29 12:27:12.000000 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 12:27:12.000000 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-29 12:27:12.000000 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-29 12:27:12.000000 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-29 12:27:12.000000 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      357 2023-05-29 12:27:12.932991 chatgpt-mixin-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 12:27:12.928991 chatgpt-mixin-0.1.7/src/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15472 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/src/chatgpt_browser.py
--rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/src/chatgpt_openai.py
--rw-r--r--   0 runner    (1001) docker     (122)    17336 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/src/mixinbot.py
--rw-r--r--   0 runner    (1001) docker     (122)     1983 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/src/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:00:34.270464 chatgpt-mixin-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-05-30 07:00:28.000000 chatgpt-mixin-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-05-30 07:00:34.270464 chatgpt-mixin-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-05-30 07:00:28.000000 chatgpt-mixin-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:00:34.270464 chatgpt-mixin-0.1.8/chatgpt_mixin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-05-30 07:00:34.000000 chatgpt-mixin-0.1.8/chatgpt_mixin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-30 07:00:34.000000 chatgpt-mixin-0.1.8/chatgpt_mixin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 07:00:34.000000 chatgpt-mixin-0.1.8/chatgpt_mixin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-30 07:00:34.000000 chatgpt-mixin-0.1.8/chatgpt_mixin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-30 07:00:34.000000 chatgpt-mixin-0.1.8/chatgpt_mixin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-30 07:00:34.000000 chatgpt-mixin-0.1.8/chatgpt_mixin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      357 2023-05-30 07:00:34.270464 chatgpt-mixin-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-30 07:00:28.000000 chatgpt-mixin-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:00:34.270464 chatgpt-mixin-0.1.8/src/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 07:00:28.000000 chatgpt-mixin-0.1.8/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-30 07:00:28.000000 chatgpt-mixin-0.1.8/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15472 2023-05-30 07:00:28.000000 chatgpt-mixin-0.1.8/src/chatgpt_browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-05-30 07:00:28.000000 chatgpt-mixin-0.1.8/src/chatgpt_openai.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17159 2023-05-30 07:00:28.000000 chatgpt-mixin-0.1.8/src/mixinbot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1983 2023-05-30 07:00:28.000000 chatgpt-mixin-0.1.8/src/test.py
```

### Comparing `chatgpt-mixin-0.1.7/LICENSE` & `chatgpt-mixin-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-mixin-0.1.7/PKG-INFO` & `chatgpt-mixin-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-mixin
-Version: 0.1.7
+Version: 0.1.8
 Summary: ChatGPT Bot For Mixin
 Home-page: https://github.com/learnforpractice/chatgpt-mixin
 Author: learnforpractice
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: browser
 License-File: LICENSE
```

### Comparing `chatgpt-mixin-0.1.7/README.md` & `chatgpt-mixin-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/PKG-INFO` & `chatgpt-mixin-0.1.8/chatgpt_mixin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-mixin
-Version: 0.1.7
+Version: 0.1.8
 Summary: ChatGPT Bot For Mixin
 Home-page: https://github.com/learnforpractice/chatgpt-mixin
 Author: learnforpractice
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: browser
 License-File: LICENSE
```

### Comparing `chatgpt-mixin-0.1.7/src/chatgpt_browser.py` & `chatgpt-mixin-0.1.8/src/chatgpt_browser.py`

 * *Files identical despite different names*

### Comparing `chatgpt-mixin-0.1.7/src/chatgpt_openai.py` & `chatgpt-mixin-0.1.8/src/chatgpt_openai.py`

 * *Files identical despite different names*

### Comparing `chatgpt-mixin-0.1.7/src/mixinbot.py` & `chatgpt-mixin-0.1.8/src/mixinbot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # -*- coding: utf-8 -*-
 
+import asyncio
+import base64
 import os
+import platform
+import signal
 import sys
 import time
-import asyncio
-import signal
-import base64
-import yaml
 import traceback
-import websockets
-import platform
-import httpx
+from dataclasses import dataclass
 from datetime import datetime
-from typing import Optional, List, Dict, Any, Union, Set
-
-from pymixin.mixin_ws_api import MixinWSApi, MessageView
-from pymixin import utils
-from pymixin import log
+from typing import Any, Dict, List, Optional, Set, Union
 
-from dataclasses import dataclass
+import httpx
+import websockets
+import yaml
+from pymixin import log, utils
+from pymixin.mixin_ws_api import MessageView, MixinWSApi
 
 logger = log.get_logger(__name__)
 logger.addHandler(log.handler)
 
 @dataclass
 class AnswerRequestTask:
     conversation_id: str
@@ -140,29 +138,21 @@
 
         if 'developer_conversation_id' in config:
             self.developer_conversation_id = config['developer_conversation_id']
             self.developer_user_id = config['developer_user_id']
         # openai_api_key
         self.bots = []
         self.standby_bots = []
-        self._paused = False
-
-    @property
-    def paused(self):
-        return self._paused
-    
-    @paused.setter
-    def paused(self, value):
-        self._paused = value
 
     async def init(self):
         asyncio.create_task(self.handle_questions())
 
         if self.chatgpt_accounts:
             from playwright.async_api import async_playwright
+
             from .chatgpt_browser import ChatGPTBot
             PLAY = await async_playwright().start()
             for account in self.chatgpt_accounts:
                 user = account['user']
                 psw = account['psw']
                 bot = ChatGPTBot(PLAY, user, psw)
                 await bot.init()
@@ -179,22 +169,17 @@
 
         loop = asyncio.get_running_loop()
         loop.add_signal_handler(signal.SIGINT, lambda: asyncio.create_task(self.handle_signal(signal.SIGINT)))
         loop.add_signal_handler(signal.SIGTERM, lambda: asyncio.create_task(self.handle_signal(signal.SIGTERM)))
 
     async def handle_signal(self, signum):
         logger.info("+++++++handle signal: %s", signum)
-        for bot in self.bots:
-            logger.info("++close bot: %s", bot)
-            await bot.close()
         loop = asyncio.get_running_loop()
-        loop.remove_signal_handler(signal.SIGINT)
-        loop.remove_signal_handler(signal.SIGTERM)
-        sys.exit(0)
-        # os.kill(os.getpid(), signal.SIGINT)
+        for task in asyncio.all_tasks(loop):
+            task.cancel()
 
     def choose_bot(self, user_id):
         bots = []
         for bot in self.bots:
             if bot.standby:
                 continue
             bots.append(bot)
@@ -258,34 +243,40 @@
         except Exception as e:
             logger.exception(e)
         self.save_question(conversation_id, user_id, message)
         return False
 
     async def handle_questions(self):
         while True:
-            await asyncio.sleep(15.0)
-            handled_question = []
-            saved_questions = self.saved_questions.copy()
-            for user_id, question in saved_questions.items():
-                try:
-                    logger.info("++++++++handle question: %s", question.data)
-                    if await self.send_message_to_chat_gpt2(question.conversation_id, question.user_id, question.data):
-                        handled_question.append(user_id)
-                except Exception as e:
-                    logger.info("%s", str(e))
-                    continue
-            for question in handled_question:
-                del self.saved_questions[question]
+            try:
+                await asyncio.sleep(15.0)
+                handled_question = []
+                saved_questions = self.saved_questions.copy()
+                for user_id, question in saved_questions.items():
+                    try:
+                        logger.info("++++++++handle question: %s", question.data)
+                        if await self.send_message_to_chat_gpt2(question.conversation_id, question.user_id, question.data):
+                            handled_question.append(user_id)
+                    except Exception as e:
+                        logger.info("%s", str(e))
+                        continue
+                for question in handled_question:
+                    del self.saved_questions[question]
+            except asyncio.exceptions.CancelledError:
+                logger.info("++++handle_questions received CancelledError exception, exit..")
+                return
 
     def save_question(self, conversation_id, user_id, data):
         self.saved_questions[user_id] = SavedQuestion(conversation_id, user_id, data)
 
     async def handle_user_message(self, conversation_id, user_id, message):
         try:
             await self.send_message_to_chat_gpt(conversation_id, user_id, message)
+        except asyncio.exceptions.CancelledError:
+            logger.info("++++handle_group_message received CancelledError, exit...")
         except Exception as e:
             logger.exception(e)
             if self.developer_user_id:
                 await self.sendUserText(self.developer_conversation_id, self.developer_user_id, f"exception occur at:{time.time()}: {traceback.format_exc()}")
 
     async def get_web_result(self, message: str):
         date = datetime.now()
@@ -310,15 +301,18 @@
             href = a['href']
             querys.append(f'[{counter}] "{body}"')
             querys.append(f"Source: {href}")
         querys.append(f"\nCurrent date: {formatted_date}")
         querys.append(f"\nInstructions: Using the provided web search results, write a comprehensive reply to the given prompt. Make sure to cite results using [[number](URL)] notation after the reference. If the provided search results refer to multiple subjects with the same name, write separate answers for each subject.\nPrompt: {prompt}")
         return "\n".join(querys)
     async def handle_group_message(self, conversation_id, user_id, data):
-        await self.send_message_to_chat_gpt2(conversation_id, user_id, data)
+        try:
+            await self.send_message_to_chat_gpt2(conversation_id, user_id, data)
+        except asyncio.exceptions.CancelledError:
+            logger.info("++++handle_group_message received CancelledError, exit...")
 
     async def on_message(self, id: str, action: str, msg: Optional[MessageView]):
         if action not in ["ACKNOWLEDGE_MESSAGE_RECEIPT", "CREATE_MESSAGE", "LIST_PENDING_MESSAGES"]:
             logger.info("unknow action %s", action)
             return
 
         if action == "ACKNOWLEDGE_MESSAGE_RECEIPT":
@@ -366,33 +360,21 @@
         if utils.unique_conversation_id(msg.user_id, self.client_id) == msg.conversation_id:
             asyncio.create_task(self.handle_user_message(msg.conversation_id, msg.user_id, data))
         else:
             asyncio.create_task(self.handle_group_message(msg.conversation_id, msg.user_id, data))
 
     async def run(self):
         try:
-            while not self.paused:
-                try:
-                    await super().run()
-                except websockets.exceptions.ConnectionClosedError as e:
-                    logger.exception(e)
-                    await asyncio.sleep(3.0)
-                    self.ws = None
-                #asyncio.exceptions.TimeoutError
-                except Exception as e:
-#
-                    logger.exception(e)
-                    await asyncio.sleep(3.0)
-                    self.ws = None
+            await super().run()
         except asyncio.CancelledError:
             if self.ws:
                 await self.ws.close()
             if self.web_client:
                 await self.web_client.aclose()
-            logger.info("mixin websocket was cancelled!")
+            logger.info("mixin websocket received CancelledError, exit...")
 
     async def close(self):
         for bot in self.bots:
             await bot.close()
 
 bot: Optional[MixinBot]  = None
 
@@ -404,15 +386,19 @@
 async def start(config_file):
     global bot
     bot = MixinBot(config_file)
     await bot.init()
     asyncio.create_task(bot.run())
     print('started')
     while not bot.paused:
-        await asyncio.sleep(1.0)
+        try:
+            await asyncio.sleep(1.0)
+        except asyncio.CancelledError:
+            logger.info("+++start received CancelledError, exit...")
+            return
 
 async def stop():
     global bot
     await bot.ws.close()
 
 async def resume():
     global bot
```

### Comparing `chatgpt-mixin-0.1.7/src/test.py` & `chatgpt-mixin-0.1.8/src/test.py`

 * *Files identical despite different names*

