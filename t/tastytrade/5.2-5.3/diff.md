# Comparing `tmp/tastytrade-5.2.tar.gz` & `tmp/tastytrade-5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-5.2.tar", last modified: Mon May 22 02:05:21 2023, max compression
+gzip compressed data, was "tastytrade-5.3.tar", last modified: Tue May 30 18:57:37 2023, max compression
```

## Comparing `tastytrade-5.2.tar` & `tastytrade-5.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:05:21.518469 tastytrade-5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-22 02:05:09.000000 tastytrade-5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-22 02:05:21.518469 tastytrade-5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-05-22 02:05:09.000000 tastytrade-5.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 02:05:21.518469 tastytrade-5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-22 02:05:09.000000 tastytrade-5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:05:21.514469 tastytrade-5.2/tastytrade/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34247 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:05:21.518469 tastytrade-5.2/tastytrade/dxfeed/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/candle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/greeks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/theoprice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/dxfeed/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    19387 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-22 02:05:09.000000 tastytrade-5.2/tastytrade/watchlists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:05:21.514469 tastytrade-5.2/tastytrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-22 02:05:21.000000 tastytrade-5.2/tastytrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-22 02:05:21.000000 tastytrade-5.2/tastytrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 02:05:21.000000 tastytrade-5.2/tastytrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-22 02:05:21.000000 tastytrade-5.2/tastytrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 02:05:21.000000 tastytrade-5.2/tastytrade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:57:37.089625 tastytrade-5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-30 18:57:26.000000 tastytrade-5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-30 18:57:37.085625 tastytrade-5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-05-30 18:57:26.000000 tastytrade-5.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:57:37.089625 tastytrade-5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-30 18:57:26.000000 tastytrade-5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:57:37.085625 tastytrade-5.3/tastytrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34247 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:57:37.085625 tastytrade-5.3/tastytrade/dxfeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/greeks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/theoprice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/timeandsale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/dxfeed/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20874 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-30 18:57:26.000000 tastytrade-5.3/tastytrade/watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:57:37.085625 tastytrade-5.3/tastytrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-30 18:57:37.000000 tastytrade-5.3/tastytrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-30 18:57:37.000000 tastytrade-5.3/tastytrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:57:37.000000 tastytrade-5.3/tastytrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-30 18:57:37.000000 tastytrade-5.3/tastytrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 18:57:37.000000 tastytrade-5.3/tastytrade.egg-info/top_level.txt
```

### Comparing `tastytrade-5.2/LICENSE` & `tastytrade-5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/PKG-INFO` & `tastytrade-5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.2
+Version: 5.3
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -22,15 +22,15 @@
    :alt: PyPI Downloads
 
 Tastytrade Python SDK
 =====================
 
 .. inclusion-marker
 
-A simple, reverse-engineered SDK for Tastytrade built on their (mostly) public API. This will allow you to create trading algorithms for whatever strategies you may have quickly and painlessly in Python.
+A simple, reverse-engineered SDK for Tastytrade built on their (now mostly public) API. This will allow you to create trading algorithms for whatever strategies you may have quickly and painlessly in Python.
 
 Installation
 ------------
 
 .. code-block:: bash
 
    $ pip install tastytrade
```

### Comparing `tastytrade-5.2/README.rst` & `tastytrade-5.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
    :alt: PyPI Downloads
 
 Tastytrade Python SDK
 =====================
 
 .. inclusion-marker
 
-A simple, reverse-engineered SDK for Tastytrade built on their (mostly) public API. This will allow you to create trading algorithms for whatever strategies you may have quickly and painlessly in Python.
+A simple, reverse-engineered SDK for Tastytrade built on their (now mostly public) API. This will allow you to create trading algorithms for whatever strategies you may have quickly and painlessly in Python.
 
 Installation
 ------------
 
 .. code-block:: bash
 
    $ pip install tastytrade
