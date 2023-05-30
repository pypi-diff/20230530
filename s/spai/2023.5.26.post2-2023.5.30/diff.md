# Comparing `tmp/spai-2023.5.26.post2.tar.gz` & `tmp/spai-2023.5.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2023.5.26.post2.tar", max compression
+gzip compressed data, was "spai-2023.5.30.tar", max compression
```

## Comparing `spai-2023.5.26.post2.tar` & `spai-2023.5.30.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.26.post2/README.md
--rw-r--r--   0        0        0      344 2023-05-26 12:14:57.517714 spai-2023.5.26.post2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.26.post2/spai/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:47:16.135084 spai-2023.5.26.post2/spai/cli/__init__.py
--rw-r--r--   0        0        0     1297 2023-05-21 08:39:35.055997 spai-2023.5.26.post2/spai/cli/cloud.py
--rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.26.post2/spai/cli/commands/__init__.py
--rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.26.post2/spai/cli/commands/hello.py
--rw-r--r--   0        0        0     3165 2023-05-26 11:47:46.887246 spai-2023.5.26.post2/spai/cli/local.py
--rw-r--r--   0        0        0     5617 2023-05-26 12:00:02.150333 spai-2023.5.26.post2/spai/cli/project-template/README.md
--rw-r--r--   0        0        0      648 2023-05-26 11:56:34.213566 spai-2023.5.26.post2/spai/cli/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0     1570 2023-05-26 11:56:34.213566 spai-2023.5.26.post2/spai/cli/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0   780104 2023-05-26 11:56:34.213566 spai-2023.5.26.post2/spai/cli/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0   783403 2023-05-26 11:56:34.213566 spai-2023.5.26.post2/spai/cli/project-template/notebooks/analytics/output.ipynb
--rw-r--r--   0        0        0       54 2023-05-26 11:59:24.882199 spai-2023.5.26.post2/spai/cli/project-template/scripts/downloader/.env.example
--rw-r--r--   0        0        0     1198 2023-05-26 11:56:34.213566 spai-2023.5.26.post2/spai/cli/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0      524 2023-05-26 11:56:34.213566 spai-2023.5.26.post2/spai/cli/project-template/scripts/ndvi/main.py
--rw-r--r--   0        0        0      529 2023-05-26 12:01:08.490568 spai-2023.5.26.post2/spai/cli/project-template/spai.config.yml
--rw-r--r--   0        0        0     1421 2023-05-26 11:56:34.225566 spai-2023.5.26.post2/spai/cli/project-template/uis/map/main.py
--rw-r--r--   0        0        0     3413 2023-05-26 11:46:05.338695 spai-2023.5.26.post2/spai/cli/validate.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.26.post2/spai/data/__init__.py
--rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.26.post2/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.5.26.post2/spai/data/satellite/download.py
--rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.5.26.post2/spai/data/satellite/explore.py
--rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.26.post2/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.5.26.post2/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.5.26.post2/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.26.post2/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.5.26.post2/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.26.post2/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.5.26.post2/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.5.26.post2/spai/image/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.5.26.post2/spai/image/utils.py
--rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.5.26.post2/spai/image/xyz/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.5.26.post2/spai/image/xyz/cache.py
--rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.5.26.post2/spai/image/xyz/errors.py
--rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.5.26.post2/spai/image/xyz/get_image_tile.py
--rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.5.26.post2/spai/image/xyz/image_utils.py
--rw-r--r--   0        0        0     1621 2023-05-26 11:47:17.739093 spai-2023.5.26.post2/spai/main.py
--rw-r--r--   0        0        0     1915 2023-05-26 08:51:56.602852 spai-2023.5.26.post2/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     3605 2023-05-26 08:52:19.331037 spai-2023.5.26.post2/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     2521 2023-05-26 08:52:44.511236 spai-2023.5.26.post2/spai/storage/Storage.py
--rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.5.26.post2/spai/storage/__init__.py
--rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.5.26.post2/spai/storage/minio.py
--rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 spai-2023.5.26.post2/setup.py
--rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 spai-2023.5.26.post2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.30/README.md
+-rw-r--r--   0        0        0      378 2023-05-30 10:06:24.520439 spai-2023.5.30/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.30/spai/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:47:16.135084 spai-2023.5.30/spai/cli/__init__.py
+-rw-r--r--   0        0        0     2522 2023-05-30 10:03:56.192086 spai-2023.5.30/spai/cli/cloud.py
+-rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.30/spai/cli/commands/__init__.py
+-rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.30/spai/cli/commands/hello.py
+-rw-r--r--   0        0        0     3165 2023-05-26 11:47:46.887246 spai-2023.5.30/spai/cli/local.py
+-rw-r--r--   0        0        0     5617 2023-05-26 12:00:02.150333 spai-2023.5.30/spai/cli/project-template/README.md
+-rw-r--r--   0        0        0      648 2023-05-26 11:56:34.213566 spai-2023.5.30/spai/cli/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0     1570 2023-05-26 11:56:34.213566 spai-2023.5.30/spai/cli/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0   780104 2023-05-26 11:56:34.213566 spai-2023.5.30/spai/cli/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0   783403 2023-05-26 11:56:34.213566 spai-2023.5.30/spai/cli/project-template/notebooks/analytics/output.ipynb
+-rw-r--r--   0        0        0       54 2023-05-26 11:59:24.882199 spai-2023.5.30/spai/cli/project-template/scripts/downloader/.env.example
+-rw-r--r--   0        0        0     1198 2023-05-26 11:56:34.213566 spai-2023.5.30/spai/cli/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0      524 2023-05-26 11:56:34.213566 spai-2023.5.30/spai/cli/project-template/scripts/ndvi/main.py
+-rw-r--r--   0        0        0      529 2023-05-26 12:01:08.490568 spai-2023.5.30/spai/cli/project-template/spai.config.yml
+-rw-r--r--   0        0        0     1421 2023-05-26 11:56:34.225566 spai-2023.5.30/spai/cli/project-template/uis/map/main.py
+-rw-r--r--   0        0        0     3432 2023-05-30 08:49:01.617233 spai-2023.5.30/spai/cli/validate.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.30/spai/data/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.30/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.5.30/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.5.30/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.30/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.5.30/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.5.30/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.30/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.5.30/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.30/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.5.30/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.5.30/spai/image/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.5.30/spai/image/utils.py
+-rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.5.30/spai/image/xyz/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.5.30/spai/image/xyz/cache.py
+-rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.5.30/spai/image/xyz/errors.py
+-rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.5.30/spai/image/xyz/get_image_tile.py
+-rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.5.30/spai/image/xyz/image_utils.py
+-rw-r--r--   0        0        0     2937 2023-05-30 09:52:23.466805 spai-2023.5.30/spai/main.py
+-rw-r--r--   0        0        0     1915 2023-05-26 08:51:56.602852 spai-2023.5.30/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     3605 2023-05-26 08:52:19.331037 spai-2023.5.30/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     2521 2023-05-26 08:52:44.511236 spai-2023.5.30/spai/storage/Storage.py
+-rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.5.30/spai/storage/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.5.30/spai/storage/minio.py
+-rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 spai-2023.5.30/setup.py
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 spai-2023.5.30/PKG-INFO
```

### Comparing `spai-2023.5.26.post2/spai/cli/local.py` & `spai-2023.5.30/spai/cli/local.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/cli/project-template/README.md` & `spai-2023.5.30/spai/cli/project-template/README.md`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/cli/project-template/apis/analytics/main.py` & `spai-2023.5.30/spai/cli/project-template/apis/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/cli/project-template/apis/xyz/main.py` & `spai-2023.5.30/spai/cli/project-template/apis/xyz/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/cli/project-template/notebooks/analytics/main.ipynb` & `spai-2023.5.30/spai/cli/project-template/notebooks/analytics/main.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/cli/project-template/notebooks/analytics/output.ipynb` & `spai-2023.5.30/spai/cli/project-template/notebooks/analytics/output.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/cli/project-template/scripts/downloader/main.py` & `spai-2023.5.30/spai/cli/project-template/scripts/downloader/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/cli/project-template/scripts/ndvi/main.py` & `spai-2023.5.30/spai/cli/project-template/scripts/ndvi/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/cli/project-template/spai.config.yml` & `spai-2023.5.30/spai/cli/project-template/spai.config.yml`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/cli/project-template/uis/map/main.py` & `spai-2023.5.30/spai/cli/project-template/uis/map/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/cli/validate.py` & `spai-2023.5.30/spai/cli/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pydantic import BaseModel
 from typing import Union, List
 
 
 class ScriptConfig(BaseModel):
     name: str
     command: Union[str, None] = None
