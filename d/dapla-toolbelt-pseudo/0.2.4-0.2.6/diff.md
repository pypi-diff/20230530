# Comparing `tmp/dapla_toolbelt_pseudo-0.2.4.tar.gz` & `tmp/dapla_toolbelt_pseudo-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt_pseudo-0.2.4.tar", max compression
+gzip compressed data, was "dapla_toolbelt_pseudo-0.2.6.tar", max compression
```

## Comparing `dapla_toolbelt_pseudo-0.2.4.tar` & `dapla_toolbelt_pseudo-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1077 2023-05-24 13:07:01.913619 dapla_toolbelt_pseudo-0.2.4/LICENSE
--rw-r--r--   0        0        0     4899 2023-05-24 13:07:01.913619 dapla_toolbelt_pseudo-0.2.4/README.md
--rw-r--r--   0        0        0     2417 2023-05-24 13:07:12.897626 dapla_toolbelt_pseudo-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1147 2023-05-24 13:07:12.897626 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/__init__.py
--rw-r--r--   0        0        0      657 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/constants.py
--rw-r--r--   0        0        0      833 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/models.py
--rw-r--r--   0        0        0        0 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/py.typed
--rw-r--r--   0        0        0      407 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/types.py
--rw-r--r--   0        0        0      888 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/utils.py
--rw-r--r--   0        0        0      316 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/__init__.py
--rw-r--r--   0        0        0    11182 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/client.py
--rw-r--r--   0        0        0     4756 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/models.py
--rw-r--r--   0        0        0    12294 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/ops.py
--rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.4/setup.py
--rw-r--r--   0        0        0     6040 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-30 11:02:56.691491 dapla_toolbelt_pseudo-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4899 2023-05-30 11:02:56.691491 dapla_toolbelt_pseudo-0.2.6/README.md
+-rw-r--r--   0        0        0     2460 2023-05-30 11:03:07.819662 dapla_toolbelt_pseudo-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1147 2023-05-30 11:02:56.695491 dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/__init__.py
+-rw-r--r--   0        0        0      657 2023-05-30 11:02:56.695491 dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/constants.py
+-rw-r--r--   0        0        0      833 2023-05-30 11:02:56.695491 dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/models.py
+-rw-r--r--   0        0        0        0 2023-05-30 11:02:56.695491 dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/py.typed
+-rw-r--r--   0        0        0      455 2023-05-30 11:02:56.695491 dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/types.py
+-rw-r--r--   0        0        0      888 2023-05-30 11:02:56.695491 dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/utils.py
+-rw-r--r--   0        0        0      316 2023-05-30 11:02:56.695491 dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/v1/__init__.py
+-rw-r--r--   0        0        0    11256 2023-05-30 11:02:56.695491 dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/v1/client.py
+-rw-r--r--   0        0        0     4756 2023-05-30 11:02:56.695491 dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/v1/models.py
+-rw-r--r--   0        0        0    12849 2023-05-30 11:02:56.695491 dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/v1/ops.py
+-rw-r--r--   0        0        0     6038 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.6/setup.py
+-rw-r--r--   0        0        0     6085 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.6/PKG-INFO
```

### Comparing `dapla_toolbelt_pseudo-0.2.4/LICENSE` & `dapla_toolbelt_pseudo-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.4/README.md` & `dapla_toolbelt_pseudo-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.4/pyproject.toml` & `dapla_toolbelt_pseudo-0.2.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt-pseudo"
-version = "0.2.4"
+version = "0.2.6"
 description = "Pseudonymization extensions for Dapla Toolbelt"
 authors = ["Team Skyinfrastruktur <dapla@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt-pseudo"
@@ -16,21 +16,22 @@
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-dapla-toolbelt = "^1.3.6"
 pydantic = "^1.10.2"
 pyhumps = "^3.8.0"
 types-requests = "^2.28.11"
 python-magic = "^0.4.27"
 pylibmagic = "^0.2.2"
 cryptography = "39.0.1"
+dapla-toolbelt = "^1.7.0"
+fsspec = "^2023.5.0"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 devtools = "^0.9.0"
@@ -58,14 +59,15 @@
 typeguard = ">=2.13.3"
 types-mock = "^4.0.15.2"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 ipykernel = "^6.21.3"
 pandas-stubs = "^1.5.3.230304"
 nbstripout = "^0.6.1"
 ipython = "^8.11.0"
+jupyterlab = "^4.0.0"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/__init__.py` & `dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/constants.py` & `dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/constants.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/models.py` & `dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/utils.py` & `dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/utils.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/client.py` & `dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/v1/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,18 @@
         self, path: str, request: APIModel, data: t.BinaryIO, name: str, content_type: Mimetypes, stream: bool = False
     ) -> requests.Response:
         auth_token = self.__auth_token()
         data_spec: _FileSpecDecl = (name, data, content_type)
         request_spec: _FileSpecDecl = (None, request.to_json(), str(Mimetypes.JSON))
         response = requests.post(
             url=f"{self.pseudo_service_url}/{path}",
-            headers={"Authorization": f"Bearer {auth_token}"},
+            headers={
+                "Authorization": f"Bearer {auth_token}",
+                "Accept-Encoding": "gzip",
+            },
             files={
                 "data": data_spec,
                 "request": request_spec,
             },
             stream=stream,
             timeout=30,  # seconds
         )
