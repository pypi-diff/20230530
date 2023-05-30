# Comparing `tmp/pymexc-1.0.1.tar.gz` & `tmp/pymexc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pymexc-1.0.1.tar", last modified: Tue May 30 13:49:16 2023, max compression
+gzip compressed data, was "dist\pymexc-1.0.2.tar", last modified: Tue May 30 18:45:17 2023, max compression
```

## Comparing `pymexc-1.0.1.tar` & `pymexc-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 13:49:16.926444 pymexc-1.0.1/
--rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3321 2023-05-30 13:49:16.926444 pymexc-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 13:49:16.909867 pymexc-1.0.1/pymexc/
--rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.1/pymexc/__init__.py
--rw-rw-rw-   0        0        0     5684 2023-05-30 13:09:13.000000 pymexc-1.0.1/pymexc/base.py
--rw-rw-rw-   0        0        0    17551 2023-05-30 13:09:35.000000 pymexc-1.0.1/pymexc/base_websocket.py
--rw-rw-rw-   0        0        0    67170 2023-05-30 13:23:09.000000 pymexc-1.0.1/pymexc/futures.py
--rw-rw-rw-   0        0        0    63611 2023-05-30 13:22:52.000000 pymexc-1.0.1/pymexc/spot.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:49:16.924444 pymexc-1.0.1/pymexc.egg-info/
--rw-rw-rw-   0        0        0     3321 2023-05-30 13:49:16.000000 pymexc-1.0.1/pymexc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-05-30 13:49:16.000000 pymexc-1.0.1/pymexc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 13:49:16.000000 pymexc-1.0.1/pymexc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-30 13:49:16.000000 pymexc-1.0.1/pymexc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-05-30 13:49:16.000000 pymexc-1.0.1/pymexc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-30 13:49:16.000000 pymexc-1.0.1/pymexc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 13:49:16.927445 pymexc-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1697 2023-05-30 13:49:09.000000 pymexc-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:45:17.558055 pymexc-1.0.2/
+-rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3321 2023-05-30 18:45:17.559055 pymexc-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 18:45:17.543052 pymexc-1.0.2/pymexc/
+-rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.2/pymexc/__init__.py
+-rw-rw-rw-   0        0        0     5684 2023-05-30 13:09:13.000000 pymexc-1.0.2/pymexc/base.py
+-rw-rw-rw-   0        0        0    17551 2023-05-30 18:42:16.000000 pymexc-1.0.2/pymexc/base_websocket.py
+-rw-rw-rw-   0        0        0    67093 2023-05-30 18:41:16.000000 pymexc-1.0.2/pymexc/futures.py
+-rw-rw-rw-   0        0        0    67652 2023-05-30 18:31:58.000000 pymexc-1.0.2/pymexc/spot.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:45:17.557055 pymexc-1.0.2/pymexc.egg-info/
+-rw-rw-rw-   0        0        0     3321 2023-05-30 18:45:17.000000 pymexc-1.0.2/pymexc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-30 18:45:17.000000 pymexc-1.0.2/pymexc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 18:45:17.000000 pymexc-1.0.2/pymexc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-30 18:45:17.000000 pymexc-1.0.2/pymexc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-05-30 18:45:17.000000 pymexc-1.0.2/pymexc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 18:45:17.000000 pymexc-1.0.2/pymexc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 18:45:17.560055 pymexc-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1697 2023-05-30 18:44:25.000000 pymexc-1.0.2/setup.py
```

### Comparing `pymexc-1.0.1/LICENSE` & `pymexc-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.1/PKG-INFO` & `pymexc-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.1.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.2.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.1/README.md` & `pymexc-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.1/pymexc/__init__.py` & `pymexc-1.0.2/pymexc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.1/pymexc/base.py` & `pymexc-1.0.2/pymexc/base.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.1/pymexc/base_websocket.py` & `pymexc-1.0.2/pymexc/base_websocket.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.1/pymexc/futures.py` & `pymexc-1.0.2/pymexc/futures.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
         Rate limit: 20 times / 2 seconds
 
         https://mxcdevelop.github.io/apidocs/contract_v1_en/#get-a-snapshot-of-the-latest-n-depth-information-of-the-contract
 
         :param symbol: the name of the contract
         :type symbol: str
-        :param limit: (optional) the limit of the depth
+        :param limit: count
         :type limit: int
 
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", f"api/v1/contract/depth_commits/{symbol}/{limit}")
@@ -299,16 +299,16 @@
         :type limit: int
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", f"api/v1/contract/deals/{symbol}",
                             params = dict(
-                                    symbol    = symbol,
-                                    limit     = limit
+                                    symbol = symbol,
+                                    limit  = limit
                             ))
     
     def ticker(self, symbol: Optional[str] = None) -> dict: 
         """
         ### Get contract trend data
 
         Rate limit: 20 times / 2 seconds
@@ -319,15 +319,15 @@
         :type symbol: str
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", "api/v1/contract/ticker",
                             params = dict(
-                                    symbol    = symbol
+                                    symbol = symbol
                             ))
     
     def risk_reverse(self) -> dict: 
         """
         ### Get all contract risk fund balance
 
         Rate limit: 20 times / 2 seconds
