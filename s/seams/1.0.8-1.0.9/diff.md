# Comparing `tmp/seams-1.0.8.tar.gz` & `tmp/seams-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seams-1.0.8.tar", last modified: Fri Feb  3 18:53:09 2023, max compression
+gzip compressed data, was "dist/seams-1.0.9.tar", last modified: Fri Feb  3 20:51:21 2023, max compression
```

## Comparing `seams-1.0.8.tar` & `seams-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 18:53:09.000000 seams-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    11008 2023-02-03 18:53:09.000000 seams-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8399 2023-02-03 18:52:52.000000 seams-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 18:53:09.000000 seams-1.0.8/seams/
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-02-03 18:52:52.000000 seams-1.0.8/seams/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-02-03 18:52:52.000000 seams-1.0.8/seams/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    15454 2023-02-03 18:52:52.000000 seams-1.0.8/seams/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)    20334 2023-02-03 18:52:52.000000 seams-1.0.8/seams/seams.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-02-03 18:52:52.000000 seams-1.0.8/seams/severity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 18:53:09.000000 seams-1.0.8/seams.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11008 2023-02-03 18:53:09.000000 seams-1.0.8/seams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2023-02-03 18:53:09.000000 seams-1.0.8/seams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-03 18:53:09.000000 seams-1.0.8/seams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-03 18:53:09.000000 seams-1.0.8/seams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-02-03 18:53:09.000000 seams-1.0.8/seams.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-02-03 18:53:09.000000 seams-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1457 2023-02-03 18:52:52.000000 seams-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 20:51:21.000000 seams-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    11008 2023-02-03 20:51:21.000000 seams-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8399 2023-02-03 20:51:02.000000 seams-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 20:51:21.000000 seams-1.0.9/seams/
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-02-03 20:51:02.000000 seams-1.0.9/seams/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-02-03 20:51:02.000000 seams-1.0.9/seams/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15855 2023-02-03 20:51:02.000000 seams-1.0.9/seams/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)    20281 2023-02-03 20:51:02.000000 seams-1.0.9/seams/seams.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-02-03 20:51:02.000000 seams-1.0.9/seams/severity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 20:51:21.000000 seams-1.0.9/seams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11008 2023-02-03 20:51:21.000000 seams-1.0.9/seams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2023-02-03 20:51:21.000000 seams-1.0.9/seams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-03 20:51:21.000000 seams-1.0.9/seams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-02-03 20:51:21.000000 seams-1.0.9/seams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-02-03 20:51:21.000000 seams-1.0.9/seams.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-02-03 20:51:21.000000 seams-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2023-02-03 20:51:02.000000 seams-1.0.9/setup.py
```

### Comparing `seams-1.0.8/PKG-INFO` & `seams-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seams
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python SDK for the Seams API
 Home-page: https://github.com/user/reponame
 Author: David Bickford
 Author-email: dbickford@rjleegroup.com
 License: UNKNOWN
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: # Seams SDK
```

### Comparing `seams-1.0.8/README.md` & `seams-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `seams-1.0.8/seams/pipeline.py` & `seams-1.0.9/seams/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,30 +7,39 @@
 import time
 import calendar
 import datetime
 import argparse
 import sys
 from seams.severity import Severity
 from traceback import format_tb
+from dotenv import load_dotenv
+load_dotenv()
 class Pipeline(ABC):
     
 
-    def __init__(self, SECRET, APP_ID, TENANT_ID, URL=None):
+    def __init__(self, SECRET=None, APP_ID=None, TENANT_ID=None, URL=None, AD_AUTH_MODE=None):
         '''
         Create an instance of the Pipeline interface
         '''
         self.result_files = []
         self.logs = []
         self.user_logs = []
         self.secret = SECRET
-        if URL:
-            self.seams = Seams(URL)
-        else:
-            self.seams = Seams()
-        self.seams.connect(SECRET, APP_ID, TENANT_ID)
+        if SECRET is None:
+            SECRET = os.getenv("AD_APP_SECRET")
+        if APP_ID is None:
+            APP_ID = os.getenv("AD_APP_ID")
+        if TENANT_ID is None:
+            TENANT_ID = os.getenv("AD_TENANT_ID")
+        if URL is None:
+            URL = os.getenv("API_URL")
+        if AD_AUTH_MODE is None:
+            AD_AUTH_MODE = os.getenv("AD_AUTH_MODE")
+        self.seams = Seams(URL)
+        self.seams.connect(SECRET, APP_ID, TENANT_ID, AD_AUTH_MODE)
 
     
     @abstractmethod
     def run(self, data):
         '''
         Abstract class that will be overwritten by the user
         '''
```

### Comparing `seams-1.0.8/seams/seams.py` & `seams-1.0.9/seams/seams.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,48 +2,49 @@
 from requests import Request, Session, utils
 from itertools import islice
 import mimetypes
 from seams.exceptions import SeamsException, SeamsAPIException
 import json
 import msal
 import os
-AD_AUTH_MODE = os.getenv("AD_AUTH_MODE")
 
 class Seams(object):
     '''
     A Python interface for the Seams API
     '''
     
     def __init__(self, 
-                 URL='https://seams-dev-api.rjlglims.com/api'):
+                 URL):
         '''
         Create an instance of the Seams API interface
         '''
 
         self.URL = URL
         self.connected = False
 
 
     def connect(self,
                 secret,
                 app_id,
-                tenant_id):
+                tenant_id,
+                ad_auth=None):
         '''
         Connect to the Seams API
         :param secret:
             A secret given by RJLG staff to access the Seams SDK  **REQUIRED**
         :param app_id:
             An application ID given by RJLG staff to access the Seams SDK  **REQUIRED**
         :param tenant_id:
             A tenant ID given by RJLG staff to access the Seams SDK  **REQUIRED**
         :returns:
             None
         '''
+        
         self.app_id = app_id
-        if AD_AUTH_MODE is not None and AD_AUTH_MODE == "local":
+        if ad_auth is not None and ad_auth == "local":
             authority = "https://seams-ad.rjlglims.com/adfs"
             self.scopes = ["openid","profile"]
         else:
             authority="https://login.microsoftonline.com/{}".format(tenant_id)
             self.scopes = ["api://{}/.default".format(self.app_id)]
 
         self.app = msal.ConfidentialClientApplication(
```

### Comparing `seams-1.0.8/seams.egg-info/PKG-INFO` & `seams-1.0.9/seams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seams
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python SDK for the Seams API
 Home-page: https://github.com/user/reponame
 Author: David Bickford
 Author-email: dbickford@rjleegroup.com
 License: UNKNOWN
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: # Seams SDK
```

### Comparing `seams-1.0.8/setup.py` & `seams-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = open('README.md').read()
 setup(
   name = 'seams',         
   packages = ['seams'],   
-  version = '1.0.8',      
+  version = '1.0.9',      
   license='',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A python SDK for the Seams API',  
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'David Bickford',                   
   author_email = 'dbickford@rjleegroup.com',   
   url = 'https://github.com/user/reponame',
```

