# Comparing `tmp/pilot_platform_object_storage-1.0.0.tar.gz` & `tmp/pilot_platform_object_storage-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot_platform_object_storage-1.0.0.tar", max compression
+gzip compressed data, was "pilot_platform_object_storage-1.1.0.tar", max compression
```

## Comparing `pilot_platform_object_storage-1.0.0.tar` & `pilot_platform_object_storage-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3325 2023-05-25 16:26:46.780757 pilot_platform_object_storage-1.0.0/README.md
--rw-r--r--   0        0        0      120 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/object_storage/__init__.py
--rw-r--r--   0        0        0      324 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/object_storage/clients/__init__.py
--rw-r--r--   0        0        0     4203 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/object_storage/clients/azure_blob_client.py
--rw-r--r--   0        0        0     4778 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/object_storage/clients/azure_container_client.py
--rw-r--r--   0        0        0     1955 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/object_storage/clients/base_container_client.py
--rw-r--r--   0        0        0     1860 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/object_storage/clients/base_file_client.py
--rw-r--r--   0        0        0     1902 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/object_storage/factories.py
--rw-r--r--   0        0        0      239 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/object_storage/managers/__init__.py
--rw-r--r--   0        0        0     3751 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/object_storage/managers/azure_blob_manager.py
--rw-r--r--   0        0        0      727 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/object_storage/managers/base_manager.py
--rw-r--r--   0        0        0      196 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/object_storage/providers/__init__.py
--rw-r--r--   0        0        0     4432 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/object_storage/providers/azure.py
--rw-r--r--   0        0        0      444 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/object_storage/providers/enum.py
--rw-r--r--   0        0        0     1009 2023-05-25 16:26:46.784757 pilot_platform_object_storage-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4265 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.0.0/setup.py
--rw-r--r--   0        0        0     3903 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3325 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/README.md
+-rw-r--r--   0        0        0      120 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/__init__.py
+-rw-r--r--   0        0        0      324 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/clients/__init__.py
+-rw-r--r--   0        0        0     4506 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/clients/azure_blob_client.py
+-rw-r--r--   0        0        0     5162 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/clients/azure_container_client.py
+-rw-r--r--   0        0        0     2143 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/clients/base_container_client.py
+-rw-r--r--   0        0        0     2051 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/clients/base_file_client.py
+-rw-r--r--   0        0        0     1902 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/factories.py
+-rw-r--r--   0        0        0      239 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/managers/__init__.py
+-rw-r--r--   0        0        0     3751 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/managers/azure_blob_manager.py
+-rw-r--r--   0        0        0      727 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/managers/base_manager.py
+-rw-r--r--   0        0        0      196 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/providers/__init__.py
+-rw-r--r--   0        0        0     4902 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/providers/azure.py
+-rw-r--r--   0        0        0      444 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/object_storage/providers/enum.py
+-rw-r--r--   0        0        0     1009 2023-05-30 16:21:58.705974 pilot_platform_object_storage-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4265 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.1.0/setup.py
+-rw-r--r--   0        0        0     3903 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.1.0/PKG-INFO
```

### Comparing `pilot_platform_object_storage-1.0.0/README.md` & `pilot_platform_object_storage-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.0.0/object_storage/clients/azure_blob_client.py` & `pilot_platform_object_storage-1.1.0/object_storage/clients/azure_blob_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,26 +77,33 @@
         file_path: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> None:
         """Download a file from the specified container."""
         key = self._get_blob_name_from_sas()
 
+        await self._create_parent_dir(file_path)
+
         async with BlobClient.from_blob_url(blob_url=self.blob_sas_url, max_chunk_get_size=chunk_size) as blob_client:
             await self._download(blob_client, key, file_path, chunk_size, progress_callback)
 
     async def copy_file_from_url(
         self,
         source_url: str,
     ) -> str:
         """Copies a file from a URL to a blob in the specified container."""
 
         async with BlobClient.from_blob_url(blob_url=self.blob_sas_url) as blob_client:
             return await self._copy_from_url(blob_client, source_url)
 
+    async def delete_file(self) -> None:
+        """Delete a file with all snapshots in a specific container."""
+        async with BlobClient.from_blob_url(blob_url=self.blob_sas_url) as blob_client:
+            return await self._delete(blob_client)
+
     async def get_file_url(
         self,
     ) -> str:
         """Returns the URL that can be used to access the specified file."""
 
         async with BlobClient.from_blob_url(blob_url=self.blob_sas_url) as blob_client:
             return blob_client.url
```

### Comparing `pilot_platform_object_storage-1.0.0/object_storage/clients/azure_container_client.py` & `pilot_platform_object_storage-1.1.0/object_storage/clients/azure_container_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,16 @@
         key: str,
         file_path: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> None:
         """Download a file from the specified container."""
 
