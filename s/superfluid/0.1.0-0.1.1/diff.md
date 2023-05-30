# Comparing `tmp/superfluid-0.1.0.tar.gz` & `tmp/superfluid-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superfluid-0.1.0.tar", last modified: Mon May 29 13:16:39 2023, max compression
+gzip compressed data, was "superfluid-0.1.1.tar", last modified: Tue May 30 14:37:13 2023, max compression
```

## Comparing `superfluid-0.1.0.tar` & `superfluid-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-29 13:16:39.536205 superfluid-0.1.0/
--rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.1.0/LICENSE.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)     2778 2023-05-29 13:16:39.536013 superfluid-0.1.0/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)     2289 2023-05-29 13:15:16.000000 superfluid-0.1.0/README.md
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-29 13:16:39.527794 superfluid-0.1.0/main/
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-29 13:16:39.528425 superfluid-0.1.0/main/superfluid/
--rw-r--r--   0 godspowereze   (501) staff       (20)      166 2023-05-29 13:16:23.000000 superfluid-0.1.0/main/superfluid/__init__.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-29 13:16:39.535045 superfluid-0.1.0/main/superfluid/src/
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:15:40.000000 superfluid-0.1.0/main/superfluid/src/__init__.py
--rw-r--r--   0 godspowereze   (501) staff       (20)    21996 2023-05-29 12:34:47.000000 superfluid-0.1.0/main/superfluid/src/cfa.py
--rw-r--r--   0 godspowereze   (501) staff       (20)      770 2023-05-29 13:11:06.000000 superfluid-0.1.0/main/superfluid/src/constants.py
--rw-r--r--   0 godspowereze   (501) staff       (20)      335 2023-05-29 08:52:33.000000 superfluid-0.1.0/main/superfluid/src/errors.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1022 2023-05-29 10:12:39.000000 superfluid-0.1.0/main/superfluid/src/host.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1956 2023-05-29 10:02:53.000000 superfluid-0.1.0/main/superfluid/src/operation.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     9946 2023-05-29 11:15:00.000000 superfluid-0.1.0/main/superfluid/src/types.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1513 2023-05-29 10:10:55.000000 superfluid-0.1.0/main/superfluid/src/utils.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-29 13:16:39.535599 superfluid-0.1.0/main/superfluid/test/
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-26 06:50:05.000000 superfluid-0.1.0/main/superfluid/test/__init__.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     5324 2023-05-29 09:57:23.000000 superfluid-0.1.0/main/superfluid/test/test_utils.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-29 13:16:39.533238 superfluid-0.1.0/main/superfluid.egg-info/
--rw-r--r--   0 godspowereze   (501) staff       (20)     2778 2023-05-29 13:16:39.000000 superfluid-0.1.0/main/superfluid.egg-info/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)      561 2023-05-29 13:16:39.000000 superfluid-0.1.0/main/superfluid.egg-info/SOURCES.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-29 13:16:39.000000 superfluid-0.1.0/main/superfluid.egg-info/dependency_links.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       53 2023-05-29 13:16:39.000000 superfluid-0.1.0/main/superfluid.egg-info/requires.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       11 2023-05-29 13:16:39.000000 superfluid-0.1.0/main/superfluid.egg-info/top_level.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-29 13:16:39.536251 superfluid-0.1.0/setup.cfg
--rw-r--r--   0 godspowereze   (501) staff       (20)      848 2023-05-29 13:05:31.000000 superfluid-0.1.0/setup.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 14:37:13.541862 superfluid-0.1.1/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.1.1/LICENSE.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2828 2023-05-30 14:37:13.541692 superfluid-0.1.1/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2339 2023-05-29 13:17:14.000000 superfluid-0.1.1/README.md
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 14:37:13.533670 superfluid-0.1.1/main/
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 14:37:13.534461 superfluid-0.1.1/main/superfluid/
+-rw-r--r--   0 godspowereze   (501) staff       (20)      166 2023-05-29 13:16:23.000000 superfluid-0.1.1/main/superfluid/__init__.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 14:37:13.539384 superfluid-0.1.1/main/superfluid/src/
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:15:40.000000 superfluid-0.1.1/main/superfluid/src/__init__.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 14:37:13.541078 superfluid-0.1.1/main/superfluid/src/abis/
+-rw-r--r--   0 godspowereze   (501) staff       (20)        0 2023-05-30 14:33:15.000000 superfluid-0.1.1/main/superfluid/src/abis/__init__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)    21996 2023-05-29 12:34:47.000000 superfluid-0.1.1/main/superfluid/src/cfa.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      700 2023-05-30 14:37:08.000000 superfluid-0.1.1/main/superfluid/src/constants.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      335 2023-05-29 08:52:33.000000 superfluid-0.1.1/main/superfluid/src/errors.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1022 2023-05-29 10:12:39.000000 superfluid-0.1.1/main/superfluid/src/host.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 14:37:13.541211 superfluid-0.1.1/main/superfluid/src/metadata/
+-rw-r--r--   0 godspowereze   (501) staff       (20)        0 2023-05-30 14:33:31.000000 superfluid-0.1.1/main/superfluid/src/metadata/__init__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1956 2023-05-29 10:02:53.000000 superfluid-0.1.1/main/superfluid/src/operation.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     9946 2023-05-29 11:15:00.000000 superfluid-0.1.1/main/superfluid/src/types.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1513 2023-05-29 10:10:55.000000 superfluid-0.1.1/main/superfluid/src/utils.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 14:37:13.541467 superfluid-0.1.1/main/superfluid/test/
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-26 06:50:05.000000 superfluid-0.1.1/main/superfluid/test/__init__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     5324 2023-05-29 09:57:23.000000 superfluid-0.1.1/main/superfluid/test/test_utils.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 14:37:13.536044 superfluid-0.1.1/main/superfluid.egg-info/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2828 2023-05-30 14:37:13.000000 superfluid-0.1.1/main/superfluid.egg-info/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)      639 2023-05-30 14:37:13.000000 superfluid-0.1.1/main/superfluid.egg-info/SOURCES.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-30 14:37:13.000000 superfluid-0.1.1/main/superfluid.egg-info/dependency_links.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       53 2023-05-30 14:37:13.000000 superfluid-0.1.1/main/superfluid.egg-info/requires.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       11 2023-05-30 14:37:13.000000 superfluid-0.1.1/main/superfluid.egg-info/top_level.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-30 14:37:13.541927 superfluid-0.1.1/setup.cfg
+-rw-r--r--   0 godspowereze   (501) staff       (20)      848 2023-05-30 14:30:40.000000 superfluid-0.1.1/setup.py
```

### Comparing `superfluid-0.1.0/LICENSE.txt` & `superfluid-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.0/PKG-INFO` & `superfluid-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -57,14 +57,15 @@
 pip install superfluid
 ```
 
 # Usage
 
 ```python
 from superfluid import CFA_V1
