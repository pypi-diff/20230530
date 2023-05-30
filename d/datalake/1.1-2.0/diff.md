# Comparing `tmp/datalake-1.1.tar.gz` & `tmp/datalake-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datalake-1.1.tar", last modified: Fri May  6 18:45:23 2022, max compression
+gzip compressed data, was "dist/datalake-2.0.tar", last modified: Tue May 30 20:37:56 2023, max compression
```

## Comparing `datalake-1.1.tar` & `datalake-2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-06 18:45:23.952287 datalake-1.1/
--rw-rw-rw-   0 root         (0) root         (0)       51 2021-10-15 23:46:15.000000 datalake-1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      524 2022-05-06 18:45:23.952287 datalake-1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11986 2021-10-15 23:46:15.000000 datalake-1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-06 18:45:23.952287 datalake-1.1/datalake/
--rw-rw-rw-   0 root         (0) root         (0)     1424 2021-10-15 23:46:15.000000 datalake-1.1/datalake/__init__.py
--rw-r--r--   0 root         (0) root         (0)      495 2022-05-06 18:45:23.952287 datalake-1.1/datalake/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    15663 2022-05-05 18:26:13.000000 datalake-1.1/datalake/archive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-06 18:45:23.948287 datalake-1.1/datalake/common/
--rw-rw-rw-   0 root         (0) root         (0)      852 2021-10-15 23:46:15.000000 datalake-1.1/datalake/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2968 2021-10-15 23:46:15.000000 datalake-1.1/datalake/common/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      783 2021-10-15 23:46:15.000000 datalake-1.1/datalake/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     7098 2022-05-05 18:26:13.000000 datalake-1.1/datalake/common/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     6701 2022-05-05 18:26:13.000000 datalake-1.1/datalake/common/record.py
--rw-rw-rw-   0 root         (0) root         (0)     1166 2021-10-15 23:46:15.000000 datalake-1.1/datalake/config_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1936 2021-10-15 23:46:15.000000 datalake-1.1/datalake/crtime.py
--rw-rw-rw-   0 root         (0) root         (0)    11143 2022-05-05 18:26:13.000000 datalake-1.1/datalake/dlfile.py
--rw-rw-rw-   0 root         (0) root         (0)     1787 2022-03-23 22:53:22.000000 datalake-1.1/datalake/logging_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     8664 2021-10-15 23:46:15.000000 datalake-1.1/datalake/queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-06 18:45:23.948287 datalake-1.1/datalake/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-10-15 23:46:15.000000 datalake-1.1/datalake/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9424 2022-05-05 18:26:13.000000 datalake-1.1/datalake/scripts/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-06 18:45:23.948287 datalake-1.1/datalake/tests/
--rw-rw-rw-   0 root         (0) root         (0)      615 2021-10-15 23:46:15.000000 datalake-1.1/datalake/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2022-05-05 18:26:13.000000 datalake-1.1/datalake/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2116 2021-10-15 23:46:15.000000 datalake-1.1/datalake/tests/test_conf.py
--rw-rw-rw-   0 root         (0) root         (0)     5942 2021-10-15 23:46:15.000000 datalake-1.1/datalake/tests/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     4494 2022-03-23 22:53:22.000000 datalake-1.1/datalake/tests/test_record.py
--rw-rw-rw-   0 root         (0) root         (0)     3329 2021-10-15 23:46:15.000000 datalake-1.1/datalake/translator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-06 18:45:23.948287 datalake-1.1/datalake.egg-info/
--rw-r--r--   0 root         (0) root         (0)      524 2022-05-06 18:45:23.000000 datalake-1.1/datalake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      990 2022-05-06 18:45:23.000000 datalake-1.1/datalake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-06 18:45:23.000000 datalake-1.1/datalake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2022-05-06 18:45:23.000000 datalake-1.1/datalake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      340 2022-05-06 18:45:23.000000 datalake-1.1/datalake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-05-06 18:45:23.000000 datalake-1.1/datalake.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-05-06 18:45:23.952287 datalake-1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1833 2022-05-06 16:07:12.000000 datalake-1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-06 18:45:23.952287 datalake-1.1/test/
--rw-rw-rw-   0 root         (0) root         (0)     2140 2022-05-05 18:26:13.000000 datalake-1.1/test/test_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     3483 2022-03-23 22:53:22.000000 datalake-1.1/test/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2021-10-15 23:46:15.000000 datalake-1.1/test/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1220 2021-10-15 23:46:15.000000 datalake-1.1/test/test_crtime.py
--rw-rw-rw-   0 root         (0) root         (0)     8342 2021-10-15 23:46:15.000000 datalake-1.1/test/test_fetch.py
--rw-rw-rw-   0 root         (0) root         (0)     5578 2022-05-05 18:26:13.000000 datalake-1.1/test/test_file.py
--rw-rw-rw-   0 root         (0) root         (0)     2080 2021-10-15 23:46:15.000000 datalake-1.1/test/test_latest.py
--rw-rw-rw-   0 root         (0) root         (0)    11863 2022-05-05 18:26:13.000000 datalake-1.1/test/test_list.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2021-10-15 23:46:15.000000 datalake-1.1/test/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     7976 2022-03-23 22:53:22.000000 datalake-1.1/test/test_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2021-10-15 23:46:15.000000 datalake-1.1/test/test_translator.py
--rw-rw-rw-   0 root         (0) root         (0)    68611 2021-10-15 23:46:15.000000 datalake-1.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 20:37:56.677403 datalake-2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-28 14:18:26.000000 datalake-2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      524 2023-05-30 20:37:56.677403 datalake-2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11986 2023-05-28 14:18:26.000000 datalake-2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 20:37:56.677403 datalake-2.0/datalake/
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-05-28 14:18:26.000000 datalake-2.0/datalake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      495 2023-05-30 20:37:56.677403 datalake-2.0/datalake/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    15591 2023-05-28 14:18:26.000000 datalake-2.0/datalake/archive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 20:37:56.673403 datalake-2.0/datalake/common/
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-28 14:18:26.000000 datalake-2.0/datalake/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2023-05-28 14:18:26.000000 datalake-2.0/datalake/common/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2023-05-28 14:18:26.000000 datalake-2.0/datalake/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7098 2023-05-28 14:18:26.000000 datalake-2.0/datalake/common/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     7231 2023-05-30 20:33:24.000000 datalake-2.0/datalake/common/record.py
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2023-05-28 14:18:26.000000 datalake-2.0/datalake/config_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-05-28 14:18:26.000000 datalake-2.0/datalake/crtime.py
+-rw-rw-rw-   0 root         (0) root         (0)    11143 2023-05-28 14:18:26.000000 datalake-2.0/datalake/dlfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2023-05-28 14:18:26.000000 datalake-2.0/datalake/logging_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     8664 2023-05-28 14:18:26.000000 datalake-2.0/datalake/queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 20:37:56.673403 datalake-2.0/datalake/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 20:37:54.000000 datalake-2.0/datalake/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9424 2023-05-28 14:18:26.000000 datalake-2.0/datalake/scripts/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 20:37:56.673403 datalake-2.0/datalake/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-05-28 14:18:26.000000 datalake-2.0/datalake/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2023-05-28 14:18:26.000000 datalake-2.0/datalake/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2116 2023-05-28 14:18:26.000000 datalake-2.0/datalake/tests/test_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2023-05-28 14:18:26.000000 datalake-2.0/datalake/tests/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     4494 2023-05-28 14:18:26.000000 datalake-2.0/datalake/tests/test_record.py
+-rw-rw-rw-   0 root         (0) root         (0)     3329 2023-05-28 14:18:26.000000 datalake-2.0/datalake/translator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 20:37:56.673403 datalake-2.0/datalake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      524 2023-05-30 20:37:56.000000 datalake-2.0/datalake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      990 2023-05-30 20:37:56.000000 datalake-2.0/datalake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 20:37:56.000000 datalake-2.0/datalake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-30 20:37:56.000000 datalake-2.0/datalake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      344 2023-05-30 20:37:56.000000 datalake-2.0/datalake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-30 20:37:56.000000 datalake-2.0/datalake.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-05-30 20:37:56.677403 datalake-2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2023-05-28 14:18:26.000000 datalake-2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 20:37:56.677403 datalake-2.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2023-05-28 14:18:26.000000 datalake-2.0/test/test_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3479 2023-05-28 14:18:26.000000 datalake-2.0/test/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-05-28 14:18:26.000000 datalake-2.0/test/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1220 2023-05-28 14:18:26.000000 datalake-2.0/test/test_crtime.py
+-rw-rw-rw-   0 root         (0) root         (0)     8342 2023-05-28 14:18:26.000000 datalake-2.0/test/test_fetch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5578 2023-05-28 14:18:26.000000 datalake-2.0/test/test_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2023-05-28 14:18:26.000000 datalake-2.0/test/test_latest.py
+-rw-rw-rw-   0 root         (0) root         (0)    11863 2023-05-28 14:18:26.000000 datalake-2.0/test/test_list.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-05-28 14:18:26.000000 datalake-2.0/test/test_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     8381 2023-05-28 14:18:26.000000 datalake-2.0/test/test_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2023-05-28 14:18:26.000000 datalake-2.0/test/test_translator.py
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-05-28 14:18:26.000000 datalake-2.0/versioneer.py
```

### Comparing `datalake-1.1/PKG-INFO` & `datalake-2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalake
-Version: 1.1
+Version: 2.0
 Summary: datalake: a metadata-aware archive
 Home-page: https://github.com/planetlabs/datalake
 Author: Brian Cavagnolo
 Author-email: brian@planet.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `datalake-1.1/README.md` & `datalake-2.0/README.md`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/__init__.py` & `datalake-2.0/datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/archive.py` & `datalake-2.0/datalake/archive.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,17 +25,15 @@
 )
 from .common.errors import InsufficientConfiguration
 from .common import Metadata
 import requests
 from io import BytesIO
 import errno
 
