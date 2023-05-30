# Comparing `tmp/inpost-0.1.0.tar.gz` & `tmp/inpost-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inpost-0.1.0.tar", max compression
+gzip compressed data, was "inpost-0.1.1.tar", max compression
```

## Comparing `inpost-0.1.0.tar` & `inpost-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      646 2023-04-25 09:56:56.661671 inpost-0.1.0/README.md
--rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.1.0/inpost/__init__.py
--rw-r--r--   0        0        0    45360 2023-05-16 17:51:57.264181 inpost-0.1.0/inpost/api.py
--rw-r--r--   0        0        0     1173 2023-05-08 21:18:45.284128 inpost-0.1.0/inpost/static/__init__.py
--rw-r--r--   0        0        0     1663 2023-02-09 11:19:43.627615 inpost-0.1.0/inpost/static/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2644 2023-05-16 17:58:27.019865 inpost-0.1.0/inpost/static/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1736 2023-02-09 11:19:43.714281 inpost-0.1.0/inpost/static/__pycache__/endpoints.cpython-310.pyc
--rw-r--r--   0        0        0     7733 2023-05-16 17:58:27.079865 inpost-0.1.0/inpost/static/__pycache__/endpoints.cpython-311.pyc
--rw-r--r--   0        0        0     3753 2023-02-09 11:19:43.710948 inpost-0.1.0/inpost/static/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     5421 2023-05-16 17:58:27.079865 inpost-0.1.0/inpost/static/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     1056 2023-02-09 11:24:57.470311 inpost-0.1.0/inpost/static/__pycache__/friends.cpython-310.pyc
--rw-r--r--   0        0        0     3107 2023-05-16 17:58:27.083199 inpost-0.1.0/inpost/static/__pycache__/friends.cpython-311.pyc
--rw-r--r--   0        0        0      202 2023-01-11 16:11:34.275165 inpost-0.1.0/inpost/static/__pycache__/headers.cpython-310.pyc
--rw-r--r--   0        0        0      223 2023-05-16 17:58:27.076532 inpost-0.1.0/inpost/static/__pycache__/headers.cpython-311.pyc
--rw-r--r--   0        0        0     1243 2023-05-16 17:58:27.086532 inpost-0.1.0/inpost/static/__pycache__/notifications.cpython-311.pyc
--rw-r--r--   0        0        0    22657 2023-02-09 11:19:43.637615 inpost-0.1.0/inpost/static/__pycache__/parcels.cpython-310.pyc
--rw-r--r--   0        0        0    44251 2023-05-16 17:58:27.049865 inpost-0.1.0/inpost/static/__pycache__/parcels.cpython-311.pyc
--rw-r--r--   0        0        0     7954 2023-01-19 11:34:51.801975 inpost-0.1.0/inpost/static/__pycache__/statuses.cpython-310.pyc
--rw-r--r--   0        0        0    12027 2023-05-16 18:02:18.314615 inpost-0.1.0/inpost/static/__pycache__/statuses.cpython-311.pyc
--rw-r--r--   0        0        0     1958 2023-05-17 18:25:42.850624 inpost-0.1.0/inpost/static/endpoints.py
--rw-r--r--   0        0        0     2515 2023-02-09 09:51:30.001451 inpost-0.1.0/inpost/static/exceptions.py
--rw-r--r--   0        0        0     1779 2023-02-09 12:35:10.844655 inpost-0.1.0/inpost/static/friends.py
--rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.1.0/inpost/static/headers.py
--rw-r--r--   0        0        0      670 2023-05-08 21:18:45.284128 inpost-0.1.0/inpost/static/notifications.py
--rw-r--r--   0        0        0    27776 2023-05-16 17:55:27.607968 inpost-0.1.0/inpost/static/parcels.py
--rw-r--r--   0        0        0     7066 2023-05-16 18:03:15.934872 inpost-0.1.0/inpost/static/statuses.py
--rw-r--r--   0        0        0     1072 2023-05-17 18:26:22.780859 inpost-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 inpost-0.1.0/setup.py
--rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 inpost-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      646 2023-04-25 09:56:56.661671 inpost-0.1.1/README.md
+-rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.1.1/inpost/__init__.py
+-rw-r--r--   0        0        0    45431 2023-05-30 14:37:20.919384 inpost-0.1.1/inpost/api.py
+-rw-r--r--   0        0        0     1173 2023-05-08 21:18:45.284128 inpost-0.1.1/inpost/static/__init__.py
+-rw-r--r--   0        0        0     1663 2023-02-09 11:19:43.627615 inpost-0.1.1/inpost/static/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2644 2023-05-16 17:58:27.019865 inpost-0.1.1/inpost/static/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1736 2023-02-09 11:19:43.714281 inpost-0.1.1/inpost/static/__pycache__/endpoints.cpython-310.pyc
+-rw-r--r--   0        0        0     2541 2023-05-30 13:20:30.662182 inpost-0.1.1/inpost/static/__pycache__/endpoints.cpython-311.pyc
+-rw-r--r--   0        0        0     3753 2023-02-09 11:19:43.710948 inpost-0.1.1/inpost/static/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     5421 2023-05-16 17:58:27.079865 inpost-0.1.1/inpost/static/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     1056 2023-02-09 11:24:57.470311 inpost-0.1.1/inpost/static/__pycache__/friends.cpython-310.pyc
+-rw-r--r--   0        0        0     3107 2023-05-16 17:58:27.083199 inpost-0.1.1/inpost/static/__pycache__/friends.cpython-311.pyc
+-rw-r--r--   0        0        0      202 2023-01-11 16:11:34.275165 inpost-0.1.1/inpost/static/__pycache__/headers.cpython-310.pyc
+-rw-r--r--   0        0        0      223 2023-05-16 17:58:27.076532 inpost-0.1.1/inpost/static/__pycache__/headers.cpython-311.pyc
+-rw-r--r--   0        0        0     1243 2023-05-16 17:58:27.086532 inpost-0.1.1/inpost/static/__pycache__/notifications.cpython-311.pyc
+-rw-r--r--   0        0        0    22657 2023-02-09 11:19:43.637615 inpost-0.1.1/inpost/static/__pycache__/parcels.cpython-310.pyc
+-rw-r--r--   0        0        0    44670 2023-05-30 14:13:11.007453 inpost-0.1.1/inpost/static/__pycache__/parcels.cpython-311.pyc
+-rw-r--r--   0        0        0     7954 2023-01-19 11:34:51.801975 inpost-0.1.1/inpost/static/__pycache__/statuses.cpython-310.pyc
+-rw-r--r--   0        0        0    11366 2023-05-30 13:20:30.648849 inpost-0.1.1/inpost/static/__pycache__/statuses.cpython-311.pyc
+-rw-r--r--   0        0        0     1958 2023-05-17 18:25:42.850624 inpost-0.1.1/inpost/static/endpoints.py
+-rw-r--r--   0        0        0     2515 2023-02-09 09:51:30.001451 inpost-0.1.1/inpost/static/exceptions.py
+-rw-r--r--   0        0        0     1779 2023-02-09 12:35:10.844655 inpost-0.1.1/inpost/static/friends.py
+-rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.1.1/inpost/static/headers.py
+-rw-r--r--   0        0        0      670 2023-05-08 21:18:45.284128 inpost-0.1.1/inpost/static/notifications.py
+-rw-r--r--   0        0        0    28065 2023-05-30 13:26:22.527921 inpost-0.1.1/inpost/static/parcels.py
+-rw-r--r--   0        0        0     7066 2023-05-16 18:03:15.934872 inpost-0.1.1/inpost/static/statuses.py
+-rw-r--r--   0        0        0     1072 2023-05-30 14:42:01.554547 inpost-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 inpost-0.1.1/setup.py
+-rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 inpost-0.1.1/PKG-INFO
```

### Comparing `inpost-0.1.0/README.md` & `inpost-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/api.py` & `inpost-0.1.1/inpost/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import logging
+from typing import List
+
 from aiohttp import ClientSession, ClientResponse
 from aiohttp.typedefs import StrOrURL
-from typing import List
-import logging
-from arrow import utcnow
+
 from inpost.static import *
 
 
 class Inpost:
     """Python representation of an Inpost app. Essentially implements methods to manage all incoming parcels"""
 
     def __init__(self):
@@ -73,14 +74,17 @@
                 {'Authorization': self.auth_token}
             )
 
         resp = await self.sess.request(method, url, headers=headers_, json=data, **kwargs)
 
         if autorefresh and resp.status == 401:
             await self.refresh_token()
+            headers_.update(
+                {'Authorization': self.auth_token}
+            )
             resp = await self.sess.request(method, url, headers=headers_, json=data, **kwargs)
 
         match resp.status:
             case 200:
                 self._log.debug(f'{action} done')
                 return resp
             case 401:
```

### Comparing `inpost-0.1.0/inpost/static/__init__.py` & `inpost-0.1.1/inpost/static/__init__.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/__pycache__/__init__.cpython-310.pyc` & `inpost-0.1.1/inpost/static/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/__pycache__/__init__.cpython-311.pyc` & `inpost-0.1.1/inpost/static/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/__pycache__/endpoints.cpython-310.pyc` & `inpost-0.1.1/inpost/static/__pycache__/endpoints.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/__pycache__/exceptions.cpython-310.pyc` & `inpost-0.1.1/inpost/static/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/__pycache__/exceptions.cpython-311.pyc` & `inpost-0.1.1/inpost/static/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/__pycache__/friends.cpython-310.pyc` & `inpost-0.1.1/inpost/static/__pycache__/friends.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/__pycache__/friends.cpython-311.pyc` & `inpost-0.1.1/inpost/static/__pycache__/friends.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/__pycache__/notifications.cpython-311.pyc` & `inpost-0.1.1/inpost/static/__pycache__/notifications.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/__pycache__/parcels.cpython-310.pyc` & `inpost-0.1.1/inpost/static/__pycache__/parcels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/__pycache__/parcels.cpython-311.pyc` & `inpost-0.1.1/inpost/static/__pycache__/parcels.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x8fc36364 (Tue May 16 17:55:27 2023 UTC)
-files sz: 27776
+moddate:  0x7ef97564 (Tue May 30 13:26:22 2023 UTC)
+files sz: 28065
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -85,117 +85,117 @@
                110 MAKE_FUNCTION            0
                112 LOAD_CONST               9 ('Parcel')
                114 LOAD_NAME               11 (BaseParcel)
                116 PRECALL                  3
                120 CALL                     3
                130 STORE_NAME              12 (Parcel)
    
-   246         132 PUSH_NULL
+   247         132 PUSH_NULL
                134 LOAD_BUILD_CLASS
-               136 LOAD_CONST              10 (<code object ReturnParcel, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 246>)
+               136 LOAD_CONST              10 (<code object ReturnParcel, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 247>)
                138 MAKE_FUNCTION            0
                140 LOAD_CONST              11 ('ReturnParcel')
                142 LOAD_NAME               11 (BaseParcel)
                144 PRECALL                  3
                148 CALL                     3
                158 STORE_NAME              13 (ReturnParcel)
    
-   261         160 PUSH_NULL
+   262         160 PUSH_NULL
                162 LOAD_BUILD_CLASS
-               164 LOAD_CONST              12 (<code object Receiver, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 261>)
+               164 LOAD_CONST              12 (<code object Receiver, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 262>)
                166 MAKE_FUNCTION            0
                168 LOAD_CONST              13 ('Receiver')
                170 PRECALL                  2
                174 CALL                     2
                184 STORE_NAME              14 (Receiver)
    
-   283         186 PUSH_NULL
+   284         186 PUSH_NULL
                188 LOAD_BUILD_CLASS
-               190 LOAD_CONST              14 (<code object Sender, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 283>)
+               190 LOAD_CONST              14 (<code object Sender, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 284>)
                192 MAKE_FUNCTION            0
                194 LOAD_CONST              15 ('Sender')
                196 PRECALL                  2
                200 CALL                     2
                210 STORE_NAME              15 (Sender)
    
-   306         212 PUSH_NULL
+   307         212 PUSH_NULL
                214 LOAD_BUILD_CLASS
-               216 LOAD_CONST              16 (<code object PickupPoint, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 306>)
+               216 LOAD_CONST              16 (<code object PickupPoint, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 307>)
                218 MAKE_FUNCTION            0
                220 LOAD_CONST              17 ('PickupPoint')
                222 PRECALL                  2
                226 CALL                     2
                236 STORE_NAME              16 (PickupPoint)
    
-   359         238 PUSH_NULL
+   360         238 PUSH_NULL
                240 LOAD_BUILD_CLASS
-               242 LOAD_CONST              18 (<code object MultiCompartment, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 359>)
+               242 LOAD_CONST              18 (<code object MultiCompartment, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 360>)
                244 MAKE_FUNCTION            0
                246 LOAD_CONST              19 ('MultiCompartment')
                248 PRECALL                  2
                252 CALL                     2
                262 STORE_NAME              17 (MultiCompartment)
    
-   383         264 PUSH_NULL
+   384         264 PUSH_NULL
                266 LOAD_BUILD_CLASS
-               268 LOAD_CONST              20 (<code object Operations, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 383>)
+               268 LOAD_CONST              20 (<code object Operations, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 384>)
                270 MAKE_FUNCTION            0
                272 LOAD_CONST              21 ('Operations')
                274 PRECALL                  2
                278 CALL                     2
                288 STORE_NAME              18 (Operations)
    
-   416         290 PUSH_NULL
+   417         290 PUSH_NULL
                292 LOAD_BUILD_CLASS
-               294 LOAD_CONST              22 (<code object EventLog, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 416>)
+               294 LOAD_CONST              22 (<code object EventLog, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 417>)
                296 MAKE_FUNCTION            0
                298 LOAD_CONST              23 ('EventLog')
                300 PRECALL                  2
                304 CALL                     2
                314 STORE_NAME              19 (EventLog)
    
-   442         316 PUSH_NULL
+   443         316 PUSH_NULL
                318 LOAD_BUILD_CLASS
-               320 LOAD_CONST              24 (<code object SharedTo, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 442>)
+               320 LOAD_CONST              24 (<code object SharedTo, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 443>)
                322 MAKE_FUNCTION            0
                324 LOAD_CONST              25 ('SharedTo')
                326 PRECALL                  2
                330 CALL                     2
                340 STORE_NAME              20 (SharedTo)
    
-   464         342 PUSH_NULL
+   465         342 PUSH_NULL
                344 LOAD_BUILD_CLASS
-               346 LOAD_CONST              26 (<code object QRCode, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 464>)
+               346 LOAD_CONST              26 (<code object QRCode, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 465>)
                348 MAKE_FUNCTION            0
                350 LOAD_CONST              27 ('QRCode')
                352 PRECALL                  2
                356 CALL                     2
                366 STORE_NAME              21 (QRCode)
    
-   509         368 PUSH_NULL
+   510         368 PUSH_NULL
                370 LOAD_BUILD_CLASS
-               372 LOAD_CONST              28 (<code object CompartmentLocation, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 509>)
+               372 LOAD_CONST              28 (<code object CompartmentLocation, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 510>)
                374 MAKE_FUNCTION            0
                376 LOAD_CONST              29 ('CompartmentLocation')
                378 PRECALL                  2
                382 CALL                     2
                392 STORE_NAME              22 (CompartmentLocation)
    
-   535         394 PUSH_NULL
+   536         394 PUSH_NULL
                396 LOAD_BUILD_CLASS
-               398 LOAD_CONST              30 (<code object CompartmentProperties, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 535>)
+               398 LOAD_CONST              30 (<code object CompartmentProperties, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 536>)
                400 MAKE_FUNCTION            0
                402 LOAD_CONST              31 ('CompartmentProperties')
                404 PRECALL                  2
                408 CALL                     2
                418 STORE_NAME              23 (CompartmentProperties)
    
-   603         420 PUSH_NULL
+   604         420 PUSH_NULL
                422 LOAD_BUILD_CLASS
-               424 LOAD_CONST              32 (<code object AirSensorData, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 603>)
+               424 LOAD_CONST              32 (<code object AirSensorData, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 604>)
                426 MAKE_FUNCTION            0
                428 LOAD_CONST              33 ('AirSensorData')
                430 PRECALL                  2
                434 CALL                     2
                444 STORE_NAME              24 (AirSensorData)
                446 LOAD_CONST               1 (None)
                448 RETURN_VALUE
@@ -243,103 +243,106 @@
             'logger'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
-                  0x9501870097007c0164011900000000000000000089005f000000000000
-                  0000007c02a001000000000000000000000000000000000000000089036a
-                  0200000000000000009b00640289006a0000000000000000009b009d03a6
-                  010000ab01000000000000000089005f0300000000000000007408000000
-                  000000000000007c01640319000000000000000000190000000000000000
-                  0089005f05000000000000000064047c0176007215740d00000000000000
-                  0000007c01640419000000000000000000a6010000ab0100000000000000
-                  006e01640089005f0700000000000000007411000000000000000000007c
-                  0164051900000000000000000089006a030000000000000000ac06a60200
-                  00ab02000000000000000089005f09000000000000000088006601640784
-                  087c016408190000000000000000004400a6000000ab0000000000000000
-                  0089005f0a000000000000000064005300
+                  0x9501870097007c01a00000000000000000000000000000000000000000
+                  006401a6010000ab01000000000000000089005f0100000000000000007c
+                  02a002000000000000000000000000000000000000000089036a03000000
+                  00000000009b00640289006a0100000000000000009b009d03a6010000ab
+                  01000000000000000089005f040000000000000000740a00000000000000
+                  0000007c016403190000000000000000001900000000000000000089005f
+                  06000000000000000064047c01760072157401000000000000000000007c
+                  01640419000000000000000000a6010000ab0100000000000000006e0164
+                  0089005f0700000000000000007411000000000000000000007c01640519
+                  00000000000000000089006a040000000000000000ac06a6020000ab0200
+                  0000000000000089005f09000000000000000088006601640784087c0164
+                  08190000000000000000004400a6000000ab00000000000000000089005f
+                  0a000000000000000064005300
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL                0 (self)
                
                 13           4 RESUME                   0
                
                 14           6 LOAD_FAST                1 (parcel_data)
-                             8 LOAD_CONST               1 ('shipmentNumber')
-                            10 BINARY_SUBSCR
-                            20 LOAD_DEREF               0 (self)
-                            22 STORE_ATTR               0 (shipment_number)
-               
-                15          32 LOAD_FAST                2 (logger)
-                            34 LOAD_METHOD              1 (getChild)
-                            56 LOAD_DEREF               3 (__class__)
-                            58 LOAD_ATTR                2 (__name__)
-                            68 FORMAT_VALUE             0
-                            70 LOAD_CONST               2 ('.')
-                            72 LOAD_DEREF               0 (self)
-                            74 LOAD_ATTR                0 (shipment_number)
-                            84 FORMAT_VALUE             0
-                            86 BUILD_STRING             3
-                            88 PRECALL                  1
-                            92 CALL                     1
-                           102 LOAD_DEREF               0 (self)
-                           104 STORE_ATTR               3 (_log)
-               
-                16         114 LOAD_GLOBAL              8 (ParcelStatus)
-                           126 LOAD_FAST                1 (parcel_data)
-                           128 LOAD_CONST               3 ('status')
-                           130 BINARY_SUBSCR
-                           140 BINARY_SUBSCR
-                           150 LOAD_DEREF               0 (self)
-                           152 STORE_ATTR               5 (status)
-               
-                17         162 LOAD_CONST               4 ('expiryDate')
-                           164 LOAD_FAST                1 (parcel_data)
-                           166 CONTAINS_OP              0
-                           168 POP_JUMP_FORWARD_IF_FALSE    21 (to 212)
-                           170 LOAD_GLOBAL             13 (NULL + get)
-                           182 LOAD_FAST                1 (parcel_data)
-                           184 LOAD_CONST               4 ('expiryDate')
-                           186 BINARY_SUBSCR
-                           196 PRECALL                  1
-                           200 CALL                     1
-                           210 JUMP_FORWARD             1 (to 214)
-                       >>  212 LOAD_CONST               0 (None)
-                       >>  214 LOAD_DEREF               0 (self)
-                           216 STORE_ATTR               7 (expiry_date)
-               
-                18         226 LOAD_GLOBAL             17 (NULL + Operations)
-                           238 LOAD_FAST                1 (parcel_data)
-                           240 LOAD_CONST               5 ('operations')
-                           242 BINARY_SUBSCR
-                           252 LOAD_DEREF               0 (self)
-                           254 LOAD_ATTR                3 (_log)
-                           264 KW_NAMES                 6
-                           266 PRECALL                  2
-                           270 CALL                     2
-                           280 LOAD_DEREF               0 (self)
-                           282 STORE_ATTR               9 (operations)
-               
-                19         292 LOAD_CLOSURE             0 (self)
-                           294 BUILD_TUPLE              1
-                           296 LOAD_CONST               7 (<code object <listcomp>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 19>)
-                           298 MAKE_FUNCTION            8 (closure)
-               
-                20         300 LOAD_FAST                1 (parcel_data)
-                           302 LOAD_CONST               8 ('eventLog')
-                           304 BINARY_SUBSCR
-               
-                19         314 GET_ITER
-                           316 PRECALL                  0
-                           320 CALL                     0
-                           330 LOAD_DEREF               0 (self)
-                           332 STORE_ATTR              10 (event_log)
-                           342 LOAD_CONST               0 (None)
-                           344 RETURN_VALUE
+                             8 LOAD_METHOD              0 (get)
+                            30 LOAD_CONST               1 ('shipmentNumber')
+                            32 PRECALL                  1
+                            36 CALL                     1
+                            46 LOAD_DEREF               0 (self)
+                            48 STORE_ATTR               1 (shipment_number)
+               
+                15          58 LOAD_FAST                2 (logger)
+                            60 LOAD_METHOD              2 (getChild)
+                            82 LOAD_DEREF               3 (__class__)
+                            84 LOAD_ATTR                3 (__name__)
+                            94 FORMAT_VALUE             0
+                            96 LOAD_CONST               2 ('.')
+                            98 LOAD_DEREF               0 (self)
+                           100 LOAD_ATTR                1 (shipment_number)
+                           110 FORMAT_VALUE             0
+                           112 BUILD_STRING             3
+                           114 PRECALL                  1
+                           118 CALL                     1
+                           128 LOAD_DEREF               0 (self)
+                           130 STORE_ATTR               4 (_log)
+               
+                16         140 LOAD_GLOBAL             10 (ParcelStatus)
+                           152 LOAD_FAST                1 (parcel_data)
+                           154 LOAD_CONST               3 ('status')
+                           156 BINARY_SUBSCR
+                           166 BINARY_SUBSCR
+                           176 LOAD_DEREF               0 (self)
+                           178 STORE_ATTR               6 (status)
+               
+                17         188 LOAD_CONST               4 ('expiryDate')
+                           190 LOAD_FAST                1 (parcel_data)
+                           192 CONTAINS_OP              0
+                           194 POP_JUMP_FORWARD_IF_FALSE    21 (to 238)
+                           196 LOAD_GLOBAL              1 (NULL + get)
+                           208 LOAD_FAST                1 (parcel_data)
+                           210 LOAD_CONST               4 ('expiryDate')
+                           212 BINARY_SUBSCR
+                           222 PRECALL                  1
+                           226 CALL                     1
+                           236 JUMP_FORWARD             1 (to 240)
+                       >>  238 LOAD_CONST               0 (None)
+                       >>  240 LOAD_DEREF               0 (self)
+                           242 STORE_ATTR               7 (expiry_date)
+               
+                18         252 LOAD_GLOBAL             17 (NULL + Operations)
+                           264 LOAD_FAST                1 (parcel_data)
+                           266 LOAD_CONST               5 ('operations')
+                           268 BINARY_SUBSCR
+                           278 LOAD_DEREF               0 (self)
+                           280 LOAD_ATTR                4 (_log)
+                           290 KW_NAMES                 6
+                           292 PRECALL                  2
+                           296 CALL                     2
+                           306 LOAD_DEREF               0 (self)
+                           308 STORE_ATTR               9 (operations)
+               
+                19         318 LOAD_CLOSURE             0 (self)
+                           320 BUILD_TUPLE              1
+                           322 LOAD_CONST               7 (<code object <listcomp>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 19>)
+                           324 MAKE_FUNCTION            8 (closure)
+               
+                20         326 LOAD_FAST                1 (parcel_data)
+                           328 LOAD_CONST               8 ('eventLog')
+                           330 BINARY_SUBSCR
+               
+                19         340 GET_ITER
+                           342 PRECALL                  0
+                           346 CALL                     0
+                           356 LOAD_DEREF               0 (self)
+                           358 STORE_ATTR              10 (event_log)
+                           368 LOAD_CONST               0 (None)
+                           370 RETURN_VALUE
                consts
                   None
                   'shipmentNumber'
                   '.'
                   'status'
                   'expiryDate'
                   'operations'
@@ -379,22 +382,22 @@
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<listcomp>'
                      firstlineno 19
                      lnotab 0x0a0102ff
                   'eventLog'
-               names      ('shipment_number', 'getChild', '__name__', '_log', 'ParcelStatus', 'status', 'get', 'expiry_date', 'Operations', 'operations', 'event_log')
+               names      ('get', 'shipment_number', 'getChild', '__name__', '_log', 'ParcelStatus', 'status', 'expiry_date', 'Operations', 'operations', 'event_log')
                varnames   ('self', 'parcel_data', 'logger')
                freevars   ('__class__',)
                cellvars   ('self',)
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
                firstlineno 13
-               lnotab 0x06011a01520130014001420108010eff
+               lnotab 0x06013401520130014001420108010eff
          names      ('__name__', '__module__', '__qualname__', 'dict', 'logging', 'Logger', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'BaseParcel'
          firstlineno 12
@@ -439,165 +442,165 @@
                       34 BUILD_TUPLE              4
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
                       40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 31>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               7 (__init__)
          
-          72          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 72>)
+          73          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 73>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (__repr__)
          
-          76          52 LOAD_CONST               6 (<code object __str__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 76>)
+          77          52 LOAD_CONST               6 (<code object __str__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 77>)
                       54 MAKE_FUNCTION            0
                       56 STORE_NAME               9 (__str__)
          
-          82          58 LOAD_NAME               10 (property)
+          83          58 LOAD_NAME               10 (property)
          
-          83          60 LOAD_CONST               7 ('return')
+          84          60 LOAD_CONST               7 ('return')
                       62 LOAD_NAME               11 (str)
                       64 LOAD_CONST               8 (None)
                       66 BINARY_OP                7 (|)
                       70 BUILD_TUPLE              2
-                      72 LOAD_CONST               9 (<code object open_code, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 82>)
+                      72 LOAD_CONST               9 (<code object open_code, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 83>)
                       74 MAKE_FUNCTION            4 (annotations)
          
-          82          76 PRECALL                  0
+          83          76 PRECALL                  0
                       80 CALL                     0
          
-          83          90 STORE_NAME              12 (open_code)
+          84          90 STORE_NAME              12 (open_code)
          
-          96          92 LOAD_NAME               10 (property)
+          97          92 LOAD_NAME               10 (property)
          
-          97          94 LOAD_CONST               7 ('return')
+          98          94 LOAD_CONST               7 ('return')
                       96 LOAD_NAME               13 (BytesIO)
                       98 LOAD_CONST               8 (None)
                      100 BINARY_OP                7 (|)
                      104 BUILD_TUPLE              2
-                     106 LOAD_CONST              10 (<code object generate_qr_image, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 96>)
+                     106 LOAD_CONST              10 (<code object generate_qr_image, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 97>)
                      108 MAKE_FUNCTION            4 (annotations)
          
-          96         110 PRECALL                  0
+          97         110 PRECALL                  0
                      114 CALL                     0
          
-          97         124 STORE_NAME              14 (generate_qr_image)
+          98         124 STORE_NAME              14 (generate_qr_image)
          
-         110         126 LOAD_NAME               10 (property)
+         111         126 LOAD_NAME               10 (property)
          
-         111         128 LOAD_CONST              11 (<code object compartment_properties, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 110>)
+         112         128 LOAD_CONST              11 (<code object compartment_properties, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 111>)
                      130 MAKE_FUNCTION            0
          
-         110         132 PRECALL                  0
+         111         132 PRECALL                  0
                      136 CALL                     0
          
-         111         146 STORE_NAME              15 (compartment_properties)
+         112         146 STORE_NAME              15 (compartment_properties)
          
-         124         148 LOAD_NAME               15 (compartment_properties)
+         125         148 LOAD_NAME               15 (compartment_properties)
                      150 LOAD_ATTR               16 (setter)
          
-         125         160 LOAD_CONST              12 ('compartmentproperties_data')
+         126         160 LOAD_CONST              12 ('compartmentproperties_data')
                      162 LOAD_NAME                4 (dict)
                      164 BUILD_TUPLE              2
-                     166 LOAD_CONST              13 (<code object compartment_properties, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 124>)
+                     166 LOAD_CONST              13 (<code object compartment_properties, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 125>)
                      168 MAKE_FUNCTION            4 (annotations)
          
-         124         170 PRECALL                  0
+         125         170 PRECALL                  0
                      174 CALL                     0
          
-         125         184 STORE_NAME              15 (compartment_properties)
+         126         184 STORE_NAME              15 (compartment_properties)
          
-         138         186 LOAD_NAME               10 (property)
+         139         186 LOAD_NAME               10 (property)
          
-         139         188 LOAD_CONST              14 (<code object compartment_location, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 138>)
+         140         188 LOAD_CONST              14 (<code object compartment_location, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 139>)
                      190 MAKE_FUNCTION            0
          
-         138         192 PRECALL                  0
+         139         192 PRECALL                  0
                      196 CALL                     0
          
-         139         206 STORE_NAME              17 (compartment_location)
+         140         206 STORE_NAME              17 (compartment_location)
          
-         152         208 LOAD_NAME               17 (compartment_location)
+         153         208 LOAD_NAME               17 (compartment_location)
                      210 LOAD_ATTR               16 (setter)
          
-         153         220 LOAD_CONST              15 ('location_data')
+         154         220 LOAD_CONST              15 ('location_data')
                      222 LOAD_NAME                4 (dict)
                      224 BUILD_TUPLE              2
-                     226 LOAD_CONST              16 (<code object compartment_location, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 152>)
+                     226 LOAD_CONST              16 (<code object compartment_location, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 153>)
                      228 MAKE_FUNCTION            4 (annotations)
          
-         152         230 PRECALL                  0
+         153         230 PRECALL                  0
                      234 CALL                     0
          
-         153         244 STORE_NAME              17 (compartment_location)
+         154         244 STORE_NAME              17 (compartment_location)
          
-         164         246 LOAD_NAME               10 (property)
+         165         246 LOAD_NAME               10 (property)
          
-         165         248 LOAD_CONST               7 ('return')
+         166         248 LOAD_CONST               7 ('return')
                      250 LOAD_NAME               18 (CompartmentActualStatus)
                      252 LOAD_CONST               8 (None)
                      254 BINARY_OP                7 (|)
                      258 BUILD_TUPLE              2
-                     260 LOAD_CONST              17 (<code object compartment_status, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 164>)
+                     260 LOAD_CONST              17 (<code object compartment_status, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 165>)
                      262 MAKE_FUNCTION            4 (annotations)
          
-         164         264 PRECALL                  0
+         165         264 PRECALL                  0
                      268 CALL                     0
          
-         165         278 STORE_NAME              19 (compartment_status)
+         166         278 STORE_NAME              19 (compartment_status)
          
-         179         280 LOAD_NAME               19 (compartment_status)
+         180         280 LOAD_NAME               19 (compartment_status)
                      282 LOAD_ATTR               16 (setter)
          
-         180         292 LOAD_CONST              18 (<code object compartment_status, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 179>)
+         181         292 LOAD_CONST              18 (<code object compartment_status, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 180>)
                      294 MAKE_FUNCTION            0
          
-         179         296 PRECALL                  0
+         180         296 PRECALL                  0
                      300 CALL                     0
          
-         180         310 STORE_NAME              19 (compartment_status)
+         181         310 STORE_NAME              19 (compartment_status)
          
-         188         312 LOAD_NAME               10 (property)
+         189         312 LOAD_NAME               10 (property)
          
