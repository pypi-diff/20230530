# Comparing `tmp/defi-services-lib-1.0.3.tar.gz` & `tmp/defi-services-lib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defi-services-lib-1.0.3.tar", last modified: Mon May 29 16:00:23 2023, max compression
+gzip compressed data, was "defi-services-lib-1.0.4.tar", last modified: Tue May 30 10:53:18 2023, max compression
```

## Comparing `defi-services-lib-1.0.3.tar` & `defi-services-lib-1.0.4.tar`

### file list

```diff
@@ -1,82 +1,109 @@
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.566275 defi-services-lib-1.0.3/
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1129 2023-05-29 07:02:16.000000 defi-services-lib-1.0.3/LICENSE
--rw-r--r--   0 vietbangpham   (501) staff       (20)      840 2023-05-29 16:00:23.564403 defi-services-lib-1.0.3/PKG-INFO
--rw-r--r--   0 vietbangpham   (501) staff       (20)      259 2023-05-29 08:02:45.000000 defi-services-lib-1.0.3/README.md
--rw-r--r--   0 vietbangpham   (501) staff       (20)      107 2023-05-29 04:51:50.000000 defi-services-lib-1.0.3/pyproject.toml
--rw-r--r--   0 vietbangpham   (501) staff       (20)       38 2023-05-29 16:00:23.566732 defi-services-lib-1.0.3/setup.cfg
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1201 2023-05-29 07:52:03.000000 defi-services-lib-1.0.3/setup.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.492294 defi-services-lib-1.0.3/src/
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.499578 defi-services-lib-1.0.3/src/defi_services/
--rw-r--r--   0 vietbangpham   (501) staff       (20)       22 2023-05-29 16:00:12.000000 defi-services-lib-1.0.3/src/defi_services/__init__.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.501031 defi-services-lib-1.0.3/src/defi_services/abis/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:43:51.000000 defi-services-lib-1.0.3/src/defi_services/abis/__init__.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.504274 defi-services-lib-1.0.3/src/defi_services/abis/dex/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:44:57.000000 defi-services-lib-1.0.3/src/defi_services/abis/dex/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    15950 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/dex/biswap_masterchef_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    18798 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/dex/pancakeswap_masterchef_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     5636 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/erc20_abi.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.524535 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:05.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    16070 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/alpaca_fair_launch_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    23376 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/alpaca_vault_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    10050 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/alpaca_vault_config_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1418 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/chain_link_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    12726 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/chef_incentives_controller.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    43379 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/cream_comptroller_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    20100 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/cream_lens_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    23605 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/ctoken_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    29034 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/lending_pool_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4399 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/oracle_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    13482 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/staked_incentives_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    21266 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/trava_lending_pool_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4507 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/trava_oracle_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     9576 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/valas_multi_fee_distribution.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    43234 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/venus_comptroller_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    18613 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/venus_lens_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    14433 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/venus_lens_abi_v1.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.528050 defi-services-lib-1.0.3/src/defi_services/abis/vault/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:15.000000 defi-services-lib-1.0.3/src/defi_services/abis/vault/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    12332 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/vault/incentive_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    31318 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/vault/trava_vault_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      598 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/vault/valuator_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    38341 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/abis/vault/ve_abi.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.532245 defi-services-lib-1.0.3/src/defi_services/constants/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:24.000000 defi-services-lib-1.0.3/src/defi_services/constants/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      136 2023-05-29 15:14:03.000000 defi-services-lib-1.0.3/src/defi_services/constants/chain_constant.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1721 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/constants/contract_address.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2492 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/constants/db_constant.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      181 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/constants/time_constant.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      540 2023-05-29 15:14:03.000000 defi-services-lib-1.0.3/src/defi_services/defi_service.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.539315 defi-services-lib-1.0.3/src/defi_services/lending_pools/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2376 2023-05-29 15:35:08.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/cream_service.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.540958 defi-services-lib-1.0.3/src/defi_services/lending_pools/lending_pools_info/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/lending_pools_info/__init__.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.545359 defi-services-lib-1.0.3/src/defi_services/lending_pools/lending_pools_info/bsc/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/lending_pools_info/bsc/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     8268 2023-05-29 15:14:03.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/lending_pools_info/bsc/cream_bsc.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     5266 2023-05-29 15:14:03.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/lending_pools_info/bsc/trava_bsc.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4095 2023-05-29 15:14:03.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/lending_pools_info/bsc/valas_bsc.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     3907 2023-05-29 15:14:03.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/lending_pools_info/bsc/venus_bsc.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.552641 defi-services-lib-1.0.3/src/defi_services/lending_pools/services/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 14:38:12.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/services/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    18980 2023-05-29 15:14:03.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/services/cream_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    15406 2023-05-29 15:53:55.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/services/trava_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    14712 2023-05-29 15:59:21.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/services/valas_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    13289 2023-05-29 15:35:08.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/services/venus_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1803 2023-05-29 15:14:03.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/trava_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1781 2023-05-29 15:35:08.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/valas_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1948 2023-05-29 15:40:41.000000 defi-services-lib-1.0.3/src/defi_services/lending_pools/venus_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4229 2023-05-29 07:59:51.000000 defi-services-lib-1.0.3/src/defi_services/state_service.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.558356 defi-services-lib-1.0.3/src/defi_services/utils/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:50.000000 defi-services-lib-1.0.3/src/defi_services/utils/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1830 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/utils/batch_queries_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     6271 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/utils/graph_operations.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      723 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/utils/market_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      851 2023-05-29 03:52:33.000000 defi-services-lib-1.0.3/src/defi_services/utils/memory_storage.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-29 16:00:23.563449 defi-services-lib-1.0.3/src/defi_services_lib.egg-info/
--rw-r--r--   0 vietbangpham   (501) staff       (20)      840 2023-05-29 16:00:23.000000 defi-services-lib-1.0.3/src/defi_services_lib.egg-info/PKG-INFO
--rw-r--r--   0 vietbangpham   (501) staff       (20)     3227 2023-05-29 16:00:23.000000 defi-services-lib-1.0.3/src/defi_services_lib.egg-info/SOURCES.txt
--rw-r--r--   0 vietbangpham   (501) staff       (20)        1 2023-05-29 16:00:23.000000 defi-services-lib-1.0.3/src/defi_services_lib.egg-info/dependency_links.txt
--rw-r--r--   0 vietbangpham   (501) staff       (20)       34 2023-05-29 16:00:23.000000 defi-services-lib-1.0.3/src/defi_services_lib.egg-info/requires.txt
--rw-r--r--   0 vietbangpham   (501) staff       (20)       14 2023-05-29 16:00:23.000000 defi-services-lib-1.0.3/src/defi_services_lib.egg-info/top_level.txt
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.378684 defi-services-lib-1.0.4/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1129 2023-05-29 07:02:16.000000 defi-services-lib-1.0.4/LICENSE
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      840 2023-05-30 10:53:18.378090 defi-services-lib-1.0.4/PKG-INFO
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      259 2023-05-29 08:02:45.000000 defi-services-lib-1.0.4/README.md
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      107 2023-05-29 04:51:50.000000 defi-services-lib-1.0.4/pyproject.toml
+-rw-r--r--   0 vietbangpham   (501) staff       (20)       38 2023-05-30 10:53:18.378948 defi-services-lib-1.0.4/setup.cfg
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1201 2023-05-29 07:52:03.000000 defi-services-lib-1.0.4/setup.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.261790 defi-services-lib-1.0.4/src/
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.271426 defi-services-lib-1.0.4/src/defi_services/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)       22 2023-05-30 10:53:07.000000 defi-services-lib-1.0.4/src/defi_services/__init__.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.273982 defi-services-lib-1.0.4/src/defi_services/abis/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:43:51.000000 defi-services-lib-1.0.4/src/defi_services/abis/__init__.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.277706 defi-services-lib-1.0.4/src/defi_services/abis/dex/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:44:57.000000 defi-services-lib-1.0.4/src/defi_services/abis/dex/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    15950 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/dex/biswap_masterchef_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    18798 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/dex/pancakeswap_masterchef_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     5636 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/erc20_abi.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.304134 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:05.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    16070 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/alpaca_fair_launch_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    23376 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/alpaca_vault_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    10050 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/alpaca_vault_config_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1418 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/chain_link_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    12726 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/chef_incentives_controller.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    43379 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/cream_comptroller_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    20100 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/cream_lens_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    23605 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/ctoken_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    29034 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/lending_pool_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4399 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/oracle_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    13482 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/staked_incentives_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    21266 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/trava_lending_pool_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4507 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/trava_oracle_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     9576 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/valas_multi_fee_distribution.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    43234 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/venus_comptroller_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    18613 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/venus_lens_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    14433 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/venus_lens_abi_v1.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.309218 defi-services-lib-1.0.4/src/defi_services/abis/vault/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:15.000000 defi-services-lib-1.0.4/src/defi_services/abis/vault/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    12332 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/vault/incentive_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    31318 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/vault/trava_vault_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      598 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/vault/valuator_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    38341 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/vault/ve_abi.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.318266 defi-services-lib-1.0.4/src/defi_services/constants/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:24.000000 defi-services-lib-1.0.4/src/defi_services/constants/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      136 2023-05-29 15:14:03.000000 defi-services-lib-1.0.4/src/defi_services/constants/chain_constant.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1931 2023-05-30 10:36:00.000000 defi-services-lib-1.0.4/src/defi_services/constants/contract_address.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2492 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/constants/db_constant.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      792 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/constants/mapping_constant.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      181 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/constants/time_constant.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1105 2023-05-30 09:09:58.000000 defi-services-lib-1.0.4/src/defi_services/defi_service.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.332294 defi-services-lib-1.0.4/src/defi_services/lending_pools/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2418 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/aave_v2_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2175 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/compound_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2475 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/cream_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1953 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/geist_service.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.334113 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/__init__.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.336147 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/arbitrum/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/arbitrum/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2635 2023-05-30 09:15:50.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/arbitrum/radiant_arbitrum.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.345177 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     8425 2023-05-30 09:48:52.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/cream_bsc.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2325 2023-05-30 07:45:58.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/radiant_bsc.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     3757 2023-05-30 07:34:54.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/trava_bsc.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4095 2023-05-30 06:42:21.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/valas_bsc.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4743 2023-05-30 09:46:20.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/venus_bsc.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.350996 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/ethereum/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/ethereum/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    11944 2023-05-30 08:21:17.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/ethereum/aave_v2_eth.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     3674 2023-05-30 09:56:27.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/ethereum/compound_eth.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1565 2023-05-30 07:34:54.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/ethereum/trava_eth.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.354169 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/fantom/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/fantom/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     3257 2023-05-30 07:24:06.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/fantom/geist_ftm.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1808 2023-05-30 07:34:54.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/fantom/trava_ftm.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.355494 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/optimism/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/optimism/__init__.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.356970 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/polygon/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/polygon/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4448 2023-05-30 08:21:17.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/polygon/aave_v2_polygon.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2021 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/radiant_service.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.368425 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 14:38:12.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    13008 2023-05-30 08:59:53.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/aave_v2_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4418 2023-05-30 10:39:37.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/compound_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    20627 2023-05-30 10:36:00.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/cream_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      689 2023-05-30 07:24:06.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/geist_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1060 2023-05-30 09:13:38.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/radiant_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    17188 2023-05-30 08:51:45.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/trava_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    15441 2023-05-30 08:59:53.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/valas_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    14936 2023-05-30 10:36:00.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/venus_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2353 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/trava_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1947 2023-05-30 10:06:57.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/valas_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2047 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/venus_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4360 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/state_service.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.372959 defi-services-lib-1.0.4/src/defi_services/utils/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:50.000000 defi-services-lib-1.0.4/src/defi_services/utils/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1830 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/utils/batch_queries_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     6271 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/utils/graph_operations.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      723 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/utils/market_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      851 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/utils/memory_storage.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.377122 defi-services-lib-1.0.4/src/defi_services_lib.egg-info/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      840 2023-05-30 10:53:18.000000 defi-services-lib-1.0.4/src/defi_services_lib.egg-info/PKG-INFO
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4692 2023-05-30 10:53:18.000000 defi-services-lib-1.0.4/src/defi_services_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        1 2023-05-30 10:53:18.000000 defi-services-lib-1.0.4/src/defi_services_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 vietbangpham   (501) staff       (20)       34 2023-05-30 10:53:18.000000 defi-services-lib-1.0.4/src/defi_services_lib.egg-info/requires.txt
+-rw-r--r--   0 vietbangpham   (501) staff       (20)       14 2023-05-30 10:53:18.000000 defi-services-lib-1.0.4/src/defi_services_lib.egg-info/top_level.txt
```

### Comparing `defi-services-lib-1.0.3/LICENSE` & `defi-services-lib-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/PKG-INFO` & `defi-services-lib-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defi-services-lib
-Version: 1.0.3
+Version: 1.0.4
 Summary: Calculate apy, apr, and wallet information,... in decentralized applications.
 Home-page: https://github.com/phamvietbang/defi-services-lib
 Author: Viet-Bang Pham
 Author-email: phamvietbang2965@gmail.com
 Project-URL: Bug Tracker, https://github.com/phamvietbang/defi-services-lib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `defi-services-lib-1.0.3/setup.py` & `defi-services-lib-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/dex/biswap_masterchef_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/dex/biswap_masterchef_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/dex/pancakeswap_masterchef_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/dex/pancakeswap_masterchef_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/erc20_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/erc20_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/alpaca_fair_launch_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/alpaca_fair_launch_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/alpaca_vault_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/alpaca_vault_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/alpaca_vault_config_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/alpaca_vault_config_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/chain_link_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/chain_link_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/chef_incentives_controller.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/chef_incentives_controller.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/cream_comptroller_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/cream_comptroller_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/cream_lens_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/cream_lens_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/ctoken_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/ctoken_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/lending_pool_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/lending_pool_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/oracle_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/oracle_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/staked_incentives_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/staked_incentives_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/trava_lending_pool_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/trava_lending_pool_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/trava_oracle_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/trava_oracle_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/valas_multi_fee_distribution.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/valas_multi_fee_distribution.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/venus_comptroller_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/venus_comptroller_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/venus_lens_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/venus_lens_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/lending_pool/venus_lens_abi_v1.py` & `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/venus_lens_abi_v1.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/vault/incentive_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/vault/incentive_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/vault/trava_vault_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/vault/trava_vault_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/vault/valuator_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/vault/valuator_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/abis/vault/ve_abi.py` & `defi-services-lib-1.0.4/src/defi_services/abis/vault/ve_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/constants/contract_address.py` & `defi-services-lib-1.0.4/src/defi_services/constants/contract_address.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,19 @@
     # MAIN_STAKING_CONTRACT_PANCAKE_FARM = "0xa5f8c5dbd5f286960b9d90548680ae5ebff07652"
     LUNA = "0xb91A659E88B51474767CD97EF3196A3e7cEDD2c8"
     UST = "0x78366446547D062f45b4C0f320cDaa6d710D87bb"
     BISWAP_FARM = "0xdbc1a13490deef9c3c12b44fe77b503c1b061739"
 
 
 class WrappedNativeTokens:
-    mapping = {
-        "0x38": "0xbb4cdb9cbd36b01bd1cbaebf2de08d9173bc095c"
-    }
+    NATIVE_TOKEN = "0x0000000000000000000000000000000000000000"
+    WBNB = "0xbb4cdb9cbd36b01bd1cbaebf2de08d9173bc095c"
+    WETH = "0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2"
+    WMATIC = "0x0000000000000000000000000000000000001010"
+    WFANTOM = "0x21be370D5312f44cB42ce377BC9b8a0cEF1A4C83"
 
 
 class AbnormalVenusPool:
     venusDOGE = "0xec3422ef92b2fb59e84c8b02ba73f1fe84ed8d71"
     venusTRON = "0xc5d3466aa484b040ee977073fcf337f2c00071c1"
     decimals = {
         venusDOGE: 20,
```

### Comparing `defi-services-lib-1.0.3/src/defi_services/constants/db_constant.py` & `defi-services-lib-1.0.4/src/defi_services/constants/db_constant.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/lending_pools/cream_service.py` & `defi-services-lib-1.0.4/src/defi_services/lending_pools/cream_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from defi_services.constants.contract_address import ContractAddresses
 from defi_services.defi_service import DefiService
 from defi_services.lending_pools.lending_pools_info.bsc.cream_bsc import CREAM_BSC
 from defi_services.lending_pools.services.cream_state_service import CreamStateService
 
 
 class CreamService(DefiService):
+    name = "cream lending pool"
+
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
         self.state_service = CreamStateService(provider_uri)
         self.defi_constant = self._get_constant()
 
     def _get_constant(self):
         if self.chain_id == Chain.bsc:
@@ -44,9 +46,10 @@
 
     def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest", **kwargs):
         return self.state_service.get_wallet_deposit_borrow_balance(
             wallet_address=wallet_address,
             lens_address=self.defi_constant.get("lensAddress"),
             reserves_info=self.defi_constant.get("reservesList"),
             wrapped_native_token_price=float(kwargs.get("wrapped_native_token_price")),
-            block_number=block_number
+            block_number=block_number,
+            wrapped_native_token=self.get_wrapped_native_token()
         )
```

### Comparing `defi-services-lib-1.0.3/src/defi_services/lending_pools/lending_pools_info/bsc/cream_bsc.py` & `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/cream_bsc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,255 +1,194 @@
 CREAM_BSC = {
-  "_id": "0x38_0x589de0f0ccf905477646599bb3e5c622c84cc0ba",
-  "chainId": "0x38",
-  "createdAt": 1577836800,
-  "comptrollerAddress": "0x589de0f0ccf905477646599bb3e5c622c84cc0ba",
-  "comptrollerImplementationAddress": "0x49a08f9f445af5734cf15a1deab3b1c6a7988fb4",
-  "projectName": "Cream",
-  "name": "Cream Lending Pool",
-  "rewardToken": "0xd4cb328a82bdf5f03eb737f37fa6b370aef3e888",
-  "lensAddress": "0x1a014ffe0cd187a298a7e79ba5ab05538686ea4a",
-  "type": "LENDING_POOL",
-  "reservesList": {
-    "0x0000000000000000000000000000000000000000": {
-      "cToken": "0x1ffe17b99b439be0afc831239ddecda2a790ff3a",
-      "createdAt": 1598976307,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0x0d8ce2a99bb6e3b7db580ed848240e4a0f9ae153": {
-      "cToken": "0x1af8c1c3ad36a041cb6678fed86b1e095004fd16",
-      "createdAt": 1602924462,
-      "isNew": True,
-      "liquidationThreshold": 0.5,
-      "ltv": 0.45
-    },
-    "0x0e09fabb73bd3ade0a17ecc321fd13a19e81ce82": {
-      "cToken": "0xbf9b95b78bc42f6cf53ff2a0ce19d607cfe1ff82",
-      "createdAt": 1612934206,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0x0eb3a705fc54725037cc9e008bdede697f62f335": {
-      "cToken": "0x0e9d900c884964dc4b26db96ba113825b1a09baa",
-      "createdAt": 1603197921,
-      "isNew": True,
-      "liquidationThreshold": 0.5,
-      "ltv": 0.45
-    },
-    "0x101d82428437127bf1608f699cd651e6abf9766e": {
-      "cToken": "0x4cb7f1f4ad7a6b53802589af3b90612c1674fec4",
-      "createdAt": 1614064019,
-      "isNew": True,
-      "liquidationThreshold": 0,
-      "ltv": 0
-    },
-    "0x16939ef78684453bfdfb47825f8a5f714f12623a": {
-      "cToken": "0xe692714717a89e4f2ab89dd17d8dddd7bb52de8e",
-      "createdAt": 1602678330,
-      "isNew": True,
-      "liquidationThreshold": 0.5,
-      "ltv": 0.45
-    },
-    "0x1af3f329e8be154074d8769d1ffa4ee058b1dbc3": {
-      "cToken": "0x9095e8d707e40982affce41c61c10895157a1b22",
-      "createdAt": 1602505224,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0x1d2f0da169ceb9fc7b3144628db156f3f6c60dbe": {
-      "cToken": "0xaa46e2c21b7763a73db48e9b318899253e66e20c",
-      "createdAt": 1599817039,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0x2170ed0880ac9a755fd29b2688956bd959f933f8": {
-      "cToken": "0xb31f5d117541825d6692c10e4357008edf3e2bcd",
-      "createdAt": 1599830200,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0x250632378e573c6be1ac2f97fcdf00515d0aa91b": {
-      "cToken": "0xdcf60e349a5aaeeecdd2fb6772931fbf3486ed1c",
-      "createdAt": 1615963243,
-      "isNew": True,
-      "liquidationThreshold": 0.7,
-      "ltv": 0.65
-    },
-    "0x3ee2200efb3400fabb9aacf31297cbdd1d435d47": {
-      "cToken": "0x81c15d3e956e55e77e1f3f257f0a65bd2725fc55",
-      "createdAt": 1601531731,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0x4338665cbb7b2485a8855a139b75d5e34ab0db94": {
-      "cToken": "0x8cc7e2a6de999758499658bb702143fd025e09b2",
-      "createdAt": 1599830749,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0x47bead2563dcbf3bf2c9407fea4dc236faba485a": {
-      "cToken": "0xa8d75a0d17d2f4f2f4673975ab8470269d019c96",
-      "createdAt": 1615963495,
-      "isNew": True,
-      "liquidationThreshold": 0.5,
-      "ltv": 0.45
-    },
-    "0x4b0f1812e5df2a09796481ff14017e6005508003": {
-      "cToken": "0x2d3bfadf9bc94e3ab796029a030e863f1898aa06",
-      "createdAt": 1605079204,
-      "isNew": True,
-      "liquidationThreshold": 0.5,
-      "ltv": 0.45
-    },
-    "0x4bd17003473389a42daf6a0a729f6fdb328bbbd7": {
-      "cToken": "0x84902bd5ccef97648bf69c5096729a9367043beb",
-      "createdAt": 1614064361,
-      "isNew": True,
-      "liquidationThreshold": 0,
-      "ltv": 0
-    },
-    "0x55d398326f99059ff775485246999027b3197955": {
-      "cToken": "0xef6d459fe81c3ed53d292c936b2df5a8084975de",
-      "createdAt": 1599898687,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0x56b6fb708fc5732dec1afc8d8556423a2edccbd6": {
-      "cToken": "0x19ee64850862cfd234e20c0db4eda286f12ec907",
-      "createdAt": 1602069181,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0x695fd30af473f2960e81dc9ba7cb67679d35edb7": {
-      "cToken": "0xbe7e1d74acae787355169bc61a8729b2040fce6b",
-      "createdAt": 1614065402,
-      "isNew": True,
-      "liquidationThreshold": 0,
-      "ltv": 0
-    },
-    "0x7083609fce4d1d8dc0c979aab8c869ea2c873402": {
-      "cToken": "0x53d88d2ffdbe71e81d95b08ae0ca49d0c4a8515f",
-      "createdAt": 1600095877,
-      "isNew": True,
-      "liquidationThreshold": 0.5,
-      "ltv": 0.45
-    },
-    "0x7130d2a12b9bcbfae4f2634d864a1ee1ce3ead9c": {
-      "cToken": "0x11883cdea6bab720092791cc89affa54428ce069",
-      "createdAt": 1599060295,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0x88f1a5ae2a3bf98aeaf342d26b30a79438c9142e": {
-      "cToken": "0xea466cd2583a0290b9e7b987a769a7eb468fb0a5",
-      "createdAt": 1603019028,
-      "isNew": True,
-      "liquidationThreshold": 0.5,
-      "ltv": 0.45
-    },
-    "0x8ac76a51cc950d9822d68b83fe1ad97b32cd580d": {
-      "cToken": "0xd83c88db3a6ca4a32fff1603b0f7ddce01f5f727",
-      "createdAt": 1603292299,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0x8ff795a6f4d97e7887c79bea79aba5cc76444adf": {
-      "cToken": "0xcb87cee8c77cdfd310fb3c58ff72e688d46f90b1",
-      "createdAt": 1599829738,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0x947950bcc74888a40ffa2593c5798f11fc9124c4": {
-      "cToken": "0x9b53e7d5e3f6cc8694840ed6c9f7fee79e7bcee5",
-      "createdAt": 1616657496,
-      "isNew": True,
-      "liquidationThreshold": 0.65,
-      "ltv": 0.6
-    },
-    "0x9678e42cebeb63f23197d726b29b1cb20d0064e5": {
-      "cToken": "0xc17c8c5b8bb9456c624f8534fde6cbda2451488c",
-      "createdAt": 1615963405,
-      "isNew": True,
-      "liquidationThreshold": 0.4,
-      "ltv": 0.35
-    },
-    "0xa184088a740c695e156f91f5cc086a06bb78b827": {
-      "cToken": "0xf77df34f4bf632fb5ca928592a73a29a42bcf0b1",
-      "createdAt": 1614064607,
-      "isNew": True,
-      "liquidationThreshold": 0.25,
-      "ltv": 0.2
-    },
-    "0xa1faa113cbe53436df28ff0aee54275c13b40975": {
-      "cToken": "0x264bc4ea2f45cf6331ad6c3ac8d7257cf487fcbc",
-      "createdAt": 1605077446,
-      "isNew": True,
-      "liquidationThreshold": 0.5,
-      "ltv": 0.45
-    },
-    "0xad6caeb32cd2c308980a548bd0bc5aa4306c6c18": {
-      "cToken": "0x738f3810b3da0f3e6dc8c689d0d72f3b4992c43b",
-      "createdAt": 1601884423,
-      "isNew": True,
-      "liquidationThreshold": 0.5,
-      "ltv": 0.45
-    },
-    "0xbf5140a22578168fd562dccf235e5d43a02ce9b1": {
-      "cToken": "0x3b0be453a4008ebc2edd457e7bd355f1c5469d68",
-      "createdAt": 1603110204,
-      "isNew": True,
-      "liquidationThreshold": 0.65,
-      "ltv": 0.6
-    },
-    "0xcf6bb5389c92bdda8a3747ddb454cb7a64626c63": {
-      "cToken": "0x4ebdef163ff08ac1d56a89bafefd6c01cc28a48f",
-      "createdAt": 1612934761,
-      "isNew": True,
-      "liquidationThreshold": 0.5,
-      "ltv": 0.45
-    },
-    "0xd4cb328a82bdf5f03eb737f37fa6b370aef3e888": {
-      "cToken": "0x426d6d53187be3288fe37f214e3f6901d8145b62",
-      "createdAt": 1601532874,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0xe9e7cea3dedca5984780bafc599bd69add087d56": {
-      "cToken": "0x2bc4eb013ddee29d37920938b96d353171289b7c",
-      "createdAt": 1599059881,
-      "isNew": True,
-      "liquidationThreshold": 0.75,
-      "ltv": 0.7
-    },
-    "0xf8a0bf9cf54bb92f17374d9e9a321e6a111a51bd": {
-      "cToken": "0x3942936782d788ce69155f776a51a5f1c9dd9b22",
-      "createdAt": 1599990262,
-      "isNew": True,
-      "liquidationThreshold": 0.5,
-      "ltv": 0.45
-    },
-    "0xfce146bf3146100cfe5db4129cf6c82b0ef4ad8c": {
-      "cToken": "0x7f746a80506a4cafa39938f7c08ad59cfa6de418",
-      "createdAt": 1614064853,
-      "isNew": True,
-      "liquidationThreshold": 0,
-      "ltv": 0
+    "_id": "0x38_0x589de0f0ccf905477646599bb3e5c622c84cc0ba",
+    "chainId": "0x38",
+    "createdAt": 1577836800,
+    "comptrollerAddress": "0x589de0f0ccf905477646599bb3e5c622c84cc0ba",
+    "comptrollerImplementationAddress": "0x49a08f9f445af5734cf15a1deab3b1c6a7988fb4",
+    "projectName": "Cream",
+    "name": "Cream Lending Pool",
+    "rewardToken": "0xd4cb328a82bdf5f03eb737f37fa6b370aef3e888",
+    "lensAddress": "0x1a014ffe0cd187a298a7e79ba5ab05538686ea4a",
+    "type": "LENDING_POOL",
+    "reservesList": {
+        "0x0000000000000000000000000000000000000000": {
+            "cToken": "0x1ffe17b99b439be0afc831239ddecda2a790ff3a",
+            "liquidationThreshold": 0.75
+        },
+        "0x7130d2a12b9bcbfae4f2634d864a1ee1ce3ead9c": {
+            "cToken": "0x11883cdea6bab720092791cc89affa54428ce069",
+            "liquidationThreshold": 0.75
+        },
+        "0xe9e7cea3dedca5984780bafc599bd69add087d56": {
+            "cToken": "0x2bc4eb013ddee29d37920938b96d353171289b7c",
+            "liquidationThreshold": 0.75
+        },
+        "0x1d2f0da169ceb9fc7b3144628db156f3f6c60dbe": {
+            "cToken": "0xaa46e2c21b7763a73db48e9b318899253e66e20c",
+            "liquidationThreshold": 0.05
+        },
+        "0x8ff795a6f4d97e7887c79bea79aba5cc76444adf": {
+            "cToken": "0xcb87cee8c77cdfd310fb3c58ff72e688d46f90b1",
+            "liquidationThreshold": 0.05
+        },
+        "0x2170ed0880ac9a755fd29b2688956bd959f933f8": {
+            "cToken": "0xb31f5d117541825d6692c10e4357008edf3e2bcd",
+            "liquidationThreshold": 0.75
+        },
+        "0x4338665cbb7b2485a8855a139b75d5e34ab0db94": {
+            "cToken": "0x8cc7e2a6de999758499658bb702143fd025e09b2",
+            "liquidationThreshold": 0.05
+        },
+        "0x55d398326f99059ff775485246999027b3197955": {
+            "cToken": "0xef6d459fe81c3ed53d292c936b2df5a8084975de",
+            "liquidationThreshold": 0.75
+        },
+        "0xf8a0bf9cf54bb92f17374d9e9a321e6a111a51bd": {
+            "cToken": "0x3942936782d788ce69155f776a51a5f1c9dd9b22",
+            "liquidationThreshold": 0.0
+        },
+        "0x7083609fce4d1d8dc0c979aab8c869ea2c873402": {
+            "cToken": "0x53d88d2ffdbe71e81d95b08ae0ca49d0c4a8515f",
+            "liquidationThreshold": 0.0
+        },
+        "0x3ee2200efb3400fabb9aacf31297cbdd1d435d47": {
+            "cToken": "0x81c15d3e956e55e77e1f3f257f0a65bd2725fc55",
+            "liquidationThreshold": 0.05
+        },
+        "0xd4cb328a82bdf5f03eb737f37fa6b370aef3e888": {
+            "cToken": "0x426d6d53187be3288fe37f214e3f6901d8145b62",
+            "liquidationThreshold": 0.05
+        },
+        "0xad6caeb32cd2c308980a548bd0bc5aa4306c6c18": {
+            "cToken": "0x738f3810b3da0f3e6dc8c689d0d72f3b4992c43b",
+            "liquidationThreshold": 0.0
+        },
+        "0x56b6fb708fc5732dec1afc8d8556423a2edccbd6": {
+            "cToken": "0x19ee64850862cfd234e20c0db4eda286f12ec907",
+            "liquidationThreshold": 0.05
+        },
+        "0x1af3f329e8be154074d8769d1ffa4ee058b1dbc3": {
+            "cToken": "0x9095e8d707e40982affce41c61c10895157a1b22",
+            "liquidationThreshold": 0.75
+        },
+        "0x16939ef78684453bfdfb47825f8a5f714f12623a": {
+            "cToken": "0xe692714717a89e4f2ab89dd17d8dddd7bb52de8e",
+            "liquidationThreshold": 0.0
+        },
+        "0x0d8ce2a99bb6e3b7db580ed848240e4a0f9ae153": {
+            "cToken": "0x1af8c1c3ad36a041cb6678fed86b1e095004fd16",
+            "liquidationThreshold": 0.0
+        },
+        "0x88f1a5ae2a3bf98aeaf342d26b30a79438c9142e": {
+            "cToken": "0xea466cd2583a0290b9e7b987a769a7eb468fb0a5",
+            "liquidationThreshold": 0.0
+        },
+        "0xbf5140a22578168fd562dccf235e5d43a02ce9b1": {
+            "cToken": "0x3b0be453a4008ebc2edd457e7bd355f1c5469d68",
+            "liquidationThreshold": 0.0
+        },
+        "0x0eb3a705fc54725037cc9e008bdede697f62f335": {
+            "cToken": "0x0e9d900c884964dc4b26db96ba113825b1a09baa",
+            "liquidationThreshold": 0.0
+        },
+        "0x8ac76a51cc950d9822d68b83fe1ad97b32cd580d": {
+            "cToken": "0xd83c88db3a6ca4a32fff1603b0f7ddce01f5f727",
+            "liquidationThreshold": 0.75
+        },
+        "0xa1faa113cbe53436df28ff0aee54275c13b40975": {
+            "cToken": "0x264bc4ea2f45cf6331ad6c3ac8d7257cf487fcbc",
+            "liquidationThreshold": 0.0
+        },
+        "0x4b0f1812e5df2a09796481ff14017e6005508003": {
+            "cToken": "0x2d3bfadf9bc94e3ab796029a030e863f1898aa06",
+            "liquidationThreshold": 0.0
+        },
+        "0x0e09fabb73bd3ade0a17ecc321fd13a19e81ce82": {
+            "cToken": "0xbf9b95b78bc42f6cf53ff2a0ce19d607cfe1ff82",
+            "liquidationThreshold": 0.75
+        },
+        "0xcf6bb5389c92bdda8a3747ddb454cb7a64626c63": {
+            "cToken": "0x4ebdef163ff08ac1d56a89bafefd6c01cc28a48f",
+            "liquidationThreshold": 0.0
+        },
+        "0x101d82428437127bf1608f699cd651e6abf9766e": {
+            "cToken": "0x4cb7f1f4ad7a6b53802589af3b90612c1674fec4",
+            "liquidationThreshold": 0.0
+        },
+        "0x4bd17003473389a42daf6a0a729f6fdb328bbbd7": {
+            "cToken": "0x84902bd5ccef97648bf69c5096729a9367043beb",
+            "liquidationThreshold": 0.0
+        },
+        "0xa184088a740c695e156f91f5cc086a06bb78b827": {
+            "cToken": "0xf77df34f4bf632fb5ca928592a73a29a42bcf0b1",
+            "liquidationThreshold": 0.0
+        },
+        "0xfce146bf3146100cfe5db4129cf6c82b0ef4ad8c": {
+            "cToken": "0x7f746a80506a4cafa39938f7c08ad59cfa6de418",
+            "liquidationThreshold": 0.0
+        },
+        "0x695fd30af473f2960e81dc9ba7cb67679d35edb7": {
+            "cToken": "0xbe7e1d74acae787355169bc61a8729b2040fce6b",
+            "liquidationThreshold": 0.0
+        },
+        "0x250632378e573c6be1ac2f97fcdf00515d0aa91b": {
+            "cToken": "0xdcf60e349a5aaeeecdd2fb6772931fbf3486ed1c",
+            "liquidationThreshold": 0.0
+        },
+        "0x9678e42cebeb63f23197d726b29b1cb20d0064e5": {
+            "cToken": "0xc17c8c5b8bb9456c624f8534fde6cbda2451488c",
+            "liquidationThreshold": 0.0
+        },
+        "0x47bead2563dcbf3bf2c9407fea4dc236faba485a": {
+            "cToken": "0xa8d75a0d17d2f4f2f4673975ab8470269d019c96",
+            "liquidationThreshold": 0.0
+        },
+        "0x947950bcc74888a40ffa2593c5798f11fc9124c4": {
+            "cToken": "0x9b53e7d5e3f6cc8694840ed6c9f7fee79e7bcee5",
+            "liquidationThreshold": 0.0
+        },
+        "0xa527a61703d82139f8a06bc30097cc9caa2df5a6": {
+            "cToken": "0x36cdf5972aca2b70f10d0f7af0d95871abc065d9",
+            "liquidationThreshold": 0.0
+        },
+        "0x1b96b92314c44b159149f7e0303511fb2fc4774f": {
+            "cToken": "0x26a490a0f419dcfbed97e568403654c2746a7110",
+            "liquidationThreshold": 0.0
+        },
+        "0x7561eee90e24f3b348e1087a005f78b4c8453524": {
+            "cToken": "0xe39b9e0366940eb3ca62b85ffae838ef0f8b14e0",
+            "liquidationThreshold": 0.0
+        },
+        "0x70d8929d04b60af4fb9b58713ebcf18765ade422": {
+            "cToken": "0x5fa61a5a65920f90af970b13b7f28daeef0440b7",
+            "liquidationThreshold": 0.0
+        },
+        "0xc15fa3e22c912a276550f3e5fe3b0deb87b55acd": {
+            "cToken": "0x19b08ff7d90d63ad109c6fabb8e0fcc866477a41",
+            "liquidationThreshold": 0.0
+        },
+        "0xbb4cdb9cbd36b01bd1cbaebf2de08d9173bc095c": {
+            "cToken": "0x15cc701370cb8ada2a2b6f4226ec5cf6aa93bc67",
+            "liquidationThreshold": 0.05
+        },
+        "0x0ed7e52944161450477ee417de9cd3a859b14fd0": {
+            "cToken": "0x98b7871702b602e65eaef46051d75ca334f872d0",
+            "liquidationThreshold": 0.0
+        },
+        "0x58f876857a02d6762e0101bb5c46a8c1ed44dc16": {
+            "cToken": "0x7fd568d6a1a11b19427c8ccb90f7bb80e4ab1c5f",
+            "liquidationThreshold": 0.0
+        },
+        "0x61eb789d75a95caa3ff50ed7e47b96c132fec082": {
+            "cToken": "0x5ea2dd1de21ed3b5316cef89985edc66cf9b2a0e",
+            "liquidationThreshold": 0.0
+        },
+        "0x74e4716e431f45807dcf19f284c7aa99f18a4fbc": {
+            "cToken": "0x9972dd9912367cf395bea752ad49d81f33f7ca85",
+            "liquidationThreshold": 0.0
+        },
+        "0x7efaef62fddcca950418312c6c91aef321375a00": {
+            "cToken": "0x04c61ef58a6f1d6c572045a39a5434ab9dee69fb",
+            "liquidationThreshold": 0.0
+        }
     }
-  },
-  "lastUpdatedAt": 199999999,
-  "intervalUpdate": 900,
-  "url": "https://app.cream.finance/"
-}
+}
```

### Comparing `defi-services-lib-1.0.3/src/defi_services/lending_pools/lending_pools_info/bsc/valas_bsc.py` & `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/valas_bsc.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/lending_pools/lending_pools_info/bsc/venus_bsc.py` & `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/venus_bsc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,103 +1,111 @@
 VENUS_BSC = {
-  "chainId": "0x38",
-  "projectName": "Venus",
-  "name": "Venus Lending Pool",
-  "rewardToken": "0xcf6bb5389c92bdda8a3747ddb454cb7a64626c63",
-  "comptrollerAddress": "0xfd36e2c2a6789db23113685031d7f16329158384",
-  "lensAddress": "0xCDa4a4Ab96DfC1728EE265B9392373DB40e769F2",
-  "type": "LENDING_POOL",
-  "reservesList": {
-    "0x0000000000000000000000000000000000000000": {
-      "liquidationThreshold": 0.8,
-      "cToken": "0xa07c5b74c9b40447a954e1466938b865b6bbea36"
-    },
-    "0x0d8ce2a99bb6e3b7db580ed848240e4a0f9ae153": {
-      "liquidationThreshold": 0.6,
-      "cToken": "0xf91d58b5ae142dacc749f58a49fcbac340cb0343"
-    },
-    "0x0e09fabb73bd3ade0a17ecc321fd13a19e81ce82": {
-      "liquidationThreshold": 0.55,
-      "cToken": "0x86ac3974e2bd0d60825230fa6f355ff11409df5c"
-    },
-    "0x14016e85a25aeb13065688cafb43044c2ef86784": {
-      "liquidationThreshold": 0.8,
-      "cToken": "0x08ceb3f4a7ed3500ca0982bcd0fc7816688084c3"
-    },
-    "0x1af3f329e8be154074d8769d1ffa4ee058b1dbc3": {
-      "liquidationThreshold": 0.6,
-      "cToken": "0x334b3ecb4dca3593bccc3c7ebd1a1c1d1780fbf1"
-    },
-    "0x1d2f0da169ceb9fc7b3144628db156f3f6c60dbe": {
-      "liquidationThreshold": 0.6,
-      "cToken": "0xb248a295732e0225acd3337607cc01068e3b9c10"
-    },
-    "0x2170ed0880ac9a755fd29b2688956bd959f933f8": {
-      "liquidationThreshold": 0.8,
-      "cToken": "0xf508fcd89b8bd15579dc79a6827cb4686a3592c8"
-    },
-    "0x250632378e573c6be1ac2f97fcdf00515d0aa91b": {
-      "liquidationThreshold": 0.6,
-      "cToken": "0x972207a639cc1b374b893cc33fa251b55ceb7c07"
-    },
-    "0x3ee2200efb3400fabb9aacf31297cbdd1d435d47": {
-      "liquidationThreshold": 0.6,
-      "cToken": "0x9a0af7fdb2065ce470d72664de73cae409da28ec"
-    },
-    "0x4338665cbb7b2485a8855a139b75d5e34ab0db94": {
-      "liquidationThreshold": 0.6,
-      "cToken": "0x57a5297f2cb2c0aac9d554660acd6d385ab50c6b"
-    },
-    "0x47bead2563dcbf3bf2c9407fea4dc236faba485a": {
-      "liquidationThreshold": 0.5,
-      "cToken": "0x2ff3d0f6990a40261c66e1ff2017acbc282eb6d0"
-    },
-    "0x55d398326f99059ff775485246999027b3197955": {
-      "liquidationThreshold": 0.8,
-      "cToken": "0xfd5840cd36d94d7229439859c0112a4185bc0255"
-    },
-    "0x7083609fce4d1d8dc0c979aab8c869ea2c873402": {
-      "liquidationThreshold": 0.6,
-      "cToken": "0x1610bc33319e9398de5f57b33a5b184c806ad217"
-    },
-    "0x7130d2a12b9bcbfae4f2634d864a1ee1ce3ead9c": {
-      "liquidationThreshold": 0.8,
-      "cToken": "0x882c173bc7ff3b7786ca16dfed3dfffb9ee7847b"
-    },
-    "0x85eac5ac2f758618dfa09bdbe0cf174e7d574d5b": {
-      "liquidationThreshold": 0.6,
-      "cToken": "0x61edcfe8dd6ba3c891cb9bec2dc7657b3b422e93"
-    },
-    "0x8ac76a51cc950d9822d68b83fe1ad97b32cd580d": {
-      "liquidationThreshold": 0.8,
-      "cToken": "0xeca88125a5adbe82614ffc12d0db554e2e2867c8"
-    },
-    "0x8ff795a6f4d97e7887c79bea79aba5cc76444adf": {
-      "liquidationThreshold": 0.6,
-      "cToken": "0x5f0388ebc2b94fa8e123f404b79ccf5f40b29176"
-    },
-    "0xba2ae424d960c26247dd6c32edc70b295c744c43": {
-      "liquidationThreshold": 0.4,
-      "cToken": "0xec3422ef92b2fb59e84c8b02ba73f1fe84ed8d71"
-    },
-    "0xcc42724c6683b7e57334c4e856f4c9965ed682bd": {
-      "liquidationThreshold": 0.6,
-      "cToken": "0x5c9476fcd6a4f9a3654139721c949c2233bbbbc8"
-    },
-    "0xcf6bb5389c92bdda8a3747ddb454cb7a64626c63": {
-      "liquidationThreshold": 0.6,
-      "cToken": "0x151b1e2635a717bcdc836ecd6fbb62b674fe3e1d"
-    },
-    "0xe9e7cea3dedca5984780bafc599bd69add087d56": {
-      "liquidationThreshold": 0.8,
-      "cToken": "0x95c78222b3d6e262426483d42cfa53685a67ab9d"
-    },
-    "0xf8a0bf9cf54bb92f17374d9e9a321e6a111a51bd": {
-      "liquidationThreshold": 0.6,
-      "cToken": "0x650b940a1033b8a1b1873f78730fcfc73ec11f1f"
-    },
-    "0xfb6115445bff7b52feb98650c87f44907e58f802": {
-      "liquidationThreshold": 0.55,
-      "cToken": "0x26da28954763b92139ed49283625cecaf52c6f94"
+    "chainId": "0x38",
+    "projectName": "Venus",
+    "name": "Venus Lending Pool",
+    "rewardToken": "0xcf6bb5389c92bdda8a3747ddb454cb7a64626c63",
+    "comptrollerAddress": "0xfd36e2c2a6789db23113685031d7f16329158384",
+    "lensAddress": "0xCDa4a4Ab96DfC1728EE265B9392373DB40e769F2",
+    "type": "LENDING_POOL",
+    "reservesList": {
+        "0x8ac76a51cc950d9822d68b83fe1ad97b32cd580d": {
+            "cToken": "0xeca88125a5adbe82614ffc12d0db554e2e2867c8",
+            "liquidationThreshold": 0.825
+        },
+        "0x55d398326f99059ff775485246999027b3197955": {
+            "cToken": "0xfd5840cd36d94d7229439859c0112a4185bc0255",
+            "liquidationThreshold": 0.8
+        },
+        "0xe9e7cea3dedca5984780bafc599bd69add087d56": {
+            "cToken": "0x95c78222b3d6e262426483d42cfa53685a67ab9d",
+            "liquidationThreshold": 0.825
+        },
+        "0x47bead2563dcbf3bf2c9407fea4dc236faba485a": {
+            "cToken": "0x2ff3d0f6990a40261c66e1ff2017acbc282eb6d0",
+            "liquidationThreshold": 0.0
+        },
+        "0xcf6bb5389c92bdda8a3747ddb454cb7a64626c63": {
+            "cToken": "0x151b1e2635a717bcdc836ecd6fbb62b674fe3e1d",
+            "liquidationThreshold": 0.55
+        },
+        "0x0000000000000000000000000000000000000000": {
+            "cToken": "0xa07c5b74c9b40447a954e1466938b865b6bbea36",
+            "liquidationThreshold": 0.75
+        },
+        "0x7130d2a12b9bcbfae4f2634d864a1ee1ce3ead9c": {
+            "cToken": "0x882c173bc7ff3b7786ca16dfed3dfffb9ee7847b",
+            "liquidationThreshold": 0.8
+        },
+        "0x2170ed0880ac9a755fd29b2688956bd959f933f8": {
+            "cToken": "0xf508fcd89b8bd15579dc79a6827cb4686a3592c8",
+            "liquidationThreshold": 0.8
+        },
+        "0x4338665cbb7b2485a8855a139b75d5e34ab0db94": {
+            "cToken": "0x57a5297f2cb2c0aac9d554660acd6d385ab50c6b",
+            "liquidationThreshold": 0.6
+        },
+        "0x1d2f0da169ceb9fc7b3144628db156f3f6c60dbe": {
+            "cToken": "0xb248a295732e0225acd3337607cc01068e3b9c10",
+            "liquidationThreshold": 0.6
+        },
+        "0x8ff795a6f4d97e7887c79bea79aba5cc76444adf": {
+            "cToken": "0x5f0388ebc2b94fa8e123f404b79ccf5f40b29176",
+            "liquidationThreshold": 0.6
+        },
+        "0x7083609fce4d1d8dc0c979aab8c869ea2c873402": {
+            "cToken": "0x1610bc33319e9398de5f57b33a5b184c806ad217",
+            "liquidationThreshold": 0.6
+        },
+        "0xf8a0bf9cf54bb92f17374d9e9a321e6a111a51bd": {
+            "cToken": "0x650b940a1033b8a1b1873f78730fcfc73ec11f1f",
+            "liquidationThreshold": 0.6
+        },
+        "0x1af3f329e8be154074d8769d1ffa4ee058b1dbc3": {
+            "cToken": "0x334b3ecb4dca3593bccc3c7ebd1a1c1d1780fbf1",
+            "liquidationThreshold": 0.6
+        },
+        "0x0d8ce2a99bb6e3b7db580ed848240e4a0f9ae153": {
+            "cToken": "0xf91d58b5ae142dacc749f58a49fcbac340cb0343",
+            "liquidationThreshold": 0.6
+        },
+        "0x250632378e573c6be1ac2f97fcdf00515d0aa91b": {
+            "cToken": "0x972207a639cc1b374b893cc33fa251b55ceb7c07",
+            "liquidationThreshold": 0.6
+        },
+        "0x20bff4bbeda07536ff00e073bd8359e5d80d733d": {
+            "cToken": "0xebd0070237a0713e8d94fef1b728d3d993d290ef",
+            "liquidationThreshold": 0.0
+        },
+        "0x3ee2200efb3400fabb9aacf31297cbdd1d435d47": {
+            "cToken": "0x9a0af7fdb2065ce470d72664de73cae409da28ec",
+            "liquidationThreshold": 0.6
+        },
+        "0xba2ae424d960c26247dd6c32edc70b295c744c43": {
+            "cToken": "0xec3422ef92b2fb59e84c8b02ba73f1fe84ed8d71",
+            "liquidationThreshold": 0.4
+        },
+        "0xcc42724c6683b7e57334c4e856f4c9965ed682bd": {
+            "cToken": "0x5c9476fcd6a4f9a3654139721c949c2233bbbbc8",
+            "liquidationThreshold": 0.6
+        },
+        "0x0e09fabb73bd3ade0a17ecc321fd13a19e81ce82": {
+            "cToken": "0x86ac3974e2bd0d60825230fa6f355ff11409df5c",
+            "liquidationThreshold": 0.55
+        },
+        "0xfb6115445bff7b52feb98650c87f44907e58f802": {
+            "cToken": "0x26da28954763b92139ed49283625cecaf52c6f94",
+            "liquidationThreshold": 0.55
+        },
+        "0x14016e85a25aeb13065688cafb43044c2ef86784": {
+            "cToken": "0x08ceb3f4a7ed3500ca0982bcd0fc7816688084c3",
+            "liquidationThreshold": 0.8
+        },
+        "0x85eac5ac2f758618dfa09bdbe0cf174e7d574d5b": {
+            "cToken": "0x61edcfe8dd6ba3c891cb9bec2dc7657b3b422e93",
+            "liquidationThreshold": 0.0
+        },
+        "0xce7de646e7208a4ef112cb6ed5038fa6cc6b12e3": {
+            "cToken": "0xc5d3466aa484b040ee977073fcf337f2c00071c1",
+            "liquidationThreshold": 0.525
+        }
     }
-  },
-}
+}
```

### Comparing `defi-services-lib-1.0.3/src/defi_services/lending_pools/services/cream_state_service.py` & `defi-services-lib-1.0.4/src/defi_services/lending_pools/services/cream_state_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 from defi_services.abis.erc20_abi import ERC20_ABI
 from defi_services.abis.lending_pool.cream_comptroller_abi import CREAM_COMPTROLLER_ABI
 from defi_services.abis.lending_pool.cream_lens_abi import CREAM_LENS_ABI
 from defi_services.abis.lending_pool.ctoken_abi import CTOKEN_ABI
-from defi_services.constants.contract_address import ContractAddresses, AbnormalCreamPool
+from defi_services.constants.contract_address import ContractAddresses, AbnormalCreamPool, WrappedNativeTokens
 from defi_services.constants.db_constant import DBConst
 from defi_services.state_service import StateService
 from defi_services.utils.batch_queries_service import add_rpc_call, decode_data_response
 
 _LOGGER = logging.getLogger("TravaVaultSS")
 
 
@@ -34,14 +34,35 @@
         tokens = [self.to_checksum(i) for i in token_addresses]
         reserve_tokens_info = lens_contract.functions.cTokenUnderlyingPriceAll(tokens).call(
             block_identifier=block_number)
         for price_token in reserve_tokens_info:
             reserve_tokens_info[price_token[0].lower()] = price_token[1] * bnb_price
         return reserve_tokens_info
 
+    def get_reserves_info(
+            self,
+            comptroller_address: str,
+            comptroller_abi: list,
+            lens_address: str,
+            lens_abi: list,
+            block_number: int = "latest"):
+        ctokens = self.get_all_markets(comptroller_address, comptroller_abi, block_number)
+        metadata = self.ctoken_metadata_all(lens_address, lens_abi, ctokens, block_number)
+        reserves_info = {}
+        for data in metadata:
+            underlying = data[11].lower()
+            ctoken = data[0].lower()
+            lt = data[10] / 10 ** 18
+            reserves_info[underlying] = {
+                "cToken": ctoken,
+                "liquidationThreshold": lt
+            }
+
+        return reserves_info
+
     def get_all_markets(
             self, comptroller: str, comptroller_abi: list, block_number: int = 'latest'):
         comptroller_contract = self._w3.eth.contract(
             address=self._w3.toChecksumAddress(comptroller), abi=comptroller_abi)
         tokens = []
         for token in comptroller_contract.functions.getAllMarkets().call(block_identifier=block_number):
             if token in [ContractAddresses.LUNA.lower(), ContractAddresses.UST.lower(), ContractAddresses.LUNA,
@@ -105,17 +126,22 @@
             ctoken_speeds[lower_address] = decoded_data.get(speeds_call_id)
             borrow_paused_tokens[lower_address] = decoded_data.get(borrow_guardian_paused_call_id)
             mint_paused_tokens[lower_address] = decoded_data.get(mint_guardian_paused_call_id)
             metadata_id = f"cTokenMetadata_{lens_address}_{token_address}_{block_number}".lower()
             reserve_tokens_info.append(decoded_data.get(metadata_id))
             underlying_id = f"cTokenUnderlyingPrice_{lens_address}_{token_address}_{block_number}".lower()
             price_token = decoded_data.get(underlying_id)
+            underlying_decimals = decoded_data.get(metadata_id)[-1]
             underlying_prices[lower_address] = price_token[1] * wrapped_native_token_price
             if lower_address in AbnormalCreamPool.decimals.keys():
                 underlying_prices[lower_address] /= 10 ** AbnormalCreamPool.decimals.get(lower_address)
+            elif underlying_decimals == 8:
+                underlying_prices[lower_address] /= 10 ** 20
+            elif underlying_decimals == 6:
+                underlying_prices[lower_address] /= 10 ** 24
         return {
             "reserve_tokens_info": reserve_tokens_info,
             "ctoken_speeds": ctoken_speeds,
             "borrow_paused_tokens": borrow_paused_tokens,
             "mint_paused_tokens": mint_paused_tokens,
             "underlying_prices": underlying_prices
         }
@@ -301,22 +327,23 @@
             self,
             wallet_address: str,
             lens_address: str,
             reserves_info: dict,
             lens_abi: list = CREAM_LENS_ABI,
             block_number: int = "latest",
             wrapped_native_token_price: float = 310,
+            wrapped_native_token: str = None
     ):
         list_rpc_call = []
         list_call_id = []
         for token in reserves_info:
             underlying = token
             value = reserves_info[token]
-            if token == ContractAddresses.BNB:
-                underlying = ContractAddresses.WBNB
+            if token == WrappedNativeTokens.NATIVE_TOKEN:
+                underlying = wrapped_native_token
             add_rpc_call(abi=lens_abi, contract_address=lens_address, fn_paras=value["cToken"],
                          block_number=block_number,
                          list_call_id=list_call_id, list_rpc_call=list_rpc_call, fn_name="cTokenUnderlyingPrice")
             add_rpc_call(abi=CTOKEN_ABI, contract_address=value["cToken"], fn_name="borrowBalanceCurrent",
                          block_number=block_number,
                          fn_paras=wallet_address, list_call_id=list_call_id, list_rpc_call=list_rpc_call)
             add_rpc_call(abi=CTOKEN_ABI, contract_address=value["cToken"], fn_name="balanceOfUnderlying",
@@ -332,16 +359,16 @@
             "deposit_amount_in_usd": 0,
             "health_factor": 0,
             'reserves_data': {}
         }
         for token in reserves_info:
             underlying = token
             value = reserves_info[token]
-            if token == ContractAddresses.BNB:
-                underlying = ContractAddresses.WBNB
+            if token == WrappedNativeTokens.NATIVE_TOKEN:
+                underlying = wrapped_native_token
             get_total_deposit_id = f"balanceOfUnderlying_{value['cToken']}_{wallet_address}_{block_number}".lower()
             get_total_borrow_id = f"borrowBalanceCurrent_{value['cToken']}_{wallet_address}_{block_number}".lower()
             get_decimals_id = f"decimals_{underlying}_{block_number}".lower()
             decimals = decoded_data[get_decimals_id]
             deposit_amount = decoded_data[get_total_deposit_id] / 10 ** decimals
             borrow_amount = decoded_data[get_total_borrow_id] / 10 ** decimals
             get_underlying_token_price = f"cTokenUnderlyingPrice_{lens_address}_{value['cToken']}_{block_number}".lower()
@@ -360,7 +387,22 @@
                     "deposit_amount_in_usd": deposit_amount_in_usd,
                 }
         if total_borrow != 0:
             result['health_factor'] /= total_borrow
         else:
             result['health_factor'] = 100
         return result
