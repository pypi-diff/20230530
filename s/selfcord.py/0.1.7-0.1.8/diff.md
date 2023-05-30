# Comparing `tmp/selfcord.py-0.1.7.tar.gz` & `tmp/selfcord.py-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.1.7.tar", last modified: Mon May 15 14:34:36 2023, max compression
+gzip compressed data, was "selfcord.py-0.1.8.tar", last modified: Tue May 30 16:51:20 2023, max compression
```

## Comparing `selfcord.py-0.1.7.tar` & `selfcord.py-0.1.8.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.900771 selfcord.py-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-15 14:34:36.900771 selfcord.py-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.896771 selfcord.py-0.1.7/selfcord/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.896771 selfcord.py-0.1.7/selfcord/api/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    20670 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.896771 selfcord.py-0.1.7/selfcord/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/api/voice/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.900771 selfcord.py-0.1.7/selfcord/models/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/models/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.900771 selfcord.py-0.1.7/selfcord/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/utils/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/selfcord/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.896771 selfcord.py-0.1.7/selfcord.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-15 14:34:36.000000 selfcord.py-0.1.7/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-15 14:34:36.000000 selfcord.py-0.1.7/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:34:36.000000 selfcord.py-0.1.7/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-15 14:34:36.000000 selfcord.py-0.1.7/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 14:34:36.000000 selfcord.py-0.1.7/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 14:34:36.900771 selfcord.py-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:36.900771 selfcord.py-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-15 14:34:25.000000 selfcord.py-0.1.7/tests/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.278997 selfcord.py-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-30 16:51:20.278997 selfcord.py-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.274997 selfcord.py-0.1.8/selfcord/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.274997 selfcord.py-0.1.8/selfcord/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14582 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.274997 selfcord.py-0.1.8/selfcord/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/api/voice/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22236 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.278997 selfcord.py-0.1.8/selfcord/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21178 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.278997 selfcord.py-0.1.8/selfcord/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/selfcord/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.274997 selfcord.py-0.1.8/selfcord.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-30 16:51:20.000000 selfcord.py-0.1.8/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-30 16:51:20.000000 selfcord.py-0.1.8/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:51:20.000000 selfcord.py-0.1.8/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 16:51:20.000000 selfcord.py-0.1.8/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 16:51:20.000000 selfcord.py-0.1.8/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:51:20.278997 selfcord.py-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:51:20.278997 selfcord.py-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-30 16:51:08.000000 selfcord.py-0.1.8/tests/test_commands.py
```

### Comparing `selfcord.py-0.1.7/PKG-INFO` & `selfcord.py-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
@@ -23,15 +23,14 @@
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
-
  - Modern Pythonic API using `async`/`await` syntax
  - Easy to use with an object oriented design
  - Optimised for both speed and memory
  - Prevents detection of user account automation
  - Clean Documentation
  - Community Support
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.7 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.8 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown Provides-Extra: voice
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
```

### Comparing `selfcord.py-0.1.7/README.md` & `selfcord.py-0.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
-
  - Modern Pythonic API using `async`/`await` syntax
  - Easy to use with an object oriented design
  - Optimised for both speed and memory
  - Prevents detection of user account automation
  - Clean Documentation
  - Community Support
```

### Comparing `selfcord.py-0.1.7/selfcord/api/errors.py` & `selfcord.py-0.1.8/selfcord/api/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from __future__ import annotations
+
+
 class DiscordException(Exception):
     pass
 
+
 class LoginFailure(DiscordException):
     def __init__(self, message: dict, status: int) -> None:
         self.message = message
         self.status = status
 
+
 class ReconnectWebsocket(DiscordException):
-    def __init__(self, message: str) -> None: self.message = message
+    def __init__(self, message: str) -> None:
+        self.message = message
+
 
 class RuntimeError(DiscordException):
-    def __init__(self, message: str) -> None: self.message = message
+    def __init__(self, message: str) -> None:
+        self.message = message
+
 
 class Funnu(DiscordException):
-    def __init__(self, *args: object) -> None: super().__init__(*args)
+    def __init__(self, *args: object) -> None:
+        super().__init__(*args)
```

### Comparing `selfcord.py-0.1.7/selfcord/api/events.py` & `selfcord.py-0.1.8/selfcord/api/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,288 +1,327 @@
 from __future__ import annotations
+
+import asyncio
+import time
 from time import perf_counter
+from typing import TYPE_CHECKING
+
+from ..models import (Client, DMChannel, GroupChannel, Guild, Message,
+                      TextChannel, User, VoiceChannel)
 from ..models.role import Role
-from ..models import User, Client, Guild, TextChannel, VoiceChannel, DMChannel, GroupChannel, Message
-from aioconsole import aprint
-import asyncio
-from .voice import Voice
 from ..utils import logging
+from .voice import Voice
+
+if TYPE_CHECKING:
+    from ..bot import Bot
+    from .http import http
 
 log = logging.getLogger("Event")
 
+
 class EventHandler:
-    '''
+    """
     Used to handle discord events
-    '''
+    """
+
     def __init__(self, bot, http, debug=False):
         self._events = {}
-        self.http    = http
-        self.bot     = bot
-        self.debug = debug
+        self.http: http = http
+        self.bot: Bot = bot
+        self.debug: bool = debug
 
-    async def handle_ready(self, data: dict, user: Client, http):
+    async def handle_ready(self, data: dict, user: Client, http: http):
         """Handles what happens when the ready event is fired, when the bot first connects
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         self.user = user
-        for relationship in data.get('relationships'):
-            if relationship.get('type') == 1:
-                self.user.friends.append(User(relationship['user'], self.bot, http))
-
-        for channel in data.get('private_channels'):
-            if channel.get('type') == 1: self.user.private_channels.append(DMChannel(channel,self.bot, http))
-            if channel.get('type') == 3: self.user.private_channels.append(GroupChannel(channel, self.bot, http))
+        for relationship in data.get("relationships"):
+            if relationship.get("type") == 1:
+                self.user.friends.append(User(relationship["user"], self.bot, http))
+
+        for channel in data.get("private_channels"):
+            if channel.get("type") == 1:
+                self.user.private_channels.append(DMChannel(channel, self.bot, http))
+            if channel.get("type") == 3:
+                self.user.private_channels.append(GroupChannel(channel, self.bot, http))
 
-        for guild in data.get('guilds'):
+        for guild in data.get("guilds"):
             await self.handle_guild_create(guild, self.user, http)
-
+        self.bot.session_id = data.get("session_id")
+        self.bot.resume_url = data.get("resume_gateway_url")
         # Sends data from ready to the event handler in main.py (if it exists)
-        await self.bot.emit('ready', perf_counter() - self.bot.t1)
+        await self.bot.emit("ready", perf_counter() - self.bot.t1)
 
-    async def handle_guild_create(self, data: dict, user: Client, http):
+    async def handle_guild_create(self, data: dict, user: Client, http: http):
         """Handles what happens when a guild is created
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         self.user = user
         guild = Guild(data, self.bot, http)
         self.user.guilds.append(guild)
 
         # Sends data from ready to the event handler in main.py (if it exists)
-        await self.bot.emit('guild_create', guild)
+        await self.bot.emit("guild_create", guild)
 
-    async def handle_message_create(self, data: dict, user: Client, http):
+    async def handle_message_create(self, data: dict, user: Client, http: http):
         """Handles what happens when a message is created, or sent
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         self.user = user
         message = Message(data, self.bot, http)
         self.user.messages.append(message)
 
         # Sends data from ready to the event handler in main.py (if it exists)
-        await self.bot.emit('message', message)
+        await self.bot.emit("message", message)
         if not self.bot.userbot:
             if message.author.id == self.bot.user.id:
                 for prefix in self.bot.prefixes:
                     # Attempts to invoke the command if has prefix and from the user
-                    if message.content.startswith(prefix): await self.bot.process_commands(message)
+                    if message.content.startswith(prefix):
+                        await self.bot.process_commands(message)
         else:
             for prefix in self.bot.prefixes:
-                    # Attempts to invoke the command if has prefix
-                    if message.content.startswith(prefix): await self.bot.process_commands(message)
+                # Attempts to invoke the command if has prefix
+                if message.content.startswith(prefix):
+                    await self.bot.process_commands(message)
 
