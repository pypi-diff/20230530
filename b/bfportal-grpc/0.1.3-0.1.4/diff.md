# Comparing `tmp/bfportal_grpc-0.1.3.tar.gz` & `tmp/bfportal_grpc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfportal_grpc-0.1.3.tar", max compression
+gzip compressed data, was "bfportal_grpc-0.1.4.tar", max compression
```

## Comparing `bfportal_grpc-0.1.3.tar` & `bfportal_grpc-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     5032 2022-09-25 13:38:31.387675 bfportal_grpc-0.1.3/Readme.md
--rw-r--r--   0        0        0      183 2022-09-25 13:00:34.707278 bfportal_grpc-0.1.3/bfportal_grpc/__init__.py
--rw-r--r--   0        0        0      892 2022-09-25 12:45:26.855873 bfportal_grpc-0.1.3/bfportal_grpc/access_token.py
--rw-r--r--   0        0        0        0 2022-09-25 13:32:08.322926 bfportal_grpc-0.1.3/bfportal_grpc/proto/__init__.py
--rw-r--r--   0        0        0     6673 2022-09-25 13:39:52.295033 bfportal_grpc-0.1.3/bfportal_grpc/proto/authentication_pb2.py
--rw-r--r--   0        0        0     4020 2022-09-25 13:40:19.774147 bfportal_grpc-0.1.3/bfportal_grpc/proto/authentication_pb2_grpc.py
--rw-r--r--   0        0        0    66061 2022-09-25 13:39:52.295033 bfportal_grpc-0.1.3/bfportal_grpc/proto/communitygames_pb2.py
--rw-r--r--   0        0        0    17777 2022-09-25 13:40:19.777480 bfportal_grpc-0.1.3/bfportal_grpc/proto/communitygames_pb2_grpc.py
--rw-r--r--   0        0        0     5901 2022-09-25 13:39:52.295033 bfportal_grpc-0.1.3/bfportal_grpc/proto/localization_pb2.py
--rw-r--r--   0        0        0     2634 2022-09-25 13:40:19.777480 bfportal_grpc-0.1.3/bfportal_grpc/proto/localization_pb2_grpc.py
--rw-r--r--   0        0        0     4105 2022-09-25 13:39:52.295033 bfportal_grpc-0.1.3/bfportal_grpc/proto/reporting_pb2.py
--rw-r--r--   0        0        0     2572 2022-09-25 13:40:19.780814 bfportal_grpc-0.1.3/bfportal_grpc/proto/reporting_pb2_grpc.py
--rw-r--r--   0        0        0     1271 2022-09-25 13:08:44.782338 bfportal_grpc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5958 1970-01-01 00:00:00.000000 bfportal_grpc-0.1.3/setup.py
--rw-r--r--   0        0        0     5831 1970-01-01 00:00:00.000000 bfportal_grpc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5980 2023-05-30 13:58:19.468939 bfportal_grpc-0.1.4/Readme.md
+-rw-r--r--   0        0        0      183 2023-01-20 10:31:40.808924 bfportal_grpc-0.1.4/bfportal_grpc/__init__.py
+-rw-r--r--   0        0        0      892 2023-01-20 10:31:40.809005 bfportal_grpc-0.1.4/bfportal_grpc/access_token.py
+-rw-r--r--   0        0        0        0 2023-01-20 10:31:40.809079 bfportal_grpc-0.1.4/bfportal_grpc/proto/__init__.py
+-rw-r--r--   0        0        0     3648 2023-05-30 15:23:31.382798 bfportal_grpc-0.1.4/bfportal_grpc/proto/authentication_pb2.py
+-rw-r--r--   0        0        0     4013 2023-05-30 15:23:31.383324 bfportal_grpc-0.1.4/bfportal_grpc/proto/authentication_pb2_grpc.py
+-rw-r--r--   0        0        0    29737 2023-05-30 15:23:31.383811 bfportal_grpc-0.1.4/bfportal_grpc/proto/communitygames_pb2.py
+-rw-r--r--   0        0        0    17770 2023-05-30 15:23:31.383872 bfportal_grpc-0.1.4/bfportal_grpc/proto/communitygames_pb2_grpc.py
+-rw-r--r--   0        0        0     2994 2023-05-30 15:23:31.384012 bfportal_grpc-0.1.4/bfportal_grpc/proto/localization_pb2.py
+-rw-r--r--   0        0        0     2627 2023-05-30 15:23:31.384280 bfportal_grpc-0.1.4/bfportal_grpc/proto/localization_pb2_grpc.py
+-rw-r--r--   0        0        0     2501 2023-05-30 15:23:31.384329 bfportal_grpc-0.1.4/bfportal_grpc/proto/reporting_pb2.py
+-rw-r--r--   0        0        0     2565 2023-05-30 15:23:31.384465 bfportal_grpc-0.1.4/bfportal_grpc/proto/reporting_pb2_grpc.py
+-rw-r--r--   0        0        0     1271 2023-05-30 15:21:57.403485 bfportal_grpc-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6782 1970-01-01 00:00:00.000000 bfportal_grpc-0.1.4/PKG-INFO
```

### Comparing `bfportal_grpc-0.1.3/Readme.md` & `bfportal_grpc-0.1.4/Readme.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,120 +1,175 @@
 # Battlefield Portal web-grpc
 
