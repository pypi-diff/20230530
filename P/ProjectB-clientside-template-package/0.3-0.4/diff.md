# Comparing `tmp/ProjectB_clientside_template_package-0.3.tar.gz` & `tmp/ProjectB_clientside_template_package-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjectB_clientside_template_package-0.3.tar", last modified: Mon May 29 07:37:21 2023, max compression
+gzip compressed data, was "ProjectB_clientside_template_package-0.4.tar", last modified: Tue May 30 02:32:43 2023, max compression
```

## Comparing `ProjectB_clientside_template_package-0.3.tar` & `ProjectB_clientside_template_package-0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 07:37:21.016081 ProjectB_clientside_template_package-0.3/
--rw-rw-rw-   0        0        0      489 2023-05-29 07:37:21.014654 ProjectB_clientside_template_package-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-29 07:37:20.971028 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/
-drwxrwxrwx   0        0        0        0 2023-05-29 07:37:20.996388 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/ClientSocketControl/
--rw-rw-rw-   0        0        0      840 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py
--rw-rw-rw-   0        0        0     3670 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py
--rw-rw-rw-   0        0        0     3981 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/MainController.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:37:21.001897 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/TradeControl/
--rw-rw-rw-   0        0        0     2292 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/TradeControl/Order.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:37:21.013204 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/
--rw-rw-rw-   0        0        0      162 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Action.py
--rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Direction.py
--rw-rw-rw-   0        0        0      161 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/ExpiryDate.py
--rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/StrikePrice.py
--rw-rw-rw-   0        0        0      365 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/TradeControl/Profile.py
--rw-rw-rw-   0        0        0     1889 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/TradeControl/TradeController.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:37:20.993037 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package.egg-info/
--rw-rw-rw-   0        0        0      489 2023-05-29 07:37:20.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      981 2023-05-29 07:37:20.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 07:37:20.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-29 07:37:20.000000 ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      526 2023-05-29 07:36:33.000000 ProjectB_clientside_template_package-0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 07:37:21.016081 ProjectB_clientside_template_package-0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 02:32:43.155577 ProjectB_clientside_template_package-0.4/
+-rw-rw-rw-   0        0        0      489 2023-05-30 02:32:43.153047 ProjectB_clientside_template_package-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 02:32:43.051525 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/
+drwxrwxrwx   0        0        0        0 2023-05-30 02:32:43.129397 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/ClientSocketControl/
+-rw-rw-rw-   0        0        0      840 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py
+-rw-rw-rw-   0        0        0     3670 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py
+-rw-rw-rw-   0        0        0     4129 2023-05-30 02:27:12.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/MainController.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:32:43.136928 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/
+-rw-rw-rw-   0        0        0     2366 2023-05-30 02:27:35.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/Order.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:32:43.150046 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/
+-rw-rw-rw-   0        0        0      162 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Action.py
+-rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Direction.py
+-rw-rw-rw-   0        0        0      161 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/ExpiryDate.py
+-rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/StrikePrice.py
+-rw-rw-rw-   0        0        0      365 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/Profile.py
+-rw-rw-rw-   0        0        0     2000 2023-05-30 02:27:47.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/TradeController.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:32:43.065614 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package.egg-info/
+-rw-rw-rw-   0        0        0      489 2023-05-30 02:32:43.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2023-05-30 02:32:43.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 02:32:43.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-30 02:32:43.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      526 2023-05-30 02:32:13.000000 ProjectB_clientside_template_package-0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 02:32:43.155577 ProjectB_clientside_template_package-0.4/setup.cfg
```

### Comparing `ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py` & `ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py` & `ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/MainController.py` & `ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/MainController.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 import datetime
-from ClientSocketControl.SocketClient import SocketClient
-from ClientSocketControl.DataStructure import DataStructure
-from TradeControl.OrderActionConstants.Action import Action
-from TradeControl.TradeController import TradeController
+from ProjectB_clientside_template_package.ClientSocketControl.SocketClient import SocketClient
+from ProjectB_clientside_template_package.ClientSocketControl.DataStructure import DataStructure
+from ProjectB_clientside_template_package.TradeControl.OrderActionConstants.Action import Action
+from ProjectB_clientside_template_package.TradeControl.TradeController import TradeController
 
 import json
 
 class MainController(ABC):
     
     dataStreaming = None
     dataStreamingRequest = None
```

### Comparing `ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/TradeControl/Order.py` & `ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/Order.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import uuid
 import random
 from datetime import datetime
 from typing import List
-from ClientSocketControl import DataStructure
-from TradeControl.OrderActionConstants import Action, Direction, ExpiryDate, StrikePrice
+from ProjectB_clientside_template_package.ClientSocketControl import DataStructure
+from ProjectB_clientside_template_package.TradeControl.OrderActionConstants import Action, Direction, ExpiryDate, StrikePrice
 from TradeControl.Profile import Profile
 import json
 
 
 class Order:
     def __init__(self, symbol, action, direction, sp, ed, quantity, remained, traded, averageTradePrice, lastUpdateDateTime, historyNodeOrNot):
         self.symbol = symbol
```

### Comparing `ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package/TradeControl/TradeController.py` & `ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/TradeController.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Union
 from ClientSocketControl import DataStructure
-from TradeControl.Order import Order
-from TradeControl.OrderActionConstants import Action, Direction, ExpiryDate, StrikePrice
-from TradeControl.Profile import Profile
+from ProjectB_clientside_template_package.TradeControl.Order import Order
+from ProjectB_clientside_template_package.TradeControl.OrderActionConstants import Action, Direction, ExpiryDate, StrikePrice
+from ProjectB_clientside_template_package.TradeControl.Profile import Profile
 import json
 import random
 
 
 class TradeController:
     def __init__(self):
         self.profile = Profile()
```

### Comparing `ProjectB_clientside_template_package-0.3/ProjectB_clientside_template_package.egg-info/SOURCES.txt` & `ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.3/pyproject.toml` & `ProjectB_clientside_template_package-0.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ProjectB_clientside_template_package"
-version = "0.3"
+version = "0.4"
 authors = [
   { name="ProjectB", email="admin@projectb.click" },
 ]
 description = "This is the pip package of ProjectB_clientside_template_package"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

