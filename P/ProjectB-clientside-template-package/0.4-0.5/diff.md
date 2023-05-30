# Comparing `tmp/ProjectB_clientside_template_package-0.4.tar.gz` & `tmp/ProjectB_clientside_template_package-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjectB_clientside_template_package-0.4.tar", last modified: Tue May 30 02:32:43 2023, max compression
+gzip compressed data, was "ProjectB_clientside_template_package-0.5.tar", last modified: Tue May 30 02:38:14 2023, max compression
```

## Comparing `ProjectB_clientside_template_package-0.4.tar` & `ProjectB_clientside_template_package-0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 02:32:43.155577 ProjectB_clientside_template_package-0.4/
--rw-rw-rw-   0        0        0      489 2023-05-30 02:32:43.153047 ProjectB_clientside_template_package-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 02:32:43.051525 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/
-drwxrwxrwx   0        0        0        0 2023-05-30 02:32:43.129397 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/ClientSocketControl/
--rw-rw-rw-   0        0        0      840 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py
--rw-rw-rw-   0        0        0     3670 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py
--rw-rw-rw-   0        0        0     4129 2023-05-30 02:27:12.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/MainController.py
-drwxrwxrwx   0        0        0        0 2023-05-30 02:32:43.136928 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/
--rw-rw-rw-   0        0        0     2366 2023-05-30 02:27:35.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/Order.py
-drwxrwxrwx   0        0        0        0 2023-05-30 02:32:43.150046 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/
--rw-rw-rw-   0        0        0      162 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Action.py
--rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Direction.py
--rw-rw-rw-   0        0        0      161 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/ExpiryDate.py
--rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/StrikePrice.py
--rw-rw-rw-   0        0        0      365 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/Profile.py
--rw-rw-rw-   0        0        0     2000 2023-05-30 02:27:47.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/TradeController.py
-drwxrwxrwx   0        0        0        0 2023-05-30 02:32:43.065614 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package.egg-info/
--rw-rw-rw-   0        0        0      489 2023-05-30 02:32:43.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      981 2023-05-30 02:32:43.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 02:32:43.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-30 02:32:43.000000 ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      526 2023-05-30 02:32:13.000000 ProjectB_clientside_template_package-0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 02:32:43.155577 ProjectB_clientside_template_package-0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 02:38:14.208033 ProjectB_clientside_template_package-0.5/
+-rw-rw-rw-   0        0        0      489 2023-05-30 02:38:14.207033 ProjectB_clientside_template_package-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 02:38:14.171531 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/
+drwxrwxrwx   0        0        0        0 2023-05-30 02:38:14.189433 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/ClientSocketControl/
+-rw-rw-rw-   0        0        0      840 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py
+-rw-rw-rw-   0        0        0     3670 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py
+-rw-rw-rw-   0        0        0     4129 2023-05-30 02:27:12.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/MainController.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:38:14.195963 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/
+-rw-rw-rw-   0        0        0     2403 2023-05-30 02:37:11.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/Order.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:38:14.204023 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/
+-rw-rw-rw-   0        0        0      162 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Action.py
+-rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/Direction.py
+-rw-rw-rw-   0        0        0      161 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/ExpiryDate.py
+-rw-rw-rw-   0        0        0      147 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/OrderActionConstants/StrikePrice.py
+-rw-rw-rw-   0        0        0      365 2023-05-29 03:28:41.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/Profile.py
+-rw-rw-rw-   0        0        0     2037 2023-05-30 02:36:48.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/TradeController.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:38:14.184935 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package.egg-info/
+-rw-rw-rw-   0        0        0      489 2023-05-30 02:38:14.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2023-05-30 02:38:14.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 02:38:14.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-30 02:38:14.000000 ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      526 2023-05-30 02:37:38.000000 ProjectB_clientside_template_package-0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 02:38:14.209032 ProjectB_clientside_template_package-0.5/setup.cfg
```

### Comparing `ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py` & `ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/ClientSocketControl/DataStructure.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py` & `ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/ClientSocketControl/SocketClient.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/MainController.py` & `ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/MainController.py`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/Order.py` & `ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/Order.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uuid
 import random
 from datetime import datetime
 from typing import List
 from ProjectB_clientside_template_package.ClientSocketControl import DataStructure
 from ProjectB_clientside_template_package.TradeControl.OrderActionConstants import Action, Direction, ExpiryDate, StrikePrice
-from TradeControl.Profile import Profile
+from ProjectB_clientside_template_package.TradeControl.Profile import Profile
 import json
 
 
 class Order:
     def __init__(self, symbol, action, direction, sp, ed, quantity, remained, traded, averageTradePrice, lastUpdateDateTime, historyNodeOrNot):
         self.symbol = symbol
         self.orderid = 1
```

### Comparing `ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package/TradeControl/TradeController.py` & `ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package/TradeControl/TradeController.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, Union
-from ClientSocketControl import DataStructure
+from ProjectB_clientside_template_package.ClientSocketControl import DataStructure
 from ProjectB_clientside_template_package.TradeControl.Order import Order
 from ProjectB_clientside_template_package.TradeControl.OrderActionConstants import Action, Direction, ExpiryDate, StrikePrice
 from ProjectB_clientside_template_package.TradeControl.Profile import Profile
 import json
 import random
```

### Comparing `ProjectB_clientside_template_package-0.4/ProjectB_clientside_template_package.egg-info/SOURCES.txt` & `ProjectB_clientside_template_package-0.5/ProjectB_clientside_template_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ProjectB_clientside_template_package-0.4/pyproject.toml` & `ProjectB_clientside_template_package-0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ProjectB_clientside_template_package"
-version = "0.4"
+version = "0.5"
 authors = [
   { name="ProjectB", email="admin@projectb.click" },
 ]
 description = "This is the pip package of ProjectB_clientside_template_package"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