@@ -336,16 +336,16 @@
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", "api/v1/contract/risk_reverse")
     
     def risk_reverse_history(self, 
-                             symbol: str, 
-                             page_num: Optional[int] = 1, 
+                             symbol:    str, 
+                             page_num:  Optional[int] = 1, 
                              page_size: Optional[int] = 20) -> dict: 
         """
         ### Get contract risk fund balance history
 
         Rate limit: 20 times / 2 seconds
 
         https://mxcdevelop.github.io/apidocs/contract_v1_en/#get-contract-risk-fund-balance-history
@@ -425,16 +425,16 @@
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", f"api/v1/private/account/asset/{currency}")
     
     def transfer_record(self, 
                         currency:  Optional[str] = None, 
-                        state:     Optional[Union[Literal["WAIT"], Literal["SUCCESS"], Literal["FAILED"]]] = None, 
-                        type:      Optional[Union[Literal["IN"], Literal["OUT"]]] = None, 
+                        state:     Literal["WAIT", "SUCCESS", "FAILED"] = None, 
+                        type:      Literal["IN", "OUT"] = None, 
                         page_num:  Optional[int] = 1, 
                         page_size: Optional[int] = 20) -> dict:
         """
         ### Get the user's asset transfer records
         #### Required permissions: Account reading permission
 
         Rate limit: 20 times / 2 seconds
@@ -625,15 +625,15 @@
                                     start_time = start_time,
                                     end_time = end_time,
                                     side = side,
                                     page_num = page_num,
                                     page_size = page_size
                             ))
     
-    def external(self, symbol: str, external_oid: int) -> dict:
+    def get_order_external(self, symbol: str, external_oid: int) -> dict:
         """
         ### Query the order based on the external number
         #### Required permissions: Trade reading permission
 
         Rate limit: 20 times / 2 seconds
 
         https://mxcdevelop.github.io/apidocs/contract_v1_en/#query-the-order-based-on-the-external-number
@@ -645,48 +645,46 @@
 
         :return: A dictionary containing the queried order based on the external number.
         :rtype: dict
         """
 
         return self.call("GET", f"api/v1/private/order/external/{symbol}/{external_oid}")
     
-    def get(self, order_id: int) -> dict:
+    def get_order(self, order_id: int) -> dict:
         """
         ### Query the order based on the order number
         #### Required permissions: Trade reading permission
 
         Rate limit: 20 times / 2 seconds
 
         https://mxcdevelop.github.io/apidocs/contract_v1_en/#query-the-order-based-on-the-order-number
 
         :param order_id: The ID of the order to query.
         :type order_id: int
 
         :return: A dictionary containing the queried order based on the order number.
         :rtype: dict
         """
-
         return self.call("GET", f"api/v1/private/order/{order_id}")
     
-    def batch_query(self, order_ids: list) -> dict:
+    def batch_query(self, order_ids: List[int]) -> dict:
         """
         ### Query the order in bulk based on the order number
         #### Required permissions: Trade reading permission
 
         Rate limit: 5 times / 2 seconds
 
         https://mxcdevelop.github.io/apidocs/contract_v1_en/#query-the-order-in-bulk-based-on-the-order-number
 
         :param order_ids: An array of order IDs, separated by ",". Maximum of 50 orders.
         :type order_ids: str
 
         :return: A dictionary containing the queried orders in bulk based on the order number.
         :rtype: dict
         """
-
         return self.call("GET", "api/v1/private/order/batch_query",
                             params = dict(
                                     order_ids = ','.join(order_ids) if isinstance(order_ids, list) else order_ids
                             ))
     
     def deal_details(self, order_id: int) -> dict:
         """
@@ -699,15 +697,14 @@
 
         :param order_id: The ID of the order to retrieve transaction details for.
         :type order_id: int
 
         :return: A dictionary containing the transaction details for the given order ID.
         :rtype: dict
         """
-
         return self.call("GET", f"api/v1/private/order/deal_details/{order_id}")
     
     def order_deals(self, 
                     symbol:     str, 
                     start_time: Optional[int] = None, 
                     end_time:   Optional[int] = None, 
                     page_num:   Optional[int] = 1, 
@@ -739,15 +736,15 @@
                                     symbol = symbol,
                                     start_time = start_time,
                                     end_time = end_time,
                                     page_num = page_num,
                                     page_size = page_size
                             ))
     