-         189         314 LOAD_CONST              19 (<code object compartment_open_data, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 188>)
+         190         314 LOAD_CONST              19 (<code object compartment_open_data, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 189>)
                      316 MAKE_FUNCTION            0
          
-         188         318 PRECALL                  0
+         189         318 PRECALL                  0
                      322 CALL                     0
          
-         189         332 STORE_NAME              20 (compartment_open_data)
+         190         332 STORE_NAME              20 (compartment_open_data)
          
-         206         334 LOAD_NAME               10 (property)
+         207         334 LOAD_NAME               10 (property)
          
-         207         336 LOAD_CONST              20 (<code object mocked_location, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 206>)
+         208         336 LOAD_CONST              20 (<code object mocked_location, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 207>)
                      338 MAKE_FUNCTION            0
          
-         206         340 PRECALL                  0
+         207         340 PRECALL                  0
                      344 CALL                     0
          
-         207         354 STORE_NAME              21 (mocked_location)
+         208         354 STORE_NAME              21 (mocked_location)
          
-         224         356 LOAD_NAME               10 (property)
+         225         356 LOAD_NAME               10 (property)
          
-         225         358 LOAD_CONST              21 (<code object is_multicompartment, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 224>)
+         226         358 LOAD_CONST              21 (<code object is_multicompartment, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 225>)
                      360 MAKE_FUNCTION            0
          
-         224         362 PRECALL                  0
+         225         362 PRECALL                  0
                      366 CALL                     0
          
-         225         376 STORE_NAME              22 (is_multicompartment)
+         226         376 STORE_NAME              22 (is_multicompartment)
          
-         231         378 LOAD_NAME               10 (property)
+         232         378 LOAD_NAME               10 (property)
          
-         232         380 LOAD_CONST              22 (<code object is_main_multicompartment, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 231>)
+         233         380 LOAD_CONST              22 (<code object is_main_multicompartment, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 232>)
                      382 MAKE_FUNCTION            0
          
-         231         384 PRECALL                  0
+         232         384 PRECALL                  0
                      388 CALL                     0
          
-         232         398 STORE_NAME              23 (is_main_multicompartment)
+         233         398 STORE_NAME              23 (is_main_multicompartment)
                      400 LOAD_CLOSURE             0 (__class__)
                      402 COPY                     1
                      404 STORE_NAME              24 (__classcell__)
                      406 RETURN_VALUE
          consts
             'Parcel'
             'Object representation of :class:`inpost.api.Inpost` compartment properties\n\n    :param parcel_data: :class:`dict` containing all parcel data\n    :type parcel_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger'
@@ -611,63 +614,69 @@
                code
                   0x950187009700740100000000000000000000a6000000ab000000000000
                   000000a00100000000000000000000000000000000000000007c017c02a6
                   020000ab02000000000000000001007c02a0020000000000000000000000
                   00000000000000000089036a0300000000000000009b00640189006a0400
                   000000000000009b009d03a6010000ab01000000000000000089005f0500
                   00000000000000740c000000000000000000007c01640219000000000000
-                  0000001900000000000000000089005f07000000000000000064037c0176
-                  0072087c016403190000000000000000006e01640489005f080000000000
-                  00000064057c017600721c7413000000000000000000007c016405190000
-                  0000000000000089006a050000000000000000ac06a6020000ab02000000
-                  00000000006e01640489005f0a000000000000000064077c017600721574
-                  17000000000000000000007c01640719000000000000000000a6010000ab
-                  0100000000000000006e01640489005f0c000000000000000064087c0176
-                  0072157417000000000000000000007c01640819000000000000000000a6
-                  010000ab0100000000000000006e01640489005f0d000000000000000089
-                  006a070000000000000000740c000000000000000000006a0e0000000000
-                  0000006b02000000007213741e000000000000000000007c016409190000
-                  00000000000000190000000000000000006e127420000000000000000000
-                  007c016409190000000000000000001900000000000000000089005f1100
-                  000000000000007425000000000000000000007c01640a19000000000000
-                  00000089006a050000000000000000ac0ba6020000ab0200000000000000
-                  0089005f1300000000000000007429000000000000000000007c01640c19
-                  00000000000000000089006a050000000000000000ac0da6020000ab0200
-                  0000000000000089005f150000000000000000640e7c017600721c742d00
-                  0000000000000000007c01640e1900000000000000000089006a05000000
-                  0000000000ac0fa6020000ab0200000000000000006e01640489005f1700
-                  0000000000000064107c017600721c7431000000000000000000007c0164
-                  101900000000000000000089006a050000000000000000ac11a6020000ab
-                  0200000000000000006e01640489005f1900000000000000007c01641219
-                  00000000000000000089005f1a0000000000000000743600000000000000
-                  0000007c016413190000000000000000001900000000000000000089005f
-                  1c00000000000000007c0164141900000000000000000089005f1d000000
-                  000000000088006601641584087c016416190000000000000000004400a6
-                  000000ab00000000000000000089005f1e0000000000000000743e000000
-                  000000000000007c01641719000000000000000000190000000000000000
-                  0089005f200000000000000000640489005f21000000000000000089006a
-                  050000000000000000a02200000000000000000000000000000000000000
-                  00641889006a0400000000000000009b009d02a6010000ab010000000000
-                  000000010089006a070000000000000000740c000000000000000000006a
-                  2300000000000000006b0200000000722389006a050000000000000000a0
-                  22000000000000000000000000000000000000000064197c016402190000
-                  000000000000009b009d02a6010000ab010000000000000000010089006a
-                  1100000000000000007420000000000000000000006a2300000000000000
-                  006b0200000000731589006a110000000000000000741e00000000000000
-                  0000006a2300000000000000006b0200000000722389006a050000000000
-                  000000a0220000000000000000000000000000000000000000641a7c0164
-                  09190000000000000000009b009d02a6010000ab01000000000000000001
-                  0089006a1c00000000000000007436000000000000000000006a23000000
-                  00000000006b0200000000722389006a050000000000000000a022000000
-                  0000000000000000000000000000000000641b7c01641319000000000000
-                  0000009b009d02a6010000ab010000000000000000010089006a20000000
-                  0000000000743e000000000000000000006a2300000000000000006b0200
-                  000000722589006a050000000000000000a0220000000000000000000000
-                  000000000000000000641c7c016417190000000000000000009b009d02a6
-                  010000ab01000000000000000001006404530064045300
+                  0000001900000000000000000089005f0700000000000000007c01a00800
+                  0000000000000000000000000000000000000064036404a6020000ab0200
+                  0000000000000089005f09000000000000000064057c017600721c741500
+                  0000000000000000007c0164051900000000000000000089006a05000000
+                  0000000000ac06a6020000ab0200000000000000006e01640489005f0b00
+                  0000000000000064077c01760072157411000000000000000000007c0164
+                  0719000000000000000000a6010000ab0100000000000000006e01640489
+                  005f0c000000000000000064087c01760072157411000000000000000000
+                  007c01640819000000000000000000a6010000ab0100000000000000006e
+                  01640489005f0d000000000000000089006a070000000000000000740c00
+                  0000000000000000006a0e00000000000000006b02000000007213741e00
+                  0000000000000000007c0164091900000000000000000019000000000000
+                  0000006e127420000000000000000000007c016409190000000000000000
+                  001900000000000000000089005f110000000000000000640a7c01760072
+                  1c7425000000000000000000007c01640b1900000000000000000089006a
+                  050000000000000000ac0ca6020000ab0200000000000000006e01640489
+                  005f130000000000000000640d7c017600721c7429000000000000000000
+                  007c01640d1900000000000000000089006a050000000000000000ac0ea6
+                  020000ab0200000000000000006e01640489005f15000000000000000064
+                  0f7c017600721c742d000000000000000000007c01640f19000000000000
+                  00000089006a050000000000000000ac10a6020000ab0200000000000000
+                  006e01640489005f17000000000000000064117c017600721c7431000000
+                  000000000000007c0164111900000000000000000089006a050000000000
+                  000000ac12a6020000ab0200000000000000006e01640489005f19000000
+                  00000000007c01a008000000000000000000000000000000000000000064
+                  136404a6020000ab02000000000000000089005f1a000000000000000064
+                  147c01760072137436000000000000000000007c01641419000000000000
+                  000000190000000000000000006e01640489005f1c00000000000000007c
+                  01a008000000000000000000000000000000000000000064156404a60200
+                  00ab02000000000000000089005f1d000000000000000064167c01760072
+                  1488006601641784087c016416190000000000000000004400a6000000ab
+                  0000000000000000006e01640489005f1e000000000000000064187c0176
+                  007213743e000000000000000000007c0164181900000000000000000019
+                  0000000000000000006e01640489005f2000000000000000007c01a00800
+                  0000000000000000000000000000000000000064196404a6020000ab0200
+                  0000000000000089005f210000000000000000640489005f220000000000
+                  00000089006a050000000000000000a02300000000000000000000000000
+                  00000000000000641a89006a0400000000000000009b009d02a6010000ab
+                  010000000000000000010089006a070000000000000000740c0000000000
+                  00000000006a2400000000000000006b0200000000722389006a05000000
+                  0000000000a0230000000000000000000000000000000000000000641b7c
+                  016402190000000000000000009b009d02a6010000ab0100000000000000
+                  00010089006a1100000000000000007420000000000000000000006a2400
+                  000000000000006b0200000000731589006a110000000000000000741e00
+                  0000000000000000006a2400000000000000006b0200000000722389006a
+                  050000000000000000a02300000000000000000000000000000000000000
+                  00641c7c016409190000000000000000009b009d02a6010000ab01000000
+                  0000000000010089006a1c00000000000000007436000000000000000000
+                  006a2400000000000000006b0200000000722389006a0500000000000000
+                  00a0230000000000000000000000000000000000000000641d7c01641419
+                  0000000000000000009b009d02a6010000ab010000000000000000010089
+                  006a200000000000000000743e000000000000000000006a240000000000
+                  0000006b0200000000722589006a050000000000000000a0230000000000
+                  000000000000000000000000000000641e7c016418190000000000000000
+                  009b009d02a6010000ab01000000000000000001006404530064045300
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL                0 (self)
                
                 31           4 RESUME                   0
                
                 33           6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
@@ -698,339 +707,386 @@
                            168 LOAD_FAST                1 (parcel_data)
                            170 LOAD_CONST               2 ('shipmentType')
                            172 BINARY_SUBSCR
                            182 BINARY_SUBSCR
                            192 LOAD_DEREF               0 (self)
                            194 STORE_ATTR               7 (shipment_type)
                
-                36         204 LOAD_CONST               3 ('openCode')
-                           206 LOAD_FAST                1 (parcel_data)
-                           208 CONTAINS_OP              0
-                           210 POP_JUMP_FORWARD_IF_FALSE     8 (to 228)
-                           212 LOAD_FAST                1 (parcel_data)
-                           214 LOAD_CONST               3 ('openCode')
-                           216 BINARY_SUBSCR
-                           226 JUMP_FORWARD             1 (to 230)
-                       >>  228 LOAD_CONST               4 (None)
-                       >>  230 LOAD_DEREF               0 (self)
-                           232 STORE_ATTR               8 (_open_code)
-               
-                38         242 LOAD_CONST               5 ('qrCode')
-                           244 LOAD_FAST                1 (parcel_data)
-                           246 CONTAINS_OP              0
-                           248 POP_JUMP_FORWARD_IF_FALSE    28 (to 306)
-               
-                37         250 LOAD_GLOBAL             19 (NULL + QRCode)
-                           262 LOAD_FAST                1 (parcel_data)
-                           264 LOAD_CONST               5 ('qrCode')
-                           266 BINARY_SUBSCR
-                           276 LOAD_DEREF               0 (self)
-                           278 LOAD_ATTR                5 (_log)
-                           288 KW_NAMES                 6
-                           290 PRECALL                  2
-                           294 CALL                     2
-                           304 JUMP_FORWARD             1 (to 308)
-               
-                38     >>  306 LOAD_CONST               4 (None)
-               
-                37     >>  308 LOAD_DEREF               0 (self)
-                           310 STORE_ATTR              10 (_qr_code)
-               
-                39         320 LOAD_CONST               7 ('storedDate')
-                           322 LOAD_FAST                1 (parcel_data)
-                           324 CONTAINS_OP              0
-                           326 POP_JUMP_FORWARD_IF_FALSE    21 (to 370)
-                           328 LOAD_GLOBAL             23 (NULL + get)
-                           340 LOAD_FAST                1 (parcel_data)
-                           342 LOAD_CONST               7 ('storedDate')
-                           344 BINARY_SUBSCR
-                           354 PRECALL                  1
-                           358 CALL                     1
-                           368 JUMP_FORWARD             1 (to 372)
-                       >>  370 LOAD_CONST               4 (None)
-                       >>  372 LOAD_DEREF               0 (self)
-                           374 STORE_ATTR              12 (stored_date)
-               
-                40         384 LOAD_CONST               8 ('pickUpDate')
-                           386 LOAD_FAST                1 (parcel_data)
-                           388 CONTAINS_OP              0
-                           390 POP_JUMP_FORWARD_IF_FALSE    21 (to 434)
-                           392 LOAD_GLOBAL             23 (NULL + get)
-                           404 LOAD_FAST                1 (parcel_data)
-                           406 LOAD_CONST               8 ('pickUpDate')
-                           408 BINARY_SUBSCR
-                           418 PRECALL                  1
-                           422 CALL                     1
-                           432 JUMP_FORWARD             1 (to 436)
-                       >>  434 LOAD_CONST               4 (None)
-                       >>  436 LOAD_DEREF               0 (self)
-                           438 STORE_ATTR              13 (pickup_date)
-               
-                42         448 LOAD_DEREF               0 (self)
-                           450 LOAD_ATTR                7 (shipment_type)
-                           460 LOAD_GLOBAL             12 (ParcelShipmentType)
-                           472 LOAD_ATTR               14 (parcel)
-                           482 COMPARE_OP               2 (==)
-                           488 POP_JUMP_FORWARD_IF_FALSE    19 (to 528)
-               
-                41         490 LOAD_GLOBAL             30 (ParcelLockerSize)
-                           502 LOAD_FAST                1 (parcel_data)
-                           504 LOAD_CONST               9 ('parcelSize')
-                           506 BINARY_SUBSCR
-                           516 BINARY_SUBSCR
-                           526 JUMP_FORWARD            18 (to 564)
-               
-                42     >>  528 LOAD_GLOBAL             32 (ParcelCarrierSize)
-                           540 LOAD_FAST                1 (parcel_data)
-                           542 LOAD_CONST               9 ('parcelSize')
-                           544 BINARY_SUBSCR
-                           554 BINARY_SUBSCR
-               
-                41     >>  564 LOAD_DEREF               0 (self)
-                           566 STORE_ATTR              17 (parcel_size)
-               
-                43         576 LOAD_GLOBAL             37 (NULL + Receiver)
-                           588 LOAD_FAST                1 (parcel_data)
-                           590 LOAD_CONST              10 ('receiver')
-                           592 BINARY_SUBSCR
-                           602 LOAD_DEREF               0 (self)
-                           604 LOAD_ATTR                5 (_log)
-                           614 KW_NAMES                11
-                           616 PRECALL                  2
-                           620 CALL                     2
-                           630 LOAD_DEREF               0 (self)
-                           632 STORE_ATTR              19 (receiver)
-               
-                44         642 LOAD_GLOBAL             41 (NULL + Sender)
-                           654 LOAD_FAST                1 (parcel_data)
-                           656 LOAD_CONST              12 ('sender')
-                           658 BINARY_SUBSCR
-                           668 LOAD_DEREF               0 (self)
-                           670 LOAD_ATTR                5 (_log)
-                           680 KW_NAMES                13
-                           682 PRECALL                  2
-                           686 CALL                     2
-                           696 LOAD_DEREF               0 (self)
-                           698 STORE_ATTR              21 (sender)
-               
-                46         708 LOAD_CONST              14 ('pickUpPoint')
-                           710 LOAD_FAST                1 (parcel_data)
-                           712 CONTAINS_OP              0
-                           714 POP_JUMP_FORWARD_IF_FALSE    28 (to 772)
-               
-                45         716 LOAD_GLOBAL             45 (NULL + PickupPoint)
-                           728 LOAD_FAST                1 (parcel_data)
-                           730 LOAD_CONST              14 ('pickUpPoint')
-                           732 BINARY_SUBSCR
-                           742 LOAD_DEREF               0 (self)
-                           744 LOAD_ATTR                5 (_log)
-                           754 KW_NAMES                15
-                           756 PRECALL                  2
-                           760 CALL                     2
-                           770 JUMP_FORWARD             1 (to 774)
-               
-                46     >>  772 LOAD_CONST               4 (None)
-               
-                45     >>  774 LOAD_DEREF               0 (self)
-                           776 STORE_ATTR              23 (pickup_point)
-               
-                48         786 LOAD_CONST              16 ('multiCompartment')
-                           788 LOAD_FAST                1 (parcel_data)
-                           790 CONTAINS_OP              0
-                           792 POP_JUMP_FORWARD_IF_FALSE    28 (to 850)
-               
-                47         794 LOAD_GLOBAL             49 (NULL + MultiCompartment)
-               
-                48         806 LOAD_FAST                1 (parcel_data)
-                           808 LOAD_CONST              16 ('multiCompartment')
-                           810 BINARY_SUBSCR
-                           820 LOAD_DEREF               0 (self)
-                           822 LOAD_ATTR                5 (_log)
-               
-                47         832 KW_NAMES                17
-                           834 PRECALL                  2
-                           838 CALL                     2
-                           848 JUMP_FORWARD             1 (to 852)
-               
-                48     >>  850 LOAD_CONST               4 (None)
-               
-                47     >>  852 LOAD_DEREF               0 (self)
-                           854 STORE_ATTR              25 (multi_compartment)
-               
-                49         864 LOAD_FAST                1 (parcel_data)
-                           866 LOAD_CONST              18 ('endOfWeekCollection')
-                           868 BINARY_SUBSCR
-                           878 LOAD_DEREF               0 (self)
-                           880 STORE_ATTR              26 (is_end_off_week_collection)
-               
-                50         890 LOAD_GLOBAL             54 (ParcelStatus)
-                           902 LOAD_FAST                1 (parcel_data)
-                           904 LOAD_CONST              19 ('status')
-                           906 BINARY_SUBSCR
-                           916 BINARY_SUBSCR
-                           926 LOAD_DEREF               0 (self)
-                           928 STORE_ATTR              28 (status)
-               
-                51         938 LOAD_FAST                1 (parcel_data)
-                           940 LOAD_CONST              20 ('avizoTransactionStatus')
-                           942 BINARY_SUBSCR
-                           952 LOAD_DEREF               0 (self)
-                           954 STORE_ATTR              29 (avizo_transaction_status)
-               
-                52         964 LOAD_CLOSURE             0 (self)
-                           966 BUILD_TUPLE              1
-                           968 LOAD_CONST              21 (<code object <listcomp>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 52>)
-                           970 MAKE_FUNCTION            8 (closure)
-               
-                53         972 LOAD_FAST                1 (parcel_data)
-                           974 LOAD_CONST              22 ('sharedTo')
-                           976 BINARY_SUBSCR
-               
-                52         986 GET_ITER
-                           988 PRECALL                  0
-                           992 CALL                     0
-                          1002 LOAD_DEREF               0 (self)
-                          1004 STORE_ATTR              30 (shared_to)
-               
-                54        1014 LOAD_GLOBAL             62 (ParcelOwnership)
-                          1026 LOAD_FAST                1 (parcel_data)
-                          1028 LOAD_CONST              23 ('ownershipStatus')
-                          1030 BINARY_SUBSCR
-                          1040 BINARY_SUBSCR
-                          1050 LOAD_DEREF               0 (self)
-                          1052 STORE_ATTR              32 (ownership_status)
-               
-                55        1062 LOAD_CONST               4 (None)
-                          1064 LOAD_DEREF               0 (self)
-                          1066 STORE_ATTR              33 (_compartment_properties)
-               
-                57        1076 LOAD_DEREF               0 (self)
-                          1078 LOAD_ATTR                5 (_log)
-                          1088 LOAD_METHOD             34 (debug)
-                          1110 LOAD_CONST              24 ('created parcel with shipment number ')
-                          1112 LOAD_DEREF               0 (self)
-                          1114 LOAD_ATTR                4 (shipment_number)
-                          1124 FORMAT_VALUE             0
-                          1126 BUILD_STRING             2
-                          1128 PRECALL                  1
-                          1132 CALL                     1
-                          1142 POP_TOP
-               
-                60        1144 LOAD_DEREF               0 (self)
-                          1146 LOAD_ATTR                7 (shipment_type)
-                          1156 LOAD_GLOBAL             12 (ParcelShipmentType)
-                          1168 LOAD_ATTR               35 (UNKNOWN)
-                          1178 COMPARE_OP               2 (==)
-                          1184 POP_JUMP_FORWARD_IF_FALSE    35 (to 1256)
-               
-                61        1186 LOAD_DEREF               0 (self)
-                          1188 LOAD_ATTR                5 (_log)
-                          1198 LOAD_METHOD             34 (debug)
-                          1220 LOAD_CONST              25 ('unexpected shipment_type: ')
-                          1222 LOAD_FAST                1 (parcel_data)
-                          1224 LOAD_CONST               2 ('shipmentType')
-                          1226 BINARY_SUBSCR
-                          1236 FORMAT_VALUE             0
-                          1238 BUILD_STRING             2
-                          1240 PRECALL                  1
-                          1244 CALL                     1
-                          1254 POP_TOP
-               
-                63     >> 1256 LOAD_DEREF               0 (self)
-                          1258 LOAD_ATTR               17 (parcel_size)
-                          1268 LOAD_GLOBAL             32 (ParcelCarrierSize)
-                          1280 LOAD_ATTR               35 (UNKNOWN)
-                          1290 COMPARE_OP               2 (==)
-                          1296 POP_JUMP_FORWARD_IF_TRUE    21 (to 1340)
+                36         204 LOAD_FAST                1 (parcel_data)
+                           206 LOAD_METHOD              8 (get)
+                           228 LOAD_CONST               3 ('openCode')
+                           230 LOAD_CONST               4 (None)
+                           232 PRECALL                  2
+                           236 CALL                     2
+                           246 LOAD_DEREF               0 (self)
+                           248 STORE_ATTR               9 (_open_code)
+               
+                38         258 LOAD_CONST               5 ('qrCode')
+                           260 LOAD_FAST                1 (parcel_data)
+                           262 CONTAINS_OP              0
+                           264 POP_JUMP_FORWARD_IF_FALSE    28 (to 322)
+               
+                37         266 LOAD_GLOBAL             21 (NULL + QRCode)
+                           278 LOAD_FAST                1 (parcel_data)
+                           280 LOAD_CONST               5 ('qrCode')
+                           282 BINARY_SUBSCR
+                           292 LOAD_DEREF               0 (self)
+                           294 LOAD_ATTR                5 (_log)
+                           304 KW_NAMES                 6
+                           306 PRECALL                  2
+                           310 CALL                     2
+                           320 JUMP_FORWARD             1 (to 324)
+               
+                38     >>  322 LOAD_CONST               4 (None)
+               
+                37     >>  324 LOAD_DEREF               0 (self)
+                           326 STORE_ATTR              11 (_qr_code)
+               
+                39         336 LOAD_CONST               7 ('storedDate')
+                           338 LOAD_FAST                1 (parcel_data)
+                           340 CONTAINS_OP              0
+                           342 POP_JUMP_FORWARD_IF_FALSE    21 (to 386)
+                           344 LOAD_GLOBAL             17 (NULL + get)
+                           356 LOAD_FAST                1 (parcel_data)
+                           358 LOAD_CONST               7 ('storedDate')
+                           360 BINARY_SUBSCR
+                           370 PRECALL                  1
+                           374 CALL                     1
+                           384 JUMP_FORWARD             1 (to 388)
+                       >>  386 LOAD_CONST               4 (None)
+                       >>  388 LOAD_DEREF               0 (self)
+                           390 STORE_ATTR              12 (stored_date)
+               
+                40         400 LOAD_CONST               8 ('pickUpDate')
+                           402 LOAD_FAST                1 (parcel_data)
+                           404 CONTAINS_OP              0
+                           406 POP_JUMP_FORWARD_IF_FALSE    21 (to 450)
+                           408 LOAD_GLOBAL             17 (NULL + get)
+                           420 LOAD_FAST                1 (parcel_data)
+                           422 LOAD_CONST               8 ('pickUpDate')
+                           424 BINARY_SUBSCR
+                           434 PRECALL                  1
+                           438 CALL                     1
+                           448 JUMP_FORWARD             1 (to 452)
+                       >>  450 LOAD_CONST               4 (None)
+                       >>  452 LOAD_DEREF               0 (self)
+                           454 STORE_ATTR              13 (pickup_date)
+               
+                42         464 LOAD_DEREF               0 (self)
+                           466 LOAD_ATTR                7 (shipment_type)
+                           476 LOAD_GLOBAL             12 (ParcelShipmentType)
+                           488 LOAD_ATTR               14 (parcel)
+                           498 COMPARE_OP               2 (==)
+                           504 POP_JUMP_FORWARD_IF_FALSE    19 (to 544)
+               
+                41         506 LOAD_GLOBAL             30 (ParcelLockerSize)
+                           518 LOAD_FAST                1 (parcel_data)
+                           520 LOAD_CONST               9 ('parcelSize')
+                           522 BINARY_SUBSCR
+                           532 BINARY_SUBSCR
+                           542 JUMP_FORWARD            18 (to 580)
+               
+                42     >>  544 LOAD_GLOBAL             32 (ParcelCarrierSize)
+                           556 LOAD_FAST                1 (parcel_data)
+                           558 LOAD_CONST               9 ('parcelSize')
+                           560 BINARY_SUBSCR
+                           570 BINARY_SUBSCR
+               
+                41     >>  580 LOAD_DEREF               0 (self)
+                           582 STORE_ATTR              17 (parcel_size)
+               
+                43         592 LOAD_CONST              10 ('reveiver')
+                           594 LOAD_FAST                1 (parcel_data)
+                           596 CONTAINS_OP              0
+                           598 POP_JUMP_FORWARD_IF_FALSE    28 (to 656)
+                           600 LOAD_GLOBAL             37 (NULL + Receiver)
+                           612 LOAD_FAST                1 (parcel_data)
+                           614 LOAD_CONST              11 ('receiver')
+                           616 BINARY_SUBSCR
+                           626 LOAD_DEREF               0 (self)
+                           628 LOAD_ATTR                5 (_log)
+                           638 KW_NAMES                12
+                           640 PRECALL                  2
+                           644 CALL                     2
+                           654 JUMP_FORWARD             1 (to 658)
+                       >>  656 LOAD_CONST               4 (None)
+                       >>  658 LOAD_DEREF               0 (self)
+                           660 STORE_ATTR              19 (receiver)
+               
+                44         670 LOAD_CONST              13 ('sender')
+                           672 LOAD_FAST                1 (parcel_data)
+                           674 CONTAINS_OP              0
+                           676 POP_JUMP_FORWARD_IF_FALSE    28 (to 734)
+                           678 LOAD_GLOBAL             41 (NULL + Sender)
+                           690 LOAD_FAST                1 (parcel_data)
+                           692 LOAD_CONST              13 ('sender')
+                           694 BINARY_SUBSCR
+                           704 LOAD_DEREF               0 (self)
+                           706 LOAD_ATTR                5 (_log)
+                           716 KW_NAMES                14
+                           718 PRECALL                  2
+                           722 CALL                     2
+                           732 JUMP_FORWARD             1 (to 736)
+                       >>  734 LOAD_CONST               4 (None)
+                       >>  736 LOAD_DEREF               0 (self)
+                           738 STORE_ATTR              21 (sender)
+               
+                46         748 LOAD_CONST              15 ('pickUpPoint')
+                           750 LOAD_FAST                1 (parcel_data)
+                           752 CONTAINS_OP              0
+                           754 POP_JUMP_FORWARD_IF_FALSE    28 (to 812)
+               
+                45         756 LOAD_GLOBAL             45 (NULL + PickupPoint)
+                           768 LOAD_FAST                1 (parcel_data)
+                           770 LOAD_CONST              15 ('pickUpPoint')
+                           772 BINARY_SUBSCR
+                           782 LOAD_DEREF               0 (self)
+                           784 LOAD_ATTR                5 (_log)
+                           794 KW_NAMES                16
+                           796 PRECALL                  2
+                           800 CALL                     2
+                           810 JUMP_FORWARD             1 (to 814)
+               
+                46     >>  812 LOAD_CONST               4 (None)
+               
+                45     >>  814 LOAD_DEREF               0 (self)
+                           816 STORE_ATTR              23 (pickup_point)
+               
+                48         826 LOAD_CONST              17 ('multiCompartment')
+                           828 LOAD_FAST                1 (parcel_data)
+                           830 CONTAINS_OP              0
+                           832 POP_JUMP_FORWARD_IF_FALSE    28 (to 890)
+               
+                47         834 LOAD_GLOBAL             49 (NULL + MultiCompartment)
+               
+                48         846 LOAD_FAST                1 (parcel_data)
+                           848 LOAD_CONST              17 ('multiCompartment')
+                           850 BINARY_SUBSCR
+                           860 LOAD_DEREF               0 (self)
+                           862 LOAD_ATTR                5 (_log)
+               
+                47         872 KW_NAMES                18
+                           874 PRECALL                  2
+                           878 CALL                     2
+                           888 JUMP_FORWARD             1 (to 892)
+               
+                48     >>  890 LOAD_CONST               4 (None)
+               
+                47     >>  892 LOAD_DEREF               0 (self)
+                           894 STORE_ATTR              25 (multi_compartment)
+               
+                49         904 LOAD_FAST                1 (parcel_data)
+                           906 LOAD_METHOD              8 (get)
+                           928 LOAD_CONST              19 ('endOfWeekCollection')
+                           930 LOAD_CONST               4 (None)
+                           932 PRECALL                  2
+                           936 CALL                     2
+                           946 LOAD_DEREF               0 (self)
+                           948 STORE_ATTR              26 (is_end_off_week_collection)
+               
+                50         958 LOAD_CONST              20 ('status')
+                           960 LOAD_FAST                1 (parcel_data)
+                           962 CONTAINS_OP              0
+                           964 POP_JUMP_FORWARD_IF_FALSE    19 (to 1004)
+                           966 LOAD_GLOBAL             54 (ParcelStatus)
+                           978 LOAD_FAST                1 (parcel_data)
+                           980 LOAD_CONST              20 ('status')
+                           982 BINARY_SUBSCR
+                           992 BINARY_SUBSCR
+                          1002 JUMP_FORWARD             1 (to 1006)
+                       >> 1004 LOAD_CONST               4 (None)
+                       >> 1006 LOAD_DEREF               0 (self)
+                          1008 STORE_ATTR              28 (status)
+               
+                51        1018 LOAD_FAST                1 (parcel_data)
+                          1020 LOAD_METHOD              8 (get)
+                          1042 LOAD_CONST              21 ('avizoTransactionStatus')
+                          1044 LOAD_CONST               4 (None)
+                          1046 PRECALL                  2
+                          1050 CALL                     2
+                          1060 LOAD_DEREF               0 (self)
+                          1062 STORE_ATTR              29 (avizo_transaction_status)
+               
+                53        1072 LOAD_CONST              22 ('sharedTo')
+                          1074 LOAD_FAST                1 (parcel_data)
+                          1076 CONTAINS_OP              0
+                          1078 POP_JUMP_FORWARD_IF_FALSE    20 (to 1120)
+               
+                52        1080 LOAD_CLOSURE             0 (self)
+                          1082 BUILD_TUPLE              1
+                          1084 LOAD_CONST              23 (<code object <listcomp>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 52>)
+                          1086 MAKE_FUNCTION            8 (closure)
+               
+                53        1088 LOAD_FAST                1 (parcel_data)
+                          1090 LOAD_CONST              22 ('sharedTo')
+                          1092 BINARY_SUBSCR
+               
+                52        1102 GET_ITER
+                          1104 PRECALL                  0
+                          1108 CALL                     0
+                          1118 JUMP_FORWARD             1 (to 1122)
+               
+                53     >> 1120 LOAD_CONST               4 (None)
+               
+                52     >> 1122 LOAD_DEREF               0 (self)
+                          1124 STORE_ATTR              30 (shared_to)
+               
+                54        1134 LOAD_CONST              24 ('ownershipStatus')
+                          1136 LOAD_FAST                1 (parcel_data)
+                          1138 CONTAINS_OP              0
+                          1140 POP_JUMP_FORWARD_IF_FALSE    19 (to 1180)
+                          1142 LOAD_GLOBAL             62 (ParcelOwnership)
+                          1154 LOAD_FAST                1 (parcel_data)
+                          1156 LOAD_CONST              24 ('ownershipStatus')
+                          1158 BINARY_SUBSCR
+                          1168 BINARY_SUBSCR
+                          1178 JUMP_FORWARD             1 (to 1182)
+                       >> 1180 LOAD_CONST               4 (None)
+                       >> 1182 LOAD_DEREF               0 (self)
+                          1184 STORE_ATTR              32 (ownership_status)
+               
+                55        1194 LOAD_FAST                1 (parcel_data)
+                          1196 LOAD_METHOD              8 (get)
+                          1218 LOAD_CONST              25 ('economyParcel')
+                          1220 LOAD_CONST               4 (None)
+                          1222 PRECALL                  2
+                          1226 CALL                     2
+                          1236 LOAD_DEREF               0 (self)
+                          1238 STORE_ATTR              33 (economy_parcel)
+               
+                56        1248 LOAD_CONST               4 (None)
+                          1250 LOAD_DEREF               0 (self)
+                          1252 STORE_ATTR              34 (_compartment_properties)
+               
+                58        1262 LOAD_DEREF               0 (self)
+                          1264 LOAD_ATTR                5 (_log)
+                          1274 LOAD_METHOD             35 (debug)
+                          1296 LOAD_CONST              26 ('created parcel with shipment number ')
                           1298 LOAD_DEREF               0 (self)
