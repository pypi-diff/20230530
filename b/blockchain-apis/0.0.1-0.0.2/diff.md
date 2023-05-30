# Comparing `tmp/blockchain-apis-0.0.1.tar.gz` & `tmp/blockchain-apis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockchain-apis-0.0.1.tar", last modified: Tue May 30 21:09:30 2023, max compression
+gzip compressed data, was "blockchain-apis-0.0.2.tar", last modified: Tue May 30 21:20:17 2023, max compression
```

## Comparing `blockchain-apis-0.0.1.tar` & `blockchain-apis-0.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:09:30.213128 blockchain-apis-0.0.1/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1095 2023-05-30 13:02:28.000000 blockchain-apis-0.0.1/LICENSE
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4609 2023-05-30 21:09:30.213128 blockchain-apis-0.0.1/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3057 2023-05-30 21:09:17.000000 blockchain-apis-0.0.1/README.md
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:09:30.209128 blockchain-apis-0.0.1/blockchain_apis/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    24780 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/BlockchainAPIs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    24174 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/BlockchainAPIsSync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       29 2023-05-30 15:57:13.000000 blockchain-apis-0.0.1/blockchain_apis/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:09:30.209128 blockchain-apis-0.0.1/blockchain_apis/blockchain_apis.egg-info/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4609 2023-05-30 21:09:30.000000 blockchain-apis-0.0.1/blockchain_apis/blockchain_apis.egg-info/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1708 2023-05-30 21:09:30.000000 blockchain-apis-0.0.1/blockchain_apis/blockchain_apis.egg-info/SOURCES.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-05-30 21:09:30.000000 blockchain-apis-0.0.1/blockchain_apis/blockchain_apis.egg-info/dependency_links.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       17 2023-05-30 21:09:30.000000 blockchain-apis-0.0.1/blockchain_apis/blockchain_apis.egg-info/requires.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       61 2023-05-30 21:09:30.000000 blockchain-apis-0.0.1/blockchain_apis/blockchain_apis.egg-info/top_level.txt
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:09:30.209128 blockchain-apis-0.0.1/blockchain_apis/exceptions/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      454 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/exceptions/BlockchainAPIsException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      717 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/exceptions/BlockchainNotSupportedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      710 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/exceptions/ExchangeNotSupportedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      807 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/exceptions/InvalidPageException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      830 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/exceptions/PairNotFoundException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      809 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/exceptions/TokenNotFoundException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      743 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/exceptions/TooManyRequestException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      727 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/exceptions/UnauthorizedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       45 2023-05-30 15:57:38.000000 blockchain-apis-0.0.1/blockchain_apis/exceptions/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:09:30.213128 blockchain-apis-0.0.1/blockchain_apis/models/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      860 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/models/AmountIn.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      871 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/models/AmountOut.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      580 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/models/Blockchain.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      548 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/models/Exchange.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      878 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/models/Exchanges.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      678 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/models/Pair.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      944 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/models/Pairs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      795 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/models/Reserve.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      761 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/models/Token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1838 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/blockchain_apis/models/Tokens.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       42 2023-05-30 15:57:25.000000 blockchain-apis-0.0.1/blockchain_apis/models/__init__.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       38 2023-05-30 21:09:30.213128 blockchain-apis-0.0.1/setup.cfg
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1923 2023-05-30 20:49:20.000000 blockchain-apis-0.0.1/setup.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:09:30.213128 blockchain-apis-0.0.1/tests/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1565 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_amount_in.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1541 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_amount_in_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1569 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_amount_out.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1545 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_amount_out_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      426 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_blockchains.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      420 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_blockchains_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      602 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_decimals.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      596 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_decimals_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1292 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_exchanges.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1232 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_exchanges_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      594 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_info.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      588 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_info_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2700 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_pairs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2568 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_pairs_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1393 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_reserves.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1369 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_reserves_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1250 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_tokens.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1190 2023-05-30 12:37:51.000000 blockchain-apis-0.0.1/tests/test_tokens_sync.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:20:17.790270 blockchain-apis-0.0.2/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1095 2023-05-30 13:02:28.000000 blockchain-apis-0.0.2/LICENSE
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4725 2023-05-30 21:20:17.790270 blockchain-apis-0.0.2/PKG-INFO
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3173 2023-05-30 21:17:27.000000 blockchain-apis-0.0.2/README.md
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:20:17.782270 blockchain-apis-0.0.2/blockchain_apis/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    24803 2023-05-30 21:18:49.000000 blockchain-apis-0.0.2/blockchain_apis/BlockchainAPIs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    24232 2023-05-30 21:19:58.000000 blockchain-apis-0.0.2/blockchain_apis/BlockchainAPIsSync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       29 2023-05-30 15:57:13.000000 blockchain-apis-0.0.2/blockchain_apis/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:20:17.782270 blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4725 2023-05-30 21:20:17.000000 blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/PKG-INFO
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1708 2023-05-30 21:20:17.000000 blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/SOURCES.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-05-30 21:20:17.000000 blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/dependency_links.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       17 2023-05-30 21:20:17.000000 blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/requires.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       61 2023-05-30 21:20:17.000000 blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/top_level.txt
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:20:17.786270 blockchain-apis-0.0.2/blockchain_apis/exceptions/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      454 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/BlockchainAPIsException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      717 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/BlockchainNotSupportedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      710 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/ExchangeNotSupportedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      807 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/InvalidPageException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      830 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/PairNotFoundException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      809 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/TokenNotFoundException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      743 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/TooManyRequestException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      727 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/UnauthorizedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       45 2023-05-30 15:57:38.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:20:17.786270 blockchain-apis-0.0.2/blockchain_apis/models/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      860 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/AmountIn.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      871 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/AmountOut.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      580 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Blockchain.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      548 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Exchange.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      878 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Exchanges.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      678 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Pair.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      944 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Pairs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      795 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Reserve.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      761 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Token.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1838 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Tokens.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       42 2023-05-30 15:57:25.000000 blockchain-apis-0.0.2/blockchain_apis/models/__init__.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       38 2023-05-30 21:20:17.790270 blockchain-apis-0.0.2/setup.cfg
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1923 2023-05-30 21:12:34.000000 blockchain-apis-0.0.2/setup.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:20:17.790270 blockchain-apis-0.0.2/tests/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1565 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_amount_in.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1541 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_amount_in_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1569 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_amount_out.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1545 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_amount_out_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      426 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_blockchains.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      420 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_blockchains_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      602 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_decimals.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      596 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_decimals_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1292 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_exchanges.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1232 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_exchanges_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      594 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_info.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      588 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_info_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2700 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_pairs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2568 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_pairs_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1393 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_reserves.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1369 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_reserves_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1250 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_tokens.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1190 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_tokens_sync.py
```

### Comparing `blockchain-apis-0.0.1/LICENSE` & `blockchain-apis-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/PKG-INFO` & `blockchain-apis-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockchain-apis
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fastest and easiest way to access decentralized finance data
 Home-page: https://www.blockchainapis.io
 Author: Clarensia
 Author-email: contact@blockchainapis.io
 License: MIT
 Project-URL: Documentation, https://api.blockchainapis.io/docs
 Project-URL: Source, https://github.com/blockchainapis/blockchain-apis-python-client
