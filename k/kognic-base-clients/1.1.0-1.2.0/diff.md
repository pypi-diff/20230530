# Comparing `tmp/kognic-base-clients-1.1.0.tar.gz` & `tmp/kognic-base-clients-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kognic-base-clients-1.1.0.tar", last modified: Wed May 10 12:38:25 2023, max compression
+gzip compressed data, was "kognic-base-clients-1.2.0.tar", last modified: Tue May 30 07:00:06 2023, max compression
```

## Comparing `kognic-base-clients-1.1.0.tar` & `kognic-base-clients-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.262431 kognic-base-clients-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.258431 kognic-base-clients-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.258431 kognic-base-clients-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-10 12:38:25.262431 kognic-base-clients-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/flake8.ini
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:38:25.262431 kognic-base-clients-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.258431 kognic-base-clients-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.258431 kognic-base-clients-1.1.0/src/kognic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.258431 kognic-base-clients-1.1.0/src/kognic/base_clients/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 12:38:25.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.262431 kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/download_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/file_resource_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/upload_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/upload_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/retry_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.262431 kognic-base-clients-1.1.0/src/kognic_base_clients.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-10 12:38:25.000000 kognic-base-clients-1.1.0/src/kognic_base_clients.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-10 12:38:25.000000 kognic-base-clients-1.1.0/src/kognic_base_clients.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:38:25.000000 kognic-base-clients-1.1.0/src/kognic_base_clients.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:38:25.000000 kognic-base-clients-1.1.0/src/kognic_base_clients.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 12:38:25.000000 kognic-base-clients-1.1.0/src/kognic_base_clients.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:00:06.165213 kognic-base-clients-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:00:06.157213 kognic-base-clients-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:00:06.157213 kognic-base-clients-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-30 07:00:06.165213 kognic-base-clients-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/flake8.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 07:00:06.165213 kognic-base-clients-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:00:06.153213 kognic-base-clients-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:00:06.153213 kognic-base-clients-1.2.0/src/kognic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:00:06.161213 kognic-base-clients-1.2.0/src/kognic/base_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/src/kognic/base_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 07:00:06.000000 kognic-base-clients-1.2.0/src/kognic/base_clients/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/src/kognic/base_clients/async_retry_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:00:06.161213 kognic-base-clients-1.2.0/src/kognic/base_clients/cloud_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/src/kognic/base_clients/cloud_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/src/kognic/base_clients/cloud_storage/async_file_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/src/kognic/base_clients/cloud_storage/download_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/src/kognic/base_clients/cloud_storage/file_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/src/kognic/base_clients/cloud_storage/upload_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/src/kognic/base_clients/cloud_storage/upload_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/src/kognic/base_clients/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/src/kognic/base_clients/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/src/kognic/base_clients/retry_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/src/kognic/base_clients/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:00:06.165213 kognic-base-clients-1.2.0/src/kognic_base_clients.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-30 07:00:06.000000 kognic-base-clients-1.2.0/src/kognic_base_clients.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-30 07:00:06.000000 kognic-base-clients-1.2.0/src/kognic_base_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 07:00:06.000000 kognic-base-clients-1.2.0/src/kognic_base_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-30 07:00:06.000000 kognic-base-clients-1.2.0/src/kognic_base_clients.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 07:00:06.000000 kognic-base-clients-1.2.0/src/kognic_base_clients.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:00:06.165213 kognic-base-clients-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:00:06.165213 kognic-base-clients-1.2.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/tests/resources/random-data-2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/tests/resources/random-data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/tests/resources/random-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/tests/test_async_download_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/tests/test_async_file_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/tests/test_async_upload_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-30 06:59:49.000000 kognic-base-clients-1.2.0/tests/test_file_resource_client.py
```

### Comparing `kognic-base-clients-1.1.0/.github/workflows/python-package.yml` & `kognic-base-clients-1.2.0/.github/workflows/python-package.yml`

 * *Files 19% similar despite different names*

```diff
@@ -26,16 +26,18 @@
       with:
         python-version: ${{ matrix.python-version }}
         cache: 'pip'
         cache-dependency-path: 'pyproject.toml'
     - name: Install build dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install flake8 pytest