-from boto.s3.connection import S3Connection
-from boto.s3.key import Key
-from boto.s3.connection import NoHostProvided
+import boto3
 import math
 from logging import getLogger
 log = getLogger('datalake-archive')
 
 # The name in s3 of the datalake metadata document
 METADATA_NAME = 'datalake'
 
@@ -206,56 +204,59 @@
 
         returns the url to which the file was pushed.
         '''
         self._upload_file(f)
         return self.url_from_file(f)
 
     def _upload_file(self, f):
-        key = self._s3_key_from_metadata(f)
+
+        # Implementation inspired by https://stackoverflow.com/a/60892027
+        obj = self._s3_object_from_metadata(f)
+
+        # NB: we have an opportunitiy to turn on threading here, which may
+        # improve performance. However, in some cases (i.e., queue-based
+        # uploader) we already use threads. So let's add it later as a
+        # configuration if/when we want to experiment.
+        config = boto3.s3.transfer.TransferConfig(
+            # All sizes are bytes
+            multipart_threshold=CHUNK_SIZE(),
+            use_threads=False,
+            multipart_chunksize=CHUNK_SIZE(),
+        )
+
+        extra = {
+            'Metadata': {
+                METADATA_NAME: json.dumps(f.metadata)
+            }
+        }
 
         spos = f.tell()
         f.seek(0, os.SEEK_END)
         f_size = f.tell()
         # seek back to the correct position.
         f.seek(spos)
 
         num_chunks = int(math.ceil(f_size / float(CHUNK_SIZE())))
         log.info("Uploading {} ({} B / {} chunks)".format(
-            key.name, f_size, num_chunks))
-        if num_chunks <= 1:
-            key.set_metadata(METADATA_NAME, json.dumps(f.metadata))
-            completed_size = key.set_contents_from_file(f)
-            log.info("Upload of {} complete (1 part / {} B).".format(
-                key.name, completed_size))
-            return
-        completed_size = 0
+            obj.key, f_size, num_chunks))
+
         chunk = 0
-        mp = key.bucket.initiate_multipart_upload(
-            key.name, metadata={
-                METADATA_NAME: json.dumps(f.metadata)
-            })
-        try:
-            for chunk in range(1, num_chunks + 1):
-                part = mp.upload_part_from_file(
-                    f, chunk, size=CHUNK_SIZE())
-                completed_size += part.size
-                log.debug("Uploaded chunk {}/{} ({}B)".format(
-                    chunk, num_chunks, part.size))
-        except:  # NOQA
-            # Any exception we want to attempt to cancel_upload, otherwise
-            # AWS will bill us every month indefnitely for storing the
-            # partial-uploaded chunks.
-            log.exception("Upload of {} failed on chunk {}".format(
-                key.name, chunk))
-            mp.cancel_upload()
-            raise
-        else:
-            completed = mp.complete_upload()
-            log.info("Upload of {} complete ({} parts / {} B).".format(
-                completed.key_name, chunk, completed_size))
+
+        def _progress(number_of_bytes):
+            nonlocal chunk
+            log.info("Uploaded chunk {}/{} ({}B)".format(
+                chunk, num_chunks, CHUNK_SIZE()))
+            chunk += 1
+
+        # NB: deep under the hood, upload_fileobj creates a
+        # CreateMultipartUploadTask. And that object cleans up after itself:
+        # https://github.com/boto/s3transfer/blob/develop/s3transfer/tasks.py#L353-L360  # noqa
+        obj.upload_fileobj(f, ExtraArgs=extra, Config=config,
+                           Callback=_progress)
+        obj.wait_until_exists()
 
     def url_from_file(self, f):
         return self._get_s3_url(f)
 
     _URL_FORMAT = 's3://{bucket}/{key}'
 
     def fetch(self, url, stream=False):
@@ -275,20 +276,19 @@
             msg = msg.format(url)
             raise InvalidDatalakePath(msg)
 
     def _is_valid_http_url(self, url):
         return url.startswith('http') and url.endswith('/data')
 
     def _fetch_s3_url(self, url, stream=False):
-        k = self._get_key_from_url(url)
-        m = self._get_metadata_from_key(k)
+        obj, m = self._get_object_from_url(url)
         if stream:
-            return StreamingFile(k, **m)
+            return StreamingFile(obj._datalake_details['Body'], **m)
         fd = BytesIO()
-        k.get_contents_to_file(fd)
+        self._s3_bucket.download_fileobj(obj.key, fd)
         fd.seek(0)
         return File(fd, **m)
 
     def _fetch_http_url(self, url, stream=False):
         m = self._get_metadata_from_http_url(url)
         k = self._stream_http_url(url)
         if stream:
@@ -327,16 +327,15 @@
         files are stored in the current directory and the filenames are the ids
         from the metadata.
 
         Returns the filename written.
         '''
         k = None
         if url.startswith('s3://'):