+from superfluid import Web3FlowInfo
 
 rpc: str = "YOUR PREFERRED RPC"
 chain_id: int = "CHAIN ID"
 
 ######################################################
 ###### CONSTANT FLOW AGREEMENT OPERATIONS ###########
 ######################################################
@@ -75,15 +76,15 @@
 sender: str = "SENDER ADDRESS"
 receiver: str = "RECEIVER ADDRESS"
 flow_rate: int = "FLOW RATE"
 
 PRIVATE_KEY: str = "YOUR PRIVATE KEY"
 OPERATOR_PRIVATE_KEY: str = "OPERATOR PRIVATE KEY"
 
-flow_data = cfaV1Instance.get_flow(super_token, sender, receiver)
+flow_data: Web3FlowInfo = cfaV1Instance.get_flow(super_token, sender, receiver)
 
 create_flow_operation = cfaV1Instance.create_flow(
     sender, receiver, super_token, flow_rate)
 transaction_hash = create_flow_operation.exec(PRIVATE_KEY)
 
 update_flow_operation = cfaV1Instance.update_flow(
     sender, receiver, super_token, flow_rate)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.1.0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.1.1 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
         ****** Welcome to Superfluid Python SDK(Unofficial) ð ******
@@ -12,23 +12,23 @@
 //app.superfluid.finance/) ### ð [Docs](https://docs.superfluid.finance)  #
 Introduction superfluid.py is an application framework for interacting with the
 Superfluid Protocol without the Python Programming Language. # Features *
 Minimal Framework initialization (`rpc` and `chain id`) * New Operation syntax
 for transactions * Read/Create/Update/Delete Agreement Operations (Constant
 Flow Agreement and Instant Distribution Agreement(In development)) # Notable
 Used Technologies * Python * Web3.py # Installation ```bash pip install
