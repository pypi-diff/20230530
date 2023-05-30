# Comparing `tmp/superfluid-0.2.0.tar.gz` & `tmp/superfluid-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superfluid-0.2.0.tar", last modified: Tue May 30 15:16:02 2023, max compression
+gzip compressed data, was "superfluid-0.2.1.tar", last modified: Tue May 30 15:36:28 2023, max compression
```

## Comparing `superfluid-0.2.0.tar` & `superfluid-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:16:02.538571 superfluid-0.2.0/
--rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.2.0/LICENSE.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)     2777 2023-05-30 15:16:02.538234 superfluid-0.2.0/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)     2288 2023-05-30 15:14:04.000000 superfluid-0.2.0/README.md
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:16:02.534360 superfluid-0.2.0/main/
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:16:02.535050 superfluid-0.2.0/main/superfluid/
--rw-r--r--   0 godspowereze   (501) staff       (20)      166 2023-05-29 13:16:23.000000 superfluid-0.2.0/main/superfluid/__init__.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:16:02.537016 superfluid-0.2.0/main/superfluid/src/
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:15:40.000000 superfluid-0.2.0/main/superfluid/src/__init__.py
--rw-r--r--   0 godspowereze   (501) staff       (20)    50176 2023-05-30 15:06:49.000000 superfluid-0.2.0/main/superfluid/src/abis.py
--rw-r--r--   0 godspowereze   (501) staff       (20)    21996 2023-05-29 12:34:47.000000 superfluid-0.2.0/main/superfluid/src/cfa.py
--rw-r--r--   0 godspowereze   (501) staff       (20)      430 2023-05-30 15:09:33.000000 superfluid-0.2.0/main/superfluid/src/constants.py
--rw-r--r--   0 godspowereze   (501) staff       (20)      335 2023-05-29 08:52:33.000000 superfluid-0.2.0/main/superfluid/src/errors.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1022 2023-05-29 10:12:39.000000 superfluid-0.2.0/main/superfluid/src/host.py
--rw-r--r--   0 godspowereze   (501) staff       (20)    21807 2023-05-30 15:07:36.000000 superfluid-0.2.0/main/superfluid/src/metadata.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1956 2023-05-29 10:02:53.000000 superfluid-0.2.0/main/superfluid/src/operation.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     9946 2023-05-29 11:15:00.000000 superfluid-0.2.0/main/superfluid/src/types.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1513 2023-05-29 10:10:55.000000 superfluid-0.2.0/main/superfluid/src/utils.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:16:02.537522 superfluid-0.2.0/main/superfluid/test/
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-26 06:50:05.000000 superfluid-0.2.0/main/superfluid/test/__init__.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     5324 2023-05-29 09:57:23.000000 superfluid-0.2.0/main/superfluid/test/test_utils.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:16:02.535763 superfluid-0.2.0/main/superfluid.egg-info/
--rw-r--r--   0 godspowereze   (501) staff       (20)     2777 2023-05-30 15:16:02.000000 superfluid-0.2.0/main/superfluid.egg-info/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)      621 2023-05-30 15:16:02.000000 superfluid-0.2.0/main/superfluid.egg-info/SOURCES.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-30 15:16:02.000000 superfluid-0.2.0/main/superfluid.egg-info/dependency_links.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       53 2023-05-30 15:16:02.000000 superfluid-0.2.0/main/superfluid.egg-info/requires.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       11 2023-05-30 15:16:02.000000 superfluid-0.2.0/main/superfluid.egg-info/top_level.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-30 15:16:02.538784 superfluid-0.2.0/setup.cfg
--rw-r--r--   0 godspowereze   (501) staff       (20)      848 2023-05-30 15:12:18.000000 superfluid-0.2.0/setup.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:36:28.419155 superfluid-0.2.1/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.2.1/LICENSE.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2775 2023-05-30 15:36:28.418983 superfluid-0.2.1/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2286 2023-05-30 15:32:30.000000 superfluid-0.2.1/README.md
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:36:28.414775 superfluid-0.2.1/main/
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:36:28.415982 superfluid-0.2.1/main/superfluid/
+-rw-r--r--   0 godspowereze   (501) staff       (20)      166 2023-05-29 13:16:23.000000 superfluid-0.2.1/main/superfluid/__init__.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:36:28.418573 superfluid-0.2.1/main/superfluid/src/
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:15:40.000000 superfluid-0.2.1/main/superfluid/src/__init__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)    50176 2023-05-30 15:06:49.000000 superfluid-0.2.1/main/superfluid/src/abis.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)    21996 2023-05-29 12:34:47.000000 superfluid-0.2.1/main/superfluid/src/cfa.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      430 2023-05-30 15:09:33.000000 superfluid-0.2.1/main/superfluid/src/constants.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      335 2023-05-29 08:52:33.000000 superfluid-0.2.1/main/superfluid/src/errors.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1022 2023-05-29 10:12:39.000000 superfluid-0.2.1/main/superfluid/src/host.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)    21807 2023-05-30 15:07:36.000000 superfluid-0.2.1/main/superfluid/src/metadata.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1956 2023-05-29 10:02:53.000000 superfluid-0.2.1/main/superfluid/src/operation.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     9946 2023-05-29 11:15:00.000000 superfluid-0.2.1/main/superfluid/src/types.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1513 2023-05-29 10:10:55.000000 superfluid-0.2.1/main/superfluid/src/utils.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:36:28.418794 superfluid-0.2.1/main/superfluid/test/
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-26 06:50:05.000000 superfluid-0.2.1/main/superfluid/test/__init__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     5324 2023-05-29 09:57:23.000000 superfluid-0.2.1/main/superfluid/test/test_utils.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-30 15:36:28.417281 superfluid-0.2.1/main/superfluid.egg-info/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2775 2023-05-30 15:36:28.000000 superfluid-0.2.1/main/superfluid.egg-info/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)      621 2023-05-30 15:36:28.000000 superfluid-0.2.1/main/superfluid.egg-info/SOURCES.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-30 15:36:28.000000 superfluid-0.2.1/main/superfluid.egg-info/dependency_links.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       53 2023-05-30 15:36:28.000000 superfluid-0.2.1/main/superfluid.egg-info/requires.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       11 2023-05-30 15:36:28.000000 superfluid-0.2.1/main/superfluid.egg-info/top_level.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-30 15:36:28.419192 superfluid-0.2.1/setup.cfg
+-rw-r--r--   0 godspowereze   (501) staff       (20)      848 2023-05-30 15:35:18.000000 superfluid-0.2.1/setup.py
```

### Comparing `superfluid-0.2.0/LICENSE.txt` & `superfluid-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superfluid-0.2.0/PKG-INFO` & `superfluid-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 
 ### 📖 [Docs](https://docs.superfluid.finance)
 
 </br>
 
 # Introduction
 