-                          1300 LOAD_ATTR               17 (parcel_size)
-                          1310 LOAD_GLOBAL             30 (ParcelLockerSize)
-                          1322 LOAD_ATTR               35 (UNKNOWN)
-                          1332 COMPARE_OP               2 (==)
-                          1338 POP_JUMP_FORWARD_IF_FALSE    35 (to 1410)
-               
-                64     >> 1340 LOAD_DEREF               0 (self)
-                          1342 LOAD_ATTR                5 (_log)
-                          1352 LOAD_METHOD             34 (debug)
-                          1374 LOAD_CONST              26 ('unexpected parcel_size: ')
-                          1376 LOAD_FAST                1 (parcel_data)
-                          1378 LOAD_CONST               9 ('parcelSize')
-                          1380 BINARY_SUBSCR
-                          1390 FORMAT_VALUE             0
-                          1392 BUILD_STRING             2
-                          1394 PRECALL                  1
-                          1398 CALL                     1
-                          1408 POP_TOP
-               
-                66     >> 1410 LOAD_DEREF               0 (self)
-                          1412 LOAD_ATTR               28 (status)
-                          1422 LOAD_GLOBAL             54 (ParcelStatus)
-                          1434 LOAD_ATTR               35 (UNKNOWN)
-                          1444 COMPARE_OP               2 (==)
-                          1450 POP_JUMP_FORWARD_IF_FALSE    35 (to 1522)
-               
-                67        1452 LOAD_DEREF               0 (self)
-                          1454 LOAD_ATTR                5 (_log)
-                          1464 LOAD_METHOD             34 (debug)
-                          1486 LOAD_CONST              27 ('unexpected parcel status: ')
-                          1488 LOAD_FAST                1 (parcel_data)
-                          1490 LOAD_CONST              19 ('status')
-                          1492 BINARY_SUBSCR
-                          1502 FORMAT_VALUE             0
-                          1504 BUILD_STRING             2
-                          1506 PRECALL                  1
-                          1510 CALL                     1
-                          1520 POP_TOP
-               
-                69     >> 1522 LOAD_DEREF               0 (self)
-                          1524 LOAD_ATTR               32 (ownership_status)
-                          1534 LOAD_GLOBAL             62 (ParcelOwnership)
-                          1546 LOAD_ATTR               35 (UNKNOWN)
-                          1556 COMPARE_OP               2 (==)
-                          1562 POP_JUMP_FORWARD_IF_FALSE    37 (to 1638)
-               
-                70        1564 LOAD_DEREF               0 (self)
-                          1566 LOAD_ATTR                5 (_log)
-                          1576 LOAD_METHOD             34 (debug)
-                          1598 LOAD_CONST              28 ('unexpected ownership status: ')
-                          1600 LOAD_FAST                1 (parcel_data)
-                          1602 LOAD_CONST              23 ('ownershipStatus')
-                          1604 BINARY_SUBSCR
-                          1614 FORMAT_VALUE             0
-                          1616 BUILD_STRING             2
-                          1618 PRECALL                  1
-                          1622 CALL                     1
-                          1632 POP_TOP
-                          1634 LOAD_CONST               4 (None)
-                          1636 RETURN_VALUE
+                          1300 LOAD_ATTR                4 (shipment_number)
+                          1310 FORMAT_VALUE             0
+                          1312 BUILD_STRING             2
+                          1314 PRECALL                  1
+                          1318 CALL                     1
+                          1328 POP_TOP
+               
+                61        1330 LOAD_DEREF               0 (self)
+                          1332 LOAD_ATTR                7 (shipment_type)
+                          1342 LOAD_GLOBAL             12 (ParcelShipmentType)
+                          1354 LOAD_ATTR               36 (UNKNOWN)
+                          1364 COMPARE_OP               2 (==)
+                          1370 POP_JUMP_FORWARD_IF_FALSE    35 (to 1442)
+               
+                62        1372 LOAD_DEREF               0 (self)
+                          1374 LOAD_ATTR                5 (_log)
+                          1384 LOAD_METHOD             35 (debug)
+                          1406 LOAD_CONST              27 ('unexpected shipment_type: ')
+                          1408 LOAD_FAST                1 (parcel_data)
+                          1410 LOAD_CONST               2 ('shipmentType')
+                          1412 BINARY_SUBSCR
+                          1422 FORMAT_VALUE             0
+                          1424 BUILD_STRING             2
+                          1426 PRECALL                  1
+                          1430 CALL                     1
+                          1440 POP_TOP
+               
+                64     >> 1442 LOAD_DEREF               0 (self)
+                          1444 LOAD_ATTR               17 (parcel_size)
+                          1454 LOAD_GLOBAL             32 (ParcelCarrierSize)
+                          1466 LOAD_ATTR               36 (UNKNOWN)
+                          1476 COMPARE_OP               2 (==)
+                          1482 POP_JUMP_FORWARD_IF_TRUE    21 (to 1526)
+                          1484 LOAD_DEREF               0 (self)
+                          1486 LOAD_ATTR               17 (parcel_size)
+                          1496 LOAD_GLOBAL             30 (ParcelLockerSize)
+                          1508 LOAD_ATTR               36 (UNKNOWN)
+                          1518 COMPARE_OP               2 (==)
+                          1524 POP_JUMP_FORWARD_IF_FALSE    35 (to 1596)
+               
+                65     >> 1526 LOAD_DEREF               0 (self)
+                          1528 LOAD_ATTR                5 (_log)
+                          1538 LOAD_METHOD             35 (debug)
+                          1560 LOAD_CONST              28 ('unexpected parcel_size: ')
+                          1562 LOAD_FAST                1 (parcel_data)
+                          1564 LOAD_CONST               9 ('parcelSize')
+                          1566 BINARY_SUBSCR
+                          1576 FORMAT_VALUE             0
+                          1578 BUILD_STRING             2
+                          1580 PRECALL                  1
+                          1584 CALL                     1
+                          1594 POP_TOP
+               
+                67     >> 1596 LOAD_DEREF               0 (self)
+                          1598 LOAD_ATTR               28 (status)
+                          1608 LOAD_GLOBAL             54 (ParcelStatus)
+                          1620 LOAD_ATTR               36 (UNKNOWN)
+                          1630 COMPARE_OP               2 (==)
+                          1636 POP_JUMP_FORWARD_IF_FALSE    35 (to 1708)
+               
+                68        1638 LOAD_DEREF               0 (self)
+                          1640 LOAD_ATTR                5 (_log)
+                          1650 LOAD_METHOD             35 (debug)
+                          1672 LOAD_CONST              29 ('unexpected parcel status: ')
+                          1674 LOAD_FAST                1 (parcel_data)
+                          1676 LOAD_CONST              20 ('status')
+                          1678 BINARY_SUBSCR
+                          1688 FORMAT_VALUE             0
+                          1690 BUILD_STRING             2
+                          1692 PRECALL                  1
+                          1696 CALL                     1
+                          1706 POP_TOP
+               
+                70     >> 1708 LOAD_DEREF               0 (self)
+                          1710 LOAD_ATTR               32 (ownership_status)
+                          1720 LOAD_GLOBAL             62 (ParcelOwnership)
+                          1732 LOAD_ATTR               36 (UNKNOWN)
+                          1742 COMPARE_OP               2 (==)
+                          1748 POP_JUMP_FORWARD_IF_FALSE    37 (to 1824)
+               
+                71        1750 LOAD_DEREF               0 (self)
+                          1752 LOAD_ATTR                5 (_log)
+                          1762 LOAD_METHOD             35 (debug)
+                          1784 LOAD_CONST              30 ('unexpected ownership status: ')
+                          1786 LOAD_FAST                1 (parcel_data)
+                          1788 LOAD_CONST              24 ('ownershipStatus')
+                          1790 BINARY_SUBSCR
+                          1800 FORMAT_VALUE             0
+                          1802 BUILD_STRING             2
+                          1804 PRECALL                  1
+                          1808 CALL                     1
+                          1818 POP_TOP
+                          1820 LOAD_CONST               4 (None)
+                          1822 RETURN_VALUE
                
-                69     >> 1638 LOAD_CONST               4 (None)
-                          1640 RETURN_VALUE
+                70     >> 1824 LOAD_CONST               4 (None)
+                          1826 RETURN_VALUE
                consts
                   'Constructor method'
                   '.'
                   'shipmentType'
                   'openCode'
                   None
                   'qrCode'
                   ('qrcode_data', 'logger')
                   'storedDate'
                   'pickUpDate'
                   'parcelSize'
+                  'reveiver'
                   'receiver'
                   ('receiver_data', 'logger')
                   'sender'
                   ('sender_data', 'logger')
                   'pickUpPoint'
                   ('pickuppoint_data', 'logger')
                   'multiCompartment'
                   ('logger',)
                   'endOfWeekCollection'
                   'status'
                   'avizoTransactionStatus'
+                  'sharedTo'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 6
                      flags     : 19
                      code
                         0x9501970067007c005d187d017401000000000000000000007c0189026a
@@ -1061,32 +1117,33 @@
                      varnames   ('.0', 'person')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<listcomp>'
                      firstlineno 52
                      lnotab 0x0a0102ff
-                  'sharedTo'
                   'ownershipStatus'
+                  'economyParcel'
                   'created parcel with shipment number '
                   'unexpected shipment_type: '
                   'unexpected parcel_size: '
                   'unexpected parcel status: '
                   'unexpected ownership status: '
-               names      ('super', '__init__', 'getChild', '__name__', 'shipment_number', '_log', 'ParcelShipmentType', 'shipment_type', '_open_code', 'QRCode', '_qr_code', 'get', 'stored_date', 'pickup_date', 'parcel', 'ParcelLockerSize', 'ParcelCarrierSize', 'parcel_size', 'Receiver', 'receiver', 'Sender', 'sender', 'PickupPoint', 'pickup_point', 'MultiCompartment', 'multi_compartment', 'is_end_off_week_collection', 'ParcelStatus', 'status', 'avizo_transaction_status', 'shared_to', 'ParcelOwnership', 'ownership_status', '_compartment_properties', 'debug', 'UNKNOWN')
+               names      ('super', '__init__', 'getChild', '__name__', 'shipment_number', '_log', 'ParcelShipmentType', 'shipment_type', 'get', '_open_code', 'QRCode', '_qr_code', 'stored_date', 'pickup_date', 'parcel', 'ParcelLockerSize', 'ParcelCarrierSize', 'parcel_size', 'Receiver', 'receiver', 'Sender', 'sender', 'PickupPoint', 'pickup_point', 'MultiCompartment', 'multi_compartment', 'is_end_off_week_collection', 'ParcelStatus', 'status', 'avizo_transaction_status', 'shared_to', 'ParcelOwnership', 'ownership_status', 'economy_parcel', '_compartment_properties', 'debug', 'UNKNOWN')
                varnames   ('self', 'parcel_data', 'logger')
                freevars   ('__class__',)
                cellvars   ('self',)
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
                firstlineno 31
                lnotab
-                  0x0602440152013001260208ff380102ff0c02400140022aff260124ff0c
-                  024201420208ff380102ff0c0308ff0c011aff120102ff0c021a0130011a
-                  0108010eff1c0230010e0244032a014602540146022a0146022a014aff
+                  0x0602440152013001360208ff380102ff0c02400140022aff260124ff0c
+                  024e014e0208ff380102ff0c0308ff0c011aff120102ff0c0236013c0136
+                  0208ff08010eff120102ff0c023c0136010e0244032a014602540146022a
+                  0146022a014aff
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 3
                code
                   0x9700740100000000000000000000640184007c006a0100000000000000
@@ -1094,32 +1151,32 @@
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000007d017c006a0300000000000000006a0400000000000000
                   00740b00000000000000000000740100000000000000000000740d000000
                   000000000000007c01a6010000ab010000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000a00700000000000000
                   0000000000000000000000000064026403a6020000ab0200000000000000
                   007a0000005300
-                72           0 RESUME                   0
+                73           0 RESUME                   0
                
-                73           2 LOAD_GLOBAL              1 (NULL + tuple)
-                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 73>)
+                74           2 LOAD_GLOBAL              1 (NULL + tuple)
+                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 74>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (__dict__)
                             30 LOAD_METHOD              2 (items)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (fields)
                
-                74          98 LOAD_FAST                0 (self)
+                75          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (__class__)
                            110 LOAD_ATTR                4 (__name__)
                            120 LOAD_GLOBAL             11 (NULL + str)
                            132 LOAD_GLOBAL              1 (NULL + tuple)
                            144 LOAD_GLOBAL             13 (NULL + sorted)
                            156 LOAD_FAST                1 (fields)
                            158 PRECALL                  1
@@ -1141,15 +1198,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d145c0200007d017d027c0164006b0300000000af
                         0b7c019b0064017c029b009d035600970101008c1564025300
-                      73           0 RETURN_GENERATOR
+                      74           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                20 (to 50)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (k)
                                   16 STORE_FAST               2 (v)
@@ -1175,78 +1232,78 @@
                         None
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<genexpr>'
-                     firstlineno 73
+                     firstlineno 74
                      lnotab 0x
                   "'"
                   ''
                names      ('tuple', '__dict__', 'items', '__class__', '__name__', 'str', 'sorted', 'replace')
                varnames   ('self', 'fields')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__repr__'
-               firstlineno 72
+               firstlineno 73
                lnotab 0x02016001
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 8
                flags     : 3
                code
                   0x970064017401000000000000000000007c006a010000000000000000a6
                   010000ab0100000000000000009b0064027c006a0200000000000000009b
                   0064037c006a0300000000000000009b0064047c006a0400000000000000
                   009b009d085300
-                76           0 RESUME                   0
+                77           0 RESUME                   0
                
-                77           2 LOAD_CONST               1 ('Sender: ')
+                78           2 LOAD_CONST               1 ('Sender: ')
                              4 LOAD_GLOBAL              1 (NULL + str)
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (sender)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 FORMAT_VALUE             0
                             44 LOAD_CONST               2 ('\nShipment number: ')
                
-                78          46 LOAD_FAST                0 (self)
+                79          46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                2 (shipment_number)
                
-                77          58 FORMAT_VALUE             0
+                78          58 FORMAT_VALUE             0
                             60 LOAD_CONST               3 ('\nStatus: ')
                
-                79          62 LOAD_FAST                0 (self)
+                80          62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                3 (status)
                
-                77          74 FORMAT_VALUE             0
+                78          74 FORMAT_VALUE             0
                             76 LOAD_CONST               4 ('\nPickup point: ')
                
-                80          78 LOAD_FAST                0 (self)
+                81          78 LOAD_FAST                0 (self)
                             80 LOAD_ATTR                4 (pickup_point)
                
-                77          90 FORMAT_VALUE             0
+                78          90 FORMAT_VALUE             0
                             92 BUILD_STRING             8
                             94 RETURN_VALUE
                consts
                   None
                   'Sender: '
                   '\nShipment number: '
                   '\nStatus: '
                   '\nPickup point: '
                names      ('str', 'sender', 'shipment_number', 'status', 'pickup_point')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__str__'
-               firstlineno 76
+               firstlineno 77
                lnotab 0x02012c010cff04020cfe04030cfd
             'return'
             None
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
@@ -1257,73 +1314,73 @@
                   000000000000007406000000000000000000006a0400000000000000006b
                   020000000072217c006a000000000000000000a001000000000000000000
                   00000000000000000000006402a6010000ab01000000000000000001007c
                   006a05000000000000000053007c006a000000000000000000a001000000
                   00000000000000000000000000000000006403740d000000000000000000
                   007c006a020000000000000000a6010000ab0100000000000000009b009d
                   02a6010000ab010000000000000000010064045300
-                82           0 RESUME                   0
+                83           0 RESUME                   0
                
-                88           2 LOAD_FAST                0 (self)
+                89           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('getting open code')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-                89          54 LOAD_FAST                0 (self)
+                90          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (shipment_type)
                             66 LOAD_GLOBAL              6 (ParcelShipmentType)
                             78 LOAD_ATTR                4 (parcel)
                             88 COMPARE_OP               2 (==)
                             94 POP_JUMP_FORWARD_IF_FALSE    33 (to 162)
                
-                90          96 LOAD_FAST                0 (self)
+                91          96 LOAD_FAST                0 (self)
                             98 LOAD_ATTR                0 (_log)
                            108 LOAD_METHOD              1 (debug)
                            130 LOAD_CONST               2 ('got open code')
                            132 PRECALL                  1
                            136 CALL                     1
                            146 POP_TOP
                
-                91         148 LOAD_FAST                0 (self)
+                92         148 LOAD_FAST                0 (self)
                            150 LOAD_ATTR                5 (_open_code)
                            160 RETURN_VALUE
                
-                93     >>  162 LOAD_FAST                0 (self)
+                94     >>  162 LOAD_FAST                0 (self)
                            164 LOAD_ATTR                0 (_log)
                            174 LOAD_METHOD              1 (debug)
                            196 LOAD_CONST               3 ('wrong ParcelShipmentType: ')
                            198 LOAD_GLOBAL             13 (NULL + repr)
                            210 LOAD_FAST                0 (self)
                            212 LOAD_ATTR                2 (shipment_type)
                            222 PRECALL                  1
                            226 CALL                     1
                            236 FORMAT_VALUE             0
                            238 BUILD_STRING             2
                            240 PRECALL                  1
                            244 CALL                     1
                            254 POP_TOP
                
-                94         256 LOAD_CONST               4 (None)
+                95         256 LOAD_CONST               4 (None)
                            258 RETURN_VALUE
                consts
                   'Returns an open code for :class:`Parcel`\n\n        :return: Open code for :class:`Parcel`\n        :rtype: str'
                   'getting open code'
                   'got open code'
                   'wrong ParcelShipmentType: '
                   None
                names      ('_log', 'debug', 'shipment_type', 'ParcelShipmentType', 'parcel', '_open_code', 'repr')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'open_code'
-               firstlineno 82
+               firstlineno 83
                lnotab 0x020634012a0134010e025e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
@@ -1333,74 +1390,74 @@
                   020000000072267c006a000000000000000000a001000000000000000000
                   00000000000000000000006402a6010000ab01000000000000000001007c
                   006a0500000000000000006a06000000000000000053007c006a00000000
                   0000000000a0010000000000000000000000000000000000000000640374
                   0f000000000000000000007c006a020000000000000000a6010000ab0100
                   000000000000009b009d02a6010000ab0100000000000000000100640453
                   00
-                96           0 RESUME                   0
+                97           0 RESUME                   0
                
-               102           2 LOAD_FAST                0 (self)
+               103           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('generating qr image')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               103          54 LOAD_FAST                0 (self)
+               104          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (shipment_type)
                             66 LOAD_GLOBAL              6 (ParcelShipmentType)
                             78 LOAD_ATTR                4 (parcel)
                             88 COMPARE_OP               2 (==)
                             94 POP_JUMP_FORWARD_IF_FALSE    38 (to 172)
                
-               104          96 LOAD_FAST                0 (self)
+               105          96 LOAD_FAST                0 (self)
                             98 LOAD_ATTR                0 (_log)
                            108 LOAD_METHOD              1 (debug)
                            130 LOAD_CONST               2 ('got qr image')
                            132 PRECALL                  1
                            136 CALL                     1
                            146 POP_TOP
                
-               105         148 LOAD_FAST                0 (self)
+               106         148 LOAD_FAST                0 (self)
                            150 LOAD_ATTR                5 (_qr_code)
                            160 LOAD_ATTR                6 (qr_image)
                            170 RETURN_VALUE
                
-               107     >>  172 LOAD_FAST                0 (self)
+               108     >>  172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                0 (_log)
                            184 LOAD_METHOD              1 (debug)
                            206 LOAD_CONST               3 ('wrong ParcelShipmentType: ')
                            208 LOAD_GLOBAL             15 (NULL + repr)
                            220 LOAD_FAST                0 (self)
                            222 LOAD_ATTR                2 (shipment_type)
                            232 PRECALL                  1
                            236 CALL                     1
                            246 FORMAT_VALUE             0
                            248 BUILD_STRING             2
                            250 PRECALL                  1
                            254 CALL                     1
                            264 POP_TOP
                
-               108         266 LOAD_CONST               4 (None)
+               109         266 LOAD_CONST               4 (None)
                            268 RETURN_VALUE
                consts
                   'Returns a QR image for :class:`Parcel`\n\n        :return: QR image for :class:`Parcel`\n        :rtype: BytesIO'
                   'generating qr image'
                   'got qr image'
                   'wrong ParcelShipmentType: '
                   None
                names      ('_log', 'debug', 'shipment_type', 'ParcelShipmentType', 'parcel', '_qr_code', 'qr_image', 'repr')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'generate_qr_image'
-               firstlineno 96
+               firstlineno 97
                lnotab 0x020634012a01340118025e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
@@ -1409,73 +1466,73 @@
                   000000000000007406000000000000000000006a0400000000000000006b
                   020000000072217c006a000000000000000000a001000000000000000000
                   00000000000000000000006402a6010000ab01000000000000000001007c
                   006a05000000000000000053007c006a000000000000000000a001000000
                   00000000000000000000000000000000006403740d000000000000000000
                   007c006a020000000000000000a6010000ab0100000000000000009b009d
                   02a6010000ab010000000000000000010064045300
-               110           0 RESUME                   0
+               111           0 RESUME                   0
                
-               116           2 LOAD_FAST                0 (self)
+               117           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('getting comparment properties')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               117          54 LOAD_FAST                0 (self)
+               118          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (shipment_type)
                             66 LOAD_GLOBAL              6 (ParcelShipmentType)
                             78 LOAD_ATTR                4 (parcel)
                             88 COMPARE_OP               2 (==)
                             94 POP_JUMP_FORWARD_IF_FALSE    33 (to 162)
                
-               118          96 LOAD_FAST                0 (self)
+               119          96 LOAD_FAST                0 (self)
                             98 LOAD_ATTR                0 (_log)
                            108 LOAD_METHOD              1 (debug)
                            130 LOAD_CONST               2 ('got compartment properties')
                            132 PRECALL                  1
                            136 CALL                     1
                            146 POP_TOP
                
-               119         148 LOAD_FAST                0 (self)
+               120         148 LOAD_FAST                0 (self)
                            150 LOAD_ATTR                5 (_compartment_properties)
                            160 RETURN_VALUE
                
-               121     >>  162 LOAD_FAST                0 (self)
+               122     >>  162 LOAD_FAST                0 (self)
                            164 LOAD_ATTR                0 (_log)
                            174 LOAD_METHOD              1 (debug)
                            196 LOAD_CONST               3 ('wrong ParcelShipmentType: ')
                            198 LOAD_GLOBAL             13 (NULL + repr)
                            210 LOAD_FAST                0 (self)
                            212 LOAD_ATTR                2 (shipment_type)
                            222 PRECALL                  1
                            226 CALL                     1
                            236 FORMAT_VALUE             0
                            238 BUILD_STRING             2
                            240 PRECALL                  1
                            244 CALL                     1
                            254 POP_TOP
                
-               122         256 LOAD_CONST               4 (None)
+               123         256 LOAD_CONST               4 (None)
                            258 RETURN_VALUE
                consts
                   'Returns a compartment properties for :class:`Parcel`\n\n        :return: Compartment properties for :class:`Parcel`\n        :rtype: CompartmentProperties'
                   'getting comparment properties'
                   'got compartment properties'
                   'wrong ParcelShipmentType: '
                   None
                names      ('_log', 'debug', 'shipment_type', 'ParcelShipmentType', 'parcel', '_compartment_properties', 'repr')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'compartment_properties'
-               firstlineno 110
+               firstlineno 111
                lnotab 0x020634012a0134010e025e01
             'compartmentproperties_data'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
@@ -1487,55 +1544,55 @@
                   00000000000000000000000000000000006402a6010000ab010000000000
                   0000000100740b000000000000000000007c017c006a0000000000000000
                   00ac03a6020000ab0200000000000000007c005f0600000000000000007c
                   006a000000000000000000a0010000000000000000000000000000000000
                   0000006404740f000000000000000000007c006a020000000000000000a6
                   010000ab0100000000000000009b009d02a6010000ab0100000000000000
                   00010064055300
-               124           0 RESUME                   0
+               125           0 RESUME                   0
                
-               130           2 LOAD_FAST                0 (self)
+               131           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('setting compartment properties with ')
                             38 LOAD_FAST                1 (compartmentproperties_data)
                             40 FORMAT_VALUE             0
                             42 BUILD_STRING             2
                             44 PRECALL                  1
                             48 CALL                     1
                             58 POP_TOP
                
-               131          60 LOAD_FAST                0 (self)
+               132          60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                2 (shipment_type)
                             72 LOAD_GLOBAL              6 (ParcelShipmentType)
                             84 LOAD_ATTR                4 (parcel)
                             94 COMPARE_OP               2 (==)
                            100 POP_JUMP_FORWARD_IF_FALSE    53 (to 208)
                
-               132         102 LOAD_FAST                0 (self)
+               133         102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (_log)
                            114 LOAD_METHOD              1 (debug)
                            136 LOAD_CONST               2 ('compartment properties set')
                            138 PRECALL                  1
                            142 CALL                     1
                            152 POP_TOP
                
-               133         154 LOAD_GLOBAL             11 (NULL + CompartmentProperties)
+               134         154 LOAD_GLOBAL             11 (NULL + CompartmentProperties)
                            166 LOAD_FAST                1 (compartmentproperties_data)
                
-               134         168 LOAD_FAST                0 (self)
+               135         168 LOAD_FAST                0 (self)
                            170 LOAD_ATTR                0 (_log)
                
-               133         180 KW_NAMES                 3
+               134         180 KW_NAMES                 3
                            182 PRECALL                  2
                            186 CALL                     2
                            196 LOAD_FAST                0 (self)
                            198 STORE_ATTR               6 (_compartment_properties)
                
-               136     >>  208 LOAD_FAST                0 (self)
+               137     >>  208 LOAD_FAST                0 (self)
                            210 LOAD_ATTR                0 (_log)
                            220 LOAD_METHOD              1 (debug)
                            242 LOAD_CONST               4 ('wrong ParcelShipmentType: ')
                            244 LOAD_GLOBAL             15 (NULL + repr)
                            256 LOAD_FAST                0 (self)
                            258 LOAD_ATTR                2 (shipment_type)
                            268 PRECALL                  1
@@ -1556,15 +1613,15 @@
                   None
                names      ('_log', 'debug', 'shipment_type', 'ParcelShipmentType', 'parcel', 'CompartmentProperties', '_compartment_properties', 'repr')
                varnames   ('self', 'compartmentproperties_data')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'compartment_properties'
-               firstlineno 124
+               firstlineno 125
                lnotab 0x02063a012a0134010e010cff1c03
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
@@ -1574,79 +1631,79 @@
                   0200000000722f7c006a000000000000000000a001000000000000000000
                   00000000000000000000006402a6010000ab01000000000000000001007c
                   006a050000000000000000720c7c006a0500000000000000006a06000000
                   00000000006e01640353007c006a000000000000000000a0010000000000
                   0000000000000000000000000000006404740f000000000000000000007c
                   006a020000000000000000a6010000ab0100000000000000009b009d02a6
                   010000ab010000000000000000010064035300
-               138           0 RESUME                   0
+               139           0 RESUME                   0
                
-               144           2 LOAD_FAST                0 (self)
+               145           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('getting compartment location')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               145          54 LOAD_FAST                0 (self)
+               146          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (shipment_type)
                             66 LOAD_GLOBAL              6 (ParcelShipmentType)
                             78 LOAD_ATTR                4 (parcel)
                             88 COMPARE_OP               2 (==)
                             94 POP_JUMP_FORWARD_IF_FALSE    47 (to 190)
                
-               146          96 LOAD_FAST                0 (self)
+               147          96 LOAD_FAST                0 (self)
                             98 LOAD_ATTR                0 (_log)
                            108 LOAD_METHOD              1 (debug)
                            130 LOAD_CONST               2 ('got compartment location')
                            132 PRECALL                  1
                            136 CALL                     1
                            146 POP_TOP
                
-               147         148 LOAD_FAST                0 (self)
+               148         148 LOAD_FAST                0 (self)
                            150 LOAD_ATTR                5 (_compartment_properties)
                            160 POP_JUMP_FORWARD_IF_FALSE    12 (to 186)
                            162 LOAD_FAST                0 (self)
                            164 LOAD_ATTR                5 (_compartment_properties)
                            174 LOAD_ATTR                6 (location)
                            184 JUMP_FORWARD             1 (to 188)
                        >>  186 LOAD_CONST               3 (None)
                        >>  188 RETURN_VALUE
                
-               149     >>  190 LOAD_FAST                0 (self)
+               150     >>  190 LOAD_FAST                0 (self)
                            192 LOAD_ATTR                0 (_log)
                            202 LOAD_METHOD              1 (debug)
                            224 LOAD_CONST               4 ('wrong ParcelShipmentType: ')
                            226 LOAD_GLOBAL             15 (NULL + repr)
                            238 LOAD_FAST                0 (self)
                            240 LOAD_ATTR                2 (shipment_type)
                            250 PRECALL                  1
                            254 CALL                     1
                            264 FORMAT_VALUE             0
                            266 BUILD_STRING             2
                            268 PRECALL                  1
                            272 CALL                     1
                            282 POP_TOP
                
-               150         284 LOAD_CONST               3 (None)
+               151         284 LOAD_CONST               3 (None)
                            286 RETURN_VALUE
                consts
                   'Returns a compartment location for :class:`Parcel`\n\n        :return: Compartment location for :class:`Parcel`\n        :rtype: CompartmentLocation'
                   'getting compartment location'
                   'got compartment location'
                   None
                   'wrong ParcelShipmentType: '
                names      ('_log', 'debug', 'shipment_type', 'ParcelShipmentType', 'parcel', '_compartment_properties', 'location', 'repr')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'compartment_location'
-               firstlineno 138
+               firstlineno 139
                lnotab 0x020634012a0134012a025e01
             'location_data'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
@@ -1657,48 +1714,48 @@
                   00000000006b020000000072267c006a000000000000000000a001000000
                   00000000000000000000000000000000006402a6010000ab010000000000
                   00000001007c017c006a0500000000000000005f0600000000000000007c
                   006a000000000000000000a0010000000000000000000000000000000000
                   0000006403740f000000000000000000007c006a020000000000000000a6
                   010000ab0100000000000000009b009d02a6010000ab0100000000000000
                   00010064045300
-               152           0 RESUME                   0
+               153           0 RESUME                   0
                
