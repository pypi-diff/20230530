# Comparing `tmp/mech_client-0.1.1.tar.gz` & `tmp/mech_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mech_client-0.1.1.tar", max compression
+gzip compressed data, was "mech_client-0.1.2.tar", max compression
```

## Comparing `mech_client-0.1.1.tar` & `mech_client-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11339 2023-05-27 20:23:22.952168 mech_client-0.1.1/LICENSE
--rw-r--r--   0        0        0     1926 2023-05-27 20:25:03.823431 mech_client-0.1.1/README.md
--rw-r--r--   0        0        0       22 2023-05-27 20:57:37.902490 mech_client-0.1.1/mech_client/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-27 20:22:42.943820 mech_client-0.1.1/mech_client/cli.py
--rw-r--r--   0        0        0     5667 2023-05-27 20:22:52.167601 mech_client-0.1.1/mech_client/interact.py
--rw-r--r--   0        0        0     1790 2023-05-27 19:55:10.151934 mech_client-0.1.1/mech_client/prompt_to_ipfs.py
--rw-r--r--   0        0        0     1670 2023-05-27 20:02:06.617746 mech_client-0.1.1/mech_client/push_to_ipfs.py
--rw-r--r--   0        0        0      558 2023-05-27 20:57:32.700887 mech_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2843 1970-01-01 00:00:00.000000 mech_client-0.1.1/setup.py
--rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 mech_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-05-27 20:23:22.952168 mech_client-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1926 2023-05-27 20:25:03.823431 mech_client-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-05-30 08:39:49.524762 mech_client-0.1.2/mech_client/__init__.py
+-rw-r--r--   0        0        0     1147 2023-05-30 08:36:18.724247 mech_client-0.1.2/mech_client/cli.py
+-rw-r--r--   0        0        0     5631 2023-05-30 08:36:32.071823 mech_client-0.1.2/mech_client/interact.py
+-rw-r--r--   0        0        0     1790 2023-05-27 19:55:10.151934 mech_client-0.1.2/mech_client/prompt_to_ipfs.py
+-rw-r--r--   0        0        0     1670 2023-05-27 20:02:06.617746 mech_client-0.1.2/mech_client/push_to_ipfs.py
+-rw-r--r--   0        0        0      558 2023-05-30 08:39:25.067038 mech_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2843 1970-01-01 00:00:00.000000 mech_client-0.1.2/setup.py
+-rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 mech_client-0.1.2/PKG-INFO
```

### Comparing `mech_client-0.1.1/LICENSE` & `mech_client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.1/README.md` & `mech_client-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.1/mech_client/cli.py` & `mech_client-0.1.2/mech_client/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 
 @click.command()
 @click.argument("prompt")
 @click.argument("tool")
 def interact(prompt: str, tool: str) -> None:
     """Interact with a mech specifying a prompt and tool."""
     interact_(prompt=prompt, tool=tool)
-    import pdb
-
-    pdb.set_trace()
 
 
 @click.command()
 @click.argument("prompt")
 @click.argument("tool")
 def prompt_to_ipfs(prompt: str, tool: str) -> None:
     """Upload a prompt and tool to IPFS as metadata."""
```

### Comparing `mech_client-0.1.1/mech_client/interact.py` & `mech_client-0.1.2/mech_client/interact.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,12 +149,9 @@
             print(f"Data arrived: {data_url}")
         count += 1
     response = requests.get(data_url + "/" + str(request_id))
     print(f"Data: {response.json()}")
 
 
 def interact(prompt: str, tool: str) -> None:
-    import pdb
-
-    pdb.set_trace()
     contract_instance, ethereum_ledger_api = send_request(prompt, tool)
     watch_for_events(contract_instance, ethereum_ledger_api)
```

### Comparing `mech_client-0.1.1/mech_client/prompt_to_ipfs.py` & `mech_client-0.1.2/mech_client/prompt_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.1/mech_client/push_to_ipfs.py` & `mech_client-0.1.2/mech_client/push_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.1/pyproject.toml` & `mech_client-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mech-client"
-version = "0.1.1"
+version = "0.1.2"
 description = "Basic client to interact with a mech"
 authors = ["David Minarsch <david.minarsch@googlemail.com>"]
 readme = "README.md"
 packages = [{include = "mech_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `mech_client-0.1.1/setup.py` & `mech_client-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'websocket-client>=0.32.0,<1']
 
 entry_points = \
 {'console_scripts': ['mechx = mech_client.cli:cli']}
 
 setup_kwargs = {
     'name': 'mech-client',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Basic client to interact with a mech',
     'long_description': '# mech-client\nBasic client to interact with a mech\n\n> **Warning**<br />\n> **This is a hacky alpha version of the client - don\'t rely on it as production software.**\n\n## Installation\n\n```bash\npip install mech-client\n```\n\n## CLI:\n\n```bash\nUsage: mechx [OPTIONS] COMMAND [ARGS]...\n\n  Command-line tool for interacting with mechs.\n\nOptions:\n  --version  Show the version and exit.\n  --help     Show this message and exit.\n\nCommands:\n  interact        Interact with a mech specifying a prompt and tool.\n  prompt-to-ipfs  Upload a prompt and tool to IPFS as metadata.\n  push-to-ipfs    Upload a file to IPFS.\n ```\n\n## Usage:\n\nFirst, create a private key in file `ethereum_private_key.txt` with this command:\n\n```bash\naea generate-key ethereum\n```\n\nEnsure the private key carries funds on Gnosis Chain.\n\nSecond, run the following command to instruct the mech with `<prompt>` and `<tool>`:\n\n```bash\nmechx interact <prompt> <tool>\n```\n\nExample output:\n```bash\nmechx interact "write a short poem" "openai-text-davinci-003"\nPrompt uploaded: https://gateway.autonolas.tech/ipfs/f01701220ad9e2d5698fbd6c3a4ce61f329590e68a23181772669e543e69decdae316423b\nTransaction sent: https://gnosisscan.io/tx/0xb3a17ef90da6cc7a86e008a3a91bd367d573b406eae53405a4aa981001a5eaf3\nRequest on-chain with id: 15263135923206312300456917202469137903009897852865973093832667165921851537677\nData arrived: https://gateway.autonolas.tech/ipfs/f017012205053a4ae3ef0cf4ed7eff0c2d74dbaf3479fbdeb292472560e7bfaa4cfecfcdc\nData: {\'requestId\': 15263135923206312300456917202469137903009897852865973093832667165921851537677, \'result\': "\\n\\nA sun-filled sky,\\nA soft breeze blowing by,\\nWhere the trees sway in the wind,\\nA peaceful moment I can\'t rewind."}\n```\n\n## Release guide:\n\nFinish edits, bump versions in `pyproject.toml` and `mech_client/__init__.py`, then `poetry lock`, then `rm -rf dist`, then `poetry publish --build --username=<username> --password=<password>`.',
     'author': 'David Minarsch',
     'author_email': 'david.minarsch@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mech_client-0.1.1/PKG-INFO` & `mech_client-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mech-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Basic client to interact with a mech
 Author: David Minarsch
 Author-email: david.minarsch@googlemail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