-    def planorder_orders(self, 
+    def get_trigger_orders(self, 
                          symbol:     Optional[str] = None, 
                          states:     Optional[str] = None, 
                          start_time: Optional[int] = None, 
                          end_time:   Optional[int] = None, 
                          page_num:   int           = 1, 
                          page_size:  int           = 20) -> dict:
         """
@@ -770,26 +767,25 @@
         :type page_num: int
         :param page_size: page size, default 20, maximum 100
         :type page_size: int
 
         :return: response dictionary
         :rtype: dict
         """
-
         return self.call("GET", f"api/v1/private/planorder/list/orders",
                             params = dict(
                                     symbol = symbol,
                                     states = states,
                                     start_time = start_time,
                                     end_time = end_time,
                                     page_num = page_num,
                                     page_size = page_size
                             ))
 
-    def stoporder_orders(self, 
+    def get_stop_limit_orders(self, 
                          symbol:      Optional[str] = None, 
                          is_finished: Optional[int] = None, 
                          start_time:  Optional[int] = None, 
                          end_time:    Optional[int] = None, 
                          page_num:    int           = 1, 
                          page_size:   int           = 20) -> dict:
         """
@@ -1053,15 +1049,14 @@
                                     externalOid = external_oid,
                                     stopLossPrice = stop_loss_price,
                                     takeProfitPrice = take_profit_price,
                                     positionMode = position_mode,
                                     reduceOnly = reduce_only
                             ))
 
-
     def bulk_order(self, 
                    symbol:            str, 
                    price:             float, 
                    vol:               float, 
                    side:              int, 
                    type:              int, 
                    open_type:         int, 
@@ -1250,15 +1245,14 @@
                                     triggerPrice = trigger_price,
                                     triggerType = trigger_type,
                                     executeCycle = execute_cycle,
                                     orderType = order_type,
                                     trend = trend
                             ))
 
-
     def cancel_trigger_order(self, order_id: int) -> dict:
         """
         ### Cancel the trigger order (Under maintenance)
 
         https://mxcdevelop.github.io/apidocs/contract_v1_en/#cancel-the-trigger-order-under-maintenance
 
         :param orderList: list of orders to be cancelled (maximum of 50)
@@ -1273,15 +1267,15 @@
         """
 
         return self.call("POST", "api/v1/private/planorder/cancel",
                             params = dict(
                                     order_id = order_id
                             ))
 
-    def cancel_all_trigger_order(self, symbol: Optional[str] = None) -> dict:
+    def cancel_all_trigger_orders(self, symbol: Optional[str] = None) -> dict:
         """
         ### Cancel all trigger orders (Under maintenance)
 
         https://mxcdevelop.github.io/apidocs/contract_v1_en/#cancel-all-trigger-orders-under-maintenance
 
         :param symbol: (optional) the name of the contract, cancel specific orders placed under this contract when filled, otherwise, cancel all orders without filling
         :type symbol: str
```

### Comparing `pymexc-1.0.1/pymexc/spot.py` & `pymexc-1.0.2/pymexc/spot.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ws_spot_client.deals_stream(handle_message, "BTCUSDT")
 
 # loop forever for save websocket connection 
 while True: 
     ...
 
 """
-from typing import Callable, Literal, List, Optional
+from typing import Callable, Literal, List, Optional, Union
 import threading, time, logging
 
 logger = logging.getLogger(__name__)
 
 try:
     from base import _SpotHTTP
     from base_websocket import _SpotWebSocket
@@ -179,15 +179,15 @@
         :type end_time: int
         :param limit: (optional) The maximum number of trades to retrieve. Default is 500. Max is 5000.
         :type limit: int
         
         :return: A dictionary containing the retrieved trades.
         :rtype: dict
         """
-        return self.call("GET", "/api/v3/trades", 
+        return self.call("GET", "/api/v3/aggTrades", 
                             params = dict(
                                     symbol    = symbol,
                                     startTime = start_time,
                                     endTime   = end_time,
                                     limit     = limit
                             ))
     
@@ -337,15 +337,15 @@
         return self.call("POST", "api/v3/sub-account/virtualSubAccount", 
                             params = dict(
                                 subAccount = sub_account,
                                 note = note
                             ))
 
 
-    def query_sub_account_list(self, 
+    def sub_account_list(self, 
                                sub_account: Optional[str] = None, 
                                is_freeze: Optional[bool]  = None, 
                                page: Optional[int]        = 1, 
                                limit: Optional[int]       = 10) -> dict:
         """
         ### Get details of the sub-account list.
         #### Required permission: SPOT_ACCOUNT_READ
@@ -373,41 +373,45 @@
                             page = page,
                             limit = limit
                         ))
 
     def create_sub_account_api_key(self, 
                                    sub_account: str, 
                                    note:        str, 
-                                   permissions: str, 
+                                   permissions: Union[str, List[Literal["SPOT_ACCOUNT_READ",     "SPOT_ACCOUNT_WRITE", 
+                                                                        "SPOT_DEAL_READ",        "SPOT_DEAL_WRITE",
+                                                                        "CONTRACT_ACCOUNT_READ", "CONTRACT_ACCOUNT_WRITE",
+                                                                        "CONTRACT_DEAL_READ",    "CONTRACT_DEAL_WRITE", 
+                                                                        "SPOT_TRANSFER_READ",    "SPOT_TRANSFER_WRITE"]]], 
                                    ip:          Optional[str] = None) -> dict:
         """
         ### Create an APIKey for a sub-account.
         #### Required permission: SPOT_ACCOUNT_READ
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#create-an-apikey-for-a-sub-account-for-master-account
 
         :param sub_account: Sub-account Name
         :type sub_account: str
         :param note: APIKey note
         :type note: str
         :param permissions: Permission of APIKey: SPOT_ACCOUNT_READ, SPOT_ACCOUNT_WRITE, SPOT_DEAL_READ, SPOT_DEAL_WRITE, CONTRACT_ACCOUNT_READ, CONTRACT_ACCOUNT_WRITE, CONTRACT_DEAL_READ, CONTRACT_DEAL_WRITE, SPOT_TRANSFER_READ, SPOT_TRANSFER_WRITE
-        :type permissions: str
+        :type permissions: list
         :param ip: (optional) Link IP addresses, separate with commas if more than one. Support up to 20 addresses.
         :type ip: str
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("POST", "api/v3/sub-account/apiKey", 
                         params = dict(
                             subAccount = sub_account,
                             note = note,
-                            permissions = permissions,
+                            permissions = ','.join(permissions) if isinstance(permissions, list) else permissions,
                             ip = ip
                         ))
 
     def query_sub_account_api_key(self, sub_account: str) -> dict:
         """
         ### Query the APIKey of a sub-account.
         #### Applies to master accounts only
@@ -447,17 +451,58 @@
         """
         return self.call("DELETE", "api/v3/sub-account/apiKey", 
                         params = dict(
                             subAccount = sub_account,
                             apiKey = api_key
                         ))
 
+    def universal_transfer(self,
+                           from_account_type: Literal["SPOT", "FUTURES"],
+                           to_account_type:   Literal["SPOT", "FUTURES"],
+                           asset:             str,
+                           amount:            float,
+                           from_account:      Optional[str] = None,
+                           to_account:        Optional[str] = None) -> dict:
+        """
+        ### Universal Transfer (For Master Account)
+        #### Required permission: SPOT_TRANSFER_WRITE
+
+        Weight(IP): 1
+
+        https://mxcdevelop.github.io/apidocs/spot_v3_en/#query-universal-transfer-history-for-master-account
+
+        :param from_account: (optional) Transfer from master account by default if fromAccount is not sent
+        :type from_account: str
+        :param to_account: (optional) Transfer to master account by default if toAccount is not sent
+        :type to_account: str
+        :param from_account_type: fromAccountType:"SPOT","FUTURES"
+        :type from_account_type: str
+        :param to_account_type: toAccountType:"SPOT","FUTURES"
+        :type to_account_type: str
+        :param asset: asset,eg:USDT
+        :type asset: str
+        :param amount: amount,eg:1.82938475
+        :type amount: float
+
+        :return: response dictionary
+        :rtype: dict
+        """
+        return self.call("POST", "api/v3/capital/sub-account/universalTransfer",
+                        params = dict(
+                            fromAccount = from_account,
+                            toAccount = to_account,
+                            fromAccountType = from_account_type,
+                            toAccountType = to_account_type,
+                            asset = asset,
+                            amount = amount
+                        ))
+
     def query_universal_transfer_history(self,
-                                        from_account_type: str,
-                                        to_account_type:   str,
+                                        from_account_type: Literal["SPOT", "FUTURES"],
+                                        to_account_type:   Literal["SPOT", "FUTURES"],
                                         from_account:      Optional[str] = None,
                                         to_account:        Optional[str] = None,
                                         start_time:        Optional[str] = None,
                                         end_time:          Optional[str] = None,
                                         page:              Optional[int] = 1,
                                         limit:             Optional[int] = 500) -> dict:
         """
@@ -466,16 +511,15 @@
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#query-universal-transfer-history-for-master-account
 
         :param from_account: (optional) Transfer from master account by default if fromAccount is not sent
         :type from_account: str
-        :param to_account: (optional) Transfer to master account by default if toAccount is not 
-    sent
+        :param to_account: (optional) Transfer to master account by default if toAccount is not sent
         :type to_account: str
         :param from_account_type: fromAccountType:"SPOT","FUTURES"
         :type from_account_type: str
         :param to_account_type: toAccountType:"SPOT","FUTURES"
         :type to_account_type: str
         :param start_time: (optional) startTime
         :type start_time: str
@@ -517,28 +561,85 @@
                             params = dict(
                                     symbol    = symbol,
                                     startTime = start_time,
                                     endTime   = end_time,
                                     limit     = limit
                             ))
                    
-    def get_self_symbols(self) -> dict:
+    def get_default_symbols(self) -> dict:
         """
         ### User API default symbol.
         #### Required permission: SPOT_ACCOUNT_R
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#user-api-default-symbol
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", "api/v3/selfSymbols")
 
+    def test_new_order(self, 
+                       symbol:              str, 
+                       side:                str, 
+                       order_type:          str, 
+                       quantity:            Optional[int] = None, 
+                       quote_order_qty:     Optional[int] = None, 
+                       price:               Optional[int] = None, 
+                       new_client_order_id: Optional[str] = None, 
+                       stop_price:          Optional[int] = None, 
+                       iceberg_qty:         Optional[int] = None, 
+                       time_in_force:       Optional[str] = None) -> dict:
+        """
+        ### New Order.
+        #### Required permission: SPOT_DEAL_WRITE
+
+        Weight(IP): 1, Weight(UID): 1
+
+        https://mxcdevelop.github.io/apidocs/spot_v3_en/#new-order
+
+        :param symbol: 
+        :type symbol: str
+        :param side: ENUM:Order Side
+        :type side: str
+        :param order_type: ENUM:Order Type
+        :type order_type: str
+        :param quantity: (optional) Quantity
+        :type quantity: int
+        :param quote_order_qty: (optional) Quote order quantity
+        :type quote_order_qty: int
+        :param price: (optional) Price
+        :type price: int
+        :param new_client_order_id: (optional) Unique order id
+        :type new_client_order_id: str
+        :param stop_price: (optional) Stop price
+        :type stop_price: int
+        :param iceberg_qty: (optional) Iceberg quantity
+        :type iceberg_qty: int
+        :param time_in_force: (optional) ENUM:Time In Force
+        :type time_in_force: str
+
+        :return: response dictionary
+        :rtype: dict
+        """
+        return self.call("POST", "/api/v3/order/test", 
+                            params = dict(
+                                    symbol = symbol, 
+                                    side = side, 
+                                    type = order_type, 
+                                    quantity = quantity, 
+                                    quoteOrderQty = quote_order_qty, 
+                                    price = price, 
+                                    newClientOrderId = new_client_order_id, 
+                                    stopPrice = stop_price, 
+                                    icebergQty = iceberg_qty, 
+                                    timeInForce = time_in_force
+                            ))   
+
     def new_order(self, 
                   symbol:              str, 
                   side:                str, 
                   order_type:          str, 
                   quantity:            Optional[int] = None, 
                   quote_order_qty:     Optional[int] = None, 
                   price:               Optional[int] = None, 
@@ -576,38 +677,35 @@
         :type time_in_force: str
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("POST", "api/v3/order", 
                             params = dict(
-                                            symbol = symbol, 
-                                            side = side, 
-                                            type = order_type, 
-                                            quantity = quantity, 
-                                            quoteOrderQty = quote_order_qty, 
-                                            price = price, 
-                                            newClientOrderId = new_client_order_id, 
-                                            stopPrice = stop_price, 
-                                            icebergQty = iceberg_qty, 
-                                            timeInForce = time_in_force
-                                ))    
+                                    symbol = symbol, 
+                                    side = side, 
+                                    type = order_type, 
+                                    quantity = quantity, 
+                                    quoteOrderQty = quote_order_qty, 
+                                    price = price, 
+                                    newClientOrderId = new_client_order_id, 
+                                    stopPrice = stop_price, 
+                                    icebergQty = iceberg_qty, 
+                                    timeInForce = time_in_force
+                            ))    
     
     def batch_orders(self,
-                batch_orders:        List[dict],
-                symbol:              str, 
-                side:                str,
-                order_type:          str,
-                quantity:            Optional[int] = None,
-                quote_order_qty:     Optional[int] = None,
-                price:               Optional[int] = None,
-                new_client_order_id: Optional[str] = None,
-                stop_price:          Optional[int] = None,
-                iceberg_qty:         Optional[int] = None,
-                time_in_force:       Optional[str] = None) -> dict:
+                     batch_orders:        List[str],
+                     symbol:              str, 
+                     side:                Literal["BUY", "SELL"],
+                     order_type:          Literal["LIMIT", "MARKET", "LIMIT_MARKET", "IMMEDIATE_OR_CANCEL", "FILL_OR_KILL"],
+                     quantity:            Optional[int] = None,
+                     quote_order_qty:     Optional[int] = None,
+                     price:               Optional[int] = None,
+                     new_client_order_id: Optional[str] = None) -> dict:
 
         """
         ### Batch Orders
         #### Supports 20 orders with a same symbol in a batch,rate limit:2 times/s.
         #### Required permission: SPOT_DEAL_WRITE
 
         Weight(IP): 1,Weight(UID): 1
@@ -627,45 +725,36 @@
         :type quantity: int
         :param quote_order_qty: (optional) quoteOrderQty
         :type quote_order_qty: int
         :param price: (optional) order price
         :type price: int
         :param new_client_order_id: (optional) ClientOrderId
         :type new_client_order_id: str
-        :param stop_price: (optional) Stop price
-        :type stop_price: int
-        :param iceberg_qty: (optional) Iceberg quantity
-        :type iceberg_qty: int
-        :param time_in_force: (optional) ENUM:Time In Force
-        :type time_in_force: str
 
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("POST", "api/v3/batchOrders",
                         params = dict(
                                 batchOrders = batch_orders,
                                 symbol = symbol,
                                 side = side,
                                 type = order_type,
                                 quantity = quantity,
                                 quoteOrderQty = quote_order_qty,
                                 price = price,
-                                newClientOrderId = new_client_order_id,
-                                stopPrice = stop_price,
-                                icebergQty = iceberg_qty,
-                                timeInForce = time_in_force
+                                newClientOrderId = new_client_order_id
                         ))
 
     def cancel_order(self,
-                symbol:               str,
-                order_id:             Optional[str] = None,
-                orig_client_order_id: Optional[str] = None,
-                new_client_order_id:  Optional[str] = None) -> dict:
+                     symbol:               str,
+                     order_id:             Optional[str] = None,
+                     orig_client_order_id: Optional[str] = None,
+                     new_client_order_id:  Optional[str] = None) -> dict:
         """
         ### Cancel Order.
         #### Required permission: SPOT_DEAL_WRITE
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#cancel-order
@@ -686,16 +775,15 @@
                         params = dict(
                                 symbol = symbol,
                                 orderId = order_id,
                                 origClientOrderId = orig_client_order_id,
                                 newClientOrderId = new_client_order_id
                         ))    
 
-
-    def cancel_all_open_orders_on_symbol(self, symbol: str) -> dict:
+    def cancel_all_open_orders(self, symbol: str) -> dict:
 
         """
         ### Cancel all Open Orders on a Symbol.
         #### Required permission: SPOT_DEAL_WRITE
 
         Weight(IP): 1
 
@@ -705,33 +793,31 @@
         :type symbol: str
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("DELETE", "api/v3/openOrders",
                         params = dict(
-                            symbol = symbol
+                                symbol = symbol
                         ))
 
     def query_order(self,
                     symbol:               str, 
                     orig_client_order_id: Optional[str] = None,
-                    order_id:             Optional[str] = None,
-                    recv_window:          Optional[int] = None) -> dict:
+                    order_id:             Optional[str] = None) -> dict:
 
         """
         ### Query Order.
         #### Required permission: SPOT_DEAL_READ
+        Check an order's status.
 
         Weight(IP): 2
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#query-order
 
-        Check an order's status.
-
         :param symbol: 
         :type symbol: str
         :param orig_client_order_id: (optional) Unique order id
         :type orig_client_order_id: str
         :param order_id: (optional) Order id
         :type order_id: str
         :param recv_window: (optional) Request timeout
@@ -740,16 +826,15 @@
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", "api/v3/order",
                         params = dict(
                                 symbol = symbol,
                                 origClientOrderId = orig_client_order_id,
-                                orderId = order_id,
-                                recvWindow = recv_window
+                                orderId = order_id
                         ))
 
     def current_open_orders(self, symbol: str) -> dict:
 
         """
         ### Current Open Orders.
         #### Required permission: SPOT_DEAL_READ
@@ -763,18 +848,18 @@
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", "api/v3/openOrders", params = dict(symbol = symbol))
 
     def all_orders(self, 
-                symbol:     str, 
-                start_time: Optional[int] = None, 
-                end_time:   Optional[int] = None, 
-                limit:      Optional[int] = None) -> dict:
+                   symbol:     str, 
+                   start_time: Optional[int] = None, 
+                   end_time:   Optional[int] = None, 
+                   limit:      Optional[int] = None) -> dict:
 
         """
         ### All Orders.
         #### Required permission: SPOT_DEAL_READ
 
         Weight(IP): 10
 
