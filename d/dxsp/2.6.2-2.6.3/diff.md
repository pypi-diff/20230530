# Comparing `tmp/dxsp-2.6.2.tar.gz` & `tmp/dxsp-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.6.2.tar", max compression
+gzip compressed data, was "dxsp-2.6.3.tar", max compression
```

## Comparing `dxsp-2.6.2.tar` & `dxsp-2.6.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-30 15:50:27.243119 dxsp-2.6.2/LICENSE
--rw-r--r--   0        0        0     2348 2023-05-30 15:50:27.243119 dxsp-2.6.2/README.md
--rw-r--r--   0        0        0       86 2023-05-30 15:50:27.947127 dxsp-2.6.2/dxsp/__init__.py
--rw-r--r--   0        0        0      386 2023-05-30 15:50:27.243119 dxsp-2.6.2/dxsp/config.py
--rw-r--r--   0        0        0     3679 2023-05-30 15:50:27.243119 dxsp-2.6.2/dxsp/default_settings.toml
--rw-r--r--   0        0        0    18916 2023-05-30 15:50:27.243119 dxsp-2.6.2/dxsp/main.py
--rw-r--r--   0        0        0     1542 2023-05-30 15:50:27.947127 dxsp-2.6.2/pyproject.toml
--rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dxsp-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-30 20:06:34.665493 dxsp-2.6.3/LICENSE
+-rw-r--r--   0        0        0     2348 2023-05-30 20:06:34.665493 dxsp-2.6.3/README.md
+-rw-r--r--   0        0        0       86 2023-05-30 20:06:35.325500 dxsp-2.6.3/dxsp/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-30 20:06:34.665493 dxsp-2.6.3/dxsp/config.py
+-rw-r--r--   0        0        0     3679 2023-05-30 20:06:34.665493 dxsp-2.6.3/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    18642 2023-05-30 20:06:34.665493 dxsp-2.6.3/dxsp/main.py
+-rw-r--r--   0        0        0     1542 2023-05-30 20:06:35.325500 dxsp-2.6.3/pyproject.toml
+-rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dxsp-2.6.3/PKG-INFO
```

### Comparing `dxsp-2.6.2/LICENSE` & `dxsp-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.2/README.md` & `dxsp-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.2/dxsp/default_settings.toml` & `dxsp-2.6.3/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.2/dxsp/main.py` & `dxsp-2.6.3/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,36 +117,25 @@
 
         except Exception as error:
             raise error
 
 ### ------🛠️ W3 UTILS ---------
 
 
-    async def _get(
-        self,
-        url,
-        params=None,
-        headers=None
-            ):
-        try:
-            self.logger.debug("url: %s", url)
-            # self.logger.debug("_header: %s", settings.headers)
-            response = requests.get(
-                url,
-                params=params,
-                headers=headers,
-                timeout=10)
-            #self.logger.debug("_response: %s", response)
-            if response:
-                #self.logger.debug("_json: %s", response.json())
+    async def _get(self, url, params=None, headers=None):
+        try:
+            self.logger.debug(f"Requesting URL: {url}")
+            response = requests.get(url, params=params, headers=headers, timeout=10)
+            if response.status_code == 200:
                 return response.json()
 
         except Exception as error:
             raise error
 
+
     async def router(self):
         try:
             router_abi = await self.get_abi(settings.dex_router_contract_addr)
             if router_abi is None:
                 router_abi = await self._get(settings.dex_router_abi_url)
             router = self.w3.eth.contract(
                 address=self.w3.to_checksum_address(
@@ -384,15 +373,15 @@
         return contract.functions.balanceOf(self.wallet_address).call() or 0
 
     async def get_token_decimals(self, token_symbol: str) -> Optional[int]:
         """Get token decimals"""
         contract = await self.get_token_contract(token_symbol)
         if not contract:
             return None
-        return int(await contract.functions.decimals().call())
+        return await contract.functions.decimals().call()
 
     async def get_account_balance(self):
         try:
             account_balance = self.w3.eth.get_balance(
                 self.w3.to_checksum_address(self.wallet_address))
             account_balance = self.w3.from_wei(account_balance, 'ether')
             trading_asset_balance = await self.get_trading_asset_balance()
```

### Comparing `dxsp-2.6.2/pyproject.toml` & `dxsp-2.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.6.2"
+version = "2.6.3"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-2.6.2/PKG-INFO` & `dxsp-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.6.2
+Version: 2.6.3
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

