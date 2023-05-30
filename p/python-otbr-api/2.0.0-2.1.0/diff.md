# Comparing `tmp/python-otbr-api-2.0.0.tar.gz` & `tmp/python-otbr-api-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-otbr-api-2.0.0.tar", last modified: Mon May 29 07:03:15 2023, max compression
+gzip compressed data, was "python-otbr-api-2.1.0.tar", last modified: Tue May 30 08:43:38 2023, max compression
```

## Comparing `python-otbr-api-2.0.0.tar` & `python-otbr-api-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:03:15.862037 python-otbr-api-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-29 07:03:15.862037 python-otbr-api-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:03:15.858037 python-otbr-api-2.0.0/python_otbr_api/
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/python_otbr_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/python_otbr_api/mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/python_otbr_api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/python_otbr_api/pskc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/python_otbr_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/python_otbr_api/tlv_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:03:15.862037 python-otbr-api-2.0.0/python_otbr_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-29 07:03:15.000000 python-otbr-api-2.0.0/python_otbr_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-29 07:03:15.000000 python-otbr-api-2.0.0/python_otbr_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 07:03:15.000000 python-otbr-api-2.0.0/python_otbr_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 07:03:15.000000 python-otbr-api-2.0.0/python_otbr_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 07:03:15.000000 python-otbr-api-2.0.0/python_otbr_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 07:03:15.000000 python-otbr-api-2.0.0/python_otbr_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 07:03:15.862037 python-otbr-api-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:38.771971 python-otbr-api-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-30 08:43:38.771971 python-otbr-api-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:38.767971 python-otbr-api-2.1.0/python_otbr_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/python_otbr_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/python_otbr_api/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/python_otbr_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/python_otbr_api/pskc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/python_otbr_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-30 08:43:18.000000 python-otbr-api-2.1.0/python_otbr_api/tlv_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:43:38.771971 python-otbr-api-2.1.0/python_otbr_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-30 08:43:38.000000 python-otbr-api-2.1.0/python_otbr_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-30 08:43:38.000000 python-otbr-api-2.1.0/python_otbr_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:43:38.000000 python-otbr-api-2.1.0/python_otbr_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 08:43:38.000000 python-otbr-api-2.1.0/python_otbr_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 08:43:38.000000 python-otbr-api-2.1.0/python_otbr_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:43:38.000000 python-otbr-api-2.1.0/python_otbr_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-30 08:43:38.771971 python-otbr-api-2.1.0/setup.cfg
```

### Comparing `python-otbr-api-2.0.0/LICENSE` & `python-otbr-api-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-otbr-api-2.0.0/pyproject.toml` & `python-otbr-api-2.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=65.6", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name         = "python-otbr-api"
-version      = "2.0.0"
+version      = "2.1.0"
 license      = {text = "MIT"}
 description  = "API to interact with an OTBR via its REST API"
 readme       = "README.md"
 authors      = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 requires-python = ">=3.9.0"
```

### Comparing `python-otbr-api-2.0.0/python_otbr_api/__init__.py` & `python-otbr-api-2.1.0/python_otbr_api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,14 +85,37 @@
             raise OTBRError(f"unexpected http status {response.status}")
 
         try:
             return bytes.fromhex(await response.text("ASCII"))
         except ValueError as exc:
             raise OTBRError("unexpected API response") from exc
 
+    async def get_pending_dataset_tlvs(self) -> bytes | None:
+        """Get current pending operational dataset in TLVS format, or None.
+
+        Returns None if there is no pending operational dataset.
+        Raises if the http status is 400 or higher or if the response is invalid.
+        """
+        response = await self._session.get(
+            f"{self._url}/node/dataset/pending",
+            headers={"Accept": "text/plain"},
+            timeout=aiohttp.ClientTimeout(total=self._timeout),
+        )
+
+        if response.status == HTTPStatus.NO_CONTENT:
+            return None
+
+        if response.status != HTTPStatus.OK:
+            raise OTBRError(f"unexpected http status {response.status}")
+
+        try:
+            return bytes.fromhex(await response.text("ASCII"))
+        except ValueError as exc:
+            raise OTBRError("unexpected API response") from exc
+
     async def create_active_dataset(self, dataset: ActiveDataSet) -> None:
         """Create active operational dataset.
 
         The passed in ActiveDataSet does not need to be fully populated, any fields
         not set will be automatically set by the open thread border router.
         Raises if the http status is 400 or higher or if the response is invalid.
         """
```

### Comparing `python-otbr-api-2.0.0/python_otbr_api/mdns.py` & `python-otbr-api-2.1.0/python_otbr_api/mdns.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-2.0.0/python_otbr_api/models.py` & `python-otbr-api-2.1.0/python_otbr_api/models.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-2.0.0/python_otbr_api/pskc.py` & `python-otbr-api-2.1.0/python_otbr_api/pskc.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     if len(passphrase_bytes) == AES_128_KEY_LEN:
         return passphrase_bytes
     c = cmac.CMAC(algorithms.AES128(b"\0" * AES_128_KEY_LEN))
     c.update(passphrase_bytes)
     return c.finalize()
 
 
-def compute_pskc(ext_pan_id: str, network_name: str, passphrase: str) -> bytes:
+def compute_pskc(ext_pan_id: bytes, network_name: str, passphrase: str) -> bytes:
     """Compute Thread PSKc."""
-    salt = SALT_PREFIX + bytes.fromhex(ext_pan_id) + network_name.encode()
+    salt = SALT_PREFIX + ext_pan_id + network_name.encode()
     key = _derive_key(passphrase)
 
     block_counter = 1
     prf_input = salt + struct.pack("!L", block_counter)
 
     # Calculate U_1
     c = cmac.CMAC(algorithms.AES128(key))
```

