# Comparing `tmp/better_slack_logger-0.12.0.post1.tar.gz` & `tmp/better_slack_logger-0.12.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_slack_logger-0.12.0.post1.tar", max compression
+gzip compressed data, was "better_slack_logger-0.12.0.post2.tar", max compression
```

## Comparing `better_slack_logger-0.12.0.post1.tar` & `better_slack_logger-0.12.0.post2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-05-16 12:07:28.007887 better_slack_logger-0.12.0.post1/LICENSE
--rw-r--r--   0        0        0     8478 2023-05-16 12:07:28.007887 better_slack_logger-0.12.0.post1/README.md
--rw-r--r--   0        0        0     1330 2023-05-16 12:07:28.011887 better_slack_logger-0.12.0.post1/pyproject.toml
--rw-r--r--   0        0        0       67 2023-05-16 12:07:28.011887 better_slack_logger-0.12.0.post1/slack_logger/__init__.py
--rw-r--r--   0        0        0     5168 2023-05-16 12:07:28.011887 better_slack_logger-0.12.0.post1/slack_logger/message_logger.py
--rw-r--r--   0        0        0      720 2023-05-16 12:07:28.015888 better_slack_logger-0.12.0.post1/slack_logger/utils.py
--rw-r--r--   0        0        0     9767 1970-01-01 00:00:00.000000 better_slack_logger-0.12.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-30 08:42:29.108310 better_slack_logger-0.12.0.post2/LICENSE
+-rw-r--r--   0        0        0     8478 2023-05-30 08:42:29.108310 better_slack_logger-0.12.0.post2/README.md
+-rw-r--r--   0        0        0     1317 2023-05-30 08:42:29.112310 better_slack_logger-0.12.0.post2/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-05-30 08:42:29.112310 better_slack_logger-0.12.0.post2/slack_logger/__init__.py
+-rw-r--r--   0        0        0     5168 2023-05-30 08:42:29.112310 better_slack_logger-0.12.0.post2/slack_logger/message_logger.py
+-rw-r--r--   0        0        0      720 2023-05-30 08:42:29.112310 better_slack_logger-0.12.0.post2/slack_logger/utils.py
+-rw-r--r--   0        0        0     9708 1970-01-01 00:00:00.000000 better_slack_logger-0.12.0.post2/PKG-INFO
```

### Comparing `better_slack_logger-0.12.0.post1/LICENSE` & `better_slack_logger-0.12.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `better_slack_logger-0.12.0.post1/README.md` & `better_slack_logger-0.12.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `better_slack_logger-0.12.0.post1/pyproject.toml` & `better_slack_logger-0.12.0.post2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 profile = "black"
 py_version = 38
 line_length = 100
 combine_as_imports = true
 
 [tool.poetry]
 name = "better-slack-logger"
-version = "0.12.0.post1"
+version = "0.12.0.post2"
 description = "Slack Logger is a custom message logger to Slack for Python 3"
 authors = [
   "Chinni Chaitanya <chchaitanya95@gmail.com>",
-  "Jay Turner <jaynicholasturner@gmail.com>",
+  "Jay Turner <jay.turner@kayenta.io>",
 ]
