# Comparing `tmp/mech_client-0.1.2.tar.gz` & `tmp/mech_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mech_client-0.1.2.tar", max compression
+gzip compressed data, was "mech_client-0.1.3.tar", max compression
```

## Comparing `mech_client-0.1.2.tar` & `mech_client-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11339 2023-05-27 20:23:22.952168 mech_client-0.1.2/LICENSE
--rw-r--r--   0        0        0     1926 2023-05-27 20:25:03.823431 mech_client-0.1.2/README.md
--rw-r--r--   0        0        0       22 2023-05-30 08:39:49.524762 mech_client-0.1.2/mech_client/__init__.py
--rw-r--r--   0        0        0     1147 2023-05-30 08:36:18.724247 mech_client-0.1.2/mech_client/cli.py
--rw-r--r--   0        0        0     5631 2023-05-30 08:36:32.071823 mech_client-0.1.2/mech_client/interact.py
--rw-r--r--   0        0        0     1790 2023-05-27 19:55:10.151934 mech_client-0.1.2/mech_client/prompt_to_ipfs.py
--rw-r--r--   0        0        0     1670 2023-05-27 20:02:06.617746 mech_client-0.1.2/mech_client/push_to_ipfs.py
--rw-r--r--   0        0        0      558 2023-05-30 08:39:25.067038 mech_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2843 1970-01-01 00:00:00.000000 mech_client-0.1.2/setup.py
--rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 mech_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-05-27 20:23:22.952168 mech_client-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2037 2023-05-30 10:09:38.116752 mech_client-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-05-30 10:32:58.756355 mech_client-0.1.3/mech_client/__init__.py
+-rw-r--r--   0        0        0     1147 2023-05-30 08:36:18.724247 mech_client-0.1.3/mech_client/cli.py
+-rw-r--r--   0        0        0     7257 2023-05-30 10:28:07.483789 mech_client-0.1.3/mech_client/interact.py
+-rw-r--r--   0        0        0     1790 2023-05-27 19:55:10.151934 mech_client-0.1.3/mech_client/prompt_to_ipfs.py
+-rw-r--r--   0        0        0     1670 2023-05-27 20:02:06.617746 mech_client-0.1.3/mech_client/push_to_ipfs.py
+-rw-r--r--   0        0        0      558 2023-05-30 10:32:52.540021 mech_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 mech_client-0.1.3/setup.py
+-rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 mech_client-0.1.3/PKG-INFO
```

### Comparing `mech_client-0.1.2/LICENSE` & `mech_client-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.2/README.md` & `mech_client-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 ## Installation
 
 ```bash
 pip install mech-client
 ```
 
+Then, set a websocket endpoint for Gnosis RPC like so:
+
+```bash
+export WEBSOCKET_ENDPOINT=<YOUR ENDPOINT>
+```
+
 ## CLI:
 
 ```bash
 Usage: mechx [OPTIONS] COMMAND [ARGS]...
 
   Command-line tool for interacting with mechs.
```