-
-    async def handle_message_delete(self, data: dict, user: Client, http):
+    async def handle_message_delete(self, data: dict, user: Client, http: http):
         """Handles what happens when a message is deleted. Very little data will be logged if the message is not in the bots cache.
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         self.user = user
-        id =data.get('id')
+        id = data.get("id")
         for message in self.user.messages:
             if message.id == id:
-                await self.bot.emit('message_delete', message)
+                setattr(message, "deleted_time", time.time())
+                await self.bot.emit("message_delete", message)
                 self.user.deleted_messages.append(message)
                 self.user.messages.remove(message)
-        else:
+        else:  # type: ignore
+
             class deleted_message:
                 def __init__(self, data) -> None:
-                    self.tts                = data.get('tts')
-                    self.references_message = data.get('referenced_message')
-                    self.mentions           = data.get('mentions')
-                    self.author             = None
-                    self.id                 = data.get('id')
-                    self.flags              = data.get('flags')
-                    self.embeds             = data.get('embeds')
-                    self.content            = data.get('content')
-                    self.components         = data.get('components')
-                    self.channel_id         = data.get('channel_id')
-                    self.attachments        = data.get('attachments')
-                    self.guild_id           = data.get('guild_id')
-                    self.channel            = None
-                    self.guild              = None
+                    self.tts = data.get("tts")
+                    self.references_message = data.get("referenced_message")
+                    self.mentions = data.get("mentions")
+                    self.author = None
+                    self.id = data.get("id")
+                    self.flags = data.get("flags")
+                    self.embeds = data.get("embeds")
+                    self.content = data.get("content")
+                    self.components = data.get("components")
+                    self.channel_id = data.get("channel_id")
+                    self.attachments = data.get("attachments")
+                    self.guild_id = data.get("guild_id")
+                    self.channel = None
+                    self.guild = None
+                    self.deleted_time = time.time()
 
             message = deleted_message(data)
-            await self.bot.emit('message_delete', message)
+            await self.bot.emit("message_delete", message)
 
-    async def handle_channel_create(self, channel: dict, user: Client, http):
+    async def handle_channel_create(self, channel: dict, user: Client, http: http):
         """Handles what happens when a channel is created
 
         Args:
             channel (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         self.user = user
-        if channel.get('type') == 0:
-            id = channel.get('guild_id')
+        if channel.get("type") == 0:
+            id = channel.get("guild_id")
             for guild in self.user.guilds:
                 if guild.id == id:
                     channel = TextChannel(channel, self.bot, self.http)
                     guild.channels.append(channel)
 
-        elif channel.get('type') == 1: self.user.private_channels.append(DMChannel(channel, self.bot, http))
+        elif channel.get("type") == 1:
+            self.user.private_channels.append(DMChannel(channel, self.bot, http))
 
-        elif channel.get('type') == 2:
-            id = channel.get('guild_id')
+        elif channel.get("type") == 2:
+            id = channel.get("guild_id")
             for guild in self.user.guilds:
                 if guild.id == id:
                     channel = VoiceChannel(channel, self.bot, self.http)
                     guild.channels.append(channel)
 
-        elif channel.get('type') == 3: self.user.private_channels.append(GroupChannel(channel, self.bot, http))
+        elif channel.get("type") == 3:
+            self.user.private_channels.append(GroupChannel(channel, self.bot, http))
 
         else:
-            id = channel.get('guild_id')
+            id = channel.get("guild_id")
             for guild in self.user.guilds:
                 if guild.id == id:
                     channel = TextChannel(channel, self.bot, self.http)
                     guild.channels.append(channel)
 
         # Sends data from ready to the event handler in main.py (if it exists)
-        await self.bot.emit('channel_create', channel)
+        await self.bot.emit("channel_create", channel)
 
-    async def handle_guild_member_list_update(self, data: dict, user: Client, http):
+    async def handle_guild_member_list_update(
+        self, data: dict, user: Client, http: http
+    ):
         """Handles what happens when a member chunk payload is received
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         self.user = user
         ops = []
-        data = data['ops']
+        data = data["ops"]
         for main in data:
-            op = main['op']
+            op = main["op"]
             ops.append(op)
 
         for main in data:
-            if ('INSERT' and 'DELETE') in ops:
+            if ("INSERT" and "DELETE") in ops:
                 try:
-                    person = User(main['item']['member']['user'], self.bot, self.http)
-                    await self.bot.emit('member_chunk', members=None, other=None, join=None, leave=person)
-                except: continue
-            elif 'INSERT' in ops:
+                    person = User(main["item"]["member"]["user"], self.bot, self.http)
+                    await self.bot.emit(
+                        "member_chunk",
+                        members=None,
+                        other=None,
+                        join=None,
+                        leave=person,
+                    )
+                except:
+                    continue
+            elif "INSERT" in ops:
                 try:
-                    person = User(main['item']['member']['user'], self.bot, self.http)
-                    await self.bot.emit('member_chunk', members=None, other=None, join=person, leave=None)
-                except: continue
-            elif 'UPDATE' in ops:
+                    person = User(main["item"]["member"]["user"], self.bot, self.http)
+                    await self.bot.emit(
+                        "member_chunk",
+                        members=None,
+                        other=None,
+                        join=person,
+                        leave=None,
+                    )
+                except:
+                    continue
+            elif "UPDATE" in ops:
                 try:
-                    person = User(main['item']['member']['user'], self.bot, self.http)
-                    await self.bot.emit('member_chunk', members=None, other=person, join=None, leave=None)
-                except: continue
-            elif 'SYNC' in ops:
-                users = [ ]
-                for item in main['items']:
+                    person = User(main["item"]["member"]["user"], self.bot, self.http)
+                    await self.bot.emit(
+                        "member_chunk",
+                        members=None,
+                        other=person,
+                        join=None,
+                        leave=None,
+                    )
+                except:
+                    continue
+            elif "SYNC" in ops:
+                users = []
+                for item in main["items"]:
                     try:
-                        users.append(User(item['member']['user'], self.bot, self.http))
-                    except: continue
-                await self.bot.emit('member_chunk', members=users, other=None, join=None, leave=None)
+                        users.append(User(item["member"]["user"], self.bot, self.http))
+                    except:
+                        continue
+                await self.bot.emit(
+                    "member_chunk", members=users, other=None, join=None, leave=None
+                )
 
-
-
-
-
-    async def handle_channel_delete(self, data, user: Client, http):
+    async def handle_channel_delete(self, data, user: Client, http: http):
         """Handles what happens when a channel is deleted
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         self.user = user
-        id = data.get('id')
+        id = data.get("id")
         for channel in self.user.private_channels:
             if channel.id == id:
-                await self.bot.emit('channel_delete', channel)
+                await self.bot.emit("channel_delete", channel)
                 self.user.private_channels.remove(channel)
                 return
 
-        guild_id = data.get('guild_id')
+        guild_id = data.get("guild_id")
         if guild_id != None:
             for guild in self.user.guilds:
                 if guild_id == guild.id:
                     for channel in guild.channels:
                         if channel.id == id:
-                            await self.bot.emit('channel_delete', channel)
+                            await self.bot.emit("channel_delete", channel)
                             guild.channels.remove(channel)
                             return
         else:
             for guild in self.user.guilds:
                 for channel in guild.channels:
                     if channel.id == id:
-                        await self.bot.emit('channel_delete', channel)
+                        await self.bot.emit("channel_delete", channel)
                         guild.channels.remove(channel)
                         return
 
-
-    async def handle_guild_role_create(self, role, user: Client, http):
+    async def handle_guild_role_create(self, role, user: Client, http: http):
         """Handles what happens when a role is created
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         self.user = user
 
         for guild in self.user.guilds:
-            if role.get('guild_id') == guild.id:
-                role = Role(role, self.http, guild_id=guild.id)
+            if role.get("guild_id") == guild.id:
+                role = Role(role, self.bot, self.http, guild_id=guild.id)
                 guild.roles.append(role)
 
-        await self.bot.emit('role_create', role)
+        await self.bot.emit("role_create", role)
 
-    async def handle_guild_role_delete(self, role: dict, user: Client, http):
+    async def handle_guild_role_delete(self, role: dict, user: Client, http: http):
         """Handles what happens when a role is deleted
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         self.user = user
 
         for guild in self.user.guilds:
-            if role.get('guild_id') == guild.id:
+            if role.get("guild_id") == guild.id:
                 for role in guild.roles:
-                    if role.get('id') == role.id:
-                        await self.bot.emit('role_delete', role)
+                    if role.get("id") == role.id:
+                        await self.bot.emit("role_delete", role)
                         guild.roles.remove(role)
                         return
 
-
-    async def handle_voice_state_update(self, data: dict, user: Client, http):
+    async def handle_voice_state_update(self, data: dict, user: Client, http: http):
         """Handles the voice state updating
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
-        if data['channel_id'] != None:
-            self.session_id = data['session_id']
+        if data["channel_id"] != None:
+            self.session_id = data["session_id"]
 
-    async def handle_presence_update(self, data: dict, user: Client, http):
+    async def handle_presence_update(self, data: dict, user: Client, http: http):
         """Handles the presence updating
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
@@ -312,40 +351,44 @@
                     type = "STREAMING"
                 elif type == WATCHING:
                     type == "WATCHING"
                 elif type == 4:
                     type = "CUSTOM"
                 activities.append({"Type": type, "Name": activity.get("name")})
 
-        await self.bot.emit('presence_update', user, status, last_modified, client_status, activities)
+        await self.bot.emit(
+            "presence_update", user, status, last_modified, client_status, activities
+        )
 
-    async def handle_voice_server_update(self, data: dict, user: Client, http):
+    async def handle_voice_server_update(self, data: dict, user: Client, http: http):
         """Handles the voice server updating
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
-        self.token = data['token']
-        self.endpoint = data['endpoint']
-        if data['guild_id'] != None:
-            self.server_id = data['guild_id']
+        self.token = data["token"]
+        self.endpoint = data["endpoint"]
+        if data["guild_id"] != None:
+            self.server_id = data["guild_id"]
         else:
-            self.server_id = data['channel_id']
+            self.server_id = data["channel_id"]
         await asyncio.sleep(1)
-        self.voice = Voice(self.session_id, self.token, self.endpoint, self.server_id, self.bot, debug=self.debug)
+        self.voice = Voice(
+            self.session_id,
+            self.token,
+            self.endpoint,
+            self.server_id,
+            self.bot,
+            debug=self.debug,
+        )
         await self.voice_start(self.voice)
 
     async def voice_start(self, voice: Voice):
         asyncio.create_task(voice.start())
         setattr(self.bot, "voice", self.voice)
         if self.debug:
             log.debug("Voice attribute created")
-            log.info(f"Created voice attribute with Session ID: {self.session_id} Endpoint: {self.endpoint}")
-
-
-
-
-
-
-
+            log.info(
+                f"Created voice attribute with Session ID: {self.session_id} Endpoint: {self.endpoint}"
+            )
```

### Comparing `selfcord.py-0.1.7/selfcord/api/gateway.py` & `selfcord.py-0.1.8/selfcord/api/gateway.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 from __future__ import annotations
+
 import asyncio
-import websockets
 import json
 import os
 import time
 import zlib
-from .events import EventHandler
-from .errors import ReconnectWebsocket
-from selfcord.models.client import Client
-import requests
 from traceback import format_exception
+
+import requests
+import websockets
+
+from selfcord.models.client import Client
+
 from ..utils import logging
+from .errors import ReconnectWebsocket
+from .events import EventHandler
 
 log = logging.getLogger("Gateway")
 
+
 class Activity:
     @staticmethod
-    def Game(name: str, details: str, state: str, buttons: dict, application_id: str, key: str) -> dict[str, int]:
+    def Game(
+        name: str,
+        details: str,
+        state: str,
+        buttons: dict,
+        application_id: str,
+        key: str,
+    ) -> dict[str, int]:
         """Method to generate activity dict for the "Playing ..." payload
 
         Args:
             name (str): Name of the activity
             details (str): Details of the activity
             state (str): State of the activity
             buttons (dict): Buttons for the activity.
@@ -31,19 +43,20 @@
 
         Returns:
             dict[str, int]: Dict for the activity object for payload
         """
         type = 0
         button_urls = [button for button in buttons.values()]
         buttons: list = [button for button in buttons.keys()]
-        req = requests.get(f"https://discordapp.com/api/oauth2/applications/{application_id}/assets")
+        req = requests.get(
+            f"https://discordapp.com/api/oauth2/applications/{application_id}/assets"
+        )
         for item in req.json():
-
-            if item['name'] == key:
-                key = item['id']
+            if item["name"] == key:
+                key = item["id"]
 
         if len(button_urls) == 0 or len(buttons) == 0:
             payload = {
                 "name": name,
                 "details": details,
                 "state": state,
                 "application_id": application_id,
@@ -63,22 +76,29 @@
                 "application_id": application_id,
                 "assets": {
                     "large_image": key,
                 },
                 "metadata": {
                     "button_urls": button_urls,
                 },
-                "created_at": int(time.time())
+                "created_at": int(time.time()),
             }
 
-
         return payload
 
     @staticmethod
-    def Stream(name: str, details: str, state: str, url: str, buttons: dict, application_id: str, key: str) -> dict[str, int] :
+    def Stream(
+        name: str,
+        details: str,
+        state: str,
+        url: str,
+        buttons: dict,
+        application_id: str,
+        key: str,
+    ) -> dict[str, int]:
         """Method to generate activity dict for the "Streaming ..." payload
 
         Args:
             name (str): Name of the activity
             details (str): Details of the activity
             state (str): State of the activitiy
             url (str): URL for streaming
@@ -90,32 +110,33 @@
 
         Returns:
             dict[str, int]: Dict for the activity object for payload
         """
         type = 1
         button_urls = [button for button in buttons.values()]
         buttons: list = [button for button in buttons.keys()]
-        req = requests.get(f"https://discordapp.com/api/oauth2/applications/{application_id}/assets")
+        req = requests.get(
+            f"https://discordapp.com/api/oauth2/applications/{application_id}/assets"
+        )
         for item in req.json():
-
-            if item['name'] == key:
-                key = item['id']
+            if item["name"] == key:
+                key = item["id"]
 
         if len(button_urls) == 0 or len(buttons) == 0:
             payload = {
                 "name": name,
                 "details": details,
                 "type": type,
                 "state": state,
                 "application_id": application_id,
                 "assets": {
                     "large_image": key,
                 },
                 "created_at": int(time.time()),
-                "url": url
+                "url": url,
             }
         else:
             payload = {
                 "name": name,
                 "details": details,
                 "type": type,
                 "buttons": buttons,
@@ -124,21 +145,28 @@
                 "application_id": application_id,
                 "assets": {
                     "large_image": key,
                 },
                 "metadata": {
                     "button_urls": button_urls,
                 },
-                "created_at": int(time.time())
+                "created_at": int(time.time()),
             }
 
         return payload
 
     @staticmethod
-    def Listen(name: str, details: str, state: str, buttons: dict, application_id: str, key: str ) -> dict[str, int]:
+    def Listen(
+        name: str,
+        details: str,
+        state: str,
+        buttons: dict,
+        application_id: str,
+        key: str,
+    ) -> dict[str, int]:
         """Method to generate activity dict for the "Listening ..." payload
 
         Args:
             name (str): Name of the activity
             details (str): Details of the activity
             state (str): State of the activity
             buttons (dict): Buttons for the activity.
@@ -149,19 +177,20 @@
 
         Returns:
             dict[str, int]: Dict for the activity object for payload
         """
         type = 2
         button_urls = [button for button in buttons.values()]
         buttons: list = [button for button in buttons.keys()]
-        req = requests.get(f"https://discordapp.com/api/oauth2/applications/{application_id}/assets")
+        req = requests.get(
+            f"https://discordapp.com/api/oauth2/applications/{application_id}/assets"
+        )
         for item in req.json():
-
-            if item['name'] == key:
-                key = item['id']
+            if item["name"] == key:
+                key = item["id"]
 
         if len(button_urls) == 0 or len(buttons) == 0:
             payload = {
                 "name": name,
                 "details": details,
                 "state": state,
                 "application_id": application_id,
@@ -181,21 +210,28 @@
                 "application_id": application_id,
                 "assets": {
                     "large_image": key,
                 },
                 "metadata": {
                     "button_urls": button_urls,
                 },
-                "created_at": int(time.time())
+                "created_at": int(time.time()),
             }
 
-
         return payload
+
     @staticmethod
-    def Watch(name: str, details: str, state: str, buttons: dict, application_id: str, key: str ) -> dict[str, int]:
+    def Watch(
+        name: str,
+        details: str,
+        state: str,
+        buttons: dict,
+        application_id: str,
+        key: str,
+    ) -> dict[str, int]:
         """Method to generate activity dict for the "Watching ..." payload
 
         Args:
             name (str): Name of the activity
             details (str): Details of the activity
             state (str): State of the activity
             buttons (dict): Buttons for the activity.
@@ -208,19 +244,20 @@
             dict[str, int]: Dict for the activity object for payload
         """
         type = 3
 
         button_urls = [button for button in buttons.values()]
         buttons: list = [button for button in buttons.keys()]
 
-        req = requests.get(f"https://discordapp.com/api/oauth2/applications/{application_id}/assets")
+        req = requests.get(
+            f"https://discordapp.com/api/oauth2/applications/{application_id}/assets"
+        )
         for item in req.json():
-
-            if item['name'] == key:
-                key = item['id']
+            if item["name"] == key:
+                key = item["id"]
 
         if len(button_urls) == 0 or len(buttons) == 0:
             payload = {
                 "name": name,
                 "details": details,
                 "state": state,
                 "application_id": application_id,
@@ -240,263 +277,286 @@
                 "application_id": application_id,
                 "assets": {
                     "large_image": key,
                 },
                 "metadata": {
                     "button_urls": button_urls,
                 },
-                "created_at": int(time.time())
+                "created_at": int(time.time()),
             }
 
-
         return payload
 
 
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from zlib import _Decompress
+
+    from .http import http
+
 
 class gateway:
-    ''' OP CODES '''
-    DISPATCH           = 0
-    HEARTBEAT          = 1
-    IDENTIFY           = 2
-    PRESENCE           = 3
-    VOICE_STATE        = 4
-    VOICE_PING         = 5
-    RESUME             = 6
-    RECONNECT          = 7
-    REQUEST_MEMBERS    = 8
+    """Discord Gateway instance, used to initialise gateway connections"""
+
+    DISPATCH = 0
+    HEARTBEAT = 1
+    IDENTIFY = 2
+    PRESENCE = 3
+    VOICE_STATE = 4
+    VOICE_PING = 5
+    RESUME = 6
+    RECONNECT = 7
+    REQUEST_MEMBERS = 8
     INVALIDATE_SESSION = 9
-    HELLO              = 10
-    HEARTBEAT_ACK      = 11
-    GUILD_SYNC         = 12
-
-    def __init__(self, http, debug=False):
-        self.debug = debug
-        self.http = http
-        self.zlib = zlib.decompressobj()
-        self.zlib_suffix = b'\x00\x00\xff\xff'
-        self.last_ack = time.perf_counter()
-        self.last_send = time.perf_counter()
-        self.latency = float('inf')
+    HELLO = 10
+    HEARTBEAT_ACK = 11
+    GUILD_SYNC = 12
+
+    def __init__(self, http: http, debug: bool = False):
+        self.debug: bool = debug
+        self.http: http = http
+        self.zlib: _Decompress = zlib.decompressobj()
+        self.zlib_suffix: bytes = b"\x00\x00\xff\xff"
+        self.last_ack: float = time.perf_counter()
+        self.last_send: float = time.perf_counter()
+        self.latency = float("inf")
+        self.resume_url = None
         self.alive = False
 
     async def recv_msg(self):
-        '''
+        """
         Receives Message from gateway, encodes as json and does things depending on op code
-        '''
+        """
         item = await self.ws.recv()
         buffer = bytearray()
         buffer.extend(item)
-        if len(item) < 4 or item[-4:] != self.zlib_suffix: return
+        if len(item) < 4 or item[-4:] != self.zlib_suffix:
+            return
 
         if item:
-            item    = self.zlib.decompress(item)
-            item    = json.loads(item) # Get json message from gateway
-
-            op      = item.get('op') # Op code
-            data    = item.get('d') # Data
-            event   = item.get('t') # The event
-
+            item = self.zlib.decompress(item)
+            item = json.loads(item)  # Get json message from gateway
 
-            if  op == self.RECONNECT:
-                await self.close()
+            op = item.get("op")  # Op code
+            data = item.get("d")  # Data
+            event = item.get("t")  # The event
+            s = item.get("s")
+            if op == self.RECONNECT:
+                await self.reconnect(s)
                 log.error("Reconnect websocket")
 
             elif op == self.INVALIDATE_SESSION:
                 if data:
                     await self.close()
                     log.error("Session Invalidated")
 
             elif op == self.HELLO:
                 # Begins heartbeat and sends identify if this op is received
-                interval = data['heartbeat_interval'] / 1000.0
+                interval = data["heartbeat_interval"] / 1000.0
                 await self.identify()
                 asyncio.create_task(self.heartbeat(interval))
 
             elif op == self.HEARTBEAT_ACK:
                 await self.heartbeat_ack()
 
             elif op == self.DISPATCH:
                 # If op is 0 it signifies a regular gateway event
                 # These events are discord events like message_create, role_create whatever.
 
-                handle = f'handle_{event.lower()}'
-
-
-                if hasattr(self.handler, handle): # If the event handler exists, so e.g handle_ready
-                    method = getattr(self.handler,handle)
+                handle = f"handle_{event.lower()}"
 
-                    val = await asyncio.gather(asyncio.create_task(method(data, self.user, self.http)), return_exceptions=True) # A background task is created to run the handler
+                if hasattr(
+                    self.handler, handle
+                ):  # If the event handler exists, so e.g handle_ready
+                    method = getattr(self.handler, handle)
+
+                    val = await asyncio.gather(
+                        asyncio.create_task(method(data, self.user, self.http)),
+                        return_exceptions=True,
+                    )  # A background task is created to run the handler
                     for item in val:
-                        if item == None: break
-                        else: await self.bot.emit('error', item)
+                        if item == None:
+                            break
+                        else:
+                            await self.bot.emit("error", item)
 
                     # asyncio.create_task(method(data, self.user, self.http))
                 # Handlers are all situated in events.py
 
-
     def roundup(self, n):
         import math
+
         return int(math.ceil(n / 100.0)) * 100
 
     def chunks(self, lst, n):
         for i in range(0, len(lst), 1):
-            if len(lst[:i+1]) > 3:
-                for i in range(i, len(lst), n): yield lst[i:i + n]
+            if len(lst[: i + 1]) > 3:
+                for i in range(i, len(lst), n):
+                    yield lst[i : i + n]
                 break
 
-            yield lst[:i+1]
+            yield lst[: i + 1]
 
     async def change_presence(self, status: str, afk: bool, activity: dict):
         """Change the clients current presence
 
         Args:
             status (str): online, offline or dnd
             afk (bool): Whether client is set as AFK
             activity (Activity): Activity object
         """
         payload = {
             "op": 3,
-            "d" : {
+            "d": {
                 "since": time.time(),
                 "activities": [activity],
                 "status": status.lower(),
-                "afk": afk
+                "afk": afk,
             },
         }
 
         await self.send_json(payload)
         if self.debug:
             log.debug("Began rich presence")
             log.info(f"{activity}")
 
-
-
     async def lazy_chunk(self, guild_id: str, channel_id: str, amount: int):
-        '''Sends lazy guild request to gather current online members
+        """Sends lazy guild request to gather current online members
 
         Args:
             guild_id (str): The guild id specified
             channel_id (str): The channel id specified
-        '''
+        """
 
         ranges = []
 
         for i in range(0, amount, 100):
-            ranges.append([i, self.roundup(i + (amount - i)) - 1]) if i + 99 > amount else ranges.append([i, i+99])
+            ranges.append(
+                [i, self.roundup(i + (amount - i)) - 1]
+            ) if i + 99 > amount else ranges.append([i, i + 99])
 
         for item in self.chunks(ranges, 3):
             payload = {
-                'op': 14,
-                'd': {
-                    'guild_id': guild_id,
-                    'typing': True,
-                    'channels': {channel_id:item}
-                }
+                "op": 14,
+                "d": {
+                    "guild_id": guild_id,
+                    "typing": True,
+                    "channels": {channel_id: item},
+                },
             }
 
             await self.send_json(payload)
+            await asyncio.sleep(2.0)
 
         if self.debug:
             log.debug("Finished guild lazy chunking")
             log.info(f"Subscription to GUILD: {guild_id} with CHANNEL: {channel_id}")
 
-
     async def send_json(self, payload: dict):
-        '''Send json to the gateway
+        """Send json to the gateway
 
         Args:
             payload (dict): Valid payload to send to the gateway
-        '''
+        """
         await self.ws.send(json.dumps(payload))
 
+    async def reconnect(self, seq: int):
+        """Reconnect to discord gateway"""
+        print(self.bot.resume_url)
+        self.ws = await websockets.connect(
+            f"{self.bot.resume_url}?encoding=json&v=9&compress=zlib-stream"
+        )
+        payload = {
+            "op": 6,
+            "d": {"token": self.token, "session_id": self.bot.session_id, "seq": seq},
+        }
+        await self.send_json(payload)
+
     async def connect(self):
-        '''Connect to discord gateway
-        '''
-        self.ws = await websockets.connect('wss://gateway.discord.gg/?encoding=json&v=9&compress=zlib-stream', origin='https://discord.com', max_size=None)
+        """Connect to discord gateway"""
+        self.ws = await websockets.connect(
+            "wss://gateway.discord.gg/?encoding=json&v=9&compress=zlib-stream",
+            origin="https://discord.com",
+            max_size=None,
+        )
         self.alive = True
         if self.debug:
             log.debug("Established connection to Discord Gateway")
 
     async def close(self):
-        '''Close the connection to discord gateway
-        '''
-        self.alive= False
+        """Close the connection to discord gateway"""
+        self.alive = False
         await self.ws.close()
         if self.debug:
             log.debug("Closed connection to discord gateway")
 
     async def identify(self):
-        '''Identify to gateway, uses amazing mobile client spoof
-        '''
+        """Identify to gateway, uses amazing mobile client spoof"""
         payload = {
-            'op': 2,
-            'd': {
-                'token': self.token,
-                'properties': {
-                    '$os': 'android',
-                    '$browser': 'Discord Android',
-                    '$device': 'Discord Android',
-                    '$referrer': '',
-                    '$referring_domain': ''
+            "op": 2,
+            "d": {
+                "token": self.token,
+                "properties": {
+                    "$os": "android",
+                    "$browser": "Discord Android",
+                    "$device": "Discord Android",
+                    "$referrer": "",
+                    "$referring_domain": "",
                 },
-            }
+            },
         }
         await self.send_json(payload)
         if self.debug:
             log.debug("Sent identify payload")
             log.info(f"Idenitified with {self.token} under Discord Android")
 
-
-
     async def heartbeat(self, interval):
-        '''Heartbeat for gateway to maintain connection
+        """Heartbeat for gateway to maintain connection
 
         Args:
             interval (int): Interval between sends
-        '''
-        log.info(f'Hearbeat loop has began with the interval of {interval} seconds!')
-        heartbeatJSON = {
-            'op': 1,
-            'd': time.time()
-        }
+        """
+        log.info(f"Hearbeat loop has began with the interval of {interval} seconds!")
+        heartbeatJSON = {"op": 1, "d": time.time()}
         while True:
             await asyncio.sleep(interval)
             await self.send_json(heartbeatJSON)
             self.last_send = time.perf_counter()
             if self.debug:
-                log.debug('Sent heartbeat')
+                log.debug("Sent heartbeat")
                 log.info(f"Delay since last heartbeat {self.latency:0.2f}ms")
 
     async def heartbeat_ack(self):
-        '''Whenever heartbeat ack is sent, logs the time between last send of heartbeat json and receive of the ack
-        '''
+        """Whenever heartbeat ack is sent, logs the time between last send of heartbeat json and receive of the ack"""
         self.last_ack = time.perf_counter()
         self.latency = self.last_ack - self.last_send
 
     async def start(self, token: str, user: Client, bot):
-        '''Start discord gateway connection
+        """Start discord gateway connection
 
         Args:
             token (str): User token
             user (Client): User client
             bot (_type_): Bot class
-        '''
+        """
         self.handler = EventHandler(bot, self.http, self.debug)
         self.bot = bot
 
-        await self.bot.inbuilt_commands() # In built commands very cool
+        await self.bot.inbuilt_commands()  # In built commands very cool
 
         self.user = user
         self.token = token
 
         await self.connect()
         while self.alive:
-            try: await self.recv_msg()
+            try:
+                await self.recv_msg()
             except KeyboardInterrupt:
-                log.critical('Shutting down...')
+                log.critical("Shutting down...")
                 await self.close()
             except Exception as e:
                 error = "".join(format_exception(e, e, e.__traceback__))
                 await self.bot.emit("error", error)
                 if self.debug:
                     log.error(f"Websocket Unexpectedly closed\n{error}")
                 await self.close()
@@ -513,26 +573,29 @@
             "d": {
                 "guild_id": guild,
                 "channel_id": channel,
                 "preferred_region": "rotterdam",
                 "self_mute": False,
                 "self_deaf": False,
                 "self_video": True,
-            }
+            },
         }
         await self.send_json(payload)
         if self.debug:
             log.debug("Initiated video call")
             log.info(f"Began video call to GUILD: {guild} and CHANNEL: {channel}")
         if guild == None:
-            await self.http.request(method="post", endpoint=f"/channels/{channel}/call/ring",json={"recipients":None})
+            await self.http.request(
+                method="post",
+                endpoint=f"/channels/{channel}/call/ring",
+                json={"recipients": None},
+            )
             if self.debug:
                 log.debug("Sent Ring")
 
-
     async def call(self, channel: str, guild=None):
         """Initiates a discord call
 
         Args:
             channel (str): Channel ID
             guild (str, optional): Guild ID. Defaults to None.
         """
@@ -541,109 +604,91 @@
             "d": {
                 "guild_id": guild,
                 "channel_id": channel,
                 "preferred_region": "rotterdam",
                 "self_mute": False,
                 "self_deaf": False,
                 "self_video": False,
-            }
+            },
         }
         await self.send_json(payload)
         if self.debug:
             log.debug("Initiated call")
             log.info(f"Began call to GUILD: {guild} and CHANNEL: {channel}")
         if guild == None:
-            await self.http.request(method="post", endpoint=f"/channels/{channel}/call/ring",json={"recipients":None})
+            await self.http.request(
+                method="post",
+                endpoint=f"/channels/{channel}/call/ring",
+                json={"recipients": None},
+            )
             if self.debug:
                 log.debug("Sent Ring")
 
-
-
     async def stream_call(self, channel: str, guild=None):
         """Initiates a discord stream call
 
         Args:
             channel (str): Channel ID
             guild (str, optional): Guild ID. Defaults to None.
         """
         type = "guild" if guild != None else "call"
         payload = {
             "op": 18,
             "d": {
                 "guild_id": guild,
                 "channel_id": channel,
                 "preferred_region": "rotterdam",
-                "type": type
-            }
+                "type": type,
+            },
         }
         await self.send_json(payload)
         if self.debug:
             log.debug("Initiated call")
             log.info(f"Began call to GUILD: {guild} and CHANNEL: {channel}")
         if guild == None:
-
-            await self.http.request(method="post", endpoint=f"/channels/{channel}/call/ring",json={"recipients":None})
+            await self.http.request(
+                method="post",
+                endpoint=f"/channels/{channel}/call/ring",
+                json={"recipients": None},
+            )
 
             payload = {
                 "op": 22,
-                "d": {
-                    "stream_key": f"call:{channel}:{self.user.id}",
-                    "paused": False
-                }
+                "d": {"stream_key": f"call:{channel}:{self.user.id}", "paused": False},
             }
             if self.debug:
                 log.debug("Initiated streaming")
                 log.info(f"Began stream to CHANNEL: {channel}")
         else:
             payload = {
                 "op": 22,
                 "d": {
                     "stream_key": f"guild:{guild}:{channel}:{self.user.id}",
-                    "paused": False
-                }
+                    "paused": False,
+                },
             }
             if self.debug:
                 log.debug("Initiated streaming")
                 log.info(f"Began stream to GUILD: {guild} and CHANNEL: {channel}")
 
         await self.send_json(payload)
 
-
-
-
     async def leave_call(self):
-        """Leaves a discord call
-        """
+        """Leaves a discord call"""
         payload = {
             "op": 4,
             "d": {
                 "guild_id": None,
                 "channel_id": None,
                 "self_mute": False,
                 "self_deaf": False,
                 "self_video": False,
-            }
+            },
         }
         await self.send_json(payload)
         if self.debug:
             log.debug("Left Voice call")
         if hasattr(self.bot, "voice"):
             await self.bot.voice.close()
             delattr(self.bot, "voice")
         if self.debug:
             log.info("Voice attribute for bot has been deleted")
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
```

### Comparing `selfcord.py-0.1.7/selfcord/api/http.py` & `selfcord.py-0.1.8/selfcord/api/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,136 +1,162 @@
 from __future__ import annotations
-from aiohttp import ClientSession
-from aioconsole import aprint
+
 import asyncio
+import random
 from base64 import b64encode
+from traceback import format_exception
+from typing import TYPE_CHECKING
+
 import aiohttp
-from selfcord.api.errors import LoginFailure
-import random
-from ..models import User, Client
+from aiohttp import ClientSession
+
+from ..models import Client, User
 from ..utils import logging
-from traceback import format_exception
 
 log = logging.getLogger("HTTP")
+
+
 class http:
-    def __init__(self, debug = False) -> None:
+    """Base HTTP class to aid making requests via discord api"""
+
+    def __init__(self, debug=False) -> None:
         self.debug = debug
-        xproperties = ['eyJvcyI6IldpbmRvd3MiLCJicm93c2VyIjoiRmlyZWZveCIsImRldmljZSI6IiIsInN5c3RlbV9sb2NhbGUiOiJmciIsImJyb3dzZXJfdXNlcl9hZ2VudCI6Ik1vemlsbGEvNS4wIChXaW5kb3dzIE5UIDEwLjA7IFdpbjY0OyB4NjQ7IHJ2OjEwMi4wKSBHZWNrby8yMDEwMDEwMSBGaXJlZm94LzEwMi4wIiwiYnJvd3Nlcl92ZXJzaW9uIjoiMTAyLjAiLCJvc192ZXJzaW9uIjoiMTAiLCJyZWZlcnJlciI6IiIsInJlZmVycmluZ19kb21haW4iOiIiLCJyZWZlcnJlcl9jdXJyZW50IjoiIiwicmVmZXJyaW5nX2RvbWFpbl9jdXJyZW50IjoiIiwicmVsZWFzZV9jaGFubmVsIjoic3RhYmxlIiwiY2xpZW50X2J1aWxkX251bWJlciI6MTU0MTg2LCJjbGllbnRfZXZlbnRfc291cmNlIjpudWxsfQ==', 'eyJvcyI6IkxpbnV4IiwiYnJvd3NlciI6IkRpc2NvcmQgQ2xpZW50IiwicmVsZWFzZV9jaGFubmVsIjoiY2FuYXJ5IiwiY2xpZW50X3ZlcnNpb24iOiIwLjAuMTQwIiwib3NfdmVyc2lvbiI6IjUuMTkuMC0zLXJ0MTAtTUFOSkFSTyIsIm9zX2FyY2giOiJ4NjQiLCJzeXN0ZW1fbG9jYWxlIjoiZW4tR0IiLCJ3aW5kb3dfbWFuYWdlciI6IktERSx1bmtub3duIiwiZGlzdHJvIjoiXCJNYW5qYXJvIExpbnV4XCIiLCJjbGllbnRfYnVpbGRfbnVtYmVyIjoxNTQyMTYsImNsaWVudF9ldmVudF9zb3VyY2UiOm51bGx9', 'eyJvcyI6IkxpbnV4IiwiYnJvd3NlciI6IkNocm9tZSIsImRldmljZSI6IiIsInN5c3RlbV9sb2NhbGUiOiJlbi1HQiIsImJyb3dzZXJfdXNlcl9hZ2VudCI6Ik1vemlsbGEvNS4wIChYMTE7IExpbnV4IHg4Nl82NCkgQXBwbGVXZWJLaXQvNTM3LjM2IChLSFRNTCwgbGlrZSBHZWNrbykgQ2hyb21lLzEwNi4wLjAuMCBTYWZhcmkvNTM3LjM2IiwiYnJvd3Nlcl92ZXJzaW9uIjoiMTA2LjAuMC4wIiwib3NfdmVyc2lvbiI6IiIsInJlZmVycmVyIjoiaHR0cHM6Ly93d3cucm9ibG94LmNvbS8iLCJyZWZlcnJpbmdfZG9tYWluIjoid3d3LnJvYmxveC5jb20iLCJyZWZlcnJlcl9jdXJyZW50IjoiIiwicmVmZXJyaW5nX2RvbWFpbl9jdXJyZW50IjoiIiwicmVsZWFzZV9jaGFubmVsIjoic3RhYmxlIiwiY2xpZW50X2J1aWxkX251bWJlciI6MTU0MTg2LCJjbGllbnRfZXZlbnRfc291cmNlIjpudWxsfQ==']
-        self.cookies        = {}
-        self.token          = None
-        self.xproperties    = random.choice(xproperties)
-        self.base_url       = 'https://discord.com/api/v9'
+        xproperties = [
+            "eyJvcyI6IldpbmRvd3MiLCJicm93c2VyIjoiRmlyZWZveCIsImRldmljZSI6IiIsInN5c3RlbV9sb2NhbGUiOiJmciIsImJyb3dzZXJfdXNlcl9hZ2VudCI6Ik1vemlsbGEvNS4wIChXaW5kb3dzIE5UIDEwLjA7IFdpbjY0OyB4NjQ7IHJ2OjEwMi4wKSBHZWNrby8yMDEwMDEwMSBGaXJlZm94LzEwMi4wIiwiYnJvd3Nlcl92ZXJzaW9uIjoiMTAyLjAiLCJvc192ZXJzaW9uIjoiMTAiLCJyZWZlcnJlciI6IiIsInJlZmVycmluZ19kb21haW4iOiIiLCJyZWZlcnJlcl9jdXJyZW50IjoiIiwicmVmZXJyaW5nX2RvbWFpbl9jdXJyZW50IjoiIiwicmVsZWFzZV9jaGFubmVsIjoic3RhYmxlIiwiY2xpZW50X2J1aWxkX251bWJlciI6MTU0MTg2LCJjbGllbnRfZXZlbnRfc291cmNlIjpudWxsfQ==",
+            "eyJvcyI6IkxpbnV4IiwiYnJvd3NlciI6IkRpc2NvcmQgQ2xpZW50IiwicmVsZWFzZV9jaGFubmVsIjoiY2FuYXJ5IiwiY2xpZW50X3ZlcnNpb24iOiIwLjAuMTQwIiwib3NfdmVyc2lvbiI6IjUuMTkuMC0zLXJ0MTAtTUFOSkFSTyIsIm9zX2FyY2giOiJ4NjQiLCJzeXN0ZW1fbG9jYWxlIjoiZW4tR0IiLCJ3aW5kb3dfbWFuYWdlciI6IktERSx1bmtub3duIiwiZGlzdHJvIjoiXCJNYW5qYXJvIExpbnV4XCIiLCJjbGllbnRfYnVpbGRfbnVtYmVyIjoxNTQyMTYsImNsaWVudF9ldmVudF9zb3VyY2UiOm51bGx9",
+            "eyJvcyI6IkxpbnV4IiwiYnJvd3NlciI6IkNocm9tZSIsImRldmljZSI6IiIsInN5c3RlbV9sb2NhbGUiOiJlbi1HQiIsImJyb3dzZXJfdXNlcl9hZ2VudCI6Ik1vemlsbGEvNS4wIChYMTE7IExpbnV4IHg4Nl82NCkgQXBwbGVXZWJLaXQvNTM3LjM2IChLSFRNTCwgbGlrZSBHZWNrbykgQ2hyb21lLzEwNi4wLjAuMCBTYWZhcmkvNTM3LjM2IiwiYnJvd3Nlcl92ZXJzaW9uIjoiMTA2LjAuMC4wIiwib3NfdmVyc2lvbiI6IiIsInJlZmVycmVyIjoiaHR0cHM6Ly93d3cucm9ibG94LmNvbS8iLCJyZWZlcnJpbmdfZG9tYWluIjoid3d3LnJvYmxveC5jb20iLCJyZWZlcnJlcl9jdXJyZW50IjoiIiwicmVmZXJyaW5nX2RvbWFpbl9jdXJyZW50IjoiIiwicmVsZWFzZV9jaGFubmVsIjoic3RhYmxlIiwiY2xpZW50X2J1aWxkX251bWJlciI6MTU0MTg2LCJjbGllbnRfZXZlbnRfc291cmNlIjpudWxsfQ==",
+        ]
+        self.cookies = {}
+        self.token = None
+        self.xproperties = random.choice(xproperties)
+        self.base_url = "https://discord.com/api/v9"
 
     async def static_login(self, token: str):
-        '''Used to retrieve basic token information
+        """Used to retrieve basic token information
 
         Args:
             token (str): User token
 
         Returns:
             Client: A Client object
-        '''
+        """
         await self.get_cookie()
         self.token = token
-        data = await self.request('get', '/users/@me')
+        data = await self.request("get", "/users/@me")
         self.client = Client(data)
         if self.debug:
             log.debug("Finished Static login")
             log.info(f"Gathered information on {self.client}")
         return data
 
     async def get_cookie(self):
-        """Gather cookie for user upon client start
-        """
+        """Gather cookie for user upon client start"""
         async with aiohttp.ClientSession() as session:
-            async with session.get('https://discord.com', headers={'user-agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) discord/0.0.139 Chrome/91.0.4472.164 Electron/13.6.6 Safari/537.36'}) as resp:
-                dcf = resp.headers['set-cookie'].split('__dcfduid=')[0].split(';')[0]
-                sdc = resp.headers['set-cookie'].split('__sdcfduid=')[0].split(';')[0]
-                cfr = resp.headers['set-cookie'].split('__cfruid=')[0].split(';')[0]
-
-                self.cookies['dcf'] = self.cookies.get('dcf') if dcf != "" else ""
-                self.cookies['sdc'] = self.cookies.get('sdc') if sdc != "" else ""
-                self.cookies['cfr'] = self.cookies.get('cfr') if cfr != "" else ""
+            async with session.get(
+                "https://discord.com",
+                headers={
+                    "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) discord/0.0.139 Chrome/91.0.4472.164 Electron/13.6.6 Safari/537.36"
+                },
+            ) as resp:
+                dcf = resp.headers["set-cookie"].split("__dcfduid=")[0].split(";")[0]
+                sdc = resp.headers["set-cookie"].split("__sdcfduid=")[0].split(";")[0]
+                cfr = resp.headers["set-cookie"].split("__cfruid=")[0].split(";")[0]
+
+                self.cookies["dcf"] = self.cookies.get("dcf") if dcf != "" else ""
+                self.cookies["sdc"] = self.cookies.get("sdc") if sdc != "" else ""
+                self.cookies["cfr"] = self.cookies.get("cfr") if cfr != "" else ""
                 self.cookie = set(self.cookies)
 
-            async with session.get('https://discord.com/api/v9/experiments', headers={'user-agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) discord/0.0.139 Chrome/91.0.4472.164 Electron/13.6.6 Safari/537.36'}) as resp:
+            async with session.get(
+                "https://discord.com/api/v9/experiments",
+                headers={
+                    "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) discord/0.0.139 Chrome/91.0.4472.164 Electron/13.6.6 Safari/537.36"
+                },
+            ) as resp:
                 json = await resp.json()
-                self.fingerprint = json['fingerprint']
+                self.fingerprint = json["fingerprint"]
         if self.debug:
             log.debug("Gathered cookie and fingerprint")
             log.info(f"Fingerprint Gathered: {self.fingerprint}")
 
     def remove_dupes(self, dictionary: dict):
         return set(dictionary)
 
     async def request(self, method: str, endpoint: str, *args, **kwargs) -> dict:
-        '''Used to send requests
+        """Used to send requests
 
         Args:
             method (str): HTTP method
             endpoint (str): Discord api endpoint
 
         Raises:
             LoginFailure: If you suck
 
         Returns:
             dict: Data, json data
-        '''
+        """
         url = self.base_url + endpoint
 
         headers = {
-            'cookie': f'{self.cookie}',
-            'authorization': self.token,
-            'user-agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) discord/0.0.139 Chrome/91.0.4472.164 Electron/13.6.6 Safari/537.36',
-            'Content-Type': 'application/json',
-            'X-Super-Properties': self.xproperties,
-            'X-Discord-Locale': 'en-GB',
-            'Sec-Fetch-Dest': 'empty',
-            'Sec-Fetch-Mode': 'cors',
-            'Sec-Fetch-Site': 'same-origin',
-            'origin': 'https://discord.com',
-            'x-debug-options': 'logGatewayEvents,logOverlayEvents,logAnalyticsEvents,bugReporterEnabled',
-            'x-fingerprint': self.fingerprint,
-            'TE': 'trailers',
+            "cookie": f"{self.cookie}",
+            "authorization": self.token,
+            "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) discord/0.0.139 Chrome/91.0.4472.164 Electron/13.6.6 Safari/537.36",
+            "Content-Type": "application/json",
+            "X-Super-Properties": self.xproperties,
+            "X-Discord-Locale": "en-GB",
+            "Sec-Fetch-Dest": "empty",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Site": "same-origin",
+            "origin": "https://discord.com",
+            "x-debug-options": "logGatewayEvents,logOverlayEvents,logAnalyticsEvents,bugReporterEnabled",
+            "x-fingerprint": self.fingerprint,
+            "TE": "trailers",
         }
 
-        async with ClientSession(headers = headers) as session:
+        async with ClientSession(headers=headers) as session:
             request = getattr(session, method)
             while True:
                 async with request(url, *args, **kwargs) as resp:
                     if self.debug:
                         log.debug(f"Sent Request URL: {url} Payload: {args} {kwargs}")
 
                     if resp.status == 429:
                         try:
                             json = await resp.json()
-                            await asyncio.sleep(json['retry_after'])
+                            await asyncio.sleep(json["retry_after"])
                             if self.debug:
                                 log.error(f"429 Ratelimited: {json}")
                             continue
                         except Exception as e:
                             error = "".join(format_exception(e, e, e.__traceback__))
                             text = await resp.text()
                             log.error(f"Error upon parsing json : {text}")
                             if self.debug:
                                 log.error(f"Error upon parsing json : \n{error}")
-                                log.info(f"Attempted to send request to URL: {url} PAYLOAD: {kwargs}")
+                                log.info(
+                                    f"Attempted to send request to URL: {url} PAYLOAD: {kwargs}"
+                                )
                             break
 
                     elif resp.status == 401:
                         json = await resp.json()
                         if self.debug:
-                            log.info(f"Attempted to send request to URL: {url} PAYLOAD: {args} {kwargs}")
+                            log.info(
+                                f"Attempted to send request to URL: {url} PAYLOAD: {args} {kwargs}"
+                            )
                         log.error(f"{json} -- {resp.status}")
+                        break
 
                     elif resp.status == 403:
                         json = await resp.json()
                         log.error(f"403 Unauthorized: {json}")
                         if self.debug:
-                            log.info(f"Attempted to send request to URL: {url} PAYLOAD: {args} {kwargs}")
+                            log.info(
+                                f"Attempted to send request to URL: {url} PAYLOAD: {args} {kwargs}"
+                            )
                         break
 
                     elif resp.status == 201:
                         data = await resp.json()
                         break
 
                     elif resp.status == 204:
@@ -140,35 +166,46 @@
                     elif resp.ok:
                         data = await resp.json()
                         break
 
                     else:
                         if self.debug:
                             log.error(f"Unknown Error: {resp.status}")
-                            log.info(f"Attempted to send request to URL: {url} PAYLOAD: {args} {kwargs}")
+                            log.info(
+                                f"Attempted to send request to URL: {url} PAYLOAD: {args} {kwargs}"
+                            )
                         try:
                             json = await resp.json()
                             log.error(f"Error Response: {json}")
+                            break
                         except Exception as e:
                             error = "".join(format_exception(e, e, e.__traceback__))
                             log.error(f"Unable to log response: \n{error}")
-                        log.error(f"{json} -- {resp.status}")
+                            break
+                        try:
+                            text = await resp.text()
+                            log.error(f"{text} -- {resp.status}")
+                            break
+                        except:
+                            log.error(f"{resp.status}")
+                            break
         try:
-            if resp.headers['set-cookie']:
-                dcf = resp.headers['set-cookie'].split('__dcfduid=')[0].split(';')[0]
-                sdc = resp.headers['set-cookie'].split('__sdcfduid=')[0].split(';')[0]
-                cfr = resp.headers['set-cookie'].split('__cfruid=')[0].split(';')[0]
-                bm = resp.headers['set-cookie'].split('__cf_bm=')[0].split(';')[0]
-
-                self.cookies['dcf'] = self.cookies.get('dcf') if dcf != "" else ""
-                self.cookies['sdc'] = self.cookies.get('sdc') if sdc != "" else ""
-                self.cookies['cfr'] = self.cookies.get('cfr') if cfr != "" else ""
-                self.cookies['bm'] = self.cookies.get('bm') if bm != "" else ""
+            if resp.headers["set-cookie"]:
+                dcf = resp.headers["set-cookie"].split("__dcfduid=")[0].split(";")[0]
+                sdc = resp.headers["set-cookie"].split("__sdcfduid=")[0].split(";")[0]
+                cfr = resp.headers["set-cookie"].split("__cfruid=")[0].split(";")[0]
+                bm = resp.headers["set-cookie"].split("__cf_bm=")[0].split(";")[0]
+
+                self.cookies["dcf"] = self.cookies.get("dcf") if dcf != "" else ""
+                self.cookies["sdc"] = self.cookies.get("sdc") if sdc != "" else ""
+                self.cookies["cfr"] = self.cookies.get("cfr") if cfr != "" else ""
+                self.cookies["bm"] = self.cookies.get("bm") if bm != "" else ""
                 self.cookie = set(self.cookies)
-        except: pass
+        except:
+            pass
 
         try:
             return data
         except:
             return None
 
     async def encode_image(self, url: str) -> str:
@@ -177,15 +214,14 @@
         Args:
             url (str): The URL of the image
 
         Returns:
             str: The b64 payload
         """
         async with ClientSession() as session:
-            async with session.get(f'{url}') as resp:
+            async with session.get(f"{url}") as resp:
                 image = b64encode(await resp.read())
                 newobj = str(image).split("'", 2)
         if self.debug:
             log.debug("Finished encoding image")
             log.info(f"Encoded Image: {url}")
-        return f'data:image/png;base64,{newobj[1]}'
-
+        return f"data:image/png;base64,{newobj[1]}"
```

### Comparing `selfcord.py-0.1.7/selfcord/api/voice/voice.py` & `selfcord.py-0.1.8/selfcord/api/voice/voice.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,103 @@
 from __future__ import annotations
+
 import asyncio
-import websockets
-from aioconsole import aprint
 import json
-import time
-import struct
 import socket
+import struct
+import time
+
+import websockets
+from aioconsole import aprint
+
 try:
-    import opuslib
-    import nacl.utils
     import nacl.secret
+    import nacl.utils
+    import opuslib
 except:
     pass
+import io
 import os
+from traceback import format_exception
+from typing import TYPE_CHECKING, Any
+
 import aiofiles
-import io
+
 # import ffmpeg
 from ...utils import logging
-from traceback import format_exception
+
+if TYPE_CHECKING:
+    from ...api import http
+    from ...bot import Bot
+
 
 log = logging.getLogger("Voice")
 
+
 class Voice:
+    """Voice class used to interact with voice websockets and send data"""
 
     SAMPLING_RATE = 48000
     CHANNELS = 2
     FRAME_LENGTH = 20  # in milliseconds
-    SAMPLE_SIZE = struct.calcsize('h') * CHANNELS
+    SAMPLE_SIZE = struct.calcsize("h") * CHANNELS
     SAMPLES_PER_FRAME = int(SAMPLING_RATE / 1000 * FRAME_LENGTH)
     FRAME_SIZE = SAMPLES_PER_FRAME * SAMPLE_SIZE
 
-
     """Op codes"""
     READY = 2
     SESSION_DESCRIPTION = 4
     HEARTBEAT_ACK = 6
     HEARTBEAT = 8
 
-
-    def __init__(self, session_id: str, token: str, endpoint: str, server_id: str, bot, debug=False) -> None:
-        self.session_id = session_id
-        self.token = token
-        self.endpoint = endpoint
-        self.server_id = server_id
-        self.bot = bot
+    def __init__(
+        self,
+        session_id: str,
+        token: str,
+        endpoint: str,
+        server_id: str,
+        bot: Bot,
+        debug=False,
+    ) -> None:
+        self.session_id: str = session_id
+        self.token: str = token
+        self.endpoint: str = endpoint
+        self.server_id: str = server_id
+        self.bot: Bot = bot
         self.alive = False
         self.mode = "xsalsa20_poly1305"
         self.sequence = 0
-        self.debug = debug
+        self.debug: bool = debug
         self.timestamp = 0
 
-
-
     async def connect(self):
-        '''Connect to discord voice ws
-        '''
-        self.ws = await websockets.connect(f'wss://{self.endpoint}', origin='https://discord.com')
+        """Connect to discord voice ws"""
+        self.ws = await websockets.connect(
+            f"wss://{self.endpoint}", origin="https://discord.com"
+        )
         self.alive = True
 
     async def recv_msg(self):
-        '''
+        """
         Receives Message from websocket, encodes as json and runs tasks
-        '''
+        """
         item = json.loads(await self.ws.recv())