@@ -792,18 +877,18 @@
         :type limit: int
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", "api/v3/allOrders",
                         params=dict(
-                            symbol=symbol,
-                            startTime=start_time,
-                            endTime=end_time,
-                            limit=limit
+                                symbol=symbol,
+                                startTime=start_time,
+                                endTime=end_time,
+                                limit=limit
                         ))
 
     def account_information(self) -> dict:
 
         """
         ### Account Information.
         #### Required permission: SPOT_ACCOUNT_READ
@@ -828,15 +913,18 @@
 
         """
         ### Account Trade List.
         #### Required permission: SPOT_ACCOUNT_READ
 
         Weight(IP): 10
 
-        Get trades for a specific account and symbol,Only the transaction records in the past 1 month can be queried. If you want to view more transaction records, please use the export function on the web side, which supports exporting transaction records of the past 3 years at most.
+        Get trades for a specific account and symbol,
+        Only the transaction records in the past 1 month can be queried.
+        If you want to view more transaction records, please use the export function on the web side, 
+        which supports exporting transaction records of the past 3 years at most.
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#account-trade-list
 
         :param symbol: 
         :type symbol: str
         :param order_id: (optional) order Id
         :type order_id: str
@@ -856,19 +944,18 @@
                                 orderId = order_id,
                                 startTime = start_time,
                                 endTime = end_time,
                                 limit = limit
                         ))
 
     def enable_mx_deduct(self, mx_deduct_enable: bool) -> dict:
-
         """
         ### Enable MX Deduct.
-        #### Enable or disable MX deduct for spot commission fee
         #### Required permission: SPOT_DEAL_WRITE
+        Enable or disable MX deduct for spot commission fee
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#enable-mx-deduct
 
         :param mx_deduct_enable: true:enable,false:disable
         :type mx_deduct_enable: bool
@@ -920,15 +1007,14 @@
                  coin:              str,
                  address:           str,
                  amount:            int,
                  withdraw_order_id: Optional[str] = None,
                  network:           Optional[str] = None,
                  memo:              Optional[str] = None,
                  remark:            Optional[str] = None) -> dict:
-
         """
         ### Withdraw.
         #### Required permission: SPOT_WITHDRAW_WRITE
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#withdraw
@@ -1045,25 +1131,24 @@
         :type end_time: str
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", "api/v3/capital/withdraw/history",
                         params = dict(
-                            coin = coin,
-                            status = status,
-                            limit = limit,
-                            startTime = start_time,
-                            endTime = end_time
+                                coin = coin,
+                                status = status,
+                                limit = limit,
+                                startTime = start_time,
+                                endTime = end_time
                         ))
 
     def generate_deposit_address(self, 
-                                 coin:      str, 
-                                 network:   str) -> dict:
-
+                                 coin:    str, 
+                                 network: str) -> dict:
         """
         ### Generate deposit address (supporting network).
         #### Required permission: SPOT_WITHDRAW_WRITE
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#generate-deposit-address-supporting-network
@@ -1081,15 +1166,14 @@
                                 coin = coin,
                                 network = network
                         ))
 
     def deposit_address(self, 
                         coin: str, 
                         network: Optional[str] = None) -> dict:
-
         """
         ### Deposit Address (supporting network).
         #### Required permission: SPOT_WITHDRAW_READ
 
         Weight(IP): 10
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#deposit-address-supporting-network
@@ -1104,19 +1188,18 @@
         """
         return self.call("GET", "api/v3/capital/deposit/address",
                         params = dict(
                                 coin = coin,
                                 network = network,
                         ))
 
-    def withdraw_address_supporting_network(self, 
-                                            coin:  Optional[str] = None, 
-                                            page:  Optional[int] = None, 
-                                            limit: Optional[int] = None) -> dict:
-
+    def withdraw_address(self, 
+                         coin:  Optional[str] = None, 
+                         page:  Optional[int] = None, 
+                         limit: Optional[int] = None) -> dict:
         """
         ### Withdraw Address (supporting network).
         #### Required permission: SPOT_WITHDRAW_R
 
         Weight(IP): 10
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#withdraw-address-supporting-network
@@ -1136,20 +1219,19 @@
         return self.call("GET", "api/v3/capital/withdraw/address",
                         params = dict(
                                 coin = coin,
                                 page = page,
                                 limit = limit
                         ))
 
