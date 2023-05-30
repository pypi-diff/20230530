# Comparing `tmp/vlogs-1.0.4.tar.gz` & `tmp/vlogs-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlogs-1.0.4.tar", max compression
+gzip compressed data, was "vlogs-1.0.5.tar", max compression
```

## Comparing `vlogs-1.0.4.tar` & `vlogs-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1222 2023-05-29 14:39:46.449093 vlogs-1.0.4/README.md
--rw-r--r--   0        0        0      342 2023-05-29 15:35:10.625758 vlogs-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       28 2023-05-29 12:28:45.438951 vlogs-1.0.4/vlogs/__init__.py
--rw-r--r--   0        0        0       43 2023-05-29 12:42:40.212891 vlogs-1.0.4/vlogs/config.py
--rw-r--r--   0        0        0    11646 2023-05-29 14:51:51.425511 vlogs-1.0.4/vlogs/model.py
--rw-r--r--   0        0        0     2554 2023-05-29 14:51:12.793514 vlogs-1.0.4/vlogs/sdk.py
--rw-r--r--   0        0        0      733 2023-05-29 15:36:08.720409 vlogs-1.0.4/vlogs/service.py
--rw-r--r--   0        0        0      500 2023-05-29 14:46:08.230314 vlogs-1.0.4/vlogs/util.py
--rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 vlogs-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1136 2023-05-30 03:04:48.623737 vlogs-1.0.5/README.md
+-rw-r--r--   0        0        0      502 2023-05-30 02:56:50.567460 vlogs-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-05-30 01:37:14.600505 vlogs-1.0.5/vlogs/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-30 01:52:01.274835 vlogs-1.0.5/vlogs/config.py
+-rw-r--r--   0        0        0    12157 2023-05-30 02:06:04.426545 vlogs-1.0.5/vlogs/model.py
+-rw-r--r--   0        0        0     3768 2023-05-30 02:54:00.618822 vlogs-1.0.5/vlogs/sdk.py
+-rw-r--r--   0        0        0     1690 2023-05-30 03:02:59.521019 vlogs-1.0.5/vlogs/service.py
+-rw-r--r--   0        0        0      500 2023-05-30 01:37:14.604505 vlogs-1.0.5/vlogs/util.py
+-rw-r--r--   0        0        0     1604 1970-01-01 00:00:00.000000 vlogs-1.0.5/PKG-INFO
```

### Comparing `vlogs-1.0.4/README.md` & `vlogs-1.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 # vLogs SDK for Python
 
 A simple way to collect logs and send to the server via simple SDK.
 
--   [x] Collect the logs
+-   [x] Collect the logs (Sync and Async support)
 -   [ ] Support local retries
 
 ### Install via `pip`
 
 ```shell
 pip install vlogs
 ```
 
 ### Usages
 
 ```python
 from vlogs.sdk import VLogs, VLogsOptions
 from vlogs.model import Collector, CollectorType, CollectorSource
-import asyncio
 
 appId = "72bd14c306a91fa8a590330e3898ddcc"
 apiKey = "vlogs_gX9WwSdKatMNdpUClLU0IfCx575tvdoeQ"
 
 # Create VLogs instance
 sdk = VLogs.create(
     VLogsOptions.builder()
     .apiKey(apiKey)
     .appId(appId)
     .build()
 )
 
-async def main():
-    response = await sdk.collect(
-        Collector.builder()
-        .type(CollectorType.Error)
-        .source(CollectorSource.Other)
-        .message("This is a test message")
-        .build()
-    )
-
-    print("Response: ", response)
+response = await sdk.collect(
+    Collector.builder()
+    .type(CollectorType.Error)
+    .source(CollectorSource.Other)
+    .message("This is a test message")
+    .build()
+)
 
-# Run the async function
-asyncio.run(main())
+print("Response: ", response)
 ```
 
 ### Build, Install, and Test from Source
 
 ```shell
 make
 ```
```

### Comparing `vlogs-1.0.4/vlogs/model.py` & `vlogs-1.0.5/vlogs/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,17 @@
             "token": self.token,
             "chat_id": self.chatId,
             "parse_mode": self.parseMode,
             "disabled": self.disabled,
             "extras": self.extras,
         }
 
+    def __str__(self) -> str:
+        return json.dumps(self.to_map())
+
     @staticmethod
     def builder():
         return TelegramBuilder()
 
 
 class TelegramBuilder:
     def __init__(self):
@@ -112,14 +115,17 @@
             "webhook_id": self.webhookId,
             "webhook_token": self.webhookToken,
             "webhook_url": self.webhookUrl,
             "disabled": self.disabled,
             "extras": self.extras,
         }
 