-        op      = item.get('op') # Op code
-        data    = item.get('d') # Data
+        op = item.get("op")  # Op code
+        data = item.get("d")  # Data
         if op == self.READY:
             await self.handle_ready(data)
 
         elif op == self.HEARTBEAT:
             asyncio.create_task(self.heartbeat(data))
 
         elif op == self.SESSION_DESCRIPTION:
             await self.handle_description(data)
 
     async def handle_description(self, data: dict):
-        self.secret_key: list[int] = data.get("secret_key")
+        self.secret_key: list[Any] = data.get("secret_key")
         if self.debug:
             log.debug("Finished session description event")
             log.info(f"Gathered Secret Key: {self.secret_key}")
 
     # def pcm_encode(self, file: str):
     #     out, err = (
     #         ffmpeg
@@ -87,25 +105,27 @@
     #         .output('-', format='s16le', acodec='pcm_s16le', ac=2, ar='48k')
     #         .overwrite_output()
     #         .run(capture_stdout=True, capture_stderr=True)
     #     )
     #     return out
 
     def encode_data(self, data: bytes):
-        self.encoder = opuslib.Encoder(self.SAMPLING_RATE, self.CHANNELS, opuslib.APPLICATION_AUDIO)
+        self.encoder = opuslib.Encoder(
+            self.SAMPLING_RATE, self.CHANNELS, opuslib.APPLICATION_AUDIO
+        )
         return self.encoder.encode(data, self.SAMPLES_PER_FRAME)
 
     def get_voice_packet(self, encoded: bytes):
         header = bytearray(12)
 
         header[0] = 0x80
         header[1] = 0x78
-        struct.pack_into('>H', header, 2, self.sequence)
-        struct.pack_into('>I', header, 4, self.timestamp)
-        struct.pack_into('>I', header, 8, self.SSRC)
+        struct.pack_into(">H", header, 2, self.sequence)
+        struct.pack_into(">I", header, 4, self.timestamp)
+        struct.pack_into(">I", header, 8, self.SSRC)
         return self.encrypt_xsalsa20_poly1305(header, encoded)
 
     def encrypt_xsalsa20_poly1305(self, header: bytes, data) -> bytes:
         box = nacl.secret.SecretBox(bytes(self.secret_key))
         nonce = bytearray(24)
         nonce[:12] = header
         return header + box.encrypt(bytes(data), bytes(nonce)).ciphertext
@@ -114,15 +134,15 @@
         val = getattr(self, attr)
         if val + value > limit:
             setattr(self, attr, 0)
         else:
             setattr(self, attr, val + value)
 
     async def send_encode_audio_data(self, data: bytes):
-        self.checked_add('sequence', 1, 65535)
+        self.checked_add("sequence", 1, 65535)
         buffer = io.BytesIO(data)
         while True:
             data = buffer.read(self.FRAME_SIZE)
             if len(data) == 0:
                 break
             encoded = self.encode_data(data)
             packet = self.get_voice_packet(encoded)
@@ -130,33 +150,32 @@
             self.socket.sendto(packet, (self.endpoint_IP, self.voice_port))
 
             await asyncio.sleep(self.FRAME_LENGTH / 1000)
         if self.debug:
             log.debug("Send Audio Packet to the voice port")
             log.info(f"Length of data {len(data)}")
         await self.speak(False)
-        self.checked_add('timestamp', self.SAMPLES_PER_FRAME, 4294967295)
+        self.checked_add("timestamp", self.SAMPLES_PER_FRAME, 4294967295)
 
     async def send_audio_data(self, data: bytes):
-        self.checked_add('sequence', 1, 65535)
+        self.checked_add("sequence", 1, 65535)
         buffer = io.BytesIO(data)
         while True:
             data = buffer.read(self.FRAME_SIZE)
             if len(data) == 0:
                 break
             packet = self.get_voice_packet(data)
             await self.speak(True)
             self.socket.sendto(packet, (self.endpoint_IP, self.voice_port))
             if self.debug:
                 log.debug("Send Audio Packet to the voice port")
                 log.info(f"Length of data {len(packet)}")
             await asyncio.sleep(self.FRAME_LENGTH / 1000)
         await self.speak(False)
-        self.checked_add('timestamp', self.SAMPLES_PER_FRAME, 4294967295)
-
+        self.checked_add("timestamp", self.SAMPLES_PER_FRAME, 4294967295)
 
     async def play(self, path):
         await self.speak(False)
         if self.debug:
             log.info(f"File Path: {path}")
         if os.path.exists(path):
             if os.path.isfile(path):
@@ -179,126 +198,126 @@
     async def speak(self, state):
         payload = {
             "op": 5,
             "d": {
                 "speaking": int(state),
                 "ssrc": self.SSRC,
                 "delay": 0,
-            }
+            },
         }
         await self.send_json(payload)
 
     async def send_json(self, payload: dict):
-        '''Send json to the websocket
+        """Send json to the websocket
         Args:
             payload (dict): Valid payload to send to the gateway
-        '''
+        """
         await self.ws.send(json.dumps(payload))
 
     async def close(self):
-        '''Close the connection to websocket
-        '''
+        """Close the connection to websocket"""
         self.alive = False
         await self.ws.close()
 
-
     async def identify(self):
         payload = {
             "op": 0,
             "d": {
                 "server_id": self.server_id,
                 "token": self.token,
                 "session_id": self.session_id,
                 "user_id": self.bot.user.id,
                 "streams": [
                     {"type": "video", "rid": "100", "quality": 100},
-                    {"type": "video", "rid": "50", "quality": 50}
+                    {"type": "video", "rid": "50", "quality": 50},
                 ],
-                "video": True
-
-            }
+                "video": True,
+            },
         }
         await self.send_json(payload)
         if self.debug:
             log.debug("Sent voice identify payload")
-            log.info(f"Identified on USER: {self.bot.user} SERVER: {self.server_id} TOKEN: {self.token} SESSION_ID: {self.session_id}")
+            log.info(
+                f"Identified on USER: {self.bot.user} SERVER: {self.server_id} TOKEN: {self.token} SESSION_ID: {self.session_id}"
+            )
 
     async def start(self):
         await self.connect()
         await self.identify()
         while self.alive:
-            try: await self.recv_msg()
+            try:
+                await self.recv_msg()
             except KeyboardInterrupt:
-                log.error('Shutting down')
+                log.error("Shutting down")
                 await self.close()
             except Exception as e:
-                log.error(f'Websocket Unexpectedly closed {e}')
+                log.error(f"Websocket Unexpectedly closed {e}")
                 await self.close()
 
-
     async def handle_ready(self, data: dict):
         self.SSRC = data.get("ssrc")
         self.endpoint_IP = data.get("ip")
         self.voice_port = data.get("port")
         await self.ip_discovery()
         if self.debug:
             log.debug("Finished voice ready event")
-            log.info(f"Gathered SSRC: {self.SSRC} ENDPOINT IP: {self.endpoint_IP} PORT: {self.voice_port}")
+            log.info(
+                f"Gathered SSRC: {self.SSRC} ENDPOINT IP: {self.endpoint_IP} PORT: {self.voice_port}"
+            )
 
     async def heartbeat(self, data: dict):
         interval = data.get("heartbeat_interval") / 1000.0
         while self.alive:
             await asyncio.sleep(interval)
-            payload = {
-                "op": 3,
-                "d": time.time()
-            }
+            payload = {"op": 3, "d": time.time()}
             await self.send_json(payload)
             if self.debug:
                 log.debug("Sent Heartbeat")
 
     async def udp_select(self):
         payload = {
             "op": 1,
             "d": {
                 "protocol": "udp",
                 "codecs": [
-                    {"name": "opus", "type": "audio", "priority": 1000, "payload_type": 120}
+                    {
+                        "name": "opus",
+                        "type": "audio",
+                        "priority": 1000,
+                        "payload_type": 120,
+                    }
                 ],
-                "data": {
-                    "address": self.IP,
-                    "port": self.port,
-                    "mode": self.mode
-                },
-            }
+                "data": {"address": self.IP, "port": self.port, "mode": self.mode},
+            },
         }
         await self.send_json(payload)
         if self.debug:
             log.debug("Sent UDP select payload")
             log.info(f"Sent on Address {self.IP} and Port {self.port}")
 
     async def ip_discovery(self):
         self.socket: socket.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self.socket.setblocking(False)
         packet = bytearray(74)
-        struct.pack_into('>H', packet, 0, 1)
-        struct.pack_into('>H', packet, 2, 70)
-        struct.pack_into('>I', packet, 4, self.SSRC)
+        struct.pack_into(">H", packet, 0, 1)
+        struct.pack_into(">H", packet, 2, 70)
+        struct.pack_into(">I", packet, 4, self.SSRC)
         self.socket.sendto(packet, (self.endpoint_IP, self.voice_port))
         if self.debug:
             log.debug("Sent IP discovery packet")
-            log.info(f"Sent packet to Address: {self.endpoint_IP} and Port: {self.voice_port}")
+            log.info(
+                f"Sent packet to Address: {self.endpoint_IP} and Port: {self.voice_port}"
+            )
         while True:
             try:
                 data = self.socket.recv(74)
                 break
             except:
                 continue
         ip_start = 8
         ip_end = data.index(0, ip_start)
-        self.IP = data[ip_start:ip_end].decode('ascii')
-        self.port = struct.unpack_from('>H', data, len(data) - 2)[0]
+        self.IP = data[ip_start:ip_end].decode("ascii")
+        self.port = struct.unpack_from(">H", data, len(data) - 2)[0]
         if self.debug:
             log.debug("Received IP discovery response")
             log.info(f"Received Address {self.IP} and Port {self.port}")
         await self.udp_select()
-
```

### Comparing `selfcord.py-0.1.7/selfcord/bot.py` & `selfcord.py-0.1.8/selfcord/bot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,89 @@
 from __future__ import annotations
+
 import asyncio
-import json
-from .api import gateway, http, Activity
+import contextlib
+import importlib
 import inspect
-from .models import Client, TextChannel, GroupChannel, DMChannel, VoiceChannel, Guild, User
-from collections import defaultdict
-from aioconsole import aprint, aexec
-import time
-from .utils import Command, CommandCollection, Context, ExtensionCollection, Extension, Event, logging
+import io
 import random
-import contextlib
+import time
+from collections import defaultdict
 from traceback import format_exception
-import io
-from functools import partial
-import importlib
+from typing import TYPE_CHECKING
+
 import aiohttp
+from aioconsole import aexec
 
+from .api import Activity, gateway, http
+from .models import (
+    Client,
+    DMChannel,
+    GroupChannel,
+    Guild,
+    InteractionUtil,
+    Search,
+    SlashCommand,
+    TextChannel,
+    User,
+    VoiceChannel,
+)
+from .utils import (
+    Command,
+    CommandCollection,
+    Context,
+    Event,
+    Extension,
+    ExtensionCollection,
+    logging,
+)
+
+if TYPE_CHECKING:
+    from .api.gateway import gateway
+    from .api.http import http
 
 log = logging.getLogger("Bot")
+
+
 class Bot:
-    def __init__(self, debug: bool = False, prefixes: list = ["s!"], inbuilt_help=True, userbot=False, eval=False) -> None:
-        self.inbuilt_help= inbuilt_help
-        self.debug = debug
+    """Bot instance as entry point to interact with the bot
+
+    Args:
+        debug (bool): Whether to start the bot in debug mode, defaults to False.
+        prefixes (list[str]): Prefixes for the bot, defaults to s!.
+        inbuilt_help (bool): Whether the inbuilt help command should be enabled, defaults to True.
+        userbot (bool): Whether the bot should be a userbot rather than selfbot, defaults to False.
+        eval (bool): Whether to have the eval command as default, defaults to False.
+    """
+
+    def __init__(
+        self,
+        debug: bool = False,
+        prefixes: list[str] = ["s!"],
+        inbuilt_help: bool = True,
+        userbot: bool = False,
+        eval: bool = False,
+    ) -> None:
+        self.inbuilt_help: bool = inbuilt_help
+        self.debug: bool = debug
         self.token = None
-        self.http = http(debug)
-        self.t1 = time.perf_counter()
-        self.gateway = gateway(self.http, self.debug)
+        self.http: http = http(debug)
+        self.t1: float = time.perf_counter()
+        self.session_id = None
+        self.resume_url = None
+        self.gateway: gateway = gateway(self.http, self.debug)
         self._events = defaultdict(list)
         self.commands = CommandCollection()
-        self.prefixes = prefixes if isinstance(prefixes, list) else [prefixes]
+        self.prefixes: list[str] = (
+            prefixes if isinstance(prefixes, list) else [prefixes]
+        )
         self.extensions = ExtensionCollection()
         self.user = None
-        self.eval = eval
-        self.userbot = userbot
-
+        self.eval: bool = eval
+        self.userbot: bool = userbot
 
     def run(self, token: str):
         """Used to start connection to gateway as well as gather user information
 
         Args:
             token (str): _description_
         """
@@ -63,18 +109,18 @@
 
     # For events
     async def inbuilt_commands(self):
         """
         I call this on bot initialisation, it's the inbuilt help command
         """
         if self.inbuilt_help:
+
             @self.cmd("The help command!", aliases=["test"])
             async def help(ctx, cat=None):
-                """The help command, dedicated to viewing all commands, extensions and information regarding commands.
-                """
+                """The help command, dedicated to viewing all commands, extensions and information regarding commands."""
                 if cat is None:
                     msg = f"```ini\n[ {self.user.name} Selfbot ]\n"
                     msg += f"[ {self.user} ]\nType <prefix>help <ext_name> to view commands relating to a specific extension. Type <prefix>help <cmd_name> to view information regarding a command.\n[ .Prefixes ] : {self.prefixes}\n\n"
                     msg += f"[ .Commands ]\n"
                     for command in self.commands:
                         msg += f". {command.name}: {command.description}\n"
                     msg += "\n[ .Extensions ]\n"
@@ -119,42 +165,40 @@
                         for ext in self.extensions:
                             for cmd in ext.commands:
                                 if name == cmd.name.lower():
                                     msg = f"```ini\n[ {self.user.name} Selfbot ]\n"
                                     msg += f"[ {self.user} ]\n\nType <prefix>help <ext_name> to view commands relating to a specific extension. Type <prefix>help <cmd_name> to view information regarding a command.\n\n[ .Prefixes ] : {self.prefixes}\n\n"
                                     msg += f"[ .{cmd.name} ]\n"
                                     msg += f"[ Description ] :  {cmd.description} \n"
-                                    msg += f"[ Long Description ] :\n{cmd.func.__doc__}\n"
+                                    msg += (
+                                        f"[ Long Description ] :\n{cmd.func.__doc__}\n"
+                                    )
                                     msg += f"[ Aliases ] :  {cmd.aliases} \n"
                                     args = inspect.signature(cmd.func)
                                     msg += f"\n[ Example Usage ] :\n[ {self.prefixes[0]}{cmd.aliases[0]}"
                                     for arg in args.parameters.keys():
                                         if arg == "self" or arg == "ctx":
                                             continue
                                         msg += f" <{arg}>"
                                     msg += f" ]"
 
-
                                     msg += f"```"
                                     return await ctx.reply(f"{msg}")
 
-
-
-
         if self.eval:
+
             def clean_code(content):
                 if content.startswith("```") and content.endswith("```"):
                     return "\n".join(content.split("\n")[1:])[:-3]
                 else:
                     return content
 
-            @self.cmd(description="Executes and runs code", aliases=['exec'])
+            @self.cmd(description="Executes and runs code", aliases=["exec"])
             async def eval(ctx, *, code):
-                """Runs python code via exec, intended for experienced usage. This can be DANGEROUS if you do not know what you are doing, use with caution.
-                """
+                """Runs python code via exec, intended for experienced usage. This can be DANGEROUS if you do not know what you are doing, use with caution."""
                 code = clean_code(code)
 
                 try:
                     with contextlib.redirect_stdout(io.StringIO()) as f:
                         await aexec(code)
                         result = f"```{f.getvalue()}\n```"
                 except Exception as e:
@@ -173,16 +217,17 @@
         def decorator(coro):
             if not inspect.iscoroutinefunction(coro):
                 log.error("Not a coroutine")
             else:
                 self._events[event].append(Event(name=event, coro=coro, ext=None))
 
                 def wrapper(*args, **kwargs):
-
-                    result = self._events[event].append(Event(name=event, coro=coro, ext=None))
+                    result = self._events[event].append(
+                        Event(name=event, coro=coro, ext=None)
+                    )
 
                     return result
 
                 return wrapper
 
         return decorator
 
@@ -194,26 +239,21 @@
         """
         on_event = "on_{}".format(event)
 
         # try:
         if hasattr(self, on_event):
             await getattr(self, on_event)(*args, **kwargs)
         if event in self._events.keys():
-
             for Event in self._events[event]:
-
                 if Event.coro.__code__.co_varnames[0] == "self":
-
                     asyncio.create_task(Event.coro(Event.ext, *args, **kwargs))
 
                 else:
-
                     asyncio.create_task(Event.coro(*args, **kwargs))
 
-
     def cmd(self, description="", aliases=[]):
         """Decorator to add commands for the bot
 
         Args:
             description (str, optional): Description of command. Defaults to "".
             aliases (list, optional): Alternative names for command. Defaults to [].
 
@@ -224,15 +264,17 @@
             aliases = [aliases]
 
         def decorator(coro):
             name = coro.__name__
             if not inspect.iscoroutinefunction(coro):
                 log.error("Not a coroutine")
             else:
-                cmd = Command(name=name, description=description, aliases=aliases, func=coro)
+                cmd = Command(
+                    name=name, description=description, aliases=aliases, func=coro
+                )
                 self.commands.add(cmd)
             return cmd
 
         return decorator
 
     def add_cmd(self, coro, description="", aliases=[]):
         """