```

### Comparing `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/models.py` & `dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/v1/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/ops.py` & `dapla_toolbelt_pseudo-0.2.6/src/dapla_pseudo/v1/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 """
 import io
 import mimetypes
 import os
 import typing as t
 from pathlib import Path
 
+import fsspec.spec
+
 
 # isort: off
 import pylibmagic  # noqa Must be imported before magic
 
 # isort: on
 import magic
 import pandas as pd
@@ -89,40 +91,48 @@
     # Avoid later type errors by making sure we have lists
     if fields is None:
         fields = []
     if sid_fields is None:
         sid_fields = []
 
     file_handle: t.Optional[_BinaryFileDecl] = None
+    name: t.Optional[str] = None
     match dataset:
         case str() | Path():
             # File path
             content_type = Mimetypes(magic.from_file(dataset, mime=True))
         case pd.DataFrame():
             # Dataframe
             content_type = Mimetypes.JSON
             file_handle = _dataframe_to_json(dataset, fields, sid_fields)
         case io.BufferedReader():
             # File handle
             content_type = Mimetypes(magic.from_buffer(dataset.read(2048), mime=True))
             dataset.seek(0)
             file_handle = dataset
+        case fsspec.spec.AbstractBufferedFile():
+            # This is a file handle to a remote storage system such as GCS.
+            # It provides random access for the underlying file-like data (without downloading the whole thing).
+            content_type = Mimetypes(magic.from_buffer(dataset.read(2048), mime=True))
+            name = dataset.path.split("/")[-1] if hasattr(dataset, "path") else None
+            dataset.seek(0)
+            file_handle = io.BufferedReader(dataset)
         case _:
             raise ValueError(f"Unsupported data type: {type(dataset)}. Supported types are {_DatasetDecl}")
     k = KeyWrapper(key)
     rules = _rules_of(fields=fields, sid_fields=sid_fields or [], key=k.key_id)
     pseudonymize_request = PseudonymizeFileRequest(
         pseudo_config=PseudoConfig(rules=rules, keysets=k.keyset_list()),
         target_content_type=content_type,
         target_uri=None,
         compression=None,
     )
 
     if file_handle is not None:
-        return _client().pseudonymize(pseudonymize_request, file_handle, stream=stream)
+        return _client().pseudonymize(pseudonymize_request, file_handle, stream=stream, name=name)
     else:
         return _client()._process_file("pseudonymize", pseudonymize_request, str(dataset), stream=stream)
 
 
 def depseudonymize(
     file_path: str,
     fields: t.List[_FieldDecl],
```

### Comparing `dapla_toolbelt_pseudo-0.2.4/setup.py` & `dapla_toolbelt_pseudo-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 ['dapla_pseudo', 'dapla_pseudo.v1']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['cryptography==39.0.1',
- 'dapla-toolbelt>=1.3.6,<2.0.0',
+ 'dapla-toolbelt>=1.7.0,<2.0.0',
+ 'fsspec>=2023.5.0,<2024.0.0',
  'pydantic>=1.10.2,<2.0.0',
  'pyhumps>=3.8.0,<4.0.0',
  'pylibmagic>=0.2.2,<0.3.0',
  'python-magic>=0.4.27,<0.5.0',
  'types-requests>=2.28.11,<3.0.0']
 
 setup_kwargs = {
     'name': 'dapla-toolbelt-pseudo',
-    'version': '0.2.4',
+    'version': '0.2.6',
     'description': 'Pseudonymization extensions for Dapla Toolbelt',
     'long_description': '# Pseudonymization extensions for Dapla Toolbelt\n\n[![PyPI](https://img.shields.io/pypi/v/dapla-toolbelt-pseudo.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/dapla-toolbelt-pseudo.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/dapla-toolbelt-pseudo)][python version]\n[![License](https://img.shields.io/pypi/l/dapla-toolbelt-pseudo)][license]\n\n[![Tests](https://github.com/statisticsnorway/dapla-toolbelt-pseudo/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/statisticsnorway/dapla-toolbelt-pseudo/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/dapla-toolbelt-pseudo/\n[status]: https://pypi.org/project/dapla-toolbelt-pseudo/\n[python version]: https://pypi.org/project/dapla-toolbelt-pseudo\n[tests]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/statisticsnorway/dapla-toolbelt-pseudo\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\nPseudonymize, repseudonymize and depseudonymize data on Dapla.\n\n## Usage\n\nSee the [command-line reference] for details.\n\n### Pseudonymize\n\n```python\nfrom dapla_pseudo import pseudonymize\n\n# Pseudonymize fields in a local file using the default key:\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"])\n\n# Pseudonymize fields in a local file, explicitly denoting the key to use:\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"], key="ssb-common-key-1")\n\n# Pseudonymize a local file using a custom key:\nimport json\ncustom_keyset = json.dumps(    {\n    "encryptedKeyset": "CiQAp91NBhLdknX3j9jF6vwhdyURaqcT9/M/iczV7fLn...8XYFKwxiwMtCzDT6QGzCCCM=",\n    "keysetInfo": {\n        "primaryKeyId": 1234567890,\n        "keyInfo": [\n            {\n                "typeUrl": "type.googleapis.com/google.crypto.tink.AesSivKey",\n                "status": "ENABLED",\n                "keyId": 1234567890,\n                "outputPrefixType": "TINK",\n            }\n        ],\n    },\n    "kekUri": "gcp-kms://projects/some-project-id/locations/europe-north1/keyRings/some-keyring/cryptoKeys/some-kek-1",\n})\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"], key=custom_keyset)\n\n# Operate on data in a streaming manner:\nimport shutil\nwith pseudonymize("./data/personer.json", fields=["fnr", "fornavn", "etternavn"], stream=True) as res:\n    with open("./data/personer_deid.json", \'wb\') as f:\n        res.raw.decode_content = True\n        shutil.copyfileobj(res.raw, f)\n\n# Map certain fields to stabil ID\npseudonymize(file_path="./data/personer.json", fields=["fornavn"], sid_fields=["fnr"])\n```\n\n### Repseudonymize\n\n```python\nfrom dapla_pseudo import repseudonymize\n\n# Repseudonymize fields in a local file, denoting source and target keys to use:\nrepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"], source_key="ssb-common-key-1", target_key="ssb-common-key-2")\n```\n\n### Depseudonymize\n\n```python\nfrom dapla_pseudo import depseudonymize\n\n# Depseudonymize fields in a local file using the default key:\ndepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"])\n\n# Depseudonymize fields in a local file, explicitly denoting the key to use:\ndepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"], key="ssb-common-key-1")\n```\n\n_Note that depseudonymization requires elevated access privileges._\n\n## Requirements\n\n- [Dapla Toolbelt](https://github.com/statisticsnorway/dapla-toolbelt)\n\n## Installation\n\nYou can install _dapla-toolbelt-pseudo_ via [pip] from [PyPI]:\n\n```console\npip install dapla-toolbelt-pseudo\n```\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Pseudonymization extensions for Dapla Toolbelt_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/blob/main/LICENSE\n[contributor guide]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/blob/main/CONTRIBUTING.md\n[command-line reference]: https://statisticsnorway.github.io/dapla-toolbelt-pseudo\n',
     'author': 'Team Skyinfrastruktur',
     'author_email': 'dapla@ssb.no',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/statisticsnorway/dapla-toolbelt-pseudo',
```

### Comparing `dapla_toolbelt_pseudo-0.2.4/PKG-INFO` & `dapla_toolbelt_pseudo-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt-pseudo
-Version: 0.2.4
+Version: 0.2.6
 Summary: Pseudonymization extensions for Dapla Toolbelt
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 License: MIT
 Author: Team Skyinfrastruktur
 Author-email: dapla@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (==39.0.1)
-Requires-Dist: dapla-toolbelt (>=1.3.6,<2.0.0)
+Requires-Dist: dapla-toolbelt (>=1.7.0,<2.0.0)
+Requires-Dist: fsspec (>=2023.5.0,<2024.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: pylibmagic (>=0.2.2,<0.3.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: types-requests (>=2.28.11,<3.0.0)
 Project-URL: Changelog, https://github.com/statisticsnorway/dapla-toolbelt-pseudo/releases
 Project-URL: Documentation, https://statisticsnorway.github.io/dapla-toolbelt-pseudo
```