+
+
+if __name__ == "__main__":
+    import json
+    from defi_services.lending_pools.lending_pools_info.bsc.cream_bsc import CREAM_BSC
+
+    service = CreamStateService(provider_uri="https://rpc.ankr.com/bsc")
+    reserve_info = service.get_reserves_info(
+        lens_address=CREAM_BSC.get("lensAddress"),
+        comptroller_address=CREAM_BSC.get("comptrollerAddress"),
+        lens_abi=CREAM_LENS_ABI,
+        comptroller_abi=CREAM_COMPTROLLER_ABI
+    )
+    with open("cream_bsc.json", "w") as f:
+        f.write(json.dumps(reserve_info, indent=1))
```

### Comparing `defi-services-lib-1.0.3/src/defi_services/lending_pools/services/trava_state_service.py` & `defi-services-lib-1.0.4/src/defi_services/lending_pools/services/trava_state_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,26 @@
         prices = contract.functions.getAssetsPrices(tokens).call(block_identifier=block_number)
         result = {}
         for i in range(len(reserves)):
             result[reserves[i].lower()] = prices[i] / 10 ** pool_decimals
 
         return result
 
+    def get_reserves_info(self, pool_address: str, pool_abi: list, block_number: int = "latest"):
+        reserves_list = self.get_reserves_list(pool_address, pool_abi, block_number)
+        reserves_data = self.get_reserve_data_of_token_list(pool_address, reserves_list, pool_abi, block_number)
+        reserves_info = {}
+        for key, value in reserves_data.items():
+            reserves_info[key] = {}
+            reserves_info[key]["tToken"] = value[6]
+            reserves_info[key]["dToken"] = value[7]
+            risk_param = bin(value[0][0])[2:]
+            reserves_info[key]["liquidationThreshold"] = int(risk_param[-31:-16], 2) / 10 ** 4
+        return reserves_info
+
     def _encode_apy_lending_pool_function_call(
             self,
             pool_address: str,
             pool_abi: list,
             reserves_list: list,
             stake_incentive_address: str = None,
             stake_incentive_abi: list = None,
@@ -155,16 +167,18 @@
             pool_abi: list = TRAVA_LENDING_POOL_ABI,
             staked_incentive_abi: list = STAKED_INCENTIVES_ABI,
             reserves_info: dict = None,
             token_prices: dict = None,
             pool_token_price: float = 1,
             block_number: int = 'latest',
     ):