-    def user_universal_transfer(self,
-                            from_account_type: str,
-                            to_account_type:   str,
-                            asset:             str,
-                            amount:            int) -> dict:
-
+    def user_universal_transfer(self, 
+                                from_account_type: str,
+                                to_account_type:   str,
+                                asset:             str,
+                                amount:            int) -> dict:
         """
         ### User Universal Transfer.
         #### Required permission: SPOT_TRANSFER_WRITE
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#user-universal-transfer
@@ -1170,24 +1252,26 @@
                         params = dict(
                                 fromAccountType = from_account_type,
                                 toAccountType = to_account_type,
                                 asset = asset,
                                 amount = amount
                         ))
 
-    def query_user_universal_transfer_history(self,
-                                        from_account_type: str,
-                                        to_account_type:   str,
+    def user_universal_transfer_history(self,
+                                        from_account_type: Literal["SPOT", "FUTURES"],
+                                        to_account_type:   Literal["SPOT", "FUTURES"],
                                         start_time:        Optional[str] = None,
                                         end_time:          Optional[str] = None,
-                                        page:              Optional[int] = None,
-                                        size:              Optional[int] = None) -> dict:
+                                        page:              Optional[int] = 1,
+                                        size:              Optional[int] = 10) -> dict:
         """
         ### Query User Universal Transfer History.
         #### Required permission: SPOT_TRANSFER_READ