+        python -m pip install flake8 pytest pytest-asyncio pytest-httpx
     - name: Install package
       run: python -m pip install .
+    - name: Test with pytest
+      run: pytest ./tests
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
```

### Comparing `kognic-base-clients-1.1.0/.github/workflows/python-publish.yml` & `kognic-base-clients-1.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kognic-base-clients-1.1.0/CHANGELOG.md` & `kognic-base-clients-1.2.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 Python 3 library for providing a base clients for interacting with the Kognic platform
 
 # Changelog
 
 All notable changes to this library will be documented in this file
 
+## [1.2.0] - 2023-05-30
+
+- Async support for file resource client. The synchronous client is now using async handlers behind the scenes.
 
 ## [1.1.0] - 2023-05-10
 
 - Failed requests will be retried in a wider range of cases than previously, including both API calls and cloud storage.
 
 ## [1.0.3] - 2022-12-02
```

### Comparing `kognic-base-clients-1.1.0/PKG-INFO` & `kognic-base-clients-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kognic-base-clients
-Version: 1.1.0
+Version: 1.2.0
 Summary: Kognic Base Clients
 Author-email: Kognic <scenes-and-predictions@kognic.com>
 License: MIT
 Project-URL: homepage, https://github.com/annotell/kognic-base-clients-python
 Keywords: Kognic,API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,17 @@
 
 Python 3 library for providing a base clients for interacting with the Kognic platform
 
 # Changelog
 
 All notable changes to this library will be documented in this file
 
+## [1.2.0] - 2023-05-30
+
+- Async support for file resource client. The synchronous client is now using async handlers behind the scenes.
 
 ## [1.1.0] - 2023-05-10
 
 - Failed requests will be retried in a wider range of cases than previously, including both API calls and cloud storage.
 
 ## [1.0.3] - 2022-12-02
```

### Comparing `kognic-base-clients-1.1.0/README.md` & `kognic-base-clients-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kognic-base-clients-1.1.0/pyproject.toml` & `kognic-base-clients-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ]
 description = "Kognic Base Clients"
 dependencies = [
     'kognic-auth>=3.0.0,<4',
     'requests>=2.23.0,<3',
     'pydantic>=1.10.0,<2',
     'pyhumps>=3.5.0,<4',
+    "httpx>=0.20,<1",
 ]
 requires-python=">=3.7"
 readme = "CHANGELOG.md"
 keywords = ["Kognic", "API"]
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/download_handler.py` & `kognic-base-clients-1.2.0/src/kognic/base_clients/cloud_storage/download_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,46 @@
 import json
 import logging
-import time
 from typing import Dict
 
-import requests
-from kognic.base_clients.util import RETRYABLE_STATUS_CODES, get_wait_time
-from requests.exceptions import HTTPError, ConnectionError
-from requests.models import Response
+import httpx
+
+from kognic.base_clients.async_retry_support import request_with_retry
 
 log = logging.getLogger(__name__)
 
 
 class DownloadHandler:
 
     def __init__(self, max_retry_attempts: int = 23, max_retry_wait_time: int = 60, timeout: int = 60) -> None:
         """
-        :param max_upload_retry_attempts: Max number of attempts to retry uploading a file to GCS.
-        :param max_upload_retry_wait_time:  Max with time before retrying an upload to GCS.
+        :param max_retry_attempts: Max number of attempts to retry requests to GCS.
+        :param max_retry_wait_time:  Max with time before retrying requests to GCS.
         :param timeout: Max time to wait for response from server.
         """
         self.max_num_retries = max_retry_attempts
         self.max_retry_wait_time = max_retry_wait_time  # seconds
         self.timeout = timeout  # seconds
 
-    def get_json(self, url: str) -> Dict:
-        return json.loads(self._download_file(url, self.max_num_retries))
+    async def get_json(self, url: str) -> Dict:
+        return json.loads(await self._download_file(url, self.max_num_retries))
 
-    def _download_file(self, url: str, number_of_retries: int) -> bytes:
+    async def _download_file(self, url: str, number_of_retries: int) -> bytes:
         """
         Download a json file from cloud storage
 
         :param url: URL of file to download
         :param number_of_retries: Number of download attempts before we stop trying to download
         :return: JSON deserialized to dictionary
         """
