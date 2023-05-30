# Comparing `tmp/xiaogpt-1.44.tar.gz` & `tmp/xiaogpt-1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-1.44.tar", last modified: Sun May  7 13:13:46 2023, max compression
+gzip compressed data, was "xiaogpt-1.45.tar", last modified: Tue May 30 12:09:42 2023, max compression
```

## Comparing `xiaogpt-1.44.tar` & `xiaogpt-1.45.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-05-07 13:13:38.724300 xiaogpt-1.44/LICENSE
--rw-r--r--   0        0        0    11110 2023-05-07 13:13:38.724300 xiaogpt-1.44/README.md
--rw-r--r--   0        0        0      919 2023-05-07 13:13:46.828448 xiaogpt-1.44/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/__main__.py
--rw-r--r--   0        0        0      639 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0      554 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3275 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1605 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/bot/gpt3_bot.py
--rw-r--r--   0        0        0     1996 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3415 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/cli.py
--rw-r--r--   0        0        0     5263 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/config.py
--rw-r--r--   0        0        0     2071 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/utils.py
--rw-r--r--   0        0        0    18548 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    11696 1970-01-01 00:00:00.000000 xiaogpt-1.44/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-30 12:09:33.756188 xiaogpt-1.45/LICENSE
+-rw-r--r--   0        0        0    11390 2023-05-30 12:09:33.756188 xiaogpt-1.45/README.md
+-rw-r--r--   0        0        0      919 2023-05-30 12:09:42.272281 xiaogpt-1.45/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/__main__.py
+-rw-r--r--   0        0        0      639 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0      554 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3275 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1605 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/bot/gpt3_bot.py
+-rw-r--r--   0        0        0     1996 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3415 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/cli.py
+-rw-r--r--   0        0        0     5263 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/config.py
+-rw-r--r--   0        0        0     2071 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/utils.py
+-rw-r--r--   0        0        0    18548 2023-05-30 12:09:33.756188 xiaogpt-1.45/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    11976 1970-01-01 00:00:00.000000 xiaogpt-1.45/PKG-INFO
```

### Comparing `xiaogpt-1.44/LICENSE` & `xiaogpt-1.45/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.44/README.md` & `xiaogpt-1.45/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,25 @@
 ![image](https://user-images.githubusercontent.com/15976103/220028375-c193a859-48a1-4270-95b6-ef540e54a621.png)
 ![image](https://user-images.githubusercontent.com/15976103/226802344-9c71f543-b73c-4a47-8703-4c200c434dec.png)
 
 ## 支持的 AI 类型
 
 - GPT3
 - ChatGPT
-- New Bing
+- New Bing 
+
+## Windows 获取小米音响DID
+
+1. `pip install miservice_fork`
+2. `set MI_USER=xxxx`
+3. `set MI_PASS=xxx`
+4. 得到did
+5. `set MI_DID=xxxx`
+6. 具体可参考 `一键启动.bat` 脚本
+- 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
 
 ## 一点原理
 
 [不用 root 使用小爱同学和 ChatGPT 交互折腾记](https://github.com/yihong0618/gitblog/issues/258)
 
 ## 准备
```

### Comparing `xiaogpt-1.44/pyproject.toml` & `xiaogpt-1.45/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "openai",
     "aiohttp",
     "rich",
     "edge-tts>=6.1.3",
     "EdgeGPT==0.1.26",
 ]
 dynamic = []
-version = "1.44"
+version = "1.45"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-1.44/xiaogpt/bot/__init__.py` & `xiaogpt-1.45/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.44/xiaogpt/bot/base_bot.py` & `xiaogpt-1.45/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.44/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-1.45/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.44/xiaogpt/bot/gpt3_bot.py` & `xiaogpt-1.45/xiaogpt/bot/gpt3_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.44/xiaogpt/bot/newbing_bot.py` & `xiaogpt-1.45/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.44/xiaogpt/cli.py` & `xiaogpt-1.45/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.44/xiaogpt/config.py` & `xiaogpt-1.45/xiaogpt/config.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.44/xiaogpt/utils.py` & `xiaogpt-1.45/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.44/xiaogpt/xiaogpt.py` & `xiaogpt-1.45/xiaogpt/xiaogpt.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.44/PKG-INFO` & `xiaogpt-1.45/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 1.44
+Version: 1.45
 Summary: Play ChatGPT with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
@@ -31,15 +31,25 @@
 ![image](https://user-images.githubusercontent.com/15976103/220028375-c193a859-48a1-4270-95b6-ef540e54a621.png)
 ![image](https://user-images.githubusercontent.com/15976103/226802344-9c71f543-b73c-4a47-8703-4c200c434dec.png)
 
 ## 支持的 AI 类型
 
 - GPT3
 - ChatGPT
-- New Bing
+- New Bing 
+
+## Windows 获取小米音响DID
+
+1. `pip install miservice_fork`
+2. `set MI_USER=xxxx`
+3. `set MI_PASS=xxx`
+4. 得到did
+5. `set MI_DID=xxxx`
+6. 具体可参考 `一键启动.bat` 脚本
+- 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
 
 ## 一点原理
 
 [不用 root 使用小爱同学和 ChatGPT 交互折腾记](https://github.com/yihong0618/gitblog/issues/258)
 
 ## 准备
```

