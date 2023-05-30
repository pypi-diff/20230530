# Comparing `tmp/hathorlib-0.3.0.tar.gz` & `tmp/hathorlib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hathorlib-0.3.0.tar", max compression
+gzip compressed data, was "hathorlib-0.4.0.tar", max compression
```

## Comparing `hathorlib-0.3.0.tar` & `hathorlib-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0    11342 2022-11-21 16:06:06.688894 hathorlib-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0      441 2022-11-21 16:06:06.689101 hathorlib-0.3.0/README.md
--rw-r--r--   0        0        0      413 2022-11-21 16:06:06.689333 hathorlib-0.3.0/hathorlib/__init__.py
--rw-r--r--   0        0        0    24470 2022-11-21 16:06:06.689542 hathorlib-0.3.0/hathorlib/base_transaction.py
--rw-r--r--   0        0        0     3357 2022-11-21 16:06:06.689725 hathorlib-0.3.0/hathorlib/block.py
--rw-r--r--   0        0        0     5099 2022-11-21 16:06:06.689841 hathorlib-0.3.0/hathorlib/client.py
--rw-r--r--   0        0        0       92 2022-11-21 16:06:06.689981 hathorlib-0.3.0/hathorlib/conf/__init__.py
--rw-r--r--   0        0        0      872 2022-11-21 16:06:06.690079 hathorlib-0.3.0/hathorlib/conf/get_settings.py
--rw-r--r--   0        0        0      352 2022-11-21 16:06:06.690173 hathorlib-0.3.0/hathorlib/conf/mainnet.py
--rw-r--r--   0        0        0     1484 2022-11-21 16:06:06.690275 hathorlib-0.3.0/hathorlib/conf/settings.py
--rw-r--r--   0        0        0      352 2022-11-21 16:06:06.690352 hathorlib-0.3.0/hathorlib/conf/testnet.py
--rw-r--r--   0        0        0     1677 2022-11-21 16:06:06.690454 hathorlib-0.3.0/hathorlib/daa.py
--rw-r--r--   0        0        0     4171 2022-11-21 16:06:06.690577 hathorlib-0.3.0/hathorlib/exceptions.py
--rw-r--r--   0        0        0        0 2022-11-21 16:06:06.690626 hathorlib-0.3.0/hathorlib/py.typed
--rw-r--r--   0        0        0    17098 2022-11-21 16:06:06.690796 hathorlib-0.3.0/hathorlib/scripts.py
--rw-r--r--   0        0        0     8466 2022-11-21 16:06:06.690957 hathorlib-0.3.0/hathorlib/token_creation_tx.py
--rw-r--r--   0        0        0     6097 2022-11-21 16:06:06.691043 hathorlib-0.3.0/hathorlib/transaction.py
--rw-r--r--   0        0        0     6878 2022-11-21 16:06:06.691190 hathorlib-0.3.0/hathorlib/utils.py
--rw-r--r--   0        0        0     2024 2022-11-21 16:06:06.691303 hathorlib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1291 2022-11-21 16:07:10.989329 hathorlib-0.3.0/setup.py
--rw-r--r--   0        0        0     1455 2022-11-21 16:07:10.989522 hathorlib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11342 2022-11-21 16:06:06.688894 hathorlib-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0      441 2022-11-21 16:06:06.689101 hathorlib-0.4.0/README.md
+-rw-r--r--   0        0        0      413 2022-11-21 16:06:06.689333 hathorlib-0.4.0/hathorlib/__init__.py
+-rw-r--r--   0        0        0    24613 2023-05-30 13:56:09.008923 hathorlib-0.4.0/hathorlib/base_transaction.py
+-rw-r--r--   0        0        0     3357 2022-11-21 16:06:06.689725 hathorlib-0.4.0/hathorlib/block.py
+-rw-r--r--   0        0        0     5099 2022-11-21 16:06:06.689841 hathorlib-0.4.0/hathorlib/client.py
+-rw-r--r--   0        0        0       92 2022-11-21 16:06:06.689981 hathorlib-0.4.0/hathorlib/conf/__init__.py
+-rw-r--r--   0        0        0      872 2022-11-21 16:06:06.690079 hathorlib-0.4.0/hathorlib/conf/get_settings.py
+-rw-r--r--   0        0        0      352 2022-11-21 16:06:06.690173 hathorlib-0.4.0/hathorlib/conf/mainnet.py
+-rw-r--r--   0        0        0     1484 2022-11-21 16:06:06.690275 hathorlib-0.4.0/hathorlib/conf/settings.py
+-rw-r--r--   0        0        0      352 2022-11-21 16:06:06.690352 hathorlib-0.4.0/hathorlib/conf/testnet.py
+-rw-r--r--   0        0        0     1677 2022-11-21 16:06:06.690454 hathorlib-0.4.0/hathorlib/daa.py
+-rw-r--r--   0        0        0     4171 2022-11-21 16:06:06.690577 hathorlib-0.4.0/hathorlib/exceptions.py
+-rw-r--r--   0        0        0      672 2023-05-30 13:56:09.009242 hathorlib-0.4.0/hathorlib/nanocontracts/__init__.py
+-rw-r--r--   0        0        0     4466 2023-05-30 13:56:09.009503 hathorlib-0.4.0/hathorlib/nanocontracts/nanocontract.py
+-rw-r--r--   0        0        0        0 2022-11-21 16:06:06.690626 hathorlib-0.4.0/hathorlib/py.typed
+-rw-r--r--   0        0        0    17098 2022-11-21 16:06:06.690796 hathorlib-0.4.0/hathorlib/scripts.py
+-rw-r--r--   0        0        0     8466 2022-11-21 16:06:06.690957 hathorlib-0.4.0/hathorlib/token_creation_tx.py
+-rw-r--r--   0        0        0     6097 2023-05-16 14:32:30.672402 hathorlib-0.4.0/hathorlib/transaction.py
+-rw-r--r--   0        0        0     6878 2022-11-21 16:06:06.691190 hathorlib-0.4.0/hathorlib/utils.py
+-rw-r--r--   0        0        0     1994 2023-05-30 13:56:09.009826 hathorlib-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1335 2023-05-30 13:56:19.290302 hathorlib-0.4.0/setup.py
+-rw-r--r--   0        0        0     1472 2023-05-30 13:56:19.290499 hathorlib-0.4.0/PKG-INFO
```

### Comparing `hathorlib-0.3.0/LICENSE.txt` & `hathorlib-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hathorlib-0.3.0/hathorlib/base_transaction.py` & `hathorlib-0.4.0/hathorlib/base_transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,32 +63,35 @@
 class TxVersion(IntEnum):
     """Versions are sequential for blocks and transactions"""
 
     REGULAR_BLOCK = 0
     REGULAR_TRANSACTION = 1
     TOKEN_CREATION_TRANSACTION = 2
     MERGE_MINED_BLOCK = 3