-        resp = requests.get(url, timeout=self.timeout)
-        try:
-            resp.raise_for_status()
-        except (HTTPError, ConnectionError) as e:
-            http_condition = number_of_retries > 0 and resp.status_code in RETRYABLE_STATUS_CODES
-            if http_condition or isinstance(e, ConnectionError):
-                self._handle_download_error(resp, number_of_retries)
-                self._download_file(url, number_of_retries - 1)
-            else:
-                raise e
 
-        return resp.content
+        async with httpx.AsyncClient() as httpx_client:
 
-    def _handle_download_error(self, resp: Response, number_of_retries: int) -> None:
-        download_attempt = self.max_num_retries - number_of_retries + 1
-        wait_time = get_wait_time(download_attempt, self.max_retry_wait_time)
-        log.error(
-            f"Failed to download file. Got response: {resp.status_code}: {resp.content}"
-            f"Attempt {download_attempt}/{self.max_num_retries}, retrying in {int(wait_time)} seconds."
-        )
-        time.sleep(wait_time)
+            resp = await request_with_retry(
+                httpx_client.get,
+                number_of_retries,
+                self.max_retry_wait_time,
+                url=url,
+                timeout=self.timeout,
+            )
+
+        return resp.content
```

### Comparing `kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/file_resource_client.py` & `kognic-base-clients-1.2.0/src/kognic/base_clients/cloud_storage/async_file_resource_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 """Client for communicating with the Kognic platform."""
 import logging
-from pathlib import Path
-from typing import Dict, Mapping, Optional, BinaryIO
+from typing import Dict, Mapping, BinaryIO
 
 from kognic.base_clients.cloud_storage.download_handler import DownloadHandler
 from kognic.base_clients.cloud_storage.upload_handler import UploadHandler
 from kognic.base_clients.cloud_storage.upload_spec import UploadSpec
 
 log = logging.getLogger(__name__)
 
 
-class FileResourceClient:
+class AsyncFileResourceClient:
 
     def __init__(self, max_retry_attempts: int = 23, max_retry_wait_time: int = 60, timeout: int = 60):
         """
-        :param max_upload_retry_attempts: Max number of attempts to retry uploading a file to GCS.
-        :param max_upload_retry_wait_time:  Max with time before retrying an upload to GCS.
+        :param max_retry_attempts: Max number of attempts to retry uploading a file to GCS.
+        :param max_retry_wait_time:  Max with time before retrying an upload to GCS.
         :param timeout: Max time to wait for response from server.
         """
         self._upload_handler = UploadHandler(max_retry_attempts, max_retry_wait_time, timeout)
         self._download_handler = DownloadHandler(max_retry_attempts, max_retry_wait_time, timeout)
 
-    def upload_files(self, upload_specs: Mapping[str, UploadSpec]) -> None:
+    async def upload_files(self, upload_specs: Mapping[str, UploadSpec]) -> None:
         """
         Upload all files to cloud storage
 
         :param upload_specs: Mapping from a source name to a destination and source of content for an upload
         """
-        self._upload_handler.upload_files(upload_specs=upload_specs)
+        await self._upload_handler.upload_files(upload_specs=upload_specs)
 
-    def upload_json(self, file: BinaryIO, url: str) -> None:
+    async def upload_json(self, file: BinaryIO, url: str) -> None:
         """
         Upload a single file to storage, using the specified url
         :param file: A binary representation of the file
         :param url: The url ot upload to file to
         """
 
-        self._upload_handler.upload_file(file, url)
+        await self._upload_handler.upload_file(file, url)
 
-    def get_json(self, url: str) -> Dict:
+    async def get_json(self, url: str) -> Dict:
         """
         Downloads a json from cloud storage
 
         :param url: Signed URL to GCS resource to download
         """
