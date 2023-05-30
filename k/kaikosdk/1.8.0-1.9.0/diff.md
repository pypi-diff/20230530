# Comparing `tmp/kaikosdk-1.8.0.tar.gz` & `tmp/kaikosdk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaikosdk-1.8.0.tar", last modified: Fri Apr 21 12:40:12 2023, max compression
+gzip compressed data, was "kaikosdk-1.9.0.tar", last modified: Tue May 30 15:19:01 2023, max compression
```

## Comparing `kaikosdk-1.8.0.tar` & `kaikosdk-1.9.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.312984 kaikosdk-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-21 12:40:12.312984 kaikosdk-1.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.300984 kaikosdk-1.8.0/kaikosdk/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.304984 kaikosdk-1.8.0/kaikosdk/core/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/data_interval_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/data_interval_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/instrument_criteria_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/instrument_criteria_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/sort_criteria_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/sort_criteria_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/source_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/source_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/wrappers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/wrappers_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/sdk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29534 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/sdk_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.304984 kaikosdk-1.8.0/kaikosdk/stream/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.304984 kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.304984 kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.304984 kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.304984 kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.308984 kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.308984 kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.308984 kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.308984 kaikosdk-1.8.0/kaikosdk/stream/index_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/commodity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/commodity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.312984 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/commodity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/commodity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.312984 kaikosdk-1.8.0/kaikosdk/stream/trades_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/trades_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/trades_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/trades_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/trades_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/trades_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.300984 kaikosdk-1.8.0/kaikosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-21 12:40:12.000000 kaikosdk-1.8.0/kaikosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-21 12:40:12.000000 kaikosdk-1.8.0/kaikosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:40:12.000000 kaikosdk-1.8.0/kaikosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:40:12.000000 kaikosdk-1.8.0/kaikosdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 12:40:12.000000 kaikosdk-1.8.0/kaikosdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:40:12.312984 kaikosdk-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-21 12:40:05.000000 kaikosdk-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.054261 kaikosdk-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 15:19:01.054261 kaikosdk-1.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.042261 kaikosdk-1.9.0/kaikosdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.046261 kaikosdk-1.9.0/kaikosdk/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/core/data_interval_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/core/data_interval_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/core/instrument_criteria_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/core/instrument_criteria_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/core/sort_criteria_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/core/sort_criteria_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/core/source_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/core/source_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/core/source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/core/source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/core/wrappers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/core/wrappers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/sdk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29534 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/sdk_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.046261 kaikosdk-1.9.0/kaikosdk/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.046261 kaikosdk-1.9.0/kaikosdk/stream/aggregated_price_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregated_price_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregated_price_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregated_price_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregated_price_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregated_price_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.046261 kaikosdk-1.9.0/kaikosdk/stream/aggregated_quote_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregated_quote_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregated_quote_v2/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregated_quote_v2/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregated_quote_v2/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregated_quote_v2/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.046261 kaikosdk-1.9.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.050261 kaikosdk-1.9.0/kaikosdk/stream/aggregates_ohlcv_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_ohlcv_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.050261 kaikosdk-1.9.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.050261 kaikosdk-1.9.0/kaikosdk/stream/aggregates_vwap_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_vwap_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_vwap_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_vwap_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_vwap_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/aggregates_vwap_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.050261 kaikosdk-1.9.0/kaikosdk/stream/index_multi_assets_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/index_multi_assets_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/index_multi_assets_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/index_multi_assets_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/index_multi_assets_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/index_multi_assets_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.050261 kaikosdk-1.9.0/kaikosdk/stream/index_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/index_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/index_v1/commodity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/index_v1/commodity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/index_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/index_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/index_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/index_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.054261 kaikosdk-1.9.0/kaikosdk/stream/market_update_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/market_update_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/market_update_v1/commodity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/market_update_v1/commodity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/market_update_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/market_update_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/market_update_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/market_update_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.054261 kaikosdk-1.9.0/kaikosdk/stream/trades_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/trades_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/trades_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/trades_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/trades_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 15:18:52.000000 kaikosdk-1.9.0/kaikosdk/stream/trades_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:19:01.042261 kaikosdk-1.9.0/kaikosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 15:19:01.000000 kaikosdk-1.9.0/kaikosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-30 15:19:01.000000 kaikosdk-1.9.0/kaikosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:19:01.000000 kaikosdk-1.9.0/kaikosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:19:00.000000 kaikosdk-1.9.0/kaikosdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 15:19:01.000000 kaikosdk-1.9.0/kaikosdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:19:01.054261 kaikosdk-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-30 15:18:54.000000 kaikosdk-1.9.0/setup.py
```

### Comparing `kaikosdk-1.8.0/kaikosdk/core/data_interval_pb2.py` & `kaikosdk-1.9.0/kaikosdk/core/data_interval_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/core/instrument_criteria_pb2.py` & `kaikosdk-1.9.0/kaikosdk/core/instrument_criteria_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/core/sort_criteria_pb2.py` & `kaikosdk-1.9.0/kaikosdk/core/sort_criteria_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/core/source_data_pb2.py` & `kaikosdk-1.9.0/kaikosdk/core/source_data_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/core/source_pb2.py` & `kaikosdk-1.9.0/kaikosdk/core/source_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/core/wrappers_pb2.py` & `kaikosdk-1.9.0/kaikosdk/core/wrappers_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/sdk_pb2.py` & `kaikosdk-1.9.0/kaikosdk/sdk_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/sdk_pb2_grpc.py` & `kaikosdk-1.9.0/kaikosdk/sdk_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/request_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/aggregated_price_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/response_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/aggregated_price_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/request_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/aggregated_quote_v2/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/response_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/aggregated_quote_v2/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/request_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/aggregates_vwap_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/response_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/aggregates_vwap_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/request_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/index_multi_assets_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/response_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/index_multi_assets_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/index_v1/commodity_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/index_v1/commodity_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/index_v1/request_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/index_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/index_v1/response_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/index_v1/response_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from kaikosdk.core import data_interval_pb2 as sdk_dot_core_dot_data__interval__pb2
 from kaikosdk.stream.index_v1 import commodity_pb2 as sdk_dot_stream_dot_index__v1_dot_commodity__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"sdk/stream/index_v1/response.proto\x12\x08kaikosdk\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1csdk/core/data_interval.proto\x1a#sdk/stream/index_v1/commodity.proto\"\x83\x01\n$StreamIndexServiceResponsePercentage\x12\x12\n\npercentage\x18\x01 \x01(\x01\x12\r\n\x05price\x18\x02 \x01(\x01\x12\x38\n\x05pairs\x18\x03 \x03(\x0b\x32).kaikosdk.StreamIndexServiceResponsePairs\"\x85\x01\n\x1fStreamIndexServiceResponsePairs\x12\x0c\n\x04pair\x18\x01 \x01(\t\x12\x0e\n\x06weight\x18\x02 \x01(\x01\x12\x44\n\x0binstruments\x18\x03 \x03(\x0b\x32/.kaikosdk.StreamIndexServiceResponseInstruments\"X\n%StreamIndexServiceResponseInstruments\x12\x10\n\x08\x65xchange\x18\x01 \x01(\t\x12\r\n\x05price\x18\x02 \x01(\x01\x12\x0e\n\x06volume\x18\x03 \x01(\x01\"D\n#StreamIndexServiceResponseBaseAsset\x12\r\n\x05\x61sset\x18\x01 \x01(\t\x12\x0e\n\x06weight\x18\x02 \x01(\x01\"\xe2\x02\n\x1cStreamIndexServiceResponseV1\x12\x12\n\nindex_code\x18\x01 \x01(\t\x12\x31\n\tcommodity\x18\x02 \x01(\x0e\x32\x1e.kaikosdk.StreamIndexCommodity\x12(\n\x08interval\x18\x03 \x01(\x0b\x32\x16.kaikosdk.DataInterval\x12\r\n\x05quote\x18\x04 \x01(\t\x12<\n\x05\x62\x61ses\x18\x05 \x03(\x0b\x32-.kaikosdk.StreamIndexServiceResponseBaseAsset\x12\x11\n\texchanges\x18\x06 \x03(\t\x12\x43\n\x0bpercentages\x18\x07 \x03(\x0b\x32..kaikosdk.StreamIndexServiceResponsePercentage\x12,\n\x08ts_event\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampBw\n\x1d\x63om.kaiko.sdk.stream.index_v1P\x01Z:github.com/kaikodata/kaiko-go-sdk/stream/index_v1;index_v1\xaa\x02\x17KaikoSdk.Stream.IndexV1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"sdk/stream/index_v1/response.proto\x12\x08kaikosdk\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1csdk/core/data_interval.proto\x1a#sdk/stream/index_v1/commodity.proto\"\x83\x01\n$StreamIndexServiceResponsePercentage\x12\x12\n\npercentage\x18\x01 \x01(\x01\x12\r\n\x05price\x18\x02 \x01(\x01\x12\x38\n\x05pairs\x18\x03 \x03(\x0b\x32).kaikosdk.StreamIndexServiceResponsePairs\"\x85\x01\n\x1fStreamIndexServiceResponsePairs\x12\x0c\n\x04pair\x18\x01 \x01(\t\x12\x0e\n\x06weight\x18\x02 \x01(\x01\x12\x44\n\x0binstruments\x18\x03 \x03(\x0b\x32/.kaikosdk.StreamIndexServiceResponseInstruments\"g\n%StreamIndexServiceResponseInstruments\x12\x10\n\x08\x65xchange\x18\x01 \x01(\t\x12\r\n\x05price\x18\x02 \x01(\x01\x12\x0e\n\x06volume\x18\x03 \x01(\x01\x12\r\n\x05\x63ount\x18\x04 \x01(\x04\"D\n#StreamIndexServiceResponseBaseAsset\x12\r\n\x05\x61sset\x18\x01 \x01(\t\x12\x0e\n\x06weight\x18\x02 \x01(\x01\"\xe2\x02\n\x1cStreamIndexServiceResponseV1\x12\x12\n\nindex_code\x18\x01 \x01(\t\x12\x31\n\tcommodity\x18\x02 \x01(\x0e\x32\x1e.kaikosdk.StreamIndexCommodity\x12(\n\x08interval\x18\x03 \x01(\x0b\x32\x16.kaikosdk.DataInterval\x12\r\n\x05quote\x18\x04 \x01(\t\x12<\n\x05\x62\x61ses\x18\x05 \x03(\x0b\x32-.kaikosdk.StreamIndexServiceResponseBaseAsset\x12\x11\n\texchanges\x18\x06 \x03(\t\x12\x43\n\x0bpercentages\x18\x07 \x03(\x0b\x32..kaikosdk.StreamIndexServiceResponsePercentage\x12,\n\x08ts_event\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampBw\n\x1d\x63om.kaiko.sdk.stream.index_v1P\x01Z:github.com/kaikodata/kaiko-go-sdk/stream/index_v1;index_v1\xaa\x02\x17KaikoSdk.Stream.IndexV1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sdk.stream.index_v1.response_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\035com.kaiko.sdk.stream.index_v1P\001Z:github.com/kaikodata/kaiko-go-sdk/stream/index_v1;index_v1\252\002\027KaikoSdk.Stream.IndexV1'
   _STREAMINDEXSERVICERESPONSEPERCENTAGE._serialized_start=149
   _STREAMINDEXSERVICERESPONSEPERCENTAGE._serialized_end=280
   _STREAMINDEXSERVICERESPONSEPAIRS._serialized_start=283
   _STREAMINDEXSERVICERESPONSEPAIRS._serialized_end=416
   _STREAMINDEXSERVICERESPONSEINSTRUMENTS._serialized_start=418