+    NANO_CONTRACT = 4
 
     @classmethod
     def _missing_(cls, value: Any) -> 'TxVersion':
         # version's first byte is reserved for future use, so we'll ignore it
         assert isinstance(value, int)
         version = value & 0xFF
         if version == value:
             # Prevent infinite recursion when starting TxVerion with wrong version
             raise ValueError('Invalid version.')
         return cls(version)
 
     def get_cls(self) -> Type['BaseTransaction']:
         from hathorlib import Block, TokenCreationTransaction, Transaction
+        from hathorlib.nanocontracts.nanocontract import NanoContract
 
         cls_map: Dict[TxVersion, Type[BaseTransaction]] = {
             TxVersion.REGULAR_BLOCK: Block,
             TxVersion.REGULAR_TRANSACTION: Transaction,
             TxVersion.TOKEN_CREATION_TRANSACTION: TokenCreationTransaction,
+            TxVersion.NANO_CONTRACT: NanoContract,
         }
 
         cls = cls_map.get(self)
 
         if cls is None:
             raise ValueError('Invalid version.')
         else:
```

### Comparing `hathorlib-0.3.0/hathorlib/block.py` & `hathorlib-0.4.0/hathorlib/block.py`

 * *Files identical despite different names*

### Comparing `hathorlib-0.3.0/hathorlib/client.py` & `hathorlib-0.4.0/hathorlib/client.py`

 * *Files identical despite different names*

### Comparing `hathorlib-0.3.0/hathorlib/conf/get_settings.py` & `hathorlib-0.4.0/hathorlib/conf/get_settings.py`

 * *Files identical despite different names*

### Comparing `hathorlib-0.3.0/hathorlib/conf/settings.py` & `hathorlib-0.4.0/hathorlib/conf/settings.py`

 * *Files identical despite different names*

### Comparing `hathorlib-0.3.0/hathorlib/daa.py` & `hathorlib-0.4.0/hathorlib/daa.py`

 * *Files identical despite different names*

### Comparing `hathorlib-0.3.0/hathorlib/exceptions.py` & `hathorlib-0.4.0/hathorlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `hathorlib-0.3.0/hathorlib/scripts.py` & `hathorlib-0.4.0/hathorlib/scripts.py`

 * *Files identical despite different names*

### Comparing `hathorlib-0.3.0/hathorlib/token_creation_tx.py` & `hathorlib-0.4.0/hathorlib/token_creation_tx.py`

 * *Files identical despite different names*

### Comparing `hathorlib-0.3.0/hathorlib/transaction.py` & `hathorlib-0.4.0/hathorlib/transaction.py`

 * *Files identical despite different names*

### Comparing `hathorlib-0.3.0/hathorlib/utils.py` & `hathorlib-0.4.0/hathorlib/utils.py`

 * *Files identical despite different names*

