# Comparing `tmp/mech_client-0.1.3.tar.gz` & `tmp/mech_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mech_client-0.1.3.tar", max compression
+gzip compressed data, was "mech_client-0.1.4.tar", max compression
```

## Comparing `mech_client-0.1.3.tar` & `mech_client-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11339 2023-05-27 20:23:22.952168 mech_client-0.1.3/LICENSE
--rw-r--r--   0        0        0     2037 2023-05-30 10:09:38.116752 mech_client-0.1.3/README.md
--rw-r--r--   0        0        0       22 2023-05-30 10:32:58.756355 mech_client-0.1.3/mech_client/__init__.py
--rw-r--r--   0        0        0     1147 2023-05-30 08:36:18.724247 mech_client-0.1.3/mech_client/cli.py
--rw-r--r--   0        0        0     7257 2023-05-30 10:28:07.483789 mech_client-0.1.3/mech_client/interact.py
--rw-r--r--   0        0        0     1790 2023-05-27 19:55:10.151934 mech_client-0.1.3/mech_client/prompt_to_ipfs.py
--rw-r--r--   0        0        0     1670 2023-05-27 20:02:06.617746 mech_client-0.1.3/mech_client/push_to_ipfs.py
--rw-r--r--   0        0        0      558 2023-05-30 10:32:52.540021 mech_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 mech_client-0.1.3/setup.py
--rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 mech_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-05-27 20:23:22.952168 mech_client-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2037 2023-05-30 10:09:38.116752 mech_client-0.1.4/README.md
+-rw-r--r--   0        0        0       22 2023-05-30 20:37:48.076470 mech_client-0.1.4/mech_client/__init__.py
+-rw-r--r--   0        0        0     1147 2023-05-30 08:36:18.724247 mech_client-0.1.4/mech_client/cli.py
+-rw-r--r--   0        0        0     7414 2023-05-30 20:39:00.456129 mech_client-0.1.4/mech_client/interact.py
+-rw-r--r--   0        0        0     1790 2023-05-27 19:55:10.151934 mech_client-0.1.4/mech_client/prompt_to_ipfs.py
+-rw-r--r--   0        0        0     1670 2023-05-27 20:02:06.617746 mech_client-0.1.4/mech_client/push_to_ipfs.py
+-rw-r--r--   0        0        0      558 2023-05-30 20:37:50.024123 mech_client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 mech_client-0.1.4/setup.py
+-rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 mech_client-0.1.4/PKG-INFO
```

### Comparing `mech_client-0.1.3/LICENSE` & `mech_client-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.3/README.md` & `mech_client-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.3/mech_client/cli.py` & `mech_client-0.1.4/mech_client/cli.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.3/mech_client/interact.py` & `mech_client-0.1.4/mech_client/interact.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 import json
 import os
 import sys
 import time
 import warnings
-from typing import Optional
+from typing import Any, Dict, Optional
 
 import requests
 import websocket
 from aea.contracts.base import Contract
 from aea_ledger_ethereum import EthereumApi, EthereumCrypto
 
 from mech_client.prompt_to_ipfs import push_metadata_to_ipfs
@@ -51,15 +51,15 @@
     "0x4bda649efe6b98b0f9c1d5e859c29e20910f45c66dabfe6fad4a4881f7faf9cc"
 )
 EVENT_SIGNATURE_DELIVER = (
     "0x3ec84da2cdc1ce60c063642b69ff2e65f3b69787a2b90443457ba274e51e7c72"
 )
 WSS_ENDPOINT = os.getenv(
     "WEBSOCKET_ENDPOINT",
-    "wss://gno.getblock.io/3042bb06-d18e-4ce0-8ccf-83eedd35532b/mainnet/",
+    "wss://rpc.eu-central-2.gateway.fm/ws/v4/gnosis/non-archival/mainnet",
 )
 
 # Ignore a specific warning message
 warnings.filterwarnings("ignore", "The log with transaction hash.*")
 
 
 def check_for_tools(tool: str) -> Optional[int]:
@@ -160,17 +160,18 @@
 
 
 def watch_for_events(
     wss: websocket.WebSocket,
     contract_instance: Contract,
     ethereum_ledger_api: EthereumApi,
     ethereum_crypto: EthereumCrypto,
-) -> None:
+) -> Dict[str, Any]:
     """Watches for events on mech."""
     is_waiting = True
+    request_id = None
     while is_waiting:
         msg = wss.recv()
         data = json.loads(msg)
         tx_hash = data["params"]["result"]["transactionHash"]
         no_receipt = True
         while no_receipt:
             try:
@@ -191,17 +192,22 @@
             request_id_ = rich_logs[0]["args"]["requestId"]
             if request_id != request_id_:
                 continue
             data_url = "https://gateway.autonolas.tech/ipfs/f01701220" + data.hex()
             print(f"Data arrived: {data_url}")
             is_waiting = False
     response = requests.get(data_url + "/" + str(request_id))
-    result = response.json()["result"]
+    response_json = response.json()
+    result = response_json["result"]
     print(f"Data:\n{result}")
+    return response_json
 
 
-def interact(prompt: str, tool: str) -> None:
+def interact(prompt: str, tool: str) -> Dict[str, Any]:
     ethereum_crypto = EthereumCrypto(private_key_path=PRIVATE_KEY_FILE_PATH)
     ethereum_ledger_api = EthereumApi(**ETHEREUM_TESTNET_CONFIG)
     wss = register_event_handlers(ethereum_crypto)
     contract_instance = send_request(ethereum_crypto, ethereum_ledger_api, prompt, tool)
-    watch_for_events(wss, contract_instance, ethereum_ledger_api, ethereum_crypto)
+    response = watch_for_events(
+        wss, contract_instance, ethereum_ledger_api, ethereum_crypto
+    )
+    return response
```

### Comparing `mech_client-0.1.3/mech_client/prompt_to_ipfs.py` & `mech_client-0.1.4/mech_client/prompt_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.3/mech_client/push_to_ipfs.py` & `mech_client-0.1.4/mech_client/push_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.3/pyproject.toml` & `mech_client-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mech-client"
-version = "0.1.3"
+version = "0.1.4"
 description = "Basic client to interact with a mech"
 authors = ["David Minarsch <david.minarsch@googlemail.com>"]
 readme = "README.md"
 packages = [{include = "mech_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `mech_client-0.1.3/setup.py` & `mech_client-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'websocket-client>=0.32.0,<1']
 
 entry_points = \
 {'console_scripts': ['mechx = mech_client.cli:cli']}
 
 setup_kwargs = {
     'name': 'mech-client',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Basic client to interact with a mech',
     'long_description': '# mech-client\nBasic client to interact with a mech\n\n> **Warning**<br />\n> **This is a hacky alpha version of the client - don\'t rely on it as production software.**\n\n## Installation\n\n```bash\npip install mech-client\n```\n\nThen, set a websocket endpoint for Gnosis RPC like so:\n\n```bash\nexport WEBSOCKET_ENDPOINT=<YOUR ENDPOINT>\n```\n\n## CLI:\n\n```bash\nUsage: mechx [OPTIONS] COMMAND [ARGS]...\n\n  Command-line tool for interacting with mechs.\n\nOptions:\n  --version  Show the version and exit.\n  --help     Show this message and exit.\n\nCommands:\n  interact        Interact with a mech specifying a prompt and tool.\n  prompt-to-ipfs  Upload a prompt and tool to IPFS as metadata.\n  push-to-ipfs    Upload a file to IPFS.\n ```\n\n## Usage:\n\nFirst, create a private key in file `ethereum_private_key.txt` with this command:\n\n```bash\naea generate-key ethereum\n```\n\nEnsure the private key carries funds on Gnosis Chain.\n\nSecond, run the following command to instruct the mech with `<prompt>` and `<tool>`:\n\n```bash\nmechx interact <prompt> <tool>\n```\n\nExample output:\n```bash\nmechx interact "write a short poem" "openai-text-davinci-003"\nPrompt uploaded: https://gateway.autonolas.tech/ipfs/f01701220ad9e2d5698fbd6c3a4ce61f329590e68a23181772669e543e69decdae316423b\nTransaction sent: https://gnosisscan.io/tx/0xb3a17ef90da6cc7a86e008a3a91bd367d573b406eae53405a4aa981001a5eaf3\nRequest on-chain with id: 15263135923206312300456917202469137903009897852865973093832667165921851537677\nData arrived: https://gateway.autonolas.tech/ipfs/f017012205053a4ae3ef0cf4ed7eff0c2d74dbaf3479fbdeb292472560e7bfaa4cfecfcdc\nData: {\'requestId\': 15263135923206312300456917202469137903009897852865973093832667165921851537677, \'result\': "\\n\\nA sun-filled sky,\\nA soft breeze blowing by,\\nWhere the trees sway in the wind,\\nA peaceful moment I can\'t rewind."}\n```\n\n## Release guide:\n\nFinish edits, bump versions in `pyproject.toml` and `mech_client/__init__.py`, then `poetry lock`, then `rm -rf dist`, then `poetry publish --build --username=<username> --password=<password>`.',
     'author': 'David Minarsch',
     'author_email': 'david.minarsch@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mech_client-0.1.3/PKG-INFO` & `mech_client-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mech-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: Basic client to interact with a mech
 Author: David Minarsch
 Author-email: david.minarsch@googlemail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