-superfluid ``` # Usage ```python from superfluid import CFA_V1 rpc: str = "YOUR
-PREFERRED RPC" chain_id: int = "CHAIN ID"
+superfluid ``` # Usage ```python from superfluid import CFA_V1 from superfluid
+import Web3FlowInfo rpc: str = "YOUR PREFERRED RPC" chain_id: int = "CHAIN ID"
 ###################################################### ###### CONSTANT FLOW
 AGREEMENT OPERATIONS ###########
 ###################################################### cfaV1Instance = CFA_V1
 (rpc, chain_id) super_token: str = "SUPER TOKEN ADDRESS" sender: str = "SENDER
 ADDRESS" receiver: str = "RECEIVER ADDRESS" flow_rate: int = "FLOW RATE"
 PRIVATE_KEY: str = "YOUR PRIVATE KEY" OPERATOR_PRIVATE_KEY: str = "OPERATOR
-PRIVATE KEY" flow_data = cfaV1Instance.get_flow(super_token, sender, receiver)
-create_flow_operation = cfaV1Instance.create_flow( sender, receiver,
-super_token, flow_rate) transaction_hash = create_flow_operation.exec
+PRIVATE KEY" flow_data: Web3FlowInfo = cfaV1Instance.get_flow(super_token,
+sender, receiver) create_flow_operation = cfaV1Instance.create_flow( sender,
+receiver, super_token, flow_rate) transaction_hash = create_flow_operation.exec
 (PRIVATE_KEY) update_flow_operation = cfaV1Instance.update_flow( sender,
 receiver, super_token, flow_rate) transaction_hash = update_flow_operation.exec
 (PRIVATE_KEY) delete_flow_operation = cfaV1Instance.delete_flow( sender,
 receiver, super_token) transaction_hash = delete_flow_operation.exec
 (PRIVATE_KEY) ```
```

### Comparing `superfluid-0.1.0/README.md` & `superfluid-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 pip install superfluid
 ```
 
 # Usage
 
 ```python
 from superfluid import CFA_V1
+from superfluid import Web3FlowInfo
 
 rpc: str = "YOUR PREFERRED RPC"
 chain_id: int = "CHAIN ID"
 
 ######################################################
 ###### CONSTANT FLOW AGREEMENT OPERATIONS ###########
 ######################################################
@@ -59,15 +60,15 @@
 sender: str = "SENDER ADDRESS"
 receiver: str = "RECEIVER ADDRESS"
 flow_rate: int = "FLOW RATE"
 
 PRIVATE_KEY: str = "YOUR PRIVATE KEY"
 OPERATOR_PRIVATE_KEY: str = "OPERATOR PRIVATE KEY"
 
-flow_data = cfaV1Instance.get_flow(super_token, sender, receiver)
+flow_data: Web3FlowInfo = cfaV1Instance.get_flow(super_token, sender, receiver)
 
 create_flow_operation = cfaV1Instance.create_flow(
     sender, receiver, super_token, flow_rate)
 transaction_hash = create_flow_operation.exec(PRIVATE_KEY)
 
 update_flow_operation = cfaV1Instance.update_flow(
     sender, receiver, super_token, flow_rate)
```

#### html2text {}

```diff
@@ -5,23 +5,23 @@
 //app.superfluid.finance/) ### ð [Docs](https://docs.superfluid.finance)  #
 Introduction superfluid.py is an application framework for interacting with the
 Superfluid Protocol without the Python Programming Language. # Features *
 Minimal Framework initialization (`rpc` and `chain id`) * New Operation syntax
 for transactions * Read/Create/Update/Delete Agreement Operations (Constant
 Flow Agreement and Instant Distribution Agreement(In development)) # Notable
 Used Technologies * Python * Web3.py # Installation ```bash pip install