-  _STREAMINDEXSERVICERESPONSEINSTRUMENTS._serialized_end=506
-  _STREAMINDEXSERVICERESPONSEBASEASSET._serialized_start=508
-  _STREAMINDEXSERVICERESPONSEBASEASSET._serialized_end=576
-  _STREAMINDEXSERVICERESPONSEV1._serialized_start=579
-  _STREAMINDEXSERVICERESPONSEV1._serialized_end=933
+  _STREAMINDEXSERVICERESPONSEINSTRUMENTS._serialized_end=521
+  _STREAMINDEXSERVICERESPONSEBASEASSET._serialized_start=523
+  _STREAMINDEXSERVICERESPONSEBASEASSET._serialized_end=591
+  _STREAMINDEXSERVICERESPONSEV1._serialized_start=594
+  _STREAMINDEXSERVICERESPONSEV1._serialized_end=948
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/commodity_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/market_update_v1/commodity_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/request_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/market_update_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/response_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/market_update_v1/response_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from kaikosdk.core import wrappers_pb2 as sdk_dot_core_dot_wrappers__pb2
 from kaikosdk.stream.market_update_v1 import commodity_pb2 as sdk_dot_stream_dot_market__update__v1_dot_commodity__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*sdk/stream/market_update_v1/response.proto\x12\x08kaikosdk\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17sdk/core/wrappers.proto\x1a+sdk/stream/market_update_v1/commodity.proto\"\xd2\x06\n\x1cStreamMarketUpdateResponseV1\x12\x38\n\tcommodity\x18\x01 \x01(\x0e\x32%.kaikosdk.StreamMarketUpdateCommodity\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x01\x12\r\n\x05\x63lass\x18\x03 \x01(\t\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\x12\x10\n\x08\x65xchange\x18\x05 \x01(\t\x12\x13\n\x0bsequence_id\x18\x06 \x01(\t\x12\n\n\x02id\x18\x07 \x01(\t\x12\r\n\x05price\x18\x08 \x01(\x01\x12-\n\x0bts_exchange\x18\t \x01(\x0b\x32\x18.kaikosdk.TimestampValue\x12/\n\rts_collection\x18\n \x01(\x0b\x32\x18.kaikosdk.TimestampValue\x12,\n\x08ts_event\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12R\n\x0bupdate_type\x18\x0c \x01(\x0e\x32=.kaikosdk.StreamMarketUpdateResponseV1.StreamMarketUpdateType\x12\x41\n\x08snapshot\x18\r \x01(\x0b\x32/.kaikosdk.StreamMarketUpdateResponseV1.Snapshot\x1a\xbc\x01\n\x08Snapshot\x12\x43\n\x04\x61sks\x18\x01 \x03(\x0b\x32\x35.kaikosdk.StreamMarketUpdateResponseV1.Snapshot.Order\x12\x43\n\x04\x62ids\x18\x02 \x03(\x0b\x32\x35.kaikosdk.StreamMarketUpdateResponseV1.Snapshot.Order\x1a&\n\x05Order\x12\x0e\n\x06\x61mount\x18\x01 \x01(\x01\x12\r\n\x05price\x18\x02 \x01(\x01\"\xa4\x01\n\x16StreamMarketUpdateType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\r\n\tTRADE_BUY\x10\x01\x12\x0e\n\nTRADE_SELL\x10\x02\x12\x0c\n\x08\x42\x45ST_ASK\x10\x03\x12\x0c\n\x08\x42\x45ST_BID\x10\x04\x12\x0f\n\x0bUPDATED_ASK\x10\x05\x12\x0f\n\x0bUPDATED_BID\x10\x06\x12\x0c\n\x08SNAPSHOT\x10\x07\x12\x12\n\x0e\x46ORCE_SNAPSHOT\x10\x08\x42\x96\x01\n%com.kaiko.sdk.stream.market_update_v1P\x01ZJgithub.com/kaikodata/kaiko-go-sdk/stream/market_update_v1;market_update_v1\xaa\x02\x1eKaikoSdk.Stream.MarketUpdateV1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*sdk/stream/market_update_v1/response.proto\x12\x08kaikosdk\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17sdk/core/wrappers.proto\x1a+sdk/stream/market_update_v1/commodity.proto\"\xe5\x06\n\x1cStreamMarketUpdateResponseV1\x12\x38\n\tcommodity\x18\x01 \x01(\x0e\x32%.kaikosdk.StreamMarketUpdateCommodity\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x01\x12\r\n\x05\x63lass\x18\x03 \x01(\t\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\x12\x10\n\x08\x65xchange\x18\x05 \x01(\t\x12\x13\n\x0bsequence_id\x18\x06 \x01(\t\x12\n\n\x02id\x18\x07 \x01(\t\x12\r\n\x05price\x18\x08 \x01(\x01\x12-\n\x0bts_exchange\x18\t \x01(\x0b\x32\x18.kaikosdk.TimestampValue\x12/\n\rts_collection\x18\n \x01(\x0b\x32\x18.kaikosdk.TimestampValue\x12,\n\x08ts_event\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12R\n\x0bupdate_type\x18\x0c \x01(\x0e\x32=.kaikosdk.StreamMarketUpdateResponseV1.StreamMarketUpdateType\x12\x41\n\x08snapshot\x18\r \x01(\x0b\x32/.kaikosdk.StreamMarketUpdateResponseV1.Snapshot\x1a\xbc\x01\n\x08Snapshot\x12\x43\n\x04\x61sks\x18\x01 \x03(\x0b\x32\x35.kaikosdk.StreamMarketUpdateResponseV1.Snapshot.Order\x12\x43\n\x04\x62ids\x18\x02 \x03(\x0b\x32\x35.kaikosdk.StreamMarketUpdateResponseV1.Snapshot.Order\x1a&\n\x05Order\x12\x0e\n\x06\x61mount\x18\x01 \x01(\x01\x12\r\n\x05price\x18\x02 \x01(\x01\"\xb7\x01\n\x16StreamMarketUpdateType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\r\n\tTRADE_BUY\x10\x01\x12\x0e\n\nTRADE_SELL\x10\x02\x12\x11\n\rTRADE_UNKNOWN\x10\t\x12\x0c\n\x08\x42\x45ST_ASK\x10\x03\x12\x0c\n\x08\x42\x45ST_BID\x10\x04\x12\x0f\n\x0bUPDATED_ASK\x10\x05\x12\x0f\n\x0bUPDATED_BID\x10\x06\x12\x0c\n\x08SNAPSHOT\x10\x07\x12\x12\n\x0e\x46ORCE_SNAPSHOT\x10\x08\x42\x96\x01\n%com.kaiko.sdk.stream.market_update_v1P\x01ZJgithub.com/kaikodata/kaiko-go-sdk/stream/market_update_v1;market_update_v1\xaa\x02\x1eKaikoSdk.Stream.MarketUpdateV1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sdk.stream.market_update_v1.response_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n%com.kaiko.sdk.stream.market_update_v1P\001ZJgithub.com/kaikodata/kaiko-go-sdk/stream/market_update_v1;market_update_v1\252\002\036KaikoSdk.Stream.MarketUpdateV1'
   _STREAMMARKETUPDATERESPONSEV1._serialized_start=160
-  _STREAMMARKETUPDATERESPONSEV1._serialized_end=1010
+  _STREAMMARKETUPDATERESPONSEV1._serialized_end=1029
   _STREAMMARKETUPDATERESPONSEV1_SNAPSHOT._serialized_start=655
   _STREAMMARKETUPDATERESPONSEV1_SNAPSHOT._serialized_end=843
   _STREAMMARKETUPDATERESPONSEV1_SNAPSHOT_ORDER._serialized_start=805
   _STREAMMARKETUPDATERESPONSEV1_SNAPSHOT_ORDER._serialized_end=843
   _STREAMMARKETUPDATERESPONSEV1_STREAMMARKETUPDATETYPE._serialized_start=846
-  _STREAMMARKETUPDATERESPONSEV1_STREAMMARKETUPDATETYPE._serialized_end=1010
+  _STREAMMARKETUPDATERESPONSEV1_STREAMMARKETUPDATETYPE._serialized_end=1029
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/trades_v1/request_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/trades_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk/stream/trades_v1/response_pb2.py` & `kaikosdk-1.9.0/kaikosdk/stream/trades_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.8.0/kaikosdk.egg-info/SOURCES.txt` & `kaikosdk-1.9.0/kaikosdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