### Comparing `mech_client-0.1.2/mech_client/cli.py` & `mech_client-0.1.3/mech_client/cli.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.2/mech_client/interact.py` & `mech_client-0.1.3/mech_client/interact.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,16 +22,18 @@
 
 Usage:
 
 python client.py <prompt> <tool>
 """
 
 import json
+import os
 import sys
 import time
+import warnings
 from typing import Optional
 
 import requests
 import websocket
 from aea.contracts.base import Contract
 from aea_ledger_ethereum import EthereumApi, EthereumCrypto
 
@@ -41,14 +43,27 @@
 ETHEREUM_TESTNET_CONFIG = {
     "address": "https://rpc.eu-central-2.gateway.fm/v4/gnosis/non-archival/mainnet",
     "chain_id": 100,
     "poa_chain": False,
     "default_gas_price_strategy": "eip1559",
 }
 PRIVATE_KEY_FILE_PATH = "ethereum_private_key.txt"
+EVENT_SIGNATURE_REQUEST = (
+    "0x4bda649efe6b98b0f9c1d5e859c29e20910f45c66dabfe6fad4a4881f7faf9cc"
+)
+EVENT_SIGNATURE_DELIVER = (
+    "0x3ec84da2cdc1ce60c063642b69ff2e65f3b69787a2b90443457ba274e51e7c72"
+)
+WSS_ENDPOINT = os.getenv(
+    "WEBSOCKET_ENDPOINT",
+    "wss://gno.getblock.io/3042bb06-d18e-4ce0-8ccf-83eedd35532b/mainnet/",
+)
+
+# Ignore a specific warning message
+warnings.filterwarnings("ignore", "The log with transaction hash.*")
 
 
 def check_for_tools(tool: str) -> Optional[int]:
     """Checks if the tool is valid and for what agent."""
     # TODO - replace hardcoded logic with on-chain check against agent mech registry
     return (
         3
@@ -59,30 +74,67 @@
             "openai-gpt-3.5-turbo",
             "openai-gpt-4",
         ]
         else None
     )
 
 
+def register_event_handlers(ethereum_crypto: EthereumCrypto) -> websocket.WebSocket:
+    """Register event handlers."""
+    wss = websocket.create_connection(WSS_ENDPOINT)
+    subscription_request = {
+        "jsonrpc": "2.0",
+        "id": 1,
+        "method": "eth_subscribe",
+        "params": [
+            "logs",
+            {
+                "address": CONTRACT_ADDRESS,
+                "topics": [
+                    EVENT_SIGNATURE_REQUEST,
+                    ["0x" + "0" * 24 + ethereum_crypto.address[2:]],
+                ],
+            },
+        ],
+    }
+    content = bytes(json.dumps(subscription_request), "utf-8")
+    wss.send(content)
+    # registration confirmation
+    msg = wss.recv()
+    subscription_deliver = {
+        "jsonrpc": "2.0",
+        "id": 1,
+        "method": "eth_subscribe",
+        "params": [
+            "logs",
+            {"address": CONTRACT_ADDRESS, "topics": [EVENT_SIGNATURE_DELIVER]},
+        ],
+    }
+    content = bytes(json.dumps(subscription_deliver), "utf-8")
+    wss.send(content)
+    # registration confirmation
+    msg = wss.recv()
+    return wss
+
+
 def send_request(
+    ethereum_crypto: EthereumCrypto,
+    ethereum_ledger_api: EthereumApi,
     prompt: str,
     tool: str,
     contract_address: str = CONTRACT_ADDRESS,
     price: int = 10_000_000_000_000_000,
 ) -> Contract:
     """Sends a request to the mech."""
     mech = check_for_tools(tool)
     if mech is None:
         raise ValueError(f"Tool {tool} is not supported by any mech.")
     v1_file_hash_hex_truncated, v1_file_hash_hex = push_metadata_to_ipfs(prompt, tool)
     print(f"Prompt uploaded: https://gateway.autonolas.tech/ipfs/{v1_file_hash_hex}")
 
-    ethereum_crypto = EthereumCrypto(private_key_path=PRIVATE_KEY_FILE_PATH)
-    ethereum_ledger_api = EthereumApi(**ETHEREUM_TESTNET_CONFIG)
-
     gnosisscan_api_url = f"https://api.gnosisscan.io/api?module=contract&action=getabi&address={contract_address}"
     response = requests.get(gnosisscan_api_url)
     abi = response.json()["result"]
     abi = json.loads(abi)
 
     contract_instance = ethereum_ledger_api.get_contract_instance(
         {"abi": abi, "bytecode": "0x"}, contract_address
@@ -100,58 +152,56 @@
         tx_args=tx_args,
     )
     raw_transaction["gas"] = 50_000
     # raw_transaction = ethereum_ledger_api.update_with_gas_estimate(raw_transaction)
     signed_transaction = ethereum_crypto.sign_transaction(raw_transaction)
     transaction_digest = ethereum_ledger_api.send_signed_transaction(signed_transaction)
     print(f"Transaction sent: https://gnosisscan.io/tx/{transaction_digest}")
-    return contract_instance, ethereum_ledger_api
+    return contract_instance
 
 
 def watch_for_events(
-    contract_instance: Contract, ethereum_ledger_api: EthereumApi
+    wss: websocket.WebSocket,
+    contract_instance: Contract,
+    ethereum_ledger_api: EthereumApi,
+    ethereum_crypto: EthereumCrypto,
 ) -> None:
     """Watches for events on mech."""
-    wss_endpoint = "wss://rpc.eu-central-2.gateway.fm/ws/v4/gnosis/non-archival/mainnet"
-    wss = websocket.create_connection(wss_endpoint)
-    subscription_msg_template = {
-        "jsonrpc": "2.0",
-        "id": 1,
-        "method": "eth_subscribe",
-        "params": ["logs", {"address": CONTRACT_ADDRESS}],
-    }
-    content = bytes(json.dumps(subscription_msg_template), "utf-8")
-    wss.send(content)
-    # registration confirmation
-    msg = wss.recv()
-    # events
-    count = 0
-    while count < 2:
+    is_waiting = True
+    while is_waiting:
         msg = wss.recv()
         data = json.loads(msg)
         tx_hash = data["params"]["result"]["transactionHash"]
         no_receipt = True
         while no_receipt:
             try:
                 tx_receipt = ethereum_ledger_api._api.eth.get_transaction_receipt(
                     tx_hash
                 )
                 no_receipt = False
             except Exception:
                 time.sleep(1)
-        if count == 0:
+        event_signature = tx_receipt["logs"][0]["topics"][0].hex()
+        if event_signature == EVENT_SIGNATURE_REQUEST:
             rich_logs = contract_instance.events.Request().processReceipt(tx_receipt)
             request_id = rich_logs[0]["args"]["requestId"]
             print(f"Request on-chain with id: {request_id}")
-        if count == 1:
+        if event_signature == EVENT_SIGNATURE_DELIVER:
             rich_logs = contract_instance.events.Deliver().processReceipt(tx_receipt)
             data = rich_logs[0]["args"]["data"]
+            request_id_ = rich_logs[0]["args"]["requestId"]
+            if request_id != request_id_:
+                continue
             data_url = "https://gateway.autonolas.tech/ipfs/f01701220" + data.hex()
             print(f"Data arrived: {data_url}")
-        count += 1
+            is_waiting = False
     response = requests.get(data_url + "/" + str(request_id))
-    print(f"Data: {response.json()}")
+    result = response.json()["result"]
+    print(f"Data:\n{result}")
 
 
 def interact(prompt: str, tool: str) -> None:
-    contract_instance, ethereum_ledger_api = send_request(prompt, tool)
-    watch_for_events(contract_instance, ethereum_ledger_api)
+    ethereum_crypto = EthereumCrypto(private_key_path=PRIVATE_KEY_FILE_PATH)
+    ethereum_ledger_api = EthereumApi(**ETHEREUM_TESTNET_CONFIG)
+    wss = register_event_handlers(ethereum_crypto)
+    contract_instance = send_request(ethereum_crypto, ethereum_ledger_api, prompt, tool)
+    watch_for_events(wss, contract_instance, ethereum_ledger_api, ethereum_crypto)
```

### Comparing `mech_client-0.1.2/mech_client/prompt_to_ipfs.py` & `mech_client-0.1.3/mech_client/prompt_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.2/mech_client/push_to_ipfs.py` & `mech_client-0.1.3/mech_client/push_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.2/pyproject.toml` & `mech_client-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mech-client"
-version = "0.1.2"
+version = "0.1.3"
 description = "Basic client to interact with a mech"
 authors = ["David Minarsch <david.minarsch@googlemail.com>"]
 readme = "README.md"
 packages = [{include = "mech_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `mech_client-0.1.2/setup.py` & `mech_client-0.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'websocket-client>=0.32.0,<1']
 
 entry_points = \
 {'console_scripts': ['mechx = mech_client.cli:cli']}
 
 setup_kwargs = {
     'name': 'mech-client',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Basic client to interact with a mech',
-    'long_description': '# mech-client\nBasic client to interact with a mech\n\n> **Warning**<br />\n> **This is a hacky alpha version of the client - don\'t rely on it as production software.**\n\n## Installation\n\n```bash\npip install mech-client\n```\n\n## CLI:\n\n```bash\nUsage: mechx [OPTIONS] COMMAND [ARGS]...\n\n  Command-line tool for interacting with mechs.\n\nOptions:\n  --version  Show the version and exit.\n  --help     Show this message and exit.\n\nCommands:\n  interact        Interact with a mech specifying a prompt and tool.\n  prompt-to-ipfs  Upload a prompt and tool to IPFS as metadata.\n  push-to-ipfs    Upload a file to IPFS.\n ```\n\n## Usage:\n\nFirst, create a private key in file `ethereum_private_key.txt` with this command:\n\n```bash\naea generate-key ethereum\n```\n\nEnsure the private key carries funds on Gnosis Chain.\n\nSecond, run the following command to instruct the mech with `<prompt>` and `<tool>`:\n\n```bash\nmechx interact <prompt> <tool>\n```\n\nExample output:\n```bash\nmechx interact "write a short poem" "openai-text-davinci-003"\nPrompt uploaded: https://gateway.autonolas.tech/ipfs/f01701220ad9e2d5698fbd6c3a4ce61f329590e68a23181772669e543e69decdae316423b\nTransaction sent: https://gnosisscan.io/tx/0xb3a17ef90da6cc7a86e008a3a91bd367d573b406eae53405a4aa981001a5eaf3\nRequest on-chain with id: 15263135923206312300456917202469137903009897852865973093832667165921851537677\nData arrived: https://gateway.autonolas.tech/ipfs/f017012205053a4ae3ef0cf4ed7eff0c2d74dbaf3479fbdeb292472560e7bfaa4cfecfcdc\nData: {\'requestId\': 15263135923206312300456917202469137903009897852865973093832667165921851537677, \'result\': "\\n\\nA sun-filled sky,\\nA soft breeze blowing by,\\nWhere the trees sway in the wind,\\nA peaceful moment I can\'t rewind."}\n```\n\n## Release guide:\n\nFinish edits, bump versions in `pyproject.toml` and `mech_client/__init__.py`, then `poetry lock`, then `rm -rf dist`, then `poetry publish --build --username=<username> --password=<password>`.',
+    'long_description': '# mech-client\nBasic client to interact with a mech\n\n> **Warning**<br />\n> **This is a hacky alpha version of the client - don\'t rely on it as production software.**\n\n## Installation\n\n```bash\npip install mech-client\n```\n\nThen, set a websocket endpoint for Gnosis RPC like so:\n\n```bash\nexport WEBSOCKET_ENDPOINT=<YOUR ENDPOINT>\n```\n\n## CLI:\n\n```bash\nUsage: mechx [OPTIONS] COMMAND [ARGS]...\n\n  Command-line tool for interacting with mechs.\n\nOptions:\n  --version  Show the version and exit.\n  --help     Show this message and exit.\n\nCommands:\n  interact        Interact with a mech specifying a prompt and tool.\n  prompt-to-ipfs  Upload a prompt and tool to IPFS as metadata.\n  push-to-ipfs    Upload a file to IPFS.\n ```\n\n## Usage:\n\nFirst, create a private key in file `ethereum_private_key.txt` with this command:\n\n```bash\naea generate-key ethereum\n```\n\nEnsure the private key carries funds on Gnosis Chain.\n\nSecond, run the following command to instruct the mech with `<prompt>` and `<tool>`:\n\n```bash\nmechx interact <prompt> <tool>\n```\n\nExample output:\n```bash\nmechx interact "write a short poem" "openai-text-davinci-003"\nPrompt uploaded: https://gateway.autonolas.tech/ipfs/f01701220ad9e2d5698fbd6c3a4ce61f329590e68a23181772669e543e69decdae316423b\nTransaction sent: https://gnosisscan.io/tx/0xb3a17ef90da6cc7a86e008a3a91bd367d573b406eae53405a4aa981001a5eaf3\nRequest on-chain with id: 15263135923206312300456917202469137903009897852865973093832667165921851537677\nData arrived: https://gateway.autonolas.tech/ipfs/f017012205053a4ae3ef0cf4ed7eff0c2d74dbaf3479fbdeb292472560e7bfaa4cfecfcdc\nData: {\'requestId\': 15263135923206312300456917202469137903009897852865973093832667165921851537677, \'result\': "\\n\\nA sun-filled sky,\\nA soft breeze blowing by,\\nWhere the trees sway in the wind,\\nA peaceful moment I can\'t rewind."}\n```\n\n## Release guide:\n\nFinish edits, bump versions in `pyproject.toml` and `mech_client/__init__.py`, then `poetry lock`, then `rm -rf dist`, then `poetry publish --build --username=<username> --password=<password>`.',
     'author': 'David Minarsch',
     'author_email': 'david.minarsch@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mech_client-0.1.2/PKG-INFO` & `mech_client-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mech-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Basic client to interact with a mech
 Author: David Minarsch
 Author-email: david.minarsch@googlemail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -22,14 +22,20 @@
 
 ## Installation
 
 ```bash
 pip install mech-client
 ```
 
+Then, set a websocket endpoint for Gnosis RPC like so:
+
+```bash
+export WEBSOCKET_ENDPOINT=<YOUR ENDPOINT>
+```
+
 ## CLI:
 
 ```bash
 Usage: mechx [OPTIONS] COMMAND [ARGS]...
 
   Command-line tool for interacting with mechs.
```