-               157           2 LOAD_FAST                0 (self)
+               158           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('setting compartment location with ')
                             38 LOAD_FAST                1 (location_data)
                             40 FORMAT_VALUE             0
                             42 BUILD_STRING             2
                             44 PRECALL                  1
                             48 CALL                     1
                             58 POP_TOP
                
-               158          60 LOAD_FAST                0 (self)
+               159          60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                2 (shipment_type)
                             72 LOAD_GLOBAL              6 (ParcelShipmentType)
                             84 LOAD_ATTR                4 (parcel)
                             94 COMPARE_OP               2 (==)
                            100 POP_JUMP_FORWARD_IF_FALSE    38 (to 178)
                
-               159         102 LOAD_FAST                0 (self)
+               160         102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (_log)
                            114 LOAD_METHOD              1 (debug)
                            136 LOAD_CONST               2 ('compartment location set')
                            138 PRECALL                  1
                            142 CALL                     1
                            152 POP_TOP
                
-               160         154 LOAD_FAST                1 (location_data)
+               161         154 LOAD_FAST                1 (location_data)
                            156 LOAD_FAST                0 (self)
                            158 LOAD_ATTR                5 (_compartment_properties)
                            168 STORE_ATTR               6 (location)
                
-               162     >>  178 LOAD_FAST                0 (self)
+               163     >>  178 LOAD_FAST                0 (self)
                            180 LOAD_ATTR                0 (_log)
                            190 LOAD_METHOD              1 (debug)
                            212 LOAD_CONST               3 ('wrong ParcelShipmentType: ')
                            214 LOAD_GLOBAL             15 (NULL + repr)
                            226 LOAD_FAST                0 (self)
                            228 LOAD_ATTR                2 (shipment_type)
                            238 PRECALL                  1
@@ -1718,15 +1775,15 @@
                   None
                names      ('_log', 'debug', 'shipment_type', 'ParcelShipmentType', 'parcel', '_compartment_properties', 'location', 'repr')
                varnames   ('self', 'location_data')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'compartment_location'
-               firstlineno 152
+               firstlineno 153
                lnotab 0x02053a012a0134011802
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
@@ -1736,79 +1793,79 @@
                   0200000000722f7c006a000000000000000000a001000000000000000000
                   00000000000000000000006402a6010000ab01000000000000000001007c
                   006a050000000000000000720c7c006a0500000000000000006a06000000
                   00000000006e01640353007c006a000000000000000000a0010000000000
                   0000000000000000000000000000006404740f000000000000000000007c
                   006a020000000000000000a6010000ab0100000000000000009b009d02a6
                   010000ab010000000000000000010064035300
-               164           0 RESUME                   0
+               165           0 RESUME                   0
                
-               170           2 LOAD_FAST                0 (self)
+               171           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('getting compartment status')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               172          54 LOAD_FAST                0 (self)
+               173          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (shipment_type)
                             66 LOAD_GLOBAL              6 (ParcelShipmentType)
                             78 LOAD_ATTR                4 (parcel)
                             88 COMPARE_OP               2 (==)
                             94 POP_JUMP_FORWARD_IF_FALSE    47 (to 190)
                
-               173          96 LOAD_FAST                0 (self)
+               174          96 LOAD_FAST                0 (self)
                             98 LOAD_ATTR                0 (_log)
                            108 LOAD_METHOD              1 (debug)
                            130 LOAD_CONST               2 ('got compartment status')
                            132 PRECALL                  1
                            136 CALL                     1
                            146 POP_TOP
                
-               174         148 LOAD_FAST                0 (self)
+               175         148 LOAD_FAST                0 (self)
                            150 LOAD_ATTR                5 (_compartment_properties)
                            160 POP_JUMP_FORWARD_IF_FALSE    12 (to 186)
                            162 LOAD_FAST                0 (self)
                            164 LOAD_ATTR                5 (_compartment_properties)
                            174 LOAD_ATTR                6 (status)
                            184 JUMP_FORWARD             1 (to 188)
                        >>  186 LOAD_CONST               3 (None)
                        >>  188 RETURN_VALUE
                
-               176     >>  190 LOAD_FAST                0 (self)
+               177     >>  190 LOAD_FAST                0 (self)
                            192 LOAD_ATTR                0 (_log)
                            202 LOAD_METHOD              1 (debug)
                            224 LOAD_CONST               4 ('wrong ParcelShipmentType: ')
                            226 LOAD_GLOBAL             15 (NULL + repr)
                            238 LOAD_FAST                0 (self)
                            240 LOAD_ATTR                2 (shipment_type)
                            250 PRECALL                  1
                            254 CALL                     1
                            264 FORMAT_VALUE             0
                            266 BUILD_STRING             2
                            268 PRECALL                  1
                            272 CALL                     1
                            282 POP_TOP
                
-               177         284 LOAD_CONST               3 (None)
+               178         284 LOAD_CONST               3 (None)
                            286 RETURN_VALUE
                consts
                   'Returns a compartment status for :class:`Parcel`\n\n        :return: Compartment status for :class:`Parcel`\n        :rtype: CompartmentActualStatus'
                   'getting compartment status'
                   'got compartment status'
                   None
                   'wrong ParcelShipmentType: '
                names      ('_log', 'debug', 'shipment_type', 'ParcelShipmentType', 'parcel', '_compartment_properties', 'status', 'repr')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'compartment_status'
-               firstlineno 164
+               firstlineno 165
                lnotab 0x020634022a0134012a025e01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
@@ -1818,48 +1875,48 @@
                   00000000006b020000000072267c006a000000000000000000a001000000
                   00000000000000000000000000000000006402a6010000ab010000000000
                   00000001007c017c006a0500000000000000005f0600000000000000007c
                   006a000000000000000000a0010000000000000000000000000000000000
                   0000006403740f000000000000000000007c006a020000000000000000a6
                   010000ab0100000000000000009b009d02a6010000ab0100000000000000
                   00010064005300
-               179           0 RESUME                   0
+               180           0 RESUME                   0
                
-               181           2 LOAD_FAST                0 (self)
+               182           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('setting compartment status with ')
                             38 LOAD_FAST                1 (status)
                             40 FORMAT_VALUE             0
                             42 BUILD_STRING             2
                             44 PRECALL                  1
                             48 CALL                     1
                             58 POP_TOP
                
-               182          60 LOAD_FAST                0 (self)
+               183          60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                2 (shipment_type)
                             72 LOAD_GLOBAL              6 (ParcelShipmentType)
                             84 LOAD_ATTR                4 (parcel)
                             94 COMPARE_OP               2 (==)
                            100 POP_JUMP_FORWARD_IF_FALSE    38 (to 178)
                
-               183         102 LOAD_FAST                0 (self)
+               184         102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                0 (_log)
                            114 LOAD_METHOD              1 (debug)
                            136 LOAD_CONST               2 ('compartment status set')
                            138 PRECALL                  1
                            142 CALL                     1
                            152 POP_TOP
                
-               184         154 LOAD_FAST                1 (status)
+               185         154 LOAD_FAST                1 (status)
                            156 LOAD_FAST                0 (self)
                            158 LOAD_ATTR                5 (_compartment_properties)
                            168 STORE_ATTR               6 (status)
                
-               186     >>  178 LOAD_FAST                0 (self)
+               187     >>  178 LOAD_FAST                0 (self)
                            180 LOAD_ATTR                0 (_log)
                            190 LOAD_METHOD              1 (debug)
                            212 LOAD_CONST               3 ('wrong ParcelShipmentType: ')
                            214 LOAD_GLOBAL             15 (NULL + repr)
                            226 LOAD_FAST                0 (self)
                            228 LOAD_ATTR                2 (shipment_type)
                            238 PRECALL                  1
@@ -1878,15 +1935,15 @@
                   'wrong ParcelShipmentType: '
                names      ('_log', 'debug', 'shipment_type', 'ParcelShipmentType', 'parcel', '_compartment_properties', 'status', 'repr')
                varnames   ('self', 'status')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'compartment_status'
-               firstlineno 179
+               firstlineno 180
                lnotab 0x02023a012a0134011802
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
@@ -1896,84 +1953,84 @@
                   020000000072347c006a000000000000000000a001000000000000000000
                   00000000000000000000006402a6010000ab01000000000000000001007c
                   006a0500000000000000007c006a0600000000000000007c006a07000000
                   00000000006a08000000000000000064039c0353007c006a000000000000
                   000000a00100000000000000000000000000000000000000006404741300
                   0000000000000000007c006a020000000000000000a6010000ab01000000
                   00000000009b009d02a6010000ab010000000000000000010064055300
-               188           0 RESUME                   0
+               189           0 RESUME                   0
                
-               194           2 LOAD_FAST                0 (self)
+               195           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('getting compartment open data')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               195          54 LOAD_FAST                0 (self)
+               196          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (shipment_type)
                             66 LOAD_GLOBAL              6 (ParcelShipmentType)
                             78 LOAD_ATTR                4 (parcel)
                             88 COMPARE_OP               2 (==)
                             94 POP_JUMP_FORWARD_IF_FALSE    52 (to 200)
                
-               196          96 LOAD_FAST                0 (self)
+               197          96 LOAD_FAST                0 (self)
                             98 LOAD_ATTR                0 (_log)
                            108 LOAD_METHOD              1 (debug)
                            130 LOAD_CONST               2 ('got compartment open data')
                            132 PRECALL                  1
                            136 CALL                     1
                            146 POP_TOP
                
-               198         148 LOAD_FAST                0 (self)
+               199         148 LOAD_FAST                0 (self)
                            150 LOAD_ATTR                5 (shipment_number)
                
-               199         160 LOAD_FAST                0 (self)
+               200         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                6 (_open_code)
                
-               200         172 LOAD_FAST                0 (self)
+               201         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                7 (receiver)
                            184 LOAD_ATTR                8 (phone_number)
                
-               197         194 LOAD_CONST               3 (('shipmentNumber', 'openCode', 'receiverPhoneNumber'))
+               198         194 LOAD_CONST               3 (('shipmentNumber', 'openCode', 'receiverPhoneNumber'))
                            196 BUILD_CONST_KEY_MAP      3
                            198 RETURN_VALUE
                
-               203     >>  200 LOAD_FAST                0 (self)
+               204     >>  200 LOAD_FAST                0 (self)
                            202 LOAD_ATTR                0 (_log)
                            212 LOAD_METHOD              1 (debug)
                            234 LOAD_CONST               4 ('wrong ParcelShipmentType: ')
                            236 LOAD_GLOBAL             19 (NULL + repr)
                            248 LOAD_FAST                0 (self)
                            250 LOAD_ATTR                2 (shipment_type)
                            260 PRECALL                  1
                            264 CALL                     1
                            274 FORMAT_VALUE             0
                            276 BUILD_STRING             2
                            278 PRECALL                  1
                            282 CALL                     1
                            292 POP_TOP
                
-               204         294 LOAD_CONST               5 (None)
+               205         294 LOAD_CONST               5 (None)
                            296 RETURN_VALUE
                consts
                   'Returns a compartment open data for :class:`Parcel`\n\n        :return: dict containing compartment open data for :class:`Parcel`\n        :rtype: dict'
                   'getting compartment open data'
                   'got compartment open data'
                   ('shipmentNumber', 'openCode', 'receiverPhoneNumber')
                   'wrong ParcelShipmentType: '
                   None
                names      ('_log', 'debug', 'shipment_type', 'ParcelShipmentType', 'parcel', 'shipment_number', '_open_code', 'receiver', 'phone_number', 'repr')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'compartment_open_data'
-               firstlineno 188
+               firstlineno 189
                lnotab 0x020634012a0134020c010c0116fd06065e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 8
                flags     : 3
                code
@@ -1990,100 +2047,100 @@
                   036404a6020000ab0200000000000000007a0000006405a6020000ab0200
                   00000000000000740b000000000000000000007411000000000000000000
                   006a09000000000000000064066407a6020000ab02000000000000000064
                   06a6020000ab02000000000000000064089c0353007c006a000000000000
                   000000a00100000000000000000000000000000000000000006409741700
                   0000000000000000007c006a020000000000000000a6010000ab01000000
                   00000000009b009d02a6010000ab0100000000000000000100640a5300
-               206           0 RESUME                   0
+               207           0 RESUME                   0
                
-               212           2 LOAD_FAST                0 (self)
+               213           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('getting mocked location')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               213          54 LOAD_FAST                0 (self)
+               214          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (shipment_type)
                             66 LOAD_GLOBAL              6 (ParcelShipmentType)
                             78 LOAD_ATTR                4 (parcel)
                             88 COMPARE_OP               2 (==)
                             94 POP_JUMP_FORWARD_IF_FALSE   157 (to 410)
                
-               214          96 LOAD_FAST                0 (self)
+               215          96 LOAD_FAST                0 (self)
                             98 LOAD_ATTR                0 (_log)
                            108 LOAD_METHOD              1 (debug)
                            130 LOAD_CONST               2 ('got mocked location')
                            132 PRECALL                  1
                            136 CALL                     1
                            146 POP_TOP
                
-               216         148 LOAD_GLOBAL             11 (NULL + round)
+               217         148 LOAD_GLOBAL             11 (NULL + round)
                            160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                6 (pickup_point)
                            172 LOAD_ATTR                7 (latitude)
                            182 LOAD_GLOBAL             17 (NULL + random)
                            194 LOAD_ATTR                9 (uniform)
                            204 LOAD_CONST               3 (-5e-05)
                            206 LOAD_CONST               4 (5e-05)
                            208 PRECALL                  2
                            212 CALL                     2
                            222 BINARY_OP                0 (+)
                            226 LOAD_CONST               5 (6)
                            228 PRECALL                  2
                            232 CALL                     2
                
-               217         242 LOAD_GLOBAL             11 (NULL + round)
+               218         242 LOAD_GLOBAL             11 (NULL + round)
                            254 LOAD_FAST                0 (self)
                            256 LOAD_ATTR                6 (pickup_point)
                            266 LOAD_ATTR               10 (longitude)
                            276 LOAD_GLOBAL             17 (NULL + random)
                            288 LOAD_ATTR                9 (uniform)
                            298 LOAD_CONST               3 (-5e-05)
                            300 LOAD_CONST               4 (5e-05)
                            302 PRECALL                  2
                            306 CALL                     2
                            316 BINARY_OP                0 (+)
                            320 LOAD_CONST               5 (6)
                            322 PRECALL                  2
                            326 CALL                     2
                
-               218         336 LOAD_GLOBAL             11 (NULL + round)
+               219         336 LOAD_GLOBAL             11 (NULL + round)
                            348 LOAD_GLOBAL             17 (NULL + random)
                            360 LOAD_ATTR                9 (uniform)
                            370 LOAD_CONST               6 (1)
                            372 LOAD_CONST               7 (4)
                            374 PRECALL                  2
                            378 CALL                     2
                            388 LOAD_CONST               6 (1)
                            390 PRECALL                  2
                            394 CALL                     2
                
-               215         404 LOAD_CONST               8 (('latitude', 'longitude', 'accuracy'))
+               216         404 LOAD_CONST               8 (('latitude', 'longitude', 'accuracy'))
                            406 BUILD_CONST_KEY_MAP      3
                            408 RETURN_VALUE
                
-               221     >>  410 LOAD_FAST                0 (self)
+               222     >>  410 LOAD_FAST                0 (self)
                            412 LOAD_ATTR                0 (_log)
                            422 LOAD_METHOD              1 (debug)
                            444 LOAD_CONST               9 ('wrong ParcelShipmentType: ')
                            446 LOAD_GLOBAL             23 (NULL + repr)
                            458 LOAD_FAST                0 (self)
                            460 LOAD_ATTR                2 (shipment_type)
                            470 PRECALL                  1
                            474 CALL                     1
                            484 FORMAT_VALUE             0
                            486 BUILD_STRING             2
                            488 PRECALL                  1
                            492 CALL                     1
                            502 POP_TOP
                
-               222         504 LOAD_CONST              10 (None)
+               223         504 LOAD_CONST              10 (None)
                            506 RETURN_VALUE
                consts
                   'Returns a mocked location for :class:`Parcel`\n\n        :return: dict containing mocked location for :class:`Parcel`\n        :rtype: dict'
                   'getting mocked location'
                   'got mocked location'
                   -5e-05
                   5e-05
@@ -2095,112 +2152,112 @@
                   None
                names      ('_log', 'debug', 'shipment_type', 'ParcelShipmentType', 'parcel', 'round', 'pickup_point', 'latitude', 'random', 'uniform', 'longitude', 'repr')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'mocked_location'
-               firstlineno 206
+               firstlineno 207
                lnotab 0x020634012a0134025e015e0144fd06065e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code 0x97007c006a000000000000000000640175015300
-               224           0 RESUME                   0
+               225           0 RESUME                   0
                
-               229           2 LOAD_FAST                0 (self)
+               230           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (multi_compartment)
                             14 LOAD_CONST               1 (None)
                             16 IS_OP                    1
                             18 RETURN_VALUE
                consts
                   'Specifies if parcel is in multi compartment\n        :return: True if parcel is in multicompartment\n        :rtype: bool'
                   None
                names      ('multi_compartment',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'is_multicompartment'
-               firstlineno 224
+               firstlineno 225
                lnotab 0x0205
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000720e7c006a0100000000000000006a
                   02000000000000000064017501530064015300
-               231           0 RESUME                   0
+               232           0 RESUME                   0
                
-               236           2 LOAD_FAST                0 (self)
+               237           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (is_multicompartment)
                             14 POP_JUMP_FORWARD_IF_FALSE    14 (to 44)
                
-               237          16 LOAD_FAST                0 (self)
+               238          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (multi_compartment)
                             28 LOAD_ATTR                2 (shipment_numbers)
                             38 LOAD_CONST               1 (None)
                             40 IS_OP                    1
                             42 RETURN_VALUE
                
-               239     >>   44 LOAD_CONST               1 (None)
+               240     >>   44 LOAD_CONST               1 (None)
                             46 RETURN_VALUE
                consts
                   'Specifies if parcel is main parcel in multi compartment\n        :return: True if parcel is in multicompartment\n        :rtype: bool'
                   None
                names      ('is_multicompartment', 'multi_compartment', 'shipment_numbers')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'is_main_multicompartment'
-               firstlineno 231
+               firstlineno 232
                lnotab 0x02050e011c02
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'dict', 'logging', 'Logger', '__init__', '__repr__', '__str__', 'property', 'str', 'open_code', 'BytesIO', 'generate_qr_image', 'compartment_properties', 'setter', 'compartment_location', 'CompartmentActualStatus', 'compartment_status', 'compartment_open_data', 'mocked_location', 'is_multicompartment', 'is_main_multicompartment', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'Parcel'
          firstlineno 23
          lnotab
-            0x0c0104071e2906040606020110ff0e01020d020110ff0e01020d020104
+            0x0c0104071e2a06040606020110ff0e01020d020110ff0e01020d020104
             ff0e01020d0c010aff0e01020d020104ff0e01020d0c010aff0e01020b02
             0110ff0e01020e0c0104ff0e010208020104ff0e010211020104ff0e0102
             11020104ff0e010206020104ff0e01
       'Parcel'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a0264016503640265046a0500000000000000
             006604880066016403840c5a06880078015a075300
                        0 MAKE_CELL                0 (__class__)
          
-         246           2 RESUME                   0
+         247           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('ReturnParcel')
                       10 STORE_NAME               2 (__qualname__)
          
-         247          12 LOAD_CONST               1 ('parcel_data')
+         248          12 LOAD_CONST               1 ('parcel_data')
                       14 LOAD_NAME                3 (dict)
                       16 LOAD_CONST               2 ('logger')
                       18 LOAD_NAME                4 (logging)
                       20 LOAD_ATTR                5 (Logger)
                       30 BUILD_TUPLE              4
                       32 LOAD_CLOSURE             0 (__class__)
                       34 BUILD_TUPLE              1
-                      36 LOAD_CONST               3 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 247>)
+                      36 LOAD_CONST               3 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 248>)
                       38 MAKE_FUNCTION           12 (annotations, closure)
                       40 STORE_NAME               6 (__init__)
                       42 LOAD_CLOSURE             0 (__class__)
                       44 COPY                     1
                       46 STORE_NAME               7 (__classcell__)
                       48 RETURN_VALUE
          consts
@@ -2223,81 +2280,81 @@
                   000000000000007c005f0700000000000000007c01640719000000000000
                   0000007c005f0800000000000000007c016408190000000000000000007c
                   005f0900000000000000007c016409190000000000000000007c005f0a00
                   000000000000007c01640a190000000000000000007c005f0b0000000000
                   00000064005300
                              0 COPY_FREE_VARS           1
                
-               247           2 RESUME                   0
+               248           2 RESUME                   0
                
-               248           4 LOAD_GLOBAL              1 (NULL + super)
+               249           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (__init__)
                             52 LOAD_FAST                1 (parcel_data)
                             54 LOAD_FAST                2 (logger)
                             56 PRECALL                  2
                             60 CALL                     2
                             70 POP_TOP
                
-               249          72 LOAD_FAST                1 (parcel_data)
+               250          72 LOAD_FAST                1 (parcel_data)
                             74 LOAD_CONST               1 ('uuid')
                             76 BINARY_SUBSCR
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               2 (uuid)
                
-               250          98 LOAD_FAST                1 (parcel_data)
+               251          98 LOAD_FAST                1 (parcel_data)
                            100 LOAD_CONST               2 ('rma')
                            102 BINARY_SUBSCR
                            112 LOAD_FAST                0 (self)
                            114 STORE_ATTR               3 (rma)
                
-               251         124 LOAD_FAST                1 (parcel_data)
+               252         124 LOAD_FAST                1 (parcel_data)
                            126 LOAD_CONST               3 ('organizationName')
                            128 BINARY_SUBSCR
                            138 LOAD_FAST                0 (self)
                            140 STORE_ATTR               4 (organization_name)
                
-               252         150 LOAD_FAST                1 (parcel_data)
+               253         150 LOAD_FAST                1 (parcel_data)
                            152 LOAD_CONST               4 ('createdDate')
                            154 BINARY_SUBSCR
                            164 LOAD_FAST                0 (self)
                            166 STORE_ATTR               5 (created_date)
                
-               253         176 LOAD_FAST                1 (parcel_data)
+               254         176 LOAD_FAST                1 (parcel_data)
                            178 LOAD_CONST               5 ('acceptedDate')
                            180 BINARY_SUBSCR
                            190 LOAD_FAST                0 (self)
                            192 STORE_ATTR               6 (accepted_date)
                
-               254         202 LOAD_FAST                1 (parcel_data)
+               255         202 LOAD_FAST                1 (parcel_data)
                            204 LOAD_CONST               6 ('expiryDate')
                            206 BINARY_SUBSCR
                            216 LOAD_FAST                0 (self)
                            218 STORE_ATTR               7 (expiry_date)
                
-               255         228 LOAD_FAST                1 (parcel_data)
+               256         228 LOAD_FAST                1 (parcel_data)
                            230 LOAD_CONST               7 ('sentDate')
                            232 BINARY_SUBSCR
                            242 LOAD_FAST                0 (self)
                            244 STORE_ATTR               8 (sent_date)
                
-               256         254 LOAD_FAST                1 (parcel_data)
+               257         254 LOAD_FAST                1 (parcel_data)
                            256 LOAD_CONST               8 ('deliveredDate')
                            258 BINARY_SUBSCR
                            268 LOAD_FAST                0 (self)
                            270 STORE_ATTR               9 (delivered_date)
                
-               257         280 LOAD_FAST                1 (parcel_data)
+               258         280 LOAD_FAST                1 (parcel_data)
                            282 LOAD_CONST               9 ('orderNumber')
                            284 BINARY_SUBSCR
                            294 LOAD_FAST                0 (self)
                            296 STORE_ATTR              10 (order_number)
                
-               258         306 LOAD_FAST                1 (parcel_data)
+               259         306 LOAD_FAST                1 (parcel_data)
                            308 LOAD_CONST              10 ('formType')
                            310 BINARY_SUBSCR
                            320 LOAD_FAST                0 (self)
                            322 STORE_ATTR              11 (form_type)
                            332 LOAD_CONST               0 (None)
                            334 RETURN_VALUE
                consts
@@ -2314,58 +2371,58 @@
                   'formType'
                names      ('super', '__init__', 'uuid', 'rma', 'organization_name', 'created_date', 'accepted_date', 'expiry_date', 'sent_date', 'delivered_date', 'order_number', 'form_type')
                varnames   ('self', 'parcel_data', 'logger')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
-               firstlineno 247
+               firstlineno 248
                lnotab 0x040144011a011a011a011a011a011a011a011a011a01
          names      ('__name__', '__module__', '__qualname__', 'dict', 'logging', 'Logger', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'ReturnParcel'
-         firstlineno 246
+         firstlineno 247
          lnotab 0x0c01
       'ReturnParcel'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504640365056a06000000
             00000000006604880066016404840c5a07640584005a08880078015a0953
             00
                        0 MAKE_CELL                0 (__class__)
          
-         261           2 RESUME                   0
+         262           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Receiver')
                       10 STORE_NAME               2 (__qualname__)
          
-         262          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` receiver\n\n    :param receiver_data: :class:`dict` containing sender data for :class:`Parcel`\n    :type receiver_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
+         263          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` receiver\n\n    :param receiver_data: :class:`dict` containing sender data for :class:`Parcel`\n    :type receiver_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
                       14 STORE_NAME               3 (__doc__)
          
-         269          16 LOAD_CONST               2 ('receiver_data')
+         270          16 LOAD_CONST               2 ('receiver_data')
                       18 LOAD_NAME                4 (dict)
                       20 LOAD_CONST               3 ('logger')
                       22 LOAD_NAME                5 (logging)
                       24 LOAD_ATTR                6 (Logger)
                       34 BUILD_TUPLE              4
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
-                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 269>)
+                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 270>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               7 (__init__)
          
-         278          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 278>)
+         279          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 279>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (__repr__)
                       52 LOAD_CLOSURE             0 (__class__)
                       54 COPY                     1
                       56 STORE_NAME               9 (__classcell__)
                       58 RETURN_VALUE
          consts
@@ -2384,44 +2441,44 @@
                   03190000000000000000007c005f0200000000000000007c02a003000000
                   000000000000000000000000000000000089036a040000000000000000a6
                   010000ab0100000000000000007c005f0500000000000000007c006a0500
                   00000000000000a006000000000000000000000000000000000000000064
                   04a6010000ab010000000000000000010064055300
                              0 COPY_FREE_VARS           1
                
-               269           2 RESUME                   0
+               270           2 RESUME                   0
                
-               271           4 LOAD_FAST                1 (receiver_data)
+               272           4 LOAD_FAST                1 (receiver_data)
                              6 LOAD_CONST               1 ('email')
                              8 BINARY_SUBSCR
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               0 (email)
                
-               272          30 LOAD_FAST                1 (receiver_data)
+               273          30 LOAD_FAST                1 (receiver_data)
                             32 LOAD_CONST               2 ('phoneNumber')
                             34 BINARY_SUBSCR
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (phone_number)
                
-               273          56 LOAD_FAST                1 (receiver_data)
+               274          56 LOAD_FAST                1 (receiver_data)
                             58 LOAD_CONST               3 ('name')
                             60 BINARY_SUBSCR
                             70 LOAD_FAST                0 (self)
                             72 STORE_ATTR               2 (name)
                
-               274          82 LOAD_FAST                2 (logger)
+               275          82 LOAD_FAST                2 (logger)
                             84 LOAD_METHOD              3 (getChild)
                            106 LOAD_DEREF               3 (__class__)
                            108 LOAD_ATTR                4 (__name__)
                            118 PRECALL                  1
                            122 CALL                     1
                            132 LOAD_FAST                0 (self)
                            134 STORE_ATTR               5 (_log)
                
-               276         144 LOAD_FAST                0 (self)
+               277         144 LOAD_FAST                0 (self)
                            146 LOAD_ATTR                5 (_log)
                            156 LOAD_METHOD              6 (debug)
                            178 LOAD_CONST               4 ('created')
                            180 PRECALL                  1
                            184 CALL                     1
                            194 POP_TOP
                            196 LOAD_CONST               5 (None)
@@ -2435,15 +2492,15 @@
                   None
                names      ('email', 'phone_number', 'name', 'getChild', '__name__', '_log', 'debug')
                varnames   ('self', 'receiver_data', 'logger')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
-               firstlineno 269
+               firstlineno 270
                lnotab 0x04021a011a011a013e02
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 3
                code
@@ -2452,32 +2509,32 @@
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000007d017c006a0300000000000000006a0400000000000000
                   00740b00000000000000000000740100000000000000000000740d000000
                   000000000000007c01a6010000ab010000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000a00700000000000000
                   0000000000000000000000000064026403a6020000ab0200000000000000
                   007a0000005300
-               278           0 RESUME                   0
+               279           0 RESUME                   0
                
-               279           2 LOAD_GLOBAL              1 (NULL + tuple)
-                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 279>)
+               280           2 LOAD_GLOBAL              1 (NULL + tuple)
+                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 280>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (__dict__)
                             30 LOAD_METHOD              2 (items)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (fields)
                
-               280          98 LOAD_FAST                0 (self)
+               281          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (__class__)
                            110 LOAD_ATTR                4 (__name__)
                            120 LOAD_GLOBAL             11 (NULL + str)
                            132 LOAD_GLOBAL              1 (NULL + tuple)
                            144 LOAD_GLOBAL             13 (NULL + sorted)
                            156 LOAD_FAST                1 (fields)
                            158 PRECALL                  1
@@ -2499,15 +2556,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d145c0200007d017d027c0164006b0300000000af
                         0b7c019b0064017c029b009d035600970101008c1564025300
-                     279           0 RETURN_GENERATOR
+                     280           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                20 (to 50)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (k)
                                   16 STORE_FAST               2 (v)
@@ -2533,75 +2590,75 @@
                         None
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<genexpr>'
-                     firstlineno 279
+                     firstlineno 280
                      lnotab 0x
                   "'"
                   ''
                names      ('tuple', '__dict__', 'items', '__class__', '__name__', 'str', 'sorted', 'replace')
                varnames   ('self', 'fields')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__repr__'
-               firstlineno 278
+               firstlineno 279
                lnotab 0x02016001
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'dict', 'logging', 'Logger', '__init__', '__repr__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'Receiver'
-         firstlineno 261
+         firstlineno 262
          lnotab 0x0c0104071e09
       'Receiver'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504640365056a06000000
             00000000006604880066016404840c5a07640584005a0864066509660264
             0784045a0a880078015a0b5300
                        0 MAKE_CELL                0 (__class__)
          
-         283           2 RESUME                   0
+         284           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Sender')
                       10 STORE_NAME               2 (__qualname__)
          
-         284          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` sender\n\n    :param sender_data: :class:`dict` containing sender data for :class:`Parcel`\n    :type sender_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
+         285          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` sender\n\n    :param sender_data: :class:`dict` containing sender data for :class:`Parcel`\n    :type sender_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
                       14 STORE_NAME               3 (__doc__)
          
-         291          16 LOAD_CONST               2 ('sender_data')
+         292          16 LOAD_CONST               2 ('sender_data')
                       18 LOAD_NAME                4 (dict)
                       20 LOAD_CONST               3 ('logger')
                       22 LOAD_NAME                5 (logging)
                       24 LOAD_ATTR                6 (Logger)
                       34 BUILD_TUPLE              4
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
-                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 291>)
+                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 292>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               7 (__init__)
          
-         298          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 298>)
+         299          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 299>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (__repr__)
          
-         302          52 LOAD_CONST               6 ('return')
+         303          52 LOAD_CONST               6 ('return')
                       54 LOAD_NAME                9 (str)
                       56 BUILD_TUPLE              2
-                      58 LOAD_CONST               7 (<code object __str__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 302>)
+                      58 LOAD_CONST               7 (<code object __str__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 303>)
                       60 MAKE_FUNCTION            4 (annotations)
                       62 STORE_NAME              10 (__str__)
                       64 LOAD_CLOSURE             0 (__class__)
                       66 COPY                     1
                       68 STORE_NAME              11 (__classcell__)
                       70 RETURN_VALUE
          consts
