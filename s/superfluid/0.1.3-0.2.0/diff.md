# Comparing `tmp/superfluid-0.1.3.tar.gz` & `tmp/superfluid-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superfluid-0.1.3.tar", last modified: Tue May 30 15:02:59 2023, max compression
+gzip compressed data, was "superfluid-0.2.0.tar", last modified: Tue May 30 15:16:02 2023, max compression
```

## Comparing `superfluid-0.1.3.tar` & `superfluid-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:02:59.793001 superfluid-0.1.3/
--rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.1.3/LICENSE.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)     2828 2023-05-30 15:02:59.792882 superfluid-0.1.3/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)     2339 2023-05-29 13:17:14.000000 superfluid-0.1.3/README.md
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:02:59.790095 superfluid-0.1.3/main/
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:02:59.790844 superfluid-0.1.3/main/superfluid/
--rw-r--r--   0 godspowereze   (501) staff       (20)      166 2023-05-29 13:16:23.000000 superfluid-0.1.3/main/superfluid/__init__.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:02:59.792422 superfluid-0.1.3/main/superfluid/src/
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:15:40.000000 superfluid-0.1.3/main/superfluid/src/__init__.py
--rw-r--r--   0 godspowereze   (501) staff       (20)    21996 2023-05-29 12:34:47.000000 superfluid-0.1.3/main/superfluid/src/cfa.py
--rw-r--r--   0 godspowereze   (501) staff       (20)      812 2023-05-30 15:01:10.000000 superfluid-0.1.3/main/superfluid/src/constants.py
--rw-r--r--   0 godspowereze   (501) staff       (20)      335 2023-05-29 08:52:33.000000 superfluid-0.1.3/main/superfluid/src/errors.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1022 2023-05-29 10:12:39.000000 superfluid-0.1.3/main/superfluid/src/host.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1956 2023-05-29 10:02:53.000000 superfluid-0.1.3/main/superfluid/src/operation.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     9946 2023-05-29 11:15:00.000000 superfluid-0.1.3/main/superfluid/src/types.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1513 2023-05-29 10:10:55.000000 superfluid-0.1.3/main/superfluid/src/utils.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:02:59.792687 superfluid-0.1.3/main/superfluid/test/
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-26 06:50:05.000000 superfluid-0.1.3/main/superfluid/test/__init__.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     5324 2023-05-29 09:57:23.000000 superfluid-0.1.3/main/superfluid/test/test_utils.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:02:59.791407 superfluid-0.1.3/main/superfluid.egg-info/
--rw-r--r--   0 godspowereze   (501) staff       (20)     2828 2023-05-30 15:02:59.000000 superfluid-0.1.3/main/superfluid.egg-info/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)      561 2023-05-30 15:02:59.000000 superfluid-0.1.3/main/superfluid.egg-info/SOURCES.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-30 15:02:59.000000 superfluid-0.1.3/main/superfluid.egg-info/dependency_links.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       53 2023-05-30 15:02:59.000000 superfluid-0.1.3/main/superfluid.egg-info/requires.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       11 2023-05-30 15:02:59.000000 superfluid-0.1.3/main/superfluid.egg-info/top_level.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-30 15:02:59.793035 superfluid-0.1.3/setup.cfg
--rw-r--r--   0 godspowereze   (501) staff       (20)      848 2023-05-30 15:02:56.000000 superfluid-0.1.3/setup.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:16:02.538571 superfluid-0.2.0/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.2.0/LICENSE.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2777 2023-05-30 15:16:02.538234 superfluid-0.2.0/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2288 2023-05-30 15:14:04.000000 superfluid-0.2.0/README.md
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:16:02.534360 superfluid-0.2.0/main/
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:16:02.535050 superfluid-0.2.0/main/superfluid/
+-rw-r--r--   0 godspowereze   (501) staff       (20)      166 2023-05-29 13:16:23.000000 superfluid-0.2.0/main/superfluid/__init__.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:16:02.537016 superfluid-0.2.0/main/superfluid/src/
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:15:40.000000 superfluid-0.2.0/main/superfluid/src/__init__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)    50176 2023-05-30 15:06:49.000000 superfluid-0.2.0/main/superfluid/src/abis.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)    21996 2023-05-29 12:34:47.000000 superfluid-0.2.0/main/superfluid/src/cfa.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      430 2023-05-30 15:09:33.000000 superfluid-0.2.0/main/superfluid/src/constants.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      335 2023-05-29 08:52:33.000000 superfluid-0.2.0/main/superfluid/src/errors.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1022 2023-05-29 10:12:39.000000 superfluid-0.2.0/main/superfluid/src/host.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)    21807 2023-05-30 15:07:36.000000 superfluid-0.2.0/main/superfluid/src/metadata.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1956 2023-05-29 10:02:53.000000 superfluid-0.2.0/main/superfluid/src/operation.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     9946 2023-05-29 11:15:00.000000 superfluid-0.2.0/main/superfluid/src/types.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1513 2023-05-29 10:10:55.000000 superfluid-0.2.0/main/superfluid/src/utils.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:16:02.537522 superfluid-0.2.0/main/superfluid/test/
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-26 06:50:05.000000 superfluid-0.2.0/main/superfluid/test/__init__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     5324 2023-05-29 09:57:23.000000 superfluid-0.2.0/main/superfluid/test/test_utils.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:16:02.535763 superfluid-0.2.0/main/superfluid.egg-info/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2777 2023-05-30 15:16:02.000000 superfluid-0.2.0/main/superfluid.egg-info/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)      621 2023-05-30 15:16:02.000000 superfluid-0.2.0/main/superfluid.egg-info/SOURCES.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-30 15:16:02.000000 superfluid-0.2.0/main/superfluid.egg-info/dependency_links.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       53 2023-05-30 15:16:02.000000 superfluid-0.2.0/main/superfluid.egg-info/requires.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       11 2023-05-30 15:16:02.000000 superfluid-0.2.0/main/superfluid.egg-info/top_level.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-30 15:16:02.538784 superfluid-0.2.0/setup.cfg
+-rw-r--r--   0 godspowereze   (501) staff       (20)      848 2023-05-30 15:12:18.000000 superfluid-0.2.0/setup.py
```

### Comparing `superfluid-0.1.3/LICENSE.txt` & `superfluid-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.3/PKG-INFO` & `superfluid-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -74,15 +74,14 @@
 
 super_token: str = "SUPER TOKEN ADDRESS"
 sender: str = "SENDER ADDRESS"
 receiver: str = "RECEIVER ADDRESS"
 flow_rate: int = "FLOW RATE"
 
 PRIVATE_KEY: str = "YOUR PRIVATE KEY"