-This npm package can be used to directly call the https://portal.battlefield.com/ api.
+This npm and python package can be used to directly call the https://portal.battlefield.com/ api.
 we're making this public since you can read the javascript of the website and figure this out yourself easily anyway, but we want to make sure only 1 github repo has to be kept in sync with the api and the rest that uses it just has to update a package and a few code changes to still have it work.
 
 https://www.npmjs.com/package/bfportal-grpc
 
+https://pypi.org/project/bfportal-grpc/
+
 ## example
 
 ```js
-import { CommunityGamesClient, communitygames } from 'bfportal-grpc';
+import { CommunityGamesClient, communitygames } from 'bfportal-grpc'
 
-const communityGames = new CommunityGamesClient('https://kingston-prod-wgw-envoy.ops.dice.se', null);
+const communityGames = new CommunityGamesClient(
+  'https://kingston-prod-wgw-envoy.ops.dice.se',
+  null
+)
 const metadata = {
-    'x-dice-tenancy': 'prod_default-prod_default-kingston-common',
-    'x-gateway-session-id': sessionId,
-    'x-grpc-web': '1',
-    'x-user-agent': 'grpc-web-javascript/0.1',
+  'x-dice-tenancy': 'prod_default-prod_default-kingston-common',
+  'x-gateway-session-id': sessionId,
+  'x-grpc-web': '1',
+  'x-user-agent': 'grpc-web-javascript/0.1',
 }
 
-const request = new communitygames.GetPlaygroundRequest();
-request.setPlaygroundid(testPlayground);
-const response = await communityGames.getPlayground(request, metadata);
-const modRules = response.getPlayground()?.getOriginalplayground()?.getModrules()?.getCompatiblerules()?.getRules();
+const request = new communitygames.GetPlaygroundRequest()
+request.setPlaygroundid(testPlayground)
+const response = await communityGames.getPlayground(request, metadata)
+const modRules = response
+  .getPlayground()
+  ?.getOriginalplayground()
+  ?.getModrules()
+  ?.getCompatiblerules()
+  ?.getRules()
 if (modRules instanceof Uint8Array) {
-    console.log(new TextDecoder().decode(modRules))
+  console.log(new TextDecoder().decode(modRules))
 }
-const playgroundName = response.getPlayground()?.getOriginalplayground()?.getName();
+const playgroundName = response
+  .getPlayground()
+  ?.getOriginalplayground()
+  ?.getName()
 ```
 
 the proto files are accessable directly via "node_modules/bfportal-grpc/proto/communitygames.proto" to for example decode to json:
+
 ```js
+import { load } from 'protobufjs'
+
 // use reponse from previous example
-const root = await load("node_modules/bfportal-grpc/proto/communitygames.proto");
-const AwesomeMessage = root.lookupType("web.communitygames.PlaygroundInfoResponse");
-const decoded = AwesomeMessage.decode(response.serializeBinary());
-const json_str = JSON.stringify(decoded, null, 4);
+const root = await load('node_modules/bfportal-grpc/proto/communitygames.proto')
+const AwesomeMessage = root.lookupType(
+  'web.communitygames.PlaygroundInfoResponse'
+)
+const decoded = AwesomeMessage.decode(response.serializeBinary())
+const json_str = JSON.stringify(decoded, null, 4)
 ```
 
 ### non-async example
 
 ```js
-import { CommunityGamesClient, communitygames } from 'bfportal-grpc';
+import { CommunityGamesClient, communitygames } from 'bfportal-grpc'
 
-const communityGames = new CommunityGamesClient('https://kingston-prod-wgw-envoy.ops.dice.se', null);
+const communityGames = new CommunityGamesClient(
+  'https://kingston-prod-wgw-envoy.ops.dice.se',
+  null
+)
 const metadata = {
-    'x-dice-tenancy': 'prod_default-prod_default-kingston-common',
-    'x-gateway-session-id': sessionId,
-    'x-grpc-web': '1',
-    'x-user-agent': 'grpc-web-javascript/0.1',
+  'x-dice-tenancy': 'prod_default-prod_default-kingston-common',
+  'x-gateway-session-id': sessionId,
+  'x-grpc-web': '1',
+  'x-user-agent': 'grpc-web-javascript/0.1',
 }
 
-const request = new communitygames.GetPlaygroundRequest();
-request.setPlaygroundid("bbe433c0-13fa-11ed-bc32-24a8c2c0764e");
-const call = communityGames.getPlayground(request, metadata,
+const request = new communitygames.GetPlaygroundRequest()
+request.setPlaygroundid('bbe433c0-13fa-11ed-bc32-24a8c2c0764e')
+const call = communityGames.getPlayground(
+  request,
+  metadata,
   (_err: grpcWeb.Error, response: communitygames.PlaygroundInfoResponse) => {
     // console.log("err:", _err)
-    var modRules = response.getPlayground()?.getOriginalplayground()?.getModrules()?.getCompatiblerules()?.getRules();
+    var modRules = response
+      .getPlayground()
+      ?.getOriginalplayground()
+      ?.getModrules()
+      ?.getCompatiblerules()
+      ?.getRules()
     if (modRules instanceof Uint8Array) {
-        console.log(new TextDecoder().decode(modRules))
+      console.log(new TextDecoder().decode(modRules))
     }
 
-    load("node_modules/bfportal-grpc/proto/communitygames.proto", function(err, root) {
-      if (err)
-        throw err;
-      if (root == undefined) 
-        return
-
-      const AwesomeMessage = root.lookupType("web.communitygames.PlaygroundInfoResponse");
-
-      let decoded = AwesomeMessage.decode(response.serializeBinary());
-      fs.writeFile("test.json", JSON.stringify(decoded, null, 4), function(err: any) {
-        if (err) {
-            console.log(err);
-        }
-      });
-    })
-});
+    load(
+      'node_modules/bfportal-grpc/proto/communitygames.proto',
+      function (err, root) {
+        if (err) throw err
+        if (root == undefined) return
+
+        const AwesomeMessage = root.lookupType(
+          'web.communitygames.PlaygroundInfoResponse'
+        )
+
+        let decoded = AwesomeMessage.decode(response.serializeBinary())
+        fs.writeFile(
+          'test.json',
+          JSON.stringify(decoded, null, 4),
+          function (err: any) {
+            if (err) {
+              console.log(err)
+            }
+          }
+        )
+      }
+    )
+  }
+)
 ```
 
 ## python
+
 for python you can use the 'sonora' package to do grpc-web
+
 ```py
+import asyncio
 import sonora.aio
-import sys
-from proto import communitygames_pb2, communitygames_pb2_grpc
+from bfportal_grpc import communitygames_pb2, communitygames_pb2_grpc, access_token, authentication_pb2, authentication_pb2_grpc
 
 async def main():
+    cookie = access_token.Cookie(sid="", remid="")
+    token = await access_token.getBf2042GatewaySession(cookie)
+
     async with sonora.aio.insecure_web_channel(
         f"https://kingston-prod-wgw-envoy.ops.dice.se"
     ) as channel:
+        stub = authentication_pb2_grpc.AuthenticationStub(channel)
+        auth_response: authentication_pb2.AuthResponse = await stub.viaAuthCode(authentication_pb2.AuthRequest(platform=1, authCode=token, redirectUri='https://portal.battlefield.com/'), metadata=(
+            ('x-dice-tenancy', 'prod_default-prod_default-kingston-common'),
+            ('x-grpc-web', '1'),
+            ('x-user-agent', 'grpc-web-javascript/0.1')
+        ))
+
         stub = communitygames_pb2_grpc.CommunityGamesStub(channel)
         response: communitygames_pb2.PlaygroundInfoResponse = await stub.getPlayground(communitygames_pb2.GetPlaygroundRequest(playgroundId="10992a10-461a-11ec-8de0-d9f491f92236"), metadata=(
             ('x-dice-tenancy', 'prod_default-prod_default-kingston-common'),
-            ('x-gateway-session-id', 'web-c6b312c9-2520-4fde-958d-60ae71840a65'),
+            ('x-gateway-session-id', auth_response.sessionId),
             ('x-grpc-web', '1'),
             ('x-user-agent', 'grpc-web-javascript/0.1')
         ))
+
+        print(response.playground.originalPlayground.name)
+
+if __name__ == "__main__":
+    asyncio.run(main())
 ```
 
 ### current build method from proto to javascript via python