@@ -2618,32 +2675,32 @@
                   0x950197007c016401190000000000000000007c005f0000000000000000
                   007c02a001000000000000000000000000000000000000000089036a0200
                   00000000000000a6010000ab0100000000000000007c005f030000000000
                   0000007c006a030000000000000000a00400000000000000000000000000
                   000000000000006402a6010000ab010000000000000000010064035300
                              0 COPY_FREE_VARS           1
                
-               291           2 RESUME                   0
+               292           2 RESUME                   0
                
-               293           4 LOAD_FAST                1 (sender_data)
+               294           4 LOAD_FAST                1 (sender_data)
                              6 LOAD_CONST               1 ('name')
                              8 BINARY_SUBSCR
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               0 (sender_name)
                
-               294          30 LOAD_FAST                2 (logger)
+               295          30 LOAD_FAST                2 (logger)
                             32 LOAD_METHOD              1 (getChild)
                             54 LOAD_DEREF               3 (__class__)
                             56 LOAD_ATTR                2 (__name__)
                             66 PRECALL                  1
                             70 CALL                     1
                             80 LOAD_FAST                0 (self)
                             82 STORE_ATTR               3 (_log)
                
-               296          92 LOAD_FAST                0 (self)
+               297          92 LOAD_FAST                0 (self)
                             94 LOAD_ATTR                3 (_log)
                            104 LOAD_METHOD              4 (debug)
                            126 LOAD_CONST               2 ('created')
                            128 PRECALL                  1
                            132 CALL                     1
                            142 POP_TOP
                            144 LOAD_CONST               3 (None)
@@ -2655,15 +2712,15 @@
                   None
                names      ('sender_name', 'getChild', '__name__', '_log', 'debug')
                varnames   ('self', 'sender_data', 'logger')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
-               firstlineno 291
+               firstlineno 292
                lnotab 0x04021a013e02
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 3
                code
@@ -2672,32 +2729,32 @@
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000007d017c006a0300000000000000006a0400000000000000
                   00740b00000000000000000000740100000000000000000000740d000000
                   000000000000007c01a6010000ab010000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000a00700000000000000
                   0000000000000000000000000064026403a6020000ab0200000000000000
                   007a0000005300
-               298           0 RESUME                   0
+               299           0 RESUME                   0
                
-               299           2 LOAD_GLOBAL              1 (NULL + tuple)
-                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 299>)
+               300           2 LOAD_GLOBAL              1 (NULL + tuple)
+                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 300>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (__dict__)
                             30 LOAD_METHOD              2 (items)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (fields)
                
-               300          98 LOAD_FAST                0 (self)
+               301          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (__class__)
                            110 LOAD_ATTR                4 (__name__)
                            120 LOAD_GLOBAL             11 (NULL + str)
                            132 LOAD_GLOBAL              1 (NULL + tuple)
                            144 LOAD_GLOBAL             13 (NULL + sorted)
                            156 LOAD_FAST                1 (fields)
                            158 PRECALL                  1
@@ -2719,15 +2776,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d145c0200007d017d027c0164006b0300000000af
                         0b7c019b0064017c029b009d035600970101008c1564025300
-                     299           0 RETURN_GENERATOR
+                     300           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                20 (to 50)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (k)
                                   16 STORE_FAST               2 (v)
@@ -2753,117 +2810,117 @@
                         None
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<genexpr>'
-                     firstlineno 299
+                     firstlineno 300
                      lnotab 0x
                   "'"
                   ''
                names      ('tuple', '__dict__', 'items', '__class__', '__name__', 'str', 'sorted', 'replace')
                varnames   ('self', 'fields')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__repr__'
-               firstlineno 298
+               firstlineno 299
                lnotab 0x02016001
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               302           0 RESUME                   0
+               303           0 RESUME                   0
                
-               303           2 LOAD_FAST                0 (self)
+               304           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sender_name)
                             14 RETURN_VALUE
                consts
                   None
                names      ('sender_name',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__str__'
-               firstlineno 302
+               firstlineno 303
                lnotab 0x0201
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'dict', 'logging', 'Logger', '__init__', '__repr__', 'str', '__str__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'Sender'
-         firstlineno 283
+         firstlineno 284
          lnotab 0x0c0104071e070604
       'Sender'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504640365056a06000000
             00000000006604880066016404840c5a07640584005a0864066509660264
             0784045a0a650b6406650c650d650d660219000000000000000000660264
             088404a6000000ab0000000000000000005a0e880078015a0f5300
                        0 MAKE_CELL                0 (__class__)
          
-         306           2 RESUME                   0
+         307           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('PickupPoint')
                       10 STORE_NAME               2 (__qualname__)
          
-         307          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` pickup point\n\n    :param pickuppoint_data: :class:`dict` containing pickup point data for :class:`Parcel`\n    :type pickuppoint_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
+         308          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` pickup point\n\n    :param pickuppoint_data: :class:`dict` containing pickup point data for :class:`Parcel`\n    :type pickuppoint_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
                       14 STORE_NAME               3 (__doc__)
          
-         314          16 LOAD_CONST               2 ('pickuppoint_data')
+         315          16 LOAD_CONST               2 ('pickuppoint_data')
                       18 LOAD_NAME                4 (dict)
                       20 LOAD_CONST               3 ('logger')
                       22 LOAD_NAME                5 (logging)
                       24 LOAD_ATTR                6 (Logger)
                       34 BUILD_TUPLE              4
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
-                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 314>)
+                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 315>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               7 (__init__)
          
-         342          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 342>)
+         343          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 343>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (__repr__)
          
-         346          52 LOAD_CONST               6 ('return')
+         347          52 LOAD_CONST               6 ('return')
                       54 LOAD_NAME                9 (str)
                       56 BUILD_TUPLE              2
-                      58 LOAD_CONST               7 (<code object __str__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 346>)
+                      58 LOAD_CONST               7 (<code object __str__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 347>)
                       60 MAKE_FUNCTION            4 (annotations)
                       62 STORE_NAME              10 (__str__)
          
-         349          64 LOAD_NAME               11 (property)
+         350          64 LOAD_NAME               11 (property)
          
-         350          66 LOAD_CONST               6 ('return')
+         351          66 LOAD_CONST               6 ('return')
                       68 LOAD_NAME               12 (Tuple)
                       70 LOAD_NAME               13 (float)
                       72 LOAD_NAME               13 (float)
                       74 BUILD_TUPLE              2
                       76 BINARY_SUBSCR
                       86 BUILD_TUPLE              2
-                      88 LOAD_CONST               8 (<code object location, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 349>)
+                      88 LOAD_CONST               8 (<code object location, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 350>)
                       90 MAKE_FUNCTION            4 (annotations)
          
-         349          92 PRECALL                  0
+         350          92 PRECALL                  0
                       96 CALL                     0
          
-         350         106 STORE_NAME              14 (location)
+         351         106 STORE_NAME              14 (location)
                      108 LOAD_CLOSURE             0 (__class__)
                      110 COPY                     1
                      112 STORE_NAME              15 (__classcell__)
                      114 RETURN_VALUE
          consts
             'PickupPoint'
             'Object representation of :class:`Parcel` pickup point\n\n    :param pickuppoint_data: :class:`dict` containing pickup point data for :class:`Parcel`\n    :type pickuppoint_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger'
@@ -2903,198 +2960,198 @@
                   00000001007430000000000000000000006a1900000000000000007c006a
                   0c0000000000000000760072257c006a160000000000000000a017000000
                   000000000000000000000000000000000064197c01641019000000000000
                   0000009b009d02a6010000ab010000000000000000010064175300641753
                   00
                              0 COPY_FREE_VARS           1
                
-               314           2 RESUME                   0
+               315           2 RESUME                   0
                
-               316           4 LOAD_FAST                1 (pickuppoint_data)
+               317           4 LOAD_FAST                1 (pickuppoint_data)
                              6 LOAD_CONST               1 ('name')
                              8 BINARY_SUBSCR
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               0 (name)
                
-               317          30 LOAD_FAST                1 (pickuppoint_data)
+               318          30 LOAD_FAST                1 (pickuppoint_data)
                             32 LOAD_CONST               2 ('location')
                             34 BINARY_SUBSCR
                             44 LOAD_CONST               3 ('latitude')
                             46 BINARY_SUBSCR
                             56 LOAD_FAST                0 (self)
                             58 STORE_ATTR               1 (latitude)
                
-               318          68 LOAD_FAST                1 (pickuppoint_data)
+               319          68 LOAD_FAST                1 (pickuppoint_data)
                             70 LOAD_CONST               2 ('location')
                             72 BINARY_SUBSCR
                             82 LOAD_CONST               4 ('longitude')
                             84 BINARY_SUBSCR
                             94 LOAD_FAST                0 (self)
                             96 STORE_ATTR               2 (longitude)
                
-               319         106 LOAD_FAST                1 (pickuppoint_data)
+               320         106 LOAD_FAST                1 (pickuppoint_data)
                            108 LOAD_CONST               5 ('locationDescription')
                            110 BINARY_SUBSCR
                            120 LOAD_FAST                0 (self)
                            122 STORE_ATTR               3 (description)
                
-               320         132 LOAD_FAST                1 (pickuppoint_data)
+               321         132 LOAD_FAST                1 (pickuppoint_data)
                            134 LOAD_CONST               6 ('openingHours')
                            136 BINARY_SUBSCR
                            146 LOAD_FAST                0 (self)
                            148 STORE_ATTR               4 (opening_hours)
                
-               321         158 LOAD_FAST                1 (pickuppoint_data)
+               322         158 LOAD_FAST                1 (pickuppoint_data)
                            160 LOAD_CONST               7 ('addressDetails')
                            162 BINARY_SUBSCR
                            172 LOAD_CONST               8 ('postCode')
                            174 BINARY_SUBSCR
                            184 LOAD_FAST                0 (self)
                            186 STORE_ATTR               5 (post_code)
                
-               322         196 LOAD_FAST                1 (pickuppoint_data)
+               323         196 LOAD_FAST                1 (pickuppoint_data)
                            198 LOAD_CONST               7 ('addressDetails')
                            200 BINARY_SUBSCR
                            210 LOAD_CONST               9 ('city')
                            212 BINARY_SUBSCR
                            222 LOAD_FAST                0 (self)
                            224 STORE_ATTR               6 (city)
                
-               323         234 LOAD_FAST                1 (pickuppoint_data)
+               324         234 LOAD_FAST                1 (pickuppoint_data)
                            236 LOAD_CONST               7 ('addressDetails')
                            238 BINARY_SUBSCR
                            248 LOAD_CONST              10 ('province')
                            250 BINARY_SUBSCR
                            260 LOAD_FAST                0 (self)
                            262 STORE_ATTR               7 (province)
                
-               324         272 LOAD_FAST                1 (pickuppoint_data)
+               325         272 LOAD_FAST                1 (pickuppoint_data)
                            274 LOAD_CONST               7 ('addressDetails')
                            276 BINARY_SUBSCR
                            286 LOAD_CONST              11 ('street')
                            288 BINARY_SUBSCR
                            298 LOAD_FAST                0 (self)
                            300 STORE_ATTR               8 (street)
                
-               325         310 LOAD_FAST                1 (pickuppoint_data)
+               326         310 LOAD_FAST                1 (pickuppoint_data)
                            312 LOAD_CONST               7 ('addressDetails')
                            314 BINARY_SUBSCR
                            324 LOAD_CONST              12 ('buildingNumber')
                            326 BINARY_SUBSCR
                            336 LOAD_FAST                0 (self)
                            338 STORE_ATTR               9 (building_number)
                
-               326         348 LOAD_FAST                1 (pickuppoint_data)
+               327         348 LOAD_FAST                1 (pickuppoint_data)
                            350 LOAD_CONST              13 ('virtual')
                            352 BINARY_SUBSCR
                            362 LOAD_FAST                0 (self)
                            364 STORE_ATTR              10 (virtual)
                
-               327         374 LOAD_FAST                1 (pickuppoint_data)
+               328         374 LOAD_FAST                1 (pickuppoint_data)
                            376 LOAD_CONST              14 ('pointType')
                            378 BINARY_SUBSCR
                            388 LOAD_FAST                0 (self)
                            390 STORE_ATTR              11 (point_type)
                
-               328         400 LOAD_CONST              15 (<code object <listcomp>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 328>)
+               329         400 LOAD_CONST              15 (<code object <listcomp>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 329>)
                            402 MAKE_FUNCTION            0
                            404 LOAD_FAST                1 (pickuppoint_data)
                            406 LOAD_CONST              16 ('type')
                            408 BINARY_SUBSCR
                            418 GET_ITER
                            420 PRECALL                  0
                            424 CALL                     0
                            434 LOAD_FAST                0 (self)
                            436 STORE_ATTR              12 (type)
                
-               329         446 LOAD_FAST                1 (pickuppoint_data)
+               330         446 LOAD_FAST                1 (pickuppoint_data)
                            448 LOAD_CONST              17 ('location247')
                            450 BINARY_SUBSCR
                            460 LOAD_FAST                0 (self)
                            462 STORE_ATTR              13 (location_round_the_clock)
                
-               330         472 LOAD_FAST                1 (pickuppoint_data)
+               331         472 LOAD_FAST                1 (pickuppoint_data)
                            474 LOAD_CONST              18 ('doubled')
                            476 BINARY_SUBSCR
                            486 LOAD_FAST                0 (self)
                            488 STORE_ATTR              14 (doubled)
                
-               331         498 LOAD_FAST                1 (pickuppoint_data)
+               332         498 LOAD_FAST                1 (pickuppoint_data)
                            500 LOAD_CONST              19 ('imageUrl')
                            502 BINARY_SUBSCR
                            512 LOAD_FAST                0 (self)
                            514 STORE_ATTR              15 (image_url)
                
-               332         524 LOAD_FAST                1 (pickuppoint_data)
+               333         524 LOAD_FAST                1 (pickuppoint_data)
                            526 LOAD_CONST              20 ('easyAccessZone')
                            528 BINARY_SUBSCR
                            538 LOAD_FAST                0 (self)
                            540 STORE_ATTR              16 (easy_access_zone)
                
-               333         550 LOAD_FAST                1 (pickuppoint_data)
+               334         550 LOAD_FAST                1 (pickuppoint_data)
                            552 LOAD_CONST              21 ('airSensor')
                            554 BINARY_SUBSCR
                            564 LOAD_FAST                0 (self)
                            566 STORE_ATTR              17 (air_sensor)
                
-               334         576 LOAD_CONST              22 ('airSensorData')
+               335         576 LOAD_CONST              22 ('airSensorData')
                            578 LOAD_FAST                1 (pickuppoint_data)
                            580 CONTAINS_OP              0
                            582 POP_JUMP_FORWARD_IF_FALSE    21 (to 626)
                            584 LOAD_GLOBAL             37 (NULL + AirSensorData)
                            596 LOAD_FAST                1 (pickuppoint_data)
                            598 LOAD_CONST              22 ('airSensorData')
                            600 BINARY_SUBSCR
                            610 PRECALL                  1
                            614 CALL                     1
                            624 JUMP_FORWARD             1 (to 628)
                        >>  626 LOAD_CONST              23 (None)
                        >>  628 LOAD_FAST                0 (self)
                            630 STORE_ATTR              19 (air_sensor_data)
                
-               336         640 LOAD_FAST                2 (logger)
+               337         640 LOAD_FAST                2 (logger)
                            642 LOAD_METHOD             20 (getChild)
                            664 LOAD_DEREF               3 (__class__)
                            666 LOAD_ATTR               21 (__name__)
                            676 PRECALL                  1
                            680 CALL                     1
                            690 LOAD_FAST                0 (self)
                            692 STORE_ATTR              22 (_log)
                
-               337         702 LOAD_FAST                0 (self)
+               338         702 LOAD_FAST                0 (self)
                            704 LOAD_ATTR               22 (_log)
                            714 LOAD_METHOD             23 (debug)
                            736 LOAD_CONST              24 ('created')
                            738 PRECALL                  1
                            742 CALL                     1
                            752 POP_TOP
                
-               339         754 LOAD_GLOBAL             48 (ParcelDeliveryType)
+               340         754 LOAD_GLOBAL             48 (ParcelDeliveryType)
                            766 LOAD_ATTR               25 (UNKNOWN)
                            776 LOAD_FAST                0 (self)
                            778 LOAD_ATTR               12 (type)
                            788 CONTAINS_OP              0
                            790 POP_JUMP_FORWARD_IF_FALSE    37 (to 866)
                
-               340         792 LOAD_FAST                0 (self)
+               341         792 LOAD_FAST                0 (self)
                            794 LOAD_ATTR               22 (_log)
                            804 LOAD_METHOD             23 (debug)
                            826 LOAD_CONST              25 ('unknown delivery type: ')
                            828 LOAD_FAST                1 (pickuppoint_data)
                            830 LOAD_CONST              16 ('type')
                            832 BINARY_SUBSCR
                            842 FORMAT_VALUE             0
                            844 BUILD_STRING             2
                            846 PRECALL                  1
                            850 CALL                     1
                            860 POP_TOP
                            862 LOAD_CONST              23 (None)
                            864 RETURN_VALUE
                
-               339     >>  866 LOAD_CONST              23 (None)
+               340     >>  866 LOAD_CONST              23 (None)
                            868 RETURN_VALUE
                consts
                   'Constructor method'
                   'name'
                   'location'
                   'latitude'
                   'longitude'
@@ -3112,15 +3169,15 @@
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d0f7d017400000000000000000000007c011900000000
                         000000000091028c105300
-                     328           0 RESUME                   0
+                     329           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                15 (to 38)
                                    8 STORE_FAST               1 (data)
                                   10 LOAD_GLOBAL              0 (ParcelDeliveryType)
                                   22 LOAD_FAST                1 (data)
                                   24 BINARY_SUBSCR
@@ -3130,15 +3187,15 @@
                      consts
                      names      ('ParcelDeliveryType',)
                      varnames   ('.0', 'data')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<listcomp>'
-                     firstlineno 328
+                     firstlineno 329
                      lnotab 0x
                   'type'
                   'location247'
                   'doubled'
                   'imageUrl'
                   'easyAccessZone'
                   'airSensor'
@@ -3148,15 +3205,15 @@
                   'unknown delivery type: '
                names      ('name', 'latitude', 'longitude', 'description', 'opening_hours', 'post_code', 'city', 'province', 'street', 'building_number', 'virtual', 'point_type', 'type', 'location_round_the_clock', 'doubled', 'image_url', 'easy_access_zone', 'air_sensor', 'AirSensorData', 'air_sensor_data', 'getChild', '__name__', '_log', 'debug', 'ParcelDeliveryType', 'UNKNOWN')
                varnames   ('self', 'pickuppoint_data', 'logger')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
-               firstlineno 314
+               firstlineno 315
                lnotab
                   0x04021a01260126011a011a01260126012601260126011a011a012e011a
                   011a011a011a011a0140023e01340226014aff
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
@@ -3167,32 +3224,32 @@
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000007d017c006a0300000000000000006a0400000000000000
                   00740b00000000000000000000740100000000000000000000740d000000
                   000000000000007c01a6010000ab010000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000a00700000000000000
                   0000000000000000000000000064026403a6020000ab0200000000000000
                   007a0000005300
-               342           0 RESUME                   0
+               343           0 RESUME                   0
                
-               343           2 LOAD_GLOBAL              1 (NULL + tuple)
-                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 343>)
+               344           2 LOAD_GLOBAL              1 (NULL + tuple)
+                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 344>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (__dict__)
                             30 LOAD_METHOD              2 (items)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (fields)
                
-               344          98 LOAD_FAST                0 (self)
+               345          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (__class__)
                            110 LOAD_ATTR                4 (__name__)
                            120 LOAD_GLOBAL             11 (NULL + str)
                            132 LOAD_GLOBAL              1 (NULL + tuple)
                            144 LOAD_GLOBAL             13 (NULL + sorted)
                            156 LOAD_FAST                1 (fields)
                            158 PRECALL                  1
@@ -3214,15 +3271,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d145c0200007d017d027c0164006b0300000000af
                         0b7c019b0064017c029b009d035600970101008c1564025300
-                     343           0 RETURN_GENERATOR
+                     344           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                20 (to 50)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (k)
                                   16 STORE_FAST               2 (v)
@@ -3248,126 +3305,126 @@
                         None
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<genexpr>'
-                     firstlineno 343
+                     firstlineno 344
                      lnotab 0x
                   "'"
                   ''
                names      ('tuple', '__dict__', 'items', '__class__', '__name__', 'str', 'sorted', 'replace')
                varnames   ('self', 'fields')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__repr__'
-               firstlineno 342
+               firstlineno 343
                lnotab 0x02016001
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               346           0 RESUME                   0
+               347           0 RESUME                   0
                
-               347           2 LOAD_FAST                0 (self)
+               348           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (name)
                             14 RETURN_VALUE
                consts
                   None
                names      ('name',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__str__'
-               firstlineno 346
+               firstlineno 347
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab01000000000000000001007c006a0200
                   000000000000007c006a03000000000000000066025300
-               349           0 RESUME                   0
+               350           0 RESUME                   0
                
-               355           2 LOAD_FAST                0 (self)
+               356           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('getting location')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               356          54 LOAD_FAST                0 (self)
+               357          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (latitude)
                             66 LOAD_FAST                0 (self)
                             68 LOAD_ATTR                3 (longitude)
                             78 BUILD_TUPLE              2
                             80 RETURN_VALUE
                consts
                   'Returns a mocked location for :class:`PickupPoint`\n\n        :return: tuple containing location for :class:`PickupPoint`\n        :rtype: tuple'
                   'getting location'
                names      ('_log', 'debug', 'latitude', 'longitude')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'location'
-               firstlineno 349
+               firstlineno 350
                lnotab 0x02063401
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'dict', 'logging', 'Logger', '__init__', '__repr__', 'str', '__str__', 'property', 'Tuple', 'float', 'location', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'PickupPoint'
-         firstlineno 306
+         firstlineno 307
          lnotab 0x0c0104071e1c06040c0302011aff0e01
       'PickupPoint'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504640365056a06000000
             00000000006604880066016404840c5a07640584005a08880078015a0953
             00
                        0 MAKE_CELL                0 (__class__)
          
-         359           2 RESUME                   0
+         360           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('MultiCompartment')
                       10 STORE_NAME               2 (__qualname__)
          
-         360          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` `multicompartment`\n\n    :param multicompartment_data: :class:`dict` containing multicompartment data for :class:`Parcel`\n    :type multicompartment_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
+         361          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` `multicompartment`\n\n    :param multicompartment_data: :class:`dict` containing multicompartment data for :class:`Parcel`\n    :type multicompartment_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
                       14 STORE_NAME               3 (__doc__)
          
-         367          16 LOAD_CONST               2 ('multicompartment_data')
+         368          16 LOAD_CONST               2 ('multicompartment_data')
                       18 LOAD_NAME                4 (dict)
                       20 LOAD_CONST               3 ('logger')
                       22 LOAD_NAME                5 (logging)
                       24 LOAD_ATTR                6 (Logger)
                       34 BUILD_TUPLE              4
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
-                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 367>)
+                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 368>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               7 (__init__)
          
-         378          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 378>)
+         379          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 379>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (__repr__)
                       52 LOAD_CLOSURE             0 (__class__)
                       54 COPY                     1
                       56 STORE_NAME               9 (__classcell__)
                       58 RETURN_VALUE
          consts
@@ -3387,59 +3444,59 @@
                   00000000007c016405190000000000000000007c005f0300000000000000
                   007c02a004000000000000000000000000000000000000000089036a0500
                   00000000000000a6010000ab0100000000000000007c005f060000000000
                   0000007c006a060000000000000000a00700000000000000000000000000
                   000000000000006406a6010000ab010000000000000000010064035300
                              0 COPY_FREE_VARS           1
                
-               367           2 RESUME                   0
+               368           2 RESUME                   0
                
-               369           4 LOAD_FAST                1 (multicompartment_data)
+               370           4 LOAD_FAST                1 (multicompartment_data)
                              6 LOAD_CONST               1 ('uuid')
                              8 BINARY_SUBSCR
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               0 (uuid)
                
-               371          30 LOAD_CONST               2 ('shipmentNumbers')
+               372          30 LOAD_CONST               2 ('shipmentNumbers')
                             32 LOAD_FAST                1 (multicompartment_data)
                             34 CONTAINS_OP              0
                             36 POP_JUMP_FORWARD_IF_FALSE     8 (to 54)
                
-               370          38 LOAD_FAST                1 (multicompartment_data)
+               371          38 LOAD_FAST                1 (multicompartment_data)
                             40 LOAD_CONST               2 ('shipmentNumbers')
                             42 BINARY_SUBSCR
                             52 JUMP_FORWARD             1 (to 56)
                
-               371     >>   54 LOAD_CONST               3 (None)
+               372     >>   54 LOAD_CONST               3 (None)
                
-               370     >>   56 LOAD_FAST                0 (self)
+               371     >>   56 LOAD_FAST                0 (self)
                             58 STORE_ATTR               1 (shipment_numbers)
                
-               372          68 LOAD_FAST                1 (multicompartment_data)
+               373          68 LOAD_FAST                1 (multicompartment_data)
                             70 LOAD_CONST               4 ('presentation')
                             72 BINARY_SUBSCR
                             82 LOAD_FAST                0 (self)
                             84 STORE_ATTR               2 (presentation)
                
-               373          94 LOAD_FAST                1 (multicompartment_data)
+               374          94 LOAD_FAST                1 (multicompartment_data)
                             96 LOAD_CONST               5 ('collected')
                             98 BINARY_SUBSCR
                            108 LOAD_FAST                0 (self)
                            110 STORE_ATTR               3 (collected)
                
-               375         120 LOAD_FAST                2 (logger)
+               376         120 LOAD_FAST                2 (logger)
                            122 LOAD_METHOD              4 (getChild)
                            144 LOAD_DEREF               3 (__class__)
                            146 LOAD_ATTR                5 (__name__)
                            156 PRECALL                  1
                            160 CALL                     1
                            170 LOAD_FAST                0 (self)
                            172 STORE_ATTR               6 (_log)
                
-               376         182 LOAD_FAST                0 (self)
+               377         182 LOAD_FAST                0 (self)
                            184 LOAD_ATTR                6 (_log)
                            194 LOAD_METHOD              7 (debug)
                            216 LOAD_CONST               6 ('created')
                            218 PRECALL                  1
                            222 CALL                     1
                            232 POP_TOP
                            234 LOAD_CONST               3 (None)
@@ -3454,15 +3511,15 @@
                   'created'
                names      ('uuid', 'shipment_numbers', 'presentation', 'collected', 'getChild', '__name__', '_log', 'debug')
                varnames   ('self', 'multicompartment_data', 'logger')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
-               firstlineno 367
+               firstlineno 368
                lnotab 0x04021a0208ff100102ff0c021a011a023e01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 3
                code
@@ -3471,32 +3528,32 @@
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000007d017c006a0300000000000000006a0400000000000000
                   00740b00000000000000000000740100000000000000000000740d000000
                   000000000000007c01a6010000ab010000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000a00700000000000000
                   0000000000000000000000000064026403a6020000ab0200000000000000
                   007a0000005300
-               378           0 RESUME                   0
+               379           0 RESUME                   0
                
-               379           2 LOAD_GLOBAL              1 (NULL + tuple)
-                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 379>)
+               380           2 LOAD_GLOBAL              1 (NULL + tuple)
+                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 380>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (__dict__)
                             30 LOAD_METHOD              2 (items)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (fields)
                
-               380          98 LOAD_FAST                0 (self)
+               381          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (__class__)
                            110 LOAD_ATTR                4 (__name__)
                            120 LOAD_GLOBAL             11 (NULL + str)
                            132 LOAD_GLOBAL              1 (NULL + tuple)
                            144 LOAD_GLOBAL             13 (NULL + sorted)
                            156 LOAD_FAST                1 (fields)
                            158 PRECALL                  1
@@ -3518,15 +3575,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d145c0200007d017d027c0164006b0300000000af
                         0b7c019b0064017c029b009d035600970101008c1564025300
-                     379           0 RETURN_GENERATOR
+                     380           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                20 (to 50)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (k)
                                   16 STORE_FAST               2 (v)
@@ -3552,68 +3609,68 @@
                         None
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<genexpr>'
-                     firstlineno 379
+                     firstlineno 380
                      lnotab 0x
                   "'"
                   ''
                names      ('tuple', '__dict__', 'items', '__class__', '__name__', 'str', 'sorted', 'replace')
                varnames   ('self', 'fields')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__repr__'
-               firstlineno 378
+               firstlineno 379
                lnotab 0x02016001
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'dict', 'logging', 'Logger', '__init__', '__repr__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'MultiCompartment'
-         firstlineno 359
+         firstlineno 360
          lnotab 0x0c0104071e0b
       'MultiCompartment'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504640365056a06000000
             00000000006604880066016404840c5a07640584005a08880078015a0953
             00
                        0 MAKE_CELL                0 (__class__)
          
-         383           2 RESUME                   0
+         384           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Operations')
                       10 STORE_NAME               2 (__qualname__)
          
-         384          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` `operations`\n\n    :param operations_data: :class:`dict` containing operations data for :class:`Parcel`\n    :type operations_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
+         385          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` `operations`\n\n    :param operations_data: :class:`dict` containing operations data for :class:`Parcel`\n    :type operations_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
                       14 STORE_NAME               3 (__doc__)
          
-         391          16 LOAD_CONST               2 ('operations_data')
+         392          16 LOAD_CONST               2 ('operations_data')
                       18 LOAD_NAME                4 (dict)
                       20 LOAD_CONST               3 ('logger')
                       22 LOAD_NAME                5 (logging)
                       24 LOAD_ATTR                6 (Logger)
                       34 BUILD_TUPLE              4
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
-                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 391>)
+                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 392>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               7 (__init__)
          
-         411          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 411>)
+         412          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 412>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (__repr__)
                       52 LOAD_CLOSURE             0 (__class__)
                       54 COPY                     1
                       56 STORE_NAME               9 (__classcell__)
                       58 RETURN_VALUE
          consts
@@ -3643,127 +3700,127 @@
                   01640e190000000000000000006e0164037c005f0d00000000000000007c
                   02a00e000000000000000000000000000000000000000089036a0f000000
                   0000000000a6010000ab0100000000000000007c005f1000000000000000
                   007c006a100000000000000000a011000000000000000000000000000000
                   0000000000640fa6010000ab010000000000000000010064035300
                              0 COPY_FREE_VARS           1
                
-               391           2 RESUME                   0
+               392           2 RESUME                   0
                
-               393           4 LOAD_FAST                1 (operations_data)
+               394           4 LOAD_FAST                1 (operations_data)
                              6 LOAD_CONST               1 ('manualArchive')
                              8 BINARY_SUBSCR
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               0 (manual_archive)
                
-               395          30 LOAD_CONST               2 ('autoArchivableSince')
+               396          30 LOAD_CONST               2 ('autoArchivableSince')
                             32 LOAD_FAST                1 (operations_data)
                             34 CONTAINS_OP              0
                             36 POP_JUMP_FORWARD_IF_FALSE    21 (to 80)
                
-               394          38 LOAD_GLOBAL              3 (NULL + get)
+               395          38 LOAD_GLOBAL              3 (NULL + get)
                
-               395          50 LOAD_FAST                1 (operations_data)
+               396          50 LOAD_FAST                1 (operations_data)
                             52 LOAD_CONST               2 ('autoArchivableSince')
                             54 BINARY_SUBSCR
                
-               394          64 PRECALL                  1
+               395          64 PRECALL                  1
                             68 CALL                     1
                             78 JUMP_FORWARD             1 (to 82)
                
-               395     >>   80 LOAD_CONST               3 (None)
+               396     >>   80 LOAD_CONST               3 (None)
                
-               394     >>   82 LOAD_FAST                0 (self)
+               395     >>   82 LOAD_FAST                0 (self)
                             84 STORE_ATTR               2 (auto_archivable_since)
                
-               396          94 LOAD_FAST                1 (operations_data)
+               397          94 LOAD_FAST                1 (operations_data)
                             96 LOAD_CONST               4 ('delete')
                             98 BINARY_SUBSCR
                            108 LOAD_FAST                0 (self)
                            110 STORE_ATTR               3 (delete)
                