@@ -248,15 +290,17 @@
         """
         if isinstance(aliases, str):
             aliases = [aliases]
         name = coro.__name__
         if not inspect.iscoroutinefunction(coro):
             log.error("Not a coroutine")
         else:
-            cmd = Command(name=name, description=description, aliases=aliases, func=coro)
+            cmd = Command(
+                name=name, description=description, aliases=aliases, func=coro
+            )
             self.commands.add(cmd)
 
     async def process_commands(self, msg):
         """
         What is called in order to actually get command input and run commands
 
         Args:
@@ -288,43 +332,80 @@
 
         try:
             spec.loader.exec_module(lib)
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Spec could not be loaded\n{error}")
         try:
-            ext = getattr(lib, 'Ext')
+            ext = getattr(lib, "Ext")
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Extension does not exist\n{error}")
 
         # Creates an Extension - ext in this case refers to the Ext class used for initialisation
-        ext = Extension(name=ext.name, description=ext.description, ext=ext(self), _events=ext._events)
+        ext = Extension(
+            name=ext.name,
+            description=ext.description,
+            ext=ext(self),
+            _events=ext._events,
+        )
         self.extensions.add(ext)
         try:
             for name, event in ext._events.items():
                 for ext_event in event:
-                    self._events[name].append(Event(name=name, coro=ext_event.coro, ext=ext.ext))
+                    self._events[name].append(
+                        Event(name=name, coro=ext_event.coro, ext=ext.ext)
+                    )
             if self.debug:
                 log.debug("Loaded Extension")
                 log.info(f"Loaded Extension {ext.name} to Bot")
 
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Failed to load extension events\n{error}")
 
+    async def trigger_slash(
+        self,
+        command: SlashCommand,
+        channel_id: str,
+        bot_id: str,
+        value: list[str] | None = None,
+        option: list[Option] | None = None,
+        guild_id: str | None = None,
+    ):
+        interaction = InteractionUtil(self, self.http)
+        await interaction.trigger_slash(
+            command, channel_id, bot_id, value, option, guild_id
+        )
+
+    async def interaction_search(
+        self,
+        query: str,
+        channel_id: str,
+        type: int = 1,
+        cursor: str = None,
+        bot_id: str = None,
+        command_id: str = None,
+    ) -> Search:
+        """Search for interactions within a specific guild channel, you can specify certain parameters
+
+        Args:
+            query (str): Query to search for
+            channel_id (str): Channel ID to search within
+            type (int): Type of command to search for
+            bot_id (str): Specify what bot specifically to search for
+            command_id (str): Specify a command id to search for, to view options
 
-
-
-
-
-
-
-
-
+        Returns:
+            Search object
+        """
+        interaction = InteractionUtil(self, self.http)
+        return await interaction.interaction_search(
+            query, channel_id, type, cursor, bot_id, command_id
+        )
 
     def get_channel(self, channel_id: str):
         """
         Function to help retrieve channel from bot cache
 
         Args:
             channel_id (str): The channel id to search for
@@ -367,69 +448,94 @@
         """
 
         data = await self.http.request(method="get", endpoint=f"/users/{user_id}")
 
         user = User(data, bot=self, http=self.http)
         return user
 
-    async def create_guild(self, name: str, icon_url: str = None, template: str = "2TffvPucqHkN"):
-        """Creates a guild
-        """
-        image = await self.http.encode_image(icon_url)
-        await self.http.request(method="post", endpoint=f"/guilds", headers={"origin": "https://discord.com", "referer": "https://discord.com/channels/@me"}, json={"name": name, "icon": image, "template": template })
+    async def create_guild(
+        self, name: str, icon_url: str = None, template: str = "2TffvPucqHkN"
+    ):
+        """Creates a guild"""
+        if icon_url is not None:
+            image = await self.http.encode_image(icon_url)
+        else:
+            image = None
+        await self.http.request(
+            method="post",
+            endpoint=f"/guilds",
+            headers={
+                "origin": "https://discord.com",
+                "referer": "https://discord.com/channels/@me",
+            },
+            json={"name": name, "icon": image, "template": template},
+        )
         if self.debug:
             log.debug("Finished Creating Guild")
-            log.info(f"Created Guild NAME: {name} TEMPLATE: {template} ICON: {icon_url}")
-
+            log.info(
+                f"Created Guild NAME: {name} TEMPLATE: {template} ICON: {icon_url}"
+            )
 
     async def add_friend(self, user_id: str):
         """
         Function to add a specific user as a friend.
 
         Args:
             user_id (str): ID of the possible random user.
 
         Returns:
             No return value.
         """
 
-        await self.http.request(method="put", endpoint=f"/users/@me/relationships/{user_id}",
-                                headers={"origin": "https://discord.com",
-                                         "referer": f"https://discord.com/channels/@me/{random.choice(self.user.private_channels).id}"},
-                                json={})
+        await self.http.request(
+            method="put",
+            endpoint=f"/users/@me/relationships/{user_id}",
+            headers={
+                "origin": "https://discord.com",
+                "referer": f"https://discord.com/channels/@me/{random.choice(self.user.private_channels).id}",
+            },
+            json={},
+        )
         if self.debug:
             log.debug("Sent Friend request")
             log.info(f"Sent Friend request to {user_id}")
 
     async def edit_profile(self, bio: str = None, accent: int = None):
-        """ Edits user profile
-        """
+        """Edits user profile"""
         fields = {}
         if bio != None:
-            fields['bio'] = bio
+            fields["bio"] = bio
         if accent != None:
-            fields['accent'] = accent
-        await self.http.request(method="patch", endpoint=f"/users/@me/profile", json=fields)
+            fields["accent"] = accent
+        await self.http.request(
+            method="patch", endpoint=f"/users/@me/profile", json=fields
+        )
         if self.debug:
             log.debug("Finished Edit profile")
 
     async def change_pfp(self, avatar_url=None):
         """Disclaimer: This may phone lock your account :(
 
         Args:
             avatar_url (str): URL of image
 
         Raises:
             TypeError: URL not specified
         """
         if avatar_url != None:
             image = await self.http.encode_image(avatar_url)
-            await self.http.request(method="patch", endpoint="/users/@me", headers={"origin": "https://discord.com",
-                                                                                    "referer": "https://discord.com/channels/@me"},
-                                    json={'avatar': image})
+            await self.http.request(
+                method="patch",
+                endpoint="/users/@me",
+                headers={
+                    "origin": "https://discord.com",
+                    "referer": "https://discord.com/channels/@me",
+                },
+                json={"avatar": image},
+            )
         else:
             log.error("Avatar URL not specified")
         if self.debug:
             log.debug("Finished changing avatar")
 
     async def create_dm(self, recipient_id: int):
         """
@@ -441,48 +547,62 @@
         Raises:
             TypeError: Recipient ID not specified
 
         Returns:
             DMChannel object
         """
         if recipient_id is not None:
-            data = await self.http.request(method="post", endpoint="/users/@me/channels",
-                                           json={"recipient_id": recipient_id})
+            data = await self.http.request(
+                method="post",
+                endpoint="/users/@me/channels",
+                json={"recipient_id": recipient_id},
+            )
             if self.debug:
                 log.debug("Created DM Channel")
             return DMChannel(data, bot=self, http=self.http)
         else:
             log.error("Recipient ID not specified")
 
     async def redeem_nitro(self, code: str):
         """Helper function to redeem nitro
 
         Args:
             code (str): Nitro code
         """
         async with aiohttp.ClientSession() as session:
-            async with session.post(f"https://canary.discord.com/api/v9/entitlements/gift-codes/{code}/redeem", headers={"authorization": f"{self.token}", "user-agent": "Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/112.0", "content-type":"application/json"}, json={}) as resp:
+            async with session.post(
+                f"https://canary.discord.com/api/v9/entitlements/gift-codes/{code}/redeem",
+                headers={
+                    "authorization": f"{self.token}",
+                    "user-agent": "Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/112.0",
+                    "content-type": "application/json",
+                },
+                json={},
+            ) as resp:
                 j = await resp.json()
-                log.info(F"Status: {resp.status} Nitro Redeem response: {j}")
-
-
-
+                log.info(f"Status: {resp.status} Nitro Redeem response: {j}")
 
     async def change_hypesquad(self, house: "str"):
         """Helper function to change hypesquad
 
         Args:
             house (str): Hypesquad name
         """
         if house.lower() == "bravery":
-            await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 1})
+            await self.http.request(
+                method="post", endpoint="/hypesquad/online", json={"house_id": 1}
+            )
         if house.lower() == "brilliance":
-            await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 2})
+            await self.http.request(
+                method="post", endpoint="/hypesquad/online", json={"house_id": 2}
+            )
         if house.lower() == "balance":
-            await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 3})
+            await self.http.request(
+                method="post", endpoint="/hypesquad/online", json={"house_id": 3}
+            )
         if self.debug:
             log.debug("Finished changing hypesquad")
             log.info(f"Changed hypesquad to {house}")
 
     async def change_presence(self, status: str, afk: bool, activity: dict):
         """Change discord activity presence
 
@@ -491,10 +611,7 @@
             afk (bool): True or False
             activity (dict): Selfcord.Activity method.
         """
         await self.gateway.change_presence(status, afk, activity=activity)
         if self.debug:
             log.debug("Finished changing presence")
             log.info(f"Changed Status to {status}, AFK to {afk}")
-
-
-
```

### Comparing `selfcord.py-0.1.7/selfcord/models/channel.py` & `selfcord.py-0.1.8/selfcord/models/channel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,67 @@
 from __future__ import annotations
+
+import asyncio
+from traceback import format_exception
+from typing import TYPE_CHECKING
+
+from ..utils import logging
 from .message import Message
-import time
 from .user import User
 from .webhook import Webhook
-import asyncio
-from ..utils import logging
-from selfcord.models import message
-from traceback import format_exception
+
+if TYPE_CHECKING:
+    from ..api.http import http
+    from ..bot import Bot
+    from ..models.permission import Permission
 
 log = logging.getLogger("Channel")
 
+
 class Messageable:
-    """Parent class specific for those classes that include a textchat for sending messages.
-    """
-    def __init__(self, http, bot) -> None:
-        self.http = http
-        self.bot = bot
+    """Parent class specific for those classes that include a textchat for sending messages."""
 
+    def __init__(self, http: http, bot: Bot) -> None:
+        self.http: http = http
+        self.bot: Bot = bot
 
-    async def history(self) -> list[Message]:
+    async def history(self) -> list[Message] | None:
         """
         Get channel message history.
 
         Args:
             No arguments required
 
         Returns:
             messages(list) : List of messages from the channel.
             None : If client does not have view permission for the channel or no data found
         """
         messages = []
-        data = await self.http.request(method="get", endpoint=f"/channels/{self.id}/messages?limit=100")
+        data = await self.http.request(
+            method="get", endpoint=f"/channels/{self.id}/messages?limit=100"
+        )
         if data is None:
             return None
 
         for msg in data:
             messages.append(Message(msg, self.bot, self.http))
         while True:
-            data = await self.http.request(method="get",
-                                           endpoint=f"/channels/{self.id}/messages?limit=100&before={data[-1]['id']}")
+            data = await self.http.request(
+                method="get",
+                endpoint=f"/channels/{self.id}/messages?limit=100&before={data[-1]['id']}",
+            )
             if len(data) > 0:
                 for msg in data:
                     messages.append(Message(msg, self.bot, self.http))
             else:
                 break
 
         return messages
 
-    async def purge(self, amount: int = None) -> None:
+    async def purge(self, amount: int = 0) -> None:
         """
         Delete a number of messages, starting from the most recent.
 
         Args:
             amount(int) : Number of messages to purge/delete.
 
         Returns:
@@ -59,30 +69,38 @@
         """
         messages = await self.history()
         msgs = []
         for msg in messages:
             if str(msg.author.id) == str(self.bot.user.id):
                 msgs.append(msg)
 
-        if amount != None:
+        if amount != 0:
             for i in range(0, len(msgs[:amount]), 3):
-                await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[:amount][i:i + 3]))
+                await asyncio.gather(
+                    *(
+                        asyncio.create_task(message.delete())
+                        for message in msgs[:amount][i : i + 3]
+                    )
+                )
         else:
             for i in range(0, len(msgs), 3):
-                await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[i:i + 3]))
-
-#            for i in range(0, len(msgs[:amount]), 2):
-#                await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[:amount][i:i + 2]))
-#                await asyncio.sleep(0.2)
-#        else:
-#            for i in range(0, len(msgs), 2):
-#                await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[i:i + 2]))
-#                await asyncio.sleep(0.2)
-
-
+                await asyncio.gather(
+                    *(
+                        asyncio.create_task(message.delete())
+                        for message in msgs[i : i + 3]
+                    )
+                )
+
+    #            for i in range(0, len(msgs[:amount]), 2):
+    #                await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[:amount][i:i + 2]))
+    #                await asyncio.sleep(0.2)
+    #        else:
+    #            for i in range(0, len(msgs), 2):
+    #                await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[i:i + 2]))
+    #                await asyncio.sleep(0.2)
 
     async def spam(self, amount: int, content: str, tts=False) -> None:
         """
         Send multiple of the same message.
 
         Args:
             - amount(int) : Number of spam messages to send.
@@ -91,116 +109,149 @@
 
         Returns:
             No return value.
         """
         amount: list[int] = [i + 1 for i in range(amount)]
         for i in range(0, len(amount), 3):
             await asyncio.gather(
-                *(asyncio.create_task(self.send(tts=tts, content=content)) for amoun in amount[i:i + 3]))
+                *(
+                    asyncio.create_task(self.send(tts=tts, content=content))
+                    for amoun in amount[i : i + 3]
+                )
+            )
             await asyncio.sleep(0.3)
 
     async def send(self, content=None, tts=False) -> Message:
         """
         Send a message to the text channel.
 
         Args:
             - content(str) : Message content. Should be string type or similar. Discord `embed` type is not allowed.
             - tts(bool) : Specify whether message is text-to-speech or not
 
         Returns:
-            No return value.
+            Message object.
         """
         if hasattr(self, "guild_id"):
-            resp = await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.guild_id}/{self.id}"},
-                                    json={"content": content, "tts": tts})
+            resp = await self.http.request(
+                method="post",
+                endpoint=f"/channels/{self.id}/messages",
+                headers={
+                    "origin": "https://discord.com",
+                    "referer": f"https://discord.com/channels/{self.guild_id}/{self.id}",
+                },
+                json={"content": content, "tts": tts},
+            )
             resp.update({"guild_id": self.guild_id})
 
         else:
-            resp = await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.id}"},
-                                    json={"content": content, "tts": tts})
+            resp = await self.http.request(
+                method="post",
+                endpoint=f"/channels/{self.id}/messages",
+                headers={
+                    "origin": "https://discord.com",
+                    "referer": f"https://discord.com/channels/{self.id}",
+                },
+                json={"content": content, "tts": tts},
+            )
 
         return Message(resp, self.bot, self.http)
 
-
     async def reply(self, message: str, content=None, tts=False) -> Message:
         """Reply to a specific message
 
         Args:
             message (str): Message to reply to
             content (_type_, optional): Message content to reply with. Defaults to None.
             tts (bool, optional): Specify whether message is text-to-speech or not. Defaults to False.
 
         Returns:
-            No return value.
+            Message object.
         """
         if hasattr(self, "guild_id"):
-            resp = await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.guild_id}/{self.id}"},
-                                    json={"content": content, "tts": tts,
-                                        "message_reference": {"channel_id": f"{self.id}", "message_id": f"{message.id}"},
-                                        "allowed_mentions": {"parse": ["users", "roles", "everyone"],
-                                                            "replied_user": False}})
+            resp = await self.http.request(
+                method="post",
+                endpoint=f"/channels/{self.id}/messages",
+                headers={
+                    "origin": "https://discord.com",
+                    "referer": f"https://discord.com/channels/{self.guild_id}/{self.id}",
+                },
+                json={
+                    "content": content,
+                    "tts": tts,
+                    "message_reference": {
+                        "channel_id": f"{self.id}",
+                        "message_id": f"{message.id}",
+                    },
+                    "allowed_mentions": {
+                        "parse": ["users", "roles", "everyone"],
+                        "replied_user": False,
+                    },
+                },
+            )
             resp.update({"guild_id": self.guild_id})
         else:
-            resp = await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.id}"},
-                                    json={"content": content, "tts": tts,
-                                        "message_reference": {"channel_id": f"{self.id}", "message_id": f"{message.id}"},
-                                        "allowed_mentions": {"parse": ["users", "roles", "everyone"],
-                                                            "replied_user": False}})
+            resp = await self.http.request(
+                method="post",
+                endpoint=f"/channels/{self.id}/messages",
+                headers={
+                    "origin": "https://discord.com",
+                    "referer": f"https://discord.com/channels/{self.id}",
+                },
+                json={
+                    "content": content,
+                    "tts": tts,
+                    "message_reference": {
+                        "channel_id": f"{self.id}",
+                        "message_id": f"{message.id}",
+                    },
+                    "allowed_mentions": {
+                        "parse": ["users", "roles", "everyone"],
+                        "replied_user": False,
+                    },
+                },
+            )
         return Message(resp, self.bot, self.http)
 
 
 class Voiceable(Messageable):
-    """Parent class specific for those classes that include a voice chat, or call functionality
-    """
-    def __init__(self, http, bot) -> None:
+    """Parent class specific for those classes that include a voice chat, or call functionality"""
+
+    def __init__(self, http: http, bot: Bot) -> None:
         super().__init__(http, bot)
-        self.http = http
-        self.bot = bot
+        self.http: http = http
+        self.bot: Bot = bot
 
     async def video_call(self):
-        """Initiates a video call on the specified channel
-        """
+        """Initiates a video call on the specified channel"""
         if hasattr(self, "guild_id"):
             await self.bot.gateway.video_call(self.id, self.guild_id)
         else:
             await self.bot.gateway.video_call(self.id)
 
     async def stream_call(self):
-        """Initiates a stream call on the specified channel
-        """
+        """Initiates a stream call on the specified channel"""
         if hasattr(self, "guild_id"):
             await self.bot.gateway.stream_call(self.id, self.guild_id)
         else:
             await self.bot.gateway.stream_call(self.id)
 
     async def call(self):
-        """Initiates a call on the specified channel
-        """
+        """Initiates a call on the specified channel"""
 
         if hasattr(self, "guild_id"):
-
             await self.bot.gateway.call(self.id, self.guild_id)
         else:
             await self.bot.gateway.call(self.id)
 
-
     async def leave_call(self):
-        """Leaves call on the specified channel
-        """
+        """Leaves call on the specified channel"""
         await self.bot.gateway.leave_call()
 
 
-
-
-
-
-
-
-
-
 class TextChannel(Messageable):
     """
     Text Channel Object
         Represents a Guild/Server channel within Discord.
         All methods are coroutines and thus need to be awaited.
 
     Returns:
@@ -229,25 +280,28 @@
           "topic": "24/7 chat about how to gank Mike #2",
           "last_message_id": "155117677105512449",
           "parent_id": "399942396007890945",
           "default_auto_archive_duration": 60
         }
     """
 
-    def __init__(self, data, bot, http) -> None:
+    def __init__(self, data, bot: Bot, http: http) -> None:
         super().__init__(http, bot)
-        self.permissions = []
-        self.webhooks = []
-        self.http = http
-        self.bot = bot
+        self.permissions: list[Permission] = []
+        self.webhooks: list[Webhook] = []
+        self.http: http = http
+        self.bot: Bot = bot
         self._update(data)
 
     def __str__(self) -> str:
         return f"{self.name}"
 
+    def __eq__(self, other):
+        return self.id == other.id
+
     def _update(self, data: dict):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
 
@@ -255,15 +309,17 @@
         self.rate_limit_per_user = data.get("rate_limit_per_user")
         self.position = data.get("position")
         self.name = data.get("name")
         self.id = data.get("id")
         self.guild_id = data.get("guild_id")
         self.last_message_id = data.get("last_message_id")
         self.flags = data.get("flags")