-superfluid ``` # Usage ```python from superfluid import CFA_V1 rpc: str = "YOUR
-PREFERRED RPC" chain_id: int = "CHAIN ID"
+superfluid ``` # Usage ```python from superfluid import CFA_V1 from superfluid
+import Web3FlowInfo rpc: str = "YOUR PREFERRED RPC" chain_id: int = "CHAIN ID"
 ###################################################### ###### CONSTANT FLOW
 AGREEMENT OPERATIONS ###########
 ###################################################### cfaV1Instance = CFA_V1
 (rpc, chain_id) super_token: str = "SUPER TOKEN ADDRESS" sender: str = "SENDER
 ADDRESS" receiver: str = "RECEIVER ADDRESS" flow_rate: int = "FLOW RATE"
 PRIVATE_KEY: str = "YOUR PRIVATE KEY" OPERATOR_PRIVATE_KEY: str = "OPERATOR
-PRIVATE KEY" flow_data = cfaV1Instance.get_flow(super_token, sender, receiver)
-create_flow_operation = cfaV1Instance.create_flow( sender, receiver,
-super_token, flow_rate) transaction_hash = create_flow_operation.exec
+PRIVATE KEY" flow_data: Web3FlowInfo = cfaV1Instance.get_flow(super_token,
+sender, receiver) create_flow_operation = cfaV1Instance.create_flow( sender,
+receiver, super_token, flow_rate) transaction_hash = create_flow_operation.exec
 (PRIVATE_KEY) update_flow_operation = cfaV1Instance.update_flow( sender,
 receiver, super_token, flow_rate) transaction_hash = update_flow_operation.exec
 (PRIVATE_KEY) delete_flow_operation = cfaV1Instance.delete_flow( sender,
 receiver, super_token) transaction_hash = delete_flow_operation.exec
 (PRIVATE_KEY) ```
```

### Comparing `superfluid-0.1.0/main/superfluid/src/cfa.py` & `superfluid-0.1.1/main/superfluid/src/cfa.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.0/main/superfluid/src/constants.py` & `superfluid-0.1.1/main/superfluid/src/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import json
+import os
 
-with open("./main/superfluid/src/abis/cfa_v1.json") as cfa_v1:
+with open("./abis/cfa_v1.json") as cfa_v1:
     cfa_v1_abi = cfa_v1.read()
 
 CFA_V1_ABI = json.loads(cfa_v1_abi)
 
-with open("./main/superfluid/src/abis/cfa_v1_forwarder.json") as cfa_v1_forwarder:
+with open("./abis/cfa_v1_forwarder.json") as cfa_v1_forwarder:
     cfa_v1_forwarder_abi = cfa_v1_forwarder.read()
 
 CFA_V1_FORWARDER_ABI = json.loads(cfa_v1_forwarder_abi)
 
-with open("./main/superfluid/src/abis/host.json") as host:
+with open("./abis/host.json") as host:
     host_abi = host.read()
 
 HOST_ABI = json.loads(host_abi)
 
-with open("./main/superfluid/src/metadata/networks.json") as networks:
+with open("./metadata/networks.json") as networks:
     networks = networks.read()
 
 NETWORKS = json.loads(networks)
 
 """
 ------- ACL AUTHORIZATION BIT OPERATIONS -------
 """
```

### Comparing `superfluid-0.1.0/main/superfluid/src/host.py` & `superfluid-0.1.1/main/superfluid/src/host.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.0/main/superfluid/src/operation.py` & `superfluid-0.1.1/main/superfluid/src/operation.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.0/main/superfluid/src/types.py` & `superfluid-0.1.1/main/superfluid/src/types.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.0/main/superfluid/src/utils.py` & `superfluid-0.1.1/main/superfluid/src/utils.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.0/main/superfluid/test/test_utils.py` & `superfluid-0.1.1/main/superfluid/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.0/main/superfluid.egg-info/PKG-INFO` & `superfluid-0.1.1/main/superfluid.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -57,14 +57,15 @@
 pip install superfluid
 ```
 
 # Usage
 
 ```python
 from superfluid import CFA_V1
+from superfluid import Web3FlowInfo
 
 rpc: str = "YOUR PREFERRED RPC"
 chain_id: int = "CHAIN ID"
 
 ######################################################
 ###### CONSTANT FLOW AGREEMENT OPERATIONS ###########
 ######################################################
