# Comparing `tmp/logrich-0.7.2.tar.gz` & `tmp/logrich-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logrich-0.7.2.tar", max compression
+gzip compressed data, was "logrich-0.7.3.tar", max compression
```

## Comparing `logrich-0.7.2.tar` & `logrich-0.7.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1184 2023-03-25 11:37:39.185788 logrich-0.7.2/README.md
--rw-r--r--   0        0        0       64 2023-05-26 12:26:29.779505 logrich-0.7.2/logrich/__init__.py
--rw-r--r--   0        0        0     2924 2023-03-25 11:37:39.181788 logrich-0.7.2/logrich/app.py
--rw-r--r--   0        0        0     1192 2023-05-26 11:10:29.839735 logrich-0.7.2/logrich/config.py
--rw-r--r--   0        0        0     4819 2023-05-26 11:25:52.964148 logrich-0.7.2/logrich/logger_assets.py
--rw-r--r--   0        0        0      904 2023-05-26 12:27:48.529242 logrich-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 logrich-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1184 2023-03-25 11:37:39.185788 logrich-0.7.3/README.md
+-rw-r--r--   0        0        0       64 2023-05-26 12:26:29.779505 logrich-0.7.3/logrich/__init__.py
+-rw-r--r--   0        0        0     2924 2023-03-25 11:37:39.181788 logrich-0.7.3/logrich/app.py
+-rw-r--r--   0        0        0     1222 2023-05-30 09:32:35.174252 logrich-0.7.3/logrich/config.py
+-rw-r--r--   0        0        0     4819 2023-05-26 11:25:52.964148 logrich-0.7.3/logrich/logger_assets.py
+-rw-r--r--   0        0        0      904 2023-05-30 09:35:12.566071 logrich-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 logrich-0.7.3/PKG-INFO
```

### Comparing `logrich-0.7.2/README.md` & `logrich-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `logrich-0.7.2/logrich/app.py` & `logrich-0.7.3/logrich/app.py`

 * *Files identical despite different names*

### Comparing `logrich-0.7.2/logrich/config.py` & `logrich-0.7.3/logrich/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
+from typing import Union
 
 from pydantic import BaseSettings
 
 
 class Settings(BaseSettings):
     """
     Server config settings
     """
 
-    LOG_LEVEL: int | str = 5
+    LOG_LEVEL: Union[int,str] = 5
     # макисмальная длина текста чтобы разместить его на одной линии с уровнем лога
     MAX_WITH_LOG_OF_OBJ: int = 120
     # https://loguru.readthedocs.io/en/stable/resources/recipes.html#adapting-colors-and-format-of-logged-messages-dynamically
     # https://docs-python.ru/standart-library/modul-string-python/klass-template-modulja-string/
     # https://loguru.readthedocs.io/en/stable/api/logger.html#color
     # https://rich.readthedocs.io/en/stable/style.html
```

### Comparing `logrich-0.7.2/logrich/logger_assets.py` & `logrich-0.7.3/logrich/logger_assets.py`

 * *Files identical despite different names*

### Comparing `logrich-0.7.2/pyproject.toml` & `logrich-0.7.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "logrich"
-version = "0.7.2"
+version = "0.7.3"
 description = "loguru + rich = logrich"
 authors = ["Dmitry Mavlin <mavlind@list.ru>"]
 license = "GPL"
 readme = "README.md"
 keywords = ["logger", "loguru", "rich"]
 
 [project.urls]
```

### Comparing `logrich-0.7.2/PKG-INFO` & `logrich-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logrich
-Version: 0.7.2
+Version: 0.7.3
 Summary: loguru + rich = logrich
 License: GPL
 Keywords: logger,loguru,rich
 Author: Dmitry Mavlin
 Author-email: mavlind@list.ru
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

