# Comparing `tmp/ipymock-1.1.1.tar.gz` & `tmp/ipymock-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-1.1.1.tar", last modified: Fri May  5 04:55:09 2023, max compression
+gzip compressed data, was "ipymock-1.1.2.tar", last modified: Tue May 30 15:37:37 2023, max compression
```

## Comparing `ipymock-1.1.1.tar` & `ipymock-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-05 04:55:09.896762 ipymock-1.1.1/
--rw-rw-r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.1.1/LICENSE
--rw-rw-r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.1.1/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)    11160 2023-05-05 04:55:09.896135 ipymock-1.1.1/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)    10417 2023-05-05 04:51:03.000000 ipymock-1.1.1/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-05 04:55:09.889799 ipymock-1.1.1/ipymock/
--rw-rw-r--   0 saintway   (501) staff       (20)     1605 2023-05-05 04:52:19.000000 ipymock-1.1.1/ipymock/__init__.py
--rw-rw-r--   0 saintway   (501) staff       (20)     3343 2023-05-05 04:52:19.000000 ipymock-1.1.1/ipymock/_nbdev.py
--rw-rw-r--   0 saintway   (501) staff       (20)    18079 2023-05-05 04:52:19.000000 ipymock-1.1.1/ipymock/agi.py
--rw-rw-r--   0 saintway   (501) staff       (20)    20838 2023-05-05 04:52:19.000000 ipymock-1.1.1/ipymock/browser.py
--rw-rw-r--   0 saintway   (501) staff       (20)      995 2023-05-05 04:52:19.000000 ipymock-1.1.1/ipymock/llm.py
--rw-rw-r--   0 saintway   (501) staff       (20)     2974 2023-05-05 04:52:19.000000 ipymock-1.1.1/ipymock/reader.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-05 04:55:09.893736 ipymock-1.1.1/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-05 04:55:09.895132 ipymock-1.1.1/ipymock.egg-info/.ipynb_checkpoints/
--rw-rw-r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.1.1/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.1.1/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-rw-r--   0 saintway   (501) staff       (20)    11160 2023-05-05 04:55:09.000000 ipymock-1.1.1/ipymock.egg-info/PKG-INFO
--rw-rw-r--   0 saintway   (501) staff       (20)      460 2023-05-05 04:55:09.000000 ipymock-1.1.1/ipymock.egg-info/SOURCES.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-05-05 04:55:09.000000 ipymock-1.1.1/ipymock.egg-info/dependency_links.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.1.1/ipymock.egg-info/not-zip-safe
--rw-rw-r--   0 saintway   (501) staff       (20)      181 2023-05-05 04:55:09.000000 ipymock-1.1.1/ipymock.egg-info/requires.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-05-05 04:55:09.000000 ipymock-1.1.1/ipymock.egg-info/top_level.txt
--rw-rw-r--   0 saintway   (501) staff       (20)     2662 2023-05-05 04:51:47.000000 ipymock-1.1.1/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-05-05 04:55:09.896918 ipymock-1.1.1/setup.cfg
--rw-rw-r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.1.1/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-30 15:37:37.037762 ipymock-1.1.2/
+-rw-rw-r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.1.2/LICENSE
+-rw-rw-r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.1.2/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)    11109 2023-05-30 15:37:37.037257 ipymock-1.1.2/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)    10366 2023-05-30 15:37:22.000000 ipymock-1.1.2/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-30 15:37:37.032378 ipymock-1.1.2/ipymock/
+-rw-rw-r--   0 saintway   (501) staff       (20)     1605 2023-05-30 15:37:02.000000 ipymock-1.1.2/ipymock/__init__.py
+-rw-rw-r--   0 saintway   (501) staff       (20)     3398 2023-05-30 15:37:02.000000 ipymock-1.1.2/ipymock/_nbdev.py
+-rw-rw-r--   0 saintway   (501) staff       (20)    18079 2023-05-30 15:37:02.000000 ipymock-1.1.2/ipymock/agi.py
+-rw-rw-r--   0 saintway   (501) staff       (20)    21444 2023-05-30 15:37:02.000000 ipymock-1.1.2/ipymock/browser.py
+-rw-rw-r--   0 saintway   (501) staff       (20)      995 2023-05-30 15:37:02.000000 ipymock-1.1.2/ipymock/llm.py
+-rw-rw-r--   0 saintway   (501) staff       (20)     2974 2023-05-30 15:37:02.000000 ipymock-1.1.2/ipymock/reader.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-30 15:37:37.034589 ipymock-1.1.2/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-30 15:37:37.036521 ipymock-1.1.2/ipymock.egg-info/.ipynb_checkpoints/
+-rw-rw-r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.1.2/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.1.2/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)    11109 2023-05-30 15:37:36.000000 ipymock-1.1.2/ipymock.egg-info/PKG-INFO
+-rw-rw-r--   0 saintway   (501) staff       (20)      460 2023-05-30 15:37:36.000000 ipymock-1.1.2/ipymock.egg-info/SOURCES.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-05-30 15:37:36.000000 ipymock-1.1.2/ipymock.egg-info/dependency_links.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.1.2/ipymock.egg-info/not-zip-safe
+-rw-rw-r--   0 saintway   (501) staff       (20)      198 2023-05-30 15:37:36.000000 ipymock-1.1.2/ipymock.egg-info/requires.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-05-30 15:37:36.000000 ipymock-1.1.2/ipymock.egg-info/top_level.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)     2686 2023-05-30 15:37:26.000000 ipymock-1.1.2/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-05-30 15:37:37.037851 ipymock-1.1.2/setup.cfg
+-rw-rw-r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.1.2/setup.py
```

### Comparing `ipymock-1.1.1/LICENSE` & `ipymock-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-1.1.1/PKG-INFO` & `ipymock-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
@@ -15,18 +15,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Running PyTest in Jupyter Notebooks
-
 > iPyMock uses GPT 3.5 turbo by browser automation and <a href='https://huggingface.co/GanymedeNil/text2vec-large-chinese'>a CoSENT based model</a> to embed English and Chinese.
 
