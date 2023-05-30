# Comparing `tmp/econuker-1.0.8.tar.gz` & `tmp/econuker-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econuker-1.0.8.tar", last modified: Mon May 29 17:11:04 2023, max compression
+gzip compressed data, was "econuker-1.0.9.tar", last modified: Tue May 30 03:08:56 2023, max compression
```

## Comparing `econuker-1.0.8.tar` & `econuker-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 17:11:04.588586 econuker-1.0.8/
--rw-rw-rw-   0        0        0     5069 2023-05-29 17:11:04.586587 econuker-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4262 2023-05-29 17:09:06.000000 econuker-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 17:11:04.549817 econuker-1.0.8/econuker/
--rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.8/econuker/Exceptions.py
--rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.8/econuker/__init__.py
--rw-rw-rw-   0        0        0    14456 2023-05-29 14:15:21.000000 econuker-1.0.8/econuker/async_client.py
--rw-rw-rw-   0        0        0    13841 2023-05-29 14:15:03.000000 econuker-1.0.8/econuker/client.py
-drwxrwxrwx   0        0        0        0 2023-05-29 17:11:04.579605 econuker-1.0.8/econuker.egg-info/
--rw-rw-rw-   0        0        0     5069 2023-05-29 17:11:03.000000 econuker-1.0.8/econuker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-29 17:11:04.000000 econuker-1.0.8/econuker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 17:11:03.000000 econuker-1.0.8/econuker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-29 17:11:03.000000 econuker-1.0.8/econuker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 17:11:03.000000 econuker-1.0.8/econuker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 17:11:04.589583 econuker-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1165 2023-05-29 17:10:58.000000 econuker-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:08:56.433760 econuker-1.0.9/
+-rw-rw-rw-   0        0        0     5098 2023-05-30 03:08:56.432759 econuker-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4291 2023-05-29 18:48:49.000000 econuker-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 03:08:56.417760 econuker-1.0.9/econuker/
+-rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.9/econuker/Exceptions.py
+-rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.9/econuker/__init__.py
+-rw-rw-rw-   0        0        0    14664 2023-05-29 18:48:03.000000 econuker-1.0.9/econuker/async_client.py
+-rw-rw-rw-   0        0        0    13972 2023-05-30 00:27:57.000000 econuker-1.0.9/econuker/client.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:08:56.429759 econuker-1.0.9/econuker.egg-info/
+-rw-rw-rw-   0        0        0     5098 2023-05-30 03:08:56.000000 econuker-1.0.9/econuker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-30 03:08:56.000000 econuker-1.0.9/econuker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 03:08:56.000000 econuker-1.0.9/econuker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-30 03:08:56.000000 econuker-1.0.9/econuker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 03:08:56.000000 econuker-1.0.9/econuker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 03:08:56.434761 econuker-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2023-05-30 03:08:51.000000 econuker-1.0.9/setup.py
```

### Comparing `econuker-1.0.8/PKG-INFO` & `econuker-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econuker
-Version: 1.0.8
+Version: 1.0.9
 Summary: API wrapper for https://api.econuker.xyz
 Home-page: https://github.com/EcoNuker/EcoNuker-API-Python/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -119,14 +119,15 @@
 ### Methods
 A list of methods you can call with either Client or AsyncClient.
 - `.status()` (class StatusData)
     - `.name` (string)
     - `.status` (string)
     - `.servers` (integer)
     - `.latency` (float)
+    - `._raw` (dict)
 - `.ping()` (bool)
 - `.verify(auth_token)` (Union(class Token, False))
     - `.authtoken` (string)
     - `.authlevel` (string)
     - `._raw` (dict)
 - `.fetch_servers()` (class ServersResult)
     - `.count` (integer)
@@ -136,15 +137,15 @@
     - `.name` (string)
     - `.id` (string)
     - `.owner` (class Owner)
         - `.name` (string)
         - `.id` (string)
         - `.nick` (Union(string, None))
         - `.profile` (string)
-        - `._raw`
+        - `._raw` (dict)
     - `.url` (Union(string, None))
     - `.verified` (bool)
     - `.created_at` (integer)
     - `.timezone` (string)
     - `.slug` (Union(string, None))
     - `.about` (Union(string, None))
     - `._raw` (dict)
```

### Comparing `econuker-1.0.8/README.md` & `econuker-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 ### Methods
 A list of methods you can call with either Client or AsyncClient.
 - `.status()` (class StatusData)
     - `.name` (string)
     - `.status` (string)
     - `.servers` (integer)
     - `.latency` (float)
+    - `._raw` (dict)
 - `.ping()` (bool)
 - `.verify(auth_token)` (Union(class Token, False))
     - `.authtoken` (string)
     - `.authlevel` (string)
     - `._raw` (dict)
 - `.fetch_servers()` (class ServersResult)
     - `.count` (integer)