-            k = self._get_key_from_url(url)
-            m = self._get_metadata_from_key(k)
+            obj, m = self._get_object_from_url(url)
         else:
             m = self._get_metadata_from_http_url(url)
         fname = self._get_filename_from_template(filename_template, m)
         dname = os.path.dirname(fname)
         self._mkdirs(dname)
         if k:
             k.get_contents_to_filename(fname)
@@ -353,26 +352,27 @@
             os.makedirs(path)
         except OSError as e:
             if e.errno == errno.EEXIST and os.path.isdir(path):
                 pass
             else:
                 raise
 
-    def _get_key_from_url(self, url):
+    def _get_object_from_url(self, url):
         self._validate_fetch_url(url)
         key_name = self._get_key_name_from_url(url)
-        k = self._s3_bucket.get_key(key_name)
-        if k is None:
+        obj = self._s3.Object(self._s3_bucket_name, key_name)
+        try:
+            # cache the results of the get on the obj to avoid superfluous
+            # network calls.
+            obj._datalake_details = obj.get()
+            m = obj._datalake_details['Metadata'].get(METADATA_NAME)
+        except self._s3.meta.client.exceptions.NoSuchKey:
             msg = 'Failed to find {} in the datalake.'.format(url)
             raise InvalidDatalakePath(msg)