+        Only can quary the data for the last six months
+        If 'startTime' and 'endTime' are not send, will return the last seven days' data by default
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#query-user-universal-transfer-history
 
         :param from_account_type: fromAccountType:"SPOT","FUTURES"
         :type from_account_type: str
@@ -1211,18 +1295,19 @@
                                 toAccountType = to_account_type,
                                 startTime = start_time,
                                 endTime = end_time,
                                 page = page,
                                 size = size
                         ))
 
-    def query_user_universal_transfer_history_by_tranid(self, tran_id: str) -> dict:
+    def user_universal_transfer_history_by_tranid(self, tran_id: str) -> dict:
         """
         ### Query User Universal Transfer History (by tranId).
         #### Required permission: SPOT_TRANSFER_R
+        Only can quary the data for the last six months
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#query-user-universal-transfer-history-by-tranid
 
         :param tran_id: tranId
         :type tran_id: str
@@ -1242,43 +1327,39 @@
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#get-assets-that-can-be-converted-into-mx
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", "api/v3/capital/convert/list")
 
-    def dust_transfer(self, asset: str, amount: str) -> dict:
+    def dust_transfer(self, asset: Union[str, List[str]]) -> dict:
         """
         ### Dust Transfer.
         #### Required permission: SPOT_ACCOUNT_W
 
         Weight(IP): 10
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#dust-transfer
 
         :param asset: The asset being converted.(max 15 assert)eg:asset=BTC,FIL,ETH
-        :type asset: str
-        :param amount: The amount of the asset being converted. eg:amount=10,10,10
-        :type amount: str
+        :type asset: Union[str, List[str]]
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("POST", "api/v3/capital/convert",
                         params = dict(
-                                asset = asset,
-                                amount = amount
+                                asset = ','.join(asset) if isinstance(asset, list) else asset
                         ))
 
     def dustlog(self, 
                 start_time: Optional[int] = None, 
                 end_time:   Optional[int] = None, 
                 page:       Optional[int] = None, 
                 limit:      Optional[int] = None) -> dict:
