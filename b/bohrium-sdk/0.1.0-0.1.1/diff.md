# Comparing `tmp/bohrium-sdk-0.1.0.tar.gz` & `tmp/bohrium-sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.1.0.tar", last modified: Tue May 30 07:09:32 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.1.1.tar", last modified: Tue May 30 07:14:33 2023, max compression
```

## Comparing `bohrium-sdk-0.1.0.tar` & `bohrium-sdk-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:09:32.685542 bohrium-sdk-0.1.0/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      206 2023-05-30 07:09:32.685274 bohrium-sdk-0.1.0/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.1.0/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:09:32.677835 bohrium-sdk-0.1.0/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      206 2023-05-30 07:09:32.000000 bohrium-sdk-0.1.0/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      459 2023-05-30 07:09:32.000000 bohrium-sdk-0.1.0/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-30 07:09:32.000000 bohrium-sdk-0.1.0/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-30 07:09:32.000000 bohrium-sdk-0.1.0/bohrium_sdk.egg-info/entry_points.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-05-30 07:09:32.000000 bohrium-sdk-0.1.0/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:09:32.683641 bohrium-sdk-0.1.0/bohriumsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.1.0/bohriumsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.1.0/bohriumsdk/__main__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     6531 2023-05-30 01:45:26.000000 bohrium-sdk-0.1.0/bohriumsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1970 2023-05-30 07:06:19.000000 bohrium-sdk-0.1.0/bohriumsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     3766 2023-05-30 07:06:03.000000 bohrium-sdk-0.1.0/bohriumsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.1.0/bohriumsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2209 2023-05-30 07:06:47.000000 bohrium-sdk-0.1.0/bohriumsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2835 2023-05-30 07:06:55.000000 bohrium-sdk-0.1.0/bohriumsdk/storage.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:09:32.684677 bohrium-sdk-0.1.0/bohriumsdk/test/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.1.0/bohriumsdk/test/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.1.0/bohriumsdk/test/test_node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2369 2023-05-30 01:45:00.000000 bohrium-sdk-0.1.0/bohriumsdk/test.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     3120 2023-05-30 07:07:00.000000 bohrium-sdk-0.1.0/bohriumsdk/util.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-30 07:09:32.685594 bohrium-sdk-0.1.0/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      502 2023-05-30 01:46:18.000000 bohrium-sdk-0.1.0/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:14:33.683892 bohrium-sdk-0.1.1/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-30 07:14:33.683622 bohrium-sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.1.1/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:14:33.670118 bohrium-sdk-0.1.1/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-30 07:14:33.000000 bohrium-sdk-0.1.1/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      459 2023-05-30 07:14:33.000000 bohrium-sdk-0.1.1/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-30 07:14:33.000000 bohrium-sdk-0.1.1/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-30 07:14:33.000000 bohrium-sdk-0.1.1/bohrium_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-05-30 07:14:33.000000 bohrium-sdk-0.1.1/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:14:33.682366 bohrium-sdk-0.1.1/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.1.1/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.1.1/bohriumsdk/__main__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     6220 2023-05-30 07:14:12.000000 bohrium-sdk-0.1.1/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1970 2023-05-30 07:06:19.000000 bohrium-sdk-0.1.1/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     3766 2023-05-30 07:06:03.000000 bohrium-sdk-0.1.1/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.1.1/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2209 2023-05-30 07:06:47.000000 bohrium-sdk-0.1.1/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2835 2023-05-30 07:06:55.000000 bohrium-sdk-0.1.1/bohriumsdk/storage.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:14:33.682933 bohrium-sdk-0.1.1/bohriumsdk/test/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.1.1/bohriumsdk/test/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.1.1/bohriumsdk/test/test_node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2369 2023-05-30 01:45:00.000000 bohrium-sdk-0.1.1/bohriumsdk/test.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     3120 2023-05-30 07:07:00.000000 bohrium-sdk-0.1.1/bohriumsdk/util.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-30 07:14:33.683950 bohrium-sdk-0.1.1/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      501 2023-05-30 07:14:29.000000 bohrium-sdk-0.1.1/setup.py
```

### Comparing `bohrium-sdk-0.1.0/bohriumsdk/client.py` & `bohrium-sdk-0.1.1/bohriumsdk/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,14 @@
 import json
 import urllib
 import getpass
 import time
 import configparser
 import re
 