-superfluid.py is an application framework for interacting with the Superfluid Protocol without the Python Programming Language.
+superfluid.py is an application framework for interacting with the Superfluid Protocol using the Python Programming Language.
 
 # Features
 
 * Minimal Framework initialization (`rpc` and `chain id`)
 * New Operation syntax for transactions
 * Read/Create/Update/Delete Agreement Operations (Constant Flow Agreement and Instant Distribution Agreement(In development))
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.2.0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.2.1 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
         ****** Welcome to Superfluid Python SDK(Unofficial) ð ******
                                [Superfluid logo]
                     [License:_MIT] [Twitter:_Superfluid_HQ]
 ### ð  [Homepage](https://superfluid.finance) ### â¨ [Superfluid App](https:
 //app.superfluid.finance/) ### ð [Docs](https://docs.superfluid.finance)  #
 Introduction superfluid.py is an application framework for interacting with the
-Superfluid Protocol without the Python Programming Language. # Features *
-Minimal Framework initialization (`rpc` and `chain id`) * New Operation syntax
-for transactions * Read/Create/Update/Delete Agreement Operations (Constant
-Flow Agreement and Instant Distribution Agreement(In development)) # Notable
-Used Technologies * Python * Web3.py # Installation ```bash pip install
-superfluid ``` # Usage ```python from superfluid import CFA_V1 from superfluid
-import Web3FlowInfo rpc: str = "YOUR PREFERRED RPC" chain_id: int = "CHAIN ID"
+Superfluid Protocol using the Python Programming Language. # Features * Minimal
+Framework initialization (`rpc` and `chain id`) * New Operation syntax for
+transactions * Read/Create/Update/Delete Agreement Operations (Constant Flow
+Agreement and Instant Distribution Agreement(In development)) # Notable Used
+Technologies * Python * Web3.py # Installation ```bash pip install superfluid
+``` # Usage ```python from superfluid import CFA_V1 from superfluid import
+Web3FlowInfo rpc: str = "YOUR PREFERRED RPC" chain_id: int = "CHAIN ID"
 ###################################################### ###### CONSTANT FLOW
 AGREEMENT OPERATIONS ###########
 ###################################################### cfaV1Instance = CFA_V1
 (rpc, chain_id) super_token: str = "SUPER TOKEN ADDRESS" sender: str = "SENDER
 ADDRESS" receiver: str = "RECEIVER ADDRESS" flow_rate: int = "FLOW RATE"
 PRIVATE_KEY: str = "YOUR PRIVATE KEY" flow_data: Web3FlowInfo =
 cfaV1Instance.get_flow(super_token, sender, receiver) create_flow_operation =
