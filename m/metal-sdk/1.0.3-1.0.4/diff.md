# Comparing `tmp/metal_sdk-1.0.3.tar.gz` & `tmp/metal_sdk-1.0.4.tar.gz`

## Comparing `metal_sdk-1.0.3.tar` & `metal_sdk-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/.github/workflows/lint.yml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/examples/example.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/examples/example_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/src/metal_sdk/__init__.py
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/src/metal_sdk/metal.py
--rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/src/metal_sdk/metal_async.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/src/metal_sdk/motorhead.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/src/metal_sdk/motorhead_async.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/src/metal_sdk/typings.py
--rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/tests/test_metal.py
--rw-r--r--   0        0        0     7180 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/tests/test_metal_async.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/tests/test_motorhead.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/tests/test_motorhead_async.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/.gitignore
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/LICENSE
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/README.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/examples/example.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/examples/example_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/src/metal_sdk/__init__.py
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/src/metal_sdk/metal.py
+-rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/src/metal_sdk/metal_async.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/src/metal_sdk/motorhead.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/src/metal_sdk/motorhead_async.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/src/metal_sdk/typings.py
+-rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/tests/test_metal.py
+-rw-r--r--   0        0        0     7180 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/tests/test_metal_async.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/tests/test_motorhead.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/tests/test_motorhead_async.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/.gitignore
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/LICENSE
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.4/PKG-INFO
```

### Comparing `metal_sdk-1.0.3/.github/workflows/publish.yml` & `metal_sdk-1.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.3/.github/workflows/test.yml` & `metal_sdk-1.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.3/examples/example.py` & `metal_sdk-1.0.4/examples/example.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.3/examples/example_async.py` & `metal_sdk-1.0.4/examples/example_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.3/src/metal_sdk/metal.py` & `metal_sdk-1.0.4/src/metal_sdk/metal.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.3/src/metal_sdk/metal_async.py` & `metal_sdk-1.0.4/src/metal_sdk/metal_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.3/src/metal_sdk/motorhead.py` & `metal_sdk-1.0.4/src/metal_sdk/motorhead.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import httpx
+from .typings import MotorheadPayload
 
 API_URL = 'https://api.getmetal.io/v1/motorhead'
 
 
 class Motorhead:
-    def __init__(self, api_key=None, client_id=None, base_url=API_URL):
-        self.api_key = api_key
-        self.client_id = client_id
-        self.base_url = base_url
+    def __init__(self, payload: MotorheadPayload = {}):
+        self.api_key = payload.get("api_key")
+        self.client_id = payload.get("client_id")
+        self.base_url = payload.get("base_url") or API_URL
 
-        if base_url == API_URL and not (api_key and client_id):
+        if self.base_url == API_URL and not (self.api_key and self.client_id):
             raise ValueError('api_key and client_id required for managed motorhead')
 
         self.client = httpx.Client(headers={
             'Content-Type': 'application/json',
             'x-metal-api-key': self.api_key,
             'x-metal-client-id': self.client_id,
         })
```

### Comparing `metal_sdk-1.0.3/src/metal_sdk/motorhead_async.py` & `metal_sdk-1.0.4/src/metal_sdk/motorhead_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.3/src/metal_sdk/typings.py` & `metal_sdk-1.0.4/src/metal_sdk/typings.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,7 +46,13 @@
     filters: NotRequired[List[SearchFilter]]
 
 
 class TunePayload(TypedDict):
     idA: str
     idB: str
     label: TuneLabel
+
+
+class MotorheadPayload(TypedDict):
+    api_key: NotRequired[str]
+    client_id: NotRequired[str]
+    base_url: NotRequired[str]
```

### Comparing `metal_sdk-1.0.3/tests/test_metal.py` & `metal_sdk-1.0.4/tests/test_metal.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.3/tests/test_metal_async.py` & `metal_sdk-1.0.4/tests/test_metal_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.3/tests/test_motorhead.py` & `metal_sdk-1.0.4/tests/test_motorhead.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from unittest.mock import MagicMock
 from src.metal_sdk.motorhead import Motorhead
 
 
 class TestMotorhead(unittest.TestCase):
 
     def setUp(self):
-        self.motorhead = Motorhead(api_key='test_key', client_id='test_client')
+        self.motorhead = Motorhead({"api_key": "test_key", "client_id": "test_client"})
 
     def test_initialization(self):
         self.assertEqual(self.motorhead.api_key, 'test_key')
         self.assertEqual(self.motorhead.client_id, 'test_client')
 
         with self.assertRaises(ValueError):
             Motorhead()
```

### Comparing `metal_sdk-1.0.3/.gitignore` & `metal_sdk-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.3/LICENSE` & `metal_sdk-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.3/README.md` & `metal_sdk-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.3/pyproject.toml` & `metal_sdk-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metal_sdk"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Metal Technologies Inc", email="james@getmetal.io" },
 ]
 description = "SDK for getmetal.io"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `metal_sdk-1.0.3/PKG-INFO` & `metal_sdk-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metal_sdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: SDK for getmetal.io
 Project-URL: Github, https://github.com/getmetal/metal-python
 Author-email: Metal Technologies Inc <james@getmetal.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

