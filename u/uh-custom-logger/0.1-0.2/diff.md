# Comparing `tmp/uh_custom_logger-0.1.tar.gz` & `tmp/uh_custom_logger-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uh_custom_logger-0.1.tar", last modified: Tue May 30 18:56:37 2023, max compression
+gzip compressed data, was "uh_custom_logger-0.2.tar", last modified: Tue May 30 19:08:01 2023, max compression
```

## Comparing `uh_custom_logger-0.1.tar` & `uh_custom_logger-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 astosi    (1000) astosi    (1000)        0 2023-05-30 18:56:37.271772 uh_custom_logger-0.1/
--rw-rw-r--   0 astosi    (1000) astosi    (1000)      168 2023-05-30 18:56:37.271772 uh_custom_logger-0.1/PKG-INFO
--rw-rw-r--   0 astosi    (1000) astosi    (1000)       38 2023-05-30 18:56:37.271772 uh_custom_logger-0.1/setup.cfg
--rw-rw-r--   0 astosi    (1000) astosi    (1000)      270 2023-05-30 18:52:15.000000 uh_custom_logger-0.1/setup.py
-drwxrwxr-x   0 astosi    (1000) astosi    (1000)        0 2023-05-30 18:56:37.271772 uh_custom_logger-0.1/uh_custom_logger/
--rw-rw-r--   0 astosi    (1000) astosi    (1000)     1195 2023-05-15 09:46:07.000000 uh_custom_logger-0.1/uh_custom_logger/CustomFormatter.py
--rw-rw-r--   0 astosi    (1000) astosi    (1000)     2610 2023-05-30 18:50:49.000000 uh_custom_logger-0.1/uh_custom_logger/Logger.py
--rw-rw-r--   0 astosi    (1000) astosi    (1000)        0 2023-05-30 18:54:43.000000 uh_custom_logger-0.1/uh_custom_logger/__init__.py
--rw-rw-r--   0 astosi    (1000) astosi    (1000)      687 2023-02-21 15:43:53.000000 uh_custom_logger-0.1/uh_custom_logger/str_tool.py
-drwxrwxr-x   0 astosi    (1000) astosi    (1000)        0 2023-05-30 18:56:37.271772 uh_custom_logger-0.1/uh_custom_logger.egg-info/
--rw-rw-r--   0 astosi    (1000) astosi    (1000)      168 2023-05-30 18:56:37.000000 uh_custom_logger-0.1/uh_custom_logger.egg-info/PKG-INFO
--rw-rw-r--   0 astosi    (1000) astosi    (1000)      289 2023-05-30 18:56:37.000000 uh_custom_logger-0.1/uh_custom_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 astosi    (1000) astosi    (1000)        1 2023-05-30 18:56:37.000000 uh_custom_logger-0.1/uh_custom_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 astosi    (1000) astosi    (1000)       17 2023-05-30 18:56:37.000000 uh_custom_logger-0.1/uh_custom_logger.egg-info/top_level.txt
+drwxrwxr-x   0 astosi    (1000) astosi    (1000)        0 2023-05-30 19:08:01.479020 uh_custom_logger-0.2/
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)      168 2023-05-30 19:08:01.479020 uh_custom_logger-0.2/PKG-INFO
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)       38 2023-05-30 19:08:01.479020 uh_custom_logger-0.2/setup.cfg
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)      270 2023-05-30 19:07:44.000000 uh_custom_logger-0.2/setup.py
+drwxrwxr-x   0 astosi    (1000) astosi    (1000)        0 2023-05-30 19:08:01.479020 uh_custom_logger-0.2/uh_custom_logger/
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)     1195 2023-05-15 09:46:07.000000 uh_custom_logger-0.2/uh_custom_logger/CustomFormatter.py
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)     2599 2023-05-30 19:07:33.000000 uh_custom_logger-0.2/uh_custom_logger/Logger.py
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)        0 2023-05-30 18:54:43.000000 uh_custom_logger-0.2/uh_custom_logger/__init__.py
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)      687 2023-02-21 15:43:53.000000 uh_custom_logger-0.2/uh_custom_logger/str_tool.py
+drwxrwxr-x   0 astosi    (1000) astosi    (1000)        0 2023-05-30 19:08:01.479020 uh_custom_logger-0.2/uh_custom_logger.egg-info/
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)      168 2023-05-30 19:08:01.000000 uh_custom_logger-0.2/uh_custom_logger.egg-info/PKG-INFO
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)      289 2023-05-30 19:08:01.000000 uh_custom_logger-0.2/uh_custom_logger.egg-info/SOURCES.txt
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)        1 2023-05-30 19:08:01.000000 uh_custom_logger-0.2/uh_custom_logger.egg-info/dependency_links.txt
+-rw-rw-r--   0 astosi    (1000) astosi    (1000)       17 2023-05-30 19:08:01.000000 uh_custom_logger-0.2/uh_custom_logger.egg-info/top_level.txt
```

### Comparing `uh_custom_logger-0.1/uh_custom_logger/CustomFormatter.py` & `uh_custom_logger-0.2/uh_custom_logger/CustomFormatter.py`

 * *Files identical despite different names*

### Comparing `uh_custom_logger-0.1/uh_custom_logger/Logger.py` & `uh_custom_logger-0.2/uh_custom_logger/Logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     def get_console_handler(self) -> logging.StreamHandler:
         console_handler = logging.StreamHandler(sys.stdout)
         console_handler.setFormatter(self.get_formatter())
         return console_handler
 
     def get_file_handler(self) -> TimedRotatingFileHandler:
-        file_handler = TimedRotatingFileHandler(os.path.join(self.__log_dir, 'log_history/logs.log'), when='midnight')
+        file_handler = TimedRotatingFileHandler(os.path.join(self.__log_dir, '/logs.log'), when='midnight')
         file_handler.setFormatter(self.get_file_formatter())
         return file_handler
 
     def get_formatter(self) -> CoolFormatter:
         return CoolFormatter()
 
     def get_file_formatter(self) -> logging.Formatter:
```

### Comparing `uh_custom_logger-0.1/uh_custom_logger/str_tool.py` & `uh_custom_logger-0.2/uh_custom_logger/str_tool.py`

 * *Files identical despite different names*