+    def __str__(self) -> str:
+        return json.dumps(self.to_map())
+
     @staticmethod
     def builder():
         return DiscordBuilder()
 
 
 class DiscordBuilder:
     def __init__(self):
@@ -156,99 +162,105 @@
             webhookUrl=self._webhookUrl,
             disabled=self._disabled,
             extras=self._extras
         )
 
 
 class SDKInfo:
-    def __init__(self, name=None, version=None, versionCode=None, hostname=None, sender=None):
+    def __init__(self, name=None, version=None, version_code=None, hostname=None, sender=None):
         self.name = name
         self.version = version
-        self.versionCode = versionCode
+        self.version_code = version_code
         self.hostname = hostname
         self.sender = sender
 
     def to_map(self):
         return {
             'name': self.name,
             'version': self.version,
-            'version_code': self.versionCode,
+            'version_code': self.version_code,
             'hostname': self.hostname,
             'sender': self.sender
         }
 
+    def __str__(self) -> str:
+        return json.dumps(self.to_map())
+
     @staticmethod
     def builder():
         return SDKInfoBuilder()
 
 
 class SDKInfoBuilder:
     def __init__(self):
         self._name = None
         self._version = None
-        self._versionCode = None
+        self._version_code = None
         self._hostname = None
         self._sender = None
 
     def name(self, name):
         self._name = name
         return self
 
     def version(self, version):
         self._version = version
         return self
 
-    def versionCode(self, versionCode):
-        self._versionCode = versionCode
+    def version_code(self, version_code):
+        self._version_code = version_code
         return self
 
     def hostname(self, hostname):
         self._hostname = hostname
         return self
 
     def sender(self, sender):
         self._sender = sender
         return self
 
     def build(self):
         return SDKInfo(
             name=self._name,
             version=self._version,
-            versionCode=self._versionCode,
+            version_code=self._version_code,
             hostname=self._hostname,
             sender=self._sender
         )
 
 
 class Target:
     def __init__(self, telegram: Telegram = None, discord: Discord = None, sdkInfo: SDKInfo = None):
         self.telegram = telegram
         self.discord = discord
         self.sdkInfo = sdkInfo
 
     def to_map(self):
         return {
-            'telegram': self.telegram.to_map() if self.telegram else None,
-            'discord': self.discord.to_map() if self.discord else None,
-            'sdk_info': self.sdkInfo.to_map() if self.sdkInfo else None
+            'telegram': self.telegram and self.telegram.to_map() or None,
+            'discord': self.discord and self.discord.to_map() or None,
+            'sdk_info': self.sdkInfo and self.sdkInfo.to_map() or None,
         }
 
     def merge(self, defaultTarget=None):
         if not defaultTarget:
             return
         self.telegram = self.telegram or defaultTarget.telegram
         self.discord = self.discord or defaultTarget.discord
 
+    def __str__(self) -> str:
+        return str(self.to_map())
+
     @staticmethod
-    def withTelegram(chatId, token=None, parseMode=None, disabled=None, extras=None):
+    def with_telegram(chatId, token=None, parseMode=None, disabled=None, extras=None):
         telegram = Telegram(chatId, token, parseMode, disabled, extras)
         return Target(telegram=telegram)
 
     @staticmethod
-    def withDiscord(webhookUrl, webhookId=None, webhookToken=None, disabled=None, extras=None):
+    def with_discord(webhookUrl, webhookId=None, webhookToken=None, disabled=None, extras=None):
         discord = Discord(webhookUrl, webhookId,
                           webhookToken, disabled, extras)
         return Target(discord=discord)
 
     @staticmethod
     def builder():
         return TargetBuilder()
@@ -273,49 +285,49 @@
         return self
 
     def build(self):
         return Target(telegram=self._telegram, discord=self._discord, sdkInfo=self._sdkInfo)
 
 
 class Collector:
-    def __init__(self, id=None, type=None, source=None, message=None, data=None, useragent=None, timestamp=None, target=None, tags=None):
+    def __init__(self, id=None, type=None, source=None, message=None, data=None, useragent=None, timestamp=None, target: Target = None, tags=None):
         self.id = id
         self.type = type
         self.source = source
         self.message = message
         self.data = data
         self.useragent = useragent
         self.timestamp = timestamp
         self.target = target
         self.tags = tags
 
