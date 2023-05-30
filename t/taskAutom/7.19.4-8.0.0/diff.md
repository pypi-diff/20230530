# Comparing `tmp/taskAutom-7.19.4.tar.gz` & `tmp/taskAutom-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskAutom-7.19.4.tar", last modified: Sat May  6 14:32:46 2023, max compression
+gzip compressed data, was "taskAutom-8.0.0.tar", last modified: Tue May 30 13:50:30 2023, max compression
```

## Comparing `taskAutom-7.19.4.tar` & `taskAutom-8.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-06 14:32:46.802196 taskAutom-7.19.4/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-7.19.4/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-05-06 14:32:46.802196 taskAutom-7.19.4/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-7.19.4/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-06 14:32:46.802196 taskAutom-7.19.4/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1000 2023-05-06 14:32:36.000000 taskAutom-7.19.4/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-06 14:32:46.802196 taskAutom-7.19.4/src/
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-06 14:32:46.802196 taskAutom-7.19.4/src/taskAutom/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       53 2023-05-06 14:32:25.000000 taskAutom-7.19.4/src/taskAutom/__init__.py
--rwxrwxr-x   0 lucas     (1000) lucas     (1000)    65695 2023-05-06 14:32:16.000000 taskAutom-7.19.4/src/taskAutom/taskAutom.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-06 14:32:46.802196 taskAutom-7.19.4/taskAutom.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-05-06 14:32:46.000000 taskAutom-7.19.4/taskAutom.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-05-06 14:32:46.000000 taskAutom-7.19.4/taskAutom.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-06 14:32:46.000000 taskAutom-7.19.4/taskAutom.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-05-06 14:32:46.000000 taskAutom-7.19.4/taskAutom.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-05-06 14:32:46.000000 taskAutom-7.19.4/taskAutom.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-05-06 14:32:46.000000 taskAutom-7.19.4/taskAutom.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 13:50:30.176309 taskAutom-8.0.0/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-8.0.0/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-05-30 13:50:30.176309 taskAutom-8.0.0/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-8.0.0/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-30 13:50:30.176309 taskAutom-8.0.0/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      999 2023-05-30 13:49:30.000000 taskAutom-8.0.0/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 13:50:30.176309 taskAutom-8.0.0/src/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 13:50:30.176309 taskAutom-8.0.0/src/taskAutom/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-05-30 13:49:14.000000 taskAutom-8.0.0/src/taskAutom/__init__.py
+-rwxrwxr-x   0 lucas     (1000) lucas     (1000)    66632 2023-05-30 13:18:23.000000 taskAutom-8.0.0/src/taskAutom/taskAutom.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 13:50:30.176309 taskAutom-8.0.0/taskAutom.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-05-30 13:50:30.000000 taskAutom-8.0.0/taskAutom.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-05-30 13:50:30.000000 taskAutom-8.0.0/taskAutom.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-30 13:50:30.000000 taskAutom-8.0.0/taskAutom.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-05-30 13:50:30.000000 taskAutom-8.0.0/taskAutom.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-05-30 13:50:30.000000 taskAutom-8.0.0/taskAutom.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-05-30 13:50:30.000000 taskAutom-8.0.0/taskAutom.egg-info/top_level.txt
```

### Comparing `taskAutom-7.19.4/LICENSE` & `taskAutom-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskAutom-7.19.4/PKG-INFO` & `taskAutom-8.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 7.19.4
+Version: 8.0.0
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `taskAutom-7.19.4/README.md` & `taskAutom-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `taskAutom-7.19.4/setup.py` & `taskAutom-8.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from importlib.metadata import entry_points
 from setuptools import setup
 
 setup(
     name='taskAutom',
-    version='7.19.4',
+    version='8.0.0',
     description='A simple task automation tool',
     long_description='A simple task automation tool for NOKIA SROS based routers',
     long_description_content_type='text/x-rst',
     url='https://github.com/laimaretto/taskAutom',
     author='Lucas Aimaretto',
     author_email='laimaretto@gmail.com',
     license='BSD 3-clause',
     packages=['src/taskAutom'],
     install_requires=['sshtunnel==0.4.0',
-                      'netmiko==4.1.0',
+                      'netmiko==4.2.0',
                       'pandas==1.5.2',
                       'pyyaml==5.3.1',
                       'python-docx==0.8.11',
                       ],
     python_requires='>=3.8',
     classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `taskAutom-7.19.4/src/taskAutom/taskAutom.py` & `taskAutom-8.0.0/src/taskAutom/taskAutom.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,26 +24,25 @@
 import calendar
 import sys
 
 # installed
 import sshtunnel
 import paramiko
 from netmiko import ConnectHandler
+from netmiko import ConnLogOnly
 from scp import SCPClient
 import pandas as pd
 import yaml
 import docx
 from docx.enum.style import WD_STYLE_TYPE 
 from docx.enum.text import WD_LINE_SPACING
 from docx.shared import Pt
 
 
-#logging.basicConfig(level=logging.DEBUG,format='[%(levelname)s] (%(threadName)-10s) %(message)s')
-
-LATEST_VERSION = '7.19.4'
+LATEST_VERSION = '8.0.0'
 
 # Constants
 IP_LOCALHOST  = "127.0.0.1"
 LOG_GLOBAL    = []
 LOG_CONSOLE   = []
 DICT_PARAM    = dict(
 	outputJob        = 0,
@@ -288,15 +287,15 @@
 		return str( timeFloat ) + unit
 
 	else:
 
 		return float(int(timeFloat*move))/move
 
 def fncPrintConsole(inText, show=1):
-	#logging.debug(inText)
+
 	localtime   = time.localtime()
 	if show:
 		output = str(time.strftime("%H:%M:%S", localtime)) + "| " + inText
 		print(output)
 		LOG_CONSOLE.append(output)
 
 def getListOfRouters(dictParam):
@@ -926,14 +925,15 @@
 			'runStatus':-1, # revisar, solo una vez
 			'strConn': "Con-" + str(thrdNum) + "| ",
 			'num':thrdNum,
 			'outRx':'',
 			'outRxJson':{},
 			'cronScript':None,
 			'auxRetry':dictParam['auxRetry'],
+			'sshDebug':dictParam['sshDebug']
 		}
 
 		self.connInfo.update(routerInfo)
 
 		# We update the outputjob relevant information...
 		if self.outputJob == 2:
 			self.connInfo['pluginScript'] = DICT_VENDOR[self.connInfo['deviceType']]['START_SCRIPT'] + \
@@ -1362,29 +1362,37 @@
 		systemIP   = connInfo['systemIP']
 		deviceType = connInfo['deviceType']
 
 		# if we have a MD-CLI device, let's make sure netmiko
 		# does support it.
 		deviceType = re.sub('^md_','',deviceType)
 
+		# We check if debug is enabled
+		if self.connInfo['sshDebug'] is True:
+			debug = self.logsDirectory + "debug.debug"
+		else:
+			debug = None
+
+
 		if connInfo['useSSHTunnel'] is True:
 			ip   = IP_LOCALHOST
 			port = connInfo['localPort']
 		else:
 			ip   = connInfo['systemIP']
 			port = connInfo['remotePort']
 
 		while aluLogged == False and index < len(self.ROUTER_USER):
 
 			tempUser = self.ROUTER_USER[index][0]
 			tempPass = self.ROUTER_USER[index][1]
 			index 	 = index + 1
 
 			try:
-				conn2rtr = ConnectHandler(device_type=deviceType, host=ip, port=port, username=tempUser, password=tempPass, fast_cli=False)
+				#conn2rtr = ConnectHandler(device_type=deviceType, host=ip, port=port, username=tempUser, password=tempPass, fast_cli=False, session_log=debug) #, log_level="DEBUG")
+				conn2rtr = ConnLogOnly(device_type=deviceType, host=ip, port=port, username=tempUser, password=tempPass, fast_cli=False, log_file=debug, log_level="DEBUG",log_format='[%(levelname)s] %(name)s: [%(threadName)s] %(message)s')
 				aluLogged    = True
 				aluLogReason = "LoggedOk"
 				aluLogUser   = tempUser
 				aluPass      = tempPass
 			except Exception as e:
 				conn2rtr     = None
 				aluLogged 	 = False
@@ -1931,14 +1939,36 @@
 	else:
 
 		print("Not enough paramteres.\nAt least define --username, --logInfo, depending on the jobType.\nRun: taskAutom -h for help.\nQuitting...")
 		quit()
 
 	return dictParam
 
+def enableLogging(dictParam):
+
+	## Netmiko Debug
+	if dictParam['sshDebug'] is True:
+		
+		debugFileName = dictParam['logsDirectory'] + 'debug.log'
+
+		logger        = logging.getLogger("netmiko")
+		logger.setLevel('DEBUG')
+		
+		handler = logging.FileHandler(debugFileName)
+		handler.setLevel(logging.DEBUG)
+		handler.setFormatter(logging.Formatter('[%(levelname)s] %(name)s: [%(threadName)s] %(message)s'))
+
+		logger.addHandler(handler)
+
+		#log_formatter = logging.Formatter("%(asctime)s [%(levelname)s] %(name)s: %(message)s [%(threadName)s] ") # I am printing thread id here
+		#logging.basicConfig(filename=debugFileName, level=logging.DEBUG)
+		
+
+	return None
+
 def fncRun(dictParam):
 	"""[summary]
 
 	Args:
 		dictParam ([dict]): [Dictionary with parameters for the connections]
 	Returns:
 		[int]: 0
@@ -1948,26 +1978,24 @@
 
 	# We take initial time 
 	timeTotalStart 	= time.time()
 
 	# Generar threads
 	threads_list = ThreadPool(dictParam['progNumThreads'])
 
-	## Netmiko Debug
-	if dictParam['sshDebug'] is True:
-		logging.basicConfig(filename='debug.log', level=logging.DEBUG)
-		logger = logging.getLogger("netmiko")
-
 	################
 	# Running...
 	if dictParam['outputJob'] == 2:
 
 		# logInfo
 		dictParam = createLogFolder(dictParam)
 
+		# debug
+		enableLogging(dictParam)
+
 		for i, IPconnect in enumerate(listOfRouters):
 
 			routerInfo = dictParam['inventory'][IPconnect]
 			routerInfo['pluginScript'].append(renderCliLine(IPconnect, dictParam, i))
 
 			# Wait before sending scripts to the routers ...
 			waitBetweenRouters(dictParam)
@@ -1992,14 +2020,17 @@
 
 	elif dictParam['outputJob'] == 3:
 
 		# logInfo
 		dictParam     = createLogFolder(dictParam)
 		listOfRouters = list(dictParam['inventory'].keys())
 
+		# debug
+		enableLogging(dictParam)
+
 		for i, IPconnect in enumerate(listOfRouters):
 
 			routerInfo = dictParam['inventory'][IPconnect]		
 
 			# Wait before sending scripts to the routers ...
 			waitBetweenRouters(dictParam)
```

### Comparing `taskAutom-7.19.4/taskAutom.egg-info/PKG-INFO` & `taskAutom-8.0.0/taskAutom.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 7.19.4
+Version: 8.0.0
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

