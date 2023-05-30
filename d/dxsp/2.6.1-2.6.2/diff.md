# Comparing `tmp/dxsp-2.6.1.tar.gz` & `tmp/dxsp-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.6.1.tar", max compression
+gzip compressed data, was "dxsp-2.6.2.tar", max compression
```

## Comparing `dxsp-2.6.1.tar` & `dxsp-2.6.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-30 12:04:39.262743 dxsp-2.6.1/LICENSE
--rw-r--r--   0        0        0     2348 2023-05-30 12:04:39.262743 dxsp-2.6.1/README.md
--rw-r--r--   0        0        0       86 2023-05-30 12:04:39.950757 dxsp-2.6.1/dxsp/__init__.py
--rw-r--r--   0        0        0      386 2023-05-30 12:04:39.262743 dxsp-2.6.1/dxsp/config.py
--rw-r--r--   0        0        0     3548 2023-05-30 12:04:39.262743 dxsp-2.6.1/dxsp/default_settings.toml
--rw-r--r--   0        0        0    19734 2023-05-30 12:04:39.262743 dxsp-2.6.1/dxsp/main.py
--rw-r--r--   0        0        0     1542 2023-05-30 12:04:39.950757 dxsp-2.6.1/pyproject.toml
--rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dxsp-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-30 15:50:27.243119 dxsp-2.6.2/LICENSE
+-rw-r--r--   0        0        0     2348 2023-05-30 15:50:27.243119 dxsp-2.6.2/README.md
+-rw-r--r--   0        0        0       86 2023-05-30 15:50:27.947127 dxsp-2.6.2/dxsp/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-30 15:50:27.243119 dxsp-2.6.2/dxsp/config.py
+-rw-r--r--   0        0        0     3679 2023-05-30 15:50:27.243119 dxsp-2.6.2/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    18916 2023-05-30 15:50:27.243119 dxsp-2.6.2/dxsp/main.py
+-rw-r--r--   0        0        0     1542 2023-05-30 15:50:27.947127 dxsp-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dxsp-2.6.2/PKG-INFO
```

### Comparing `dxsp-2.6.1/LICENSE` & `dxsp-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.1/README.md` & `dxsp-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.1/dxsp/default_settings.toml` & `dxsp-2.6.2/dxsp/default_settings.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 dex_block_explorer_url = "https://api.etherscan.io/api?"
 dex_block_explorer_api =  "798437294880920392"  #this is an example
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D" #UNI_V2
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
 # dex_router_contract_addr = "0x68b3465833fb72A70ecDF485E0e4C7bD8665Fc45" #UNI_V3
 dex_quoter_contract_addr = "0x61fFE014bA17989E743c5F6cB21bF9697530B21e" #UNI_V3_QUOTERV2
+dex_quoter_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v3/quoter.abi"
 #protocol specific
 #🦄1inch
 dex_1inch_url = "https://api.1inch.exchange/v5.0/"
 dex_1inch_limit_url = "https://limit-orders.1inch.io/v3.0/"
 #0️⃣0x
 dex_0x_url = "https://api.0x.org/mainnet"
 dex_0x_api_key = ""
```

### Comparing `dxsp-2.6.1/dxsp/main.py` & `dxsp-2.6.2/dxsp/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,16 +39,16 @@
         """Execute swap function."""
         action = order_params.get('action')
         instrument = order_params.get('instrument')
         quantity = order_params.get('quantity', 1)
 
         try:
             sell_token, buy_token = (
-                (settings.trading_asset, instrument) 
-                if action == 'BUY' 
+                (settings.trading_asset, instrument)
+                if action == 'BUY'
                 else (instrument, settings.trading_asset))
 
             sell_contract = await self.get_token_contract(sell_token)
             sell_decimals = sell_contract.functions.decimals().call() or 18
 
             sell_balance = await self.get_token_balance(sell_token)
             risk_percentage = settings.trading_risk_amount