-OPERATOR_PRIVATE_KEY: str = "OPERATOR PRIVATE KEY"
 
 flow_data: Web3FlowInfo = cfaV1Instance.get_flow(super_token, sender, receiver)
 
 create_flow_operation = cfaV1Instance.create_flow(
     sender, receiver, super_token, flow_rate)
 transaction_hash = create_flow_operation.exec(PRIVATE_KEY)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.1.3 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.2.0 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
         ****** Welcome to Superfluid Python SDK(Unofficial) ð ******
@@ -19,16 +19,16 @@
 superfluid ``` # Usage ```python from superfluid import CFA_V1 from superfluid
 import Web3FlowInfo rpc: str = "YOUR PREFERRED RPC" chain_id: int = "CHAIN ID"
 ###################################################### ###### CONSTANT FLOW
 AGREEMENT OPERATIONS ###########
 ###################################################### cfaV1Instance = CFA_V1
 (rpc, chain_id) super_token: str = "SUPER TOKEN ADDRESS" sender: str = "SENDER
 ADDRESS" receiver: str = "RECEIVER ADDRESS" flow_rate: int = "FLOW RATE"
-PRIVATE_KEY: str = "YOUR PRIVATE KEY" OPERATOR_PRIVATE_KEY: str = "OPERATOR
-PRIVATE KEY" flow_data: Web3FlowInfo = cfaV1Instance.get_flow(super_token,
-sender, receiver) create_flow_operation = cfaV1Instance.create_flow( sender,
-receiver, super_token, flow_rate) transaction_hash = create_flow_operation.exec
-(PRIVATE_KEY) update_flow_operation = cfaV1Instance.update_flow( sender,
-receiver, super_token, flow_rate) transaction_hash = update_flow_operation.exec
+PRIVATE_KEY: str = "YOUR PRIVATE KEY" flow_data: Web3FlowInfo =
+cfaV1Instance.get_flow(super_token, sender, receiver) create_flow_operation =
+cfaV1Instance.create_flow( sender, receiver, super_token, flow_rate)
+transaction_hash = create_flow_operation.exec(PRIVATE_KEY)
+update_flow_operation = cfaV1Instance.update_flow( sender, receiver,
+super_token, flow_rate) transaction_hash = update_flow_operation.exec
 (PRIVATE_KEY) delete_flow_operation = cfaV1Instance.delete_flow( sender,
 receiver, super_token) transaction_hash = delete_flow_operation.exec
 (PRIVATE_KEY) ```
```

