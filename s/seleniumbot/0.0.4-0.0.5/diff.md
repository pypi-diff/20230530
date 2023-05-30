# Comparing `tmp/seleniumbot-0.0.4.tar.gz` & `tmp/seleniumbot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seleniumbot-0.0.4.tar", last modified: Tue May 30 19:02:54 2023, max compression
+gzip compressed data, was "seleniumbot-0.0.5.tar", last modified: Tue May 30 20:49:27 2023, max compression
```

## Comparing `seleniumbot-0.0.4.tar` & `seleniumbot-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 19:02:54.906433 seleniumbot-0.0.4/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4790 2023-05-30 19:02:54.906433 seleniumbot-0.0.4/PKG-INFO
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4528 2023-05-23 19:49:50.000000 seleniumbot-0.0.4/README.md
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 19:02:54.906433 seleniumbot-0.0.4/seleniumbot/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      270 2023-05-30 18:59:50.000000 seleniumbot-0.0.4/seleniumbot/__init__.py
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 19:02:54.906433 seleniumbot-0.0.4/seleniumbot/core/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      158 2023-05-23 15:57:49.000000 seleniumbot-0.0.4/seleniumbot/core/__init__.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     1450 2023-05-23 15:53:54.000000 seleniumbot-0.0.4/seleniumbot/core/action.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     3225 2023-05-25 09:00:55.000000 seleniumbot-0.0.4/seleniumbot/core/client.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     2065 2023-05-30 18:59:03.000000 seleniumbot-0.0.4/seleniumbot/core/seleniumbot.py
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 19:02:54.906433 seleniumbot-0.0.4/seleniumbot/utils/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      100 2023-05-23 15:58:29.000000 seleniumbot-0.0.4/seleniumbot/utils/__init__.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      322 2023-05-30 18:59:50.000000 seleniumbot-0.0.4/seleniumbot/utils/logger.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      634 2023-05-23 16:44:25.000000 seleniumbot-0.0.4/seleniumbot/utils/randomizer.py
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 19:02:54.906433 seleniumbot-0.0.4/seleniumbot.egg-info/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4790 2023-05-30 19:02:54.000000 seleniumbot-0.0.4/seleniumbot.egg-info/PKG-INFO
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      421 2023-05-30 19:02:54.000000 seleniumbot-0.0.4/seleniumbot.egg-info/SOURCES.txt
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)        1 2023-05-30 19:02:54.000000 seleniumbot-0.0.4/seleniumbot.egg-info/dependency_links.txt
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       23 2023-05-30 19:02:54.000000 seleniumbot-0.0.4/seleniumbot.egg-info/requires.txt
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       12 2023-05-30 19:02:54.000000 seleniumbot-0.0.4/seleniumbot.egg-info/top_level.txt
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       38 2023-05-30 19:02:54.906433 seleniumbot-0.0.4/setup.cfg
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      651 2023-05-30 19:02:49.000000 seleniumbot-0.0.4/setup.py
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 20:49:27.415940 seleniumbot-0.0.5/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4790 2023-05-30 20:49:27.415940 seleniumbot-0.0.5/PKG-INFO
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4528 2023-05-23 19:49:50.000000 seleniumbot-0.0.5/README.md
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 20:49:27.411940 seleniumbot-0.0.5/seleniumbot/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      270 2023-05-30 18:59:50.000000 seleniumbot-0.0.5/seleniumbot/__init__.py
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 20:49:27.415940 seleniumbot-0.0.5/seleniumbot/core/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      158 2023-05-23 15:57:49.000000 seleniumbot-0.0.5/seleniumbot/core/__init__.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     1495 2023-05-30 20:43:09.000000 seleniumbot-0.0.5/seleniumbot/core/action.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     3290 2023-05-30 20:39:13.000000 seleniumbot-0.0.5/seleniumbot/core/client.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     2485 2023-05-30 20:45:10.000000 seleniumbot-0.0.5/seleniumbot/core/seleniumbot.py
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 20:49:27.415940 seleniumbot-0.0.5/seleniumbot/utils/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      100 2023-05-23 15:58:29.000000 seleniumbot-0.0.5/seleniumbot/utils/__init__.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      322 2023-05-30 18:59:50.000000 seleniumbot-0.0.5/seleniumbot/utils/logger.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      634 2023-05-23 16:44:25.000000 seleniumbot-0.0.5/seleniumbot/utils/randomizer.py
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-30 20:49:27.415940 seleniumbot-0.0.5/seleniumbot.egg-info/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4790 2023-05-30 20:49:27.000000 seleniumbot-0.0.5/seleniumbot.egg-info/PKG-INFO
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      421 2023-05-30 20:49:27.000000 seleniumbot-0.0.5/seleniumbot.egg-info/SOURCES.txt
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)        1 2023-05-30 20:49:27.000000 seleniumbot-0.0.5/seleniumbot.egg-info/dependency_links.txt
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       23 2023-05-30 20:49:27.000000 seleniumbot-0.0.5/seleniumbot.egg-info/requires.txt
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       12 2023-05-30 20:49:27.000000 seleniumbot-0.0.5/seleniumbot.egg-info/top_level.txt
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       38 2023-05-30 20:49:27.415940 seleniumbot-0.0.5/setup.cfg
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      651 2023-05-30 20:46:29.000000 seleniumbot-0.0.5/setup.py
```

### Comparing `seleniumbot-0.0.4/PKG-INFO` & `seleniumbot-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seleniumbot
-Version: 0.0.4
+Version: 0.0.5
 Summary: SeleniumBot
 Home-page: https://github.com/Mercurial5
 Author: Mercurial5
 Author-email: dias.nespayev@gmail.com
 Keywords: SeleniumBot
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `seleniumbot-0.0.4/README.md` & `seleniumbot-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `seleniumbot-0.0.4/seleniumbot/core/action.py` & `seleniumbot-0.0.5/seleniumbot/core/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 from seleniumbot.core.client import SeleniumClient
 from seleniumbot.utils import get_logger
 
 logger = get_logger()
 
 
