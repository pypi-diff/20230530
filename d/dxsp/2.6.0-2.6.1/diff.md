# Comparing `tmp/dxsp-2.6.0.tar.gz` & `tmp/dxsp-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.6.0.tar", max compression
+gzip compressed data, was "dxsp-2.6.1.tar", max compression
```

## Comparing `dxsp-2.6.0.tar` & `dxsp-2.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-28 17:08:53.609362 dxsp-2.6.0/LICENSE
--rw-r--r--   0        0        0     2439 2023-05-28 17:08:53.609362 dxsp-2.6.0/README.md
--rw-r--r--   0        0        0       86 2023-05-28 17:08:54.277380 dxsp-2.6.0/dxsp/__init__.py
--rw-r--r--   0        0        0      386 2023-05-28 17:08:53.609362 dxsp-2.6.0/dxsp/config.py
--rw-r--r--   0        0        0     3548 2023-05-28 17:08:53.609362 dxsp-2.6.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    20968 2023-05-28 17:08:53.609362 dxsp-2.6.0/dxsp/main.py
--rw-r--r--   0        0        0     1542 2023-05-28 17:08:54.273380 dxsp-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-30 12:04:39.262743 dxsp-2.6.1/LICENSE
+-rw-r--r--   0        0        0     2348 2023-05-30 12:04:39.262743 dxsp-2.6.1/README.md
+-rw-r--r--   0        0        0       86 2023-05-30 12:04:39.950757 dxsp-2.6.1/dxsp/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-30 12:04:39.262743 dxsp-2.6.1/dxsp/config.py
+-rw-r--r--   0        0        0     3548 2023-05-30 12:04:39.262743 dxsp-2.6.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    19734 2023-05-30 12:04:39.262743 dxsp-2.6.1/dxsp/main.py
+-rw-r--r--   0        0        0     1542 2023-05-30 12:04:39.950757 dxsp-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dxsp-2.6.1/PKG-INFO
```

### Comparing `dxsp-2.6.0/LICENSE` & `dxsp-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.0/README.md` & `dxsp-2.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # DXSP (DeX SwaP)
 
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy |
 | ------------- | ------------- |
