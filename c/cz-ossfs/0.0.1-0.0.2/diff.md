# Comparing `tmp/cz-ossfs-0.0.1.tar.gz` & `tmp/cz-ossfs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz-ossfs-0.0.1.tar", last modified: Tue May 30 13:36:34 2023, max compression
+gzip compressed data, was "cz-ossfs-0.0.2.tar", last modified: Tue May 30 13:48:30 2023, max compression
```

## Comparing `cz-ossfs-0.0.1.tar` & `cz-ossfs-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 13:36:34.397618 cz-ossfs-0.0.1/
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11345 2023-05-30 11:40:20.000000 cz-ossfs-0.0.1/LICENSE
--rw-r--r--   0 lihanmiao   (501) staff       (20)       46 2023-05-30 11:40:20.000000 cz-ossfs-0.0.1/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5596 2023-05-30 13:36:34.397721 cz-ossfs-0.0.1/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4990 2023-05-30 11:40:20.000000 cz-ossfs-0.0.1/README.rst
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1685 2023-05-30 13:36:27.000000 cz-ossfs-0.0.1/pyproject.toml
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1275 2023-05-30 13:36:34.398120 cz-ossfs-0.0.1/setup.cfg
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 13:36:34.394486 cz-ossfs-0.0.1/src/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 13:36:34.396019 cz-ossfs-0.0.1/src/cz_ossfs.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5596 2023-05-30 13:36:34.000000 cz-ossfs-0.0.1/src/cz_ossfs.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)      411 2023-05-30 13:36:34.000000 cz-ossfs-0.0.1/src/cz_ossfs.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-30 13:36:34.000000 cz-ossfs-0.0.1/src/cz_ossfs.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-30 13:32:38.000000 cz-ossfs-0.0.1/src/cz_ossfs.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      631 2023-05-30 13:36:34.000000 cz-ossfs-0.0.1/src/cz_ossfs.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        6 2023-05-30 13:36:34.000000 cz-ossfs-0.0.1/src/cz_ossfs.egg-info/top_level.txt
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 13:36:34.397509 cz-ossfs-0.0.1/src/ossfs/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      303 2023-05-30 11:40:20.000000 cz-ossfs-0.0.1/src/ossfs/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    23854 2023-05-30 11:40:20.000000 cz-ossfs-0.0.1/src/ossfs/async_oss.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     9608 2023-05-30 11:40:20.000000 cz-ossfs-0.0.1/src/ossfs/base.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    19742 2023-05-30 11:40:20.000000 cz-ossfs-0.0.1/src/ossfs/core.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1908 2023-05-30 11:40:20.000000 cz-ossfs-0.0.1/src/ossfs/exceptions.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1741 2023-05-30 11:41:58.000000 cz-ossfs-0.0.1/src/ossfs/file.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3573 2023-05-30 11:40:20.000000 cz-ossfs-0.0.1/src/ossfs/utils.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 13:48:30.740055 cz-ossfs-0.0.2/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11345 2023-05-30 11:40:20.000000 cz-ossfs-0.0.2/LICENSE
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       46 2023-05-30 11:40:20.000000 cz-ossfs-0.0.2/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5596 2023-05-30 13:48:30.740166 cz-ossfs-0.0.2/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4990 2023-05-30 11:40:20.000000 cz-ossfs-0.0.2/README.rst
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1688 2023-05-30 13:48:22.000000 cz-ossfs-0.0.2/pyproject.toml
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1275 2023-05-30 13:48:30.740537 cz-ossfs-0.0.2/setup.cfg
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 13:48:30.737339 cz-ossfs-0.0.2/src/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 13:48:30.739169 cz-ossfs-0.0.2/src/cz_ossfs/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      303 2023-05-30 11:40:20.000000 cz-ossfs-0.0.2/src/cz_ossfs/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    23872 2023-05-30 13:48:22.000000 cz-ossfs-0.0.2/src/cz_ossfs/async_oss.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     9623 2023-05-30 13:48:22.000000 cz-ossfs-0.0.2/src/cz_ossfs/base.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    19757 2023-05-30 13:48:22.000000 cz-ossfs-0.0.2/src/cz_ossfs/core.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1908 2023-05-30 11:40:20.000000 cz-ossfs-0.0.2/src/cz_ossfs/exceptions.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1744 2023-05-30 13:48:22.000000 cz-ossfs-0.0.2/src/cz_ossfs/file.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3576 2023-05-30 13:48:22.000000 cz-ossfs-0.0.2/src/cz_ossfs/utils.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 13:48:30.739959 cz-ossfs-0.0.2/src/cz_ossfs.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5596 2023-05-30 13:48:30.000000 cz-ossfs-0.0.2/src/cz_ossfs.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      432 2023-05-30 13:48:30.000000 cz-ossfs-0.0.2/src/cz_ossfs.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-30 13:48:30.000000 cz-ossfs-0.0.2/src/cz_ossfs.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-30 13:48:30.000000 cz-ossfs-0.0.2/src/cz_ossfs.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      631 2023-05-30 13:48:30.000000 cz-ossfs-0.0.2/src/cz_ossfs.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        9 2023-05-30 13:48:30.000000 cz-ossfs-0.0.2/src/cz_ossfs.egg-info/top_level.txt
```

### Comparing `cz-ossfs-0.0.1/LICENSE` & `cz-ossfs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cz-ossfs-0.0.1/PKG-INFO` & `cz-ossfs-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz-ossfs
-Version: 0.0.1
+Version: 0.0.2
 Summary: fsspec filesystem for OSS
 Home-page: 
 Download-URL: 
 Maintainer-email: 
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cz-ossfs-0.0.1/README.rst` & `cz-ossfs-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `cz-ossfs-0.0.1/pyproject.toml` & `cz-ossfs-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cz-ossfs"
-version = "0.0.1"
+version = "0.0.2"
 
 [build-system]
 requires = ["setuptools>=48", "setuptools_scm[toml]>=6.3.1"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 
@@ -32,15 +32,15 @@
 line_length = 88
 
 [tool.pytest.ini_options]
 addopts = "-ra"
 
 [tool.coverage.run]
 branch = true
-source = ["ossfs", "tests"]
+source = ["cz_ossfs", "tests"]
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 exclude_lines = [
```