-        return k
-
-    def _get_metadata_from_key(self, key):
-        m = key.get_metadata(METADATA_NAME)
-        return Metadata.from_json(m)
+        return obj, Metadata.from_json(m)
 
     def _get_filename_from_template(self, template, metadata):
         if template is None:
             template = '{id}'
         try:
             return template.format(**metadata)
         except KeyError as e:
@@ -384,69 +384,70 @@
 
     def _get_key_name_from_url(self, url):
         parts = urlparse(url)
         if not parts.path:
             msg = '{} is not a valid datalake url'.format(url)
             raise InvalidDatalakePath(msg)
 
-        return parts.path
+        # NB: under boto 2 we didn't used to have to have the lstrip. It seems
+        # that boto2 explicitly stripped these leading slashes for us:
+        # https://groups.google.com/g/boto-users/c/mv--NMPUXoU ...but boto3
+        # does not. So we must take care to strip it whenever we parse a URL to
+        # get a key.
+        return parts.path.lstrip('/')
 
     def _validate_fetch_url(self, url):
         valid_base_urls = (self.storage_url, self.http_url)
         if not [u for u in valid_base_urls if url.startswith(u)]:
             msg = 'url {} does not start with the configured storage urls {}.'
             msg = msg.format(url, valid_base_urls)
             raise InvalidDatalakePath(msg)
 
     def _get_s3_url(self, f):
-        key = self._s3_key_from_metadata(f)
+        obj = self._s3_object_from_metadata(f)
         return self._URL_FORMAT.format(bucket=self._s3_bucket_name,
-                                       key=key.name)
+                                       key=obj.key)
 
     @property
     def _s3_bucket_name(self):
         return self._parsed_storage_url.netloc
 
     @memoized_property
     def _s3_bucket(self):
-        # Note: we pass validate=False because we may just have push
-        # permissions. If validate is not False, boto tries to list the
-        # bucket. And this will 403.
-        return self._s3_conn.get_bucket(self._s3_bucket_name, validate=False)
+        return self._s3.Bucket(self._s3_bucket_name)
 
     _KEY_FORMAT = '{id}/data'
 
-    def _s3_key_from_metadata(self, f):
-        # For performance reasons, s3 keys should start with a short random
-        # sequence:
-        # https://aws.amazon.com/blogs/aws/amazon-s3-performance-tips-tricks-seattle-hiring-event/
-        # http://docs.aws.amazon.com/AmazonS3/latest/dev/request-rate-perf-considerations.html
+    def _s3_object_from_metadata(self, f):
         key_name = self._KEY_FORMAT.format(**f.metadata)
-        return Key(self._s3_bucket, name=key_name)
+        return self._s3_bucket.Object(key_name)
 
     @property
     def _s3_host(self):
         h = environ.get('AWS_S3_HOST')
         if h is not None:
-            return h
+            return 'https://' + h
         r = environ.get('AWS_REGION') or environ.get('AWS_DEFAULT_REGION')
         if r is not None:
-            return 's3-' + r + '.amazonaws.com'
+            return 'https://s3-' + r + '.amazonaws.com'
         else:
-            return NoHostProvided
+            return None
 
-    @property
-    def _s3_conn(self):
-        if not hasattr(self, '_conn'):
-            k = environ.get('AWS_ACCESS_KEY_ID')
-            s = environ.get('AWS_SECRET_ACCESS_KEY')
-            self._conn = S3Connection(aws_access_key_id=k,
-                                      aws_secret_access_key=s,
-                                      host=self._s3_host)
-        return self._conn
+    @memoized_property
+    def _s3(self):
+        # boto3 uses AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY
+        # boto3 will use AWS_DEFAULT_REGION if AWS_REGION is not set
+        return boto3.resource('s3',
+                              region_name=environ.get('AWS_REGION'),
+                              endpoint_url=self._s3_host)
+
+    @memoized_property
+    def _s3_client(self):
+        boto_session = boto3.Session()
+        return boto_session.client('s3')
 
     def _requests_get(self, url, **kwargs):
         return self._session.get(url, timeout=TIMEOUT(), **kwargs)
 
     @property
     def _session(self):
         if self.__session:
```

### Comparing `datalake-1.1/datalake/common/__init__.py` & `datalake-2.0/datalake/common/__init__.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/common/conf.py` & `datalake-2.0/datalake/common/conf.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/common/errors.py` & `datalake-2.0/datalake/common/errors.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/common/metadata.py` & `datalake-2.0/datalake/common/metadata.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/common/record.py` & `datalake-2.0/datalake/common/record.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
-from . import Metadata, InvalidDatalakeMetadata
+from . import Metadata
 from six.moves.urllib.parse import urlparse
 import json
 import os
 
 
 from .errors import InsufficientConfiguration, UnsupportedTimeRange, \
     NoSuchDatalakeFile
