# Comparing `tmp/taskAutom-8.0.0.tar.gz` & `tmp/taskAutom-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskAutom-8.0.0.tar", last modified: Tue May 30 13:50:30 2023, max compression
+gzip compressed data, was "taskAutom-8.0.1.tar", last modified: Tue May 30 14:00:23 2023, max compression
```

## Comparing `taskAutom-8.0.0.tar` & `taskAutom-8.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 13:50:30.176309 taskAutom-8.0.0/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-8.0.0/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-05-30 13:50:30.176309 taskAutom-8.0.0/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-8.0.0/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-30 13:50:30.176309 taskAutom-8.0.0/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      999 2023-05-30 13:49:30.000000 taskAutom-8.0.0/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 13:50:30.176309 taskAutom-8.0.0/src/
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 13:50:30.176309 taskAutom-8.0.0/src/taskAutom/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-05-30 13:49:14.000000 taskAutom-8.0.0/src/taskAutom/__init__.py
--rwxrwxr-x   0 lucas     (1000) lucas     (1000)    66632 2023-05-30 13:18:23.000000 taskAutom-8.0.0/src/taskAutom/taskAutom.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 13:50:30.176309 taskAutom-8.0.0/taskAutom.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-05-30 13:50:30.000000 taskAutom-8.0.0/taskAutom.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-05-30 13:50:30.000000 taskAutom-8.0.0/taskAutom.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-30 13:50:30.000000 taskAutom-8.0.0/taskAutom.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-05-30 13:50:30.000000 taskAutom-8.0.0/taskAutom.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-05-30 13:50:30.000000 taskAutom-8.0.0/taskAutom.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-05-30 13:50:30.000000 taskAutom-8.0.0/taskAutom.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 14:00:23.798750 taskAutom-8.0.1/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-8.0.1/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-05-30 14:00:23.798750 taskAutom-8.0.1/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-8.0.1/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-30 14:00:23.798750 taskAutom-8.0.1/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      999 2023-05-30 14:00:13.000000 taskAutom-8.0.1/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 14:00:23.794750 taskAutom-8.0.1/src/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 14:00:23.794750 taskAutom-8.0.1/src/taskAutom/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-05-30 14:00:09.000000 taskAutom-8.0.1/src/taskAutom/__init__.py
+-rwxrwxr-x   0 lucas     (1000) lucas     (1000)    66714 2023-05-30 13:59:08.000000 taskAutom-8.0.1/src/taskAutom/taskAutom.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 14:00:23.798750 taskAutom-8.0.1/taskAutom.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-05-30 14:00:23.000000 taskAutom-8.0.1/taskAutom.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-05-30 14:00:23.000000 taskAutom-8.0.1/taskAutom.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-30 14:00:23.000000 taskAutom-8.0.1/taskAutom.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-05-30 14:00:23.000000 taskAutom-8.0.1/taskAutom.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-05-30 14:00:23.000000 taskAutom-8.0.1/taskAutom.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-05-30 14:00:23.000000 taskAutom-8.0.1/taskAutom.egg-info/top_level.txt
```

### Comparing `taskAutom-8.0.0/LICENSE` & `taskAutom-8.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskAutom-8.0.0/PKG-INFO` & `taskAutom-8.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 8.0.0
+Version: 8.0.1
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `taskAutom-8.0.0/README.md` & `taskAutom-8.0.1/README.md`

 * *Files identical despite different names*

### Comparing `taskAutom-8.0.0/setup.py` & `taskAutom-8.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from importlib.metadata import entry_points
 from setuptools import setup
 
 setup(
     name='taskAutom',
-    version='8.0.0',
+    version='8.0.1',
     description='A simple task automation tool',
     long_description='A simple task automation tool for NOKIA SROS based routers',
     long_description_content_type='text/x-rst',
     url='https://github.com/laimaretto/taskAutom',
     author='Lucas Aimaretto',
     author_email='laimaretto@gmail.com',
     license='BSD 3-clause',
```

### Comparing `taskAutom-8.0.0/src/taskAutom/taskAutom.py` & `taskAutom-8.0.1/src/taskAutom/taskAutom.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import yaml
 import docx
 from docx.enum.style import WD_STYLE_TYPE 
 from docx.enum.text import WD_LINE_SPACING
 from docx.shared import Pt
 
 
-LATEST_VERSION = '8.0.0'
+LATEST_VERSION = '8.0.1'
 
 # Constants
 IP_LOCALHOST  = "127.0.0.1"
 LOG_GLOBAL    = []
 LOG_CONSOLE   = []
 DICT_PARAM    = dict(
 	outputJob        = 0,
@@ -1362,21 +1362,14 @@
 		systemIP   = connInfo['systemIP']
 		deviceType = connInfo['deviceType']
 
 		# if we have a MD-CLI device, let's make sure netmiko
 		# does support it.
 		deviceType = re.sub('^md_','',deviceType)
 
-		# We check if debug is enabled
-		if self.connInfo['sshDebug'] is True:
-			debug = self.logsDirectory + "debug.debug"
-		else:
-			debug = None
-
-
 		if connInfo['useSSHTunnel'] is True:
 			ip   = IP_LOCALHOST
 			port = connInfo['localPort']
 		else:
 			ip   = connInfo['systemIP']
 			port = connInfo['remotePort']
 
@@ -1384,15 +1377,19 @@
 
 			tempUser = self.ROUTER_USER[index][0]
 			tempPass = self.ROUTER_USER[index][1]
 			index 	 = index + 1
 
 			try:
 				#conn2rtr = ConnectHandler(device_type=deviceType, host=ip, port=port, username=tempUser, password=tempPass, fast_cli=False, session_log=debug) #, log_level="DEBUG")
-				conn2rtr = ConnLogOnly(device_type=deviceType, host=ip, port=port, username=tempUser, password=tempPass, fast_cli=False, log_file=debug, log_level="DEBUG",log_format='[%(levelname)s] %(name)s: [%(threadName)s] %(message)s')
+				if self.connInfo['sshDebug'] is True:
+					debug = self.logsDirectory + "debug.debug"
+					conn2rtr = ConnLogOnly(device_type=deviceType, host=ip, port=port, username=tempUser, password=tempPass, fast_cli=False, log_file=debug, log_level="DEBUG",log_format='[%(levelname)s] %(name)s: [%(threadName)s] %(message)s')
+				else:
+					conn2rtr = ConnLogOnly(device_type=deviceType, host=ip, port=port, username=tempUser, password=tempPass, fast_cli=False)
 				aluLogged    = True
 				aluLogReason = "LoggedOk"
 				aluLogUser   = tempUser
 				aluPass      = tempPass
 			except Exception as e:
 				conn2rtr     = None
 				aluLogged 	 = False
```

### Comparing `taskAutom-8.0.0/taskAutom.egg-info/PKG-INFO` & `taskAutom-8.0.1/taskAutom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 8.0.0
+Version: 8.0.1
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

