# Comparing `tmp/python-printr-2.7.tar.gz` & `tmp/python-printr-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-printr-2.7.tar", last modified: Sun Mar 26 18:57:40 2023, max compression
+gzip compressed data, was "python-printr-2.8.tar", last modified: Tue May 30 12:55:46 2023, max compression
```

## Comparing `python-printr-2.7.tar` & `python-printr-2.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 18:57:40.719978 python-printr-2.7/
--rw-rw-rw-   0        0        0       66 2022-04-13 16:11:03.000000 python-printr-2.7/.gitignore
--rw-rw-rw-   0        0        0     3350 2023-03-26 18:57:40.720977 python-printr-2.7/PKG-INFO
--rw-rw-rw-   0        0        0     3092 2023-03-11 18:19:37.000000 python-printr-2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-26 18:57:40.715981 python-printr-2.7/printr/
--rw-rw-rw-   0        0        0     7469 2023-03-26 18:56:06.000000 python-printr-2.7/printr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-26 18:57:40.719978 python-printr-2.7/python_printr.egg-info/
--rw-rw-rw-   0        0        0     3350 2023-03-26 18:57:38.000000 python-printr-2.7/python_printr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-03-26 18:57:39.000000 python-printr-2.7/python_printr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 18:57:38.000000 python-printr-2.7/python_printr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-03-26 18:57:38.000000 python-printr-2.7/python_printr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-26 18:57:38.000000 python-printr-2.7/python_printr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-26 18:57:40.720977 python-printr-2.7/setup.cfg
--rw-rw-rw-   0        0        0      427 2023-03-26 18:57:35.000000 python-printr-2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:55:46.375472 python-printr-2.8/
+-rw-rw-rw-   0        0        0       66 2022-04-13 16:11:03.000000 python-printr-2.8/.gitignore
+-rw-rw-rw-   0        0        0     3350 2023-05-30 12:55:46.375472 python-printr-2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3092 2023-03-11 18:19:37.000000 python-printr-2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 12:55:46.369478 python-printr-2.8/printr/
+-rw-rw-rw-   0        0        0     7818 2023-05-30 12:55:28.000000 python-printr-2.8/printr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:55:46.374473 python-printr-2.8/python_printr.egg-info/
+-rw-rw-rw-   0        0        0     3350 2023-05-30 12:55:45.000000 python-printr-2.8/python_printr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-30 12:55:46.000000 python-printr-2.8/python_printr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 12:55:45.000000 python-printr-2.8/python_printr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-30 12:55:45.000000 python-printr-2.8/python_printr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 12:55:45.000000 python-printr-2.8/python_printr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-30 12:55:46.375472 python-printr-2.8/setup.cfg
+-rw-rw-rw-   0        0        0      427 2023-05-30 12:55:41.000000 python-printr-2.8/setup.py
```

### Comparing `python-printr-2.7/PKG-INFO` & `python-printr-2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-printr
-Version: 2.7
+Version: 2.8
 Summary: printr
 Home-page: https://github.com/xjxckk/python-printr/
 Download-URL: https://github.com/xjxckk/python-printr/archive/refs/tags/v0.1.tar.gz
 Description-Content-Type: text/markdown
 
 ### python-printr
 Python print functions to beautify output
```

### Comparing `python-printr-2.7/README.md` & `python-printr-2.8/README.md`

 * *Files identical despite different names*

### Comparing `python-printr-2.7/printr/__init__.py` & `python-printr-2.8/printr/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import sys, logging, json, os, shutil, coloredlogs
 from pathlib import Path
 from datetime import datetime
 
 class logger:
-    def __init__(self, log_filepath=None, max_lines=100_000, level='info', name=None):
+    def __init__(self, log_filepath=None, max_lines=100_000, level='info', name=None, log_to_file=True):
         filename = Path(sys.argv[0]).stem
         self.filename = filename
         if not log_filepath:
             log_filepath = f'{os.getcwd()}/{filename}.txt'
         self.log_filepath = log_filepath
         self.max_lines = max_lines
+        self.log_to_file = log_to_file
 
         logger = logging.getLogger(__name__)
         logger.setLevel(logging.DEBUG)
 