-        return self._download_handler.get_json(url)
+        return await self._download_handler.get_json(url)
```

### Comparing `kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/upload_spec.py` & `kognic-base-clients-1.2.0/src/kognic/base_clients/cloud_storage/upload_spec.py`

 * *Files identical despite different names*

### Comparing `kognic-base-clients-1.1.0/src/kognic/base_clients/http_client.py` & `kognic-base-clients-1.2.0/src/kognic/base_clients/http_client.py`

 * *Files identical despite different names*

### Comparing `kognic-base-clients-1.1.0/src/kognic/base_clients/models.py` & `kognic-base-clients-1.2.0/src/kognic/base_clients/models.py`

 * *Files identical despite different names*

### Comparing `kognic-base-clients-1.1.0/src/kognic/base_clients/retry_support.py` & `kognic-base-clients-1.2.0/src/kognic/base_clients/retry_support.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,34 @@
 from kognic.base_clients.util import RETRYABLE_STATUS_CODES, get_wait_time
 
 log = logging.getLogger(__name__)
 
 HTTPErrorHandler = Callable[[HTTPError], None]
 
 
-def request_with_retry(method: Callable[..., Response], max_num_retries: int,
-                       max_retry_wait_time: int, http_error_handler: Optional[HTTPErrorHandler] = None,
-                       *args, **kwargs) -> Response:
-    return _request_with_retry(method, max_num_retries, max_num_retries, max_retry_wait_time, http_error_handler,
-                               *args, **kwargs)
-
-
-def _request_with_retry(method: Callable[..., Response], number_of_retries: int, max_num_retries: int,
-                        max_retry_wait_time: int, http_error_handler: Optional[HTTPErrorHandler] = None,
-                        *args, **kwargs) -> Response:
+def request_with_retry(
+    method: Callable[..., Response],
+    max_num_retries: int,
+    max_retry_wait_time: int,
+    http_error_handler: Optional[HTTPErrorHandler] = None,
+    *args,
+    **kwargs
+) -> Response:
+    return _request_with_retry(method, max_num_retries, max_num_retries, max_retry_wait_time, http_error_handler, *args, **kwargs)
+
+
+def _request_with_retry(
+    method: Callable[..., Response],
+    number_of_retries: int,
+    max_num_retries: int,
+    max_retry_wait_time: int,
+    http_error_handler: Optional[HTTPErrorHandler] = None,
+    *args,
+    **kwargs
+) -> Response:
     """
     Retrying HTTP request with exponential backoff.
 
     :param method: HTTP method executor (probably something like requests.put, auth_session.put).
     :param number_of_retries: Remaining number of retries
     :param max_num_retries: Max number of retry attempts
     :param max_retry_wait_time: Upper bound on wait time between retries (seconds)
@@ -32,16 +42,17 @@
     :param kwargs: kwargs for `method`
     :return: Response
     """
 
     def handle_error(error_type: str, re: RequestException, retries_remaining: int):
         if retries_remaining > 0:
             _generic_error(error_type, retries_remaining, max_num_retries, max_retry_wait_time)
-            return _request_with_retry(method, retries_remaining - 1, max_num_retries, max_retry_wait_time,
-                                       http_error_handler, *args, **kwargs)
+            return _request_with_retry(
+                method, retries_remaining - 1, max_num_retries, max_retry_wait_time, http_error_handler, *args, **kwargs
+            )
         else:
             log.error("Request error, no more retries left", re)
             raise re
 
     try:
         resp = method(*args, **kwargs)
         resp.raise_for_status()
```

### Comparing `kognic-base-clients-1.1.0/src/kognic/base_clients/util.py` & `kognic-base-clients-1.2.0/src/kognic/base_clients/util.py`

 * *Files identical despite different names*

### Comparing `kognic-base-clients-1.1.0/src/kognic_base_clients.egg-info/PKG-INFO` & `kognic-base-clients-1.2.0/src/kognic_base_clients.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kognic-base-clients
-Version: 1.1.0
+Version: 1.2.0
 Summary: Kognic Base Clients
 Author-email: Kognic <scenes-and-predictions@kognic.com>
 License: MIT
 Project-URL: homepage, https://github.com/annotell/kognic-base-clients-python
 Keywords: Kognic,API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,17 @@
 
 Python 3 library for providing a base clients for interacting with the Kognic platform
 
 # Changelog
 
 All notable changes to this library will be documented in this file
 
+## [1.2.0] - 2023-05-30
+
+- Async support for file resource client. The synchronous client is now using async handlers behind the scenes.
 
 ## [1.1.0] - 2023-05-10
 
 - Failed requests will be retried in a wider range of cases than previously, including both API calls and cloud storage.
 
 ## [1.0.3] - 2022-12-02
```