-        self.default_thread_rate_limit_per_user = data.get("default_thread_rate_limit_per_user")
+        self.default_thread_rate_limit_per_user = data.get(
+            "default_thread_rate_limit_per_user"
+        )
         self.category_id = data.get("parent_id")
 
     async def delete(self):
         """
         Deletes the text channel object.
 
         Args:
@@ -271,15 +327,21 @@
 
         Returns:
             No return value
         """
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}")
         del self
 
-    async def edit(self, name: str = None, parent_id: int = None, position: int = None, topic: str = None):
+    async def edit(
+        self,
+        name: str = None,
+        parent_id: int = None,
+        position: int = None,
+        topic: str = None,
+    ):
         """
         Edits the text channel object details. Requires the `Manage Channels` permission.
         Not all details can be modified.
 
         Args:
             - name(str) : Optional - Specifies a new name for the channel object. Defaults to None.
             - parent_id(int) : Optional - Specifies a new parent (category) for the text channel object.
@@ -289,24 +351,26 @@
         Notice: Each parent category can contain up to 50 channels.
 
         Returns:
             e(str) : Exception parsed as string value.
         """
         payload = {}
         if name is not None:
-            payload['name'] = name
+            payload["name"] = name
         if parent_id is not None:
-            payload['parent_id'] = parent_id
+            payload["parent_id"] = parent_id
         if position is not None:
-            payload['position'] = position
+            payload["position"] = position
         if topic is not None and topic != "":
-            payload['topic'] = topic
+            payload["topic"] = topic
 
         try:
-            await self.http.request(method="patch", endpoint=f"/channels/{self.id}", json=payload)
+            await self.http.request(
+                method="patch", endpoint=f"/channels/{self.id}", json=payload
+            )
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Could not edit channel \n{error}")
 
     async def create_webhook(self, name: str = None, avatar_url: str = None) -> Webhook:
         """
         Creates a webhook in the specified channel
@@ -319,41 +383,69 @@
             webhook (Webhook): Returns the created webhook object.
 
         Raises:
             NameError: Name is required
         """
         fields = {}
         if name != None:
-            fields['name'] = name
+            fields["name"] = name
         else:
             log.error("Name is required")
         if avatar_url != None:
             data = await self.http.encode_image(avatar_url)
-            fields['avatar'] = data
-        data = await self.http.request(method="post", endpoint=f"/channels/{self.id}/webhooks", json=fields)
+            fields["avatar"] = data
+        data = await self.http.request(
+            method="post", endpoint=f"/channels/{self.id}/webhooks", json=fields
+        )
         webhook = Webhook(data, self.bot, http=self.http)
         self.webhooks.append(webhook)
         return webhook
 
+    async def create_invite(self, max_age: int = 0, max_uses: int = 0) -> str:
+        """
+        Creates an invite in the specified channel
+
+        Args:
+            max_age (int, optional) Seconds to invite expiration. Defaults to 0 (infinite).
+            max_uses (int, optional) Maximum uses to invite expiration. Defaults to 0 (infinite).
+
+        Returns:
+            invite (str): Returns the channel invite link
+        """
+        data = await self.http.request(
+            method="post",
+            endpoint=f"/channels/{self.id}/invites",
+            json={
+                "max_age": max_age,
+                "max_uses": max_uses,
+                "target_type": None,
+                "temporary": False,
+                "flags": 0,
+            },
+        )
+        return "https://discord.gg/" + data["code"]
+
 
 class VoiceChannel(Voiceable, Messageable):
-    """Voice Channel Object
-    """
+    """Voice Channel Object"""
 
-    def __init__(self, data, bot, http) -> None:
+    def __init__(self, data: dict, bot: Bot, http: http) -> None:
         super().__init__(http, bot)
-        self.permissions = []
-        self.webhooks = []
+        self.permissions: list[Permission] = []
+        self.webhooks: list[Webhook] = []
         self.http = http
         self.bot = bot
         self._update(data)
 
     def __str__(self) -> str:
         return f"{self.name}"
 
+    def __eq__(self, other):
+        return self.id == other.id
+
     def _update(self, data: dict):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
         self.name = data.get("name")
@@ -370,15 +462,15 @@
     async def delete(self):
         """
         Deletes the voice channel object.
         """
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}")
         del self
 
-    async def create_webhook(self, name: str = None, avatar_url: str = None) -> Webhook :
+    async def create_webhook(self, name: str = None, avatar_url: str = None) -> Webhook:
         """
         Creates a webhook in the specified channel
 
         Args:
             name (str, optional): Name of the webhook. Defaults to None.
             avatar_url (str, optional): Avatar of the webhook. Requires a URL. Defaults to None.
 
@@ -387,107 +479,135 @@
 
         Raises:
             NameError: Name is required
         """
 
         fields = {}
         if name != None:
-            fields['name'] = name
+            fields["name"] = name
         else:
             log.error("Name is required...")
         if avatar_url != None:
             data = await self.http.encode_image(avatar_url)
-            fields['avatar'] = data
-        data = await self.http.request(method="post", endpoint=f"/channels/{self.id}/webhooks", json=fields)
+            fields["avatar"] = data
+        data = await self.http.request(
+            method="post", endpoint=f"/channels/{self.id}/webhooks", json=fields
+        )
         webhook = Webhook(data, self.bot, self.http)
         self.webhooks.append(webhook)
         return webhook
 
+    async def create_invite(self, max_age: int = 0, max_uses: int = 0) -> str:
+        """
+        Creates an invite in the specified channel
 
+        Args:
+            max_age (int, optional) Seconds to invite expiration. Defaults to 0 (infinite).
+            max_uses (int, optional) Maximum uses to invite expiration. Defaults to 0 (infinite).
+
+        Returns:
+            invite (str): Returns the channel invite link
+        """
+        data = await self.http.request(
+            method="post",
+            endpoint=f"/channels/{self.id}/invites",
+            json={
+                "max_age": max_age,
+                "max_uses": max_uses,
+                "target_type": None,
+                "temporary": False,
+                "flags": 0,
+            },
+        )
+        return "https://discord.gg/" + data["code"]
 
 
 class Category:
-    """Category Object
-    """
+    """Category Object"""
 
-    def __init__(self, data, bot, http) -> None:
-        self.bot = bot
-        self.http = http
-        self.permissions = []
+    def __init__(self, data: dict, bot: Bot, http: http) -> None:
+        self.bot: Bot = bot
+        self.http: http = http
+        self.permissions: list[Permission] = []
         self._update(data)
 
     def __str__(self) -> str:
         return f"{self.name}"
 
+    def __eq__(self, other):
+        return self.id == other.id
+
     def _update(self, data: dict):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
         self.name = data.get("name")
         self.id = data.get("id")
         self.guild_id = data.get("guild_id")
         self.position = data.get("position")
         self.flags = data.get("flags")
 
     async def delete(self):
-        """Deletes the Category object.
-        """
+        """Deletes the Category object."""
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}")
         del self
 
 
 class DMChannel(Voiceable, Messageable):
-    """DM Channel Object
-    """
+    """DM Channel Object"""
 
-    def __init__(self, data, bot, http) -> None:
+    def __init__(self, data: dict, bot: Bot, http: http) -> None:
         super().__init__(http, bot)
-        self.http = http
-        self.bot = bot
+        self.http: http = http
+        self.bot: Bot = bot
         self._update(data)
 
     def __str__(self) -> str:
         return f"{self.recipient}"
 
+    def __eq__(self, other):
+        return self.id == other.id
+
     def _update(self, data: dict):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
         self.recipient = User(data.get("recipients")[0], self.bot, self.http)
         self.last_message_id = data.get("last_message_id")
         self.id = data.get("id")
         self.flags = data.get("id")
 
     async def delete(self):
-        """Deletes the DM Channel object.
-        """
-        await self.http.request(method="delete", endpoint=f"/channels/{self.id}?silent=false")
+        """Deletes the DM Channel object."""
+        await self.http.request(
+            method="delete", endpoint=f"/channels/{self.id}?silent=false"
+        )
         del self
 
 
-
-
 class GroupChannel(Voiceable, Messageable):
-    """Group Channel Object
-    """
+    """Group Channel Object"""
 
-    def __init__(self, data, bot, http) -> None:
+    def __init__(self, data: dict, bot: Bot, http: http) -> None:
         super().__init__(http, bot)
         self.recipients = []
-        self.http = http
-        self.bot = bot
+        self.http: http = http
+        self.bot: Bot = bot
         self._update(data)
 
     def __str__(self) -> str:
         return f"{self.name}"
 
+    def __eq__(self, other):
+        return self.id == other.id
+
     def _update(self, data: dict):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
         for user in data.get("recipients"):
@@ -496,13 +616,29 @@
         self.owner_id = data.get("owner_id")
         self.last_message_id = data.get("last_message_id")
         self.id = data.get("id")
         self.flags = data.get("flags")
         self.icon = data.get("icon")
 
     async def delete(self):
-        """Deletes the Group Channel Object
-        """
-        await self.http.request(method="delete", endpoint=f"/channels/{self.id}?silent=true")
+        """Deletes the Group Channel Object"""
+        await self.http.request(
+            method="delete", endpoint=f"/channels/{self.id}?silent=true"
+        )
         del self
 
+    async def create_invite(self) -> str:
+        """
+        Creates an invite in the specified group channel
 
+        Args:
+            None
+
+        Returns:
+            invite (str): Returns the channel invite link
+        """
+        data = await self.http.request(
+            method="post",
+            endpoint=f"/channels/{self.id}/invites",
+            json={"max_age": 86400},
+        )
+        return "https://discord.gg/" + data["code"]
```

### Comparing `selfcord.py-0.1.7/selfcord/models/emoji.py` & `selfcord.py-0.1.8/selfcord/models/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 from __future__ import annotations
 
-class Emoji:
-    """Emoji Object
-    """
-    def __init__(self, data, bot, http) -> None:
-        self.bot = bot
-        self.http = http
-        self._update(data)
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from .channel import Voiceable
+    from .guild import Guild
+    from .message import Message
+    from .user import User
+
+
+class Client:
+    """Client Object"""
+
+    def __init__(self, UserPayload: dict) -> None:
+        self.guilds: list[Guild] = []
+        self.private_channels: list[Voiceable] = []
+        self.friends: list[User] = []
+        self.messages: list[Message] = []
+        self.deleted_messages: list[Message] = []
+        self._update(UserPayload)
 
     def __str__(self) -> str:
-        return f"{self.name}"
+        return f"""{self.name}#{self.discriminator}"""
+
+    def __eq__(self, other):
+        return self.id == other.id
 
-    def _update(self, data: dict):
+    def _update(self, data):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
-        self.name = data.get("name")
+        self.name = data.get("username")
         self.id = data.get("id")
-        self.roles = data.get("roles")
-        self.managed = data.get("managed")
-        self.available = data.get("available")
-        self.animated = data.get("animated")
-        self.guild_id = data.get("guild_id")
-
-
-    async def delete(self):
-        """Deletes the Emoji Object
-        """
-        await self.http.request(method="delete", endpoint=f"/guilds/{self.guild_id}/emojis/{self.id}")
-        del self
+        self.discriminator = data.get("discriminator")
+        self.avatar = data.get("avatar")
+        self.banner = data.get("banner")
+        self.bio = data.get("bio")
+        self.email = data.get("email")
+        self.phone = data.get("phone")
+        self.accent_colour = data.get("accent_color")
+        self.public_flags = data.get("public_flags")
+        self.bot_acc = data.get("bot")
+        self.system = data.get("system")
```

### Comparing `selfcord.py-0.1.7/selfcord/models/guild.py` & `selfcord.py-0.1.8/selfcord/models/guild.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,81 @@
 from __future__ import annotations
-from .user import User
-from .channel import TextChannel, VoiceChannel, Category
-from .role import Role
-from .emoji import Emoji
-from itertools import zip_longest
-from aiohttp import ClientSession
-from base64 import b64encode
+
 import random
 from datetime import datetime, timedelta, timezone
+from itertools import zip_longest
+from typing import TYPE_CHECKING
+
+from .channel import Category, Messageable, TextChannel, VoiceChannel
+from .emoji import Emoji
+from .role import Role
+from .user import User
+
+if TYPE_CHECKING:
+    from ..api import http
+    from ..bot import Bot
+
+
 class Guild:
-    """Guild Object
-    """
+    """Guild Object"""
+
     TEXTCHANNEL = 0
     VOICECHANNEL = 2
     CATEGORY = 4
     GUILD_ANNOUNCEMENT = 5
     ANNOUNCEMENT_THREAD = 10
     PUBLIC_THREAD = 11
     PRIVATE_THREAD = 12
     GUILD_STAGE_VOICE = 13
     GUILD_DIRECTORY = 14
     GUILD_FORUM = 15
 
-    def __init__(self, data, bot, http) -> None:
-        self.roles = []
-        self.emojis = []
-        self.members = []
-        self.channels = []
-        self.http = http
-        self.bot = bot
+    def __init__(self, data: dict, bot: Bot, http: http) -> None:
+        self.roles: list[Role] = []
+        self.emojis: list[Emoji] = []
+        self.members: list[User] = []
+        self.channels: list[Messageable] = []
+        self.http: http = http
+        self.bot: Bot = bot
         self._update(data)
 
     def __str__(self) -> str:
         return f"{self.name}"
 
+    def __eq__(self, other):
+        return self.id == other.id
+
     def _update(self, data):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
-        self.id = data.get('id')
-        self.name = data.get('name')
-        self.icon = data.get('icon')
-        self.region = data.get('region')
-        self.splash = data.get('splash')
-        self.mfa_level = data.get('mfa_level')
-        self.features = data.get('features')
+        self.id = data.get("id")
+        self.name = data.get("name")
+        self.icon = data.get("icon")
+        self.icon_url = (
+            f"https://cdn.discordapp.com/icons/{self.id}/{self.icon}.webp?size=96"
+        )
+        self.region = data.get("region")
+        self.splash = data.get("splash")
+        self.mfa_level = data.get("mfa_level")
+        self.features = data.get("features")
         self.member_count = data.get("member_count")
-        self.unavailable = data.get('unavailable')
-        self.verification_level = data.get('verification_level')
-        self.explicit_content_filter = data.get('explicit_content_filter')
-        self.owner_id = data.get('owner_id')
-
-        for (member, channel, role, emoji) in zip_longest(data.get('members'), data.get("channels"), data.get("roles"), data.get("emojis")):
+        self.unavailable = data.get("unavailable")
+        self.verification_level = data.get("verification_level")
+        self.explicit_content_filter = data.get("explicit_content_filter")
+        self.owner_id = data.get("owner_id")
+
+        for member, channel, role, emoji in zip_longest(
+            data.get("members"),
+            data.get("channels"),
+            data.get("roles"),
+            data.get("emojis"),
+        ):
             if member != None:
                 user = User(member, self.bot, self.http)
 
                 self.members.append(user)
 
             if channel != None:
                 type = channel.get("type")
@@ -75,132 +93,178 @@
                     self.channels.append(channel)
                 else:
                     channel = TextChannel(channel, self.bot, self.http)
                     channel.guild_id = self.id
                     self.channels.append(channel)
 
             if role != None:
-                role = Role(role, self.http, guild_id = self.id)
+                role = Role(role, self.bot, self.http, guild_id=self.id)
                 self.roles.append(role)
 
             if emoji != None:
                 emoji = Emoji(emoji, self.bot, self.http)
                 emoji.guild_id = self.id
                 self.emojis.append(emoji)
 
     async def ban(self, user_id: str):
         """Bans a user from the guild
 
         Args:
             user_id (str): User ID specified to ban
         """
-        await self.http.request(method="put", endpoint=f"/guilds/{self.id}/bans/{user_id}", json={"delete_message_days":"7"})
+        await self.http.request(
+            method="put",
+            endpoint=f"/guilds/{self.id}/bans/{user_id}",
+            json={"delete_message_days": "7"},
+        )
 
     async def kick(self, user_id: str):
         """Kicks a user from the guild
 
         Args:
             user_id (str): User ID specified to kick
         """
-        await self.http.request(method="delete", endpoint=f"/guilds/{self.id}/members/{user_id}")
+        await self.http.request(
+            method="delete", endpoint=f"/guilds/{self.id}/members/{user_id}"
+        )
 
     def utc_now(self):
         return datetime.now(timezone.utc)
 
-    async def timeout(self, user_id: str, hours=0, mins=0, seconds=0):
+    async def timeout(
+        self, user_id: str, hours: int = 0, mins: int = 0, seconds: int = 0
+    ):
         """Timeouts a user in the guild
 
         Args:
             user_id (str): User ID specified to timeout
         """
-        duration = self.utc_now() + timedelta(hours=hours, minutes=mins, seconds=seconds)
-        await self.http.request(method="patch", endpoint=f"/guilds/{self.id}/members/{user_id}", json={"communication_disabled_until": str(duration)})
+        duration = self.utc_now() + timedelta(
+            hours=hours, minutes=mins, seconds=seconds
+        )
+        await self.http.request(
+            method="patch",
+            endpoint=f"/guilds/{self.id}/members/{user_id}",
+            json={"communication_disabled_until": str(duration)},
+        )
 
-    async def txt_channel_create(self, name:str, parent_id: str=None):
+    async def txt_channel_create(self, name: str, parent_id: str = None):
         """Creates a Text Channel in the guild
 
         Args:
             name (str): Name of the channel
             parent_id (str, optional): ID of the category. Defaults to None.
         """
         payload = {"name": name}
         payload.update({"permission_overwrites": []})
         payload.update({"type": 0})
-        if parent_id:
+        if parent_id != None:
             payload.update({"parent_id": parent_id})
 
-        await self.http.request(method="post", endpoint=f"/guilds/{self.id}/channels", json=payload)
+        channel = await self.http.request(
+            method="post", endpoint=f"/guilds/{self.id}/channels", json=payload
+        )
+        return TextChannel(channel, self.bot, self.http)
 
     async def vc_channel_create(self, name: str):
         """Creates a voice channel in the guild
 
         Args:
             name (str): Name of the channel
         """
-        await self.http.request(method="post", endpoint=f"/guilds/{self.id}/channels", json={"name": f"{name}", "permission_overwrites": [], "type": 2})
+        channel = await self.http.request(
+            method="post",
+            endpoint=f"/guilds/{self.id}/channels",
+            json={"name": f"{name}", "permission_overwrites": [], "type": 2},
+        )
+        return VoiceChannel(channel, self.bot, self.http)
 
     async def role_create(self, name: str):
         """Creates a role in the guild
 
         Args:
             name (str): Name of the role
         """
-        await self.http.request(method = "post", endpoint = f"/guilds/{self.id}/roles", json = {"name": f"{name}"})
+        role = await self.http.request(
+            method="post", endpoint=f"/guilds/{self.id}/roles", json={"name": f"{name}"}
+        )
+        return Role(role, self.bot, self.http, guild_id=self.id)
 
-    async def category_channel_create(self, name):
+    async def category_channel_create(self, name: str):
         """Creates a category in the guild
 
         Args:
             name (str): Name of the category
         """
-        await self.http.request(method = "post", endpoint = f"/guilds/{self.id}/channels", json={"name": f"{name}", "permission_overwrites": [], "type": 4})
+        channel = await self.http.request(
+            method="post",
+            endpoint=f"/guilds/{self.id}/channels",
+            json={"name": f"{name}", "permission_overwrites": [], "type": 4},
+        )
+        return Category(channel, self.bot, self.http)
 
     async def emoji_create(self, name: str, image_url: str):
         """Creates an emoji in the guild
 
         Args:
             name (str): Name of the emoji
             image_url (str): URL for an image
         """
         image = await self.http.encode_image(image_url)
