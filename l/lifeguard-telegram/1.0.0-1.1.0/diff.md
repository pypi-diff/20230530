# Comparing `tmp/lifeguard-telegram-1.0.0.tar.gz` & `tmp/lifeguard-telegram-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-telegram-1.0.0.tar", last modified: Fri May 26 14:56:04 2023, max compression
+gzip compressed data, was "lifeguard-telegram-1.1.0.tar", last modified: Tue May 30 19:18:40 2023, max compression
```

## Comparing `lifeguard-telegram-1.0.0.tar` & `lifeguard-telegram-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:56:04.952862 lifeguard-telegram-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-26 14:56:04.952862 lifeguard-telegram-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:56:04.952862 lifeguard-telegram-1.0.0/lifeguard_telegram/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/lifeguard_telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/lifeguard_telegram/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:56:04.952862 lifeguard-telegram-1.0.0/lifeguard_telegram/bot_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/lifeguard_telegram/bot_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/lifeguard_telegram/bot_handlers/builtin_bot_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/lifeguard_telegram/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:56:04.952862 lifeguard-telegram-1.0.0/lifeguard_telegram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-26 14:56:04.000000 lifeguard-telegram-1.0.0/lifeguard_telegram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-26 14:56:04.000000 lifeguard-telegram-1.0.0/lifeguard_telegram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:56:04.000000 lifeguard-telegram-1.0.0/lifeguard_telegram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 14:56:04.000000 lifeguard-telegram-1.0.0/lifeguard_telegram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 14:56:04.000000 lifeguard-telegram-1.0.0/lifeguard_telegram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 14:56:04.952862 lifeguard-telegram-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:18:40.905910 lifeguard-telegram-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-30 19:18:40.905910 lifeguard-telegram-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:18:40.905910 lifeguard-telegram-1.1.0/lifeguard_telegram/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/lifeguard_telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/lifeguard_telegram/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:18:40.905910 lifeguard-telegram-1.1.0/lifeguard_telegram/bot_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/lifeguard_telegram/bot_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/lifeguard_telegram/bot_handlers/builtin_bot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/lifeguard_telegram/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/lifeguard_telegram/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:18:40.905910 lifeguard-telegram-1.1.0/lifeguard_telegram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-30 19:18:40.000000 lifeguard-telegram-1.1.0/lifeguard_telegram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-30 19:18:40.000000 lifeguard-telegram-1.1.0/lifeguard_telegram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:18:40.000000 lifeguard-telegram-1.1.0/lifeguard_telegram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:18:40.000000 lifeguard-telegram-1.1.0/lifeguard_telegram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-30 19:18:40.000000 lifeguard-telegram-1.1.0/lifeguard_telegram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:18:40.905910 lifeguard-telegram-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/setup.py
```

### Comparing `lifeguard-telegram-1.0.0/PKG-INFO` & `lifeguard-telegram-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-telegram
-Version: 1.0.0
+Version: 1.1.0
 Summary: Lifeguard integration with Telegram
 Home-page: https://github.com/LifeguardSystem/lifeguard-telegram
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-telegram-1.0.0/lifeguard_telegram/__init__.py` & `lifeguard-telegram-1.1.0/lifeguard_telegram/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 Lifeguard integration with Telegram
 """
-import _thread
 import os
 
+from lifeguard.notifications import append_notification_implementation
 from lifeguard.logger import lifeguard_logger as logger
 
-from lifeguard_telegram.bot import load_bot_handlers, init_updater
+from lifeguard_telegram.bot import init_updater
+from lifeguard_telegram.notifications import TelegramNotificationBase
 
 
 class LifeguardTelegramPlugin:
     """
     Telegram Plugin
     """
 
     def __init__(self, lifeguard_context):
         self.lifeguard_context = lifeguard_context
         init_updater()
 
 
 def init(lifeguard_context):
+    append_notification_implementation(TelegramNotificationBase)
     newpid = os.fork()
     if newpid == 0:
         logger.info("starting telegram process")
         LifeguardTelegramPlugin(lifeguard_context)
```

### Comparing `lifeguard-telegram-1.0.0/lifeguard_telegram/bot.py` & `lifeguard-telegram-1.1.0/lifeguard_telegram/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import sys
 from functools import wraps
 
 from lifeguard.logger import lifeguard_logger as logger
 from lifeguard.settings import LIFEGUARD_DIRECTORY
 from telegram.ext import CommandHandler, Updater
 
-from lifeguard_telegram.settings import LIFEGUARD_TELEGRAM_BOT_TOKEN
+from lifeguard_telegram.settings import TELEGRAM_API_KEY
 
 CONTEXT = {"updater": None}
 
 
 def init_updater():
     """
     Init start polling
     """
-    CONTEXT["updater"] = Updater(LIFEGUARD_TELEGRAM_BOT_TOKEN, use_context=True)
+    CONTEXT["updater"] = Updater(TELEGRAM_API_KEY, use_context=True)
 
     load_bot_handlers()
 
     CONTEXT["updater"].start_polling()
     CONTEXT["updater"].idle()
```

### Comparing `lifeguard-telegram-1.0.0/lifeguard_telegram/bot_handlers/builtin_bot_handler.py` & `lifeguard-telegram-1.1.0/lifeguard_telegram/bot_handlers/builtin_bot_handler.py`

 * *Files identical despite different names*

### Comparing `lifeguard-telegram-1.0.0/lifeguard_telegram/settings.py` & `lifeguard-telegram-1.1.0/lifeguard_telegram/settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """
 Lifeguard Telegram Settings
 """
 from lifeguard.settings import SettingsManager
 
 SETTINGS_MANAGER = SettingsManager(
     {
-        "LIFEGUARD_TELEGRAM_BOT_TOKEN": {
-            "default": "",
-            "description": "Telegram bot token",
-        },
         "LIFEGUARD_TELEGRAM_VALIDATIONS_HANDLER": {
             "default": "true",
             "description": "Enable telegram validations handler",
         },
+        "TELEGRAM_API_KEY": {
+            "default": "",
+            "description": "Telegram bot token",
+        },
+        "TELEGRAM_DEFAULT_CHAT_ID": {
+            "default": "",
+            "description": "Telegram default chat id",
+        },
     }
 )
 
-LIFEGUARD_TELEGRAM_BOT_TOKEN = SETTINGS_MANAGER.read_value(
-    "LIFEGUARD_TELEGRAM_BOT_TOKEN"
-)
 LIFEGUARD_TELEGRAM_VALIDATIONS_HANDLER_ENABLED = (
     SETTINGS_MANAGER.read_value("LIFEGUARD_TELEGRAM_VALIDATIONS_HANDLER_ENABLED")
     == "true"
 )
+TELEGRAM_API_KEY = SETTINGS_MANAGER.read_value("TELEGRAM_API_KEY")
+TELEGRAM_DEFAULT_CHAT_ID = SETTINGS_MANAGER.read_value("TELEGRAM_DEFAULT_CHAT_ID")
```

### Comparing `lifeguard-telegram-1.0.0/lifeguard_telegram.egg-info/PKG-INFO` & `lifeguard-telegram-1.1.0/lifeguard_telegram.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-telegram
-Version: 1.0.0
+Version: 1.1.0
 Summary: Lifeguard integration with Telegram
 Home-page: https://github.com/LifeguardSystem/lifeguard-telegram
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-telegram-1.0.0/setup.py` & `lifeguard-telegram-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard-telegram",
-    version="1.0.0",
+    version="1.1.0",
     url="https://github.com/LifeguardSystem/lifeguard-telegram",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=[],
     include_package_data=True,
     description="Lifeguard integration with Telegram",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["lifeguard", "python-telegram-bot"],
+    install_requires=["lifeguard", "python-telegram-bot", "telepot"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Plugins",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