@@ -116,15 +117,15 @@
     - `.name` (string)
     - `.id` (string)
     - `.owner` (class Owner)
         - `.name` (string)
         - `.id` (string)
         - `.nick` (Union(string, None))
         - `.profile` (string)
-        - `._raw`
+        - `._raw` (dict)
     - `.url` (Union(string, None))
     - `.verified` (bool)
     - `.created_at` (integer)
     - `.timezone` (string)
     - `.slug` (Union(string, None))
     - `.about` (Union(string, None))
     - `._raw` (dict)
```

### Comparing `econuker-1.0.8/econuker/Exceptions.py` & `econuker-1.0.9/econuker/Exceptions.py`

 * *Files identical despite different names*

### Comparing `econuker-1.0.8/econuker/async_client.py` & `econuker-1.0.9/econuker/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,23 +37,23 @@
     Owner object.
 
     Attributes:
         _raw (str): Raw owner data.
         name (str): Owner name.
         id (str): Owner ID.
         nick (str, None): Owner nickname.
-        profile (str, None): Owner profile.
+        profile (str): Owner profile.
     """
 
     def __init__(self, data):
         self._raw: str = data
         self.name = data["name"]
         self.id = data["id"]
-        self.nick = data.get("nick")
-        self.profile = data.get("profile")
+        self.nick:str|None = data.get("nick")
+        self.profile:str = data.get("profile")
 
 class ItemPrice:
     """
     ItemPrice object.
 
     Attributes:
         _raw (dict): Raw item price data, excluding worth.
@@ -103,17 +103,14 @@
     """
 
     def __init__(self, auth_token: str = None, beta: bool = False):
         self.auth_token: str = auth_token
         self.base_url: str = "https://beta.econuker.xyz/api" if beta else "https://econuker.xyz/api"
         self.auth_level: str = None
 
-        if not beta:
-            raise EconukerException("Main API is not available at this moment.")
-
         def __check_verify(self) -> Token:
             """
             Verifies an authentication token.
 
             Args:
                 auth_token (str): The authentication token to verify.
 
@@ -162,21 +159,22 @@
         """
         StatusData object.
 
         Args:
             data (dict): Data containing the route information.
 
         Attributes:
+            _raw (dict): Raw data returned from the API.
             name (str): The name of the route.
             status (str): The status of the route.
             servers (int): The number of servers associated with the route.
             latency (float): The latency of the route.
-
         """
         def __init__(self, data):
+            self._raw:dict = data
             self.name:str = data["name"]
             self.status:str = data["status"]
             self.servers:int = data["servers"]
             self.latency:float = data["latency"]
 
     async def status(self) -> StatusData:
         """
@@ -220,43 +218,47 @@
         ServersResult object.
 
         Attributes:
             _raw (dict): Raw API JSON data.
             count (int): Server count.
             server_ids (list): List of server IDs.
         """
+        def __init__(self, data):
+            self._raw: dict = data
+            self.count: int = data.get("count", 0)
+            self.server_ids: list = data.get("servers", [])
 
     class ServerResult:
         """
         ServerResult object.
 
         Attributes:
             _raw (dict): Raw API JSON data.
             name (str): Server name.
             id (str): Server ID.
             owner (Owner): Owner object.
             url (str, None): The vanity URL of the server, if it exists.
             verified (bool): Indicates whether the server is verified.
             created_at (int): Epoch timestamp.
-            timezone (str): The raw timezone of the server.
-            slug (str): The server's slug.
+            timezone (str, None): The raw timezone of the server.
+            slug (str, None): The server's slug.
             about (str, None): The server's "about me" information.
         """
 
         def __init__(self, data):
             self._raw: dict = data
             self.id: str = data["id"]
             self.name: str = data["name"]
             self.owner: Owner = Owner(data["owner"])
-            self.url: str = data["vanity_url"]
+            self.url: str|None = data["vanity_url"]
             self.verified: bool = data["verified"]
             self.created_at: int = data["created_at"]
-            self.timezone: str = data["timezone"]
-            self.slug: str = data["slug"]
-            self.about: str = data["about"]
+            self.timezone: str|None = data["timezone"]
+            self.slug: str|None = data["slug"]
+            self.about: str|None = data["about"]
 
     async def fetch_servers(self) -> ServersResult:
         """
         Fetches a list of all servers.
 
         Returns:
             ServersResult
```

### Comparing `econuker-1.0.8/econuker/client.py` & `econuker-1.0.9/econuker/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         response (requests.Response): The response object from the API request.
 
     Raises:
         Forbidden: If the response status code is 403.
         Unauthorized: If the response status code is 401.
         NotFound: If the response status code is 404.
         InternalServerError: If the response status code is 500.
-        RateLimited: If the response status code is 429.
+        RateLimited: tIf the response status code is 429.
         EconukerException: If the response status code does not match any known error codes.
     """
     if response.status_code == 403:
         raise Forbidden(f"{response.content.decode()}")
     elif response.status_code == 401:
         raise Unauthorized(f"{response.content.decode()}")
     elif response.status_code == 404:
@@ -37,23 +37,23 @@
     Owner object.
 
     Attributes:
         _raw (str): Raw owner data.
         name (str): Owner name.
         id (str): Owner ID.
         nick (str, None): Owner nickname.
-        profile (str, None): Owner profile.
+        profile (str): Owner profile.
     """
 
     def __init__(self, data):
         self._raw: str = data
         self.name = data["name"]
         self.id = data["id"]
-        self.nick = data.get("nick")
-        self.profile = data.get("profile")
+        self.nick:str|None = data.get("nick")
+        self.profile:str = data.get("profile")
 
 class ItemPrice:
     """
     ItemPrice object.
 
     Attributes:
         _raw (dict): Raw item price data, excluding worth.
@@ -142,21 +142,22 @@
         """
         StatusData object.
 
         Args:
             data (dict): Data containing the route information.
 
         Attributes:
+            _raw (dict): Raw data returned from the API.
             name (str): The name of the route.
             status (str): The status of the route.
             servers (int): The number of servers associated with the route.
             latency (float): The latency of the route.
-
         """
         def __init__(self, data):
+            self._raw:dict = data
             self.name:str = data["name"]
             self.status:str = data["status"]
             self.servers:int = data["servers"]
             self.latency:float = data["latency"]
 
     def status(self) -> StatusData:
         """
@@ -233,30 +234,30 @@
             _raw (dict): Raw API JSON data.
             name (str): Server name.
             id (str): Server ID.
             owner (Owner): Owner object.
             url (str, None): The vanity URL of the server, if it exists.
             verified (bool): Indicates whether the server is verified.
             created_at (int): Epoch timestamp.
-            timezone (str): The raw timezone of the server.
-            slug (str): The server's slug.
+            timezone (str, None): The raw timezone of the server.
+            slug (str, None): The server's slug.
             about (str, None): The server's "about me" information.
         """
 
         def __init__(self, data):
             self._raw: dict = data
             self.id: str = data["id"]
             self.name: str = data["name"]
             self.owner: Owner = Owner(data["owner"])
-            self.url: str = data["vanity_url"]
+            self.url: str|None = data["vanity_url"]
             self.verified: bool = data["verified"]
             self.created_at: int = data["created_at"]
-            self.timezone: str = data["timezone"]
-            self.slug: str = data["slug"]
-            self.about: str = data["about"]
+            self.timezone: str|None = data["timezone"]
+            self.slug: str|None = data["slug"]
+            self.about: str|None = data["about"]
     
     def fetch_servers(self) -> ServersResult:
         """
         Fetches a list of all servers.
         
         Returns:
             ServersResult
```

### Comparing `econuker-1.0.8/econuker.egg-info/PKG-INFO` & `econuker-1.0.9/econuker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econuker
-Version: 1.0.8
+Version: 1.0.9
 Summary: API wrapper for https://api.econuker.xyz
 Home-page: https://github.com/EcoNuker/EcoNuker-API-Python/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -119,14 +119,15 @@
 ### Methods
 A list of methods you can call with either Client or AsyncClient.
 - `.status()` (class StatusData)
     - `.name` (string)
     - `.status` (string)
     - `.servers` (integer)
     - `.latency` (float)
+    - `._raw` (dict)
 - `.ping()` (bool)
 - `.verify(auth_token)` (Union(class Token, False))
     - `.authtoken` (string)
     - `.authlevel` (string)
     - `._raw` (dict)
 - `.fetch_servers()` (class ServersResult)
     - `.count` (integer)
@@ -136,15 +137,15 @@
     - `.name` (string)
     - `.id` (string)
     - `.owner` (class Owner)
         - `.name` (string)
         - `.id` (string)
         - `.nick` (Union(string, None))
         - `.profile` (string)
-        - `._raw`
+        - `._raw` (dict)
     - `.url` (Union(string, None))
     - `.verified` (bool)
     - `.created_at` (integer)
     - `.timezone` (string)
     - `.slug` (Union(string, None))
     - `.about` (Union(string, None))
     - `._raw` (dict)
```

### Comparing `econuker-1.0.8/setup.py` & `econuker-1.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='econuker',
-    version='1.0.8',
+    version='1.0.9',
     author='YumYummity',
     author_email='034nop@gmail.com',
     description='API wrapper for https://api.econuker.xyz',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type
     url='https://github.com/EcoNuker/EcoNuker-API-Python/',
     packages=find_packages(),
```