-        await self.http.request(method = "post", endpoint = f"/guilds/{self.id}/emojis", json= {"name": f"{name}", "image": image})
+        emoji = await self.http.request(
+            method="post",
+            endpoint=f"/guilds/{self.id}/emojis",
+            json={"name": f"{name}", "image": image},
+        )
+        return Emoji(emoji, self.bot, self.http)
 
     async def get_members(self, channel_id: str):
         """Get guild members for a guild via chunking
 
         Args:
             channel_id (str): Channel ID to chunk from
         """
         await self.bot.gateway.lazy_chunk(self.id, channel_id, self.member_count)
 
-    async def edit(self, name: str=None, icon_url: str=None, banner_url: str=None, description: str=None):
+    async def edit(
+        self,
+        name: str = None,
+        icon_url: str = None,
+        banner_url: str = None,
+        description: str = None,
+    ):
         """Edits attributes for a guild
 
         Args:
             name (str, optional): Name of the guild. Defaults to None.
             icon_url (str, optional): Image URL for Icon. Defaults to None.
             banner_url (str, optional): Image URL for Banner. Defaults to None.
             description (str, optional): Description of the guild. Defaults to None.
         """
         fields = {}
         if name != None:
-            fields['name'] = name
+            fields["name"] = name
 
         if description != None:
-            fields['description'] = description
+            fields["description"] = description
 
         if icon_url != None:
             data = await self.http.encode_image(icon_url)
-            fields['icon'] = data
+            fields["icon"] = data
 
         if banner_url != None:
             data = await self.http.encode_image(banner_url)
-            fields['banner'] = data
-
+            fields["banner"] = data
 
-        await self.http.request(method = "patch", endpoint = f"/guilds/{self.id}", headers={"origin":"https://discord.com", "referer":f"https://discord.com/channels/{self.id}/{random.choice(self.channels)}"},json=fields)
+        await self.http.request(
+            method="patch",
+            endpoint=f"/guilds/{self.id}",
+            headers={
+                "origin": "https://discord.com",
+                "referer": f"https://discord.com/channels/{self.id}/{random.choice(self.channels)}",
+            },
+            json=fields,
+        )
 
     async def delete(self):
-        """Deletes the Guild Object
-        """
-        await self.http.request(method = "delete", endpoint = f"/guilds/{self.id}")
-
+        """Deletes the Guild Object"""
+        await self.http.request(method="delete", endpoint=f"/guilds/{self.id}")
```

### Comparing `selfcord.py-0.1.7/selfcord/models/member.py` & `selfcord.py-0.1.8/selfcord/models/member.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from .role import Role
+
+
 class Member:
-    """Member Object
-    """
+    """Member Object"""
+
     def __init__(self, UserPayload: dict) -> None:
-        self.roles = []
+        self.roles: list[Role] = []
 
         self._update(UserPayload)
 
     def __str__(self):
         return f"""{self.name}#{self.discriminator}"""
 
+    def __eq__(self, other):
+        return self.id == other.id
 
-    def _update(self, data):
+    def _update(self, data: dict):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
         user = data.get("user")
         self.name = user.get("username")
         self.id = user.get("id")
         self.discriminator = user.get("discriminator")
         self._avatar = user.get("avatar")
         self._banner = user.get("banner")
-        self._accent_colour = user.get('accent_color')
-        self._public_flags = user.get('public_flags')
-        self.bot_acc = user.get('bot')
-        self.joined_at = data.get('joined_at')
+        self._accent_colour = user.get("accent_color")
+        self._public_flags = user.get("public_flags")
+        self.bot_acc = user.get("bot")
+        self.joined_at = data.get("joined_at")
         self.nick = data.get("nick")
-        self.system = data.get('system')
+        self.system = data.get("system")
```

### Comparing `selfcord.py-0.1.7/selfcord/models/message.py` & `selfcord.py-0.1.8/selfcord/models/message.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 from __future__ import annotations
-from .user import User
+
 import asyncio
+import time
 import urllib
 
+from .user import User
+
+
+class Attachment:
+    def __init__(self, data) -> None:
+        self.proxy_url = data.get("proxy_url")
+        self.url = data.get("url")
+        self.name = data.get("filename")
+        self.size = data.get("size")
+        self.id = data.get("id")
+
+
 class Message:
-    """Message Object
-    """
+    """Message Object"""
+
     def __init__(self, data, bot, http) -> None:
         self.bot = bot
         self.channel = None
         self.guild = None
         self.http = http
         self._update(data)
 
     def __str__(self) -> str:
         return f"{self.content}"
 
+    def __eq__(self, other):
+        return self.id == other.id
+
     def _update(self, data):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
         self.tts = data.get("tts")
@@ -27,50 +43,65 @@
         self.mentions = data.get("mentions")
         self.author = User(data.get("author"), self.bot, self.http)
         self.id = data.get("id")
         self.flags = data.get("flags")
         self.embeds = data.get("embeds")
         self.content = data.get("content")
         self.components = data.get("components")
-
+        self.timestamp = time.time()
         self.channel_id = data.get("channel_id")
 
-        self.attachments = data.get("attachments")
+        attachments = data.get("attachments")
+        self.attachments = [Attachment(atch) for atch in attachments]
         self.guild_id = data.get("guild_id")
 
         self.channel = self.bot.get_channel(self.channel_id)
 
         self.guild = self.bot.get_guild(self.guild_id)
 
     async def delete(self):
-        """Delete the Message Object
-        """
-        await self.http.request(method="delete", endpoint=f"/channels/{self.channel_id}/messages/{self.id}")
+        """Delete the Message Object"""
+        await self.http.request(
+            method="delete", endpoint=f"/channels/{self.channel_id}/messages/{self.id}"
+        )
 
-    async def edit(self, content: str):
+    async def edit(self, content: str) -> Message:
         """Edits the specified message
 
         Args:
             content (str): Content to edit message to.
         """
         if self.guild_id != None:
-            resp = await self.http.request(method="patch", endpoint=f"/channels/{self.channel_id}/messages/{self.id}", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.channel_id}/{self.guild_id}"}, json={"content":content})
-            resp.update({"guild_id" : self.guild_id})
+            resp = await self.http.request(
+                method="patch",
+                endpoint=f"/channels/{self.channel_id}/messages/{self.id}",
+                headers={
+                    "origin": "https://discord.com",
+                    "referer": f"https://discord.com/channels/{self.channel_id}/{self.guild_id}",
+                },
+                json={"content": content},
+            )
+            resp.update({"guild_id": self.guild_id})
         else:
-            resp = await self.http.request(method="patch", endpoint=f"/channels/{self.channel_id}/messages/{self.id}", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.channel_id}"}, json={"content":content})
+            resp = await self.http.request(
+                method="patch",
+                endpoint=f"/channels/{self.channel_id}/messages/{self.id}",
+                headers={
+                    "origin": "https://discord.com",
+                    "referer": f"https://discord.com/channels/{self.channel_id}",
+                },
+                json={"content": content},
+            )
         return Message(resp, self.bot, self.http)
 
-
     async def react(self, emoji: str):
         """React to a message with an emoji
 
         Args:
             emoji (str): The emoji
         """
         raw_reaction = urllib.parse.urlencode({"emoji": emoji}).split("emoji=")[1]
-        await self.http.request(method="put", endpoint=f"/channels/{self.channel_id}/messages/{self.id}/reactions/{raw_reaction}/%40me?location=Message&burst=false", headers={"referer": f"https://discord.com/channels/@me/{self.channel_id}"})
-
-
-
-
-
-
+        await self.http.request(
+            method="put",
+            endpoint=f"/channels/{self.channel_id}/messages/{self.id}/reactions/{raw_reaction}/%40me?location=Message&burst=false",
+            headers={"referer": f"https://discord.com/channels/@me/{self.channel_id}"},
+        )
```

### Comparing `selfcord.py-0.1.7/selfcord/models/permission.py` & `selfcord.py-0.1.8/selfcord/models/permission.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 from __future__ import annotations
+
+
 class Permission:
-    """Permission Object
-    """
+    """Permission Object"""
 
-    def __init__(self, data) -> None:
+    def __init__(self, data: int) -> None:
         self.perms = {
             "CREATE_INSTANT_INVITE": 0x1,
             "KICK_MEMBERS": 0x2,
             "BAN_MEMBERS": 0x4,
-            "ADMINISTRATOR" : 0x8,
+            "ADMINISTRATOR": 0x8,
             "MANAGE_CHANNELS": 0x10,
-            "MANAGE_GUILD" : 0x20,
-            "ADD_REACTIONS" : 0X40,
-            "VIEW_AUDIT_LOG" : 0x80,
-            "PRIORITY_SPEAKER" : 0x100,
-            "STREAM" : 0x200,
-            "VIEW_CHANNEL" : 0x400,
-            "SEND_MESSAGES" : 0x800,
-            "SEND_TTS_MESSAGES" : 0x1000,
-            "MANAGE_MESSAGES" : 0x2000,
-            "EMBED_LINKS" : 0x4000,
-            "ATTACH_FILES" : 0x8000,
-            "READ_MESSAGE_HISTORY" : 0x10000,
-            "MENTION_EVERYONE" : 0x20000,
-            "USE_EXTERNAL_EMOJIS" : 0x40000,
-            "VIEW_GUILD_INSIGHTS" : 0x80000,
-            "CONNECT" : 0x100000,
-            "SPEAK" : 0x200000,
-            "MUTE_MEMBERS" : 0x400000,
-            "DEAFEN_MEMBERS" : 0x800000,
-            "MOVE_MEMBERS" : 0x1000000,
-            "USE_VAD" : 0x2000000,
-            "CHANGE_NICK" : 0x4000000,
-            "MANAGE_NICK" : 0x8000000,
-            "MANAGE_ROLES" : 0x10000000,
-            "MANAGE_WEBHOOKS" : 0x20000000,
-            "MANAGE_EMOJIS_AND_STICKERS" : 0x40000000,
-            "USE_APPLICATION_COMMANDS" : 0x80000000,
-            "REQUEST_TO_SPEAK" : 0x100000000,
-            "MANAGE_EVENTS" : 0x200000000,
-            "MANAGE_THREADS" : 0x400000000,
-            "CREATE_PUBLIC_THREADS" : 0x800000000,
-            "CREATE_PRIVATE_THREADS" : 0x1000000000,
-            "USE_EXTERNAL_STICKERS" : 0x2000000000,
-            "SEND_MESSAGES_IN_THREADS" : 0x4000000000,
-            "USE_EMBEDDED_ACTIVITIES" : 0x8000000000,
-            "MODERATE_MEMBERS" : 0x10000000000
+            "MANAGE_GUILD": 0x20,
+            "ADD_REACTIONS": 0x40,
+            "VIEW_AUDIT_LOG": 0x80,
+            "PRIORITY_SPEAKER": 0x100,
+            "STREAM": 0x200,
+            "VIEW_CHANNEL": 0x400,
+            "SEND_MESSAGES": 0x800,
+            "SEND_TTS_MESSAGES": 0x1000,
+            "MANAGE_MESSAGES": 0x2000,
+            "EMBED_LINKS": 0x4000,
+            "ATTACH_FILES": 0x8000,
+            "READ_MESSAGE_HISTORY": 0x10000,
+            "MENTION_EVERYONE": 0x20000,
+            "USE_EXTERNAL_EMOJIS": 0x40000,
+            "VIEW_GUILD_INSIGHTS": 0x80000,
+            "CONNECT": 0x100000,
+            "SPEAK": 0x200000,
+            "MUTE_MEMBERS": 0x400000,
+            "DEAFEN_MEMBERS": 0x800000,
+            "MOVE_MEMBERS": 0x1000000,
+            "USE_VAD": 0x2000000,
+            "CHANGE_NICK": 0x4000000,
+            "MANAGE_NICK": 0x8000000,
+            "MANAGE_ROLES": 0x10000000,
+            "MANAGE_WEBHOOKS": 0x20000000,
+            "MANAGE_EMOJIS_AND_STICKERS": 0x40000000,
+            "USE_APPLICATION_COMMANDS": 0x80000000,
+            "REQUEST_TO_SPEAK": 0x100000000,
+            "MANAGE_EVENTS": 0x200000000,
+            "MANAGE_THREADS": 0x400000000,
+            "CREATE_PUBLIC_THREADS": 0x800000000,
+            "CREATE_PRIVATE_THREADS": 0x1000000000,
+            "USE_EXTERNAL_STICKERS": 0x2000000000,
+            "SEND_MESSAGES_IN_THREADS": 0x4000000000,
+            "USE_EMBEDDED_ACTIVITIES": 0x8000000000,
+            "MODERATE_MEMBERS": 0x10000000000,
         }
         self.permissions = self.calculate_permissions(data)
 
-
     def calculate_permissions(self, perm_value: int):
         permissions = []
         for perm, value in self.perms.items():
             if (perm_value & value) == value:
                 permissions.append(perm)
 
         return permissions
-
-
-
```

### Comparing `selfcord.py-0.1.7/selfcord/models/role.py` & `selfcord.py-0.1.8/selfcord/models/role.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from .permission import Permission
 
+if TYPE_CHECKING:
+    from ..api.http import http
+    from ..bot import Bot
+
+
 class Role:
-    """Role Object
-    """
-    def __init__(self, data: dict, http, **kwargs) -> None:
+    """Role Object"""
+
+    def __init__(self, data: dict, bot: Bot, http: http, **kwargs) -> None:
         self.guild_id = kwargs.get("guild_id")
-        self.http = http
+        self.http: http = http
+        self.bot: Bot = bot
         self._update(data)
 
+    def __eq__(self, other):
+        return self.id == other.id
+
     def _update(self, data):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
         role = data.get("role")
 
-        self.id = data.get("id") if role==None else role.get("id")
-        self.permissions = Permission(int(data.get("permissions"))).permissions if role==None else Permission(int(role.get("permissions"))).permissions
-        self.name = data.get("name") if role==None else role.get("name")
-        self.mentionable = data.get("mentionable") if role==None else role.get("mentionable")
-        self.managed = data.get("managed") if role==None else role.get("managed")
-        self.icon = data.get("icon") if role==None else role.get("icon")
-        self.flags = data.get("flags") if role==None else role.get("flags")
+        self.id = data.get("id") if role == None else role.get("id")
+        self.permissions = (
+            Permission(int(data.get("permissions"))).permissions
+            if role == None
+            else Permission(int(role.get("permissions"))).permissions
+        )
+        self.name = data.get("name") if role == None else role.get("name")
+        self.mentionable = (
+            data.get("mentionable") if role == None else role.get("mentionable")
+        )
+        self.managed = data.get("managed") if role == None else role.get("managed")
+        self.icon = data.get("icon") if role == None else role.get("icon")
+        self.flags = data.get("flags") if role == None else role.get("flags")
 
-        self.color = data.get("color") if role==None else role.get("color")
-        self.hoist = data.get("hoist") if role==None else role.get("hoist")
+        self.color = data.get("color") if role == None else role.get("color")
+        self.hoist = data.get("hoist") if role == None else role.get("hoist")
         if self.guild_id is None:
             self.guild_id = data.get("guild_id")
 
-
-
     def __str__(self) -> str:
         return f"{self.name}"
 
     async def delete(self):
-        """Delete the Role Object
-        """
-        await self.http.request(method="delete", endpoint=f"/guilds/{self.guild_id}/roles/{self.id}")
-        del self
+        """Delete the Role Object"""
+        await self.http.request(
+            method="delete", endpoint=f"/guilds/{self.guild_id}/roles/{self.id}"
+        )
+        del self
```

### Comparing `selfcord.py-0.1.7/selfcord/models/user.py` & `selfcord.py-0.1.8/selfcord/models/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from __future__ import annotations
-from base64 import b64encode
+
 import datetime
+from base64 import b64encode
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from ..api.http import http
+    from ..bot import Bot
 
 
 class Profile:
-    def __init__(self, UserPayload: dict, bot, http) -> None:
-        self.bot = bot
-        self.http = http
+    def __init__(self, UserPayload: dict, bot: Bot, http: http) -> None:
+        self.bot: Bot = bot
+        self.http: http = http
 
         self.__update(UserPayload)
 
-
-
     def __update(self, data: dict):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
 
-        self.connected_accounts = [Connected_Account(account) for account in data.get("connected_accounts")]
-
-
-        self.mutual_guilds = [self.bot.get_guild(guild['id']) for guild in data.get("mutual_guilds")]
+        self.connected_accounts = [
+            Connected_Account(account) for account in data.get("connected_accounts")
+        ]
+
+        self.mutual_guilds = [
+            self.bot.get_guild(guild["id"]) for guild in data.get("mutual_guilds")
+        ]
 
-        self.id = data['user']['id']
+        self.id = data["user"]["id"]
         self.premium_type = data.get("premium_type")
         user_profile = data.get("user_profile")
         try:
             self.emoji = user_profile.get("emoji")
         except:
             self.emoji = None
         try:
@@ -39,15 +46,20 @@
             self.accent_color = user_profile.get("accent_color")
         except:
             self.accent_color = None
         try:
             self.banner = user_profile.get("banner")
         except:
             self.banner = None
-        self.banner_url = f"https://cdn.discordapp.com/banners/{self.id}/{self.banner}.png?size=1024" if self.banner!=None else None
+        self.banner_url = (
+            f"https://cdn.discordapp.com/banners/{self.id}/{self.banner}.png?size=1024"
+            if self.banner != None
+            else None
+        )
+
 
 class Connected_Account:
     def __init__(self, data) -> None:
         self.__update(data)
 
     def __update(self, data: dict):
         """Updater method intended to create the attributes for the object
@@ -57,88 +69,104 @@
         """
         self.type = data.get("type")
         self.name = data.get("name")
         self.id = data.get("id")
 
 
 class User:
-    """User Object
-    """
-    def __init__(self, UserPayload: dict, bot, http) -> None:
-        self.bot = bot
+    """User Object"""
+
+    def __init__(self, UserPayload: dict, bot: Bot, http: http) -> None:
+        self.bot: Bot = bot
 
-        self.http = http
+        self.http: http = http
         self._update(UserPayload)
 
+    def __eq__(self, other):
+        return self.id == other.id
+
     def __str__(self):
         return f"""{self.name}#{self.discriminator}"""
 
     @property
     def created_at(self) -> datetime.datetime:
         """Returns the time in which the User was created
 
         Returns:
             datetime.datetime: The timestamp
         """
-        return datetime.datetime.utcfromtimestamp(((int(self.id) >> 22) + 1420070400000) / 1000)
+        return datetime.datetime.utcfromtimestamp(
+            ((int(self.id) >> 22) + 1420070400000) / 1000
+        )
 
     @property
     def b64token(self) -> str:
         """Returns the b64 user id
 
         Returns:
             str: The b64 user id
         """
         return str(b64encode(self.id.encode("utf-8")), "utf-8")
 
-
     def _update(self, data):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
         self.name = data.get("username")
         self.id = data.get("id")
         self.discriminator = data.get("discriminator")
         self.avatar = data.get("avatar")
         self.banner = data.get("banner")
-        self.accent_colour = data.get('accent_color')
-        self.public_flags = data.get('public_flags')
-        self.bot_acc = data.get('bot')
-        self.avatar_url = f"https://cdn.discordapp.com/avatars/{self.id}/{self.avatar}.png?size=4096" if self.avatar!=None else None
-        self.banner_url = f"https://cdn.discordapp.com/banners/{self.id}/{self.banner}.png?size=1024" if self.banner!=None else None
-        self.system = data.get('system')
-
+        self.accent_colour = data.get("accent_color")
+        self.public_flags = data.get("public_flags")
+        self.bot_acc = data.get("bot")
+        self.avatar_url = (
+            f"https://cdn.discordapp.com/avatars/{self.id}/{self.avatar}.png?size=4096"
+            if self.avatar != None
+            else None
+        )
+        self.banner_url = (
+            f"https://cdn.discordapp.com/banners/{self.id}/{self.banner}.png?size=1024"
+            if self.banner != None
+            else None
+        )
+        self.system = data.get("system")
 
     async def create_dm(self):
-        """Create a dm for the user
-        """
-        await self.http.request(method="post", endpoint="/users/@me/channels", json={"recipients": [self.id]})
-
+        """Create a dm for the user"""
+        await self.http.request(
+            method="post",
+            endpoint="/users/@me/channels",
+            json={"recipients": [self.id]},
+        )
 
     async def get_profile(self) -> Profile:
         """Get the User profile
 
         Returns:
             Profile: The User Profile object
         """