-    run_every: Union[int, None] = None  # seconds
+    run_every: Union[int, None] = None  # seconds (in cloud minutes)
     run_on_start: bool = True
 
 
 class NotebookConfig(BaseModel):
     name: str
     command: Union[str, None] = None
     run_every: Union[int, None] = None  # seconds
```

### Comparing `spai-2023.5.26.post2/spai/data/satellite/download.py` & `spai-2023.5.30/spai/data/satellite/download.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/data/satellite/explore.py` & `spai-2023.5.30/spai/data/satellite/explore.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2023.5.30/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2023.5.30/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2023.5.30/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2023.5.30/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/image/utils.py` & `spai-2023.5.30/spai/image/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/image/xyz/cache.py` & `spai-2023.5.30/spai/image/xyz/cache.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/image/xyz/errors.py` & `spai-2023.5.30/spai/image/xyz/errors.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/image/xyz/get_image_tile.py` & `spai-2023.5.30/spai/image/xyz/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/image/xyz/image_utils.py` & `spai-2023.5.30/spai/image/xyz/image_utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/storage/BaseStorage.py` & `spai-2023.5.30/spai/storage/BaseStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/storage/CloudStorage.py` & `spai-2023.5.30/spai/storage/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/storage/Storage.py` & `spai-2023.5.30/spai/storage/Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/spai/storage/minio.py` & `spai-2023.5.30/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.26.post2/setup.py` & `spai-2023.5.30/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,28 +17,32 @@
  'spai.image.xyz',
  'spai.storage']
 
 package_data = \
 {'': ['*'],
  'spai.cli': ['project-template/*', 'project-template/notebooks/analytics/*']}
 
+install_requires = \
+['minio>=7.1.15,<8.0.0', 'pandas>=2.0.2,<3.0.0']
+
 entry_points = \
 {'console_scripts': ['spai = spai.main:app']}
 
 setup_kwargs = {
     'name': 'spai',
-    'version': '2023.5.26.post2',
+    'version': '2023.5.30',
     'description': '',
     'long_description': '',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