-               397         120 LOAD_FAST                1 (operations_data)
+               398         120 LOAD_FAST                1 (operations_data)
                            122 LOAD_CONST               5 ('collect')
                            124 BINARY_SUBSCR
                            134 LOAD_FAST                0 (self)
                            136 STORE_ATTR               4 (collect)
                
-               398         146 LOAD_FAST                1 (operations_data)
+               399         146 LOAD_FAST                1 (operations_data)
                            148 LOAD_CONST               6 ('expandAvizo')
                            150 BINARY_SUBSCR
                            160 LOAD_FAST                0 (self)
                            162 STORE_ATTR               5 (expand_avizo)
                
-               399         172 LOAD_FAST                1 (operations_data)
+               400         172 LOAD_FAST                1 (operations_data)
                            174 LOAD_CONST               7 ('highlight')
                            176 BINARY_SUBSCR
                            186 LOAD_FAST                0 (self)
                            188 STORE_ATTR               6 (highlight)
                
-               400         198 LOAD_GLOBAL              3 (NULL + get)
+               401         198 LOAD_GLOBAL              3 (NULL + get)
                            210 LOAD_FAST                1 (operations_data)
                            212 LOAD_CONST               8 ('refreshUntil')
                            214 BINARY_SUBSCR
                            224 PRECALL                  1
                            228 CALL                     1
                            238 LOAD_FAST                0 (self)
                            240 STORE_ATTR               7 (refresh_until)
                
-               401         250 LOAD_FAST                1 (operations_data)
+               402         250 LOAD_FAST                1 (operations_data)
                            252 LOAD_CONST               9 ('requestEasyAccessZone')
                            254 BINARY_SUBSCR
                            264 LOAD_FAST                0 (self)
                            266 STORE_ATTR               8 (request_easy_access_zone)
                
-               402         276 LOAD_FAST                1 (operations_data)
+               403         276 LOAD_FAST                1 (operations_data)
                            278 LOAD_CONST              10 ('voicebot')
                            280 BINARY_SUBSCR
                            290 LOAD_FAST                0 (self)
                            292 STORE_ATTR               9 (is_voicebot)
                
-               403         302 LOAD_FAST                1 (operations_data)
+               404         302 LOAD_FAST                1 (operations_data)
                            304 LOAD_CONST              11 ('canShareToObserve')
                            306 BINARY_SUBSCR
                            316 LOAD_FAST                0 (self)
                            318 STORE_ATTR              10 (can_share_to_observe)
                
-               404         328 LOAD_FAST                1 (operations_data)
+               405         328 LOAD_FAST                1 (operations_data)
                            330 LOAD_CONST              12 ('canShareOpenCode')
                            332 BINARY_SUBSCR
                            342 LOAD_FAST                0 (self)
                            344 STORE_ATTR              11 (can_share_open_code)
                
-               405         354 LOAD_FAST                1 (operations_data)
+               406         354 LOAD_FAST                1 (operations_data)
                            356 LOAD_CONST              13 ('canShareParcel')
                            358 BINARY_SUBSCR
                            368 LOAD_FAST                0 (self)
                            370 STORE_ATTR              12 (can_share_parcel)
                
-               406         380 LOAD_CONST              14 ('send')
+               407         380 LOAD_CONST              14 ('send')
                            382 LOAD_FAST                1 (operations_data)
                            384 CONTAINS_OP              0
                            386 POP_JUMP_FORWARD_IF_FALSE     8 (to 404)
                            388 LOAD_FAST                1 (operations_data)
                            390 LOAD_CONST              14 ('send')
                            392 BINARY_SUBSCR
                            402 JUMP_FORWARD             1 (to 406)
                        >>  404 LOAD_CONST               3 (None)
                        >>  406 LOAD_FAST                0 (self)
                            408 STORE_ATTR              13 (send)
                
-               408         418 LOAD_FAST                2 (logger)
+               409         418 LOAD_FAST                2 (logger)
                            420 LOAD_METHOD             14 (getChild)
                            442 LOAD_DEREF               3 (__class__)
                            444 LOAD_ATTR               15 (__name__)
                            454 PRECALL                  1
                            458 CALL                     1
                            468 LOAD_FAST                0 (self)
                            470 STORE_ATTR              16 (_log)
                
-               409         480 LOAD_FAST                0 (self)
+               410         480 LOAD_FAST                0 (self)
                            482 LOAD_ATTR               16 (_log)
                            492 LOAD_METHOD             17 (debug)
                            514 LOAD_CONST              15 ('created')
                            516 PRECALL                  1
                            520 CALL                     1
                            530 POP_TOP
                            532 LOAD_CONST               3 (None)
@@ -3787,15 +3844,15 @@
                   'created'
                names      ('manual_archive', 'get', 'auto_archivable_since', 'delete', 'collect', 'expand_avizo', 'highlight', 'refresh_until', 'request_easy_access_zone', 'is_voicebot', 'can_share_to_observe', 'can_share_open_code', 'can_share_parcel', 'send', 'getChild', '__name__', '_log', 'debug')
                varnames   ('self', 'operations_data', 'logger')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
-               firstlineno 391
+               firstlineno 392
                lnotab
                   0x04021a0208ff0c010eff100102ff0c021a011a011a011a0134011a011a
                   011a011a011a0126023e01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
@@ -3806,32 +3863,32 @@
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000007d017c006a0300000000000000006a0400000000000000
                   00740b00000000000000000000740100000000000000000000740d000000
                   000000000000007c01a6010000ab010000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000a00700000000000000
                   0000000000000000000000000064026403a6020000ab0200000000000000
                   007a0000005300
-               411           0 RESUME                   0
+               412           0 RESUME                   0
                
-               412           2 LOAD_GLOBAL              1 (NULL + tuple)
-                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 412>)
+               413           2 LOAD_GLOBAL              1 (NULL + tuple)
+                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 413>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (__dict__)
                             30 LOAD_METHOD              2 (items)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (fields)
                
-               413          98 LOAD_FAST                0 (self)
+               414          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (__class__)
                            110 LOAD_ATTR                4 (__name__)
                            120 LOAD_GLOBAL             11 (NULL + str)
                            132 LOAD_GLOBAL              1 (NULL + tuple)
                            144 LOAD_GLOBAL             13 (NULL + sorted)
                            156 LOAD_FAST                1 (fields)
                            158 PRECALL                  1
@@ -3853,15 +3910,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d145c0200007d017d027c0164006b0300000000af
                         0b7c019b0064017c029b009d035600970101008c1564025300
-                     412           0 RETURN_GENERATOR
+                     413           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                20 (to 50)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (k)
                                   16 STORE_FAST               2 (v)
@@ -3887,68 +3944,68 @@
                         None
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<genexpr>'
-                     firstlineno 412
+                     firstlineno 413
                      lnotab 0x
                   "'"
                   ''
                names      ('tuple', '__dict__', 'items', '__class__', '__name__', 'str', 'sorted', 'replace')
                varnames   ('self', 'fields')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__repr__'
-               firstlineno 411
+               firstlineno 412
                lnotab 0x02016001
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'dict', 'logging', 'Logger', '__init__', '__repr__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'Operations'
-         firstlineno 383
+         firstlineno 384
          lnotab 0x0c0104071e14
       'Operations'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504640365056a06000000
             00000000006604880066016404840c5a07640584005a08880078015a0953
             00
                        0 MAKE_CELL                0 (__class__)
          
-         416           2 RESUME                   0
+         417           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('EventLog')
                       10 STORE_NAME               2 (__qualname__)
          
-         417          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` single eventlog\n\n    :param eventlog_data: :class:`dict` containing single eventlog data for :class:`Parcel`\n    :type eventlog_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
+         418          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` single eventlog\n\n    :param eventlog_data: :class:`dict` containing single eventlog data for :class:`Parcel`\n    :type eventlog_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
                       14 STORE_NAME               3 (__doc__)
          
-         424          16 LOAD_CONST               2 ('eventlog_data')
+         425          16 LOAD_CONST               2 ('eventlog_data')
                       18 LOAD_NAME                4 (dict)
                       20 LOAD_CONST               3 ('logger')
                       22 LOAD_NAME                5 (logging)
                       24 LOAD_ATTR                6 (Logger)
                       34 BUILD_TUPLE              4
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
-                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 424>)
+                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 425>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               7 (__init__)
          
-         437          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 437>)
+         438          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 438>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (__repr__)
                       52 LOAD_CLOSURE             0 (__class__)
                       54 COPY                     1
                       56 STORE_NAME               9 (__classcell__)
                       58 RETURN_VALUE
          consts
@@ -3977,86 +4034,86 @@
                   04000000000000000000006a0a00000000000000006b0200000000722d7c
                   006a080000000000000000a0090000000000000000000000000000000000
                   00000064067c006a0000000000000000009b0064077c0164031900000000
                   00000000009b009d04a6010000ab01000000000000000001006408530064
                   085300
                              0 COPY_FREE_VARS           1
                
-               424           2 RESUME                   0
+               425           2 RESUME                   0
                
-               426           4 LOAD_FAST                1 (eventlog_data)
+               427           4 LOAD_FAST                1 (eventlog_data)
                              6 LOAD_CONST               1 ('type')
                              8 BINARY_SUBSCR
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               0 (type)
                
-               428          30 LOAD_FAST                0 (self)
+               429          30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                0 (type)
                             42 LOAD_CONST               2 ('PARCEL_STATUS')
                             44 COMPARE_OP               2 (==)
                             50 POP_JUMP_FORWARD_IF_FALSE    19 (to 90)
                
-               427          52 LOAD_GLOBAL              2 (ParcelStatus)
+               428          52 LOAD_GLOBAL              2 (ParcelStatus)
                
-               428          64 LOAD_FAST                1 (eventlog_data)
+               429          64 LOAD_FAST                1 (eventlog_data)
                             66 LOAD_CONST               3 ('name')
                             68 BINARY_SUBSCR
                
-               427          78 BINARY_SUBSCR
+               428          78 BINARY_SUBSCR
                             88 JUMP_FORWARD            18 (to 126)
                
-               428     >>   90 LOAD_GLOBAL              4 (ReturnsStatus)
+               429     >>   90 LOAD_GLOBAL              4 (ReturnsStatus)
                            102 LOAD_FAST                1 (eventlog_data)
                            104 LOAD_CONST               3 ('name')
                            106 BINARY_SUBSCR
                            116 BINARY_SUBSCR
                
-               427     >>  126 LOAD_FAST                0 (self)
+               428     >>  126 LOAD_FAST                0 (self)
                            128 STORE_ATTR               3 (name)
                
-               429         138 LOAD_GLOBAL              9 (NULL + get)
+               430         138 LOAD_GLOBAL              9 (NULL + get)
                            150 LOAD_FAST                1 (eventlog_data)
                            152 LOAD_CONST               4 ('date')
                            154 BINARY_SUBSCR
                            164 PRECALL                  1
                            168 CALL                     1
                            178 LOAD_FAST                0 (self)
                            180 STORE_ATTR               5 (date)
                
-               431         190 LOAD_FAST                2 (logger)
+               432         190 LOAD_FAST                2 (logger)
                            192 LOAD_METHOD              6 (getChild)
                            214 LOAD_DEREF               3 (__class__)
                            216 LOAD_ATTR                7 (__name__)
                            226 PRECALL                  1
                            230 CALL                     1
                            240 LOAD_FAST                0 (self)
                            242 STORE_ATTR               8 (_log)
                
-               432         252 LOAD_FAST                0 (self)
+               433         252 LOAD_FAST                0 (self)
                            254 LOAD_ATTR                8 (_log)
                            264 LOAD_METHOD              9 (debug)
                            286 LOAD_CONST               5 ('created')
                            288 PRECALL                  1
                            292 CALL                     1
                            302 POP_TOP
                
-               434         304 LOAD_FAST                0 (self)
+               435         304 LOAD_FAST                0 (self)
                            306 LOAD_ATTR                3 (name)
                            316 LOAD_GLOBAL              2 (ParcelStatus)
                            328 LOAD_ATTR               10 (UNKNOWN)
                            338 COMPARE_OP               2 (==)
                            344 POP_JUMP_FORWARD_IF_TRUE    21 (to 388)
                            346 LOAD_FAST                0 (self)
                            348 LOAD_ATTR                3 (name)
                            358 LOAD_GLOBAL              4 (ReturnsStatus)
                            370 LOAD_ATTR               10 (UNKNOWN)
                            380 COMPARE_OP               2 (==)
                            386 POP_JUMP_FORWARD_IF_FALSE    45 (to 478)
                
-               435     >>  388 LOAD_FAST                0 (self)
+               436     >>  388 LOAD_FAST                0 (self)
                            390 LOAD_ATTR                8 (_log)
                            400 LOAD_METHOD              9 (debug)
                            422 LOAD_CONST               6 ('unknown ')
                            424 LOAD_FAST                0 (self)
                            426 LOAD_ATTR                0 (type)
                            436 FORMAT_VALUE             0
                            438 LOAD_CONST               7 (': ')
@@ -4067,15 +4124,15 @@
                            456 BUILD_STRING             4
                            458 PRECALL                  1
                            462 CALL                     1
                            472 POP_TOP
                            474 LOAD_CONST               8 (None)
                            476 RETURN_VALUE
                
-               434     >>  478 LOAD_CONST               8 (None)
+               435     >>  478 LOAD_CONST               8 (None)
                            480 RETURN_VALUE
                consts
                   'Constructor method'
                   'type'
                   'PARCEL_STATUS'
                   'name'
                   'date'
@@ -4085,15 +4142,15 @@
                   None
                names      ('type', 'ParcelStatus', 'ReturnsStatus', 'name', 'get', 'date', 'getChild', '__name__', '_log', 'debug', 'UNKNOWN')
                varnames   ('self', 'eventlog_data', 'logger')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
-               firstlineno 424
+               firstlineno 425
                lnotab 0x04021a0216ff0c010eff0c0124ff0c0234023e01340254015aff
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 3
                code
@@ -4102,32 +4159,32 @@
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000007d017c006a0300000000000000006a0400000000000000
                   00740b00000000000000000000740100000000000000000000740d000000
                   000000000000007c01a6010000ab010000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000a00700000000000000
                   0000000000000000000000000064026403a6020000ab0200000000000000
                   007a0000005300
-               437           0 RESUME                   0
+               438           0 RESUME                   0
                
-               438           2 LOAD_GLOBAL              1 (NULL + tuple)
-                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 438>)
+               439           2 LOAD_GLOBAL              1 (NULL + tuple)
+                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 439>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (__dict__)
                             30 LOAD_METHOD              2 (items)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (fields)
                
-               439          98 LOAD_FAST                0 (self)
+               440          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (__class__)
                            110 LOAD_ATTR                4 (__name__)
                            120 LOAD_GLOBAL             11 (NULL + str)
                            132 LOAD_GLOBAL              1 (NULL + tuple)
                            144 LOAD_GLOBAL             13 (NULL + sorted)
                            156 LOAD_FAST                1 (fields)
                            158 PRECALL                  1
@@ -4149,15 +4206,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d145c0200007d017d027c0164006b0300000000af
                         0b7c019b0064017c029b009d035600970101008c1564025300
-                     438           0 RETURN_GENERATOR
+                     439           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                20 (to 50)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (k)
                                   16 STORE_FAST               2 (v)
@@ -4183,68 +4240,68 @@
                         None
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<genexpr>'
-                     firstlineno 438
+                     firstlineno 439
                      lnotab 0x
                   "'"
                   ''
                names      ('tuple', '__dict__', 'items', '__class__', '__name__', 'str', 'sorted', 'replace')
                varnames   ('self', 'fields')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__repr__'
-               firstlineno 437
+               firstlineno 438
                lnotab 0x02016001
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'dict', 'logging', 'Logger', '__init__', '__repr__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'EventLog'
-         firstlineno 416
+         firstlineno 417
          lnotab 0x0c0104071e0d
       'EventLog'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504640365056a06000000
             00000000006604880066016404840c5a07640584005a08880078015a0953
             00
                        0 MAKE_CELL                0 (__class__)
          
-         442           2 RESUME                   0
+         443           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('SharedTo')
                       10 STORE_NAME               2 (__qualname__)
          
-         443          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` single shared to\n\n    :param sharedto_data: :class:`dict` containing shared to data for :class:`Parcel`\n    :type sharedto_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
+         444          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` single shared to\n\n    :param sharedto_data: :class:`dict` containing shared to data for :class:`Parcel`\n    :type sharedto_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
                       14 STORE_NAME               3 (__doc__)
          
-         450          16 LOAD_CONST               2 ('sharedto_data')
+         451          16 LOAD_CONST               2 ('sharedto_data')
                       18 LOAD_NAME                4 (dict)
                       20 LOAD_CONST               3 ('logger')
                       22 LOAD_NAME                5 (logging)
                       24 LOAD_ATTR                6 (Logger)
                       34 BUILD_TUPLE              4
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
-                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 450>)
+                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 451>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               7 (__init__)
          
-         459          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 459>)
+         460          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 460>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (__repr__)
                       52 LOAD_CLOSURE             0 (__class__)
                       54 COPY                     1
                       56 STORE_NAME               9 (__classcell__)
                       58 RETURN_VALUE
          consts
@@ -4263,44 +4320,44 @@
                   03190000000000000000007c005f0200000000000000007c02a003000000
                   000000000000000000000000000000000089036a040000000000000000a6
                   010000ab0100000000000000007c005f0500000000000000007c006a0500
                   00000000000000a006000000000000000000000000000000000000000064
                   04a6010000ab010000000000000000010064055300
                              0 COPY_FREE_VARS           1
                
-               450           2 RESUME                   0
+               451           2 RESUME                   0
                
-               452           4 LOAD_FAST                1 (sharedto_data)
+               453           4 LOAD_FAST                1 (sharedto_data)
                              6 LOAD_CONST               1 ('uuid')
                              8 BINARY_SUBSCR
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               0 (uuid)
                
-               453          30 LOAD_FAST                1 (sharedto_data)
+               454          30 LOAD_FAST                1 (sharedto_data)
                             32 LOAD_CONST               2 ('name')
                             34 BINARY_SUBSCR
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (name)
                
-               454          56 LOAD_FAST                1 (sharedto_data)
+               455          56 LOAD_FAST                1 (sharedto_data)
                             58 LOAD_CONST               3 ('phoneNumber')
                             60 BINARY_SUBSCR
                             70 LOAD_FAST                0 (self)
                             72 STORE_ATTR               2 (phone_number)
                
-               456          82 LOAD_FAST                2 (logger)
+               457          82 LOAD_FAST                2 (logger)
                             84 LOAD_METHOD              3 (getChild)
                            106 LOAD_DEREF               3 (__class__)
                            108 LOAD_ATTR                4 (__name__)
                            118 PRECALL                  1
                            122 CALL                     1
                            132 LOAD_FAST                0 (self)
                            134 STORE_ATTR               5 (_log)
                
-               457         144 LOAD_FAST                0 (self)
+               458         144 LOAD_FAST                0 (self)
                            146 LOAD_ATTR                5 (_log)
                            156 LOAD_METHOD              6 (debug)
                            178 LOAD_CONST               4 ('created')
                            180 PRECALL                  1
                            184 CALL                     1
                            194 POP_TOP
                            196 LOAD_CONST               5 (None)
@@ -4314,15 +4371,15 @@
                   None
                names      ('uuid', 'name', 'phone_number', 'getChild', '__name__', '_log', 'debug')
                varnames   ('self', 'sharedto_data', 'logger')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
-               firstlineno 450
+               firstlineno 451
                lnotab 0x04021a011a011a023e01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 3
                code
@@ -4331,32 +4388,32 @@
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000007d017c006a0300000000000000006a0400000000000000
                   00740b00000000000000000000740100000000000000000000740d000000
                   000000000000007c01a6010000ab010000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000a00700000000000000
                   0000000000000000000000000064026403a6020000ab0200000000000000
                   007a0000005300
-               459           0 RESUME                   0
+               460           0 RESUME                   0
                
-               460           2 LOAD_GLOBAL              1 (NULL + tuple)
-                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 460>)
+               461           2 LOAD_GLOBAL              1 (NULL + tuple)
+                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 461>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (__dict__)
                             30 LOAD_METHOD              2 (items)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (fields)
                
-               461          98 LOAD_FAST                0 (self)
+               462          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (__class__)
                            110 LOAD_ATTR                4 (__name__)
                            120 LOAD_GLOBAL             11 (NULL + str)
                            132 LOAD_GLOBAL              1 (NULL + tuple)
                            144 LOAD_GLOBAL             13 (NULL + sorted)
                            156 LOAD_FAST                1 (fields)
                            158 PRECALL                  1
@@ -4378,15 +4435,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d145c0200007d017d027c0164006b0300000000af
                         0b7c019b0064017c029b009d035600970101008c1564025300
-                     460           0 RETURN_GENERATOR
+                     461           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                20 (to 50)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (k)
                                   16 STORE_FAST               2 (v)
@@ -4412,83 +4469,83 @@
                         None
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<genexpr>'
-                     firstlineno 460
+                     firstlineno 461
                      lnotab 0x
                   "'"
                   ''
                names      ('tuple', '__dict__', 'items', '__class__', '__name__', 'str', 'sorted', 'replace')
                varnames   ('self', 'fields')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__repr__'
-               firstlineno 459
+               firstlineno 460
                lnotab 0x02016001
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'dict', 'logging', 'Logger', '__init__', '__repr__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'SharedTo'
-         firstlineno 442
+         firstlineno 443
          lnotab 0x0c0104071e09
       'SharedTo'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504640365056a06000000
             00000000006604880066016404840c5a07640584005a0865096406650a66
             0264078404a6000000ab0000000000000000005a0b880078015a0c5300
                        0 MAKE_CELL                0 (__class__)
          
-         464           2 RESUME                   0
+         465           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('QRCode')
                       10 STORE_NAME               2 (__qualname__)
          
-         465          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` QRCode\n\n    :param qrcode_data: :class:`str` containing qrcode data for :class:`Parcel`\n    :type qrcode_data: str\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
+         466          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` QRCode\n\n    :param qrcode_data: :class:`str` containing qrcode data for :class:`Parcel`\n    :type qrcode_data: str\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
                       14 STORE_NAME               3 (__doc__)
          
-         472          16 LOAD_CONST               2 ('qrcode_data')
+         473          16 LOAD_CONST               2 ('qrcode_data')
                       18 LOAD_NAME                4 (str)
                       20 LOAD_CONST               3 ('logger')
                       22 LOAD_NAME                5 (logging)
                       24 LOAD_ATTR                6 (Logger)
                       34 BUILD_TUPLE              4
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
-                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 472>)
+                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 473>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               7 (__init__)
          
-         479          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 479>)
+         480          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 480>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (__repr__)
          
-         483          52 LOAD_NAME                9 (property)
+         484          52 LOAD_NAME                9 (property)
          
-         484          54 LOAD_CONST               6 ('return')
+         485          54 LOAD_CONST               6 ('return')
                       56 LOAD_NAME               10 (BytesIO)
                       58 BUILD_TUPLE              2
-                      60 LOAD_CONST               7 (<code object qr_image, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 483>)
+                      60 LOAD_CONST               7 (<code object qr_image, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 484>)
                       62 MAKE_FUNCTION            4 (annotations)
          
-         483          64 PRECALL                  0
+         484          64 PRECALL                  0
                       68 CALL                     0
          
-         484          78 STORE_NAME              11 (qr_image)
+         485          78 STORE_NAME              11 (qr_image)
                       80 LOAD_CLOSURE             0 (__class__)
                       82 COPY                     1
                       84 STORE_NAME              12 (__classcell__)
                       86 RETURN_VALUE
          consts
             'QRCode'
             'Object representation of :class:`Parcel` QRCode\n\n    :param qrcode_data: :class:`str` containing qrcode data for :class:`Parcel`\n    :type qrcode_data: str\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger'
@@ -4503,30 +4560,30 @@
                   0x950197007c017c005f0000000000000000007c02a00100000000000000
                   0000000000000000000000000089036a020000000000000000a6010000ab
                   0100000000000000007c005f0300000000000000007c006a030000000000
                   000000a00400000000000000000000000000000000000000006401a60100
                   00ab010000000000000000010064025300
                              0 COPY_FREE_VARS           1
                
-               472           2 RESUME                   0
+               473           2 RESUME                   0
                
-               474           4 LOAD_FAST                1 (qrcode_data)
+               475           4 LOAD_FAST                1 (qrcode_data)
                              6 LOAD_FAST                0 (self)
                              8 STORE_ATTR               0 (_qr_code)
                
-               476          18 LOAD_FAST                2 (logger)
+               477          18 LOAD_FAST                2 (logger)
                             20 LOAD_METHOD              1 (getChild)
                             42 LOAD_DEREF               3 (__class__)
                             44 LOAD_ATTR                2 (__name__)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (_log)
                
-               477          80 LOAD_FAST                0 (self)
+               478          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                3 (_log)
                             92 LOAD_METHOD              4 (debug)
                            114 LOAD_CONST               1 ('created')
                            116 PRECALL                  1
                            120 CALL                     1
                            130 POP_TOP
                            132 LOAD_CONST               2 (None)
@@ -4537,15 +4594,15 @@
                   None
                names      ('_qr_code', 'getChild', '__name__', '_log', 'debug')
                varnames   ('self', 'qrcode_data', 'logger')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
-               firstlineno 472
+               firstlineno 473
                lnotab 0x04020e023e01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 3
                code
@@ -4554,32 +4611,32 @@
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000007d017c006a0300000000000000006a0400000000000000
                   00740b00000000000000000000740100000000000000000000740d000000
                   000000000000007c01a6010000ab010000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000a00700000000000000
                   0000000000000000000000000064026403a6020000ab0200000000000000
                   007a0000005300
-               479           0 RESUME                   0
+               480           0 RESUME                   0
                
-               480           2 LOAD_GLOBAL              1 (NULL + tuple)
-                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 480>)
+               481           2 LOAD_GLOBAL              1 (NULL + tuple)
+                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 481>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (__dict__)
                             30 LOAD_METHOD              2 (items)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (fields)
                
-               481          98 LOAD_FAST                0 (self)
+               482          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (__class__)
                            110 LOAD_ATTR                4 (__name__)
                            120 LOAD_GLOBAL             11 (NULL + str)
                            132 LOAD_GLOBAL              1 (NULL + tuple)
                            144 LOAD_GLOBAL             13 (NULL + sorted)
                            156 LOAD_FAST                1 (fields)
                            158 PRECALL                  1
@@ -4601,15 +4658,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d145c0200007d017d027c0164006b0300000000af
                         0b7c019b0064017c029b009d035600970101008c1564025300
-                     480           0 RETURN_GENERATOR
+                     481           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                20 (to 50)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (k)
                                   16 STORE_FAST               2 (v)
@@ -4635,25 +4692,25 @@
                         None
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<genexpr>'
-                     firstlineno 480
+                     firstlineno 481
                      lnotab 0x
                   "'"
                   ''
                names      ('tuple', '__dict__', 'items', '__class__', '__name__', 'str', 'sorted', 'replace')
                varnames   ('self', 'fields')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__repr__'
-               firstlineno 479
+               firstlineno 480
                lnotab 0x02016001
             'return'
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 7
                flags     : 3
@@ -4670,102 +4727,102 @@
                   00000000007d02741500000000000000000000a6000000ab000000000000
                   0000007d03640c7c035f0b00000000000000007c02a00c00000000000000
                   000000000000000000000000007c03640da6020000ab0200000000000000
                   0001007c03a00d0000000000000000000000000000000000000000640ea6
                   010000ab01000000000000000001007c006a000000000000000000a00100
                   00000000000000000000000000000000000000640fa6010000ab01000000
                   000000000001007c035300
-               483           0 RESUME                   0
+               484           0 RESUME                   0
                
-               489           2 LOAD_FAST                0 (self)
+               490           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('generating qr image')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               490          54 LOAD_GLOBAL              5 (NULL + qrcode)
+               491          54 LOAD_GLOBAL              5 (NULL + qrcode)
                             66 LOAD_ATTR                3 (QRCode)
                
-               491          76 LOAD_CONST               2 (3)
+               492          76 LOAD_CONST               2 (3)
                
-               492          78 LOAD_GLOBAL              4 (qrcode)
+               493          78 LOAD_GLOBAL              4 (qrcode)
                             90 LOAD_ATTR                4 (constants)
                            100 LOAD_ATTR                5 (ERROR_CORRECT_H)
                
-               493         110 LOAD_CONST               3 (20)
+               494         110 LOAD_CONST               3 (20)
                
-               494         112 LOAD_CONST               4 (4)
+               495         112 LOAD_CONST               4 (4)
                
-               495         114 LOAD_CONST               5 (5)
+               496         114 LOAD_CONST               5 (5)
                
-               490         116 KW_NAMES                 6
+               491         116 KW_NAMES                 6
                            118 PRECALL                  5
                            122 CALL                     5
                            132 STORE_FAST               1 (qr)
                
-               498         134 LOAD_FAST                1 (qr)
+               499         134 LOAD_FAST                1 (qr)
                            136 LOAD_METHOD              6 (add_data)
                            158 LOAD_FAST                0 (self)
                            160 LOAD_ATTR                7 (_qr_code)
                            170 PRECALL                  1
                            174 CALL                     1
                            184 POP_TOP
                
-               499         186 LOAD_FAST                1 (qr)
+               500         186 LOAD_FAST                1 (qr)
                            188 LOAD_METHOD              8 (make)
                            210 LOAD_CONST               7 (False)
                            212 KW_NAMES                 8
                            214 PRECALL                  1
                            218 CALL                     1
                            228 POP_TOP
                
-               500         230 LOAD_FAST                1 (qr)
+               501         230 LOAD_FAST                1 (qr)
                            232 LOAD_METHOD              9 (make_image)
                            254 LOAD_CONST               9 ('black')
                            256 LOAD_CONST              10 ('white')
                            258 KW_NAMES                11
                            260 PRECALL                  2
                            264 CALL                     2
                            274 STORE_FAST               2 (img1)
                
-               501         276 LOAD_GLOBAL             21 (NULL + BytesIO)
+               502         276 LOAD_GLOBAL             21 (NULL + BytesIO)
                            288 PRECALL                  0
                            292 CALL                     0
                            302 STORE_FAST               3 (bio)
                
-               502         304 LOAD_CONST              12 ('qr.png')
+               503         304 LOAD_CONST              12 ('qr.png')
                            306 LOAD_FAST                3 (bio)
                            308 STORE_ATTR              11 (name)
                
-               503         318 LOAD_FAST                2 (img1)
+               504         318 LOAD_FAST                2 (img1)
                            320 LOAD_METHOD             12 (save)
                            342 LOAD_FAST                3 (bio)
                            344 LOAD_CONST              13 ('PNG')
                            346 PRECALL                  2
                            350 CALL                     2
                            360 POP_TOP
                
-               504         362 LOAD_FAST                3 (bio)
+               505         362 LOAD_FAST                3 (bio)
                            364 LOAD_METHOD             13 (seek)
                            386 LOAD_CONST              14 (0)
                            388 PRECALL                  1
                            392 CALL                     1
                            402 POP_TOP
                
-               505         404 LOAD_FAST                0 (self)
+               506         404 LOAD_FAST                0 (self)
                            406 LOAD_ATTR                0 (_log)
                            416 LOAD_METHOD              1 (debug)
                            438 LOAD_CONST              15 ('generated qr image')
                            440 PRECALL                  1
                            444 CALL                     1
                            454 POP_TOP
                
-               506         456 LOAD_FAST                3 (bio)
+               507         456 LOAD_FAST                3 (bio)
                            458 RETURN_VALUE
                consts
                   'Returns a generated QR image for :class:`QRCode`\n\n        :return: QR Code image\n        :rtype: BytesIO'
                   'generating qr image'
                   3
                   20
                   4
@@ -4782,60 +4839,60 @@
                   'generated qr image'
                names      ('_log', 'debug', 'qrcode', 'QRCode', 'constants', 'ERROR_CORRECT_H', 'add_data', '_qr_code', 'make', 'make_image', 'BytesIO', 'name', 'save', 'seek')
                varnames   ('self', 'qr', 'img1', 'bio')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'qr_image'