+
 needs proto-compile, which can be installed with:
 `pip3 install proto-compile`
 
 and build with:
 `proto-compile --clear-output-dirs --verbosity=1 ./proto ./src/proto grpc-web --grpc_web_out_options="import_style=typescript,mode=grpcweb"`
 
 building for python requires grpcio-tools, which can be installed with:
 `pip3 install grpcio-tools`
 
 and build with:
-`python3 -m grpc_tools.protoc -I. --python_out=./grpc-python --grpc_python_out=./grpc-python ./proto/communitygames.proto ./proto/localization.proto ./proto/authentication.proto ./proto/reporting.proto`
+`python3 -m grpc_tools.protoc -I. --python_out=./bfportal_grpc --grpc_python_out=./bfportal_grpc ./proto/communitygames.proto ./proto/localization.proto ./proto/authentication.proto ./proto/reporting.proto`
 
 python package used: https://github.com/romnn/proto-compile
 
 ### Pushing your changes
+
 package versions can be made with `npm run build` and `npm version patch` `git push --tags origin main` to release.
 for python patch with `npm run build:python`, `npm run python:setimports` and `poetry build`.
 
 example library used: https://github.com/tomchen/example-typescript-package
```

### Comparing `bfportal_grpc-0.1.3/bfportal_grpc/access_token.py` & `bfportal_grpc-0.1.4/bfportal_grpc/access_token.py`

 * *Files identical despite different names*

### Comparing `bfportal_grpc-0.1.3/bfportal_grpc/proto/authentication_pb2_grpc.py` & `bfportal_grpc-0.1.4/bfportal_grpc/proto/authentication_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import authentication_pb2 as authentication__pb2
+import authentication_pb2 as authentication__pb2
 
 
 class AuthenticationStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `bfportal_grpc-0.1.3/bfportal_grpc/proto/communitygames_pb2_grpc.py` & `bfportal_grpc-0.1.4/bfportal_grpc/proto/communitygames_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import communitygames_pb2 as communitygames__pb2
+import communitygames_pb2 as communitygames__pb2
 
 
 class CommunityGamesStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `bfportal_grpc-0.1.3/bfportal_grpc/proto/localization_pb2_grpc.py` & `bfportal_grpc-0.1.4/bfportal_grpc/proto/localization_pb2_grpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import localization_pb2 as localization__pb2