@@ -57,26 +57,32 @@
             order = await self.get_swap(sell_token, buy_token, sell_amount)
             if order:
                 return order['confirmation']
         except Exception as error:
             raise error
 
     async def get_quote(self, sell_token):
-        buy_token = await self.search_contract(settings.trading_asset)
-
-        if buy_token is None:
-            self.logger.warning("No valid contract")
+        """
+        Asynchronously gets a quote for a specified sell token using the given `sell_token` parameter,
+        """
+        buy_address = await self.search_contract(settings.trading_asset)
+        sell_address = await self.search_contract(sell_token)
+        if sell_address is None:
             return
 
         try:
             if self.protocol_type in {"uniswap_v2", "uniswap_v3"}:
-                return await self.get_quote_uniswap(sell_token, buy_token)
+                return await self.get_quote_uniswap(
+                    buy_address,
+                    sell_address)
 
             if self.protocol_type == "0x":
-                return await self.get_0x_quote(sell_token, buy_token)
+                return await self.get_0x_quote(
+                    buy_address,
+                    sell_address)
 
         except Exception as error:
             raise error
 
     async def get_swap(self, sell_token: str, buy_token: str, amount: int) -> None:
         """Main swap function"""
         try:
@@ -125,62 +131,60 @@
             self.logger.debug("url: %s", url)
             # self.logger.debug("_header: %s", settings.headers)
             response = requests.get(
                 url,
                 params=params,
                 headers=headers,
                 timeout=10)
-            self.logger.debug("_response: %s", response)
+            #self.logger.debug("_response: %s", response)
             if response:
-                self.logger.debug("_json: %s", response.json())
+                #self.logger.debug("_json: %s", response.json())
                 return response.json()
 
-        except Exception as e:
-            self.logger.error("_get: %s", e)
+        except Exception as error:
+            raise error
 
     async def router(self):
         try:
             router_abi = await self.get_abi(settings.dex_router_contract_addr)
             if router_abi is None:
-                self.logger.debug("using setting dex_router_abi_url")
-                router_abi = requests.get(settings.dex_router_abi_url).text
-            self.logger.debug("router_abi: %s", router_abi)
+                router_abi = await self._get(settings.dex_router_abi_url)
             router = self.w3.eth.contract(
                 address=self.w3.to_checksum_address(
                     settings.dex_router_contract_addr),
                 abi=router_abi)
             return router
-        except Exception as e:
-            self.logger.error("router setup: %s", e)
+        except Exception as error:
+            raise error
 
     async def get_name(self):
         try:
             return settings.dex_router_contract_addr[-8:]
-        except Exception as e:
-            self.logger.error("router name %s", e)
+        except Exception as error:
+            raise error
 
     async def quoter(self):
         try:
             quoter_abi = await self.get_abi(settings.dex_quoter_contract_addr)
-            self.logger.debug("quoter_abi: %s", quoter_abi)
+            if quoter_abi is None:
+                quoter_abi = await self._get(settings.dex_quoter_abi_url)
             contract = self.w3.eth.contract(
                 address=self.w3.to_checksum_address(
                     settings.dex_quoter_contract_addr),
                 abi=quoter_abi)
             return contract
-        except Exception as e:
-            self.logger.error("quoter setup: %s", e)
+        except Exception as error:
+            raise error
 
     async def get_approve(self, symbol):
         try:
             if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
                 await self.get_approve_uniswap(symbol)
-        except Exception as e:
-            self.logger.error("Error in get_approve: %s", e)
-            return None
+        except Exception as error:
+            raise error
 
     async def get_sign(self, transaction):
         try:
             if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
                 transaction_params = {
                     'from': self.wallet_address,
                     'gas': await self.get_gas(transaction),
@@ -189,20 +193,16 @@
                         self.wallet_address),
                 }
                 transaction = transaction.build_transaction(transaction_params)
             signed = self.w3.eth.account.sign_transaction(
                 transaction, self.private_key)
             tx_hash = self.w3.eth.send_raw_transaction(signed.rawTransaction)
             return tx_hash