@@ -24,30 +24,34 @@
 '''whether or not s3 features are available
 
 Users may wish to check if s3 features are available before invoking them. If
 they are unavailable, the affected functions will raise
 InsufficientConfiguration.'''
 has_s3 = True
 try:
-    import boto.s3
-    from boto.exception import S3ResponseError
+    import boto3
 except ImportError:
     has_s3 = False
 
 
 def requires_s3(f):
     def wrapped(*args, **kwargs):
         if not has_s3:
             msg = 'This feature requires s3 features.  '
             msg += '`pip install datalake-common[s3]` to turn this feature on.'
             raise InsufficientConfiguration(msg)
         return f(*args, **kwargs)
     return wrapped
 
 
+# NB: Some time ago we migrated this class from datalake-common to datalake in
+# order to reduce the number of packages that comprise the datalake. As a side
+# effect of this migration this class contains some code duplicated with the
+# datalake.Archive. There is an opportunity to clean this up, but we can take
+# that on after getting off of boto 2.
 class DatalakeRecord(dict):
 
     def __init__(self, url, metadata, time_bucket, create_time, size):
         self.metadata = metadata
         parts = {
             'version': 0,
             'url': url,
@@ -60,90 +64,93 @@
         }
         super(DatalakeRecord, self).__init__(parts)
 
     @classmethod
     @requires_s3
     def list_from_url(cls, url):
         '''return a list of DatalakeRecords for the specified url'''
-        key = cls._get_key(url)
-        metadata = cls._get_metadata_from_key(key)
-        ct = cls._get_create_time(key)
+        obj, metadata = cls._get_object(url)
+        ct = cls._get_create_time(obj)
         time_buckets = cls.get_time_buckets_from_metadata(metadata)
-        return [cls(url, metadata, t, ct, key.size) for t in time_buckets]
+
+        return [
+            cls(url, metadata, t, ct, obj.content_length) for t in time_buckets
+        ]
 
     @classmethod
     @requires_s3
     def list_from_metadata(cls, url, metadata):
         '''return a list of DatalakeRecords for the url and metadata'''
-        key = cls._get_key(url)
+        obj, _ = cls._get_object(url)
         metadata = Metadata(**metadata)
-        ct = cls._get_create_time(key)
+        ct = cls._get_create_time(obj)
         time_buckets = cls.get_time_buckets_from_metadata(metadata)
-        return [cls(url, metadata, t, ct, key.size) for t in time_buckets]
+        return [
+            cls(url, metadata, t, ct, obj.content_length) for t in time_buckets
+        ]
 
     @classmethod
-    def _get_create_time(cls, key):
-        return Metadata.normalize_date(key.last_modified)
+    def _get_create_time(cls, obj):
+        return Metadata.normalize_date(obj.last_modified)
 
     @classmethod
-    def _get_key(cls, url):
+    def _get_object(cls, url):
         parsed_url = urlparse(url)
-        bucket = cls._get_bucket(parsed_url.netloc)
-        key = bucket.get_key(parsed_url.path)
-        if key is None:
+        bucket = parsed_url.netloc
+
+        # NB: under boto 2 we didn't used to have to have the lstrip. It seems
+        # that boto2 explicitly stripped these leading slashes for us:
+        # https://groups.google.com/g/boto-users/c/mv--NMPUXoU ...but boto3
+        # does not. So we must take care to strip it whenever we parse a URL to
+        # get a key.
+        key_name = parsed_url.path.lstrip('/')
+        obj = cls._connection().Object(parsed_url.netloc, key_name)
+
+        try:
+            # cache the results of the get on the obj to avoid superfluous
+            # network calls.
+            obj._datalake_details = obj.get()
+            m = obj._datalake_details['Metadata'].get('datalake')
+        except cls._connection().meta.client.exceptions.NoSuchKey:
             msg = '{} does not appear to be in the datalake'
             msg = msg.format(url)
             raise NoSuchDatalakeFile(msg)
-        return key
-
-    @classmethod
-    def _get_metadata_from_key(cls, key):
-        metadata = key.get_metadata('datalake')
-        if not metadata:
-            msg = 'No datalake metadata for s3://{}{}'
-            msg = msg.format(key.bucket.name, key.name)
-            raise InvalidDatalakeMetadata(msg)
-        return Metadata.from_json(metadata)
-
-    _BUCKETS = {}
-
-    @classmethod
-    def _get_bucket(cls, bucket_name):
-        if bucket_name not in cls._BUCKETS:
-            bucket = cls._get_bucket_from_s3(bucket_name)
-            DatalakeRecord._BUCKETS[bucket_name] = bucket
-        return cls._BUCKETS[bucket_name]
+        except cls._connection().meta.client.exceptions.NoSuchBucket:
+            msg = 'Cannot find datalake file (s3 bucket {} does not exist)'
+            msg = msg.format(bucket)
+            raise NoSuchDatalakeFile(msg)
 