-               firstlineno 483
+               firstlineno 484
                lnotab
                   0x020634011601020120010201020102fb120834012c012e011c010e012c
                   012a013401
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', 'logging', 'Logger', '__init__', '__repr__', 'property', 'BytesIO', 'qr_image', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'QRCode'
-         firstlineno 464
+         firstlineno 465
          lnotab 0x0c0104071e07060402010aff0e01
       'QRCode'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504640365056a06000000
             00000000006604880066016404840c5a07640584005a08880078015a0953
             00
                        0 MAKE_CELL                0 (__class__)
          
-         509           2 RESUME                   0
+         510           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('CompartmentLocation')
                       10 STORE_NAME               2 (__qualname__)
          
-         510          12 LOAD_CONST               1 ('Object representation of :class:`CompartmentProperties` compartment location\n\n    :param compartmentlocation_data: :class:`dict` containing compartment location data for :class:`Parcel`\n    :type compartmentlocation_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
+         511          12 LOAD_CONST               1 ('Object representation of :class:`CompartmentProperties` compartment location\n\n    :param compartmentlocation_data: :class:`dict` containing compartment location data for :class:`Parcel`\n    :type compartmentlocation_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
                       14 STORE_NAME               3 (__doc__)
          
-         517          16 LOAD_CONST               2 ('compartmentlocation_data')
+         518          16 LOAD_CONST               2 ('compartmentlocation_data')
                       18 LOAD_NAME                4 (dict)
                       20 LOAD_CONST               3 ('logger')
                       22 LOAD_NAME                5 (logging)
                       24 LOAD_ATTR                6 (Logger)
                       34 BUILD_TUPLE              4
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
-                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 517>)
+                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 518>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               7 (__init__)
          
-         530          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 530>)
+         531          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 531>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (__repr__)
                       52 LOAD_CLOSURE             0 (__class__)
                       54 COPY                     1
                       56 STORE_NAME               9 (__classcell__)
                       58 RETURN_VALUE
          consts
@@ -4860,82 +4917,82 @@
                   00000000007c016409190000000000000000007c005f0600000000000000
                   007c02a007000000000000000000000000000000000000000089036a0800
                   00000000000000a6010000ab0100000000000000007c005f090000000000
                   0000007c006a090000000000000000a00a00000000000000000000000000
                   00000000000000640aa6010000ab0100000000000000000100640b5300
                              0 COPY_FREE_VARS           1
                
-               517           2 RESUME                   0
+               518           2 RESUME                   0
                
-               519           4 LOAD_FAST                1 (compartmentlocation_data)
+               520           4 LOAD_FAST                1 (compartmentlocation_data)
                              6 LOAD_CONST               1 ('compartment')
                              8 BINARY_SUBSCR
                             18 LOAD_CONST               2 ('name')
                             20 BINARY_SUBSCR
                             30 LOAD_FAST                0 (self)
                             32 STORE_ATTR               0 (name)
                
-               520          42 LOAD_FAST                1 (compartmentlocation_data)
+               521          42 LOAD_FAST                1 (compartmentlocation_data)
                             44 LOAD_CONST               1 ('compartment')
                             46 BINARY_SUBSCR
                             56 LOAD_CONST               3 ('location')
                             58 BINARY_SUBSCR
                             68 LOAD_CONST               4 ('side')
                             70 BINARY_SUBSCR
                             80 LOAD_FAST                0 (self)
                             82 STORE_ATTR               1 (side)
                
-               521          92 LOAD_FAST                1 (compartmentlocation_data)
+               522          92 LOAD_FAST                1 (compartmentlocation_data)
                             94 LOAD_CONST               1 ('compartment')
                             96 BINARY_SUBSCR
                            106 LOAD_CONST               3 ('location')
                            108 BINARY_SUBSCR
                            118 LOAD_CONST               5 ('column')
                            120 BINARY_SUBSCR
                            130 LOAD_FAST                0 (self)
                            132 STORE_ATTR               2 (column)
                
-               522         142 LOAD_FAST                1 (compartmentlocation_data)
+               523         142 LOAD_FAST                1 (compartmentlocation_data)
                            144 LOAD_CONST               1 ('compartment')
                            146 BINARY_SUBSCR
                            156 LOAD_CONST               3 ('location')
                            158 BINARY_SUBSCR
                            168 LOAD_CONST               6 ('row')
                            170 BINARY_SUBSCR
                            180 LOAD_FAST                0 (self)
                            182 STORE_ATTR               3 (row)
                
-               523         192 LOAD_FAST                1 (compartmentlocation_data)
+               524         192 LOAD_FAST                1 (compartmentlocation_data)
                            194 LOAD_CONST               7 ('openCompartmentWaitingTime')
                            196 BINARY_SUBSCR
                            206 LOAD_FAST                0 (self)
                            208 STORE_ATTR               4 (open_compartment_waiting_time)
                
-               524         218 LOAD_FAST                1 (compartmentlocation_data)
+               525         218 LOAD_FAST                1 (compartmentlocation_data)
                            220 LOAD_CONST               8 ('actionTime')
                            222 BINARY_SUBSCR
                            232 LOAD_FAST                0 (self)
                            234 STORE_ATTR               5 (action_time)
                
-               525         244 LOAD_FAST                1 (compartmentlocation_data)
+               526         244 LOAD_FAST                1 (compartmentlocation_data)
                            246 LOAD_CONST               9 ('confirmActionTime')
                            248 BINARY_SUBSCR
                            258 LOAD_FAST                0 (self)
                            260 STORE_ATTR               6 (confirm_action_time)
                
-               527         270 LOAD_FAST                2 (logger)
+               528         270 LOAD_FAST                2 (logger)
                            272 LOAD_METHOD              7 (getChild)
                            294 LOAD_DEREF               3 (__class__)
                            296 LOAD_ATTR                8 (__name__)
                            306 PRECALL                  1
                            310 CALL                     1
                            320 LOAD_FAST                0 (self)
                            322 STORE_ATTR               9 (_log)
                
-               528         332 LOAD_FAST                0 (self)
+               529         332 LOAD_FAST                0 (self)
                            334 LOAD_ATTR                9 (_log)
                            344 LOAD_METHOD             10 (debug)
                            366 LOAD_CONST              10 ('created')
                            368 PRECALL                  1
                            372 CALL                     1
                            382 POP_TOP
                            384 LOAD_CONST              11 (None)
@@ -4955,15 +5012,15 @@
                   None
                names      ('name', 'side', 'column', 'row', 'open_compartment_waiting_time', 'action_time', 'confirm_action_time', 'getChild', '__name__', '_log', 'debug')
                varnames   ('self', 'compartmentlocation_data', 'logger')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
-               firstlineno 517
+               firstlineno 518
                lnotab 0x040226013201320132011a011a011a023e01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 3
                code
@@ -4972,32 +5029,32 @@
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000007d017c006a0300000000000000006a0400000000000000
                   00740b00000000000000000000740100000000000000000000740d000000
                   000000000000007c01a6010000ab010000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000a00700000000000000
                   0000000000000000000000000064026403a6020000ab0200000000000000
                   007a0000005300
-               530           0 RESUME                   0
+               531           0 RESUME                   0
                
-               531           2 LOAD_GLOBAL              1 (NULL + tuple)
-                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 531>)
+               532           2 LOAD_GLOBAL              1 (NULL + tuple)
+                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 532>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (__dict__)
                             30 LOAD_METHOD              2 (items)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (fields)
                
-               532          98 LOAD_FAST                0 (self)
+               533          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (__class__)
                            110 LOAD_ATTR                4 (__name__)
                            120 LOAD_GLOBAL             11 (NULL + str)
                            132 LOAD_GLOBAL              1 (NULL + tuple)
                            144 LOAD_GLOBAL             13 (NULL + sorted)
                            156 LOAD_FAST                1 (fields)
                            158 PRECALL                  1
@@ -5019,15 +5076,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d145c0200007d017d027c0164006b0300000000af
                         0b7c019b0064017c029b009d035600970101008c1564025300
-                     531           0 RETURN_GENERATOR
+                     532           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                20 (to 50)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (k)
                                   16 STORE_FAST               2 (v)
@@ -5053,33 +5110,33 @@
                         None
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<genexpr>'
-                     firstlineno 531
+                     firstlineno 532
                      lnotab 0x
                   "'"
                   ''
                names      ('tuple', '__dict__', 'items', '__class__', '__name__', 'str', 'sorted', 'replace')
                varnames   ('self', 'fields')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__repr__'
-               firstlineno 530
+               firstlineno 531
                lnotab 0x02016001
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'dict', 'logging', 'Logger', '__init__', '__repr__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'CompartmentLocation'
-         firstlineno 509
+         firstlineno 510
          lnotab 0x0c0104071e0d
       'CompartmentLocation'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
@@ -5089,98 +5146,98 @@
             000000ab0000000000000000005a0a650964078400a6000000ab00000000
             00000000005a0b650b6a0c000000000000000064086504660264098404a6
             000000ab0000000000000000005a0b6509640a8400a6000000ab00000000
             00000000005a0d650d6a0c0000000000000000640b650e650f7a07000066
             02640c8404a6000000ab0000000000000000005a0d880078015a105300
                        0 MAKE_CELL                0 (__class__)
          
-         535           2 RESUME                   0
+         536           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('CompartmentProperties')
                       10 STORE_NAME               2 (__qualname__)
          
-         536          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` compartment properties\n\n    :param compartmentproperties_data: :class:`dict` containing compartment properties data for :class:`Parcel`\n    :type compartmentproperties_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
+         537          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` compartment properties\n\n    :param compartmentproperties_data: :class:`dict` containing compartment properties data for :class:`Parcel`\n    :type compartmentproperties_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
                       14 STORE_NAME               3 (__doc__)
          
-         543          16 LOAD_CONST               2 ('compartmentproperties_data')
+         544          16 LOAD_CONST               2 ('compartmentproperties_data')
                       18 LOAD_NAME                4 (dict)
                       20 LOAD_CONST               3 ('logger')
                       22 LOAD_NAME                5 (logging)
                       24 LOAD_ATTR                6 (Logger)
                       34 BUILD_TUPLE              4
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
-                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 543>)
+                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 544>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               7 (__init__)
          
-         553          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 553>)
+         554          46 LOAD_CONST               5 (<code object __repr__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 554>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (__repr__)
          
-         557          52 LOAD_NAME                9 (property)
+         558          52 LOAD_NAME                9 (property)
          
-         558          54 LOAD_CONST               6 (<code object session_uuid, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 557>)
+         559          54 LOAD_CONST               6 (<code object session_uuid, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 558>)
                       56 MAKE_FUNCTION            0
          
-         557          58 PRECALL                  0
+         558          58 PRECALL                  0
                       62 CALL                     0
          
-         558          72 STORE_NAME              10 (session_uuid)
+         559          72 STORE_NAME              10 (session_uuid)
          
-         566          74 LOAD_NAME                9 (property)
+         567          74 LOAD_NAME                9 (property)
          
-         567          76 LOAD_CONST               7 (<code object location, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 566>)
+         568          76 LOAD_CONST               7 (<code object location, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 567>)
                       78 MAKE_FUNCTION            0
          
-         566          80 PRECALL                  0
+         567          80 PRECALL                  0
                       84 CALL                     0
          
-         567          94 STORE_NAME              11 (location)
+         568          94 STORE_NAME              11 (location)
          
-         575          96 LOAD_NAME               11 (location)
+         576          96 LOAD_NAME               11 (location)
                       98 LOAD_ATTR               12 (setter)
          
-         576         108 LOAD_CONST               8 ('location_data')
+         577         108 LOAD_CONST               8 ('location_data')
                      110 LOAD_NAME                4 (dict)
                      112 BUILD_TUPLE              2
-                     114 LOAD_CONST               9 (<code object location, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 575>)
+                     114 LOAD_CONST               9 (<code object location, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 576>)
                      116 MAKE_FUNCTION            4 (annotations)
          
-         575         118 PRECALL                  0
+         576         118 PRECALL                  0
                      122 CALL                     0
          
-         576         132 STORE_NAME              11 (location)
+         577         132 STORE_NAME              11 (location)
          
-         584         134 LOAD_NAME                9 (property)
+         585         134 LOAD_NAME                9 (property)
          
-         585         136 LOAD_CONST              10 (<code object status, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 584>)
+         586         136 LOAD_CONST              10 (<code object status, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 585>)
                      138 MAKE_FUNCTION            0
          
-         584         140 PRECALL                  0
+         585         140 PRECALL                  0
                      144 CALL                     0
          
-         585         154 STORE_NAME              13 (status)
+         586         154 STORE_NAME              13 (status)
          
-         593         156 LOAD_NAME               13 (status)
+         594         156 LOAD_NAME               13 (status)
                      158 LOAD_ATTR               12 (setter)
          
-         594         168 LOAD_CONST              11 ('status_data')
+         595         168 LOAD_CONST              11 ('status_data')
                      170 LOAD_NAME               14 (str)
                      172 LOAD_NAME               15 (CompartmentActualStatus)
                      174 BINARY_OP                7 (|)
                      178 BUILD_TUPLE              2
-                     180 LOAD_CONST              12 (<code object status, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 593>)
+                     180 LOAD_CONST              12 (<code object status, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 594>)
                      182 MAKE_FUNCTION            4 (annotations)
          
-         593         184 PRECALL                  0
+         594         184 PRECALL                  0
                      188 CALL                     0
          
-         594         198 STORE_NAME              13 (status)
+         595         198 STORE_NAME              13 (status)
                      200 LOAD_CLOSURE             0 (__class__)
                      202 COPY                     1
                      204 STORE_NAME              16 (__classcell__)
                      206 RETURN_VALUE
          consts
             'CompartmentProperties'
             'Object representation of :class:`Parcel` compartment properties\n\n    :param compartmentproperties_data: :class:`dict` containing compartment properties data for :class:`Parcel`\n    :type compartmentproperties_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger'
@@ -5197,46 +5254,46 @@
                   005f02000000000000000064037c005f0300000000000000007c02a00400
                   0000000000000000000000000000000000000089036a0500000000000000
                   00a6010000ab0100000000000000007c005f0600000000000000007c006a
                   060000000000000000a00700000000000000000000000000000000000000
                   006404a6010000ab010000000000000000010064035300
                              0 COPY_FREE_VARS           1
                
-               543           2 RESUME                   0
+               544           2 RESUME                   0
                
-               545           4 LOAD_FAST                1 (compartmentproperties_data)
+               546           4 LOAD_FAST                1 (compartmentproperties_data)
                              6 LOAD_CONST               1 ('sessionUuid')
                              8 BINARY_SUBSCR
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               0 (_session_uuid)
                
-               546          30 LOAD_FAST                1 (compartmentproperties_data)
+               547          30 LOAD_FAST                1 (compartmentproperties_data)
                             32 LOAD_CONST               2 ('sessionExpirationTime')
                             34 BINARY_SUBSCR
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (_session_expiration_time)
                
-               547          56 LOAD_CONST               3 (None)
+               548          56 LOAD_CONST               3 (None)
                             58 LOAD_FAST                0 (self)
                             60 STORE_ATTR               2 (_location)
                
-               548          70 LOAD_CONST               3 (None)
+               549          70 LOAD_CONST               3 (None)
                             72 LOAD_FAST                0 (self)
                             74 STORE_ATTR               3 (_status)
                
-               550          84 LOAD_FAST                2 (logger)
+               551          84 LOAD_FAST                2 (logger)
                             86 LOAD_METHOD              4 (getChild)
                            108 LOAD_DEREF               3 (__class__)
                            110 LOAD_ATTR                5 (__name__)
                            120 PRECALL                  1
                            124 CALL                     1
                            134 LOAD_FAST                0 (self)
                            136 STORE_ATTR               6 (_log)
                
-               551         146 LOAD_FAST                0 (self)
+               552         146 LOAD_FAST                0 (self)
                            148 LOAD_ATTR                6 (_log)
                            158 LOAD_METHOD              7 (debug)
                            180 LOAD_CONST               4 ('created')
                            182 PRECALL                  1
                            186 CALL                     1
                            196 POP_TOP
                            198 LOAD_CONST               3 (None)
@@ -5249,15 +5306,15 @@
                   'created'
                names      ('_session_uuid', '_session_expiration_time', '_location', '_status', 'getChild', '__name__', '_log', 'debug')
                varnames   ('self', 'compartmentproperties_data', 'logger')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
-               firstlineno 543
+               firstlineno 544
                lnotab 0x04021a011a010e010e023e01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 8
                flags     : 3
                code
@@ -5266,32 +5323,32 @@
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000007d017c006a0300000000000000006a0400000000000000
                   00740b00000000000000000000740100000000000000000000740d000000
                   000000000000007c01a6010000ab010000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000a00700000000000000
                   0000000000000000000000000064026403a6020000ab0200000000000000
                   007a0000005300
-               553           0 RESUME                   0
+               554           0 RESUME                   0
                
-               554           2 LOAD_GLOBAL              1 (NULL + tuple)
-                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 554>)
+               555           2 LOAD_GLOBAL              1 (NULL + tuple)
+                            14 LOAD_CONST               1 (<code object <genexpr>, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 555>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (__dict__)
                             30 LOAD_METHOD              2 (items)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (fields)
                
-               555          98 LOAD_FAST                0 (self)
+               556          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                3 (__class__)
                            110 LOAD_ATTR                4 (__name__)
                            120 LOAD_GLOBAL             11 (NULL + str)
                            132 LOAD_GLOBAL              1 (NULL + tuple)
                            144 LOAD_GLOBAL             13 (NULL + sorted)
                            156 LOAD_FAST                1 (fields)
                            158 PRECALL                  1
@@ -5313,15 +5370,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d145c0200007d017d027c0164006b0300000000af
                         0b7c019b0064017c029b009d035600970101008c1564025300
-                     554           0 RETURN_GENERATOR
+                     555           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                20 (to 50)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (k)
                                   16 STORE_FAST               2 (v)
@@ -5347,114 +5404,114 @@
                         None
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                      name       '<genexpr>'
-                     firstlineno 554
+                     firstlineno 555
                      lnotab 0x
                   "'"
                   ''
                names      ('tuple', '__dict__', 'items', '__class__', '__name__', 'str', 'sorted', 'replace')
                varnames   ('self', 'fields')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__repr__'
-               firstlineno 553
+               firstlineno 554
                lnotab 0x02016001
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab01000000000000000001007c006a0200
                   000000000000005300
-               557           0 RESUME                   0
+               558           0 RESUME                   0
                
-               563           2 LOAD_FAST                0 (self)
+               564           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('getting session uuid')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               564          54 LOAD_FAST                0 (self)
+               565          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (_session_uuid)
                             66 RETURN_VALUE
                consts
                   'Returns a session unique identified for :class:`CompartmentProperties`\n\n        :return: string containing session unique identified for :class:`CompartmentProperties`\n        :rtype: str'
                   'getting session uuid'
                names      ('_log', 'debug', '_session_uuid')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'session_uuid'
-               firstlineno 557
+               firstlineno 558
                lnotab 0x02063401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab01000000000000000001007c006a0200
                   000000000000005300
-               566           0 RESUME                   0
+               567           0 RESUME                   0
                
-               572           2 LOAD_FAST                0 (self)
+               573           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('getting location')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               573          54 LOAD_FAST                0 (self)
+               574          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (_location)
                             66 RETURN_VALUE
                consts
                   'Returns a compartment location for :class:`CompartmentProperties`\n\n        :return: compartment location for :class:`CompartmentProperties`\n        :rtype: str'
                   'getting location'
                names      ('_log', 'debug', '_location')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'location'
-               firstlineno 566
+               firstlineno 567
                lnotab 0x02063401
             'location_data'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab01000000000000000001007405000000
                   000000000000007c017c006a000000000000000000a6020000ab02000000
                   00000000007c005f03000000000000000064025300
-               575           0 RESUME                   0
+               576           0 RESUME                   0
                
-               581           2 LOAD_FAST                0 (self)
+               582           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('setting location')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               582          54 LOAD_GLOBAL              5 (NULL + CompartmentLocation)
+               583          54 LOAD_GLOBAL              5 (NULL + CompartmentLocation)
                             66 LOAD_FAST                1 (location_data)
                             68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                0 (_log)
                             80 PRECALL                  2
                             84 CALL                     2
                             94 LOAD_FAST                0 (self)
                             96 STORE_ATTR               3 (_location)
@@ -5466,48 +5523,48 @@
                   None
                names      ('_log', 'debug', 'CompartmentLocation', '_location')
                varnames   ('self', 'location_data')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'location'
-               firstlineno 575
+               firstlineno 576
                lnotab 0x02063401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab01000000000000000001007c006a0200
                   000000000000005300
-               584           0 RESUME                   0
+               585           0 RESUME                   0
                
-               590           2 LOAD_FAST                0 (self)
+               591           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('getting status')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               591          54 LOAD_FAST                0 (self)
+               592          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (_status)
                             66 RETURN_VALUE
                consts
                   'Returns a compartment status for :class:`CompartmentProperties`\n\n        :return: compartment location for :class:`CompartmentProperties`\n        :rtype: CompartmentActualStatus'
                   'getting status'
                names      ('_log', 'debug', '_status')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'status'
-               firstlineno 584
+               firstlineno 585
                lnotab 0x02063401
             'status_data'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
@@ -5518,121 +5575,121 @@
                   000000000072027c016e0c7406000000000000000000007c011900000000
                   00000000007c005f0400000000000000007c006a04000000000000000074
                   06000000000000000000006a0500000000000000006b0200000000723474
                   05000000000000000000007c01740c00000000000000000000a6020000ab
                   02000000000000000072217c006a000000000000000000a0010000000000
                   00000000000000000000000000000064027c019b009d02a6010000ab0100
                   000000000000000100640053006400530064005300
-               593           0 RESUME                   0
+               594           0 RESUME                   0
                
-               595           2 LOAD_FAST                0 (self)
+               596           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_log)
                             14 LOAD_METHOD              1 (debug)
                             36 LOAD_CONST               1 ('setting status')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               596          54 LOAD_GLOBAL              5 (NULL + isinstance)
+               597          54 LOAD_GLOBAL              5 (NULL + isinstance)
                             66 LOAD_FAST                1 (status_data)
                             68 LOAD_GLOBAL              6 (CompartmentActualStatus)
                             80 PRECALL                  2
                             84 CALL                     2
                             94 POP_JUMP_FORWARD_IF_FALSE     2 (to 100)
                             96 LOAD_FAST                1 (status_data)
                             98 JUMP_FORWARD            12 (to 124)
                
-               597     >>  100 LOAD_GLOBAL              6 (CompartmentActualStatus)
+               598     >>  100 LOAD_GLOBAL              6 (CompartmentActualStatus)
                            112 LOAD_FAST                1 (status_data)
                            114 BINARY_SUBSCR
                
-               596     >>  124 LOAD_FAST                0 (self)
+               597     >>  124 LOAD_FAST                0 (self)
                            126 STORE_ATTR               4 (_status)
                
-               599         136 LOAD_FAST                0 (self)
+               600         136 LOAD_FAST                0 (self)
                            138 LOAD_ATTR                4 (_status)
                            148 LOAD_GLOBAL              6 (CompartmentActualStatus)
                            160 LOAD_ATTR                5 (UNKNOWN)
                            170 COMPARE_OP               2 (==)
                            176 POP_JUMP_FORWARD_IF_FALSE    52 (to 282)
                            178 LOAD_GLOBAL              5 (NULL + isinstance)
                            190 LOAD_FAST                1 (status_data)
                            192 LOAD_GLOBAL             12 (str)
                            204 PRECALL                  2
                            208 CALL                     2
                            218 POP_JUMP_FORWARD_IF_FALSE    33 (to 286)
                
-               600         220 LOAD_FAST                0 (self)
+               601         220 LOAD_FAST                0 (self)
                            222 LOAD_ATTR                0 (_log)
                            232 LOAD_METHOD              1 (debug)
                            254 LOAD_CONST               2 ('unexpected compartment actual status: ')
                            256 LOAD_FAST                1 (status_data)
                            258 FORMAT_VALUE             0
                            260 BUILD_STRING             2
                            262 PRECALL                  1
                            266 CALL                     1
                            276 POP_TOP
                            278 LOAD_CONST               0 (None)
                            280 RETURN_VALUE
                
-               599     >>  282 LOAD_CONST               0 (None)
+               600     >>  282 LOAD_CONST               0 (None)
                            284 RETURN_VALUE
                        >>  286 LOAD_CONST               0 (None)
                            288 RETURN_VALUE
                consts
                   None
                   'setting status'
                   'unexpected compartment actual status: '
                names      ('_log', 'debug', 'isinstance', 'CompartmentActualStatus', '_status', 'UNKNOWN', 'str')
                varnames   ('self', 'status_data')
                freevars   ()
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       'status'
-               firstlineno 593
+               firstlineno 594
                lnotab 0x020234012e0118ff0c0354013eff
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'dict', 'logging', 'Logger', '__init__', '__repr__', 'property', 'session_uuid', 'location', 'setter', 'status', 'str', 'CompartmentActualStatus', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'CompartmentProperties'
-         firstlineno 535
+         firstlineno 536
          lnotab
             0x0c0104071e0a0604020104ff0e010208020104ff0e0102080c010aff0e
             010208020104ff0e0102080c0110ff0e01
       'CompartmentProperties'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504640365056a06000000
             00000000006604880066016404840c5a07880078015a085300
                        0 MAKE_CELL                0 (__class__)
          
-         603           2 RESUME                   0
+         604           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AirSensorData')
                       10 STORE_NAME               2 (__qualname__)
          
-         604          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` air sensor data\n\n    :param airsensor_data: :class:`dict` containing air sensor data for :class:`Parcel`\n    :type airsensor_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
+         605          12 LOAD_CONST               1 ('Object representation of :class:`Parcel` air sensor data\n\n    :param airsensor_data: :class:`dict` containing air sensor data for :class:`Parcel`\n    :type airsensor_data: dict\n    :param logger: :class:`logging.Logger` parent instance\n    :type logger: logging.Logger')
                       14 STORE_NAME               3 (__doc__)
          
-         610          16 LOAD_CONST               2 ('airsensor_data')
+         611          16 LOAD_CONST               2 ('airsensor_data')
                       18 LOAD_NAME                4 (dict)
                       20 LOAD_CONST               3 ('logger')
                       22 LOAD_NAME                5 (logging)
                       24 LOAD_ATTR                6 (Logger)
                       34 BUILD_TUPLE              4
                       36 LOAD_CLOSURE             0 (__class__)
                       38 BUILD_TUPLE              1
-                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 610>)
+                      40 LOAD_CONST               4 (<code object __init__, file "/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py", line 611>)
                       42 MAKE_FUNCTION           12 (annotations, closure)
                       44 STORE_NAME               7 (__init__)
                       46 LOAD_CLOSURE             0 (__class__)
                       48 COPY                     1
                       50 STORE_NAME               8 (__classcell__)
                       52 RETURN_VALUE
          consts
@@ -5660,96 +5717,96 @@
                   00000000007c02a009000000000000000000000000000000000000000089
                   036a0a0000000000000000a6010000ab0100000000000000007c005f0b00
                   000000000000007c006a0b0000000000000000a00c000000000000000000
                   0000000000000000000000640ba6010000ab010000000000000000010064
                   005300
                              0 COPY_FREE_VARS           1
                
-               610           2 RESUME                   0
+               611           2 RESUME                   0
                
-               611           4 LOAD_FAST                1 (airsensor_data)
+               612           4 LOAD_FAST                1 (airsensor_data)
                              6 LOAD_CONST               1 ('updatedUntil')
                              8 BINARY_SUBSCR
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               0 (updated_until)
                
-               612          30 LOAD_FAST                1 (airsensor_data)
+               613          30 LOAD_FAST                1 (airsensor_data)
                             32 LOAD_CONST               2 ('airQuality')
                             34 BINARY_SUBSCR
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (air_quality)
                
-               613          56 LOAD_FAST                1 (airsensor_data)
+               614          56 LOAD_FAST                1 (airsensor_data)
                             58 LOAD_CONST               3 ('temperature')
                             60 BINARY_SUBSCR
                             70 LOAD_FAST                0 (self)
                             72 STORE_ATTR               2 (temperature)
                
-               614          82 LOAD_FAST                1 (airsensor_data)
+               615          82 LOAD_FAST                1 (airsensor_data)
                             84 LOAD_CONST               4 ('humidity')
                             86 BINARY_SUBSCR
                             96 LOAD_FAST                0 (self)
                             98 STORE_ATTR               3 (humidity)
                
-               615         108 LOAD_FAST                1 (airsensor_data)
+               616         108 LOAD_FAST                1 (airsensor_data)
                            110 LOAD_CONST               5 ('pressure')
                            112 BINARY_SUBSCR
                            122 LOAD_FAST                0 (self)
                            124 STORE_ATTR               4 (pressure)
                
-               616         134 LOAD_FAST                1 (airsensor_data)
+               617         134 LOAD_FAST                1 (airsensor_data)
                            136 LOAD_CONST               6 ('pollutants')
                            138 BINARY_SUBSCR
                            148 LOAD_CONST               7 ('pm25')
                            150 BINARY_SUBSCR
                            160 LOAD_CONST               8 ('value')
                            162 BINARY_SUBSCR
                            172 LOAD_FAST                0 (self)
                            174 STORE_ATTR               5 (pm25_value)
                
-               617         184 LOAD_FAST                1 (airsensor_data)
+               618         184 LOAD_FAST                1 (airsensor_data)
                            186 LOAD_CONST               6 ('pollutants')
                            188 BINARY_SUBSCR
                            198 LOAD_CONST               7 ('pm25')
                            200 BINARY_SUBSCR
                            210 LOAD_CONST               9 ('percent')
                            212 BINARY_SUBSCR
                            222 LOAD_FAST                0 (self)
                            224 STORE_ATTR               6 (pm25_percent)
                
-               618         234 LOAD_FAST                1 (airsensor_data)
+               619         234 LOAD_FAST                1 (airsensor_data)
                            236 LOAD_CONST               6 ('pollutants')
                            238 BINARY_SUBSCR
                            248 LOAD_CONST              10 ('pm10')
                            250 BINARY_SUBSCR
                            260 LOAD_CONST               8 ('value')
                            262 BINARY_SUBSCR
                            272 LOAD_FAST                0 (self)
                            274 STORE_ATTR               7 (pm10_value)
                
-               619         284 LOAD_FAST                1 (airsensor_data)
+               620         284 LOAD_FAST                1 (airsensor_data)
                            286 LOAD_CONST               6 ('pollutants')
                            288 BINARY_SUBSCR
                            298 LOAD_CONST              10 ('pm10')
                            300 BINARY_SUBSCR
                            310 LOAD_CONST               9 ('percent')
                            312 BINARY_SUBSCR
                            322 LOAD_FAST                0 (self)
                            324 STORE_ATTR               8 (pm10_percent)
                
-               621         334 LOAD_FAST                2 (logger)
+               622         334 LOAD_FAST                2 (logger)
                            336 LOAD_METHOD              9 (getChild)
                            358 LOAD_DEREF               3 (__class__)
                            360 LOAD_ATTR               10 (__name__)
                            370 PRECALL                  1
                            374 CALL                     1
                            384 LOAD_FAST                0 (self)
                            386 STORE_ATTR              11 (_log)
                
-               622         396 LOAD_FAST                0 (self)
+               623         396 LOAD_FAST                0 (self)
                            398 LOAD_ATTR               11 (_log)
                            408 LOAD_METHOD             12 (debug)
                            430 LOAD_CONST              11 ('created')
                            432 PRECALL                  1
                            436 CALL                     1
                            446 POP_TOP
                            448 LOAD_CONST               0 (None)
@@ -5769,28 +5826,28 @@
                   'created'
                names      ('updated_until', 'air_quality', 'temperature', 'humidity', 'pressure', 'pm25_value', 'pm25_percent', 'pm10_value', 'pm10_percent', 'getChild', '__name__', '_log', 'debug')
                varnames   ('self', 'airsensor_data', 'logger')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
                name       '__init__'
-               firstlineno 610
+               firstlineno 611
                lnotab 0x04011a011a011a011a011a0132013201320132023e01
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'dict', 'logging', 'Logger', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
          name       'AirSensorData'
-         firstlineno 603
+         firstlineno 604
          lnotab 0x0c010406
       'AirSensorData'
    names      ('logging', 'random', 'io', 'BytesIO', 'typing', 'List', 'Tuple', 'qrcode', 'arrow', 'get', 'inpost.static.statuses', 'BaseParcel', 'Parcel', 'ReturnParcel', 'Receiver', 'Sender', 'PickupPoint', 'MultiCompartment', 'Operations', 'EventLog', 'SharedTo', 'QRCode', 'CompartmentLocation', 'CompartmentProperties', 'AirSensorData')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/loobson/pyprojects/inpost-python/inpost/static/parcels.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080108010c0110020801100208031a0b1c7f00601c0f1a161a
+      0x00ff0201080108010c0110020801100208031a0b1c7f00611c0f1a161a
       171a351a181a211a1a1a161a2d1a1a1a44
```