### Comparing `cz-ossfs-0.0.1/setup.cfg` & `cz-ossfs-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `cz-ossfs-0.0.1/src/cz_ossfs.egg-info/PKG-INFO` & `cz-ossfs-0.0.2/src/cz_ossfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz-ossfs
-Version: 0.0.1
+Version: 0.0.2
 Summary: fsspec filesystem for OSS
 Home-page: 
 Download-URL: 
 Maintainer-email: 
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cz-ossfs-0.0.1/src/cz_ossfs.egg-info/requires.txt` & `cz-ossfs-0.0.2/src/cz_ossfs.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cz-ossfs-0.0.1/src/ossfs/async_oss.py` & `cz-ossfs-0.0.2/src/cz_ossfs/async_oss.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,30 +33,30 @@
         InitMultipartUploadResult,
         ListBucketsResult,
         PutObjectResult,
         SimplifiedBucketInfo,
         SimplifiedObjectInfo,
     )
 
-logger = logging.getLogger("ossfs")
+logger = logging.getLogger("cz_ossfs")
 
 
 class AioOSSFileSystem(BaseOSSFileSystem, AsyncFileSystem):
     # pylint: disable=abstract-method
     """
     A pythonic file-systems interface to OSS (Object Storage Service)
     Base on async operations.
 
     Examples
     --------
-    >>> ossfs = AioOSSFileSystem(anon=False)
-    >>> ossfs.ls('my-bucket/')
+    >>> cz_ossfs = AioOSSFileSystem(anon=False)
+    >>> cz_ossfs.ls('my-bucket/')
     ['my-file.txt']
 
-    >>> with ossfs.open('my-bucket/my-file.txt', mode='rb') as f:
+    >>> with cz_ossfs.open('my-bucket/my-file.txt', mode='rb') as f:
     ...     print(f.read())
     b'Hello, world!'
     """
 
     # pylint:disable=no-value-for-parameter
 
     protocol = "oss"
@@ -93,15 +93,15 @@
         try:
             return AioBucket(
                 auth=self._auth,
                 endpoint=self._endpoint,
                 bucket_name=bucket_name,
                 connect_timeout=connect_timeout,
                 session=self._session,
-                app_name="ossfs",
+                app_name="cz_ossfs",
             )
         except ClientError as err:
             raise FileNotFoundError(bucket_name) from err
 
     async def set_session(self, refresh: bool = False):
         """Establish a connection session object.
         Returns
@@ -145,15 +145,15 @@
             service: Union[AioService, AioBucket] = self._get_bucket(bucket, timeout)
         else:
             service = AioService(
                 auth=self._auth,
                 endpoint=self._endpoint,
                 session=self._session,
                 connect_timeout=timeout,
-                app_name="ossfs",
+                app_name="cz_ossfs",
             )
         method = getattr(service, method_name, None)
         try:
             if not method:
                 method = getattr(aiooss2, method_name)
                 logger.debug("CALL: %s - %s - %s", method.__name__, args, kwargs)
                 out = method(service, *args, **kwargs)
```

### Comparing `cz-ossfs-0.0.1/src/ossfs/base.py` & `cz-ossfs-0.0.2/src/cz_ossfs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from fsspec.spec import AbstractFileSystem
 from fsspec.utils import stringify_path
 from oss2.auth import AnonymousAuth, Auth, StsAuth
 from oss2.defaults import multiget_threshold
 
 from .file import OSSFile
 
-logger = logging.getLogger("ossfs")
+logger = logging.getLogger("cz_ossfs")
 logging.getLogger("oss2").setLevel(logging.CRITICAL)
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 
 if TYPE_CHECKING:
     from oss2.models import SimplifiedObjectInfo
 
 
@@ -26,15 +26,15 @@
 SIMPLE_TRANSFER_THRESHOLD = multiget_threshold
 
 
 class BaseOSSFileSystem(AbstractFileSystem):
     # pylint: disable=abstract-method
 
     """