-        data = await self.http.request(method="get", endpoint=f"/users/{self.id}/profile?with_mutual_guilds=true")
+        data = await self.http.request(
+            method="get", endpoint=f"/users/{self.id}/profile?with_mutual_guilds=true"
+        )
 
         if data != None:
             data = Profile(data, self.bot, self.http)
 
         return data
 
     async def get_mutual_friends(self) -> list[User]:
         """Get the User mutual friends
 
         Returns:
             list[User]: Mutual friends
         """
-        data = await self.http.request(method="get", endpoint=f"/users/{self.id}/relationships")
+        data = await self.http.request(
+            method="get", endpoint=f"/users/{self.id}/relationships"
+        )
 
         if len(data) != 0:
             return [User(user, self.bot, self.http) for user in data]
         else:
             return []
-
```

### Comparing `selfcord.py-0.1.7/selfcord/models/webhook.py` & `selfcord.py-0.1.8/selfcord/models/webhook.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from __future__ import annotations
 
+
 class Webhook:
     def __init__(self, data: dict, bot, http) -> None:
         self.http = http
         self.bot = bot
         self._update(data)
 
+    def __eq__(self, other):
+        return self.id == other.id
+
     def _update(self, data):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
         self.id = data.get("id")
@@ -26,13 +30,18 @@
 
     async def send(self, content: str):
         """Send a message via the webhook
 
         Args:
             content (str): Content of the message to send
         """
-        await self.http.request(method = "post", endpoint = f"/webhooks/{self.id}/{self.token}", json = {"content": content})
+        await self.http.request(
+            method="post",
+            endpoint=f"/webhooks/{self.id}/{self.token}",
+            json={"content": content},
+        )
 
     async def delete(self):
-        """Deletes the webhook object
-        """
-        await self.http.request(method = "delete", endpoint = f"/webhooks/{self.id}/{self.token}")
+        """Deletes the webhook object"""
+        await self.http.request(
+            method="delete", endpoint=f"/webhooks/{self.id}/{self.token}"
+        )
```

### Comparing `selfcord.py-0.1.7/selfcord/utils/command.py` & `selfcord.py-0.1.8/selfcord/utils/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 from __future__ import annotations
+
 import inspect
 import re
 from collections import defaultdict
-from .logging import logging
 from traceback import format_exception
+from typing import TYPE_CHECKING, Any
+
+from .logging import logging
+
+if TYPE_CHECKING:
+    from ..api import *
+    from ..bot import Bot
+    from ..models import *
+
 
 log = logging.getLogger("Commands")
 
+
 class Extension:
-    """Extension object. Discord.py equivalent of cogs, a helper system to help manage and organise code into multiple files
-    """
+    """Extension object. Discord.py equivalent of cogs, a helper system to help manage and organise code into multiple files"""
+
     def __init__(self, **kwargs):
         self.name: str | None = kwargs.get("name")
-        self.description: str | None = kwargs.get('description')
-        self.ext = kwargs.get("ext")
+        self.description: str | None = kwargs.get("description")
+        self.ext: Extension | None = kwargs.get("ext")
         self._events = defaultdict(list)
-        _events = self.ext._events
-        commands = self.ext.commands
+        _events: defaultdict = self.ext._events
+        commands: CommandCollection = self.ext.commands
         self.commands = CommandCollection()
         for cmd in commands.recents():
             setattr(cmd, "ext", self.ext)
             self.commands.add(cmd)
         self.commands.copy()
         commands.clear()
         self._events.update(_events)
         _events.clear()
 
 
-
-
 class ExtensionCollection:
-    """Extension collection, where extensions are stored into. Utilised for Extender, Extensions as a whole. This is also used within help commands and command invocation.
-    """
+    """Extension collection, where extensions are stored into. Utilised for Extender, Extensions as a whole. This is also used within help commands and command invocation."""
+
     def __init__(self):
         self.extensions = {}
 
     def __iter__(self):
         for cmd in self.extensions.values():
             yield cmd
 
@@ -69,15 +77,15 @@
         if not isinstance(ext, Extension):
             log.error(f"ext is not an Extension or subclass of Extension")
         if self._is_already_registered(ext):
             log.error("Name or Alias is already registered")
         # Add extension to the collection
         self.extensions[ext.name] = ext
 
-    def get(self, alias: str) -> Extension:
+    def get(self, alias: str) -> Extension | None:
         """Get an extension
 
         Args:
             alias (str): Name of the extension
 
         Returns:
             Extension: Extension obtained
@@ -87,35 +95,36 @@
         except KeyError as e:
             log.error(f"{e}")
         for extension in self.extensions:
             if extension.name in extension.aliases:
                 return extension
 
 
-
 class Command:
-    """Command Object pretty much
-    """
+    """Command Object pretty much"""
+
     def __init__(self, **kwargs):
-        self.name = kwargs.get("name")
-        self.aliases = [self.name] + kwargs.get('aliases', [])
-        self.description = kwargs.get('description')
-        self.func = kwargs.get("func")
-        self.check = inspect.signature(self.func).return_annotation
+        self.name: str | None = kwargs.get("name")
+        self.aliases: list[str] | None = [self.name] + kwargs.get("aliases", [])
+        self.description: str | None = kwargs.get("description")
+        self.func: function | None = kwargs.get("func")
+        self.check: Any = inspect.signature(self.func).return_annotation
         self.signature = inspect.signature(self.func).parameters.items()
 
+
 class CommandCollection:
-    """Commands collection, where commands are stored into. Utilised for help commands and general command invocation.
-    """
+    """Commands collection, where commands are stored into. Utilised for help commands and general command invocation."""
+
     def __init__(self, **kwargs):
-        self.commands = {}
-        self.recent_commands = {}
+        self.commands: dict[CommandCollection, function] = {}
+        self.recent_commands: dict[CommandCollection, function] = {}
 
     def __len__(self):
         return len(self.commands)
+
     def __iter__(self):
         for cmd in self.commands.values():
             yield cmd
 
     def _is_already_registered(self, cmd: Command) -> bool:
         """Whether the specified Command is already registered
 
@@ -174,25 +183,23 @@
         Yields:
             Generator: [Command]
         """
         for cmd in self.recent_commands.values():
             yield cmd
 
     def copy(self):
-        """Copy commands from recents to main collection
-        """
+        """Copy commands from recents to main collection"""
         self.commands.update(self.recent_commands)
         self.clear()
 
     def clear(self):
-        """Clear recents
-        """
+        """Clear recents"""
         self.recent_commands.clear()
 
-    def get(self, alias) -> Command:
+    def get(self, alias) -> Command | None:
         """Get a specific command from the collection
 
         Args:
             alias (str): Name of the command
 
         Returns:
             Command: Command obtained
@@ -200,38 +207,38 @@
         try:
             return self.commands[alias]
         except KeyError as e:
             log.error(f"{e}")
         for command in self.commands:
             if alias in command.aliases:
                 return command
+
+
 class Event:
-    """Event object
-    """
-    def __init__(self, name, coro, ext) -> None:
-        self.name = name
+    """Event object"""
+
+    def __init__(self, name: str, coro, ext: Extension) -> None:
+        self.name: str = name
         self.coro = coro
-        self.ext = ext
+        self.ext: Extension = ext
 
 
 class Extender:
-    """Extender subclass for extensions, used for implementing the decorators.
-    """
+    """Extender subclass for extensions, used for implementing the decorators."""
+
     commands = CommandCollection()
-    _events = defaultdict(list)
-    def __init_subclass__(cls, name: str =None, description: str="") -> None:
+    _events: defaultdict = defaultdict(list)
+
+    def __init_subclass__(cls, name: str, description: str = "") -> None:
         super().__init_subclass__()
         cls.name = name
         cls.description = description
 
-
-
-
     @classmethod
-    def cmd(cls, description: str="", aliases: list[str]=[]):
+    def cmd(cls, description: str = "", aliases: list[str] = []):
         """Decorator to add commands for the bot
 
         Args:
             description (str, optional): Description of command. Defaults to "".
             aliases (list[str], optional): Alternative names for command. Defaults to [].
 
         Raises:
@@ -241,15 +248,17 @@
             aliases = [aliases]
 
         def decorator(coro):
             name = coro.__name__
             if not inspect.iscoroutinefunction(coro):
                 log.error("Not a coroutine")
             else:
-                cmd = Command(name=name, description=description, aliases=aliases, func=coro)
+                cmd = Command(
+                    name=name, description=description, aliases=aliases, func=coro
+                )
                 cls.commands.add(cmd)
 
             return cmd
 
         return decorator
 
     @classmethod
@@ -268,16 +277,16 @@
                 cls._events[event].append(eve)
 
                 def wrapper(*args, **kwargs):
                     result = cls._events[event].append(eve)
                     return result
 
                 return wrapper
-        return decorator
 
+        return decorator
 
     @classmethod
     def add_cmd(cls, coro, description="", aliases=[]):
         """
         Function to add commands manually without decorator
 
         Args:
@@ -290,109 +299,104 @@
         """
         if isinstance(aliases, str):
             aliases = [aliases]
         name = coro.__name__
         if not inspect.iscoroutinefunction(coro):
             log.error("Not a coroutine")
         else:
-
-
-            cmd = Command(name=name, description=description, aliases=aliases, func=coro, ext=cls)
+            cmd = Command(
+                name=name, description=description, aliases=aliases, func=coro, ext=cls
+            )
             cls.commands.add(cmd)
 
 
 class Context:
-    """Context related for commands, and invocation
-    """
+    """Context related for commands, and invocation"""
+
     def __init__(self, bot, message, http) -> None:
-        self.bot = bot
+        self.bot: Bot = bot
         self.message = message
         self.http = http
 
-
     @property
-    def author(self):
+    def author(self) -> User:
         return self.message.author
 
     @property
-    def guild(self):
+    def guild(self) -> Guild:
         return self.message.guild
 
     @property
-    def channel(self):
+    def channel(self) -> Messageable | Voiceable:
         return self.message.channel
 
     @property
-    def content(self):
+    def content(self) -> str:
         return self.message.content
 
     @property
-    def command(self):
+    def command(self) -> function | None:
         if self.prefix is None:
             return None
         for command in self.bot.commands:
             for alias in command.aliases:
                 if self.content.lower().startswith(self.prefix + alias):
                     return command
         for extension in self.bot.extensions:
-
             for command in extension.commands:
-
                 for alias in command.aliases:
-
-                    if self.content.startswith(self.prefix + alias):
-
+                    if self.content.lower().split(" ")[0] == self.prefix + alias:
                         self.extension = extension.ext
                         return command
         return None
 
     @property
-    def alias(self):
+    def alias(self) -> str | None:
         for command in self.bot.commands:
             for alias in command.aliases:
                 if self.content.lower().startswith(self.prefix + alias.lower()):
                     return alias
         for extension in self.bot.extensions:
             for command in extension.commands:
                 for alias in command.aliases:
                     if self.content.lower().startswith(self.prefix + alias.lower()):
                         self.extension = extension.ext
                         return alias
         return None
 
     @property
-    def prefix(self):
+    def prefix(self) -> str | None:
         for prefix in self.bot.prefixes:
             if self.content.startswith(prefix):
                 return prefix
 
     @property
-    def command_content(self):
+    def command_content(self) -> str | None:
         """The content minus the prefix and command name, essentially the args
 
         Returns:
             str: String of content
         """
         if self.alias == None:
             return
         try:
             cut = len(self.prefix + self.alias)
             return self.content[cut:]
         except:
             return None
 
-    def get_converter(self, param):
+    def get_converter(self, param) -> type[str] | Any | None:
         if param.annotation is param.empty:
             return str
         if callable(param.annotation):
             return param.annotation
         else:
             log.error("Parameter annotation must be callable")
 
-    def convert(self, param, value):
+    def convert(self, param, value) -> str | Any:
         """Attempts to turn x value in y value, using get_converter func for the values
 
         Args:
             param (_type_): function parameter
             value (_type_): value in message
 
         Returns:
@@ -403,16 +407,16 @@
 
     async def get_arguments(self) -> tuple[list, dict]:
         """Get arguments by checking function arguments and comparing to arguments in message.
 
         Returns:
             _type_: _description_
         """
-        args = []
-        kwargs = {}
+        args: list[Any] = []
+        kwargs: dict[Any, Any] = {}
 
         if self.command.signature is not None:
             signature = self.command.signature
         if self.command_content != "":
             splitted = self.command_content.split(" ")[1:]
 
             for index, item in enumerate(splitted):
@@ -422,121 +426,98 @@
                     if len(x) > 0:
                         val = x[0]
                         splitted[index] = val
                 break
         else:
             return args, kwargs
 
-
-
-
         for index, (name, param) in enumerate(signature):
             if name == "ctx" or name == "self":
                 continue
 
-
             if param.kind is param.POSITIONAL_OR_KEYWORD:
                 try:
-
-                    arg = self.convert(param, splitted.pop(0))
+                    arg: str | Any = self.convert(param, splitted.pop(0))
                     args.append(arg)
-                except:
+                except Exception:
                     pass
             if param.kind is param.VAR_KEYWORD:
-
                 for arg in splitted:
                     arg = self.convert(param, arg)
                     args.append(arg)
 
-
             if param.kind is param.KEYWORD_ONLY:
-
-                arg = self.convert(param, ' '.join(splitted))
+                arg = self.convert(param, " ".join(splitted))
                 kwargs[name] = arg
 
-
         for key in kwargs.copy():
             if not kwargs[key]:
                 kwargs.pop(key)
 
         return args, kwargs
 
-
-
-
     async def invoke(self):
-        """Used to actually run the command
-        """
+        """Used to actually run the command"""
         if self.command is None:
             return
         if not self.bot.userbot:
             if self.message.author.id != self.bot.user.id:
                 return
         if self.command_content != None:
             args, kwargs = await self.get_arguments()
             func = self.command.func
             if func.__code__.co_varnames[0] == "self":
-
                 args.insert(0, self.extension)
                 args.insert(1, self)
             else:
-
                 args.insert(0, self)
         try:
             await func(*args, **kwargs)
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Could not run command \n{error}")
 
-
-
-
-    async def reply(self, content: str, tts=False):
+    async def reply(self, content: str, tts=False) -> Message:
         """Helper function to reply to your own message containing the command
 
         Args:
             content (str): The message you would like to send
             tts (bool, optional): Whether message should be tts or not. Defaults to False.
         """
-        message = await self.channel.reply(self.message, content, tts)
+        message: Message = await self.channel.reply(self.message, content, tts)
         return message
 
-    async def send(self, content: str, tts=False):
+    async def send(self, content: str, tts=False) -> Message:
         """Helper function to send message to the current channel
 
         Args:
             content (str): The message you would like to send
             tts (bool, optional): Whether message should be tts or not. Defaults to False.
         """
-        message = await self.channel.send( content=content, tts=tts)
+        message: Message = await self.channel.send(content=content, tts=tts)
         return message
 
     async def spam(self, amount: int, content: str):
         """Helper function to spam messages in the current channel (uses asyncio.gather !!!!)
 
         Args:
             amount (int): Amount of messages to spam
             content (str): The message you would like to send
         """
         await self.channel.spam(amount, content)
 
-    async def purge(self, amount: int=None):
+    async def purge(self, amount: int = 0):
         """Helper function to purge messages in the current channel, uses asyncio gather.
 
         Args:
             amount (int): The amount of messages to purge, defaults to All.
         """
         await self.channel.purge(amount)
 
-    async def edit(self, content: str):
+    async def edit(self, content: str) -> Message:
         """Helper function to edit the message you sent
 
         Args:
             content (str): Content to edit to
         """
         message = await self.message.edit(content)
         return message
-
-
-
-
-
```

### Comparing `selfcord.py-0.1.7/selfcord/utils/logging.py` & `selfcord.py-0.1.8/selfcord/utils/logging.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import logging
-
 import logging.config
 
-logging.config.dictConfig({
-    'version': 1,
-    'disable_existing_loggers': True,
-})
+logging.config.dictConfig(
+    {
+        "version": 1,
+        "disable_existing_loggers": True,
+    }
+)
 
 logging.getLogger("websockets.client").disabled = True
 logging.getLogger("urllib3.connectionpool").disabled = True
 
 FMT = "[{asctime}][{levelname:^9}] {name}: {message}"
 
 FORMATS = {
     logging.DEBUG: f"\33[93m{FMT}\33[0m",
     logging.INFO: f"\33[34m{FMT}\33[0m",
     logging.WARNING: f"\33[33m{FMT}\33[0m",
     logging.ERROR: f"\33[31m{FMT}\33[0m",
     logging.CRITICAL: "\33[31m{message}\33[0m",
 }
 
+
 class CustomFormatter(logging.Formatter):
     def format(self, record: logging.LogRecord) -> str:
         log_fmt = FORMATS[record.levelno]
         formatter = logging.Formatter(log_fmt, style="{", datefmt="%H:%M:%S")
         return formatter.format(record)
 
+
 handler = logging.StreamHandler()
 handler.setFormatter(CustomFormatter())
 
 logging.basicConfig(
     level=logging.DEBUG,
     handlers=[handler],
-)
+)
```

### Comparing `selfcord.py-0.1.7/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.1.8/selfcord.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
@@ -23,15 +23,14 @@
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
-
  - Modern Pythonic API using `async`/`await` syntax
  - Easy to use with an object oriented design
  - Optimised for both speed and memory
  - Prevents detection of user account automation
  - Clean Documentation
  - Community Support
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.7 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.8 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown Provides-Extra: voice
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
```

### Comparing `selfcord.py-0.1.7/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.1.8/selfcord.py.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 selfcord/api/voice/__init__.py
 selfcord/api/voice/voice.py
 selfcord/models/__init__.py
 selfcord/models/channel.py
 selfcord/models/client.py
 selfcord/models/emoji.py
 selfcord/models/guild.py
+selfcord/models/interactions.py
 selfcord/models/member.py
 selfcord/models/message.py
 selfcord/models/permission.py
 selfcord/models/role.py
 selfcord/models/user.py
 selfcord/models/webhook.py
 selfcord/utils/__init__.py
```

### Comparing `selfcord.py-0.1.7/setup.py` & `selfcord.py-0.1.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,39 @@
-from setuptools import setup, find_packages
 from pathlib import Path
+
+from setuptools import find_packages, setup
+
 this_directory = Path(__file__).parent
 if __name__ == "__main__":
-
     this_directory = Path(__file__).parent
-    long_description = ( this_directory /"README.md").read_text()
+    long_description = (this_directory / "README.md").read_text()
     setup(
         name="selfcord.py",
-        packages=find_packages(include=['selfcord', 'selfcord.api', 'selfcord.utils', 'selfcord.models', 'selfcord.api.voice']),
-        version="0.1.7",
+        packages=find_packages(
+            include=[
+                "selfcord",
+                "selfcord.api",
+                "selfcord.utils",
+                "selfcord.models",
+                "selfcord.api.voice",
+            ]
+        ),
+        version="0.1.8",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell",
-        extras_require={"voice": ["pynacl==1.5.0","opuslib==3.0.1"]},
+        extras_require={"voice": ["pynacl==1.5.0", "opuslib==3.0.1"]},
         license="MIT",
-        install_requires=["aiohttp==3.7.4.post0","aioconsole==0.3.3", "websockets==10.1", "requests"],
-        setup_requires=['pytest-runner'],
-        tests_require=['pytest'],
-        test_suite='tests',
+        install_requires=[
+            "aiohttp==3.7.4.post0",
+            "aioconsole==0.3.3",
+            "websockets==10.1",
+            "requests",
+        ],
+        setup_requires=["pytest-runner"],
+        tests_require=["pytest"],
+        test_suite="tests",
         keywords=["selfbot", "discord", "discordapi", "discordwrapper"],
         long_description=long_description,
         url="https://github.com/Shell1010/Selfcord",
         long_description_content_type="text/markdown",
     )
```