-
         """
         ### DustLog.
         #### Required permission: SPOT_DEAL_READ
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#dustlog
@@ -1308,15 +1389,14 @@
     # <=================================================================>
     #
     #                               ETF
     #
     # <=================================================================>
 
     def get_etf_info(self, symbol: Optional[str] = None) -> dict:
-
         """
         ### Get ETF info.
         #### Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#get-etf-info
 
         :param symbol: (optional) ETF symbol
@@ -1331,14 +1411,16 @@
                         ))
 
     # <=================================================================>
     #
     #                     Websocket Market Streams
     #
     # <=================================================================>
+    
+    # realized in spot.WebSocket class
 
     # <=================================================================>
     #
     #                   Websocket User Data Streams
     #
     # <=================================================================>
 
@@ -1381,27 +1463,23 @@
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#listen-key
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("DELETE", "api/v3/userDataStream", params = {"please_sign_it": None})
 
-
-
     # <=================================================================>
     #
     #                          Rabate Endpoints
     #
     # <=================================================================>
     def get_rebate_history_records(self, 
                                    start_time: Optional[int] = None, 
                                    end_time:   Optional[int] = None, 
-                                   page:       Optional[int] = None, 
-                                   limit:      Optional[int] = None) -> dict:
-
+                                   page:       Optional[int] = None) -> dict:
         """
         ### Get Rebate History Records.
         #### Required permission: SPOT_ACCOUNT_READ
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#rebate-endpoints
@@ -1409,31 +1487,29 @@
         
         :param start_time: (optional) 
         :type start_time: int
         :param end_time: (optional) 
         :type end_time: int
         :param page: (optional) default 1
         :type page: int
-        :param limit: (optional) default 100
-        :type limit: int
-
-
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", "api/v3/rebate/taxQuery",
                         params = dict(
                                 startTime = start_time,
                                 endTime = end_time,
-                                page = page,
-                                limit = limit
+                                page = page
                         ))
 
-    def get_rebate_records_detail(self, start_time: Optional[int] = None, end_time: Optional[int] = None, page: Optional[int] = None, limit: Optional[int] = None) -> dict:
+    def get_rebate_records_detail(self, 
+                                  start_time: Optional[int] = None,
+                                  end_time:   Optional[int] = None, 
+                                  page:       Optional[int] = None) -> dict:
 
         """
         ### Get Rebate Records Detail.
         #### Required permission: SPOT_ACCOUNT_READ
 
         Weight(IP): 1
 
@@ -1442,79 +1518,68 @@
 
         :param start_time: (optional) 
         :type start_time: int
         :param end_time: (optional) 
         :type end_time: int
         :param page: (optional) default 1
         :type page: int
-        :param limit: (optional) default 100
-        :type limit: int
 
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", "api/v3/rebate/detail", 
                             params = dict(
                                     startTime = start_time, 
                                     endTime = end_time, 
-                                    page = page, 
-                                    limit = limit
+                                    page = page
                             ))
 
     def get_self_rebate_records_detail(self, 
                                        start_time: Optional[int] = None, 
                                        end_time:   Optional[int] = None, 
-                                       page:       Optional[int] = None, 
-                                       limit:      Optional[int] = None) -> dict:
-
+                                       page:       Optional[int] = None) -> dict:
         """
         ### Get Self Rebate Records Detail.
         #### Required permission: SPOT_ACCOUNT_READ
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#get-self-rebate-records-detail
 
         :param start_time: (optional) 
         :type start_time: int
         :param end_time: (optional) 
         :type end_time: int
         :param page: (optional) default 1
         :type page: int
-        :param limit: (optional) default 20
-        :type limit: int
 
         :return: response dictionary
         :rtype: dict
         """
         return self.call("GET", "api/v3/rebate/detail/kickback",
                         params = dict(
                                 startTime = start_time,
                                 endTime = end_time,
-                                page = page,
-                                limit = limit
+                                page = page
                         ))
 
-    def query_refercode(self, symbol: str) -> dict:
+    def query_refercode(self) -> dict:
         """
         ### Query ReferCode.
         #### Required permission: SPOT_ACCOUNT_READ
 
         Weight(IP): 1
 
         https://mxcdevelop.github.io/apidocs/spot_v3_en/#query-refercode
 
-        :param symbol: 
-        :type symbol: str
-
         :return: response dictionary
         :rtype: dict
         """
-        return self.call("GET", "api/v3/rebate/referCode", params=dict(symbol=symbol))
+        return self.call("GET", "api/v3/rebate/referCode", params=dict(please_sign_me = None))
 
 class WebSocket(_SpotWebSocket):
     def __init__(self, 
                  api_key:          Optional[str]  = None, 
                  api_secret:       Optional[str]  = None,
                  listenKey:        Optional[str]  = None,
                  ping_interval:    Optional[int]  = 20,
```

### Comparing `pymexc-1.0.1/pymexc.egg-info/PKG-INFO` & `pymexc-1.0.2/pymexc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.1.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.2.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.1/setup.py` & `pymexc-1.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 :author: abuztrade
 :license: MIT License, see LICENSE file.
 :copyright: (c) 2022 by abuztrade.
 """
 
 
-version = '1.0.1'
+version = '1.0.2'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pymexc",
     version=version,
```

