# Comparing `tmp/dexie_rewards-0.0.8.tar.gz` & `tmp/dexie_rewards-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexie_rewards-0.0.8.tar", max compression
+gzip compressed data, was "dexie_rewards-1.8.0.tar", max compression
```

## Comparing `dexie_rewards-0.0.8.tar` & `dexie_rewards-1.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-0.0.8/LICENSE
--rw-r--r--   0        0        0     5641 2023-05-26 14:42:14.551472 dexie_rewards-0.0.8/README.md
--rw-r--r--   0        0        0      768 2023-05-26 14:46:27.159293 dexie_rewards-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-0.0.8/src/dexie_rewards/__init__.py
--rw-r--r--   0        0        0     1126 2023-05-13 02:26:45.947358 dexie_rewards-0.0.8/src/dexie_rewards/config.py
--rw-r--r--   0        0        0      822 2023-05-12 12:18:23.796037 dexie_rewards-0.0.8/src/dexie_rewards/decorators/with_db_connection.py
--rw-r--r--   0        0        0     1207 2023-05-11 04:12:56.210275 dexie_rewards-0.0.8/src/dexie_rewards/decorators/with_wallet_rpc_client.py
--rw-r--r--   0        0        0      234 2023-05-08 10:51:08.009870 dexie_rewards-0.0.8/src/dexie_rewards/main.py
--rw-r--r--   0        0        0     3505 2023-05-13 03:54:19.525074 dexie_rewards-0.0.8/src/dexie_rewards/rewards/claim.py
--rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.188725 dexie_rewards-0.0.8/src/dexie_rewards/rewards/list.py
--rw-r--r--   0        0        0      272 2023-05-08 10:18:31.545940 dexie_rewards-0.0.8/src/dexie_rewards/rewards/main.py
--rw-r--r--   0        0        0     4791 2023-05-19 15:21:53.340874 dexie_rewards-0.0.8/src/dexie_rewards/rewards/utils.py
--rw-r--r--   0        0        0     2294 2023-05-19 15:21:53.341294 dexie_rewards-0.0.8/src/dexie_rewards/services/dexie_api.py
--rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.828154 dexie_rewards-0.0.8/src/dexie_rewards/services/dexie_db.py
--rw-r--r--   0        0        0     1759 2023-05-26 14:42:14.553106 dexie_rewards-0.0.8/src/dexie_rewards/services/wallet_rpc_client.py
--rw-r--r--   0        0        0      801 2023-05-16 00:41:08.479451 dexie_rewards-0.0.8/src/dexie_rewards/types/offer_reward.py
--rw-r--r--   0        0        0      229 2023-05-09 11:06:14.984159 dexie_rewards-0.0.8/src/dexie_rewards/types/utils.py
--rw-r--r--   0        0        0     1851 2023-05-12 13:28:19.018840 dexie_rewards-0.0.8/src/dexie_rewards/utils.py
--rw-r--r--   0        0        0     6396 1970-01-01 00:00:00.000000 dexie_rewards-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 14:18:44.184005 dexie_rewards-1.8.0/LICENSE
+-rw-r--r--   0        0        0     5648 2023-05-30 14:22:56.660449 dexie_rewards-1.8.0/README.md
+-rw-r--r--   0        0        0      796 2023-05-30 14:22:07.469088 dexie_rewards-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-30 14:18:44.186020 dexie_rewards-1.8.0/src/dexie_rewards/__init__.py
+-rw-r--r--   0        0        0     1126 2023-05-30 14:18:44.186139 dexie_rewards-1.8.0/src/dexie_rewards/config.py
+-rw-r--r--   0        0        0      822 2023-05-30 14:18:44.186320 dexie_rewards-1.8.0/src/dexie_rewards/decorators/with_db_connection.py
+-rw-r--r--   0        0        0     1207 2023-05-30 14:18:44.186442 dexie_rewards-1.8.0/src/dexie_rewards/decorators/with_wallet_rpc_client.py
+-rw-r--r--   0        0        0      234 2023-05-30 14:18:44.186544 dexie_rewards-1.8.0/src/dexie_rewards/main.py
+-rw-r--r--   0        0        0     3505 2023-05-30 14:18:44.186731 dexie_rewards-1.8.0/src/dexie_rewards/rewards/claim.py
+-rw-r--r--   0        0        0     1921 2023-05-30 14:18:44.186863 dexie_rewards-1.8.0/src/dexie_rewards/rewards/list.py
+-rw-r--r--   0        0        0      272 2023-05-30 14:18:44.186965 dexie_rewards-1.8.0/src/dexie_rewards/rewards/main.py
+-rw-r--r--   0        0        0     4791 2023-05-30 14:18:44.187119 dexie_rewards-1.8.0/src/dexie_rewards/rewards/utils.py
+-rw-r--r--   0        0        0     2294 2023-05-30 14:18:44.187307 dexie_rewards-1.8.0/src/dexie_rewards/services/dexie_api.py
+-rw-r--r--   0        0        0     3756 2023-05-30 14:18:44.187448 dexie_rewards-1.8.0/src/dexie_rewards/services/dexie_db.py
+-rw-r--r--   0        0        0     1759 2023-05-30 14:18:44.187557 dexie_rewards-1.8.0/src/dexie_rewards/services/wallet_rpc_client.py
+-rw-r--r--   0        0        0      801 2023-05-30 14:18:44.187717 dexie_rewards-1.8.0/src/dexie_rewards/types/offer_reward.py
+-rw-r--r--   0        0        0      229 2023-05-30 14:18:44.187821 dexie_rewards-1.8.0/src/dexie_rewards/types/utils.py
+-rw-r--r--   0        0        0     1851 2023-05-30 14:18:44.187935 dexie_rewards-1.8.0/src/dexie_rewards/utils.py
+-rw-r--r--   0        0        0     6431 1970-01-01 00:00:00.000000 dexie_rewards-1.8.0/PKG-INFO
```

### Comparing `dexie_rewards-0.0.8/LICENSE` & `dexie_rewards-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.8/README.md` & `dexie_rewards-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Auto-Claim dexie rewards
 
 [![PyPI version](https://badge.fury.io/py/dexie-rewards.svg)](https://badge.fury.io/py/dexie-rewards)
 [![Python version](https://img.shields.io/pypi/pyversions/dexie-rewards.svg)](https://pypi.python.org/pypi/dexie-rewards)
 
-dexie-rewards is a Python CLI helper tool designed automatically claim [dexie liquidity rewards](https://dexie.space/incentives) for offers created using the official Chia Wallet. The tool communicates locally with the Chia Wallet RPC, requests all created offers, and checks them for claimable rewards.
+dexie-rewards is a Python CLI helper tool designed automatically to claim [dexie liquidity rewards](https://dexie.space/incentives) for offers created using the official Chia Wallet. The tool communicates locally with the Chia Wallet RPC, requests all created offers, and checks them for claimable rewards.
 
 When rewards are claimed, a message from the input (maker) address of the offer is signed to prove ownership of the offer. The signature is then sent to dexie to claim the rewards. dexie distributes claimed rewards to the input (maker) address in batches approximately every 15 minutes.
 
 ## Example Output
 
 ```
 ❯ dexie rewards claim
@@ -30,14 +30,15 @@
 It is recommended to install dexie-rewards using pip.
 
 ### Install via pip
 
 ```sh
 pip install dexie-rewards
 ```
+
 Note for macOS: If `pip` is not found, try `pip3` instead.
 
 ### Install from the repository (optional)
 
 1. Clone the repository
 
 ```sh
@@ -71,24 +72,26 @@
 ## Available Commands
 
 Make sure that your Chia wallet is running and fully synced before using dexie-rewards. A full node is not required.
 
 Run any command with the `--help` option to see all available functionality.
 
 ### List offers with outstanding (claimable) rewards
+
 ```
 ❯ dexie rewards list
 
   --fingerprint  -f        Set the fingerprint to specify which wallet to use
   --json         -j        Displays offers as JSON
   --verbose      -v        Display verbose output
   --help                   Show help and exit
 ```
 
 ### Claim all outstanding (claimable) rewards
+
 ```
 ❯ dexie rewards claim
 
   --fingerprint  -f         Set the fingerprint to specify which wallet to use
   --verify-only  -vo        Only verify the claim, don't actually claim
   --yes          -y         Skip claim confirmation
   --verbose      -v         Display verbose output
@@ -115,8 +118,8 @@
 
 ## Alternatives
 
 Advanced market makers may develop their own tools for claiming liquidity rewards. Refer to the [dexie API documentation](https://dexie.space/api) for information on how to claim rewards for offers using the API.
 
 ## Contributions
 
-Contributions are welcome and encouraged. Please fork the repository and submit a pull request to the `main` branch. If you have any questions, feel free to reach out to us on [Discord](https://discord.gg/3xUrkAxUmd).
+Contributions are welcome and encouraged. Please fork the repository and submit a pull request to the `main` branch. If you have any questions, feel free to reach out to us on [Discord](https://discord.gg/3xUrkAxUmd).
```

### Comparing `dexie_rewards-0.0.8/pyproject.toml` & `dexie_rewards-1.8.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dexie-rewards"
-version = "0.0.8"
-description = "An open source Python tool which runs locally and will automatically claim rewards for all your created offers on dexie."
+version = "1.8.0"
+description = "dexie-rewards is a Python CLI helper tool designed automatically to claim dexie liquidity rewards for offers created using the official Chia Wallet."
 authors = ["Dexie Contributors <pypi@dexie.space>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "dexie_rewards", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dexie_rewards-0.0.8/src/dexie_rewards/config.py` & `dexie_rewards-1.8.0/src/dexie_rewards/config.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.8/src/dexie_rewards/decorators/with_db_connection.py` & `dexie_rewards-1.8.0/src/dexie_rewards/decorators/with_db_connection.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.8/src/dexie_rewards/decorators/with_wallet_rpc_client.py` & `dexie_rewards-1.8.0/src/dexie_rewards/decorators/with_wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.8/src/dexie_rewards/rewards/claim.py` & `dexie_rewards-1.8.0/src/dexie_rewards/rewards/claim.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.8/src/dexie_rewards/rewards/list.py` & `dexie_rewards-1.8.0/src/dexie_rewards/rewards/list.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.8/src/dexie_rewards/rewards/utils.py` & `dexie_rewards-1.8.0/src/dexie_rewards/rewards/utils.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.8/src/dexie_rewards/services/dexie_api.py` & `dexie_rewards-1.8.0/src/dexie_rewards/services/dexie_api.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.8/src/dexie_rewards/services/dexie_db.py` & `dexie_rewards-1.8.0/src/dexie_rewards/services/dexie_db.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.8/src/dexie_rewards/services/wallet_rpc_client.py` & `dexie_rewards-1.8.0/src/dexie_rewards/services/wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.8/src/dexie_rewards/types/offer_reward.py` & `dexie_rewards-1.8.0/src/dexie_rewards/types/offer_reward.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.8/src/dexie_rewards/utils.py` & `dexie_rewards-1.8.0/src/dexie_rewards/utils.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.8/PKG-INFO` & `dexie_rewards-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dexie-rewards
-Version: 0.0.8
-Summary: An open source Python tool which runs locally and will automatically claim rewards for all your created offers on dexie.
+Version: 1.8.0
+Summary: dexie-rewards is a Python CLI helper tool designed automatically to claim dexie liquidity rewards for offers created using the official Chia Wallet.
 License: Apache-2.0
 Author: Dexie Contributors
 Author-email: pypi@dexie.space
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 
 # Auto-Claim dexie rewards
 
 [![PyPI version](https://badge.fury.io/py/dexie-rewards.svg)](https://badge.fury.io/py/dexie-rewards)
 [![Python version](https://img.shields.io/pypi/pyversions/dexie-rewards.svg)](https://pypi.python.org/pypi/dexie-rewards)
 
-dexie-rewards is a Python CLI helper tool designed automatically claim [dexie liquidity rewards](https://dexie.space/incentives) for offers created using the official Chia Wallet. The tool communicates locally with the Chia Wallet RPC, requests all created offers, and checks them for claimable rewards.
+dexie-rewards is a Python CLI helper tool designed automatically to claim [dexie liquidity rewards](https://dexie.space/incentives) for offers created using the official Chia Wallet. The tool communicates locally with the Chia Wallet RPC, requests all created offers, and checks them for claimable rewards.
 
 When rewards are claimed, a message from the input (maker) address of the offer is signed to prove ownership of the offer. The signature is then sent to dexie to claim the rewards. dexie distributes claimed rewards to the input (maker) address in batches approximately every 15 minutes.
 
 ## Example Output
 
 ```
 ❯ dexie rewards claim
@@ -49,14 +49,15 @@
 It is recommended to install dexie-rewards using pip.
 
 ### Install via pip
 
 ```sh
 pip install dexie-rewards
 ```
+
 Note for macOS: If `pip` is not found, try `pip3` instead.
 
 ### Install from the repository (optional)
 
 1. Clone the repository
 
 ```sh
@@ -90,24 +91,26 @@
 ## Available Commands
 
 Make sure that your Chia wallet is running and fully synced before using dexie-rewards. A full node is not required.
 
 Run any command with the `--help` option to see all available functionality.
 
 ### List offers with outstanding (claimable) rewards
+
 ```
 ❯ dexie rewards list
 
   --fingerprint  -f        Set the fingerprint to specify which wallet to use
   --json         -j        Displays offers as JSON
   --verbose      -v        Display verbose output
   --help                   Show help and exit
 ```
 
 ### Claim all outstanding (claimable) rewards
+
 ```
 ❯ dexie rewards claim
 
   --fingerprint  -f         Set the fingerprint to specify which wallet to use
   --verify-only  -vo        Only verify the claim, don't actually claim
   --yes          -y         Skip claim confirmation
   --verbose      -v         Display verbose output
@@ -135,7 +138,8 @@
 ## Alternatives
 
 Advanced market makers may develop their own tools for claiming liquidity rewards. Refer to the [dexie API documentation](https://dexie.space/api) for information on how to claim rewards for offers using the API.
 
 ## Contributions
 
 Contributions are welcome and encouraged. Please fork the repository and submit a pull request to the `main` branch. If you have any questions, feel free to reach out to us on [Discord](https://discord.gg/3xUrkAxUmd).
+
```