```

### Comparing `tastytrade-5.2/setup.py` & `tastytrade-5.3/setup.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/account.py` & `tastytrade-5.3/tastytrade/account.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/dxfeed/candle.py` & `tastytrade-5.3/tastytrade/dxfeed/candle.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/dxfeed/event.py` & `tastytrade-5.3/tastytrade/dxfeed/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,20 @@
     the quote streamer.
 
     Information on different types of events, their uses and their properties can be
     found at the `dxfeed Knowledge Base <https://kb.dxfeed.com/en/data-model/dxfeed-api-market-events.html>`_.
     """
     CANDLE = 'Candle'
     GREEKS = 'Greeks'
-    QUOTE = 'Quote'
-    TRADE = 'Trade'
     PROFILE = 'Profile'
+    QUOTE = 'Quote'
     SUMMARY = 'Summary'
     THEO_PRICE = 'TheoPrice'
+    TIME_AND_SALE = 'TimeAndSale'
+    TRADE = 'Trade'
 
 
 class Event(ABC):
     @classmethod
     def from_stream(cls, data: list) -> list['Event']:
         """
         Takes a list of raw trade data fetched by :class:`~tastyworks.streamer.DataStreamer`
```

### Comparing `tastytrade-5.2/tastytrade/dxfeed/greeks.py` & `tastytrade-5.3/tastytrade/dxfeed/greeks.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/dxfeed/profile.py` & `tastytrade-5.3/tastytrade/dxfeed/profile.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/dxfeed/quote.py` & `tastytrade-5.3/tastytrade/dxfeed/quote.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/dxfeed/summary.py` & `tastytrade-5.3/tastytrade/dxfeed/summary.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/dxfeed/theoprice.py` & `tastytrade-5.3/tastytrade/dxfeed/theoprice.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/dxfeed/trade.py` & `tastytrade-5.3/tastytrade/dxfeed/trade.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/instruments.py` & `tastytrade-5.3/tastytrade/instruments.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/metrics.py` & `tastytrade-5.3/tastytrade/metrics.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/order.py` & `tastytrade-5.3/tastytrade/order.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,20 @@
     RECEIVED = 'Received'
     CANCELLED = 'Cancelled'
     FILLED = 'Filled'
     EXPIRED = 'Expired'
     LIVE = 'Live'
     REJECTED = 'Rejected'
     CONTINGENT = 'Contingent'
+    ROUTED = 'Routed'
+    IN_FLIGHT = 'In Flight'
+    CANCEL_REQUESTED = 'Cancel Requested'
+    REPLACE_REQUESTED = 'Replace Requested'
+    REMOVED = 'Removed'
+    PARTIALLY_REMOVED = 'Partially Removed'
 
 
 class OrderTimeInForce(str, Enum):
     """
     This is an :class:`~enum.Enum` that contains the valid TIFs for orders.
     """
     DAY = 'Day'
```

### Comparing `tastytrade-5.2/tastytrade/search.py` & `tastytrade-5.3/tastytrade/search.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/session.py` & `tastytrade-5.3/tastytrade/session.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/streamer.py` & `tastytrade-5.3/tastytrade/streamer.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 from enum import Enum
 from typing import Any, AsyncIterator, Optional, Union
 
 import requests
 import websockets
 
 from tastytrade import logger
-from tastytrade.account import Account
+from tastytrade.account import (Account, AccountBalance, CurrentPosition,
+                                TradingStatus)
 from tastytrade.dxfeed import Channel
 from tastytrade.dxfeed.candle import Candle
 from tastytrade.dxfeed.event import Event, EventType
 from tastytrade.dxfeed.greeks import Greeks
 from tastytrade.dxfeed.profile import Profile
 from tastytrade.dxfeed.quote import Quote
 from tastytrade.dxfeed.summary import Summary
 from tastytrade.dxfeed.theoprice import TheoPrice
+from tastytrade.dxfeed.timeandsale import TimeAndSale
 from tastytrade.dxfeed.trade import Trade
+from tastytrade.order import PlacedOrder
 from tastytrade.session import Session
 from tastytrade.utils import TastytradeError, validate_response
 
 CERT_STREAMER_URL = 'wss://streamer.cert.tastyworks.com'
 STREAMER_URL = 'wss://streamer.tastyworks.com'
 
 
@@ -97,22 +100,59 @@
             self._heartbeat_task = asyncio.create_task(self._heartbeat())
 
             while not self._done:
                 raw_message = await self._websocket.recv()  # type: ignore
                 logger.debug('raw message: %s', raw_message)
                 await self._queue.put(json.loads(raw_message))
 
