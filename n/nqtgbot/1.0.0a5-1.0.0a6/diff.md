# Comparing `tmp/nqtgbot-1.0.0a5.tar.gz` & `tmp/nqtgbot-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nqtgbot-1.0.0a5.tar", max compression
+gzip compressed data, was "nqtgbot-1.0.0a6.tar", max compression
```

## Comparing `nqtgbot-1.0.0a5.tar` & `nqtgbot-1.0.0a6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      557 2023-03-26 09:02:50.446375 nqtgbot-1.0.0a5/LICENSE
--rw-r--r--   0        0        0      368 2023-05-20 13:15:49.684187 nqtgbot-1.0.0a5/README.md
--rw-r--r--   0        0        0        0 2022-10-25 20:19:55.516251 nqtgbot-1.0.0a5/nqtgbot/__init__.py
--rw-r--r--   0        0        0     1174 2022-10-27 17:57:15.551527 nqtgbot-1.0.0a5/nqtgbot/message.py
--rw-r--r--   0        0        0     2253 2022-11-17 19:12:38.249444 nqtgbot-1.0.0a5/nqtgbot/provider.py
--rw-r--r--   0        0        0     1336 2023-01-22 20:06:46.830008 nqtgbot-1.0.0a5/nqtgbot/quotas.py
--rw-r--r--   0        0        0      264 2022-10-25 20:19:55.516251 nqtgbot-1.0.0a5/nqtgbot/resources/config_schema.json
--rw-r--r--   0        0        0     1294 2023-05-22 11:06:32.697850 nqtgbot-1.0.0a5/pyproject.toml
--rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 nqtgbot-1.0.0a5/PKG-INFO
+-rw-r--r--   0        0        0      557 2023-03-26 09:02:50.446375 nqtgbot-1.0.0a6/LICENSE
+-rw-r--r--   0        0        0      368 2023-05-20 13:15:49.684187 nqtgbot-1.0.0a6/README.md
+-rw-r--r--   0        0        0        0 2022-10-25 20:19:55.516251 nqtgbot-1.0.0a6/nqtgbot/__init__.py
+-rw-r--r--   0        0        0     1174 2022-10-27 17:57:15.551527 nqtgbot-1.0.0a6/nqtgbot/message.py
+-rw-r--r--   0        0        0     2253 2022-11-17 19:12:38.249444 nqtgbot-1.0.0a6/nqtgbot/provider.py
+-rw-r--r--   0        0        0     1336 2023-01-22 20:06:46.830008 nqtgbot-1.0.0a6/nqtgbot/quotas.py
+-rw-r--r--   0        0        0      264 2022-10-25 20:19:55.516251 nqtgbot-1.0.0a6/nqtgbot/resources/config_schema.json
+-rw-r--r--   0        0        0     1294 2023-05-30 12:02:06.035772 nqtgbot-1.0.0a6/pyproject.toml
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 nqtgbot-1.0.0a6/PKG-INFO
```

### Comparing `nqtgbot-1.0.0a5/LICENSE` & `nqtgbot-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `nqtgbot-1.0.0a5/nqtgbot/message.py` & `nqtgbot-1.0.0a6/nqtgbot/message.py`

 * *Files identical despite different names*

### Comparing `nqtgbot-1.0.0a5/nqtgbot/provider.py` & `nqtgbot-1.0.0a6/nqtgbot/provider.py`

 * *Files identical despite different names*

### Comparing `nqtgbot-1.0.0a5/nqtgbot/quotas.py` & `nqtgbot-1.0.0a6/nqtgbot/quotas.py`

 * *Files identical despite different names*

### Comparing `nqtgbot-1.0.0a5/pyproject.toml` & `nqtgbot-1.0.0a6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry_core >= 1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nqtgbot"
-version = "1.0.0-alpha-5"
+version = "1.0.0-alpha-6"
 description = "NQ Telegram Bot Provider"
 authors = [ "Inqana Ltd. <develop@inqana.com>",]
 readme = "README.md"
 classifiers = [ "Development Status :: 3 - Alpha", "Intended Audience :: Developers", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 
 [tool.black]
 line-length = 100
@@ -27,15 +27,15 @@
 known_third_party = [ "nqsdk",]
 sections = [ "FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER",]
 no_lines_before = "LOCALFOLDER"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 python-telegram-bot = "^13.14"
-nqsdk = "1.0.0a14"
+nqsdk = "1.0.0a16"
 
 [tool.pytest.ini_options]
 addopts = [ "-s",]
 testpaths = [ "tests",]
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20"
```

### Comparing `nqtgbot-1.0.0a5/PKG-INFO` & `nqtgbot-1.0.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nqtgbot
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: NQ Telegram Bot Provider
 Author: Inqana Ltd.
 Author-email: develop@inqana.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nqsdk (==1.0.0a14)
+Requires-Dist: nqsdk (==1.0.0a16)
 Requires-Dist: python-telegram-bot (>=13.14,<14.0)
 Description-Content-Type: text/markdown
 
 # NQ Telegram Bot Provider
 
 Part of NQ suite by [Inqana](https://inqana.com). Built with [NQ SDK](https://pypi.org/project/nqsdk/).
```