+import localization_pb2 as localization__pb2
 
 
 class ClientLocalizationStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `bfportal_grpc-0.1.3/bfportal_grpc/proto/reporting_pb2.py` & `bfportal_grpc-0.1.4/bfportal_grpc/proto/reporting_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: reporting.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0freporting.proto\x12\rweb.reporting\"\x1c\n\x0bStringValue\x12\r\n\x05value\x18\x01 \x01(\t\"\xd4\x01\n\x17ReportPlaygroundRequest\x12\x17\n\x0fprotocolVersion\x18\x01 \x01(\t\x12\x14\n\x0cplaygroundId\x18\x02 \x01(\t\x12)\n\x08\x63\x61tegory\x18\x03 \x01(\x0e\x32\x17.web.reporting.Category\x12\x32\n\x0erequesterEmail\x18\x04 \x01(\x0b\x32\x1a.web.reporting.StringValue\x12+\n\x07subject\x18\x05 \x01(\x0b\x32\x1a.web.reporting.StringValue\".\n\x18ReportPlaygroundResponse\x12\x12\n\npetitionId\x18\x01 \x01(\t*\xc7\x02\n\x08\x43\x61tegory\x12\x14\n\x10UNKNOWN_CATEGORY\x10\x00\x12\x0c\n\x08\x43HEATING\x10\x01\x12\x0e\n\nHARASSMENT\x10\x02\x12\x08\n\x04SPAM\x10\x03\x12\x0e\n\nPLAGIARISM\x10\x04\x12\x0f\n\x0bHATE_SPEECH\x10\x05\x12\x15\n\x11SEXUALLY_EXPLICIT\x10\x06\x12\x16\n\x12\x43HILD_SOLICITATION\x10\x07\x12\x14\n\x10TERRORIST_THREAT\x10\x08\x12\x0f\n\x0b\x43LIENT_HACK\x10\t\x12\x12\n\x0eSUICIDE_THREAT\x10\n\x12\n\n\x06\x44OXING\x10\x0b\x12\x0f\n\x0b\x41\x44VERTISING\x10\x0c\x12\x11\n\rINAPPROPRIATE\x10\r\x12\x0b\n\x07VIOLENT\x10\x0e\x12\r\n\tOFFENSIVE\x10\x0f\x12\x12\n\x0eOFFENSIVE_CHAT\x10\x10\x12\x12\n\x0eOFFENSIVE_NAME\x10\x11\x32u\n\x0cWebReporting\x12\x65\n\x10reportPlayground\x12&.web.reporting.ReportPlaygroundRequest\x1a\'.web.reporting.ReportPlaygroundResponse\"\x00\x62\x06proto3')
 
-_CATEGORY = DESCRIPTOR.enum_types_by_name['Category']
-Category = enum_type_wrapper.EnumTypeWrapper(_CATEGORY)
-UNKNOWN_CATEGORY = 0
-CHEATING = 1
-HARASSMENT = 2
-SPAM = 3
-PLAGIARISM = 4
-HATE_SPEECH = 5
-SEXUALLY_EXPLICIT = 6
-CHILD_SOLICITATION = 7
-TERRORIST_THREAT = 8
-CLIENT_HACK = 9
-SUICIDE_THREAT = 10
-DOXING = 11
-ADVERTISING = 12
-INAPPROPRIATE = 13
-VIOLENT = 14
-OFFENSIVE = 15
-OFFENSIVE_CHAT = 16
-OFFENSIVE_NAME = 17
-
-
-_STRINGVALUE = DESCRIPTOR.message_types_by_name['StringValue']
-_REPORTPLAYGROUNDREQUEST = DESCRIPTOR.message_types_by_name['ReportPlaygroundRequest']
-_REPORTPLAYGROUNDRESPONSE = DESCRIPTOR.message_types_by_name['ReportPlaygroundResponse']
-StringValue = _reflection.GeneratedProtocolMessageType('StringValue', (_message.Message,), {
-  'DESCRIPTOR' : _STRINGVALUE,
-  '__module__' : 'reporting_pb2'
-  # @@protoc_insertion_point(class_scope:web.reporting.StringValue)
-  })
-_sym_db.RegisterMessage(StringValue)
-
-ReportPlaygroundRequest = _reflection.GeneratedProtocolMessageType('ReportPlaygroundRequest', (_message.Message,), {
-  'DESCRIPTOR' : _REPORTPLAYGROUNDREQUEST,
-  '__module__' : 'reporting_pb2'
-  # @@protoc_insertion_point(class_scope:web.reporting.ReportPlaygroundRequest)
-  })
-_sym_db.RegisterMessage(ReportPlaygroundRequest)
-
-ReportPlaygroundResponse = _reflection.GeneratedProtocolMessageType('ReportPlaygroundResponse', (_message.Message,), {
-  'DESCRIPTOR' : _REPORTPLAYGROUNDRESPONSE,
-  '__module__' : 'reporting_pb2'
-  # @@protoc_insertion_point(class_scope:web.reporting.ReportPlaygroundResponse)
-  })
-_sym_db.RegisterMessage(ReportPlaygroundResponse)
-
-_WEBREPORTING = DESCRIPTOR.services_by_name['WebReporting']
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'reporting_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _CATEGORY._serialized_start=328
   _CATEGORY._serialized_end=655
   _STRINGVALUE._serialized_start=34
   _STRINGVALUE._serialized_end=62
```

### Comparing `bfportal_grpc-0.1.3/bfportal_grpc/proto/reporting_pb2_grpc.py` & `bfportal_grpc-0.1.4/bfportal_grpc/proto/reporting_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import reporting_pb2 as reporting__pb2
+import reporting_pb2 as reporting__pb2
 
 
 class WebReportingStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `bfportal_grpc-0.1.3/pyproject.toml` & `bfportal_grpc-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "bfportal_grpc"
-version = "0.1.3"
+version = "0.1.4"
 description = " bf2042 portal web grpc as python package "
 readme = "Readme.md"
 authors = ["iiTzArcur <arcur@gametools.network>"]
 # license = { file = "LICENSE" }
 classifiers = [
     # "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `bfportal_grpc-0.1.3/setup.py` & `bfportal_grpc-0.1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,196 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: bfportal-grpc