### Comparing `inpost-0.1.0/inpost/static/__pycache__/statuses.cpython-310.pyc` & `inpost-0.1.1/inpost/static/__pycache__/statuses.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/__pycache__/statuses.cpython-311.pyc` & `inpost-0.1.1/inpost/static/__pycache__/statuses.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x25c56364 (Tue May 16 18:02:13 2023 UTC)
-files sz: 7735
+moddate:  0x63c56364 (Tue May 16 18:03:15 2023 UTC)
+files sz: 7066
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -128,57 +128,57 @@
                264 MAKE_FUNCTION            0
                266 LOAD_CONST              21 ('ParcelStatus')
                268 LOAD_NAME                6 (ParcelBase)
                270 PRECALL                  3
                274 CALL                     3
                284 STORE_NAME              13 (ParcelStatus)
    
-   172         286 PUSH_NULL
+   163         286 PUSH_NULL
                288 LOAD_BUILD_CLASS
-               290 LOAD_CONST              22 (<code object ReturnsStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 172>)
+               290 LOAD_CONST              22 (<code object ReturnsStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 163>)
                292 MAKE_FUNCTION            0
                294 LOAD_CONST              23 ('ReturnsStatus')
                296 LOAD_NAME                6 (ParcelBase)
                298 PRECALL                  3
                302 CALL                     3
                312 STORE_NAME              14 (ReturnsStatus)
    
-   179         314 PUSH_NULL
+   170         314 PUSH_NULL
                316 LOAD_BUILD_CLASS
-               318 LOAD_CONST              24 (<code object ParcelOwnership, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 179>)
+               318 LOAD_CONST              24 (<code object ParcelOwnership, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 170>)
                320 MAKE_FUNCTION            0
                322 LOAD_CONST              25 ('ParcelOwnership')
                324 LOAD_NAME                6 (ParcelBase)
                326 PRECALL                  3
                330 CALL                     3
                340 STORE_NAME              15 (ParcelOwnership)
    
-   187         342 PUSH_NULL
+   178         342 PUSH_NULL
                344 LOAD_BUILD_CLASS
-               346 LOAD_CONST              26 (<code object CompartmentExpectedStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 187>)
+               346 LOAD_CONST              26 (<code object CompartmentExpectedStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 178>)
                348 MAKE_FUNCTION            0
                350 LOAD_CONST              27 ('CompartmentExpectedStatus')
                352 LOAD_NAME                6 (ParcelBase)
                354 PRECALL                  3
                358 CALL                     3
                368 STORE_NAME              16 (CompartmentExpectedStatus)
    
-   194         370 PUSH_NULL
+   185         370 PUSH_NULL
                372 LOAD_BUILD_CLASS
-               374 LOAD_CONST              28 (<code object CompartmentActualStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 194>)
+               374 LOAD_CONST              28 (<code object CompartmentActualStatus, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 185>)
                376 MAKE_FUNCTION            0
                378 LOAD_CONST              29 ('CompartmentActualStatus')
                380 LOAD_NAME                6 (ParcelBase)
                382 PRECALL                  3
                386 CALL                     3
                396 STORE_NAME              17 (CompartmentActualStatus)
    
-   201         398 PUSH_NULL
+   192         398 PUSH_NULL
                400 LOAD_BUILD_CLASS
-               402 LOAD_CONST              30 (<code object ParcelServiceName, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 201>)
+               402 LOAD_CONST              30 (<code object ParcelServiceName, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 192>)
                404 MAKE_FUNCTION            0
                406 LOAD_CONST              31 ('ParcelServiceName')
                408 LOAD_NAME                6 (ParcelBase)
                410 PRECALL                  3
                414 CALL                     3
                424 STORE_NAME              18 (ParcelServiceName)
                426 LOAD_CONST              32 (None)
@@ -1132,25 +1132,24 @@
          name       'ParcelType'
          firstlineno 108
          lnotab 0x0a010401040104010401
       'ParcelType'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 3
+         stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
             0764065a0864075a0964085a0a64095a0b640a5a0c640b5a0d640c5a0e64
             0d5a0f640e5a10640f5a1164105a1264115a1364125a1464135a1564145a
             1664155a1764165a1864175a1964185a1a64195a1b641a5a1c641b5a1d64
             1c5a1e641d5a1f641e5a2064135a21641f5a2264205a2364215a2464225a
             2564235a2664245a2764255a2864265a2964125a2a64275a2b64285a2c64
-            295a2d642a5a2e642b652f6400190000000000000000006602642c84045a
-            30642d5300
+            295a2d642a5a2e642b5300
          116           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParcelStatus')
                        8 STORE_NAME               2 (__qualname__)
          
          117          10 LOAD_CONST               1 (':class:`Enum` that holds parcel statuses')
@@ -1280,25 +1279,16 @@
                      176 STORE_NAME              44 (UNDELIVERED_COD_CASH_RECEIVER)
          
          159         178 LOAD_CONST              41 ('Przekierowana do paczkomatu')
                      180 STORE_NAME              45 (REDIRECT_TO_BOX)
          
          160         182 LOAD_CONST              42 ('Anulowano przekierowanie do paczkomatu')
                      184 STORE_NAME              46 (CANCELED_REDIRECT_TO_BOX)
-         
-         162         186 LOAD_CONST              43 ('return')
-                     188 LOAD_NAME               47 (List)
-                     190 LOAD_CONST               0 ('ParcelStatus')
-                     192 BINARY_SUBSCR
-                     202 BUILD_TUPLE              2
-                     204 LOAD_CONST              44 (<code object pending, file "/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py", line 162>)
-                     206 MAKE_FUNCTION            4 (annotations)
-                     208 STORE_NAME              48 (pending)
-                     210 LOAD_CONST              45 (None)
-                     212 RETURN_VALUE
+                     186 LOAD_CONST              43 (None)
+                     188 RETURN_VALUE
          consts
             'ParcelStatus'
             ':class:`Enum` that holds parcel statuses'
             'UNKNOWN DATA'
             'Utworzona'
             'Oferty przygotowane'
             'Oferta wybrana'
@@ -1335,119 +1325,51 @@
             'Odebrana z paczkomatu'
             'Przyjęta w sortowni'
             'Gotowa do doręczenia'
             'Nie dostarczono z powodu złego adresu'
             'Nie dostarczono z powodu nieopłacenia'
             'Przekierowana do paczkomatu'
             'Anulowano przekierowanie do paczkomatu'
-            'return'
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 14
-               flags     : 3
-               code
-                  0x97007400000000000000000000006a0100000000000000007400000000
-                  000000000000006a0200000000000000007400000000000000000000006a
-                  0300000000000000007400000000000000000000006a0400000000000000
-                  007400000000000000000000006a05000000000000000074000000000000
-                  00000000006a0600000000000000007400000000000000000000006a0700
-                  000000000000007400000000000000000000006a08000000000000000074
-                  00000000000000000000006a090000000000000000740000000000000000
-                  0000006a0a00000000000000007400000000000000000000006a0b000000
-                  00000000007400000000000000000000006a0c0000000000000000740000
-                  0000000000000000006a0d00000000000000007400000000000000000000
-                  006a0e0000000000000000670e5300
-               162           0 RESUME                   0
-               
-               163           2 LOAD_GLOBAL              0 (ParcelStatus)
-                            14 LOAD_ATTR                1 (READY_TO_PICKUP)
-                            24 LOAD_GLOBAL              0 (ParcelStatus)
-                            36 LOAD_ATTR                2 (CONFIRMED)
-               
-               164          46 LOAD_GLOBAL              0 (ParcelStatus)
-                            58 LOAD_ATTR                3 (ADOPTED_AT_SORTING_CENTER)
-                            68 LOAD_GLOBAL              0 (ParcelStatus)
-                            80 LOAD_ATTR                4 (ADOPTED_AT_SOURCE_BRANCH)
-               
-               165          90 LOAD_GLOBAL              0 (ParcelStatus)
-                           102 LOAD_ATTR                5 (COLLECTED_FROM_SENDER)
-                           112 LOAD_GLOBAL              0 (ParcelStatus)
-                           124 LOAD_ATTR                6 (DISPATCHED_BY_SENDER)
-               
-               166         134 LOAD_GLOBAL              0 (ParcelStatus)
-                           146 LOAD_ATTR                7 (DISPATCHED_BY_SENDER_TO_POK)
-                           156 LOAD_GLOBAL              0 (ParcelStatus)
-                           168 LOAD_ATTR                8 (OUT_FOR_DELIVERY)
-               
-               167         178 LOAD_GLOBAL              0 (ParcelStatus)
-                           190 LOAD_ATTR                9 (OUT_FOR_DELIVERY_TO_ADDRESS)
-                           200 LOAD_GLOBAL              0 (ParcelStatus)
-                           212 LOAD_ATTR               10 (SENT_FROM_SOURCE_BRANCH)
-               
-               168         222 LOAD_GLOBAL              0 (ParcelStatus)
-                           234 LOAD_ATTR               11 (TAKEN_BY_COURIER)
-                           244 LOAD_GLOBAL              0 (ParcelStatus)
-                           256 LOAD_ATTR               12 (TAKEN_BY_COURIER_FROM_POK)
-               
-               169         266 LOAD_GLOBAL              0 (ParcelStatus)
-                           278 LOAD_ATTR               13 (STACK_IN_BOX_MACHINE)
-                           288 LOAD_GLOBAL              0 (ParcelStatus)
-                           300 LOAD_ATTR               14 (STACK_IN_CUSTOMER_SERVICE_POINT)
-               
-               163         310 BUILD_LIST              14
-                           312 RETURN_VALUE
-               consts
-                  None
-               names      ('ParcelStatus', 'READY_TO_PICKUP', 'CONFIRMED', 'ADOPTED_AT_SORTING_CENTER', 'ADOPTED_AT_SOURCE_BRANCH', 'COLLECTED_FROM_SENDER', 'DISPATCHED_BY_SENDER', 'DISPATCHED_BY_SENDER_TO_POK', 'OUT_FOR_DELIVERY', 'OUT_FOR_DELIVERY_TO_ADDRESS', 'SENT_FROM_SOURCE_BRANCH', 'TAKEN_BY_COURIER', 'TAKEN_BY_COURIER_FROM_POK', 'STACK_IN_BOX_MACHINE', 'STACK_IN_CUSTOMER_SERVICE_POINT')
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
-               name       'pending'
-               firstlineno 162
-               lnotab 0x02012c012c012c012c012c012c012cfa
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'CREATED', 'OFFERS_PREPARED', 'OFFER_SELECTED', 'CONFIRMED', 'READY_TO_PICKUP_FROM_POK', 'OVERSIZED', 'DISPATCHED_BY_SENDER_TO_POK', 'DISPATCHED_BY_SENDER', 'COLLECTED_FROM_SENDER', 'TAKEN_BY_COURIER', 'ADOPTED_AT_SOURCE_BRANCH', 'SENT_FROM_SOURCE_BRANCH', 'READDRESSED', 'OUT_FOR_DELIVERY', 'READY_TO_PICKUP', 'PICKUP_REMINDER_SENT', 'PICKUP_TIME_EXPIRED', 'AVIZO', 'TAKEN_BY_COURIER_FROM_POK', 'REJECTED_BY_RECEIVER', 'UNDELIVERED', 'DELAY_IN_DELIVERY', 'RETURNED_TO_SENDER', 'READY_TO_PICKUP_FROM_BRANCH', 'DELIVERED', 'CANCELED', 'CLAIMED', 'STACK_IN_CUSTOMER_SERVICE_POINT', 'STACK_PARCEL_PICKUP_TIME_EXPIRED', 'UNSTACK_FROM_CUSTOMER_SERVICE_POINT', 'COURIER_AVIZO_IN_CUSTOMER_SERVICE_POINT', 'TAKEN_BY_COURIER_FROM_CUSTOMER_SERVICE_POINT', 'STACK_IN_BOX_MACHINE', 'STACK_PARCEL_IN_BOX_MACHINE_PICKUP_TIME_EXPIRED', 'UNSTACK_FROM_BOX_MACHINE', 'ADOPTED_AT_SORTING_CENTER', 'OUT_FOR_DELIVERY_TO_ADDRESS', 'PICKUP_REMINDER_SENT_ADDRESS', 'UNDELIVERED_WRONG_ADDRESS', 'UNDELIVERED_COD_CASH_RECEIVER', 'REDIRECT_TO_BOX', 'CANCELED_REDIRECT_TO_BOX', 'List', 'pending')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'CREATED', 'OFFERS_PREPARED', 'OFFER_SELECTED', 'CONFIRMED', 'READY_TO_PICKUP_FROM_POK', 'OVERSIZED', 'DISPATCHED_BY_SENDER_TO_POK', 'DISPATCHED_BY_SENDER', 'COLLECTED_FROM_SENDER', 'TAKEN_BY_COURIER', 'ADOPTED_AT_SOURCE_BRANCH', 'SENT_FROM_SOURCE_BRANCH', 'READDRESSED', 'OUT_FOR_DELIVERY', 'READY_TO_PICKUP', 'PICKUP_REMINDER_SENT', 'PICKUP_TIME_EXPIRED', 'AVIZO', 'TAKEN_BY_COURIER_FROM_POK', 'REJECTED_BY_RECEIVER', 'UNDELIVERED', 'DELAY_IN_DELIVERY', 'RETURNED_TO_SENDER', 'READY_TO_PICKUP_FROM_BRANCH', 'DELIVERED', 'CANCELED', 'CLAIMED', 'STACK_IN_CUSTOMER_SERVICE_POINT', 'STACK_PARCEL_PICKUP_TIME_EXPIRED', 'UNSTACK_FROM_CUSTOMER_SERVICE_POINT', 'COURIER_AVIZO_IN_CUSTOMER_SERVICE_POINT', 'TAKEN_BY_COURIER_FROM_CUSTOMER_SERVICE_POINT', 'STACK_IN_BOX_MACHINE', 'STACK_PARCEL_IN_BOX_MACHINE_PICKUP_TIME_EXPIRED', 'UNSTACK_FROM_BOX_MACHINE', 'ADOPTED_AT_SORTING_CENTER', 'OUT_FOR_DELIVERY_TO_ADDRESS', 'PICKUP_REMINDER_SENT_ADDRESS', 'UNDELIVERED_WRONG_ADDRESS', 'UNDELIVERED_COD_CASH_RECEIVER', 'REDIRECT_TO_BOX', 'CANCELED_REDIRECT_TO_BOX')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ParcelStatus'
          firstlineno 116
          lnotab
             0x0a01040104010401040104010401040104010401040104010401040104
             010401040104010401040104010401040104010401040104010401040104
-            010401040104010401040104010401040104010401040104010401040104
-            02
+            0104010401040104010401040104010401040104010401040104010401
       'ParcelStatus'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a06640553
             00
-         172           0 RESUME                   0
+         163           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ReturnsStatus')
                        8 STORE_NAME               2 (__qualname__)
          
-         173          10 LOAD_CONST               1 ('Zaakceptowano')
+         164          10 LOAD_CONST               1 ('Zaakceptowano')
                       12 STORE_NAME               3 (ACCEPTED)
          
-         174          14 LOAD_CONST               2 ('Nadano')
+         165          14 LOAD_CONST               2 ('Nadano')
                       16 STORE_NAME               4 (USED)
          
-         175          18 LOAD_CONST               3 ('Dostarczono')
+         166          18 LOAD_CONST               3 ('Dostarczono')
                       20 STORE_NAME               5 (DELIVERED)
          
-         176          22 LOAD_CONST               4 ('UNKNOWN DATA')
+         167          22 LOAD_CONST               4 ('UNKNOWN DATA')
                       24 STORE_NAME               6 (UNKNOWN)
                       26 LOAD_CONST               5 (None)
                       28 RETURN_VALUE
          consts
             'ReturnsStatus'
             'Zaakceptowano'
             'Nadano'
@@ -1456,41 +1378,41 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'ACCEPTED', 'USED', 'DELIVERED', 'UNKNOWN')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ReturnsStatus'
-         firstlineno 172
+         firstlineno 163
          lnotab 0x0a01040104010401
       'ReturnsStatus'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a06640553
             00
-         179           0 RESUME                   0
+         170           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParcelOwnership')
                        8 STORE_NAME               2 (__qualname__)
          
-         180          10 LOAD_CONST               1 (':class:`Enum` that holds parcel ownership types')
+         171          10 LOAD_CONST               1 (':class:`Enum` that holds parcel ownership types')
                       12 STORE_NAME               3 (__doc__)
          
-         181          14 LOAD_CONST               2 ('UNKNOWN DATA')
+         172          14 LOAD_CONST               2 ('UNKNOWN DATA')
                       16 STORE_NAME               4 (UNKNOWN)
          
-         182          18 LOAD_CONST               3 ('Zaprzyjaźniona')
+         173          18 LOAD_CONST               3 ('Zaprzyjaźniona')
                       20 STORE_NAME               5 (FRIEND)
          
-         183          22 LOAD_CONST               4 ('Własna')
+         174          22 LOAD_CONST               4 ('Własna')
                       24 STORE_NAME               6 (OWN)
                       26 LOAD_CONST               5 (None)
                       28 RETURN_VALUE
          consts
             'ParcelOwnership'
             ':class:`Enum` that holds parcel ownership types'
             'UNKNOWN DATA'
@@ -1499,41 +1421,41 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'FRIEND', 'OWN')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ParcelOwnership'
-         firstlineno 179
+         firstlineno 170
          lnotab 0x0a01040104010401
       'ParcelOwnership'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a06640553
             00
-         187           0 RESUME                   0
+         178           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CompartmentExpectedStatus')
                        8 STORE_NAME               2 (__qualname__)
          
-         188          10 LOAD_CONST               1 (':class:`Enum` that holds compartment expected statuses')
+         179          10 LOAD_CONST               1 (':class:`Enum` that holds compartment expected statuses')
                       12 STORE_NAME               3 (__doc__)
          
-         189          14 LOAD_CONST               2 ('UNKNOWN DATA')
+         180          14 LOAD_CONST               2 ('UNKNOWN DATA')
                       16 STORE_NAME               4 (UNKNOWN)
          
-         190          18 LOAD_CONST               3 ('Otwarta')
+         181          18 LOAD_CONST               3 ('Otwarta')
                       20 STORE_NAME               5 (OPENED)
          
-         191          22 LOAD_CONST               4 ('Zamknięta')
+         182          22 LOAD_CONST               4 ('Zamknięta')
                       24 STORE_NAME               6 (CLOSED)
                       26 LOAD_CONST               5 (None)
                       28 RETURN_VALUE
          consts
             'CompartmentExpectedStatus'
             ':class:`Enum` that holds compartment expected statuses'
             'UNKNOWN DATA'
@@ -1542,41 +1464,41 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'OPENED', 'CLOSED')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'CompartmentExpectedStatus'
-         firstlineno 187
+         firstlineno 178
          lnotab 0x0a01040104010401
       'CompartmentExpectedStatus'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a06640553
             00
-         194           0 RESUME                   0
+         185           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CompartmentActualStatus')
                        8 STORE_NAME               2 (__qualname__)
          
-         195          10 LOAD_CONST               1 (':class:`Enum` that holds compartment actual statuses')
+         186          10 LOAD_CONST               1 (':class:`Enum` that holds compartment actual statuses')
                       12 STORE_NAME               3 (__doc__)
          
-         196          14 LOAD_CONST               2 ('UNKNOWN DATA')
+         187          14 LOAD_CONST               2 ('UNKNOWN DATA')
                       16 STORE_NAME               4 (UNKNOWN)
          
-         197          18 LOAD_CONST               3 ('Otwarta')
+         188          18 LOAD_CONST               3 ('Otwarta')
                       20 STORE_NAME               5 (OPENED)
          
-         198          22 LOAD_CONST               4 ('Zamknięta')
+         189          22 LOAD_CONST               4 ('Zamknięta')
                       24 STORE_NAME               6 (CLOSED)
                       26 LOAD_CONST               5 (None)
                       28 RETURN_VALUE
          consts
             'CompartmentActualStatus'
             ':class:`Enum` that holds compartment actual statuses'
             'UNKNOWN DATA'
@@ -1585,66 +1507,66 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'UNKNOWN', 'OPENED', 'CLOSED')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'CompartmentActualStatus'
-         firstlineno 194
+         firstlineno 185
          lnotab 0x0a01040104010401
       'CompartmentActualStatus'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
             0764065a0864075a0964085a0a64095a0b640a5a0c640b5a0d640c5a0e64
             0d5300
-         201           0 RESUME                   0
+         192           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ParcelServiceName')
                        8 STORE_NAME               2 (__qualname__)
          
-         202          10 LOAD_CONST               1 ('UNKNOWN DATA')
+         193          10 LOAD_CONST               1 ('UNKNOWN DATA')
                       12 STORE_NAME               3 (UNKNOWN)
          
-         203          14 LOAD_CONST               2 (1)
+         194          14 LOAD_CONST               2 (1)
                       16 STORE_NAME               4 (ALLEGRO_PARCEL)
          
-         204          18 LOAD_CONST               3 (2)
+         195          18 LOAD_CONST               3 (2)
                       20 STORE_NAME               5 (ALLEGRO_PARCEL_SMART)
          
-         205          22 LOAD_CONST               4 (3)
+         196          22 LOAD_CONST               4 (3)
                       24 STORE_NAME               6 (ALLEGRO_LETTER)
          
-         206          26 LOAD_CONST               5 (4)
+         197          26 LOAD_CONST               5 (4)
                       28 STORE_NAME               7 (ALLEGRO_COURIER)
          
-         207          30 LOAD_CONST               6 (5)
+         198          30 LOAD_CONST               6 (5)
                       32 STORE_NAME               8 (STANDARD)
          
-         208          34 LOAD_CONST               7 (6)
+         199          34 LOAD_CONST               7 (6)
                       36 STORE_NAME               9 (STANDARD_PARCEL_SMART)
          
-         209          38 LOAD_CONST               8 (7)
+         200          38 LOAD_CONST               8 (7)
                       40 STORE_NAME              10 (PASS_THRU)
          
-         210          42 LOAD_CONST               9 (8)
+         201          42 LOAD_CONST               9 (8)
                       44 STORE_NAME              11 (CUSTOMER_SERVICE_POINT)
          
-         211          46 LOAD_CONST              10 (9)
+         202          46 LOAD_CONST              10 (9)
                       48 STORE_NAME              12 (REVERSE)
          
-         212          50 LOAD_CONST              11 (10)
+         203          50 LOAD_CONST              11 (10)
                       52 STORE_NAME              13 (STANDARD_COURIER)
          
-         213          54 LOAD_CONST              12 (11)
+         204          54 LOAD_CONST              12 (11)
                       56 STORE_NAME              14 (REVERSE_RETURN)
                       58 LOAD_CONST              13 (None)
                       60 RETURN_VALUE
          consts
             'ParcelServiceName'
             'UNKNOWN DATA'
             1
@@ -1661,21 +1583,21 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'UNKNOWN', 'ALLEGRO_PARCEL', 'ALLEGRO_PARCEL_SMART', 'ALLEGRO_LETTER', 'ALLEGRO_COURIER', 'STANDARD', 'STANDARD_PARCEL_SMART', 'PASS_THRU', 'CUSTOMER_SERVICE_POINT', 'REVERSE', 'STANDARD_COURIER', 'REVERSE_RETURN')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
          name       'ParcelServiceName'
-         firstlineno 201
+         firstlineno 192
          lnotab 0x0a0104010401040104010401040104010401040104010401
       'ParcelServiceName'
       None
    names      ('enum', 'Enum', 'EnumMeta', 'typing', 'List', 'Meta', 'ParcelBase', 'ParcelCarrierSize', 'ParcelLockerSize', 'ParcelDeliveryType', 'ParcelShipmentType', 'ParcelAdditionalInsurance', 'ParcelType', 'ParcelStatus', 'ReturnsStatus', 'ParcelOwnership', 'CompartmentExpectedStatus', 'CompartmentActualStatus', 'ParcelServiceName')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/loobson/pyprojects/inpost-python/inpost/static/statuses.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010c031c1720261c0a1c081c081c081c081c081c381c071c
+      0x00ff020110010c031c1720261c0a1c081c081c081c081c081c2f1c071c
       081c071c07
```

### Comparing `inpost-0.1.0/inpost/static/endpoints.py` & `inpost-0.1.1/inpost/static/endpoints.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/exceptions.py` & `inpost-0.1.1/inpost/static/exceptions.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/friends.py` & `inpost-0.1.1/inpost/static/friends.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/notifications.py` & `inpost-0.1.1/inpost/static/notifications.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/inpost/static/parcels.py` & `inpost-0.1.1/inpost/static/parcels.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from arrow import get, arrow
 
 from inpost.static.statuses import *
 
 
 class BaseParcel:
     def __init__(self, parcel_data: dict, logger: logging.Logger):
-        self.shipment_number: str = parcel_data['shipmentNumber']
+        self.shipment_number: str = parcel_data.get('shipmentNumber')
         self._log: logging.Logger = logger.getChild(f'{__class__.__name__}.{self.shipment_number}')
         self.status: ParcelStatus = ParcelStatus[parcel_data['status']]
         self.expiry_date: arrow | None = get(parcel_data['expiryDate']) if 'expiryDate' in parcel_data else None
         self.operations: Operations = Operations(operations_data=parcel_data['operations'], logger=self._log)
         self.event_log: List[EventLog] = [EventLog(eventlog_data=event, logger=self._log)
                                           for event in parcel_data['eventLog']]
 
@@ -29,33 +29,34 @@
     :type logger: logging.Logger"""
 
     def __init__(self, parcel_data: dict, logger: logging.Logger):
         """Constructor method"""
         super().__init__(parcel_data, logger)
         self._log: logging.Logger = logger.getChild(f'{__class__.__name__}.{self.shipment_number}')
         self.shipment_type: ParcelShipmentType = ParcelShipmentType[parcel_data['shipmentType']]
-        self._open_code: str | None = parcel_data['openCode'] if 'openCode' in parcel_data else None
+        self._open_code: str | None = parcel_data.get('openCode', None)
         self._qr_code: QRCode | None = QRCode(qrcode_data=parcel_data['qrCode'], logger=self._log) \
             if 'qrCode' in parcel_data else None
         self.stored_date: arrow | None = get(parcel_data['storedDate']) if 'storedDate' in parcel_data else None
         self.pickup_date: arrow | None = get(parcel_data['pickUpDate']) if 'pickUpDate' in parcel_data else None
         self.parcel_size: ParcelLockerSize | ParcelCarrierSize = ParcelLockerSize[parcel_data['parcelSize']] \
             if self.shipment_type == ParcelShipmentType.parcel else ParcelCarrierSize[parcel_data['parcelSize']]
-        self.receiver: Receiver = Receiver(receiver_data=parcel_data['receiver'], logger=self._log)
-        self.sender: Sender = Sender(sender_data=parcel_data['sender'], logger=self._log)
+        self.receiver: Receiver = Receiver(receiver_data=parcel_data['receiver'], logger=self._log) if 'reveiver' in parcel_data else None
+        self.sender: Sender = Sender(sender_data=parcel_data['sender'], logger=self._log) if 'sender' in parcel_data else None
         self.pickup_point: PickupPoint = PickupPoint(pickuppoint_data=parcel_data['pickUpPoint'], logger=self._log) \
             if 'pickUpPoint' in parcel_data else None
         self.multi_compartment: MultiCompartment | None = MultiCompartment(
             parcel_data['multiCompartment'], logger=self._log) if 'multiCompartment' in parcel_data else None
-        self.is_end_off_week_collection: bool = parcel_data['endOfWeekCollection']
-        self.status: ParcelStatus = ParcelStatus[parcel_data['status']]
-        self.avizo_transaction_status: str = parcel_data['avizoTransactionStatus']
+        self.is_end_off_week_collection: bool | None = parcel_data.get('endOfWeekCollection', None)
+        self.status: ParcelStatus = ParcelStatus[parcel_data['status']] if 'status' in parcel_data else None
+        self.avizo_transaction_status: str | None = parcel_data.get('avizoTransactionStatus', None)
         self.shared_to: List[SharedTo] = [SharedTo(sharedto_data=person, logger=self._log)
-                                          for person in parcel_data['sharedTo']]
-        self.ownership_status: ParcelOwnership = ParcelOwnership[parcel_data['ownershipStatus']]
+                                          for person in parcel_data['sharedTo']] if 'sharedTo' in parcel_data else None
+        self.ownership_status: ParcelOwnership = ParcelOwnership[parcel_data['ownershipStatus']] if 'ownershipStatus' in parcel_data else None
+        self.economy_parcel: bool | None = parcel_data.get('economyParcel', None)
         self._compartment_properties: CompartmentProperties | None = None
 
         self._log.debug(f'created parcel with shipment number {self.shipment_number}')
 
         # log all unexpected things, so you can make an issue @github
         if self.shipment_type == ParcelShipmentType.UNKNOWN:
             self._log.debug(f'unexpected shipment_type: {parcel_data["shipmentType"]}')
```

### Comparing `inpost-0.1.0/inpost/static/statuses.py` & `inpost-0.1.1/inpost/static/statuses.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.0/pyproject.toml` & `inpost-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inpost"
-version = "0.1.0"
+version = "0.1.1"
 description = "Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app"
 authors = ["loboda4450 <loboda4450@gmail.com>", "MrKazik99 <mrkazik99@gmail.com>"]
 maintainers = ["loboda4450 <loboda4450@gmail.com>"]
 documentation = 'https://inpost-python.readthedocs.io/en/latest/index.html'
 repository = "https://github.com/IFOSSA/inpost-python"
 readme = "README.md"
 packages = [
```

### Comparing `inpost-0.1.0/setup.py` & `inpost-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['Pillow>=9.4.0,<10.0.0',
  'aiohttp>=3.8.1,<4.0.0',
  'arrow>=1.2.3,<2.0.0',
  'qrcode>=7.3.1,<8.0.0']
 
 setup_kwargs = {
     'name': 'inpost',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app',
     'long_description': "\n# Inpost Python\n\nFully async Inpost library using Python 3.10.\n\n\n\n\n## Documentation\n\n[Readthedocs.io](https://inpost-python.readthedocs.io/en/latest/)\n\n\n## Usage/Examples\n\n\n```python\nfrom inpost.api import Inpost\n\ninp = await Inpost.from_phone_number('555333444')\nawait inp.send_sms_code():\n...\nif await inp.confirm_sms_code(123321):\n   print('Congratulations, you initialized successfully!')\n```\n\n\n## Authors\n\n- [@loboda4450](https://www.github.com/loboda4450)\n- [@mrkazik99](https://www.github.com/mrkazik99)\n\n\n## Used By\n\nThis project is used by the following repos:\n\n[Inpost Telegram Bot](https://github.com/loboda4450/inpost-telegram-bot)\n\n",
     'author': 'loboda4450',
     'author_email': 'loboda4450@gmail.com',
     'maintainer': 'loboda4450',
     'maintainer_email': 'loboda4450@gmail.com',
     'url': 'https://github.com/IFOSSA/inpost-python',
```

### Comparing `inpost-0.1.0/PKG-INFO` & `inpost-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inpost
-Version: 0.1.0
+Version: 0.1.1
 Summary: Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app
 Home-page: https://github.com/IFOSSA/inpost-python
 Author: loboda4450
 Author-email: loboda4450@gmail.com
 Maintainer: loboda4450
 Maintainer-email: loboda4450@gmail.com
 Requires-Python: >=3.10,<4.0
```