-    @classmethod
-    def _get_bucket_from_s3(cls, bucket_name):
-        try:
-            return cls._connection().get_bucket(bucket_name)
-        except S3ResponseError as e:
-            if e.error_code == 'NoSuchBucket':
-                msg = 'Cannot find datalake file (s3 bucket {} does not exist)'
-                msg = msg.format(bucket_name)
-                raise NoSuchDatalakeFile(msg)
-            else:
-                raise
+        return obj, Metadata.from_json(m)
 
     _CONNECTION = None
 
     @classmethod
     def _connection(cls):
         if cls._CONNECTION is None:
             cls._CONNECTION = cls._prepare_connection()
         return cls._CONNECTION
 
     @classmethod
+    def _s3_host(cls):
+        h = os.environ.get('AWS_S3_HOST')
+        if h is not None:
+            return 'https://' + h
+        r = (os.environ.get('AWS_REGION') or
+             os.environ.get('AWS_DEFAULT_REGION'))
+        if r is not None:
+            return 'https://s3-' + r + '.amazonaws.com'
+        else:
+            return None
+
+    @classmethod
     def _prepare_connection(cls):
-        kwargs = {}
-        s3_host = os.environ.get('AWS_S3_HOST')
-        if s3_host:
-            kwargs['host'] = s3_host
-        return boto.connect_s3(**kwargs)
+
+        return boto3.resource('s3',
+                              region_name=os.environ.get('AWS_REGION'),
+                              endpoint_url=cls._s3_host())
 
     _ONE_DAY_IN_MS = 24*60*60*1000
 
     '''The size of a time bucket in milliseconds
 
     Each datalake record appears once in each time bucket that it covers. For
     example, suppose the time buckets are one day long. If a record has a start
```

### Comparing `datalake-1.1/datalake/config_helpers.py` & `datalake-2.0/datalake/config_helpers.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/crtime.py` & `datalake-2.0/datalake/crtime.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/dlfile.py` & `datalake-2.0/datalake/dlfile.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/logging_helpers.py` & `datalake-2.0/datalake/logging_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''helper facilities for logging
 
 The datalake client does not generally configure its own logging. But the
 command line client may choose to configure logging in some cases. Users with
 sentry accounts may wish to configure it by installing the sentry extras.
 '''
 import os
-import logging
+import logging.config
 from .common.errors import InsufficientConfiguration
 
 
 def sentry_available():
     try:
         import raven.handlers.logging
         return hasattr(raven.handlers.logging, 'SentryHandler')
```

### Comparing `datalake-1.1/datalake/queue.py` & `datalake-2.0/datalake/queue.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/scripts/cli.py` & `datalake-2.0/datalake/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/tests/__init__.py` & `datalake-2.0/datalake/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/tests/conftest.py` & `datalake-2.0/datalake/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 import random
 import string
 import os
 import six
 
 
 try:
-    from moto import mock_s3_deprecated
-    import boto.s3
-    from boto.s3.key import Key
+    from moto import mock_s3
+    import boto3
     from six.moves.urllib.parse import urlparse
     import json
 except ImportError:
     # if developers use s3-test features without having installed s3 stuff,
     # things will fail. So it goes.
     pass
 
@@ -110,14 +109,26 @@
         f.write(content)
         return str(f)
 
     return get_tmpfile
 
 
 @pytest.fixture
+def tmpfile_maker(tmpdir):
+
+    def get_tmpfile(content):
+        name = random_word(10)
+        f = tmpdir.join(name)
+        f.write(content)
+        return str(f)
+
+    return get_tmpfile
+
+
+@pytest.fixture
 def aws_connector(request):
 
     def create_connection(mocker, connector):
         mock = mocker()
         mock.start()
 
         def tear_down():
@@ -127,42 +138,45 @@
         return connector()
 
     return create_connection
 
 
 @pytest.fixture
 def s3_connection(aws_connector):
-    return aws_connector(mock_s3_deprecated, boto.connect_s3)
+    with mock_s3():
+        yield boto3.resource('s3')
 
 
 @pytest.fixture
 def s3_bucket_maker(s3_connection):
 
     def maker(bucket_name):
-        return s3_connection.create_bucket(bucket_name)
+        b = s3_connection.Bucket(bucket_name)
+        b.create()
+        return b
 
     return maker
 
 
 @pytest.fixture
 def s3_file_maker(s3_bucket_maker):
 
     def maker(bucket, key, content, metadata):
         b = s3_bucket_maker(bucket)
-        k = Key(b)
-        k.key = key
-        if metadata:
-            k.set_metadata('datalake', json.dumps(metadata))
-        k.set_contents_from_string(content)
+        b.Object(key).put(
+            Body=content,
+            Metadata={'datalake': json.dumps(metadata)} if metadata else {}
+        )
 
     return maker
 
 
 @pytest.fixture
 def s3_file_from_metadata(s3_file_maker):
 
     def maker(url, metadata):
         url = urlparse(url)
         assert url.scheme == 's3'
-        s3_file_maker(url.netloc, url.path, '', metadata)
+        # NB: clean up leading slash.
+        s3_file_maker(url.netloc, url.path.lstrip('/'), '', metadata)
 
     return maker