-    def getId(self):
+    def get_id(self):
         if not self.id:
             self.id = generate_uuid()
         return self.id
 
     def get_timestamp(self):
         if not self.timestamp:
             self.timestamp = int(time.time() * 1000)
         return self.timestamp
 
     def to_map(self):
         return {
-            'id': self.getId(),
+            'id': self.get_id(),
             'type': self.type,
             'source': self.source,
             'message': self.message,
             'data': self.data,
             'user_agent': self.useragent,
             'timestamp': self.get_timestamp(),
-            'target': self.target.to_map() if self.target else None,
+            'target': self.target and self.target.to_map() or None,
             'tags': self.tags,
         }
 
-    def toJson(self):
+    def __str__(self):
         return json.dumps(self.to_map())
 
     @staticmethod
     def builder():
         return CollectorBuilder()
 
 
@@ -382,56 +394,65 @@
 
 
 class CollectorResponse:
     def __init__(self, message=None, id=None):
         self.message = message
         self.id = id
 
+    def to_map(self):
+        return {
+            'message': self.message,
+            'id': self.id
+        }
+
+    def __str__(self) -> str:
+        return json.dumps(self.to_map())
+
 
 class VLogsOptions:
-    def __init__(self, url=None, appId=None, apiKey=None, connectionTimeout=None, testConnection=None, target: Target=None):
+    def __init__(self, url=None, appId=None, apiKey=None, connection_timeout=None, test_connection=None, target: Target = None):
         self.url = url
         self.appId = appId
         self.apiKey = apiKey
-        self.connectionTimeout = connectionTimeout
-        self.testConnection = testConnection
+        self.connection_timeout = connection_timeout
+        self.test_connection = test_connection
         self.target = target
 
     @staticmethod
     def builder():
         return VLogsOptionsBuilder()
 
 
 class VLogsOptionsBuilder:
     def __init__(self):
         self._url = None
         self._appId = None
         self._apiKey = None
-        self._connectionTimeout = None
-        self._testConnection = None
+        self._connection_timeout = None
+        self._test_connection = None
         self._target = None
 
     def url(self, url):
         self._url = url
         return self
 
     def appId(self, appId):
         self._appId = appId
         return self
 
     def apiKey(self, apiKey):
         self._apiKey = apiKey
         return self
 
-    def connectionTimeout(self, connectionTimeout):
-        self._connectionTimeout = connectionTimeout
+    def connection_timeout(self, connection_timeout):
+        self._connection_timeout = connection_timeout
         return self
 
-    def testConnection(self, testConnection):
-        self._testConnection = testConnection
+    def test_connection(self, test_connection):
+        self._test_connection = test_connection
         return self
 
     def target(self, target):
         self._target = target
         return self
 
     def telegram(self, telegram):
@@ -449,11 +470,11 @@
         return self
 
     def build(self):
         return VLogsOptions(
             url=self._url,
             appId=self._appId,
             apiKey=self._apiKey,
-            connectionTimeout=self._connectionTimeout,
-            testConnection=self._testConnection,
+            connection_timeout=self._connection_timeout,
+            test_connection=self._test_connection,
             target=self._target,
         )
```

### Comparing `vlogs-1.0.4/vlogs/sdk.py` & `vlogs-1.0.5/vlogs/sdk.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from vlogs.model import Collector, CollectorResponse, SDKInfo, Target, VLogsOptions
+import asyncio
+
+from vlogs.config import BASE_URL
+from vlogs.model import (Collector, CollectorResponse, SDKInfo, Target,
+                         VLogsOptions)
 from vlogs.service import VLogsService
 from vlogs.util import get_system_hostname, get_system_username
-from vlogs.config import BASE_URL
 
 
 class VLogs:
     _logger = print
     NAME = 'vlogs'
     VERSION = '1.0.0'
     VERSION_CODE = '1'
@@ -23,46 +26,77 @@
 
         # Initialize service
         self._service = VLogsService(self._options.url)
 
         VLogs._logger(
             f'VLogs: Initialized AppID: {self._options.appId} | SDK Version: {VLogs.VERSION}-{VLogs.VERSION_CODE}')
 
-    async def collect(self, request: Collector) -> CollectorResponse:
-        VLogs._logger(f'VLogs: Collecting logs for {request.getId()}')
+    def collect(self, request: Collector) -> CollectorResponse:
+        VLogs._logger(f'VLogs: Collecting logs for {request.get_id()}')
 
         headers = {
             VLogs.APP_ID_HEADER_PREFIX: self._options.appId,
             VLogs.API_KEY_HEADER_PREFIX: self._options.apiKey,
-            'Content-Type': 'application/json',
         }
 
         hostname = get_system_hostname()
         sender = get_system_username()