```

### Comparing `superfluid-0.2.0/README.md` & `superfluid-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ### 📖 [Docs](https://docs.superfluid.finance)
 
 </br>
 
 # Introduction
 
-superfluid.py is an application framework for interacting with the Superfluid Protocol without the Python Programming Language.
+superfluid.py is an application framework for interacting with the Superfluid Protocol using the Python Programming Language.
 
 # Features
 
 * Minimal Framework initialization (`rpc` and `chain id`)
 * New Operation syntax for transactions
 * Read/Create/Update/Delete Agreement Operations (Constant Flow Agreement and Instant Distribution Agreement(In development))
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
         ****** Welcome to Superfluid Python SDK(Unofficial) ð ******
                                [Superfluid logo]
                     [License:_MIT] [Twitter:_Superfluid_HQ]
 ### ð  [Homepage](https://superfluid.finance) ### â¨ [Superfluid App](https:
 //app.superfluid.finance/) ### ð [Docs](https://docs.superfluid.finance)  #
 Introduction superfluid.py is an application framework for interacting with the
-Superfluid Protocol without the Python Programming Language. # Features *
-Minimal Framework initialization (`rpc` and `chain id`) * New Operation syntax
-for transactions * Read/Create/Update/Delete Agreement Operations (Constant
-Flow Agreement and Instant Distribution Agreement(In development)) # Notable
-Used Technologies * Python * Web3.py # Installation ```bash pip install
-superfluid ``` # Usage ```python from superfluid import CFA_V1 from superfluid
-import Web3FlowInfo rpc: str = "YOUR PREFERRED RPC" chain_id: int = "CHAIN ID"
+Superfluid Protocol using the Python Programming Language. # Features * Minimal
+Framework initialization (`rpc` and `chain id`) * New Operation syntax for
+transactions * Read/Create/Update/Delete Agreement Operations (Constant Flow
+Agreement and Instant Distribution Agreement(In development)) # Notable Used
+Technologies * Python * Web3.py # Installation ```bash pip install superfluid
+``` # Usage ```python from superfluid import CFA_V1 from superfluid import
+Web3FlowInfo rpc: str = "YOUR PREFERRED RPC" chain_id: int = "CHAIN ID"
 ###################################################### ###### CONSTANT FLOW
 AGREEMENT OPERATIONS ###########
 ###################################################### cfaV1Instance = CFA_V1
 (rpc, chain_id) super_token: str = "SUPER TOKEN ADDRESS" sender: str = "SENDER
 ADDRESS" receiver: str = "RECEIVER ADDRESS" flow_rate: int = "FLOW RATE"
 PRIVATE_KEY: str = "YOUR PRIVATE KEY" flow_data: Web3FlowInfo =
 cfaV1Instance.get_flow(super_token, sender, receiver) create_flow_operation =