+Version: 0.1.4
+Summary:  bf2042 portal web grpc as python package 
+Home-page: https://github.com/community-network/bfportal-grpc
+Keywords: bfportal,grpc,Battlefield portal
+Author: iiTzArcur
+Author-email: arcur@gametools.network
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: grpcio (==1.48.1)
+Requires-Dist: protobuf (==4.21.6)
+Project-URL: Bug Tracker, https://github.com/community-network/bfportal-grpc/issues
+Project-URL: Repository, https://github.com/community-network/bfportal-grpc
+Description-Content-Type: text/markdown
+
+# Battlefield Portal web-grpc
+
+This npm and python package can be used to directly call the https://portal.battlefield.com/ api.
+we're making this public since you can read the javascript of the website and figure this out yourself easily anyway, but we want to make sure only 1 github repo has to be kept in sync with the api and the rest that uses it just has to update a package and a few code changes to still have it work.
+
+https://www.npmjs.com/package/bfportal-grpc
+
+https://pypi.org/project/bfportal-grpc/
+
+## example
+
+```js
+import { CommunityGamesClient, communitygames } from 'bfportal-grpc'
+
+const communityGames = new CommunityGamesClient(
+  'https://kingston-prod-wgw-envoy.ops.dice.se',
+  null
+)
+const metadata = {
+  'x-dice-tenancy': 'prod_default-prod_default-kingston-common',
+  'x-gateway-session-id': sessionId,
+  'x-grpc-web': '1',
+  'x-user-agent': 'grpc-web-javascript/0.1',
+}
+
+const request = new communitygames.GetPlaygroundRequest()
+request.setPlaygroundid(testPlayground)
+const response = await communityGames.getPlayground(request, metadata)
+const modRules = response
+  .getPlayground()
+  ?.getOriginalplayground()
+  ?.getModrules()
+  ?.getCompatiblerules()
+  ?.getRules()
+if (modRules instanceof Uint8Array) {
+  console.log(new TextDecoder().decode(modRules))
+}
+const playgroundName = response
+  .getPlayground()
+  ?.getOriginalplayground()
+  ?.getName()
+```
+
+the proto files are accessable directly via "node_modules/bfportal-grpc/proto/communitygames.proto" to for example decode to json:
+
+```js
+import { load } from 'protobufjs'
+
+// use reponse from previous example
+const root = await load('node_modules/bfportal-grpc/proto/communitygames.proto')
+const AwesomeMessage = root.lookupType(
+  'web.communitygames.PlaygroundInfoResponse'
+)
+const decoded = AwesomeMessage.decode(response.serializeBinary())
+const json_str = JSON.stringify(decoded, null, 4)
+```
+
+### non-async example
+
+```js
+import { CommunityGamesClient, communitygames } from 'bfportal-grpc'
+
+const communityGames = new CommunityGamesClient(
+  'https://kingston-prod-wgw-envoy.ops.dice.se',
+  null
+)
+const metadata = {
+  'x-dice-tenancy': 'prod_default-prod_default-kingston-common',
+  'x-gateway-session-id': sessionId,
+  'x-grpc-web': '1',
+  'x-user-agent': 'grpc-web-javascript/0.1',
+}
 
-packages = \
-['bfportal_grpc', 'bfportal_grpc.proto']
+const request = new communitygames.GetPlaygroundRequest()
+request.setPlaygroundid('bbe433c0-13fa-11ed-bc32-24a8c2c0764e')
+const call = communityGames.getPlayground(
+  request,
+  metadata,
+  (_err: grpcWeb.Error, response: communitygames.PlaygroundInfoResponse) => {
+    // console.log("err:", _err)
+    var modRules = response
+      .getPlayground()
+      ?.getOriginalplayground()
+      ?.getModrules()
+      ?.getCompatiblerules()
+      ?.getRules()
+    if (modRules instanceof Uint8Array) {
+      console.log(new TextDecoder().decode(modRules))
+    }
+
+    load(
+      'node_modules/bfportal-grpc/proto/communitygames.proto',
+      function (err, root) {
+        if (err) throw err
+        if (root == undefined) return
+
+        const AwesomeMessage = root.lookupType(
+          'web.communitygames.PlaygroundInfoResponse'
+        )
+
+        let decoded = AwesomeMessage.decode(response.serializeBinary())
+        fs.writeFile(
+          'test.json',
+          JSON.stringify(decoded, null, 4),
+          function (err: any) {
+            if (err) {
+              console.log(err)
+            }
+          }
+        )
+      }
+    )
+  }
+)
+```
+
+## python
+
+for python you can use the 'sonora' package to do grpc-web
+
+```py
+import asyncio
+import sonora.aio
+from bfportal_grpc import communitygames_pb2, communitygames_pb2_grpc, access_token, authentication_pb2, authentication_pb2_grpc
+
+async def main():
+    cookie = access_token.Cookie(sid="", remid="")
+    token = await access_token.getBf2042GatewaySession(cookie)
+
+    async with sonora.aio.insecure_web_channel(
+        f"https://kingston-prod-wgw-envoy.ops.dice.se"
+    ) as channel:
+        stub = authentication_pb2_grpc.AuthenticationStub(channel)
+        auth_response: authentication_pb2.AuthResponse = await stub.viaAuthCode(authentication_pb2.AuthRequest(platform=1, authCode=token, redirectUri='https://portal.battlefield.com/'), metadata=(
+            ('x-dice-tenancy', 'prod_default-prod_default-kingston-common'),
+            ('x-grpc-web', '1'),
+            ('x-user-agent', 'grpc-web-javascript/0.1')
+        ))
+
+        stub = communitygames_pb2_grpc.CommunityGamesStub(channel)
+        response: communitygames_pb2.PlaygroundInfoResponse = await stub.getPlayground(communitygames_pb2.GetPlaygroundRequest(playgroundId="10992a10-461a-11ec-8de0-d9f491f92236"), metadata=(
+            ('x-dice-tenancy', 'prod_default-prod_default-kingston-common'),
+            ('x-gateway-session-id', auth_response.sessionId),
+            ('x-grpc-web', '1'),
+            ('x-user-agent', 'grpc-web-javascript/0.1')
+        ))
+
+        print(response.playground.originalPlayground.name)
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+### current build method from proto to javascript via python
+
+needs proto-compile, which can be installed with:
+`pip3 install proto-compile`
+
+and build with:
+`proto-compile --clear-output-dirs --verbosity=1 ./proto ./src/proto grpc-web --grpc_web_out_options="import_style=typescript,mode=grpcweb"`
+
+building for python requires grpcio-tools, which can be installed with:
+`pip3 install grpcio-tools`
+
+and build with:
+`python3 -m grpc_tools.protoc -I. --python_out=./bfportal_grpc --grpc_python_out=./bfportal_grpc ./proto/communitygames.proto ./proto/localization.proto ./proto/authentication.proto ./proto/reporting.proto`
 
-package_data = \
-{'': ['*']}
+python package used: https://github.com/romnn/proto-compile
 
-install_requires = \
-['aiohttp>=3.8.1,<4.0.0', 'grpcio==1.48.1', 'protobuf==4.21.6']
-
-setup_kwargs = {
-    'name': 'bfportal-grpc',
-    'version': '0.1.3',
-    'description': ' bf2042 portal web grpc as python package ',
-    'long_description': '# Battlefield Portal web-grpc\n\nThis npm package can be used to directly call the https://portal.battlefield.com/ api.\nwe\'re making this public since you can read the javascript of the website and figure this out yourself easily anyway, but we want to make sure only 1 github repo has to be kept in sync with the api and the rest that uses it just has to update a package and a few code changes to still have it work.\n\nhttps://www.npmjs.com/package/bfportal-grpc\n\n## example\n\n```js\nimport { CommunityGamesClient, communitygames } from \'bfportal-grpc\';\n\nconst communityGames = new CommunityGamesClient(\'https://kingston-prod-wgw-envoy.ops.dice.se\', null);\nconst metadata = {\n    \'x-dice-tenancy\': \'prod_default-prod_default-kingston-common\',\n    \'x-gateway-session-id\': sessionId,\n    \'x-grpc-web\': \'1\',\n    \'x-user-agent\': \'grpc-web-javascript/0.1\',\n}\n\nconst request = new communitygames.GetPlaygroundRequest();\nrequest.setPlaygroundid(testPlayground);\nconst response = await communityGames.getPlayground(request, metadata);\nconst modRules = response.getPlayground()?.getOriginalplayground()?.getModrules()?.getCompatiblerules()?.getRules();\nif (modRules instanceof Uint8Array) {\n    console.log(new TextDecoder().decode(modRules))\n}\nconst playgroundName = response.getPlayground()?.getOriginalplayground()?.getName();\n```\n\nthe proto files are accessable directly via "node_modules/bfportal-grpc/proto/communitygames.proto" to for example decode to json:\n```js\n// use reponse from previous example\nconst root = await load("node_modules/bfportal-grpc/proto/communitygames.proto");\nconst AwesomeMessage = root.lookupType("web.communitygames.PlaygroundInfoResponse");\nconst decoded = AwesomeMessage.decode(response.serializeBinary());\nconst json_str = JSON.stringify(decoded, null, 4);\n```\n\n### non-async example\n\n```js\nimport { CommunityGamesClient, communitygames } from \'bfportal-grpc\';\n\nconst communityGames = new CommunityGamesClient(\'https://kingston-prod-wgw-envoy.ops.dice.se\', null);\nconst metadata = {\n    \'x-dice-tenancy\': \'prod_default-prod_default-kingston-common\',\n    \'x-gateway-session-id\': sessionId,\n    \'x-grpc-web\': \'1\',\n    \'x-user-agent\': \'grpc-web-javascript/0.1\',\n}\n\nconst request = new communitygames.GetPlaygroundRequest();\nrequest.setPlaygroundid("bbe433c0-13fa-11ed-bc32-24a8c2c0764e");\nconst call = communityGames.getPlayground(request, metadata,\n  (_err: grpcWeb.Error, response: communitygames.PlaygroundInfoResponse) => {\n    // console.log("err:", _err)\n    var modRules = response.getPlayground()?.getOriginalplayground()?.getModrules()?.getCompatiblerules()?.getRules();\n    if (modRules instanceof Uint8Array) {\n        console.log(new TextDecoder().decode(modRules))\n    }\n\n    load("node_modules/bfportal-grpc/proto/communitygames.proto", function(err, root) {\n      if (err)\n        throw err;\n      if (root == undefined) \n        return\n\n      const AwesomeMessage = root.lookupType("web.communitygames.PlaygroundInfoResponse");\n\n      let decoded = AwesomeMessage.decode(response.serializeBinary());\n      fs.writeFile("test.json", JSON.stringify(decoded, null, 4), function(err: any) {\n        if (err) {\n            console.log(err);\n        }\n      });\n    })\n});\n```\n\n## python\nfor python you can use the \'sonora\' package to do grpc-web\n```py\nimport sonora.aio\nimport sys\nfrom proto import communitygames_pb2, communitygames_pb2_grpc\n\nasync def main():\n    async with sonora.aio.insecure_web_channel(\n        f"https://kingston-prod-wgw-envoy.ops.dice.se"\n    ) as channel:\n        stub = communitygames_pb2_grpc.CommunityGamesStub(channel)\n        response: communitygames_pb2.PlaygroundInfoResponse = await stub.getPlayground(communitygames_pb2.GetPlaygroundRequest(playgroundId="10992a10-461a-11ec-8de0-d9f491f92236"), metadata=(\n            (\'x-dice-tenancy\', \'prod_default-prod_default-kingston-common\'),\n            (\'x-gateway-session-id\', \'web-c6b312c9-2520-4fde-958d-60ae71840a65\'),\n            (\'x-grpc-web\', \'1\'),\n            (\'x-user-agent\', \'grpc-web-javascript/0.1\')\n        ))\n```\n\n### current build method from proto to javascript via python\nneeds proto-compile, which can be installed with:\n`pip3 install proto-compile`\n\nand build with:\n`proto-compile --clear-output-dirs --verbosity=1 ./proto ./src/proto grpc-web --grpc_web_out_options="import_style=typescript,mode=grpcweb"`\n\nbuilding for python requires grpcio-tools, which can be installed with:\n`pip3 install grpcio-tools`\n\nand build with:\n`python3 -m grpc_tools.protoc -I. --python_out=./grpc-python --grpc_python_out=./grpc-python ./proto/communitygames.proto ./proto/localization.proto ./proto/authentication.proto ./proto/reporting.proto`\n\npython package used: https://github.com/romnn/proto-compile\n\n### Pushing your changes\npackage versions can be made with `npm run build` and `npm version patch` `git push --tags origin main` to release.\nfor python patch with `npm run build:python`, `npm run python:setimports` and `poetry build`.\n\nexample library used: https://github.com/tomchen/example-typescript-package\n',
-    'author': 'iiTzArcur',
-    'author_email': 'arcur@gametools.network',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/community-network/bfportal-grpc',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+### Pushing your changes
+
+package versions can be made with `npm run build` and `npm version patch` `git push --tags origin main` to release.
+for python patch with `npm run build:python`, `npm run python:setimports` and `poetry build`.
 
+example library used: https://github.com/tomchen/example-typescript-package
 
-setup(**setup_kwargs)
```