-        sdk_info = SDKInfo.builder().hostname(hostname).sender(sender).name(
-            VLogs.NAME).version(VLogs.VERSION).versionCode(VLogs.VERSION_CODE).build()
+        sdkInfo = SDKInfo.builder().hostname(hostname).sender(sender).name(
+            VLogs.NAME).version(VLogs.VERSION).version_code(VLogs.VERSION_CODE).build()
 
         if not request.target:
             if self._options.target:
                 request.target = self._options.target
             else:
                 request.target = Target.builder().build()
         else:
             if self._options.target:
                 request.target.merge(self._options.target)
 
         # Set SDK info to request
-        request.target.sdk_info = sdk_info
+        request.target.sdkInfo = sdkInfo
 
         # Append user agent to request
         request.useragent = f'vlogs-python-sdk/{VLogs.VERSION}-{VLogs.VERSION_CODE} ({hostname})'
 
-        response = await self._service.post(request.to_map(), headers, self._options.connectionTimeout or VLogs.DEFAULT_CONNECT_TIMEOUT)
+        response = self._service.post(request.to_map(
+        ), headers, self._options.connection_timeout or VLogs.DEFAULT_CONNECT_TIMEOUT)
         return response
 
+    async def collect_async(self, request: Collector) -> CollectorResponse:
+        VLogs._logger(f'VLogs: Collecting logs for {request.get_id()}')
+
+        headers = {
+            VLogs.APP_ID_HEADER_PREFIX: self._options.appId,
+            VLogs.API_KEY_HEADER_PREFIX: self._options.apiKey,
+        }
+
+        hostname = get_system_hostname()
+        sender = get_system_username()
+        sdkInfo = SDKInfo.builder().hostname(hostname).sender(sender).name(
+            VLogs.NAME).version(VLogs.VERSION).version_code(VLogs.VERSION_CODE).build()
+
+        if not request.target:
+            if self._options.target:
+                request.target = self._options.target
+            else:
+                request.target = Target.builder().build()
+        else:
+            if self._options.target:
+                request.target.merge(self._options.target)
+
+        # Set SDK info to request
+        request.target.sdkInfo = sdkInfo
+
+        # Append user agent to request
+        request.useragent = f'vlogs-python-sdk/{VLogs.VERSION}-{VLogs.VERSION_CODE} ({hostname})'
+
+        return await self._service.post_async(request.to_map(
+        ), headers, self._options.connection_timeout or VLogs.DEFAULT_CONNECT_TIMEOUT)
+
     @staticmethod
     def create(options: VLogsOptions) -> 'VLogs':
         return VLogs(options)
 
     @staticmethod
     def create_with(appId: str, apiKey: str) -> 'VLogs':
         return VLogs.create(
```

### Comparing `vlogs-1.0.4/PKG-INFO` & `vlogs-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,61 @@
 Metadata-Version: 2.1
 Name: vlogs
-Version: 1.0.4
+Version: 1.0.5
 Summary: CUBETIQ vLogs SDK for Python
 License: MIT
 Author: Sambo Chea
 Author-email: sombochea@cubetiqs.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Description-Content-Type: text/markdown
 
 # vLogs SDK for Python
 
 A simple way to collect logs and send to the server via simple SDK.
 
--   [x] Collect the logs
+-   [x] Collect the logs (Sync and Async support)
 -   [ ] Support local retries
 
 ### Install via `pip`
 
 ```shell
 pip install vlogs
 ```
 
 ### Usages
 
 ```python
 from vlogs.sdk import VLogs, VLogsOptions
 from vlogs.model import Collector, CollectorType, CollectorSource
-import asyncio
 
 appId = "72bd14c306a91fa8a590330e3898ddcc"
 apiKey = "vlogs_gX9WwSdKatMNdpUClLU0IfCx575tvdoeQ"
 
 # Create VLogs instance
 sdk = VLogs.create(
     VLogsOptions.builder()
     .apiKey(apiKey)
     .appId(appId)
     .build()
 )
 
-async def main():
-    response = await sdk.collect(
-        Collector.builder()
-        .type(CollectorType.Error)
-        .source(CollectorSource.Other)
-        .message("This is a test message")
-        .build()
-    )
-
-    print("Response: ", response)
+response = await sdk.collect(
+    Collector.builder()
+    .type(CollectorType.Error)
+    .source(CollectorSource.Other)
+    .message("This is a test message")
+    .build()
+)
 
-# Run the async function
-asyncio.run(main())
+print("Response: ", response)
 ```
 
 ### Build, Install, and Test from Source
 
 ```shell
 make
 ```
```