@@ -36,26 +36,27 @@
 ## Introduction
 
 The fastest and easiest way to interact with DeFi.
 
 With this SDK you can:
 - Get the price of any pair across all marketplaces in one API call
 - Get the current reserves of any pair
-- Same code to gather data from many blockchain and exchanges
+- Use the same code to gather data from many blockchains and exchanges
 
-Since DeFi is volatile and fast moving, so you need an SDK that is high performant. Here are the capabilities of **Blockchain APIs**:
-- Make async API calls for 1000+ requests per second
+Since DeFi is volatile and fast moving space, you need an SDK that is highly performant. Here are the capabilities of **Blockchain APIs**:
+- Make async API calls for more than 1000 requests per second
 - Processing time 20 times faster than the blockchain
 
 Examples of project that you can make with **Blockchain APIs**:
 - Arbitrage trading bot
 - Aggregator
 - Application to track cryptocurrency prices
 
 To get any help, feel free to join [our discord](https://discord.gg/GphRMJXmS5)
+Documentation link: [https://api.blockchainapis.io/docs](https://api.blockchainapis.io/docs)
 
 ## Quickstart
 
 ### Install the package
 
 `pip install blockchain-apis`
```

### Comparing `blockchain-apis-0.0.1/README.md` & `blockchain-apis-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 ## Introduction
 
 The fastest and easiest way to interact with DeFi.
 
 With this SDK you can:
 - Get the price of any pair across all marketplaces in one API call
 - Get the current reserves of any pair
-- Same code to gather data from many blockchain and exchanges
+- Use the same code to gather data from many blockchains and exchanges
 
-Since DeFi is volatile and fast moving, so you need an SDK that is high performant. Here are the capabilities of **Blockchain APIs**:
-- Make async API calls for 1000+ requests per second
+Since DeFi is volatile and fast moving space, you need an SDK that is highly performant. Here are the capabilities of **Blockchain APIs**:
+- Make async API calls for more than 1000 requests per second
 - Processing time 20 times faster than the blockchain
 
 Examples of project that you can make with **Blockchain APIs**:
 - Arbitrage trading bot
 - Aggregator
 - Application to track cryptocurrency prices
 
 To get any help, feel free to join [our discord](https://discord.gg/GphRMJXmS5)
+Documentation link: [https://api.blockchainapis.io/docs](https://api.blockchainapis.io/docs)
 
 ## Quickstart
 
 ### Install the package
 
 `pip install blockchain-apis`
```

### Comparing `blockchain-apis-0.0.1/blockchain_apis/BlockchainAPIs.py` & `blockchain-apis-0.0.2/blockchain_apis/BlockchainAPIs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,22 +23,27 @@
 
 
 
 class BlockchainAPIs:
     """High-frequency DEX API
 
         
-    Our API empowers you to access live financial data across multiple blockchains (currently supporting 6, with more on the way) with unparalleled speed and efficiency.
+    Our API empowers you to access live financial data across multiple blockchains (currently supporting 6, with more on the way)
+    with unparalleled speed and efficiency.
     
-    What sets our API apart? We've optimized performance to deliver an impressive 1000+ calls per second per user, with a lightning-fast processing time of less than 2 millisecond per request. Compare that to other solutions with a 20-millisecond processing time and fewer requests per second, and it's clear why developers choose our API for their trading bots.
+    What sets our API apart? We've optimized performance to deliver an impressive 1000+ calls per second per user, with a
+    lightning-fast processing time of less than 2 millisecond per request. Compare that to other solutions with a 20-millisecond
+    processing time and fewer requests per second, and it's clear why developers choose our API for their trading bots.
     
-    Another game-changing feature is our seamless integration across various blockchains and protocols. With our API, you can reuse the same code without changing a single line, simplifying the development process and saving you valuable time.
+    Another game-changing feature is our seamless integration across various blockchains and protocols. With our API, you can reuse
+    the same code without changing a single line, simplifying the development process and saving you valuable time.
     
-    Ready to try it out? [Sign up for a free API key here](https://dashboard.blockchainapis.io) or start exploring the possibilities on this page. Need support or have questions? Join our [Discord community](https://discord.gg/GphRMJXmS5) where our team and fellow developers are eager to help you make the most of our powerful API.
-
+    Ready to try it out? [Sign up for a free API key here](https://dashboard.blockchainapis.io) or start exploring the possibilities
+    on this page. Need support or have questions? Join our [Discord community](https://discord.gg/GphRMJXmS5) where our team and
+    fellow developers are eager to help you make the most of our powerful API.
     """
 
     _session: ClientSession
     """The session that is used by async operation.
     
     This session must be closed at the end of your program or usage of the API.
```

### Comparing `blockchain-apis-0.0.1/blockchain_apis/BlockchainAPIsSync.py` & `blockchain-apis-0.0.2/blockchain_apis/BlockchainAPIsSync.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,30 @@
 from exceptions.UnauthorizedException import UnauthorizedException
 
 
 
 class BlockchainAPIsSync:
     """High-frequency DEX API
 
-        
-    Our API empowers you to access live financial data across multiple blockchains (currently supporting 6, with more on the way) with unparalleled speed and efficiency.
+    Our API empowers you to access live financial data across multiple blockchains (currently supporting 6, with more on the way)
+    with unparalleled speed and efficiency.
     
-    What sets our API apart? We've optimized performance to deliver an impressive 1000+ calls per second per user, with a lightning-fast processing time of less than 2 millisecond per request. Compare that to other solutions with a 20-millisecond processing time and fewer requests per second, and it's clear why developers choose our API for their trading bots.
+    What sets our API apart? We've optimized performance to deliver an impressive 1000+ calls per second per user, with a
+    lightning-fast processing time of less than 2 millisecond per request. Compare that to other solutions with a 20-millisecond
+    processing time and fewer requests per second, and it's clear why developers choose our API for their trading bots.
     
-    Another game-changing feature is our seamless integration across various blockchains and protocols. With our API, you can reuse the same code without changing a single line, simplifying the development process and saving you valuable time.
+    Another game-changing feature is our seamless integration across various blockchains and protocols. With our API, you can reuse
+    the same code without changing a single line, simplifying the development process and saving you valuable time.
     
-    Ready to try it out? [Sign up for a free API key here](https://dashboard.blockchainapis.io) or start exploring the possibilities on this page. Need support or have questions? Join our [Discord community](https://discord.gg/GphRMJXmS5) where our team and fellow developers are eager to help you make the most of our powerful API.
+    Ready to try it out? [Sign up for a free API key here](https://dashboard.blockchainapis.io) or start exploring the possibilities
+    on this page. Need support or have questions? Join our [Discord community](https://discord.gg/GphRMJXmS5) where our team and
+    fellow developers are eager to help you make the most of our powerful API.
 
-    Please note that this class is not async which is less optimized. To run more otpimized
-    requests, please use: BlockchainAPIs
+    Please note that this class is using sync which is less optimized. To run more otpimized requests and take advantage of
+    modern async Python, please use: BlockchainAPIs
     """
     
     def __init__(self, api_key: str | None = None):
         """Creates a BlockchainAPIsSync sync instance that allow you to make API calls
         in a synchronous way.
 
         The client works without an API key, but for better performance, we advise you
```

### Comparing `blockchain-apis-0.0.1/blockchain_apis/blockchain_apis.egg-info/PKG-INFO` & `blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockchain-apis
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fastest and easiest way to access decentralized finance data
 Home-page: https://www.blockchainapis.io
 Author: Clarensia
 Author-email: contact@blockchainapis.io
 License: MIT
 Project-URL: Documentation, https://api.blockchainapis.io/docs
 Project-URL: Source, https://github.com/blockchainapis/blockchain-apis-python-client
@@ -36,26 +36,27 @@
 ## Introduction
 
 The fastest and easiest way to interact with DeFi.
 
 With this SDK you can:
 - Get the price of any pair across all marketplaces in one API call
 - Get the current reserves of any pair
-- Same code to gather data from many blockchain and exchanges
+- Use the same code to gather data from many blockchains and exchanges
 
-Since DeFi is volatile and fast moving, so you need an SDK that is high performant. Here are the capabilities of **Blockchain APIs**:
-- Make async API calls for 1000+ requests per second
+Since DeFi is volatile and fast moving space, you need an SDK that is highly performant. Here are the capabilities of **Blockchain APIs**:
+- Make async API calls for more than 1000 requests per second
 - Processing time 20 times faster than the blockchain
 
 Examples of project that you can make with **Blockchain APIs**:
 - Arbitrage trading bot
 - Aggregator
 - Application to track cryptocurrency prices
 
 To get any help, feel free to join [our discord](https://discord.gg/GphRMJXmS5)
+Documentation link: [https://api.blockchainapis.io/docs](https://api.blockchainapis.io/docs)
 
 ## Quickstart
 
 ### Install the package
 
 `pip install blockchain-apis`
```

### Comparing `blockchain-apis-0.0.1/blockchain_apis/blockchain_apis.egg-info/SOURCES.txt` & `blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/exceptions/BlockchainNotSupportedException.py` & `blockchain-apis-0.0.2/blockchain_apis/exceptions/BlockchainNotSupportedException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/exceptions/ExchangeNotSupportedException.py` & `blockchain-apis-0.0.2/blockchain_apis/exceptions/ExchangeNotSupportedException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/exceptions/InvalidPageException.py` & `blockchain-apis-0.0.2/blockchain_apis/exceptions/InvalidPageException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/exceptions/PairNotFoundException.py` & `blockchain-apis-0.0.2/blockchain_apis/exceptions/PairNotFoundException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/exceptions/TokenNotFoundException.py` & `blockchain-apis-0.0.2/blockchain_apis/exceptions/TokenNotFoundException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/exceptions/TooManyRequestException.py` & `blockchain-apis-0.0.2/blockchain_apis/exceptions/TooManyRequestException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/exceptions/UnauthorizedException.py` & `blockchain-apis-0.0.2/blockchain_apis/exceptions/UnauthorizedException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/models/AmountIn.py` & `blockchain-apis-0.0.2/blockchain_apis/models/AmountIn.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/models/AmountOut.py` & `blockchain-apis-0.0.2/blockchain_apis/models/AmountOut.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/models/Blockchain.py` & `blockchain-apis-0.0.2/blockchain_apis/models/Blockchain.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/models/Exchange.py` & `blockchain-apis-0.0.2/blockchain_apis/models/Exchange.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/models/Exchanges.py` & `blockchain-apis-0.0.2/blockchain_apis/models/Exchanges.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/models/Pair.py` & `blockchain-apis-0.0.2/blockchain_apis/models/Pair.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/models/Pairs.py` & `blockchain-apis-0.0.2/blockchain_apis/models/Pairs.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/models/Reserve.py` & `blockchain-apis-0.0.2/blockchain_apis/models/Reserve.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/models/Token.py` & `blockchain-apis-0.0.2/blockchain_apis/models/Token.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/blockchain_apis/models/Tokens.py` & `blockchain-apis-0.0.2/blockchain_apis/models/Tokens.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/setup.py` & `blockchain-apis-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setuptools.setup(
     name = "blockchain-apis",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "Clarensia",
     author_email = "contact@blockchainapis.io",
     description = "Fastest and easiest way to access decentralized finance data",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://www.blockchainapis.io",
     license="MIT",
```

### Comparing `blockchain-apis-0.0.1/tests/test_amount_in.py` & `blockchain-apis-0.0.2/tests/test_amount_in.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_amount_in_sync.py` & `blockchain-apis-0.0.2/tests/test_amount_in_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_amount_out.py` & `blockchain-apis-0.0.2/tests/test_amount_out.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_amount_out_sync.py` & `blockchain-apis-0.0.2/tests/test_amount_out_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_decimals.py` & `blockchain-apis-0.0.2/tests/test_decimals.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_decimals_sync.py` & `blockchain-apis-0.0.2/tests/test_decimals_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_exchanges.py` & `blockchain-apis-0.0.2/tests/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_exchanges_sync.py` & `blockchain-apis-0.0.2/tests/test_exchanges_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_info.py` & `blockchain-apis-0.0.2/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_info_sync.py` & `blockchain-apis-0.0.2/tests/test_info_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_pairs.py` & `blockchain-apis-0.0.2/tests/test_pairs.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_pairs_sync.py` & `blockchain-apis-0.0.2/tests/test_pairs_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_reserves.py` & `blockchain-apis-0.0.2/tests/test_reserves.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_reserves_sync.py` & `blockchain-apis-0.0.2/tests/test_reserves_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_tokens.py` & `blockchain-apis-0.0.2/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.1/tests/test_tokens_sync.py` & `blockchain-apis-0.0.2/tests/test_tokens_sync.py`

 * *Files identical despite different names*