### Comparing `superfluid-0.1.3/README.md` & `superfluid-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 
 super_token: str = "SUPER TOKEN ADDRESS"
 sender: str = "SENDER ADDRESS"
 receiver: str = "RECEIVER ADDRESS"
 flow_rate: int = "FLOW RATE"
 
 PRIVATE_KEY: str = "YOUR PRIVATE KEY"
-OPERATOR_PRIVATE_KEY: str = "OPERATOR PRIVATE KEY"
 
 flow_data: Web3FlowInfo = cfaV1Instance.get_flow(super_token, sender, receiver)
 
 create_flow_operation = cfaV1Instance.create_flow(
     sender, receiver, super_token, flow_rate)
 transaction_hash = create_flow_operation.exec(PRIVATE_KEY)
```

#### html2text {}

```diff
@@ -12,16 +12,16 @@
 superfluid ``` # Usage ```python from superfluid import CFA_V1 from superfluid
 import Web3FlowInfo rpc: str = "YOUR PREFERRED RPC" chain_id: int = "CHAIN ID"
 ###################################################### ###### CONSTANT FLOW
 AGREEMENT OPERATIONS ###########
 ###################################################### cfaV1Instance = CFA_V1
 (rpc, chain_id) super_token: str = "SUPER TOKEN ADDRESS" sender: str = "SENDER
 ADDRESS" receiver: str = "RECEIVER ADDRESS" flow_rate: int = "FLOW RATE"
-PRIVATE_KEY: str = "YOUR PRIVATE KEY" OPERATOR_PRIVATE_KEY: str = "OPERATOR
-PRIVATE KEY" flow_data: Web3FlowInfo = cfaV1Instance.get_flow(super_token,
-sender, receiver) create_flow_operation = cfaV1Instance.create_flow( sender,
-receiver, super_token, flow_rate) transaction_hash = create_flow_operation.exec
-(PRIVATE_KEY) update_flow_operation = cfaV1Instance.update_flow( sender,
-receiver, super_token, flow_rate) transaction_hash = update_flow_operation.exec
+PRIVATE_KEY: str = "YOUR PRIVATE KEY" flow_data: Web3FlowInfo =
+cfaV1Instance.get_flow(super_token, sender, receiver) create_flow_operation =
+cfaV1Instance.create_flow( sender, receiver, super_token, flow_rate)
+transaction_hash = create_flow_operation.exec(PRIVATE_KEY)
+update_flow_operation = cfaV1Instance.update_flow( sender, receiver,
+super_token, flow_rate) transaction_hash = update_flow_operation.exec
 (PRIVATE_KEY) delete_flow_operation = cfaV1Instance.delete_flow( sender,
 receiver, super_token) transaction_hash = delete_flow_operation.exec
 (PRIVATE_KEY) ```
```

### Comparing `superfluid-0.1.3/main/superfluid/src/cfa.py` & `superfluid-0.2.0/main/superfluid/src/cfa.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.3/main/superfluid/src/host.py` & `superfluid-0.2.0/main/superfluid/src/host.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.3/main/superfluid/src/operation.py` & `superfluid-0.2.0/main/superfluid/src/operation.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.3/main/superfluid/src/types.py` & `superfluid-0.2.0/main/superfluid/src/types.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.3/main/superfluid/src/utils.py` & `superfluid-0.2.0/main/superfluid/src/utils.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.3/main/superfluid/test/test_utils.py` & `superfluid-0.2.0/main/superfluid/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.1.3/main/superfluid.egg-info/PKG-INFO` & `superfluid-0.2.0/main/superfluid.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -74,15 +74,14 @@
 
 super_token: str = "SUPER TOKEN ADDRESS"
 sender: str = "SENDER ADDRESS"
 receiver: str = "RECEIVER ADDRESS"
 flow_rate: int = "FLOW RATE"
 
 PRIVATE_KEY: str = "YOUR PRIVATE KEY"