-[![Discord Follow](https://dcbadge.vercel.app/api/server/ARTMvTQv?style=flat)](https://discord.gg/ARTMvTQv)
+
+[![Discord Follow](https://dcbadge.vercel.app/api/server/8YhXA7TYrC?style=flat)](https://discord.gg/8YhXA7TYrC)
 [![Twitter Follow](https://img.shields.io/twitter/follow/seii_saintway?style=social)](https://twitter.com/seii_saintway)
 
 ## Setup iPyMock
 
 `gmail_address` and `gmail_password` are needed for utilizing chrome automation locally.
 
 `conversation_id` could be found in the url of `chat.openai.com/c/<conversation_id>`.
@@ -41,15 +41,15 @@
   "conversation_id": "<conversation_id>"
 }
 EOF
 
 pip install --upgrade ipymock
 ```
 
-`access_token` at [openai api session](https://chat.openai.com/api/auth/session) are needed for utilizing a backend api proxy.
+`access_token` at [openai api session](https://chat.openai.com/api/auth/session) is needed for utilizing a backend api proxy.
 
 ```bash
 mkdir -p ~/.config/ipymock
 
 cat << EOF > ~/.config/ipymock/config.json
 {
   "chat_gpt_base_url": "<chat_gpt_base_url>",
@@ -148,15 +148,15 @@
 
 This project is still under development and lack of documentation.
 
 This is [an article](https://seii-saintway.github.io/2023/04/06/Autonomous-Agents/) I wrote that mock openai to test autonomous robots.
 
 ## The Mechanism of PyTesting the Python Testfiles
 
-```python
+```
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -164,24 +164,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ### PyTesting the Python Testcases within iPyNb Runtimes
 
-```python
+```
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -227,15 +227,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -244,22 +244,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```python
+```
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```python
+```
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -304,34 +304,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to Use the Do-PyTest?
 
-```python
+```
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```python
+```
 from ipymock import do
 ```
 
-```python
+```
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
```

### Comparing `ipymock-1.1.1/README.md` & `ipymock-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Running PyTest in Jupyter Notebooks
-
 > iPyMock uses GPT 3.5 turbo by browser automation and <a href='https://huggingface.co/GanymedeNil/text2vec-large-chinese'>a CoSENT based model</a> to embed English and Chinese.
 
-[![Discord Follow](https://dcbadge.vercel.app/api/server/ARTMvTQv?style=flat)](https://discord.gg/ARTMvTQv)
+
+[![Discord Follow](https://dcbadge.vercel.app/api/server/8YhXA7TYrC?style=flat)](https://discord.gg/8YhXA7TYrC)
 [![Twitter Follow](https://img.shields.io/twitter/follow/seii_saintway?style=social)](https://twitter.com/seii_saintway)
 
 ## Setup iPyMock
 
 `gmail_address` and `gmail_password` are needed for utilizing chrome automation locally.
 
 `conversation_id` could be found in the url of `chat.openai.com/c/<conversation_id>`.
@@ -21,15 +21,15 @@
   "conversation_id": "<conversation_id>"
 }
 EOF
 
 pip install --upgrade ipymock
 ```
 
-`access_token` at [openai api session](https://chat.openai.com/api/auth/session) are needed for utilizing a backend api proxy.
+`access_token` at [openai api session](https://chat.openai.com/api/auth/session) is needed for utilizing a backend api proxy.
 
 ```bash
 mkdir -p ~/.config/ipymock
 
 cat << EOF > ~/.config/ipymock/config.json
 {
   "chat_gpt_base_url": "<chat_gpt_base_url>",
@@ -128,15 +128,15 @@
 
 This project is still under development and lack of documentation.
 
 This is [an article](https://seii-saintway.github.io/2023/04/06/Autonomous-Agents/) I wrote that mock openai to test autonomous robots.
 
 ## The Mechanism of PyTesting the Python Testfiles
 
-```python
+```
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -144,24 +144,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ### PyTesting the Python Testcases within iPyNb Runtimes
 
-```python
+```
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -207,15 +207,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -224,22 +224,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```python
+```
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```python
+```
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -284,34 +284,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to Use the Do-PyTest?
 
-```python
+```
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```python
+```
 from ipymock import do
 ```
 
-```python
+```
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
```

### Comparing `ipymock-1.1.1/ipymock/__init__.py` & `ipymock-1.1.2/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.1.1/ipymock/_nbdev.py` & `ipymock-1.1.2/ipymock/_nbdev.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
          "ChatGPTConverter": "2_browser.ipynb",
          "markdownize": "2_browser.ipynb",
          "init": "2_browser.ipynb",
          "login": "2_browser.ipynb",
          "open_chat": "2_browser.ipynb",
          "remove_portal": "2_browser.ipynb",
          "chatgpt_textbox": "2_browser.ipynb",
+         "chatgpt_disabled_button": "2_browser.ipynb",
          "chatgpt_streaming": "2_browser.ipynb",
          "chatgpt_response": "2_browser.ipynb",
          "chatgpt_red_500": "2_browser.ipynb",
          "chatgpt_big_response": "2_browser.ipynb",
          "chatgpt_small_response": "2_browser.ipynb",
          "request": "2_browser.ipynb",
          "get_last_response": "2_browser.ipynb",
```

### Comparing `ipymock-1.1.1/ipymock/agi.py` & `ipymock-1.1.2/ipymock/agi.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.1.1/ipymock/browser.py` & `ipymock-1.1.2/ipymock/browser.py`

 * *Files 3% similar despite different names*

```diff
@@ -361,27 +361,39 @@
     if conversation_id == '':
         common.driver.get('https://chat.openai.com')
     else:
         common.driver.get(f'https://chat.openai.com/c/{conversation_id}')
         if common.conversation_id != conversation_id:
             common.conversation_id = conversation_id
             common.parent_message_id = ''
-    remove_portal()
 
-def remove_portal():
-    WebDriverWait(common.driver, 10).until(
-        expected_conditions.presence_of_element_located((By.ID, 'headlessui-portal-root'))
+    WebDriverWait(common.driver, 30).until(
+        lambda driver: driver.execute_script('return document.readyState') == 'complete'
     )
 
-    common.driver.execute_script('''
-    document.getElementById('headlessui-portal-root').remove();
-    ''')
+    remove_portal()
+
+def remove_portal():
+    while True:
+        try:
+            WebDriverWait(common.driver, 5).until(
+                expected_conditions.element_to_be_clickable((By.XPATH, '//div[text()="Next"]'))
+            ).click()
+        except TimeoutException:
+            break
+    try:
+        WebDriverWait(common.driver, 5).until(
+            expected_conditions.element_to_be_clickable((By.XPATH, '//div[text()="Done"]'))
+        ).click()
+    except TimeoutException:
+        pass
 
 # Internal Cell
 chatgpt_textbox = (By.TAG_NAME, 'textarea')
+chatgpt_disabled_button = (By.XPATH, '//textarea/following-sibling::button[@disabled]')
 chatgpt_streaming = (By.CLASS_NAME, 'result-streaming')
 chatgpt_response = (By.XPATH, '//div[starts-with(@class, "flex flex-grow flex-col gap-3")]')
 chatgpt_red_500 = (By.XPATH, '//div[contains(@class, "border-red-500 bg-red-500/10")]')
 chatgpt_big_response = (By.XPATH, '//div[@class="flex-1 overflow-hidden"]//div[p]')
 chatgpt_small_response = (By.XPATH, '//div[starts-with(@class, "markdown prose w-full break-words")]')
 
 # Cell
@@ -400,14 +412,18 @@
     var element = arguments[0], txt = arguments[1];
     element.value += txt;
     element.dispatchEvent(new Event("change"));
     ''',
         textbox,
         prompt,
     )
+    # textbox.send_keys(prompt)
+    # WebDriverWait(common.driver, 3).until_not(
+    #     expected_conditions.presence_of_element_located(chatgpt_disabled_button)
+    # )
     textbox.send_keys(Keys.ENTER)
 
 def get_last_response():
     responses = common.driver.find_elements(*chatgpt_big_response)
     if responses != []:
         return responses[-1]
     responses = common.driver.find_elements(*chatgpt_small_response)
```

### Comparing `ipymock-1.1.1/ipymock/llm.py` & `ipymock-1.1.2/ipymock/llm.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.1.1/ipymock/reader.py` & `ipymock-1.1.2/ipymock/reader.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.1.1/ipymock.egg-info/PKG-INFO` & `ipymock-1.1.2/ipymock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
@@ -15,18 +15,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Running PyTest in Jupyter Notebooks
-
 > iPyMock uses GPT 3.5 turbo by browser automation and <a href='https://huggingface.co/GanymedeNil/text2vec-large-chinese'>a CoSENT based model</a> to embed English and Chinese.
 
-[![Discord Follow](https://dcbadge.vercel.app/api/server/ARTMvTQv?style=flat)](https://discord.gg/ARTMvTQv)
+
+[![Discord Follow](https://dcbadge.vercel.app/api/server/8YhXA7TYrC?style=flat)](https://discord.gg/8YhXA7TYrC)
 [![Twitter Follow](https://img.shields.io/twitter/follow/seii_saintway?style=social)](https://twitter.com/seii_saintway)
 
 ## Setup iPyMock
 
 `gmail_address` and `gmail_password` are needed for utilizing chrome automation locally.
 
 `conversation_id` could be found in the url of `chat.openai.com/c/<conversation_id>`.
@@ -41,15 +41,15 @@
   "conversation_id": "<conversation_id>"
 }
 EOF
 
 pip install --upgrade ipymock
 ```
 
-`access_token` at [openai api session](https://chat.openai.com/api/auth/session) are needed for utilizing a backend api proxy.
+`access_token` at [openai api session](https://chat.openai.com/api/auth/session) is needed for utilizing a backend api proxy.
 
 ```bash
 mkdir -p ~/.config/ipymock
 
 cat << EOF > ~/.config/ipymock/config.json
 {
   "chat_gpt_base_url": "<chat_gpt_base_url>",
@@ -148,15 +148,15 @@
 
 This project is still under development and lack of documentation.
 
 This is [an article](https://seii-saintway.github.io/2023/04/06/Autonomous-Agents/) I wrote that mock openai to test autonomous robots.
 
 ## The Mechanism of PyTesting the Python Testfiles
 
-```python
+```
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -164,24 +164,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ### PyTesting the Python Testcases within iPyNb Runtimes
 
-```python
+```
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -227,15 +227,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -244,22 +244,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```python
+```
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```python
+```
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -304,34 +304,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to Use the Do-PyTest?
 
-```python
+```
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```python
+```
 from ipymock import do
 ```
 
-```python
+```
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
```

### Comparing `ipymock-1.1.1/settings.ini` & `ipymock-1.1.2/settings.ini`

 * *Files 3% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 user = seii-saintway
 description = A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
 copyright = 2023 onwards, Neuro Spirit, DAO.
 branch = main
-version = 1.1.1
+version = 1.1.2
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
 # From 1-7: Planning Pre-Alpha Alpha Beta Production Mature Inactive
 status = 2
 
 # Optional. Same format as setuptools requirements
-requirements = pytest==6.* nbdev==1.* openai==0.* sentence_transformers==2.* pydantic==1.* langchain==0.* faiss-cpu==1.* duckduckgo_search==2.* undetected_chromedriver==3.* selenium_profiles==2.*
+requirements = pytest==6.* nbdev==1.* openai==0.* sentence_transformers==2.* pydantic==1.* langchain==0.* faiss-cpu==1.* duckduckgo_search==2.* undetected_chromedriver==3.* selenium_profiles==2.* markdownify==0.*
 # Optional. Same format as setuptools console_scripts
 # console_scripts = 
 # Optional. Same format as setuptools dependency-links
 # dep_links = 
 
 ###
 # You probably won't need to change anything under here,
@@ -61,15 +61,17 @@
 
 lib_path = %(lib_name)s
 title = %(lib_name)s
 
 #Optional advanced parameters
 #Monospace docstings: adds <pre> tags around the doc strings, preserving newlines/indentation.
 #monospace_docstrings = False
-#Test flags: introduce here the test flags you want to use separated by |
-#tst_flags = 
+
+# Test flags: introduce here the test flags you want to use separated by |
+tst_flags = gmail
+
 #Custom sidebar: customize sidebar.json yourself for advanced sidebars (False/True)
 #custom_sidebar = 
 #Cell spacing: if you want cell blocks in code separated by more than one new line
 #cell_spacing = 
 #Custom jekyll styles: if you want more jekyll styles than tip/important/warning, set them here
 #jekyll_styles = note,warning,tip,important
```

### Comparing `ipymock-1.1.1/setup.py` & `ipymock-1.1.2/setup.py`

 * *Files identical despite different names*