+        if not reserves_info:
+            reserves_info = self.get_reserves_info(pool_address, pool_abi, block_number)
 
-        reserves_list = self.get_reserves_list(pool_address, pool_abi, block_number)
+        reserves_list = list(reserves_info.keys())
         token_prices = self.get_assets_price(oracle_address, oracle_abi, reserves_list, block_number)
         list_rpc_call, list_call_id = self._encode_apy_lending_pool_function_call(
             pool_address, pool_abi, reserves_list, staked_incentive_address, staked_incentive_abi,
             oracle_address, oracle_abi, block_number,
         )
         # Decode data
         decoded_data = self._decode_apy_lending_pool_function_call(
@@ -191,18 +205,24 @@
             asset_data_d = asset_data_tokens.get(debt_token)
             # update deposit, borrow apy
             total_supply_t = total_supply_t / 10 ** decimal
             total_supply_d = total_supply_d / 10 ** decimal
             eps_t = asset_data_t[1] / 10 ** 18
             eps_d = asset_data_d[1] / 10 ** 18
             token_price = token_prices.get(token_address)
-            deposit_apr = eps_t * TimeConstants.A_YEAR * pool_token_price / (
-                    total_supply_t * token_price)
-            borrow_apr = eps_d * TimeConstants.A_YEAR * pool_token_price / (
-                    total_supply_d * token_price)
+            if total_supply_t:
+                deposit_apr = eps_t * TimeConstants.A_YEAR * pool_token_price / (
+                        total_supply_t * token_price)
+            else:
+                deposit_apr = 0
+            if total_supply_d:
+                borrow_apr = eps_d * TimeConstants.A_YEAR * pool_token_price / (
+                        total_supply_d * token_price)
+            else:
+                borrow_apr = 0
             interest_rate[token_address].update({
                 "utilization": total_supply_d / total_supply_t,
                 DBConst.reward_deposit_apy: deposit_apr,
                 DBConst.reward_borrow_apy: borrow_apr})
             # update liquidity
             liquidity_log = {
                 DBConst.total_borrow: {
@@ -217,61 +237,59 @@
         return interest_rate
 
     def get_rewards_balance(
             self,
             wallet_address,
             pool_address,
             staked_incentive_address: str,
+            reserves_info: dict = None,
             pool_abi: list = TRAVA_LENDING_POOL_ABI,
             staked_incentive_abi: list = STAKED_INCENTIVES_ABI,
             block_number: int = "latest"
     ):
-        reserves_list = self.get_reserves_list(pool_address, pool_abi, block_number)
-        reserves_data = self.get_reserve_data_of_token_list(pool_address, reserves_list, pool_abi, block_number)
+        if not reserves_info:
+            reserves_info = self.get_reserves_info(pool_address, pool_abi, block_number)
+
         tokens = []
-        for key, value in reserves_data.items():
-            tokens += [self.to_checksum(value[6]), self.to_checksum(value[7])]
+        for key, value in reserves_info.items():
+            tokens += [self.to_checksum(value["tToken"]), self.to_checksum(value["dToken"])]
         contract = self._w3.eth.contract(address=self.to_checksum(staked_incentive_address), abi=staked_incentive_abi)
         reward = contract.functions.getRewardsBalance(tokens, self.to_checksum(wallet_address)).call(
             block_identifier=block_number)
         return reward / 10 ** 18
 
     def get_wallet_deposit_borrow_balance(
             self,
             wallet_address: str,
             pool_address: str,
             oracle_address: str,
+            reserves_info: dict = None,
             pool_abi: list = TRAVA_LENDING_POOL_ABI,
             oracle_abi: list = ORACLE_ABI,
             block_number: int = "latest"
     ):
-        reserves_list = self.get_reserves_list(pool_address, pool_abi, block_number)
+        if not reserves_info:
+            reserves_info = self.get_reserves_info(pool_address, pool_abi)
+
+        reserves_list = list(reserves_info.keys())
         token_prices = self.get_assets_price(oracle_address, oracle_abi, reserves_list, block_number)
-        reserves_data = self.get_reserve_data_of_token_list(pool_address, reserves_list, pool_abi, block_number)
-        reserves_info = {}
-        for key, value in reserves_data.items():
-            reserves_info[key] = {}
-            reserves_info[key]["tToken"] = value[6]
-            reserves_info[key]["dToken"] = value[7]
-            risk_param = bin(value[0][0])[2:]
-            reserves_info[key]["liquidationThreshold"] = int(risk_param[-31:-16], 2) / 10 ** 4
         list_rpc_call = []
         list_call_id = []
         for token in reserves_info:
             value = reserves_info[token]
             add_rpc_call(abi=ERC20_ABI, contract_address=value["tToken"], fn_paras=wallet_address,
                          block_number=block_number,
                          list_call_id=list_call_id, list_rpc_call=list_rpc_call, fn_name="balanceOf")
             add_rpc_call(abi=ERC20_ABI, contract_address=value["dToken"], fn_paras=wallet_address,
                          block_number=block_number,
                          list_call_id=list_call_id, list_rpc_call=list_rpc_call, fn_name="balanceOf")
             add_rpc_call(abi=ERC20_ABI, contract_address=token, fn_name="decimals", block_number=block_number,
                          list_call_id=list_call_id, list_rpc_call=list_rpc_call)
 
-        data_response = self.client_querier.sent_batch_to_provider(list_rpc_call)
+        data_response = self.client_querier.sent_batch_to_provider(list_rpc_call, batch_size=100)
         decoded_data = decode_data_response(data_response, list_call_id)
         total_borrow, result = 0, {
             "borrow_amount_in_usd": 0,
             "deposit_amount_in_usd": 0,
             "health_factor": 0,
             "reserves_data": {}
         }
@@ -298,7 +316,30 @@
                 }
 
         if total_borrow != 0:
             result['health_factor'] /= total_borrow
         else:
             result['health_factor'] = 100
         return result
+
+
+if __name__ == "__main__":
+    import json
+    from defi_services.lending_pools.lending_pools_info.ethereum.trava_eth import TRAVA_ETH
+    from defi_services.lending_pools.lending_pools_info.bsc.trava_bsc import TRAVA_BSC
+    from defi_services.lending_pools.lending_pools_info.fantom.trava_ftm import TRAVA_FTM
+    from defi_services.abis.lending_pool.trava_lending_pool_abi import TRAVA_LENDING_POOL_ABI
+
+    service = TravaStateService(provider_uri="https://rpc.ankr.com/eth")
+    reserve_info = service.get_reserves_info(TRAVA_ETH.get("address"), TRAVA_LENDING_POOL_ABI)
+    with open("trava_eth.json", "w") as f:
+        f.write(json.dumps(reserve_info, indent=1))
+
+    service = TravaStateService(provider_uri="https://rpc.ankr.com/fantom")
+    reserve_info = service.get_reserves_info(TRAVA_FTM.get("address"), TRAVA_LENDING_POOL_ABI)
+    with open("trava_ftm.json", "w") as f:
+        f.write(json.dumps(reserve_info, indent=1))
+
+    service = TravaStateService(provider_uri="https://rpc.ankr.com/bsc")
+    reserve_info = service.get_reserves_info(TRAVA_BSC.get("address"), TRAVA_LENDING_POOL_ABI)
+    with open("trava_bsc.json", "w") as f:
+        f.write(json.dumps(reserve_info, indent=1))
```

### Comparing `defi-services-lib-1.0.3/src/defi_services/lending_pools/services/valas_state_service.py` & `defi-services-lib-1.0.4/src/defi_services/lending_pools/services/valas_state_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,27 @@
         result = {}
         for token_address in token_addresses:
             get_asset_data_call_id = f'poolInfo_{chef_incentive_address}_{token_address}_{block_number}'.lower()
             result[token_address.lower()] = decoded_data.get(get_asset_data_call_id)
 
         return result
 
+    def get_reserves_info(self, pool_address: str, pool_abi: list, block_number: int = "latest"):
+        reserves_list = self.get_reserves_list(pool_address, pool_abi, block_number)
+        reserves_data = self.get_reserve_data_of_token_list(pool_address, reserves_list, pool_abi, block_number)
+        reserves_info = {}
+        for key, value in reserves_data.items():
+            reserves_info[key] = {}
+            reserves_info[key]["tToken"] = value[7]
+            reserves_info[key]["dToken"] = value[9]
+            reserves_info[key]["sdToken"] = value[8]
+            risk_param = bin(value[0][0])[2:]
+            reserves_info[key]["liquidationThreshold"] = int(risk_param[-31:-16], 2) / 10 ** 4
+        return reserves_info
+
     def _encode_apy_lending_pool_function_call(
             self,
             pool_address: str,
             pool_abi: list,
             reserves_list: list,
             chef_incentive_address: str = None,
             chef_incentives_abi: list = None,
@@ -128,17 +141,22 @@
             chef_incentive_address: str,
             chef_incentive_abi: list = CHEF_INCENTIVES_CONTROLLER,
             pool_abi: list = LENDING_POOL_ABI,
             oracle_abi: list = ORACLE_ABI,
             reserves_info: dict = None,
             block_number: int = 'latest',
             token_prices: dict = None,
-            pool_token_price: float = 1):
-        reserves_list = self.get_reserves_list(pool_address, pool_abi, block_number)
-        token_prices = self.get_assets_price(oracle_address, oracle_abi, reserves_list, block_number, 18)
+            pool_token_price: float = 1,
+            pool_decimals: int = 18
+    ):
+        if not reserves_info:
+            reserves_info = self.get_reserves_info(pool_address, pool_abi)
+
+        reserves_list = list(reserves_info.keys())
+        token_prices = self.get_assets_price(oracle_address, oracle_abi, reserves_list, block_number, pool_decimals)
         list_rpc_call, list_call_id = self._encode_apy_lending_pool_function_call(
             pool_address, pool_abi, reserves_list, chef_incentive_address, chef_incentive_abi,
             oracle_address, oracle_abi, block_number,
         )
         decoded_data = self._decode_apy_lending_pool_function_call(
             list_rpc_call, list_call_id, pool_address,
             reserves_list, chef_incentive_address, oracle_address, block_number
@@ -165,18 +183,24 @@
             asset_data_d = asset_data_tokens.get(debt_token)
             # update deposit, borrow apy
             total_supply_t = total_supply_t / 10 ** decimal
             total_supply_d = total_supply_d / 10 ** decimal
             eps_t = rewards_per_second * asset_data_t[1] / (total_alloc_point * 10 ** 18)
             eps_d = rewards_per_second * asset_data_d[1] / (total_alloc_point * 10 ** 18)
             token_price = token_prices.get(token_address)
-            deposit_apr = eps_t * TimeConstants.A_YEAR * pool_token_price / (
-                    total_supply_t * token_price)
-            borrow_apr = eps_d * TimeConstants.A_YEAR * pool_token_price / (
-                    total_supply_d * token_price)
+            if total_supply_t:
+                deposit_apr = eps_t * TimeConstants.A_YEAR * pool_token_price / (
+                        total_supply_t * token_price)
+            else:
+                deposit_apr = 0
+            if total_supply_d:
+                borrow_apr = eps_d * TimeConstants.A_YEAR * pool_token_price / (
+                        total_supply_d * token_price)
+            else:
+                borrow_apr = 0
             # update deposit, borrow reward apr
             interest_rate[token_address].update({DBConst.reward_deposit_apy: deposit_apr,
                                                  DBConst.reward_borrow_apy: borrow_apr})
             # update liquidity
             liquidity_log = {
                 DBConst.total_borrow: {
                     DBConst.amount: total_supply_d,
@@ -189,42 +213,38 @@
         return interest_rate
 
     def get_rewards_balance(
             self,
             wallet_address,
             pool_address,
             multi_fee_address: str,
+            reserves_info: dict = None,
             pool_abi: list = LENDING_POOL_ABI,
             multi_fee_distribution: list = VALAS_MULTI_FEE_DISTRIBUTION,
             block_number: int = "latest"
     ):
         contract = self._w3.eth.contract(address=self.to_checksum(multi_fee_address), abi=multi_fee_distribution)
         reward = contract.functions.earnedBalances(self.to_checksum(wallet_address)).call(block_identifier=block_number)
         return reward[0] / 10 ** 18
 
     def get_wallet_deposit_borrow_balance(
             self,
             wallet_address: str,
             pool_address: str,
             oracle_address: str,
+            reserves_info: str = None,
             pool_abi: list = LENDING_POOL_ABI,
             oracle_abi: list = ORACLE_ABI,
-            block_number: int = "latest"
+            block_number: int = "latest",
+            pool_decimals: int = 18
     ):
-        reserves_list = self.get_reserves_list(pool_address, pool_abi, block_number)
-        token_prices = self.get_assets_price(oracle_address, oracle_abi, reserves_list, block_number, 18)
-        reserves_data = self.get_reserve_data_of_token_list(pool_address, reserves_list, pool_abi, block_number)
-        reserves_info = {}
-        for key, value in reserves_data.items():
-            reserves_info[key] = {}
-            reserves_info[key]["tToken"] = value[7]
-            reserves_info[key]["dToken"] = value[9]
-            reserves_info[key]["sdToken"] = value[8]
-            risk_param = bin(value[0][0])[2:]
-            reserves_info[key]["liquidationThreshold"] = int(risk_param[-31:-16], 2) / 10 ** 4
+        if not reserves_info:
+            reserves_info = self.get_reserves_info(pool_address, pool_abi)
+        reserves_list = list(reserves_info.keys())
+        token_prices = self.get_assets_price(oracle_address, oracle_abi, reserves_list, block_number, pool_decimals)
         list_rpc_call = []
         list_call_id = []
         for token in reserves_info:
             value = reserves_info[token]
             add_rpc_call(abi=ERC20_ABI, contract_address=value["tToken"], fn_paras=wallet_address,
                          block_number=block_number,
                          list_call_id=list_call_id, list_rpc_call=list_rpc_call, fn_name="balanceOf")
@@ -232,15 +252,15 @@
                          block_number=block_number,
                          list_call_id=list_call_id, list_rpc_call=list_rpc_call, fn_name="balanceOf")
             add_rpc_call(abi=ERC20_ABI, contract_address=value["sdToken"], fn_paras=wallet_address,
                          block_number=block_number,
                          list_call_id=list_call_id, list_rpc_call=list_rpc_call, fn_name="balanceOf")
             add_rpc_call(abi=ERC20_ABI, contract_address=token, fn_name="decimals", block_number=block_number,
                          list_call_id=list_call_id, list_rpc_call=list_rpc_call)
-        data_response = self.client_querier.sent_batch_to_provider(list_rpc_call)
+        data_response = self.client_querier.sent_batch_to_provider(list_rpc_call, batch_size=100)
         decoded_data = decode_data_response(data_response, list_call_id)
         total_borrow, result = 0, {
             "borrow_amount_in_usd": 0,
             "deposit_amount_in_usd": 0,
             "health_factor": 0,
             "reserves_data": {}
         }
```

### Comparing `defi-services-lib-1.0.3/src/defi_services/lending_pools/services/venus_state_service.py` & `defi-services-lib-1.0.4/src/defi_services/lending_pools/services/venus_state_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from defi_services.abis.erc20_abi import ERC20_ABI
 from defi_services.abis.lending_pool.ctoken_abi import CTOKEN_ABI
 from defi_services.abis.lending_pool.venus_comptroller_abi import VENUS_COMPTROLLER_ABI
 from defi_services.abis.lending_pool.venus_lens_abi import VENUS_LENS_ABI
-from defi_services.constants.contract_address import ContractAddresses, AbnormalVenusPool
+from defi_services.constants.contract_address import ContractAddresses, AbnormalVenusPool, WrappedNativeTokens
 from defi_services.lending_pools.services.cream_state_service import CreamStateService
 from defi_services.utils.batch_queries_service import add_rpc_call, decode_data_response
 
 
 class VenusStateService(CreamStateService):
     def __init__(self, provider_uri):
         super().__init__(provider_uri)
@@ -29,14 +29,35 @@
         tokens = [self.to_checksum(i) for i in token_addresses]
         reserve_tokens_info = lens_contract.functions.vTokenUnderlyingPriceAll(tokens).call(
             block_identifier=block_number)
         for price_token in reserve_tokens_info:
             reserve_tokens_info[price_token[0].lower()] = price_token[1] * bnb_price
         return reserve_tokens_info
 
+    def get_reserves_info(
+            self,
+            comptroller_address: str,
+            comptroller_abi: list,
+            lens_address: str,
+            lens_abi: list,
+            block_number: int = 'latest'):
+        ctokens = self.get_all_markets(comptroller_address, comptroller_abi, block_number)
+        metadata = self.vtoken_metadata_all(lens_address, lens_abi, ctokens, block_number)
+        reserves_info = {}
+        for data in metadata:
+            underlying = data[11].lower()
+            ctoken = data[0].lower()
+            lt = data[10] / 10 ** 18
+            reserves_info[underlying] = {
+                "cToken": ctoken,
+                "liquidationThreshold": lt
+            }
+
+        return reserves_info
+
     def get_token_speed(
             self, token_addresses: list, comptroller: str,
             comptroller_abi: list = VENUS_COMPTROLLER_ABI, block_number: int = 'latest'):
         list_rpc_call = []
         list_call_id = []
         for token_address in token_addresses:
             add_rpc_call(
@@ -93,17 +114,22 @@
         for token_address in token_addresses:
             lower_address = token_address.lower()
             metadata_id = f"vTokenMetadata_{lens_address}_{token_address}_{block_number}".lower()
             speeds_call_id = f'venusSpeeds_{comptroller_address}_{token_address}_{block_number}'.lower()
             reserve_tokens_info.append(decoded_data.get(metadata_id))
             underlying_id = f"vTokenUnderlyingPrice_{lens_address}_{token_address}_{block_number}".lower()
             price_token = decoded_data.get(underlying_id)
+            underlying_decimals = decoded_data.get(metadata_id)[-1]
             underlying_prices[lower_address] = price_token[1]
             if lower_address in AbnormalVenusPool.decimals.keys():
                 underlying_prices[lower_address] /= 10 ** AbnormalVenusPool.decimals.get(lower_address)
+            elif underlying_decimals == 8:
+                underlying_prices[lower_address] /= 10 ** 20
+            elif underlying_decimals == 6:
+                underlying_prices[lower_address] /= 10 ** 24
             ctoken_speeds[token_address.lower()] = decoded_data.get(speeds_call_id)
             borrow_paused_tokens[token_address.lower()] = False
             mint_paused_tokens[token_address.lower()] = False
 
         return {
             "reserve_tokens_info": reserve_tokens_info,
             "ctoken_speeds": ctoken_speeds,
@@ -187,22 +213,23 @@
             self,
             wallet_address: str,
             lens_address: str,
             reserves_info: dict,
             lens_abi: list = VENUS_LENS_ABI,
             block_number: int = "latest",
             wrapped_native_token_price: float = 310,
+            wrapped_native_token: str = None
     ):
         list_rpc_call = []
         list_call_id = []
         for token in reserves_info:
             underlying = token
             value = reserves_info[token]
-            if token == ContractAddresses.BNB:
-                underlying = ContractAddresses.WBNB
+            if token == WrappedNativeTokens.NATIVE_TOKEN:
+                underlying = wrapped_native_token
             add_rpc_call(abi=lens_abi, contract_address=lens_address, fn_paras=value["cToken"],
                          block_number=block_number,
                          list_call_id=list_call_id, list_rpc_call=list_rpc_call, fn_name="vTokenUnderlyingPrice")
             add_rpc_call(abi=CTOKEN_ABI, contract_address=value["cToken"], fn_name="borrowBalanceCurrent",
                          block_number=block_number,
                          fn_paras=wallet_address, list_call_id=list_call_id, list_rpc_call=list_rpc_call)
             add_rpc_call(abi=CTOKEN_ABI, contract_address=value["cToken"], fn_name="balanceOfUnderlying",
@@ -218,16 +245,16 @@
             "deposit_amount_in_usd": 0,
             "health_factor": 0,
             'reserves_data': {}
         }
         for token in reserves_info:
             underlying = token
             value = reserves_info[token]
-            if token == ContractAddresses.BNB:
-                underlying = ContractAddresses.WBNB
+            if token == WrappedNativeTokens.NATIVE_TOKEN:
+                underlying = wrapped_native_token
             get_total_deposit_id = f"balanceOfUnderlying_{value['cToken']}_{wallet_address}_{block_number}".lower()
             get_total_borrow_id = f"borrowBalanceCurrent_{value['cToken']}_{wallet_address}_{block_number}".lower()
             get_decimals_id = f"decimals_{underlying}_{block_number}".lower()
             decimals = decoded_data[get_decimals_id]
             deposit_amount = decoded_data[get_total_deposit_id] / 10 ** decimals
             borrow_amount = decoded_data[get_total_borrow_id] / 10 ** decimals
             get_underlying_token_price = f"vTokenUnderlyingPrice_{lens_address}_{value['cToken']}_{block_number}".lower()
@@ -249,7 +276,22 @@
                     "deposit_amount_in_usd": deposit_amount_in_usd,
                 }
         if total_borrow != 0:
             result['health_factor'] /= total_borrow
         else:
             result['health_factor'] = 100
         return result
+
+
+if __name__ == "__main__":
+    import json
+    from defi_services.lending_pools.lending_pools_info.bsc.venus_bsc import VENUS_BSC
+
+    service = VenusStateService(provider_uri="https://rpc.ankr.com/bsc")
+    reserve_info = service.get_reserves_info(
+        lens_address=VENUS_BSC.get("lensAddress"),
+        comptroller_address=VENUS_BSC.get("comptrollerAddress"),
+        lens_abi=VENUS_LENS_ABI,
+        comptroller_abi=VENUS_COMPTROLLER_ABI
+    )
+    with open("venus_bsc.json", "w") as f:
+        f.write(json.dumps(reserve_info, indent=1))
```

### Comparing `defi-services-lib-1.0.3/src/defi_services/lending_pools/trava_service.py` & `defi-services-lib-1.0.4/src/defi_services/lending_pools/valas_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 from defi_services.constants.chain_constant import Chain
 from defi_services.defi_service import DefiService
-from defi_services.lending_pools.lending_pools_info.bsc.trava_bsc import TRAVA_BSC
-from defi_services.lending_pools.services.trava_state_service import TravaStateService
+from defi_services.lending_pools.lending_pools_info.bsc.valas_bsc import VALAS_BSC
+from defi_services.lending_pools.services.valas_state_service import ValasStateService
 
 
-class TravaService(DefiService):
+class ValasService(DefiService):
+    name = "valas lending pool"
+
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
-        self.state_service = TravaStateService(provider_uri)
+        self.state_service = ValasStateService(provider_uri)
         self.defi_constant = self._get_constant()
 
     def _get_constant(self):
         if self.chain_id == Chain.bsc:
-            return TRAVA_BSC
+            return VALAS_BSC
         return None
 
     def get_apy_defi_app(self, block_number: int = "latest"):
         return self.state_service.get_apy_lending_pool(
             pool_address=self.defi_constant.get("address"),
-            staked_incentive_address=self.defi_constant.get("stakedIncentiveAddress"),
+            chef_incentive_address=self.defi_constant.get("chefIncentiveAddress"),
             oracle_address=self.defi_constant.get("oracleAddress"),
             block_number=block_number
         )
-    
+
     def get_rewards_balance(self, wallet_address: str, block_number: int = "latest"):
         return self.state_service.get_rewards_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
-            staked_incentive_address=self.defi_constant.get("stakedIncentiveAddress"),
-            block_number=block_number
+            multi_fee_address=self.defi_constant.get("multiFeeAddress"),
+            block_number=block_number,
+            reserves_info=self.defi_constant.get("reservesList")
         )
 
     def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest"):
         return self.state_service.get_wallet_deposit_borrow_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
             oracle_address=self.defi_constant.get("oracleAddress"),
-            block_number=block_number
-        )
+            block_number=block_number,
+            reserves_info=self.defi_constant.get("reservesList")
+        )
```

### Comparing `defi-services-lib-1.0.3/src/defi_services/lending_pools/valas_service.py` & `defi-services-lib-1.0.4/src/defi_services/lending_pools/geist_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from defi_services.constants.chain_constant import Chain
 from defi_services.defi_service import DefiService