-def check_email(email):
-    email_regex = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\\.[a-zA-Z]{2,}$'
-    if re.match(email_regex, email): return True
-    else: return False
-
 class RequestInfoException(Exception):
     pass
 
 class Client:
     def __init__(
             self, 
             api_version: str = 'v2',
@@ -25,51 +20,50 @@
             base_url_v2: str = "https://openapi.dp.tech",
             token: str = "",
             debug: bool = False,
             use_config_file: bool = False,
             config_file_location_v1: str = '~/.lebesgue_config.json',
             config_file_location_v2: str ='~/.brmconfig'
         ) -> None:
-        match api_version:
-            case "v1":
-                self.debug = debug
-                self.debug = os.getenv('LBG_CLI_DEBUG_PRINT', debug)
-                self.config = {}
-                config_file_location_expand = os.path.expanduser(config_file_location_v1)
-                file_data = {}
-                self.token = ''
-                self.user_id = None
-                if use_config_file:
-                    if os.path.exists(config_file_location_expand):
-                        with open(config_file_location_expand, 'r') as f:
-                            file_data = json.loads(f.read())
-                    self.config['email'] = file_data.get('email', email)
-                    self.config['password'] = file_data.get('password', password)
-                    self.base_url = file_data.get('base_url', base_url_v1)
-                else:
-                    self.config['email'] = email
-                    self.config['password'] = password
-                    self.base_url = base_url_v1
-                if token is not None:
-                    self.token = token
-                else:
-                    self._login()
-            case "v2":
-                self.config_file_location_expand = os.path.expanduser(config_file_location_v2)
-                if not os.path.exists(self.config_file_location_expand):
-                    print("Config File ~/.brmconfig not found! Now login to bohrium and generate it!")
-                    self.login()
-                    access_key_name = input("Please enter access_key name: ")
-                    self.generate_access_key(access_key_name)
-                config = configparser.ConfigParser()
-                config.read(self.config_file_location_expand)
-                self.base_url = config.get('Credentials', 'baseUrl')
-                self.access_key = config.get('Credentials', 'accessKey')
-                self.params = {"accessKey": self.access_key}
-                self.token = ""
+        if api_version == "v1":
+            self.debug = debug
+            self.debug = os.getenv('LBG_CLI_DEBUG_PRINT', debug)
+            self.config = {}
+            config_file_location_expand = os.path.expanduser(config_file_location_v1)
+            file_data = {}
+            self.token = ''
+            self.user_id = None
+            if use_config_file:
+                if os.path.exists(config_file_location_expand):
+                    with open(config_file_location_expand, 'r') as f:
+                        file_data = json.loads(f.read())
+                self.config['email'] = file_data.get('email', email)
+                self.config['password'] = file_data.get('password', password)
+                self.base_url = file_data.get('base_url', base_url_v1)
+            else:
+                self.config['email'] = email
+                self.config['password'] = password
+                self.base_url = base_url_v1
+            if token is not None:
+                self.token = token
+            else:
+                self._login()
+        elif api_version == "v2":
+            self.config_file_location_expand = os.path.expanduser(config_file_location_v2)
+            if not os.path.exists(self.config_file_location_expand):
+                print("Config File ~/.brmconfig not found! Now login to bohrium and generate it!")
+                self.login()
+                access_key_name = input("Please enter access_key name: ")
+                self.generate_access_key(access_key_name)
+            config = configparser.ConfigParser()
+            config.read(self.config_file_location_expand)
+            self.base_url = config.get('Credentials', 'baseUrl')
+            self.access_key = config.get('Credentials', 'accessKey')
+            self.params = {"accessKey": self.access_key}
+            self.token = ""
 
     def post(self, url, host="", data=None, headers=None, params=None, stream=False, retry=5):
         return self._req('POST', url, host=host, data=data, headers=headers, params=params, stream=stream, retry=retry)
 
     def get(self, url, host="", data=None, headers=None, params=None, stream=False, retry=5):
         return self._req('GET', url, host=host, data=data, headers=headers, params=params, stream=stream, retry=retry)
```

### Comparing `bohrium-sdk-0.1.0/bohriumsdk/image.py` & `bohrium-sdk-0.1.1/bohriumsdk/image.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.0/bohriumsdk/job.py` & `bohrium-sdk-0.1.1/bohriumsdk/job.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.0/bohriumsdk/node.py` & `bohrium-sdk-0.1.1/bohriumsdk/node.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.0/bohriumsdk/project.py` & `bohrium-sdk-0.1.1/bohriumsdk/project.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.0/bohriumsdk/storage.py` & `bohrium-sdk-0.1.1/bohriumsdk/storage.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.0/bohriumsdk/test.py` & `bohrium-sdk-0.1.1/bohriumsdk/test.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.0/bohriumsdk/util.py` & `bohrium-sdk-0.1.1/bohriumsdk/util.py`

 * *Files identical despite different names*