### Comparing `hathorlib-0.3.0/pyproject.toml` & `hathorlib-0.4.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool.poetry]
 name = "hathorlib"
-version = "0.3.0"
+version = "0.4.0"
 description = "Hathor Network base objects library"
 authors = ["Hathor Team <contact@hathor.network>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://hathor.network/"
 repository = "https://github.com/HathorNetwork/python-hathorlib/"
 # https://pypi.org/classifiers/
@@ -29,29 +29,28 @@
     "Operating System :: OS Independent",
     "License :: OSI Approved :: Apache Software License",
 ]
 include = ["hathorlib/py.typed"]
 exclude = ["tests", "tests.*"]
 
 [tool.poetry.dependencies]
-python = ">=3.6,<4.0"
-base58 = ">=2.1.0"
-structlog = {version = ">=20.0.0", optional = true}
-aiohttp = {version = ">=3.7.0", optional = true}
-cryptography = ">=38.0.3"
-pycoin = "^0.92.20220529"
+python = ">=3.9,<4"
+base58 = "~2.1.1"
+structlog = {version = "~22.3.0", optional = true}
+aiohttp = {version = "~3.8.3", optional = true}
+cryptography = "~38.0.3"
+pycoin = "~0.92"
 
-# TODO: We should migrate from asynctest to pytest-asyncio when we raise our minimum Python version to 3.7
 [tool.poetry.dev-dependencies]
-isort = ">=5.7.0"
-mypy = ">=0.812"
-pytest = ">=6.2.0"
-pytest-cov = ">=2.11.0"
-flake8 = "^4.0.1"
-asynctest = "^0.13.0"
+isort = {version = "~5.10.1", extras = ["colors"]}
+mypy = {version = "^1.0.0", markers = "implementation_name == 'cpython'"}
+pytest = "~7.2.0"
+pytest-cov = "~4.0.0"
+flake8 = "~6.0.0"
+pytest-asyncio = "~0.21.0"
 
 [tool.poetry.extras]
 client = ["aiohttp", "structlog"]
 
 [tool.isort]
 combine_as_imports = true
 default_section = "THIRDPARTY"
```

### Comparing `hathorlib-0.3.0/setup.py` & `hathorlib-0.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['hathorlib', 'hathorlib.conf']
+['hathorlib', 'hathorlib.conf', 'hathorlib.nanocontracts']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['base58>=2.1.0', 'cryptography>=38.0.3', 'pycoin>=0.92.20220529,<0.93.0']
+['base58>=2.1.1,<2.2.0', 'cryptography>=38.0.3,<38.1.0', 'pycoin>=0.92,<0.93']
 
 extras_require = \
-{'client': ['structlog>=20.0.0', 'aiohttp>=3.7.0']}
+{'client': ['structlog>=22.3.0,<22.4.0', 'aiohttp>=3.8.3,<3.9.0']}
 
 setup_kwargs = {
     'name': 'hathorlib',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Hathor Network base objects library',
     'long_description': "hathorlib\n=========\n\nHathor Network base library.\n\n## Configuration\n\nTo install dependencies, including optionals, run:\n\n    poetry install -E client\n\n## Running the tests\n\nTo run the tests using poetry virtualenv:\n\n    poetry run make tests\n\nIf are managing virtualenvs without poetry, make sure it's activated and run:\n\n    make tests\n\n## Running linters\n\nTo run linters:\n\n    poetry run make check\n\nOr without poetry venv:\n\n    make check",
     'author': 'Hathor Team',
     'author_email': 'contact@hathor.network',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://hathor.network/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.9,<4',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `hathorlib-0.3.0/PKG-INFO` & `hathorlib-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: hathorlib
-Version: 0.3.0
+Version: 0.4.0
 Summary: Hathor Network base objects library
 Home-page: https://hathor.network/
 License: Apache-2.0
 Author: Hathor Team
 Author-email: contact@hathor.network
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: client
-Requires-Dist: aiohttp (>=3.7.0); extra == "client"
-Requires-Dist: base58 (>=2.1.0)
-Requires-Dist: cryptography (>=38.0.3)
-Requires-Dist: pycoin (>=0.92.20220529,<0.93.0)
-Requires-Dist: structlog (>=20.0.0); extra == "client"
+Requires-Dist: aiohttp (>=3.8.3,<3.9.0); extra == "client"
+Requires-Dist: base58 (>=2.1.1,<2.2.0)
+Requires-Dist: cryptography (>=38.0.3,<38.1.0)
+Requires-Dist: pycoin (>=0.92,<0.93)
+Requires-Dist: structlog (>=22.3.0,<22.4.0); extra == "client"
 Project-URL: Repository, https://github.com/HathorNetwork/python-hathorlib/
 Description-Content-Type: text/markdown
 
 hathorlib
 =========
 
 Hathor Network base library.
```