-from defi_services.lending_pools.lending_pools_info.bsc.valas_bsc import VALAS_BSC
-from defi_services.lending_pools.services.valas_state_service import ValasStateService
+from defi_services.lending_pools.lending_pools_info.fantom.geist_ftm import GEIST_ETH
+from defi_services.lending_pools.services.geist_state_service import GeistStateService
 
 
-class ValasService(DefiService):
+class GeistService(DefiService):
+    name = "geist lending pool"
+
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
-        self.state_service = ValasStateService(provider_uri)
+        self.state_service = GeistStateService(provider_uri)
         self.defi_constant = self._get_constant()
 
     def _get_constant(self):
-        if self.chain_id == Chain.bsc:
-            return VALAS_BSC
+        if self.chain_id == Chain.fantom:
+            return GEIST_ETH
         return None
 
     def get_apy_defi_app(self, block_number: int = "latest"):
         return self.state_service.get_apy_lending_pool(
             pool_address=self.defi_constant.get("address"),
             chef_incentive_address=self.defi_constant.get("chefIncentiveAddress"),
             oracle_address=self.defi_constant.get("oracleAddress"),
@@ -24,17 +26,19 @@
         )
 
     def get_rewards_balance(self, wallet_address: str, block_number: int = "latest"):
         return self.state_service.get_rewards_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
             multi_fee_address=self.defi_constant.get("multiFeeAddress"),