-        log_file = logging.FileHandler(log_filepath, encoding='utf-8')
-        log_format = logging.Formatter(fmt='%(message)s')
-        log_file.setFormatter(log_format)
-        logger.addHandler(log_file)
-        self.log_file = log_file
-        
-        logger.info('') # add line break in between runs in log file
-        log_format = logging.Formatter(fmt='%(levelname)s - %(asctime)s.%(msecs)03d - Line %(lineno)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
-        log_file.setFormatter(log_format)
+        if log_to_file:
+            log_file = logging.FileHandler(log_filepath, encoding='utf-8')
+            log_format = logging.Formatter(fmt='%(message)s')
+            log_file.setFormatter(log_format)
+            logger.addHandler(log_file)
+            self.log_file = log_file
+            
+            logger.info('') # add line break in between runs in log file
+            log_format = logging.Formatter(fmt='%(levelname)s - %(asctime)s.%(msecs)03d - Line %(lineno)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+            log_file.setFormatter(log_format)
 
         if level == 'info':
             self.level = logging.INFO
         elif level == 'debug':
             self.level = logging.DEBUG
         coloredlogs.install(level=self.level, logger=logger, fmt='%(message)s')
         self.logger = logger
@@ -52,44 +54,47 @@
                     formatted_item += json.dumps(item, indent=4) # Beautify JSON objects
                     item = formatted_item + '\n'
                 except TypeError:
                     pass
             message += str(item)
 
         if not message:
-            log_format = logging.Formatter(fmt=self.indent + '%(message)s')
-            self.log_file.setFormatter(log_format)
+            if self.log_to_file:
+                log_format = logging.Formatter(fmt=self.indent + '%(message)s')
+                self.log_file.setFormatter(log_format)
             coloredlogs.install(level=self.level, logger=self.logger, fmt='%(message)s')
 
         if level == 'info':
             self.logger.info(message)
         elif level == 'error':
             self.logger.error(message)
         elif level == 'debug':
             self.logger.debug(message)
         elif level == 'success':
             self.logger.success(message)
         elif level == 'warning':
             self.logger.warning(message)
 
         if not message:
-            log_format = logging.Formatter(fmt=self.indent + '%(levelname)s - %(asctime)s.%(msecs)03d - Line %(lineno)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S') # Reset to default log format
-            self.log_file.setFormatter(log_format)
+            if self.log_to_file:
+                log_format = logging.Formatter(fmt=self.indent + '%(levelname)s - %(asctime)s.%(msecs)03d - Line %(lineno)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S') # Reset to default log format
+                self.log_file.setFormatter(log_format)
             coloredlogs.install(level=self.level, logger=self.logger, fmt=self.indent + '%(message)s') # Reset to default log format
 
-        log_file = open(self.log_filepath, 'r+', encoding='utf-8', errors='ignore').read()
-        number_of_lines = len(log_file.splitlines())
-        if number_of_lines > self.max_lines:
-            self.logger.info('Resetting log file')
-            self.log_file.close()
-            log_file = logging.FileHandler(self.log_filepath, mode='w', encoding='utf-8')
-            log_format = logging.Formatter(fmt=self.indent + '%(levelname)s - %(asctime)s.%(msecs)03d - Line %(lineno)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
-            log_file.setFormatter(log_format)
-            self.logger.addHandler(log_file)
-            self.log_file = log_file
+        if self.log_to_file:
+            log_file = open(self.log_filepath, 'r+', encoding='utf-8', errors='ignore').read()
+            number_of_lines = len(log_file.splitlines())
+            if number_of_lines > self.max_lines:
+                self.logger.info('Resetting log file')
+                self.log_file.close()
+                log_file = logging.FileHandler(self.log_filepath, mode='w', encoding='utf-8')
+                log_format = logging.Formatter(fmt=self.indent + '%(levelname)s - %(asctime)s.%(msecs)03d - Line %(lineno)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+                log_file.setFormatter(log_format)
+                self.logger.addHandler(log_file)
+                self.log_file = log_file
     
     def error(self, *items):
         self.log(*items, level='error')
     
     def debug(self, *items):
         self.log(*items, level='debug')
     
@@ -101,22 +106,24 @@
     
     def current_time(self, *items, level='info'):
         current_time = datetime.now()
         current_time = current_time.strftime('%H:%M:%S:%f') + ':'
         self.log(current_time, *items, level=level)
     
     def set_indent(self, indent=' - '):
-        log_format = logging.Formatter(fmt=indent + '%(levelname)s - %(asctime)s.%(msecs)03d - Line %(lineno)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
-        self.log_file.setFormatter(log_format)
+        if self.log_to_file:
+            log_format = logging.Formatter(fmt=indent + '%(levelname)s - %(asctime)s.%(msecs)03d - Line %(lineno)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+            self.log_file.setFormatter(log_format)
         coloredlogs.install(level=self.level, logger=self.logger, fmt=indent + '%(message)s')
         self.indent = indent
     
     def remove_indent(self):
-        log_format = logging.Formatter(fmt='%(levelname)s - %(asctime)s.%(msecs)03d - Line %(lineno)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
-        self.log_file.setFormatter(log_format)
+        if self.log_to_file:
+            log_format = logging.Formatter(fmt='%(levelname)s - %(asctime)s.%(msecs)03d - Line %(lineno)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+            self.log_file.setFormatter(log_format)
         coloredlogs.install(level=self.level, logger=self.logger, fmt='%(message)s') # Reset to default log format
         self.indent = ''
 
 class printr:
     '''printr'''
     def __init__(self, *items, same_line=False, current_time=False, check_for_log=True, level='info'):
         if len(items) == 1:
```

### Comparing `python-printr-2.7/python_printr.egg-info/PKG-INFO` & `python-printr-2.8/python_printr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-printr
-Version: 2.7
+Version: 2.8
 Summary: printr
 Home-page: https://github.com/xjxckk/python-printr/
 Download-URL: https://github.com/xjxckk/python-printr/archive/refs/tags/v0.1.tar.gz
 Description-Content-Type: text/markdown
 
 ### python-printr
 Python print functions to beautify output
```