+class ActionException(Exception):
+    pass
+
+
 class Action(ABC):
     name: str
     coefficient: float
 
     # If after specific action previous actions may be outdated, make this property True
     flush_actions: bool = False
```

### Comparing `seleniumbot-0.0.4/seleniumbot/core/client.py` & `seleniumbot-0.0.5/seleniumbot/core/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,17 @@
         expect = expected_conditions.presence_of_element_located((by, value))
         return WebDriverWait(self._driver, self.__webdriver_wait_time).until(expect)
 
     @_delay
     def send_keys(self, element: WebElement, value: str) -> None:
         element.send_keys(value)
 
+    def get_driver(self) -> Chrome:
+        return self._driver
+
     def __del__(self):
         self._driver.close()
 
     def __get_driver(self, options: Options | None, seleniumwire_options: dict | None) -> Chrome:
         if not options:
             options = self.__get_default_options()
         if not seleniumwire_options:
```

### Comparing `seleniumbot-0.0.4/seleniumbot/core/seleniumbot.py` & `seleniumbot-0.0.5/seleniumbot/core/seleniumbot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,52 @@
-import inspect
 import random
+from datetime import timedelta, datetime
 from typing import Type
 
-from seleniumbot.core.action import Action, AFKAction
+from seleniumbot.core.action import Action, AFKAction, ActionException
 from seleniumbot.core.client import SeleniumClient
+from seleniumbot.utils import get_logger
 from seleniumbot.utils.randomizer import Randomizer
 
+logger = get_logger(__name__)
+
 
 class SeleniumBot:
-    def __init__(self, start_action: Type[Action] | Action, **kwargs):
+    def __init__(self, start_action: Type[Action], work_time: timedelta, **kwargs):
+        self.start_time = datetime.now()
+        self.end_time = self.start_time + work_time
+
         options = kwargs.get('options')
         seleniumwire_options = kwargs.get('seleniumwire_options')
         self.client = SeleniumClient(options=options, seleniumwire_options=seleniumwire_options)
 
         self.navigations = []
         self.actions: list[Action] = []
         self.last_action: Action | None = None
 
-        if inspect.isclass(start_action):
-            start_action = start_action()
-
-        start_action.execute(self.client, self.last_action)
+        start_action().execute(self.client, self.last_action)
 
         self.history = set()
 
         self.__comp = lambda action, x: action.coefficient > x
 
     def set_navigation_actions(self, actions: list[Type[Action]]):
         self.navigations = [action() for action in actions]
 
     def start(self) -> None:
         while True:
-            self._run_action()
+            if datetime.now() > self.end_time:
+                logger.info('Work time ended, going home. Bye.')
+                break
+
+            try:
+                self._run_action()
+            except ActionException as e:
+                logger.error(f'ActionException raised - {e}')
+                break
 
     def _run_action(self) -> None:
         if not self.actions:
             action = Randomizer.random_item_from_list(items=self.navigations, comp=self.__comp, default=AFKAction())
             new_actions = action.execute(self.client, self.last_action)
             self.__set_actions(new_actions)
         else:
```

### Comparing `seleniumbot-0.0.4/seleniumbot/utils/randomizer.py` & `seleniumbot-0.0.5/seleniumbot/utils/randomizer.py`

 * *Files identical despite different names*

### Comparing `seleniumbot-0.0.4/seleniumbot.egg-info/PKG-INFO` & `seleniumbot-0.0.5/seleniumbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seleniumbot
-Version: 0.0.4
+Version: 0.0.5
 Summary: SeleniumBot
 Home-page: https://github.com/Mercurial5
 Author: Mercurial5
 Author-email: dias.nespayev@gmail.com
 Keywords: SeleniumBot
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `seleniumbot-0.0.4/setup.py` & `seleniumbot-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='seleniumbot',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     url='https://github.com/Mercurial5',
     author='Mercurial5',
     author_email='dias.nespayev@gmail.com',
     keywords='SeleniumBot',
     description='SeleniumBot',
     python_requires=">=3.11",
```