-OPERATOR_PRIVATE_KEY: str = "OPERATOR PRIVATE KEY"
 
 flow_data: Web3FlowInfo = cfaV1Instance.get_flow(super_token, sender, receiver)
 
 create_flow_operation = cfaV1Instance.create_flow(
     sender, receiver, super_token, flow_rate)
 transaction_hash = create_flow_operation.exec(PRIVATE_KEY)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.1.3 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.2.0 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
         ****** Welcome to Superfluid Python SDK(Unofficial) ð ******
@@ -19,16 +19,16 @@
 superfluid ``` # Usage ```python from superfluid import CFA_V1 from superfluid
 import Web3FlowInfo rpc: str = "YOUR PREFERRED RPC" chain_id: int = "CHAIN ID"
 ###################################################### ###### CONSTANT FLOW
 AGREEMENT OPERATIONS ###########
 ###################################################### cfaV1Instance = CFA_V1
 (rpc, chain_id) super_token: str = "SUPER TOKEN ADDRESS" sender: str = "SENDER
 ADDRESS" receiver: str = "RECEIVER ADDRESS" flow_rate: int = "FLOW RATE"
-PRIVATE_KEY: str = "YOUR PRIVATE KEY" OPERATOR_PRIVATE_KEY: str = "OPERATOR
-PRIVATE KEY" flow_data: Web3FlowInfo = cfaV1Instance.get_flow(super_token,
-sender, receiver) create_flow_operation = cfaV1Instance.create_flow( sender,
-receiver, super_token, flow_rate) transaction_hash = create_flow_operation.exec
-(PRIVATE_KEY) update_flow_operation = cfaV1Instance.update_flow( sender,
-receiver, super_token, flow_rate) transaction_hash = update_flow_operation.exec
+PRIVATE_KEY: str = "YOUR PRIVATE KEY" flow_data: Web3FlowInfo =
+cfaV1Instance.get_flow(super_token, sender, receiver) create_flow_operation =
+cfaV1Instance.create_flow( sender, receiver, super_token, flow_rate)
+transaction_hash = create_flow_operation.exec(PRIVATE_KEY)
+update_flow_operation = cfaV1Instance.update_flow( sender, receiver,
+super_token, flow_rate) transaction_hash = update_flow_operation.exec
 (PRIVATE_KEY) delete_flow_operation = cfaV1Instance.delete_flow( sender,
 receiver, super_token) transaction_hash = delete_flow_operation.exec
 (PRIVATE_KEY) ```
```

### Comparing `superfluid-0.1.3/main/superfluid.egg-info/SOURCES.txt` & `superfluid-0.2.0/main/superfluid.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 main/superfluid/__init__.py
 main/superfluid.egg-info/PKG-INFO
 main/superfluid.egg-info/SOURCES.txt
 main/superfluid.egg-info/dependency_links.txt
 main/superfluid.egg-info/requires.txt
 main/superfluid.egg-info/top_level.txt
 main/superfluid/src/__init__.py
+main/superfluid/src/abis.py
 main/superfluid/src/cfa.py
 main/superfluid/src/constants.py
 main/superfluid/src/errors.py
 main/superfluid/src/host.py
+main/superfluid/src/metadata.py
 main/superfluid/src/operation.py
 main/superfluid/src/types.py
 main/superfluid/src/utils.py
 main/superfluid/test/__init__.py
 main/superfluid/test/test_utils.py
```

### Comparing `superfluid-0.1.3/setup.py` & `superfluid-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="superfluid",
-    version="0.1.3",
+    version="0.2.0",
     description="Python SDK for the Superfluid Protocol",
     package_dir={"": "main"},
     packages=find_packages(where="main"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Godspower-Eze/superfluid.py",
     author="Godspower-Eze",
```