```

### Comparing `datalake-1.1/datalake/tests/test_conf.py` & `datalake-2.0/datalake/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/tests/test_metadata.py` & `datalake-2.0/datalake/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/tests/test_record.py` & `datalake-2.0/datalake/tests/test_record.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake/translator.py` & `datalake-2.0/datalake/translator.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/datalake.egg-info/PKG-INFO` & `datalake-2.0/datalake.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalake
-Version: 1.1
+Version: 2.0
 Summary: datalake: a metadata-aware archive
 Home-page: https://github.com/planetlabs/datalake
 Author: Brian Cavagnolo
 Author-email: brian@planet.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `datalake-1.1/datalake.egg-info/SOURCES.txt` & `datalake-2.0/datalake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalake-1.1/setup.py` & `datalake-2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,28 +17,28 @@
       version=get_version(),
       cmdclass=versioneer.get_cmdclass(),
       description='datalake: a metadata-aware archive',
       author='Brian Cavagnolo',
       author_email='brian@planet.com',
       packages=find_packages(exclude=['test']),
       install_requires=[
-          'boto>=2.38.0',
+          'boto3>=1.9.68',
           'memoized_property>=1.0.1',
           'pyblake2>=0.9.3; python_version<"3.6"',
           'click>=4.1',
           'python-dotenv>=0.1.3',
           'requests>=2.5',
           'six>=1.10.0',
           'python-dateutil>=2.4.2',
           'pytz>=2015.4',
       ],
       extras_require={
           'test': [
               'pytest<8.0.0',
-              'moto<3.0.0',
+              'moto[s3]>4,<5',
               'twine<4.0.0',
               'pip>=20.0.0,<22.0.0',
               'wheel<0.38.0',
               'flake8>=2.5.0,<4.1',
               'responses<0.22.0',
           ],
           # the queuable feature allows users to offload their datalake pushes
```

### Comparing `datalake-1.1/test/test_archive.py` & `datalake-2.0/test/test_archive.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,36 +12,40 @@
 # License for the specific language governing permissions and limitations under
 # the License.
 
 import json
 import re
 
 
-def test_push_file(archive, random_metadata, tmpfile, s3_key):
+def _get_contents_as_string(obj):
+    return obj.get()['Body'].read()
+
+
+def test_push_file(archive, random_metadata, tmpfile, s3_object):
     expected_content = 'mwahaha'.encode('utf-8')
     f = tmpfile(expected_content)
     url = archive.prepare_metadata_and_push(f, **random_metadata)
-    from_s3 = s3_key(url)
-    assert from_s3.get_contents_as_string() == expected_content
-    metadata = from_s3.get_metadata('datalake')
+    from_s3 = s3_object(url)
+    assert _get_contents_as_string(from_s3) == expected_content
+    metadata = from_s3.get()['Metadata'].get('datalake')
     assert metadata is not None
     metadata = json.loads(metadata)
     common_keys = set(metadata.keys()).intersection(random_metadata.keys())
     assert common_keys == set(random_metadata.keys())
 
 
 def test_push_large_file(
-        monkeypatch, archive, random_metadata, tmpfile, s3_key):
-    monkeypatch.setenv('DATALAKE_CHUNK_SIZE_MB', 5)
+        monkeypatch, archive, random_metadata, tmpfile, s3_object):
+    monkeypatch.setenv('DATALAKE_CHUNK_SIZE_MB', '5')
     expected_content = ('big data' * 1024 * 1024).encode('utf-8')
     f = tmpfile(expected_content)
     url = archive.prepare_metadata_and_push(f, **random_metadata)
-    from_s3 = s3_key(url)
-    assert from_s3.get_contents_as_string() == expected_content
-    metadata = from_s3.get_metadata('datalake')
+    from_s3 = s3_object(url)
+    assert _get_contents_as_string(from_s3) == expected_content
+    metadata = from_s3.get()['Metadata'].get('datalake')
     assert metadata is not None
     metadata = json.loads(metadata)
     common_keys = set(metadata.keys()).intersection(random_metadata.keys())
     assert common_keys == set(random_metadata.keys())
     for k in common_keys:
         assert metadata[k] == random_metadata[k]
```

### Comparing `datalake-1.1/test/test_cli.py` & `datalake-2.0/test/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
 import pytest
 from test_crtime import crtime_setuid
-from click.testing import CliRunner
 import random
 
+
 def test_cli_without_command_fails(cli_tester):
     cli_tester('', expected_exit=2)
 
 
 def test_cli_with_version_succeeds(cli_tester):
     cli_tester('--version')
 
@@ -58,25 +58,26 @@
 def test_translate_with_good_args_succceeds(cli_tester):
     cmd = ("translate .*job-(?P<job_id>[0-9]+).log$~job{job_id} "
            "/var/log/job-456.log")
     print(cmd)
     cli_tester(cmd)
 
 
-@pytest.mark.parametrize("content", [['text'], ['multiple', 'things']])  
-def test_cat(cli_tester, datalake_url_maker, random_metadata, content):
+@pytest.mark.parametrize("content", [['text'], ['multiple', 'things']])
+def test_cat(cli_tester, datalake_url_maker, random_metadata, content,
+             s3_connection):
     metadata1 = random_metadata
     metadata2 = random_metadata.copy()
     metadata2['id'] = ('%0' + str(40) + 'x') % random.randrange(16**40)
     url = ""+datalake_url_maker(metadata=metadata1, content=content[0])
     if content[0] == 'multiple':