-            block_number=block_number
+            block_number=block_number,
+            reserves_info=self.defi_constant.get("reservesList")
         )
 
     def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest"):
         return self.state_service.get_wallet_deposit_borrow_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
             oracle_address=self.defi_constant.get("oracleAddress"),
-            block_number=block_number
-        )
+            block_number=block_number,
+            reserves_info=self.defi_constant.get("reservesList")
+        )
```

### Comparing `defi-services-lib-1.0.3/src/defi_services/lending_pools/venus_service.py` & `defi-services-lib-1.0.4/src/defi_services/lending_pools/venus_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from defi_services.constants.chain_constant import Chain
 from defi_services.defi_service import DefiService
 from defi_services.lending_pools.lending_pools_info.bsc.venus_bsc import VENUS_BSC
 from defi_services.lending_pools.services.venus_state_service import VenusStateService
 
 
 class VenusService(DefiService):
+    name = "venus lending pool"
+
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
         self.state_service = VenusStateService(provider_uri)
         self.defi_constant = self._get_constant()
 
     def _get_constant(self):
         if self.chain_id == Chain.bsc:
@@ -36,9 +38,10 @@
         )
 
     def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest"):
         return self.state_service.get_wallet_deposit_borrow_balance(
             wallet_address=wallet_address,
             lens_address=self.defi_constant.get("lensAddress"),
             reserves_info=self.defi_constant.get("reservesList"),
-            block_number=block_number
+            block_number=block_number,
+            wrapped_native_token=self.get_wrapped_native_token()
         )