-|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br> [![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|Key blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>Key swap protocol (UniV2 router)
+|[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br> [![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|Key blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>Key swap protocol (UniV2 router)
 
 Key features:
 
 - Any blockchains mainnet or testnet supported by web3py, 1inch or uniswap type router.
 
 
 Other features:
@@ -40,13 +40,9 @@
 
 ### Real use case
 
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
 ## Documentation
 
-[wiki](https://github.com/mraniki/dxsp/wiki)
+[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/)
 
-## Questions? Want to help?
-
-[![discord](https://badgen.net/badge/icon/discord/purple?icon=discord&label)](https://discord.gg/vegJQGrRRa)
-[![telegram](https://badgen.net/badge/icon/telegram?icon=telegram&label)](https://t.me/TTTalkyTraderChat/1)
```

### Comparing `dxsp-2.6.0/dxsp/default_settings.toml` & `dxsp-2.6.1/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.0/dxsp/main.py` & `dxsp-2.6.1/dxsp/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,135 +2,244 @@
  DEX SWAP Main
 """
 
 import logging
 from typing import Optional
 
 import requests
-from dxsp import __version__
-from dxsp.config import settings
-
 from pycoingecko import CoinGeckoAPI
 from web3 import Web3
 from web3.gas_strategies.time_based import medium_gas_price_strategy
 
+from dxsp import __version__
+from dxsp.config import settings
 
 class DexSwap:
     """swap  class"""
     def __init__(self, w3: Optional[Web3] = None):
         self.logger = logging.getLogger(name="DexSwap")
-        self.logger.info(f"DexSwap: {__version__}")
 
         self.w3 = w3 or Web3(Web3.HTTPProvider(settings.dex_rpc))
         self.w3.eth.set_gas_price_strategy(medium_gas_price_strategy)
         try:
             if self.w3.net.listening:
-                self.logger.info(f"connected {self.w3}")
-        except Exception as e:
-            self.logger.error(f"connectivity failed {e}")
-            return
+                self.logger.info("connected %s",self.w3)
+        except Exception as error:
+            raise error
 
         self.protocol_type = settings.dex_protocol_type
         self.chain_id = settings.dex_chain_id
         self.wallet_address = self.w3.to_checksum_address(
             settings.dex_wallet_address)
         self.account = str(self.chain_id) + " - "+str(self.wallet_address[-8:])
         self.private_key = settings.dex_private_key
 
+        self.cg = CoinGeckoAPI()
+
+    async def execute_order(self, order_params):
+        """Execute swap function."""
+        action = order_params.get('action')
+        instrument = order_params.get('instrument')
+        quantity = order_params.get('quantity', 1)
+
         try:
-            self.cg = CoinGeckoAPI()
-            asset_platforms = self.cg.get_asset_platforms()
-            output_dict = next(
-                x for x in asset_platforms
-                if x["chain_identifier"] == int(self.chain_id)
-            )
-            self.cg_platform = output_dict["id"]
-            self.logger.debug(f"cg_platform {self.cg_platform}")
-        except Exception as e:
-            self.logger.error(f"CG: {e}")
-
-    async def get_quote(self, symbol):
-        self.logger.debug("get_quote")
-
-        asset_in_address = await self.search_contract(symbol)
-        asset_out_symbol = settings.trading_asset
-        asset_out_address = await self.search_contract(asset_out_symbol)
+            sell_token, buy_token = (
+                (settings.trading_asset, instrument) 
+                if action == 'BUY' 
+                else (instrument, settings.trading_asset))
+
+            sell_contract = await self.get_token_contract(sell_token)
+            sell_decimals = sell_contract.functions.decimals().call() or 18
+
+            sell_balance = await self.get_token_balance(sell_token)
+            risk_percentage = settings.trading_risk_amount
+            sell_amount = (sell_balance / (risk_percentage ** sell_decimals)) * (float(quantity) / 100)
+
+            order = await self.get_swap(sell_token, buy_token, sell_amount)
+            if order:
+                return order['confirmation']
+        except Exception as error:
+            raise error
+
+    async def get_quote(self, sell_token):
+        buy_token = await self.search_contract(settings.trading_asset)
 
-        if asset_out_address is None:
+        if buy_token is None:
             self.logger.warning("No valid contract")
             return
 
         try:
             if self.protocol_type in {"uniswap_v2", "uniswap_v3"}:
-                self.logger.debug("uniswap getquote")
-                return await self.get_quote_uniswap(
-                    asset_in_address,
-                    asset_out_address)
+                return await self.get_quote_uniswap(sell_token, buy_token)
 
             if self.protocol_type == "0x":
-                self.logger.debug("0x getquote")
-                return await self.get_0x_quote(
-                    asset_in_address,
-                    asset_out_address)
+                return await self.get_0x_quote(sell_token, buy_token)
 
-        except Exception as e:
-            self.logger.error("get_quote %s", e)
-            return
+        except Exception as error:
+            raise error
 
-    async def get_swap(
-        self, asset_out_symbol: str, asset_in_symbol: str, amount: int
-    ) -> None:
+    async def get_swap(self, sell_token: str, buy_token: str, amount: int) -> None:
         """Main swap function"""
         try:
-            asset_out_address = await self.search_contract(
-                asset_out_symbol)
-            asset_out_contract = await self.get_token_contract(
-                asset_out_symbol)
-            if asset_out_contract is None:
-                raise ValueError("No contract identified")
-            asset_out_balance = await self.get_token_balance(
-                asset_out_symbol)
-            if asset_out_balance in (0, None):
-                raise ValueError("No Money")
+            sell_token_address = await self.search_contract(sell_token)
+            sell_token_balance = await self.get_token_balance(sell_token)
+            if not sell_token_address or sell_token_balance in (0, None):
+                return
 
-            asset_in_address = await self.search_contract(asset_in_symbol)
-            if asset_in_address is None:
+            buy_token_address = await self.search_contract(buy_token)
+            if not buy_token_address:
                 return
 
-            asset_out_decimals = asset_out_contract.functions.decimals().call()
-            asset_out_amount = amount * 10 ** asset_out_decimals
-            asset_out_amount_converted = self.w3.to_wei(
-                asset_out_amount, "ether")
+            sell_token_amount_wei = self.w3.to_wei(amount * 10 ** (await self.get_token_decimals(sell_token)), "ether")
 
-            order_amount = int(asset_out_amount_converted * (
-                settings.dex_trading_slippage / 100))
+            if await self.get_approve(sell_token) is None:
+                return
 
-            if await self.get_approve(asset_out_symbol) is None:
+            swap_order = await self.get_swap_order(sell_token_address, buy_token_address, sell_token_amount_wei)
+            if not swap_order:
                 return
 
-            swap_order = None
-            if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
-                swap_order = await self.get_swap_uniswap(
-                    asset_out_address, asset_in_address, order_amount)
-            elif self.protocol_type == "0x":
-                swap_order = await self.get_0x_quote(
-                    asset_out_address, asset_in_address, order_amount)
+            if self.protocol_type == "0x":
                 await self.get_sign(swap_order)
 
-            if swap_order:
-                signed_order = await self.get_sign(swap_order)
-                order_hash = str(self.w3.to_hex(signed_order))
-                order_hash_details = self.w3.wait_for_transaction_receipt(
-                    order_hash, timeout=120, poll_latency=0.1)
-                if order_hash_details["status"] == 1:
-                    await self.get_confirmation(order_hash)
+            signed_order = await self.get_sign(swap_order)
+            order_hash = str(self.w3.to_hex(signed_order))
+
+            if self.w3.wait_for_transaction_receipt(order_hash, timeout=120, poll_latency=0.1)["status"] != 1:
+                return
+
+            await self.get_confirmation(order_hash)
+
+        except Exception as error:
+            raise error
+
+### ------🛠️ W3 UTILS ---------
+
+
+    async def _get(
+        self,
+        url,
+        params=None,
+        headers=None
+            ):
+        try:
+            self.logger.debug("url: %s", url)
+            # self.logger.debug("_header: %s", settings.headers)
+            response = requests.get(
+                url,
+                params=params,
+                headers=headers,
+                timeout=10)
+            self.logger.debug("_response: %s", response)
+            if response:
+                self.logger.debug("_json: %s", response.json())
+                return response.json()
+
+        except Exception as e:
+            self.logger.error("_get: %s", e)
+
+    async def router(self):
+        try:
+            router_abi = await self.get_abi(settings.dex_router_contract_addr)
+            if router_abi is None:
+                self.logger.debug("using setting dex_router_abi_url")
+                router_abi = requests.get(settings.dex_router_abi_url).text
+            self.logger.debug("router_abi: %s", router_abi)
+            router = self.w3.eth.contract(
+                address=self.w3.to_checksum_address(
+                    settings.dex_router_contract_addr),
+                abi=router_abi)
+            return router
+        except Exception as e:
+            self.logger.error("router setup: %s", e)
+
+    async def get_name(self):
+        try:
+            return settings.dex_router_contract_addr[-8:]
+        except Exception as e:
+            self.logger.error("router name %s", e)
+
+    async def quoter(self):
+        try:
+            quoter_abi = await self.get_abi(settings.dex_quoter_contract_addr)
+            self.logger.debug("quoter_abi: %s", quoter_abi)
+            contract = self.w3.eth.contract(
+                address=self.w3.to_checksum_address(
+                    settings.dex_quoter_contract_addr),
+                abi=quoter_abi)
+            return contract
+        except Exception as e:
+            self.logger.error("quoter setup: %s", e)
+
+    async def get_approve(self, symbol):
+        try:
+            if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
+                await self.get_approve_uniswap(symbol)
+        except Exception as e:
+            self.logger.error("Error in get_approve: %s", e)
+            return None
 
+    async def get_sign(self, transaction):
+        try:
+            if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
+                transaction_params = {
+                    'from': self.wallet_address,
+                    'gas': await self.get_gas(transaction),
+                    'gasPrice': await self.get_gas_price(),
+                    'nonce': self.w3.eth.get_transaction_count(
+                        self.wallet_address),
+                }
+                transaction = transaction.build_transaction(transaction_params)
+            signed = self.w3.eth.account.sign_transaction(
+                transaction, self.private_key)
+            tx_hash = self.w3.eth.send_raw_transaction(signed.rawTransaction)
+            return tx_hash
+        except (ValueError, TypeError, KeyError) as e:
+            self.logger.error("Failed to sign transaction: %s", e)
+            raise
         except Exception as e:
-            self.logger.error("Error in get_swap: %s", e)
-            return e
+            self.logger.error("Failed to sign transaction: %s", e)
+            raise RuntimeError("Failed to sign transaction")
+
+    async def get_abi(self, address):
+        if not settings.dex_block_explorer_api:
+            self.logger.warning("No block_explorer_api.")
+            return None
+
+        params = {
+            "module": "contract",
+            "action": "getabi",
+            "address": address,
+            "apikey": settings.dex_block_explorer_api
+        }
+
+        try:
+            resp = await self._get(
+                url=settings.dex_block_explorer_url, params=params)
+            if resp['status'] == "1":
+                self.logger.debug("ABI found %s", resp)
+                return resp["result"]
+            else:
+                self.logger.warning("No ABI identified")
+                return None
+        except Exception as error:
+            self.logger.error("get_abi %s", error)
+            return None
+
+    async def get_swap_order(self, sell_token_address: str, buy_token_address: str, sell_token_amount_wei: int) -> Optional[str]:
+        """Get swap order"""
+        order_amount = int(sell_token_amount_wei * (settings.dex_trading_slippage / 100))
+
+        if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
+            return await self.get_swap_uniswap(sell_token_address, buy_token_address, order_amount)
+        elif self.protocol_type == "0x":
+            order = await self.get_0x_quote(sell_token_address, buy_token_address, order_amount)
+            return order if not order else await self.get_sign(order)
+
+        return None
 
     async def get_confirmation(self, order_hash):
         """Returns trade confirmation."""
         try:
             receipt = self.w3.eth.get_transaction(order_hash)
             block = self.w3.eth.get_block(receipt["blockNumber"])
             trade = {
@@ -145,59 +254,30 @@
                     f"➕ Size: {round(receipt['value'], 4)}\n"
                     f"⚫️ Entry: {round(receipt['value'], 4)}\n"
                     f"ℹ️ {receipt['blockHash']}\n"
                     f"🗓️ {block['timestamp']}"
                 ),
             }
             return trade
-        except Exception as e:
-            self.logger.error("Error getting trade confirmation: %s", e)
+        except Exception as error:
+            raise error
 
-    async def execute_order(self, order_params):
-        """Execute swap function."""
-        action = order_params.get('action')
-        instrument = order_params.get('instrument')
-        quantity = order_params.get('quantity', 1)
-
-        try:
-            if action == "BUY":
-                asset_out_symbol = settings.trading_asset
-                asset_in_symbol = instrument
-            else:
-                asset_out_symbol = instrument
-                asset_in_symbol = settings.trading_asset
-
-            try:
-                asset_out_contract = await self.get_token_contract(
-                    asset_out_symbol)
-                asset_out_decimals = asset_out_contract.functions.decimals().call() or 18
-            except Exception as e:
-                self.logger.error("execute_order decimals: %s", e)
-                asset_out_decimals = 18
-
-            asset_out_balance = await self.get_token_balance(asset_out_symbol)
-
-            # Amount to risk percentage - DEFAULT OPTION is 10%
-            asset_out_amount = (
-                asset_out_balance /
-                (settings.trading_risk_amount ** asset_out_decimals)) * (
-                    float(quantity) / 100)
-
-            order = await self.get_swap(
-                asset_out_symbol,
-                asset_in_symbol,
-                asset_out_amount
-            )
-            if order:
-                return order['confirmation']
+    async def get_gas(self, tx):
+        gas_estimate = self.w3.eth.estimate_gas(tx) * 1.25
+        self.logger.debug("gas_estimate %s", gas_estimate)
+        return int(self.w3.to_wei(gas_estimate, 'wei'))
 
-        except Exception as e:
-            self.logger.debug("error execute_order %s", e)
-            return "error processing order in DXSP"
+    async def get_gas_price(self):
+        gas_price = round(self.w3.from_wei(
+            self.w3.eth.generate_gas_price(),
+            'gwei'), 2)
+        self.logger.debug("gas_price %s", gas_price)
+        return gas_price
 
+### ------✍️ CONTRACT ---------
     async def search_contract(self, token):
         """search a contract function"""
         self.logger.debug("search_contract")
 
         try:
             contract_lists = [
                 settings.token_personal_list,
@@ -218,42 +298,51 @@
             token_contract = await self.search_cg_contract(token)
             if token_contract is not None:
                 self.logger.info("%s token: contract found %s",
                                  token, token_contract)
                 return self.w3.to_checksum_address(token_contract)
 
             return f"no contract found for {token}"
-        except Exception as e:
-            self.logger.error("search_contract %s", e)
-            return
+        except Exception as error:
+            raise error
+
+    async def search_cg_platform(self):
+        """search coingecko platform"""
+        asset_platforms = self.cg.get_asset_platforms()
+        output_dict = next(
+            x for x in asset_platforms
+            if x["chain_identifier"] == int(self.chain_id)
+        )
+        cg_platform = output_dict["id"] or None
+        return cg_platform
 
     async def search_cg(self, token):
         """search coingecko"""
         try:
             search_results = self.cg.search(query=token)
             search_dict = search_results['coins']
             filtered_dict = [x for x in search_dict if
                              x['symbol'] == token.upper()]
             api_dict = [sub['api_symbol'] for sub in filtered_dict]
             for i in api_dict:
                 coin_dict = self.cg.get_coin_by_id(i)
                 try:
-                    if coin_dict['platforms'][f'{self.cg_platform}']:
+                    if coin_dict['platforms'][f'{await self.search_cg_platform()}']:
                         return coin_dict
                 except (KeyError, requests.exceptions.HTTPError):
                     pass
         except Exception as e:
             self.logger.error("search_cg %s", e)
             return
 
     async def search_cg_contract(self, token):
         """search coingecko contract"""
         try:
             coin_info = await self.search_cg(token)
-            return (coin_info['platforms'][f'{self.cg_platform}']
+            return (coin_info['platforms'][f'{await self.search_cg_platform()}']
                     if coin_info is not None else None)
         except Exception as e:
             self.logger.error(" search_cg_contract: %s", e)
             return
 
     async def get_contract_address(self, token_list_url, symbol):
         """Given a token symbol and json tokenlist, get token address"""
@@ -280,158 +369,40 @@
             return self.w3.eth.contract(
                 address=token_address,
                 abi=token_abi)
         except Exception as e:
             self.logger.error("get_token_contract %s", e)
             return
 
-# 🛠️ W3 UTILS
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
-            # self.logger.debug("_response: %s", response)
-            if response:
-                # self.logger.debug("_json: %s", response.json())
-                return response.json()
-
-        except Exception as e:
-            self.logger.error("_get: %s", e)
-
-    async def router(self):
-        try:
-            router_abi = await self.get_abi(settings.dex_router_contract_addr)
-            if router_abi is None:
-                self.logger.debug("using setting dex_router_abi_url")
-                router_abi = requests.get(settings.dex_router_abi_url).text
-            self.logger.debug("router_abi: %s", router_abi)
-            router = self.w3.eth.contract(
-                address=self.w3.to_checksum_address(
-                    settings.dex_router_contract_addr),
-                abi=router_abi)
-            return router
-        except Exception as e:
-            self.logger.error("router setup: %s", e)
-
-    async def quoter(self):
-        try:
-            quoter_abi = await self.get_abi(settings.dex_quoter_contract_addr)
-            self.logger.debug("quoter_abi: %s", quoter_abi)
-            contract = self.w3.eth.contract(
-                address=self.w3.to_checksum_address(
-                    settings.dex_quoter_contract_addr),
-                abi=quoter_abi)
-            return contract
-        except Exception as e:
-            self.logger.error("quoter setup: %s", e)
-
-    async def get_approve(self, symbol):
-        try:
-            if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
-                await self.get_approve_uniswap(symbol)
-        except Exception as e:
-            self.logger.error("Error in get_approve: %s", e)
+# 🔒 USER RELATED
+    async def get_token_balance(self, token_symbol: str) -> Optional[int]:
+        """Get token balance"""
+        contract_address = await self.search_contract(token_symbol)
+        if not contract_address:
             return None
-
-    async def get_sign(self, transaction):
-        try:
-            if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
-                transaction_params = {
-                    'from': self.wallet_address,
-                    'gas': await self.get_gas(transaction),
-                    'gasPrice': await self.get_gas_price(),
-                    'nonce': self.w3.eth.get_transaction_count(
-                        self.wallet_address),
-                }
-                transaction = transaction.build_transaction(transaction_params)
-            signed = self.w3.eth.account.sign_transaction(
-                transaction, self.private_key)
-            tx_hash = self.w3.eth.send_raw_transaction(signed.rawTransaction)
-            return tx_hash
-        except (ValueError, TypeError, KeyError) as e:
-            self.logger.error("Failed to sign transaction: %s", e)
-            raise
-        except Exception as e:
-            self.logger.error("Failed to sign transaction: %s", e)
-            raise RuntimeError("Failed to sign transaction")
-
-    async def get_gas(self, tx):
-        gas_estimate = self.w3.eth.estimate_gas(tx) * 1.25
-        self.logger.debug("gas_estimate %s", gas_estimate)
-        return int(self.w3.to_wei(gas_estimate, 'wei'))
-
-    async def get_gas_price(self):
-        gas_price = round(self.w3.from_wei(
-            self.w3.eth.generate_gas_price(),
-            'gwei'), 2)
-        self.logger.debug("gas_price %s", gas_price)
-        return gas_price
-
-    async def get_abi(self, address):
-        if not settings.dex_block_explorer_api:
-            self.logger.warning("No block_explorer_api.")
+        contract = await self.get_token_contract(token_symbol)
+        if not contract:
             return None
+        return contract.functions.balanceOf(self.wallet_address).call() or 0
 
-        params = {
-            "module": "contract",
-            "action": "getabi",
-            "address": address,
-            "apikey": settings.dex_block_explorer_api
-        }
-
-        try:
-            resp = await self._get(
-                url=settings.dex_block_explorer_url, params=params)
-            if resp['status'] == "1":
-                self.logger.debug("ABI found %s", resp)
-                return resp["result"]
-            else:
-                self.logger.warning("No ABI identified")
-                return None
-        except Exception as e:
-            self.logger.error("get_abi %s", e)
+    async def get_token_decimals(self, token_symbol: str) -> Optional[int]:
+        """Get token decimals"""
+        contract = await self.get_token_contract(token_symbol)
+        if not contract:
             return None
-
-    async def get_name(self):
-        try:
-            return settings.dex_router_contract_addr[-8:]
-        except Exception as e:
-            self.logger.error("router name %s", e)
-# 🔒 USER RELATED
-    async def get_token_balance(self, token):
-        try:
-            contract = await self.get_token_contract(token)
-            balance = contract.functions.balanceOf(self.wallet_address).call()
-            return max(0, balance)
-        except Exception as e:
-            self.logger.error("Failed to get token balance: %s", e)
-            return 0
+        return int(await contract.functions.decimals().call())
 
     async def get_account_balance(self):
         try:
             account_balance = self.w3.eth.get_balance(
                 self.w3.to_checksum_address(self.wallet_address))
             account_balance = self.w3.from_wei(account_balance, 'ether')
-            try:
-                trading_asset_balance = await self.get_trading_asset_balance()
-                if trading_asset_balance:
-                    account_balance += f"💵{trading_asset_balance}"
-            except Exception:
-                pass
-
+            trading_asset_balance = await self.get_trading_asset_balance()
+            if trading_asset_balance:
+                account_balance += f"💵{trading_asset_balance}"
             return round(account_balance, 5)
 
         except Exception as e:
             self.logger.error(f"get_account_balance: {e}")
             return 0
 
     async def get_trading_asset_balance(self):
@@ -517,30 +488,19 @@
                 return swap_order
             elif self.protocol_type == "uniswap_v3":
                 return None
         except Exception as e:
             self.logger.error(f"Error in get_swap_uniswap: {e}")
 
 # 0️⃣x
-    async def get_0x_quote(
-        self,
-        in_address,
-        out_address,
-        amount=1
-    ):
+    async def get_0x_quote(self, buy_token, sell_token, amount=1):
         try:
             out_amount = self.w3.to_wei(amount, 'ether')
-            url = (
-                settings.dex_0x_url
-                + "/swap/v1/quote?buyToken="
-                + str(in_address)
-                + "&sellToken="
-                + str(out_address)
-                + "&buyAmount="
-                + str(out_amount))
+            url = (settings.dex_0x_url + "/swap/v1/quote?buyToken=" + str(buy_token) + 
+                "&sellToken=" + str(sell_token) + "&buyAmount=" + str(out_amount))
             headers = {"0x-api-key": settings.dex_0x_api_key}
             response = await self._get(url, params=None, headers=headers)
+            print(response)
             if response:
-                quote = response['guaranteedPrice']
-                return round(float(quote), 3)
+                return round(float(response['guaranteedPrice']), 3)
         except Exception as e:
-            self.logger.error("get_0x_quote %s", e)
+            raise e
```

### Comparing `dxsp-2.6.0/pyproject.toml` & `dxsp-2.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.6.0"
+version = "2.6.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-2.6.0/PKG-INFO` & `dxsp-2.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.6.0
+Version: 2.6.1
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
 
 # DXSP (DeX SwaP)
 
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy |
 | ------------- | ------------- |
-|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br> [![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|Key blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>Key swap protocol (UniV2 router)
+|[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br> [![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|Key blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>Key swap protocol (UniV2 router)
 
 Key features:
 
 - Any blockchains mainnet or testnet supported by web3py, 1inch or uniswap type router.
 
 
 Other features:
@@ -61,14 +61,10 @@
 
 ### Real use case
 
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
 ## Documentation
 
-[wiki](https://github.com/mraniki/dxsp/wiki)
+[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/)
 
-## Questions? Want to help?
-
-[![discord](https://badgen.net/badge/icon/discord/purple?icon=discord&label)](https://discord.gg/vegJQGrRRa)
-[![telegram](https://badgen.net/badge/icon/telegram?icon=telegram&label)](https://t.me/TTTalkyTraderChat/1)
```