-maintainers = ["Jay Turner <jaynicholasturner@gmail.com>"]
+maintainers = ["Jay Turner <jay.turner@kayenta.io>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{ include = "slack_logger" }]
-repository = "https://github.com/TurnrDev/better-slack-logger"
+repository = "https://github.com/Kayenta/better-slack-logger"
 keywords = [
   "monitoring",
   "slack",
   "messaging",
   "logging",
   "health-check",
   "notification-service",
```

### Comparing `better_slack_logger-0.12.0.post1/slack_logger/message_logger.py` & `better_slack_logger-0.12.0.post2/slack_logger/message_logger.py`

 * *Files identical despite different names*

### Comparing `better_slack_logger-0.12.0.post1/slack_logger/utils.py` & `better_slack_logger-0.12.0.post2/slack_logger/utils.py`

 * *Files identical despite different names*

### Comparing `better_slack_logger-0.12.0.post1/PKG-INFO` & `better_slack_logger-0.12.0.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: better-slack-logger
-Version: 0.12.0.post1
+Version: 0.12.0.post2
 Summary: Slack Logger is a custom message logger to Slack for Python 3
-Home-page: https://github.com/TurnrDev/better-slack-logger
+Home-page: https://github.com/Kayenta/better-slack-logger
 License: MIT
 Keywords: monitoring,slack,messaging,logging,health-check,notification-service,notification,slack-api
 Author: Chinni Chaitanya
 Author-email: chchaitanya95@gmail.com
 Maintainer: Jay Turner
-Maintainer-email: jaynicholasturner@gmail.com
+Maintainer-email: jay.turner@kayenta.io
 Requires-Python: >=3.7
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: pyyaml (>=5.1)
 Requires-Dist: slack-sdk (>=3.0.0)
-Project-URL: Repository, https://github.com/TurnrDev/better-slack-logger
+Project-URL: Repository, https://github.com/Kayenta/better-slack-logger
 Description-Content-Type: text/markdown
 
 # Better Slack Logger
 
 This is a fork is [`python-slack-logger`](https://github.com/chinnichaitanya/python-slack-logger) package by [Chaitanya Chinni](https://github.com/chinnichaitanya/). If using this, please remove that from your environment.
 
 A custom message logger to Slack for Python 3.
```

#### html2text {}

```diff
@@ -1,33 +1,32 @@
-Metadata-Version: 2.1 Name: better-slack-logger Version: 0.12.0.post1 Summary:
+Metadata-Version: 2.1 Name: better-slack-logger Version: 0.12.0.post2 Summary:
 Slack Logger is a custom message logger to Slack for Python 3 Home-page: https:
-//github.com/TurnrDev/better-slack-logger License: MIT Keywords:
+//github.com/Kayenta/better-slack-logger License: MIT Keywords:
 monitoring,slack,messaging,logging,health-check,notification-
 service,notification,slack-api Author: Chinni Chaitanya Author-email:
 chchaitanya95@gmail.com Maintainer: Jay Turner Maintainer-email:
-jaynicholasturner@gmail.com Requires-Python: >=3.7 Classifier: Environment ::
-Web Environment Classifier: Intended Audience :: Developers Classifier: License
-:: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+jay.turner@kayenta.io Requires-Python: >=3.7 Classifier: Environment :: Web
+Environment Classifier: Intended Audience :: Developers Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic
-Content Requires-Dist: pyyaml (>=5.1) Requires-Dist: slack-sdk (>=3.0.0)
-Project-URL: Repository, https://github.com/TurnrDev/better-slack-logger
-Description-Content-Type: text/markdown # Better Slack Logger This is a fork is
-[`python-slack-logger`](https://github.com/chinnichaitanya/python-slack-logger)
-package by [Chaitanya Chinni](https://github.com/chinnichaitanya/). If using
-this, please remove that from your environment. A custom message logger to
-Slack for Python 3. This project was built using [`slackclient`](https://
-github.com/slackapi/python-slackclient) and the latest [Block Kit UI](https://
-api.slack.com/block-kit). [PyPI_-_Python_Version] [![PyPI version](https://
-badge.fury.io/py/better-slack-logger.svg)](https://badge.fury.io/py/better-
-slack-logger) [Downloads] [PyPI_-_Wheel] [![License: MIT](https://
+Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/
+HTTP :: Dynamic Content Requires-Dist: pyyaml (>=5.1) Requires-Dist: slack-sdk
+(>=3.0.0) Project-URL: Repository, https://github.com/Kayenta/better-slack-
+logger Description-Content-Type: text/markdown # Better Slack Logger This is a
+fork is [`python-slack-logger`](https://github.com/chinnichaitanya/python-
+slack-logger) package by [Chaitanya Chinni](https://github.com/chinnichaitanya/
+). If using this, please remove that from your environment. A custom message
+logger to Slack for Python 3. This project was built using [`slackclient`]
+(https://github.com/slackapi/python-slackclient) and the latest [Block Kit UI]
+(https://api.slack.com/block-kit). [PyPI_-_Python_Version] [![PyPI version]
+(https://badge.fury.io/py/better-slack-logger.svg)](https://badge.fury.io/py/
+better-slack-logger) [Downloads] [PyPI_-_Wheel] [![License: MIT](https://
 img.shields.io/pypi/l/better-slack-logger)](https://github.com/TurnrDev/better-
 slack-logger/blob/master/LICENSE) [![Code style: black](https://img.shields.io/
 badge/code%20style-black-000000.svg)](https://github.com/python/black) ##
 Install Uninstall [`python-slack-logger`](https://github.com/chinnichaitanya/
 python-slack-logger) package by [Chaitanya Chinni](https://github.com/
 chinnichaitanya/) first: `pip uninstall python-slack-logger` Install via pip:
 `pip install better-slack-logger` ## Basic Usage ```python from slack_logger
```