```

### Comparing `superfluid-0.2.0/main/superfluid/src/abis.py` & `superfluid-0.2.1/main/superfluid/src/abis.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.2.0/main/superfluid/src/cfa.py` & `superfluid-0.2.1/main/superfluid/src/cfa.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.2.0/main/superfluid/src/host.py` & `superfluid-0.2.1/main/superfluid/src/host.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.2.0/main/superfluid/src/metadata.py` & `superfluid-0.2.1/main/superfluid/src/metadata.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.2.0/main/superfluid/src/operation.py` & `superfluid-0.2.1/main/superfluid/src/operation.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.2.0/main/superfluid/src/types.py` & `superfluid-0.2.1/main/superfluid/src/types.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.2.0/main/superfluid/src/utils.py` & `superfluid-0.2.1/main/superfluid/src/utils.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.2.0/main/superfluid/test/test_utils.py` & `superfluid-0.2.1/main/superfluid/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.2.0/main/superfluid.egg-info/PKG-INFO` & `superfluid-0.2.1/main/superfluid.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 
 ### 📖 [Docs](https://docs.superfluid.finance)
 
 </br>
 
 # Introduction
 
-superfluid.py is an application framework for interacting with the Superfluid Protocol without the Python Programming Language.
+superfluid.py is an application framework for interacting with the Superfluid Protocol using the Python Programming Language.
 
 # Features
 
 * Minimal Framework initialization (`rpc` and `chain id`)
 * New Operation syntax for transactions
 * Read/Create/Update/Delete Agreement Operations (Constant Flow Agreement and Instant Distribution Agreement(In development))
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.2.0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.2.1 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
         ****** Welcome to Superfluid Python SDK(Unofficial) ð ******
                                [Superfluid logo]
                     [License:_MIT] [Twitter:_Superfluid_HQ]
 ### ð  [Homepage](https://superfluid.finance) ### â¨ [Superfluid App](https:
 //app.superfluid.finance/) ### ð [Docs](https://docs.superfluid.finance)  #
 Introduction superfluid.py is an application framework for interacting with the
-Superfluid Protocol without the Python Programming Language. # Features *
-Minimal Framework initialization (`rpc` and `chain id`) * New Operation syntax
-for transactions * Read/Create/Update/Delete Agreement Operations (Constant
-Flow Agreement and Instant Distribution Agreement(In development)) # Notable
-Used Technologies * Python * Web3.py # Installation ```bash pip install
-superfluid ``` # Usage ```python from superfluid import CFA_V1 from superfluid
-import Web3FlowInfo rpc: str = "YOUR PREFERRED RPC" chain_id: int = "CHAIN ID"
+Superfluid Protocol using the Python Programming Language. # Features * Minimal
+Framework initialization (`rpc` and `chain id`) * New Operation syntax for
+transactions * Read/Create/Update/Delete Agreement Operations (Constant Flow
+Agreement and Instant Distribution Agreement(In development)) # Notable Used
+Technologies * Python * Web3.py # Installation ```bash pip install superfluid
+``` # Usage ```python from superfluid import CFA_V1 from superfluid import
+Web3FlowInfo rpc: str = "YOUR PREFERRED RPC" chain_id: int = "CHAIN ID"
 ###################################################### ###### CONSTANT FLOW
 AGREEMENT OPERATIONS ###########
 ###################################################### cfaV1Instance = CFA_V1
 (rpc, chain_id) super_token: str = "SUPER TOKEN ADDRESS" sender: str = "SENDER
 ADDRESS" receiver: str = "RECEIVER ADDRESS" flow_rate: int = "FLOW RATE"
 PRIVATE_KEY: str = "YOUR PRIVATE KEY" flow_data: Web3FlowInfo =
 cfaV1Instance.get_flow(super_token, sender, receiver) create_flow_operation =
```

### Comparing `superfluid-0.2.0/main/superfluid.egg-info/SOURCES.txt` & `superfluid-0.2.1/main/superfluid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `superfluid-0.2.0/setup.py` & `superfluid-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="superfluid",
-    version="0.2.0",
+    version="0.2.1",
     description="Python SDK for the Superfluid Protocol",
     package_dir={"": "main"},
     packages=find_packages(where="main"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Godspower-Eze/superfluid.py",
     author="Godspower-Eze",
```