-        except (ValueError, TypeError, KeyError) as e:
-            self.logger.error("Failed to sign transaction: %s", e)
-            raise
-        except Exception as e:
-            self.logger.error("Failed to sign transaction: %s", e)
-            raise RuntimeError("Failed to sign transaction")
+        except Exception as error:
+            raise error
 
     async def get_abi(self, address):
         if not settings.dex_block_explorer_api:
             self.logger.warning("No block_explorer_api.")
             return None
 
         params = {
@@ -257,24 +257,26 @@
                     f"🗓️ {block['timestamp']}"
                 ),
             }
             return trade
         except Exception as error:
             raise error
 
-    async def get_gas(self, tx):
-        gas_estimate = self.w3.eth.estimate_gas(tx) * 1.25
-        self.logger.debug("gas_estimate %s", gas_estimate)
-        return int(self.w3.to_wei(gas_estimate, 'wei'))
+
+    async def get_gas(self, transaction):
+        """get gas estimate"""
+        gas_limit = self.w3.eth.estimate_gas(transaction) * 1.25
+        return int(self.w3.to_wei(gas_limit, 'wei'))
+
 
     async def get_gas_price(self):
+        """search get gas price"""
         gas_price = round(self.w3.from_wei(
             self.w3.eth.generate_gas_price(),
             'gwei'), 2)
-        self.logger.debug("gas_price %s", gas_price)
         return gas_price
 
 ### ------✍️ CONTRACT ---------
     async def search_contract(self, token):
         """search a contract function"""
         self.logger.debug("search_contract")
 
@@ -297,17 +299,17 @@
 
             token_contract = await self.search_cg_contract(token)
             if token_contract is not None:
                 self.logger.info("%s token: contract found %s",
                                  token, token_contract)
                 return self.w3.to_checksum_address(token_contract)
 
-            return f"no contract found for {token}"
-        except Exception as error:
-            raise error
+            return None
+        except Exception:
+            return None
 
     async def search_cg_platform(self):
         """search coingecko platform"""
         asset_platforms = self.cg.get_asset_platforms()
         output_dict = next(
             x for x in asset_platforms
             if x["chain_identifier"] == int(self.chain_id)
@@ -355,27 +357,24 @@
                     return keyval['address']
         except Exception as e:
             self.logger.debug("get_contract_address %s", e)
             return
 
     async def get_token_contract(self, token):
         """Given a token symbol, returns a contract object. """
-        self.logger.debug("get_token_contract %s", token)
         try:
             token_address = await self.search_contract(token)
             token_abi = await self.get_abi(token_address)
             if token_abi is None:
-                self.logger.debug("using setting dex_erc20_abi_url")
-                token_abi = requests.get(settings.dex_erc20_abi_url).text
+                token_abi = await self._get(settings.dex_erc20_abi_url)
             return self.w3.eth.contract(
                 address=token_address,
                 abi=token_abi)
         except Exception as e:
-            self.logger.error("get_token_contract %s", e)
-            return
+            raise e
 
 # 🔒 USER RELATED
     async def get_token_balance(self, token_symbol: str) -> Optional[int]:
         """Get token balance"""
         contract_address = await self.search_contract(token_symbol)
         if not contract_address:
             return None
@@ -397,16 +396,15 @@
                 self.w3.to_checksum_address(self.wallet_address))
             account_balance = self.w3.from_wei(account_balance, 'ether')
             trading_asset_balance = await self.get_trading_asset_balance()
             if trading_asset_balance:
                 account_balance += f"💵{trading_asset_balance}"
             return round(account_balance, 5)
 
-        except Exception as e:
-            self.logger.error(f"get_account_balance: {e}")
+        except Exception:
             return 0
 
     async def get_trading_asset_balance(self):
         try:
             trading_asset_balance = await self.get_token_balance(
                 settings.trading_asset)
             return trading_asset_balance if trading_asset_balance else 0