-    base class of the ossfs (ossfs) OSS file system access OSS(Object
+    base class of the cz_ossfs (cz_ossfs) OSS file system access OSS(Object
     Storage Service) as if it were a file system.
 
     This exposes a filesystem-like API (ls, cp, open, etc.) on top of OSS
     storage.
 
     Provide credentials with `key` and `secret`, or together with `token`.
     If anonymous leave all these argument empty.
@@ -88,30 +88,30 @@
         else:
             self._auth = AnonymousAuth()
         self._endpoint = endpoint or os.getenv("OSS_ENDPOINT")
         if self._endpoint is None:
             logger.warning(
                 "OSS endpoint is not set, OSSFS could not work properly"
                 "without a endpoint, please set it manually with "
-                "`ossfs.set_endpoint` later"
+                "`cz_ossfs.set_endpoint` later"
             )
 
         super_kwargs = {
             k: kwargs.pop(k)
             for k in ["use_listings_cache", "listings_expiry_time", "max_paths"]
             if k in kwargs
         }  # passed to fsspec superclass
         super().__init__(**super_kwargs)
 
         self._default_block_size = default_block_size or DEFAULT_BLOCK_SIZE
         self._default_cache_type = default_cache_type
 
     def set_endpoint(self, endpoint: str):
         """
-        Reset the endpoint for ossfs
+        Reset the endpoint for cz_ossfs
         endpoint : string (None)
             Default endpoints of the fs
             Endpoints are the adderss where OSS locate
             like: http://oss-cn-hangzhou.aliyuncs.com or
         """
         if not endpoint:
             raise ValueError("Not a valid endpoint")
```

### Comparing `cz-ossfs-0.0.1/src/ossfs/core.py` & `cz-ossfs-0.0.2/src/cz_ossfs/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,29 +22,29 @@
         GetObjectResult,
         InitMultipartUploadResult,
         PutObjectResult,
         SimplifiedObjectInfo,
     )
 
 
-logger = logging.getLogger("ossfs")
+logger = logging.getLogger("cz_ossfs")
 
 
 class OSSFileSystem(BaseOSSFileSystem):  # pylint:disable=too-many-public-methods
     # pylint:disable=no-value-for-parameter
     """
     A pythonic file-systems interface to OSS (Object Storage Service)
 
     Examples
     --------
-    >>> ossfs = OSSFileSystem(anon=False)
-    >>> ossfs.ls('my-bucket/')
+    >>> cz_ossfs = OSSFileSystem(anon=False)
+    >>> cz_ossfs.ls('my-bucket/')
     ['my-file.txt']
 
-    >>> with ossfs.open('my-bucket/my-file.txt', mode='rb') as f:
+    >>> with cz_ossfs.open('my-bucket/my-file.txt', mode='rb') as f:
     ...     print(f.read())
     b'Hello, world!'
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._session = oss2.Session()
@@ -60,15 +60,15 @@
         try:
             return oss2.Bucket(
                 self._auth,
                 self._endpoint,
                 bucket_name,
                 session=self._session,
                 connect_timeout=connect_timeout,
-                app_name="ossfs",
+                app_name="cz_ossfs",
             )
         except oss2.exceptions.ClientError as err:
             raise FileNotFoundError(bucket_name) from err
 
     def _call_oss(
         self,
         method_name: str,
```

### Comparing `cz-ossfs-0.0.1/src/ossfs/exceptions.py` & `cz-ossfs-0.0.2/src/cz_ossfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `cz-ossfs-0.0.1/src/ossfs/file.py` & `cz-ossfs-0.0.2/src/cz_ossfs/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from fsspec.spec import AbstractBufferedFile
 
 if TYPE_CHECKING:
     from .async_oss import AioOSSFileSystem
     from .core import OSSFileSystem
 
 
-logger = logging.getLogger("ossfs")
+logger = logging.getLogger("cz_ossfs")
 logging.getLogger("oss2").setLevel(logging.CRITICAL)
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 
 
 class OSSFile(AbstractBufferedFile):
     """A file living in OSSFileSystem"""
```

### Comparing `cz-ossfs-0.0.1/src/ossfs/utils.py` & `cz-ossfs-0.0.2/src/cz_ossfs/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""utils of ossfs"""
+"""utils of cz_ossfs"""
 import copy
 import inspect
 from functools import wraps
 from typing import Any, Dict, List
 
 
 def _copy_and_pretify_list(
```