+        await self._create_parent_dir(file_path)
+
         async with ContainerClient.from_container_url(
             container_url=self.container_sas_url, max_chunk_get_size=chunk_size
         ) as container_client:
             blob_client = container_client.get_blob_client(key)
             await self._download(blob_client, key, file_path, chunk_size, progress_callback)
 
     async def copy_file_from_url(
@@ -101,14 +103,21 @@
     ) -> str:
         """Copies a file from a URL to a blob in the specified container."""
 
         async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
             blob_client = container_client.get_blob_client(key)
             return await self._copy_from_url(blob_client, source_url)
 
+    async def delete_file(self, key: str) -> None:
+        """Deleted a file with all its snapshots."""
+
+        async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
+            blob_client = container_client.get_blob_client(key)
+            return await self._delete(blob_client)
+
     async def get_file_url(
         self,
         key: str,
     ) -> str:
         """Returns the URL that can be used to access the specified file."""
 
         async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
```

### Comparing `pilot_platform_object_storage-1.0.0/object_storage/clients/base_container_client.py` & `pilot_platform_object_storage-1.1.0/object_storage/clients/base_file_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,63 +7,66 @@
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Dict
 from typing import Optional
 
 
-class BaseContainerClient(ABC):
+class BaseFileClient(ABC):
     """Abstract base class for object storage clients."""
 
     @abstractmethod
     async def upload_file(
         self,
-        key: str,
         file_path: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> Dict[str, Any]:
         """Uploads a file to the specified bucket."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def download_file_to_bytes(
         self,
-        key: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> bytes:
         """Returns content in bytes of the specific file from the specified bucket."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def download_file(
         self,
-        key: str,
         file_path: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> None:
         """Download the specific file from the specified bucket to file_path."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def copy_file_from_url(
         self,
-        key: str,
         source_url: str,
     ) -> str:
         """Copies a file from a URL to a blob in the specified container."""
 
         raise NotImplementedError()
 
     @abstractmethod
+    async def delete_file(
+        self,
+    ) -> None:
+        """Copies a file from a URL to a blob in the specified container."""
+
+        raise NotImplementedError()
+
+    @abstractmethod
     async def get_file_url(
         self,
-        key: str,
     ) -> str:
         """Returns the URL that can be used to access the specified file."""
 
         raise NotImplementedError()
```

### Comparing `pilot_platform_object_storage-1.0.0/object_storage/clients/base_file_client.py` & `pilot_platform_object_storage-1.1.0/object_storage/clients/base_container_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,58 +7,72 @@
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Dict
 from typing import Optional
 
 
-class BaseFileClient(ABC):
+class BaseContainerClient(ABC):
     """Abstract base class for object storage clients."""
 
     @abstractmethod
     async def upload_file(
         self,
+        key: str,
         file_path: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> Dict[str, Any]:
         """Uploads a file to the specified bucket."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def download_file_to_bytes(
         self,
+        key: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> bytes:
         """Returns content in bytes of the specific file from the specified bucket."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def download_file(
         self,
+        key: str,
         file_path: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> None:
         """Download the specific file from the specified bucket to file_path."""
 
         raise NotImplementedError()
 
     @abstractmethod
     async def copy_file_from_url(
         self,
+        key: str,
         source_url: str,
     ) -> str:
         """Copies a file from a URL to a blob in the specified container."""
 
         raise NotImplementedError()
 
     @abstractmethod
+    async def delete_file(
+        self,
+        key: str,
+    ) -> None:
+        """Delete a file in the specified container."""
+
+        raise NotImplementedError()
+
+    @abstractmethod
     async def get_file_url(
         self,
+        key: str,
     ) -> str:
         """Returns the URL that can be used to access the specified file."""
 
         raise NotImplementedError()
```

### Comparing `pilot_platform_object_storage-1.0.0/object_storage/factories.py` & `pilot_platform_object_storage-1.1.0/object_storage/factories.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.0.0/object_storage/managers/azure_blob_manager.py` & `pilot_platform_object_storage-1.1.0/object_storage/managers/azure_blob_manager.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.0.0/object_storage/managers/base_manager.py` & `pilot_platform_object_storage-1.1.0/object_storage/managers/base_manager.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.0.0/object_storage/providers/azure.py` & `pilot_platform_object_storage-1.1.0/object_storage/providers/azure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Copyright (C) 2023 Indoc Research
 #
 # Contact Indoc Research for any questions regarding the use of this source code.
 
-
+from pathlib import Path
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Dict
 from typing import Optional
 from uuid import uuid4
 
 import aiofiles
 import aiofiles.os
+from aiofiles.os import makedirs
 from azure.storage.blob import BlobBlock
 from azure.storage.blob.aio import BlobClient
 
 
 class AzureClient:
     """Base base class for object storage clients."""
 
@@ -82,14 +83,19 @@
         source_url: str,
     ) -> str:
         """Copies a file from a URL to a blob in the specified container."""
 
         resp = await client.start_copy_from_url(source_url=source_url)
         return resp['copy_status']
 
+    async def _delete(self, client: BlobClient) -> None:
+        """Delete the blob and all its snapshots."""
+
+        return await client.delete_blob(delete_snapshots='include')
+
     async def _resume_upload(
         self,
         client: BlobClient,
         key: str,
         file_path: str,
         chunk_size: int = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
@@ -122,7 +128,13 @@
                         await blob_client.stage_block(block_id=block_id, data=chunk)
                         current += chunk_size
                         if progress_callback:
                             await progress_callback(key, current, file_length)
                         uploaded_blocks.append(BlobBlock(block_id=block_id))
 
             await blob_client.commit_block_list(uploaded_blocks)
+
+    async def _create_parent_dir(self, file_path: str) -> None:
+        """The funtion will create the parent folder by the file path."""
+
+        dirname = str(Path(file_path).parent)
+        await makedirs(dirname, exist_ok=True)
```

### Comparing `pilot_platform_object_storage-1.0.0/pyproject.toml` & `pilot_platform_object_storage-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pilot-platform-object-storage"
-version = "1.0.0"
+version = "1.1.0"
 description = "Python library for interacting with multiple object storage APIs."
 authors = ["Indoc Research"]
 readme = "README.md"
 packages = [{include = "object_storage"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pilot_platform_object_storage-1.0.0/setup.py` & `pilot_platform_object_storage-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 install_requires = \
 ['aiofiles>=23.1.0,<24.0.0',
  'aiohttp>=3.8.4,<4.0.0',
  'azure-storage-blob>=12.16.0,<13.0.0']
 
 setup_kwargs = {
     'name': 'pilot-platform-object-storage',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': 'Python library for interacting with multiple object storage APIs.',
     'long_description': '# Pilot Platform Storage Manager\n\n[![Run Tests](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml/badge.svg?branch=develop)](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml)\n[![Python](https://img.shields.io/badge/python-3.9-brightgreen.svg)](https://www.python.org/)\n[![PyPI](https://img.shields.io/pypi/v/pilot-platform-object-storage.svg)](https://pypi.org/project/pilot-platform-object-storage/)\n\nProvides a simple and flexible Python library for efficient and reliable object storage solutions. Enables direct interaction with multiple object storage APIs, starting with Azure Blob API and with plans to add more in the future\n\n\n## Getting Started\n\n### Manager\n```python\nimport asyncio\nfrom object_storage.factories import get_manager\n\nconnection_string = \'DefaultEndpointsProtocol=https;AccountName=pilot;AccountKey=any;EndpointSuffix=core.windows.net\'\nazr_manager = get_manager(\'azure\', connection_string)\n\naccount_sas = asyncio.run(azr_manager.get_account_sas())\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\n\n\nblob_sas = asyncio.run(azr_manager.get_blob_sas(\'test\', \'small.txt\'))\n\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=blob_signature\'\n\n\nblobs_list = asyncio.run(azr_manager.list_objects(\'test\'))\nprint(blobs_list)\n> [<class \'azure.storage.blob._models.BlobProperties\'>, ...]\n\n\nblobs_list = asyncio.run(azr_manager.create_container(\'test\'))\n```\n\n### File Client\n```python\nimport asyncio\nfrom object_storage.factories import get_file_client\n\nblob_sas_url = \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_account_client = get_file_client(\'azure\', blob_sas_url)\nasyncio.run(azr_account_client.upload_file(\'./small.txt\'))\n```\n\n### Container Client\n```python\nimport asyncio\nfrom object_storage.factories import get_container_client\n\ncontainer_sas_url = \'https://pilot.blob.core.windows.net/test?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_account_client = get_file_client(\'azure\', container_sas_url)\nasyncio.run(azr_account_client.upload_file(\'small.txt\', \'./small.txt\'))\n\n```\n\n\n## Installation & Quick Start\nThe latest version of the object-storage package is available on [PyPi](https://pypi.org/project/pilot-platform-object-storage/) and can be installed into another service via Pip.\n\nPip install from PyPi:\n```\npip install pilot-platform-object-storage\n```\n\nIn `pyproject.toml`:\n```\npilot-platform-object-storage = "^<VERSION>"\n```\n\nPip install from a local `.whl` file:\n```\npip install pilot_platform_object_storage-<VERSION>-py3-none-any.whl\n```\n\n## Contribution\n\nYou can contribute the project in following ways:\n\n* Report a bug.\n* Suggest a feature.\n* Open a pull request for fixing issues or adding functionality. Please consider using [pre-commit](https://pre-commit.com) in this case.\n* For general guidelines on how to contribute to the project, please take a look at the [contribution guide](CONTRIBUTING.md).\n',
     'author': 'Indoc Research',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pilot_platform_object_storage-1.0.0/PKG-INFO` & `pilot_platform_object_storage-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-object-storage
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python library for interacting with multiple object storage APIs.
 Author: Indoc Research
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