-        for i in range (1, len(content)):
-            url = url + " " + datalake_url_maker(metadata=metadata2, content=content[i])
-    cmd = ("cat "+url)
-    print(cmd)
+        for i in range(1, len(content)):
+            url = (url + " " +
+                   datalake_url_maker(metadata=metadata2, content=content[i]))
+    cmd = "cat " + url
     output = cli_tester(cmd)
     output = output.split('\n')
     for i in range(len(content)):
         assert output[i] == content[i]
 
 
 @pytest.mark.skipif(not crtime_setuid, reason='crtime required')
```

### Comparing `datalake-1.1/test/test_config.py` & `datalake-2.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/test/test_crtime.py` & `datalake-2.0/test/test_crtime.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/test/test_fetch.py` & `datalake-2.0/test/test_fetch.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/test/test_file.py` & `datalake-2.0/test/test_file.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/test/test_latest.py` & `datalake-2.0/test/test_latest.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/test/test_list.py` & `datalake-2.0/test/test_list.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/test/test_logging.py` & `datalake-2.0/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/test/test_queue.py` & `datalake-2.0/test/test_queue.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # License for the specific language governing permissions and limitations under
 # the License.
 
 import pytest
 import json
 from threading import Timer
 import os
-from datalake.tests import random_word
+from datalake.tests import random_word, generate_random_metadata
 from datalake.common.errors import InsufficientConfiguration
 from datalake import Enqueuer, Uploader, InvalidDatalakeBundle
 from datalake.queue import has_queue
 from conftest import crtime_setuid
 from gzip import GzipFile
 import zlib
 
@@ -49,26 +49,31 @@
     def cb(*args, **kwargs):
         raise Exception('Boo!')
 
     return Uploader(archive, queue_dir, callback=cb)
 
 
 @pytest.fixture
-def uploaded_content_validator(s3_key):
+def uploaded_content_validator(s3_object):
 
     def validator(expected_content, expected_metadata=None, compressed=False):
 
-        from_s3 = s3_key()
+        if expected_metadata:
+            from_s3 = s3_object(
+                f's3://datalake-test/{expected_metadata["id"]}/data'
+            )
+        else:
+            from_s3 = s3_object()
         assert from_s3 is not None
-        content = from_s3.get_contents_as_string()
+        content = from_s3.get()['Body'].read()
         if compressed:
             content = zlib.decompress(content, 16 + zlib.MAX_WBITS)
         assert content == expected_content
         if expected_metadata is not None:
-            metadata = json.loads(from_s3.get_metadata('datalake'))
+            metadata = json.loads(from_s3.get()['Metadata'].get('datalake'))
             assert metadata == expected_metadata
 
     return validator
 
 
 @pytest.fixture
 def uploaded_file_validator(archive, uploaded_content_validator):
@@ -80,25 +85,35 @@
     return validator
 
 
 @pytest.fixture
 def assert_s3_bucket_empty(s3_bucket):
 
     def asserter():
-        assert len([k for k in s3_bucket.list()]) == 0
+        assert len(list(s3_bucket.objects.all())) == 0
 
     return asserter
 
 
 @pytest.fixture
 def random_file(tmpfile, random_metadata):
     expected_content = random_word(100)
     return tmpfile(expected_content)
 
 
+@pytest.fixture
+def random_file_maker(tmpfile_maker):
+
+    def maker():
+        expected_content = random_word(100)
+        return tmpfile_maker(expected_content)
+
+    return maker
+
+
 @pytest.mark.skipif(not has_queue, reason='requires queuable features')
 def test_upload_existing(enqueuer, uploader, random_file, random_metadata,
                          uploaded_file_validator):
     f = enqueuer.enqueue(random_file, **random_metadata)
     uploader.listen(timeout=0.1)
     uploaded_file_validator(f)
 
@@ -216,33 +231,33 @@
     uploader.listen(timeout=0.1)
 
     expected_content = open(random_file, 'rb').read()
     uploaded_content_validator(expected_content, compressed=True)
 
 
 @pytest.mark.skipif(not has_queue, reason='requires queuable features')
-def test_threaded_upload(enqueuer, uploader, random_file, random_metadata,
+def test_threaded_upload(enqueuer, uploader, random_file_maker,
                          uploaded_file_validator):
 
     # This test does not actually validate that multiple threads are running.
     # But it does validate that when the number of workers is greater than 3,
     # multiple files get uploaded.
     enqueued_files = []
 
     def enqueue():
-        f = enqueuer.enqueue(random_file, **random_metadata)
+        m = generate_random_metadata()
+        f = enqueuer.enqueue(random_file_maker(), **m)
         enqueued_files.append(f)
         if len(enqueued_files) < 3:
             t = Timer(0.1, enqueue)
             t.start()
 
     t = Timer(0.5, enqueue)
     t.start()
     uploader.listen(timeout=1.0, workers=3)
-
     assert len(enqueued_files) == 3
     for f in enqueued_files:
         uploaded_file_validator(f)
 
 
 @pytest.mark.skipif(not has_queue, reason='requires queuable features')
 def test_threaded_uploader_exits(enqueuer, faulty_uploader, random_file,
```

### Comparing `datalake-1.1/test/test_translator.py` & `datalake-2.0/test/test_translator.py`

 * *Files identical despite different names*

### Comparing `datalake-1.1/versioneer.py` & `datalake-2.0/versioneer.py`

 * *Files identical despite different names*

