# Comparing `tmp/uh_custom_logger-0.0.2.tar.gz` & `tmp/uh_custom_logger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uh_custom_logger-0.0.2.tar", last modified: Tue May 30 19:17:15 2023, max compression
+gzip compressed data, was "uh_custom_logger-0.0.3.tar", last modified: Tue May 30 19:42:53 2023, max compression
```

## Comparing `uh_custom_logger-0.0.2.tar` & `uh_custom_logger-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 astosi    (1000) astosi    (1000)        0 2023-05-30 19:17:15.878455 uh_custom_logger-0.0.2/
--rw-rw-r--   0 astosi    (1000) astosi    (1000)      170 2023-05-30 19:17:15.878455 uh_custom_logger-0.0.2/PKG-INFO
--rw-rw-r--   0 astosi    (1000) astosi    (1000)       38 2023-05-30 19:17:15.878455 uh_custom_logger-0.0.2/setup.cfg
--rw-rw-r--   0 astosi    (1000) astosi    (1000)      272 2023-05-30 19:17:14.000000 uh_custom_logger-0.0.2/setup.py
-drwxrwxr-x   0 astosi    (1000) astosi    (1000)        0 2023-05-30 19:17:15.878455 uh_custom_logger-0.0.2/uh_custom_logger/
--rw-rw-r--   0 astosi    (1000) astosi    (1000)     1195 2023-05-15 09:46:07.000000 uh_custom_logger-0.0.2/uh_custom_logger/CustomFormatter.py
--rw-rw-r--   0 astosi    (1000) astosi    (1000)     2598 2023-05-30 19:12:08.000000 uh_custom_logger-0.0.2/uh_custom_logger/Logger.py
--rw-rw-r--   0 astosi    (1000) astosi    (1000)        0 2023-05-30 18:54:43.000000 uh_custom_logger-0.0.2/uh_custom_logger/__init__.py
--rw-rw-r--   0 astosi    (1000) astosi    (1000)      687 2023-02-21 15:43:53.000000 uh_custom_logger-0.0.2/uh_custom_logger/str_tool.py
-drwxrwxr-x   0 astosi    (1000) astosi    (1000)        0 2023-05-30 19:17:15.878455 uh_custom_logger-0.0.2/uh_custom_logger.egg-info/
--rw-rw-r--   0 astosi    (1000) astosi    (1000)      170 2023-05-30 19:17:15.000000 uh_custom_logger-0.0.2/uh_custom_logger.egg-info/PKG-INFO
--rw-rw-r--   0 astosi    (1000) astosi    (1000)      289 2023-05-30 19:17:15.000000 uh_custom_logger-0.0.2/uh_custom_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 astosi    (1000) astosi    (1000)        1 2023-05-30 19:17:15.000000 uh_custom_logger-0.0.2/uh_custom_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 astosi    (1000) astosi    (1000)       17 2023-05-30 19:17:15.000000 uh_custom_logger-0.0.2/uh_custom_logger.egg-info/top_level.txt
+drwxrwxr-x   0 astosi    (1000) astosi    (1000)        0 2023-05-30 19:42:53.098887 uh_custom_logger-0.0.3/
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)      170 2023-05-30 19:42:53.098887 uh_custom_logger-0.0.3/PKG-INFO
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)       38 2023-05-30 19:42:53.098887 uh_custom_logger-0.0.3/setup.cfg
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)      349 2023-05-30 19:41:37.000000 uh_custom_logger-0.0.3/setup.py
+drwxrwxr-x   0 astosi    (1000) astosi    (1000)        0 2023-05-30 19:42:53.098887 uh_custom_logger-0.0.3/uh_custom_logger/
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)     1195 2023-05-15 09:46:07.000000 uh_custom_logger-0.0.3/uh_custom_logger/CustomFormatter.py
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)     2761 2023-05-30 19:42:50.000000 uh_custom_logger-0.0.3/uh_custom_logger/Logger.py
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)        0 2023-05-30 18:54:43.000000 uh_custom_logger-0.0.3/uh_custom_logger/__init__.py
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)      687 2023-02-21 15:43:53.000000 uh_custom_logger-0.0.3/uh_custom_logger/str_tool.py
+drwxrwxr-x   0 astosi    (1000) astosi    (1000)        0 2023-05-30 19:42:53.098887 uh_custom_logger-0.0.3/uh_custom_logger.egg-info/
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)      170 2023-05-30 19:42:53.000000 uh_custom_logger-0.0.3/uh_custom_logger.egg-info/PKG-INFO
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)      328 2023-05-30 19:42:53.000000 uh_custom_logger-0.0.3/uh_custom_logger.egg-info/SOURCES.txt
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)        1 2023-05-30 19:42:53.000000 uh_custom_logger-0.0.3/uh_custom_logger.egg-info/dependency_links.txt
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)       14 2023-05-30 19:42:53.000000 uh_custom_logger-0.0.3/uh_custom_logger.egg-info/requires.txt
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)       17 2023-05-30 19:42:53.000000 uh_custom_logger-0.0.3/uh_custom_logger.egg-info/top_level.txt
```

### Comparing `uh_custom_logger-0.0.2/uh_custom_logger/CustomFormatter.py` & `uh_custom_logger-0.0.3/uh_custom_logger/CustomFormatter.py`

 * *Files identical despite different names*

### Comparing `uh_custom_logger-0.0.2/uh_custom_logger/Logger.py` & `uh_custom_logger-0.0.3/uh_custom_logger/Logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import logging
 import os
 import sys
 from logging.handlers import TimedRotatingFileHandler
 from typing import Any, Union
 
+from dotenv import load_dotenv
+
 from .CustomFormatter import CoolFormatter
 
 # Define the default logging level
 DEFAULT_LOGGING_LEVEL = logging.INFO
+load_dotenv()
 
-# Define the default log directory
-DEFAULT_LOG_DIR = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'logs')
+ROOT_DIR = os.getenv('ROOT_DIR')
 
+# Check if ROOT_DIR is set
+if ROOT_DIR is None:
+    raise Exception("The ROOT_DIR environment variable must be set.")
+
+# Define the default log directory
+DEFAULT_LOG_DIR = os.path.join(ROOT_DIR, 'logs')
 
 class LoggerSingleton:
     __instance: 'LoggerSingleton' = None
     __log_level: int = DEFAULT_LOGGING_LEVEL
     __log_dir: str = DEFAULT_LOG_DIR
 
     @classmethod
```

### Comparing `uh_custom_logger-0.0.2/uh_custom_logger/str_tool.py` & `uh_custom_logger-0.0.3/uh_custom_logger/str_tool.py`

 * *Files identical despite different names*