```

### Comparing `defi-services-lib-1.0.3/src/defi_services/state_service.py` & `defi-services-lib-1.0.4/src/defi_services/state_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 from query_state_lib.client.client_querier import ClientQuerier
 from web3 import Web3
 from web3.middleware import geth_poa_middleware
 from defi_services.abis.erc20_abi import ERC20_ABI
+from defi_services.constants.chain_constant import Chain
+from defi_services.constants.contract_address import WrappedNativeTokens
 from defi_services.utils.batch_queries_service import add_rpc_call, decode_data_response
 from defi_services.utils.graph_operations import BlockTimestampGraph, GraphOperations
 from defi_services.utils.market_service import MarketService
 from defi_services.utils.memory_storage import MemoryStorage
 
 _LOGGER = logging.getLogger("StateService")
 
@@ -79,8 +81,8 @@
         data_response = self.client_querier.sent_batch_to_provider(list_rpc_call, batch_size=100)
         decoded_data = decode_data_response(data_response, list_call_id)
         result = {}
         for token_address in token_addresses:
             total_supply_call_id = f'totalSupply_{token_address}_{block_number}'.lower()
             result[token_address.lower()] = decoded_data.get(total_supply_call_id)
 
-        return result
+        return result
```

### Comparing `defi-services-lib-1.0.3/src/defi_services/utils/batch_queries_service.py` & `defi-services-lib-1.0.4/src/defi_services/utils/batch_queries_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/utils/graph_operations.py` & `defi-services-lib-1.0.4/src/defi_services/utils/graph_operations.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/utils/market_service.py` & `defi-services-lib-1.0.4/src/defi_services/utils/market_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services/utils/memory_storage.py` & `defi-services-lib-1.0.4/src/defi_services/utils/memory_storage.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.3/src/defi_services_lib.egg-info/PKG-INFO` & `defi-services-lib-1.0.4/src/defi_services_lib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defi-services-lib
-Version: 1.0.3
+Version: 1.0.4
 Summary: Calculate apy, apr, and wallet information,... in decentralized applications.
 Home-page: https://github.com/phamvietbang/defi-services-lib
 Author: Viet-Bang Pham
 Author-email: phamvietbang2965@gmail.com
 Project-URL: Bug Tracker, https://github.com/phamvietbang/defi-services-lib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