@@ -444,37 +442,31 @@
                 quote = quoter.functions.quoteExactInputSingle(
                     asset_in_address,
                     asset_out_address,
                     fee, amount, sqrtPriceLimitX96).call()
             return ("🦄 " + quote + " " +
                     settings.trading_asset)
         except Exception as e:
-            self.logger.error("get_quote_uniswap %s", e)
-            return
+            raise e
 
     async def get_approve_uniswap(self, symbol):
         try:
             contract = await self.get_token_contract(symbol)
-            approved_amount = self.w3.to_wei(2**64-1, 'ether')
-            approval_check = contract.functions.allowance(
-                self.w3.to_checksum_address(self.wallet_address),
-                self.w3.to_checksum_address(settings.dex_router_contract_addr)
-            ).call()
-            if approval_check == 0:
-                approval_transaction = contract.functions.approve(
-                    self.w3.to_checksum_address(
-                        settings.dex_router_contract_addr),
-                    approved_amount)
-                approval_txHash = await self.get_sign(approval_transaction)
-                approval_txHash_complete = self.w3.eth.wait_for_transaction_receipt(
-                    approval_txHash, timeout=120, poll_latency=0.1)
-                return approval_txHash_complete
-        except Exception as e:
-            self.logger.error("Error in get_approve_uniswap: %s", e)
-            return None
+            approved_amount = self.w3.to_wei(2 ** 64 - 1, 'ether')
+            owner_address = self.w3.to_checksum_address(self.wallet_address)
+            dex_router_address = self.w3.to_checksum_address(settings.dex_router_contract_addr)
+            allowance = contract.functions.allowance(owner_address, dex_router_address).call()
+            if allowance == 0:
+                approval_tx = contract.functions.approve(dex_router_address, approved_amount)
+                approval_tx_hash = await self.get_sign(approval_tx)
+                approval_receipt = self.w3.eth.wait_for_transaction_receipt(
+                    approval_tx_hash, timeout=120, poll_latency=0.1)
+                return approval_receipt
+        except Exception as error:
+            raise error
 
     async def get_swap_uniswap(self, asset_out_address, asset_in_address, amount):
         try:
             path = [self.w3.to_checksum_address(asset_out_address),
                     self.w3.to_checksum_address(asset_in_address)]
             deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
             router_instance = await self.router()
@@ -485,22 +477,22 @@
                 swap_order = router_instance.functions.swapExactTokensForTokens(
                     int(amount), int(min_amount), tuple(path),
                     self.wallet_address, deadline)
                 return swap_order
             elif self.protocol_type == "uniswap_v3":
                 return None
         except Exception as e:
-            self.logger.error(f"Error in get_swap_uniswap: {e}")
+            raise e
 
 # 0️⃣x
-    async def get_0x_quote(self, buy_token, sell_token, amount=1):
+    async def get_0x_quote(self, buy_address, sell_address, amount=1):
         try:
             out_amount = self.w3.to_wei(amount, 'ether')
-            url = (settings.dex_0x_url + "/swap/v1/quote?buyToken=" + str(buy_token) + 
-                "&sellToken=" + str(sell_token) + "&buyAmount=" + str(out_amount))
+            url = (settings.dex_0x_url + "/swap/v1/quote?buyToken=" + str(buy_address) +
+                "&sellToken=" + str(sell_address) + "&buyAmount=" + str(out_amount))
             headers = {"0x-api-key": settings.dex_0x_api_key}
             response = await self._get(url, params=None, headers=headers)
             print(response)
             if response:
                 return round(float(response['guaranteedPrice']), 3)
         except Exception as e:
             raise e
```

### Comparing `dxsp-2.6.1/pyproject.toml` & `dxsp-2.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.6.1"
+version = "2.6.2"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-2.6.1/PKG-INFO` & `dxsp-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.6.1
+Version: 2.6.2
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