-    async def listen(self) -> AsyncIterator[Any]:
+    async def listen(self) -> AsyncIterator[Union[
+        AccountBalance,
+        CurrentPosition,
+        PlacedOrder,
+        TradingStatus,
+        dict  # some possible messages are not yet implemented
+    ]]:
         """
-        Iterate over non-heartbeat messages received from the streamer.
+        Iterate over non-heartbeat messages received from the streamer,
+        mapping them to their appropriate data class.
         """
         while True:
             data = await self._queue.get()
-            if data.get('action') != SubscriptionType.HEARTBEAT:
-                yield data
+            type_str = data.get('type')
+            if type_str is not None:
+                yield self._map_message(type_str, data['data'])
+            elif data.get('action') != 'heartbeat':
+                logger.debug('subscription message: %s', data)
+
+    def _map_message(self, type_str: str, data: dict) -> Union[
+        AccountBalance,
+        CurrentPosition,
+        PlacedOrder,
+        TradingStatus,
+        dict  # some possible messages are not yet implemented
+    ]:
+        """
+        TODO: implement the following:
+        - OrderChain
+        - UnderlyingYearGainSummary
+        - User status related messages
+        - Watchlist related messages
+        - Quote alert messages
+        - Others?
+        """
+        if type_str == 'AccountBalance':
+            return AccountBalance(**data)
+        elif type_str == 'CurrentPosition':
+            return CurrentPosition(**data)
+        elif type_str == 'Order':
+            return PlacedOrder(**data)
+        elif type_str == 'TradingStatus':
+            return TradingStatus(**data)
+        else:
+            return data
 
     async def account_subscribe(self, accounts: list[Account]) -> None:
         """
         Subscribes to account-level updates (balances, orders, positions).
 
         :param accounts: list of :class:`tastytrade.account.Account`s to subscribe to updates for
         """
@@ -493,13 +533,15 @@
         res = Profile.from_stream(data)
     elif msg_type == EventType.QUOTE:
         res = Quote.from_stream(data)
     elif msg_type == EventType.SUMMARY:
         res = Summary.from_stream(data)
     elif msg_type == EventType.THEO_PRICE:
         res = TheoPrice.from_stream(data)
+    elif msg_type == EventType.TIME_AND_SALE:
+        res = TimeAndSale.from_stream(data)
     elif msg_type == EventType.TRADE:
         res = Trade.from_stream(data)
     else:
         raise TastytradeError(f'Unknown message type received from streamer: {message}')
 
     return res
```

### Comparing `tastytrade-5.2/tastytrade/utils.py` & `tastytrade-5.3/tastytrade/utils.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade/watchlists.py` & `tastytrade-5.3/tastytrade/watchlists.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.2/tastytrade.egg-info/PKG-INFO` & `tastytrade-5.3/tastytrade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.2
+Version: 5.3
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -22,15 +22,15 @@
    :alt: PyPI Downloads
 
 Tastytrade Python SDK
 =====================
 
 .. inclusion-marker
 
-A simple, reverse-engineered SDK for Tastytrade built on their (mostly) public API. This will allow you to create trading algorithms for whatever strategies you may have quickly and painlessly in Python.
+A simple, reverse-engineered SDK for Tastytrade built on their (now mostly public) API. This will allow you to create trading algorithms for whatever strategies you may have quickly and painlessly in Python.
 
 Installation
 ------------
 
 .. code-block:: bash
 
    $ pip install tastytrade
```

### Comparing `tastytrade-5.2/tastytrade.egg-info/SOURCES.txt` & `tastytrade-5.3/tastytrade.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 tastytrade/dxfeed/candle.py
 tastytrade/dxfeed/event.py
 tastytrade/dxfeed/greeks.py
 tastytrade/dxfeed/profile.py
 tastytrade/dxfeed/quote.py
 tastytrade/dxfeed/summary.py
 tastytrade/dxfeed/theoprice.py
+tastytrade/dxfeed/timeandsale.py
 tastytrade/dxfeed/trade.py
```