@@ -75,15 +76,15 @@
 sender: str = "SENDER ADDRESS"
 receiver: str = "RECEIVER ADDRESS"
 flow_rate: int = "FLOW RATE"
 
 PRIVATE_KEY: str = "YOUR PRIVATE KEY"
 OPERATOR_PRIVATE_KEY: str = "OPERATOR PRIVATE KEY"
 
-flow_data = cfaV1Instance.get_flow(super_token, sender, receiver)
+flow_data: Web3FlowInfo = cfaV1Instance.get_flow(super_token, sender, receiver)
 
 create_flow_operation = cfaV1Instance.create_flow(
     sender, receiver, super_token, flow_rate)
 transaction_hash = create_flow_operation.exec(PRIVATE_KEY)
 
 update_flow_operation = cfaV1Instance.update_flow(
     sender, receiver, super_token, flow_rate)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.1.0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.1.1 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
         ****** Welcome to Superfluid Python SDK(Unofficial) ð ******
@@ -12,23 +12,23 @@
 //app.superfluid.finance/) ### ð [Docs](https://docs.superfluid.finance)  #
 Introduction superfluid.py is an application framework for interacting with the
 Superfluid Protocol without the Python Programming Language. # Features *
 Minimal Framework initialization (`rpc` and `chain id`) * New Operation syntax
 for transactions * Read/Create/Update/Delete Agreement Operations (Constant
 Flow Agreement and Instant Distribution Agreement(In development)) # Notable
 Used Technologies * Python * Web3.py # Installation ```bash pip install
-superfluid ``` # Usage ```python from superfluid import CFA_V1 rpc: str = "YOUR
-PREFERRED RPC" chain_id: int = "CHAIN ID"
+superfluid ``` # Usage ```python from superfluid import CFA_V1 from superfluid
+import Web3FlowInfo rpc: str = "YOUR PREFERRED RPC" chain_id: int = "CHAIN ID"
 ###################################################### ###### CONSTANT FLOW
 AGREEMENT OPERATIONS ###########
 ###################################################### cfaV1Instance = CFA_V1
 (rpc, chain_id) super_token: str = "SUPER TOKEN ADDRESS" sender: str = "SENDER
 ADDRESS" receiver: str = "RECEIVER ADDRESS" flow_rate: int = "FLOW RATE"
 PRIVATE_KEY: str = "YOUR PRIVATE KEY" OPERATOR_PRIVATE_KEY: str = "OPERATOR
-PRIVATE KEY" flow_data = cfaV1Instance.get_flow(super_token, sender, receiver)
-create_flow_operation = cfaV1Instance.create_flow( sender, receiver,
-super_token, flow_rate) transaction_hash = create_flow_operation.exec
+PRIVATE KEY" flow_data: Web3FlowInfo = cfaV1Instance.get_flow(super_token,
+sender, receiver) create_flow_operation = cfaV1Instance.create_flow( sender,
+receiver, super_token, flow_rate) transaction_hash = create_flow_operation.exec
 (PRIVATE_KEY) update_flow_operation = cfaV1Instance.update_flow( sender,
 receiver, super_token, flow_rate) transaction_hash = update_flow_operation.exec
 (PRIVATE_KEY) delete_flow_operation = cfaV1Instance.delete_flow( sender,
 receiver, super_token) transaction_hash = delete_flow_operation.exec
 (PRIVATE_KEY) ```
```

### Comparing `superfluid-0.1.0/main/superfluid.egg-info/SOURCES.txt` & `superfluid-0.1.1/main/superfluid.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -11,9 +11,11 @@
 main/superfluid/src/cfa.py
 main/superfluid/src/constants.py
 main/superfluid/src/errors.py
 main/superfluid/src/host.py
 main/superfluid/src/operation.py
 main/superfluid/src/types.py
 main/superfluid/src/utils.py
+main/superfluid/src/abis/__init__.py
+main/superfluid/src/metadata/__init__.py
 main/superfluid/test/__init__.py
 main/superfluid/test/test_utils.py
```

### Comparing `superfluid-0.1.0/setup.py` & `superfluid-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="superfluid",
-    version="0.1.0",
+    version="0.1.1",
     description="Python SDK for the Superfluid Protocol",
     package_dir={"": "main"},
     packages=find_packages(where="main"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Godspower-Eze/superfluid.py",
     author="Godspower-Eze",
```

