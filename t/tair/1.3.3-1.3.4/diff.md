# Comparing `tmp/tair-1.3.3.tar.gz` & `tmp/tair-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tair-1.3.3.tar", last modified: Mon Apr 10 06:00:31 2023, max compression
+gzip compressed data, was "tair-1.3.4.tar", last modified: Tue May 30 11:01:38 2023, max compression
```

## Comparing `tair-1.3.3.tar` & `tair-1.3.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-04-10 06:00:31.554691 tair-1.3.3/
--rw-r--r--   0 yangbodong   (502) staff       (20)     1064 2022-07-27 06:08:53.000000 tair-1.3.3/LICENSE
--rw-r--r--   0 yangbodong   (502) staff       (20)     4612 2023-04-10 06:00:31.554505 tair-1.3.3/PKG-INFO
--rw-r--r--   0 yangbodong   (502) staff       (20)     4331 2023-01-05 08:19:35.000000 tair-1.3.3/README.md
--rw-r--r--   0 yangbodong   (502) staff       (20)       38 2023-04-10 06:00:31.554752 tair-1.3.3/setup.cfg
--rwxr-xr-x   0 yangbodong   (502) staff       (20)      488 2023-04-10 05:59:28.000000 tair-1.3.3/setup.py
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-04-10 06:00:31.547172 tair-1.3.3/tair/
--rw-r--r--   0 yangbodong   (502) staff       (20)     1557 2023-02-17 07:55:24.000000 tair-1.3.3/tair/__init__.py
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-04-10 06:00:31.549170 tair-1.3.3/tair/asyncio/
--rw-r--r--   0 yangbodong   (502) staff       (20)     1412 2022-08-16 03:42:18.000000 tair-1.3.3/tair/asyncio/__init__.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     3293 2023-01-05 06:47:04.000000 tair-1.3.3/tair/asyncio/client.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1639 2023-01-05 07:08:21.000000 tair-1.3.3/tair/asyncio/cluster.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1005 2023-01-05 06:47:04.000000 tair-1.3.3/tair/asyncio/pipeline.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     3308 2022-08-16 03:42:18.000000 tair-1.3.3/tair/client.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1866 2022-08-16 03:42:18.000000 tair-1.3.3/tair/cluster.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     5361 2023-02-17 07:55:24.000000 tair-1.3.3/tair/commands.py
--rw-r--r--   0 yangbodong   (502) staff       (20)      334 2022-07-27 06:08:53.000000 tair-1.3.3/tair/exceptions.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1184 2022-08-16 03:42:18.000000 tair-1.3.3/tair/pipeline.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1582 2022-08-16 03:42:18.000000 tair-1.3.3/tair/tairbloom.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    11976 2022-09-01 08:46:46.000000 tair-1.3.3/tair/taircpc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     3156 2022-08-25 09:35:31.000000 tair-1.3.3/tair/tairdoc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     5190 2022-08-25 09:35:31.000000 tair-1.3.3/tair/tairgis.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    14354 2022-08-25 09:35:31.000000 tair-1.3.3/tair/tairhash.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     4944 2022-08-16 03:42:18.000000 tair-1.3.3/tair/tairroaring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     6759 2023-04-10 02:26:45.000000 tair-1.3.3/tair/tairsearch.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     9196 2023-01-05 06:47:04.000000 tair-1.3.3/tair/tairstring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    13708 2022-09-01 08:46:46.000000 tair-1.3.3/tair/tairts.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    14047 2023-02-17 07:55:24.000000 tair-1.3.3/tair/tairvector.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     7377 2022-08-16 03:42:18.000000 tair-1.3.3/tair/tairzset.py
--rw-r--r--   0 yangbodong   (502) staff       (20)      259 2022-08-16 03:42:18.000000 tair-1.3.3/tair/typing.py
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-04-10 06:00:31.548043 tair-1.3.3/tair.egg-info/
--rw-r--r--   0 yangbodong   (502) staff       (20)     4612 2023-04-10 06:00:31.000000 tair-1.3.3/tair.egg-info/PKG-INFO
--rw-r--r--   0 yangbodong   (502) staff       (20)      874 2023-04-10 06:00:31.000000 tair-1.3.3/tair.egg-info/SOURCES.txt
--rw-r--r--   0 yangbodong   (502) staff       (20)        1 2023-04-10 06:00:31.000000 tair-1.3.3/tair.egg-info/dependency_links.txt
--rw-r--r--   0 yangbodong   (502) staff       (20)       13 2023-04-10 06:00:31.000000 tair-1.3.3/tair.egg-info/requires.txt
--rw-r--r--   0 yangbodong   (502) staff       (20)        5 2023-04-10 06:00:31.000000 tair-1.3.3/tair.egg-info/top_level.txt
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-04-10 06:00:31.554112 tair-1.3.3/tests/
--rw-r--r--   0 yangbodong   (502) staff       (20)     2256 2023-01-05 07:58:42.000000 tair-1.3.3/tests/test_from_url.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     2223 2023-01-05 06:47:04.000000 tair-1.3.3/tests/test_pipeline.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     2484 2022-08-16 03:42:18.000000 tair-1.3.3/tests/test_tairbloom.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    24057 2022-09-01 08:46:46.000000 tair-1.3.3/tests/test_taircpc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     4708 2022-08-25 09:35:31.000000 tair-1.3.3/tests/test_tairdoc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     8533 2022-08-25 09:35:31.000000 tair-1.3.3/tests/test_tairgis.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    41035 2022-08-16 03:42:18.000000 tair-1.3.3/tests/test_tairhash.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     9432 2022-08-16 03:42:18.000000 tair-1.3.3/tests/test_tairroaring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    18793 2023-04-10 02:26:45.000000 tair-1.3.3/tests/test_tairsearch.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    19152 2022-08-16 03:42:18.000000 tair-1.3.3/tests/test_tairstring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    13908 2022-09-01 08:46:46.000000 tair-1.3.3/tests/test_tairts.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    16086 2023-02-17 07:55:24.000000 tair-1.3.3/tests/test_tairvector.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    23955 2022-08-16 03:42:18.000000 tair-1.3.3/tests/test_tairzset.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-05-30 11:01:38.163755 tair-1.3.4/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1064 2022-07-27 06:08:53.000000 tair-1.3.4/LICENSE
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4659 2023-05-30 11:01:38.163536 tair-1.3.4/PKG-INFO
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4378 2023-05-06 06:15:53.000000 tair-1.3.4/README.md
+-rw-r--r--   0 yangbodong   (502) staff       (20)       38 2023-05-30 11:01:38.163815 tair-1.3.4/setup.cfg
+-rwxr-xr-x   0 yangbodong   (502) staff       (20)      488 2023-05-30 11:00:40.000000 tair-1.3.4/setup.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-05-30 11:01:38.135491 tair-1.3.4/tair/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1557 2023-02-17 07:55:24.000000 tair-1.3.4/tair/__init__.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-05-30 11:01:38.156460 tair-1.3.4/tair/asyncio/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1412 2022-08-16 03:42:18.000000 tair-1.3.4/tair/asyncio/__init__.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     3293 2023-01-05 06:47:04.000000 tair-1.3.4/tair/asyncio/client.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1639 2023-01-05 07:08:21.000000 tair-1.3.4/tair/asyncio/cluster.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1005 2023-01-05 06:47:04.000000 tair-1.3.4/tair/asyncio/pipeline.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     3308 2022-08-16 03:42:18.000000 tair-1.3.4/tair/client.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1866 2022-08-16 03:42:18.000000 tair-1.3.4/tair/cluster.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     5361 2023-02-17 07:55:24.000000 tair-1.3.4/tair/commands.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)      334 2022-07-27 06:08:53.000000 tair-1.3.4/tair/exceptions.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1184 2022-08-16 03:42:18.000000 tair-1.3.4/tair/pipeline.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1582 2022-08-16 03:42:18.000000 tair-1.3.4/tair/tairbloom.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    11976 2022-09-01 08:46:46.000000 tair-1.3.4/tair/taircpc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     3156 2022-08-25 09:35:31.000000 tair-1.3.4/tair/tairdoc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     5190 2022-08-25 09:35:31.000000 tair-1.3.4/tair/tairgis.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    14354 2022-08-25 09:35:31.000000 tair-1.3.4/tair/tairhash.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4944 2022-08-16 03:42:18.000000 tair-1.3.4/tair/tairroaring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     6759 2023-04-10 02:26:45.000000 tair-1.3.4/tair/tairsearch.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     9196 2023-01-05 06:47:04.000000 tair-1.3.4/tair/tairstring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    13708 2022-09-01 08:46:46.000000 tair-1.3.4/tair/tairts.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    14123 2023-04-28 05:48:28.000000 tair-1.3.4/tair/tairvector.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     7377 2022-08-16 03:42:18.000000 tair-1.3.4/tair/tairzset.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)      259 2022-08-16 03:42:18.000000 tair-1.3.4/tair/typing.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-05-30 11:01:38.154450 tair-1.3.4/tair.egg-info/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4659 2023-05-30 11:01:38.000000 tair-1.3.4/tair.egg-info/PKG-INFO
+-rw-r--r--   0 yangbodong   (502) staff       (20)      874 2023-05-30 11:01:38.000000 tair-1.3.4/tair.egg-info/SOURCES.txt
+-rw-r--r--   0 yangbodong   (502) staff       (20)        1 2023-05-30 11:01:38.000000 tair-1.3.4/tair.egg-info/dependency_links.txt
+-rw-r--r--   0 yangbodong   (502) staff       (20)       13 2023-05-30 11:01:38.000000 tair-1.3.4/tair.egg-info/requires.txt
+-rw-r--r--   0 yangbodong   (502) staff       (20)        5 2023-05-30 11:01:38.000000 tair-1.3.4/tair.egg-info/top_level.txt
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-05-30 11:01:38.163135 tair-1.3.4/tests/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     2256 2023-01-05 07:58:42.000000 tair-1.3.4/tests/test_from_url.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     2223 2023-01-05 06:47:04.000000 tair-1.3.4/tests/test_pipeline.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     2484 2022-08-16 03:42:18.000000 tair-1.3.4/tests/test_tairbloom.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    24057 2022-09-01 08:46:46.000000 tair-1.3.4/tests/test_taircpc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4708 2022-08-25 09:35:31.000000 tair-1.3.4/tests/test_tairdoc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     8533 2022-08-25 09:35:31.000000 tair-1.3.4/tests/test_tairgis.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    41035 2022-08-16 03:42:18.000000 tair-1.3.4/tests/test_tairhash.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     9432 2022-08-16 03:42:18.000000 tair-1.3.4/tests/test_tairroaring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    18793 2023-04-10 02:26:45.000000 tair-1.3.4/tests/test_tairsearch.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    19152 2022-08-16 03:42:18.000000 tair-1.3.4/tests/test_tairstring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    13908 2022-09-01 08:46:46.000000 tair-1.3.4/tests/test_tairts.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    16155 2023-04-28 05:48:28.000000 tair-1.3.4/tests/test_tairvector.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    23955 2022-08-16 03:42:18.000000 tair-1.3.4/tests/test_tairzset.py
```

### Comparing `tair-1.3.3/LICENSE` & `tair-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/PKG-INFO` & `tair-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tair
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python client for Tair
 Home-page: https://github.com/alibaba/tair-py
 Author: Vincil Lau
 Author-email: vincillau@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -25,15 +25,15 @@
 - [TairString](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairstring-commands), is a string that contains a version number. ([Open sourced](https://github.com/alibaba/TairString))
 - [TairHash](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairhash-commands), is a hash that allows you to specify the expiration time and version number of a field. ([Open sourced](https://github.com/alibaba/TairHash))
 - [TairZset](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairzset-commands), allows you to sort data of the double type based on multiple dimensions. ([Open sourced](https://github.com/alibaba/TairZset))
 - [TairBloom](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairbloom-commands), is a Bloom filter that supports dynamic scaling. (Coming soon)
 - [TairRoaring](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairroaring-commands), is a more efficient and balanced type of compressed bitmaps recognized by the industry. (Coming soon)
 - [TairSearch](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairsearch-command), is a full-text search module developed in-house based on Redis modules. (Coming soon)
 - [TairDoc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairdoc-commands), to perform create, read, update, and delete (CRUD) operations on JSON data. (Coming soon)
-- [TairGis](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairgis-commands), allowing you to query points, linestrings, and polygons. (Coming soon)
+- [TairGis](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairgis-commands), allowing you to query points, linestrings, and polygons. ([Open Sourced](https://github.com/tair-opensource/TairGis))
 - [TairTs](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairts-commands), is a time series data structure that is developed on top of Redis modules.  (Coming soon)
 - [TairCpc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/taircpc-commands), is a data structure developed based on the compressed probability counting (CPC) sketch. (Coming soon)
 - [TairVector](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairvector),  is a self-developed data structure that provides high-performance real-time storage and retrieval of vectors. (Coming soon)
 
 ## Install
 
 Install from pip:
```

### Comparing `tair-1.3.3/README.md` & `tair-1.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - [TairString](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairstring-commands), is a string that contains a version number. ([Open sourced](https://github.com/alibaba/TairString))
 - [TairHash](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairhash-commands), is a hash that allows you to specify the expiration time and version number of a field. ([Open sourced](https://github.com/alibaba/TairHash))
 - [TairZset](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairzset-commands), allows you to sort data of the double type based on multiple dimensions. ([Open sourced](https://github.com/alibaba/TairZset))
 - [TairBloom](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairbloom-commands), is a Bloom filter that supports dynamic scaling. (Coming soon)
 - [TairRoaring](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairroaring-commands), is a more efficient and balanced type of compressed bitmaps recognized by the industry. (Coming soon)
 - [TairSearch](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairsearch-command), is a full-text search module developed in-house based on Redis modules. (Coming soon)
 - [TairDoc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairdoc-commands), to perform create, read, update, and delete (CRUD) operations on JSON data. (Coming soon)
-- [TairGis](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairgis-commands), allowing you to query points, linestrings, and polygons. (Coming soon)
+- [TairGis](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairgis-commands), allowing you to query points, linestrings, and polygons. ([Open Sourced](https://github.com/tair-opensource/TairGis))
 - [TairTs](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairts-commands), is a time series data structure that is developed on top of Redis modules.  (Coming soon)
 - [TairCpc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/taircpc-commands), is a data structure developed based on the compressed probability counting (CPC) sketch. (Coming soon)
 - [TairVector](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairvector),  is a self-developed data structure that provides high-performance real-time storage and retrieval of vectors. (Coming soon)
 
 ## Install
 
 Install from pip:
```

### Comparing `tair-1.3.3/tair/__init__.py` & `tair-1.3.4/tair/__init__.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/asyncio/__init__.py` & `tair-1.3.4/tair/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/asyncio/client.py` & `tair-1.3.4/tair/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/asyncio/cluster.py` & `tair-1.3.4/tair/asyncio/cluster.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/asyncio/pipeline.py` & `tair-1.3.4/tair/asyncio/pipeline.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/client.py` & `tair-1.3.4/tair/client.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/cluster.py` & `tair-1.3.4/tair/cluster.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/commands.py` & `tair-1.3.4/tair/commands.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/pipeline.py` & `tair-1.3.4/tair/pipeline.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/tairbloom.py` & `tair-1.3.4/tair/tairbloom.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/taircpc.py` & `tair-1.3.4/tair/taircpc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/tairdoc.py` & `tair-1.3.4/tair/tairdoc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/tairgis.py` & `tair-1.3.4/tair/tairgis.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/tairhash.py` & `tair-1.3.4/tair/tairhash.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/tairroaring.py` & `tair-1.3.4/tair/tairroaring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/tairsearch.py` & `tair-1.3.4/tair/tairsearch.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/tairstring.py` & `tair-1.3.4/tair/tairstring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/tairts.py` & `tair-1.3.4/tair/tairts.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair/tairvector.py` & `tair-1.3.4/tair/tairvector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from functools import partial, reduce
-from typing import Dict, Iterable, List, Sequence, Tuple, Union
+from typing import Dict, List, Sequence, Tuple, Union, Optional
 
 from redis.client import pairs_to_dict
 from redis.utils import str_if_bytes
 
-from tair.typing import ResponseT
 
 VectorType = Sequence[Union[int, float]]
 
 
 class DistanceMetric:
     Euclidean = "L2"  # an alias to L2
     L2 = "L2"
@@ -30,27 +29,29 @@
     Binary = "BINARY"
 
 
 class TextVectorEncoder:
     SEP = bytes(",", "ascii")
     BITS = ("0", "1")
 
-    def encode(vector: Sequence[Union[float, int]], is_binary=False) -> bytes:
+    @classmethod
+    def encode(cls, vector: VectorType, is_binary=False) -> bytes:
         s = ""
         if is_binary:
-            s = "[" + ",".join([TextVectorEncoder.BITS[x] for x in vector]) + "]"
+            s = "[" + ",".join([cls.BITS[x] for x in vector]) + "]"
         else:
             s = "[" + ",".join(["%f" % x for x in vector]) + "]"
         return bytes(s, encoding="ascii")  # ascii is enough
 
-    def decode(buf: bytes) -> Tuple[float]:
+    @classmethod
+    def decode(cls, buf: bytes) -> Tuple[float]:
         if buf[0] != ord("[") or buf[-1] != ord("]"):
             raise ValueError("invalid text vector value")
         is_int = True
-        components = buf[1:-1].split(TextVectorEncoder.SEP)
+        components = buf[1:-1].split(cls.SEP)
         for x in components:
             if not x.isdigit():
                 is_int = False
 
         if is_int:
             return tuple(int(x) for x in components)
         return tuple(float(x) for x in components)
@@ -87,15 +88,15 @@
             self.batch = res[1]
             self.idx = 0
         if self.idx >= len(self.batch):
             # in case the first batch from server is empty
             raise StopIteration
         ret = self.batch[self.idx]
         self.idx += 1
-        return ret.decode("utf-8")
+        return ret
 
     def iter(self):
         """
         create an iterator from the result
         """
         return iter(self)
 
@@ -134,32 +135,40 @@
         """get and update index info"""
         self.params = self.client.tvs_get_index(self.name)
         if self.params is None:
             # not exist
             raise ValueError("index not exist")
         return self.params
 
-    def tvs_hset(self, key: str, vector: Union[VectorType, str] = None, **kwargs):
+    def tvs_hset(self, key: str, vector: Union[VectorType, str, None] = None, **kwargs):
         """add/update a data entry to index
         @key: key for the data entry
         @vector: optional, vector value of the data entry
         @kwargs: optional, attribute pairs for the data entry
         """
         return self.client.tvs_hset(self.name, key, vector, self.is_binary, **kwargs)
 
     def tvs_knnsearch(
-        self, k: int, vector: Union[VectorType, str], filter_str: str = None, **kwargs
+        self,
+        k: int,
+        vector: Union[VectorType, str],
+        filter_str: Optional[str] = None,
+        **kwargs
     ):
         """search for the top @k approximate nearest neighbors of @vector"""
         return self.client.tvs_knnsearch(
             self.name, k, vector, self.is_binary, filter_str, **kwargs
         )
 
     def tvs_mknnsearch(
-        self, k: int, vectors: Sequence[VectorType], filter_str: str = None, **kwargs
+        self,
+        k: int,
+        vectors: Sequence[VectorType],
+        filter_str: Optional[str] = None,
+        **kwargs
     ):
         """batch approximate nearest neighbors search for a list of vectors"""
         return self.client.tvs_mknnsearch(
             self.name, k, vectors, self.is_binary, filter_str, **kwargs
         )
 
     def __str__(self):
@@ -216,21 +225,23 @@
     def tvs_del_index(self, name: str):
         """
         delete an index and all its data
         """
         return self.execute_command(self.DEL_INDEX_CMD, name)
 
     def tvs_scan_index(
-        self, pattern: str = None, batch: int = 10
+        self, pattern: Optional[str] = None, batch: int = 10
     ) -> TairVectorScanResult:
         """
         scan all the indices
         """
         args = ([] if pattern is None else ["MATCH", pattern]) + ["COUNT", batch]
-        get_batch = lambda c: self.execute_command(self.SCAN_INDEX_CMD, c, *args)
+
+        def get_batch(c):
+            return self.execute_command(self.SCAN_INDEX_CMD, c, *args)
 
         return TairVectorScanResult(self, get_batch)
 
     def tvs_index(self, name: str, **index_params) -> TairVectorIndex:
         """
         get or create an index
         """
@@ -243,15 +254,15 @@
     HMGET_CMD = "TVS.HMGET"
     SCAN_CMD = "TVS.SCAN"
 
     def tvs_hset(
         self,
         index: str,
         key: str,
-        vector: Union[VectorType, str] = None,
+        vector: Union[VectorType, str, None] = None,
         is_binary=False,
         **kwargs
     ):
         """
         add/update a data entry to index
           @index: index name
           @key: key for the data entry
@@ -294,35 +305,37 @@
         get specified attributes of a data entry, use attribute key "VECTOR" to get vector value
         """
         return self.execute_command(self.HMGET_CMD, index, key, *args)
 
     # def tvs_hmget(self, index: str, key: str,fields: Iterable[str]):
     #     return self.execute_command(self.HMGET_CMD, index,key, *fields)
 
-    def tvs_scan(self, index: str, pattern: str = None, batch: int = 10):
+    def tvs_scan(self, index: str, pattern: Optional[str] = None, batch: int = 10):
         """
         scan all data entries in an index
         """
         args = ([] if pattern is None else ["MATCH", pattern]) + ["COUNT", batch]
-        get_batch = lambda c: self.execute_command(self.SCAN_CMD, index, c, *args)
+
+        def get_batch(c):
+            return self.execute_command(self.SCAN_CMD, index, c, *args)
 
         return TairVectorScanResult(self, get_batch)
 
     SEARCH_CMD = "TVS.KNNSEARCH"
     MSEARCH_CMD = "TVS.MKNNSEARCH"
     MINDEXKNNSEARCH_CMD = "TVS.MINDEXKNNSEARCH"
     MINDEXMKNNSEARCH_CMD = "TVS.MINDEXMKNNSEARCH"
 
     def tvs_knnsearch(
         self,
         index: str,
         k: int,
         vector: Union[VectorType, str],
         is_binary: bool = False,
-        filter_str: str = None,
+        filter_str: Optional[str] = None,
         **kwargs
     ):
         """
         search for the top @k approximate nearest neighbors of @vector in an index
         """
         params = reduce(lambda x, y: x + y, kwargs.items(), ())
         if not isinstance(vector, str):
@@ -335,15 +348,15 @@
 
     def tvs_mknnsearch(
         self,
         index: str,
         k: int,
         vectors: Sequence[VectorType],
         is_binary: bool = False,
-        filter_str: str = None,
+        filter_str: Optional[str] = None,
         **kwargs
     ):
         """
         batch approximate nearest neighbors search for a list of vectors
         """
         params = reduce(lambda x, y: x + y, kwargs.items(), ())
         encoded_vectors = [
@@ -370,15 +383,15 @@
 
     def tvs_mindexknnsearch(
         self,
         index: Sequence[str],
         k: int,
         vector: Union[VectorType, str],
         is_binary: bool = False,
-        filter_str: str = None,
+        filter_str: Optional[str] = None,
         **kwargs
     ):
         """
         search for the top @k approximate nearest neighbors of @vector in indexs
         """
         params = reduce(lambda x, y: x + y, kwargs.items(), ())
         if not isinstance(vector, str):
@@ -393,15 +406,15 @@
 
     def tvs_mindexmknnsearch(
         self,
         index: Sequence[str],
         k: int,
         vectors: Sequence[VectorType],
         is_binary: bool = False,
-        filter_str: str = None,
+        filter_str: Optional[str] = None,
         **kwargs
     ):
         """
         batch approximate nearest neighbors search for a list of vectors
         """
         params = reduce(lambda x, y: x + y, kwargs.items(), ())
         encoded_vectors = [
@@ -442,18 +455,18 @@
         result[Constants.VECTOR_KEY] = TextVectorEncoder.decode(
             result[Constants.VECTOR_KEY]
         )
     values = map(str_if_bytes, result.values())
     return dict(zip(result.keys(), values))
 
 
-def parse_tvs_hmget_result(resp) -> tuple:
+def parse_tvs_hmget_result(resp) -> Optional[Tuple]:
     if len(resp) == 0:
         return None
-    return [resp[i].decode("ascii") if resp[i] else None for i in range(0, len(resp))]
+    return resp
 
 
 def parse_tvs_search_result(resp) -> List[Tuple]:
     return [(resp[i], float(resp[i + 1])) for i in range(0, len(resp), 2)]
 
 
 def parse_tvs_msearch_result(resp) -> List[List[Tuple]]:
```

### Comparing `tair-1.3.3/tair/tairzset.py` & `tair-1.3.4/tair/tairzset.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tair.egg-info/PKG-INFO` & `tair-1.3.4/tair.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tair
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python client for Tair
 Home-page: https://github.com/alibaba/tair-py
 Author: Vincil Lau
 Author-email: vincillau@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -25,15 +25,15 @@
 - [TairString](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairstring-commands), is a string that contains a version number. ([Open sourced](https://github.com/alibaba/TairString))
 - [TairHash](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairhash-commands), is a hash that allows you to specify the expiration time and version number of a field. ([Open sourced](https://github.com/alibaba/TairHash))
 - [TairZset](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairzset-commands), allows you to sort data of the double type based on multiple dimensions. ([Open sourced](https://github.com/alibaba/TairZset))
 - [TairBloom](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairbloom-commands), is a Bloom filter that supports dynamic scaling. (Coming soon)
 - [TairRoaring](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairroaring-commands), is a more efficient and balanced type of compressed bitmaps recognized by the industry. (Coming soon)
 - [TairSearch](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairsearch-command), is a full-text search module developed in-house based on Redis modules. (Coming soon)
 - [TairDoc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairdoc-commands), to perform create, read, update, and delete (CRUD) operations on JSON data. (Coming soon)
-- [TairGis](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairgis-commands), allowing you to query points, linestrings, and polygons. (Coming soon)
+- [TairGis](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairgis-commands), allowing you to query points, linestrings, and polygons. ([Open Sourced](https://github.com/tair-opensource/TairGis))
 - [TairTs](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairts-commands), is a time series data structure that is developed on top of Redis modules.  (Coming soon)
 - [TairCpc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/taircpc-commands), is a data structure developed based on the compressed probability counting (CPC) sketch. (Coming soon)
 - [TairVector](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairvector),  is a self-developed data structure that provides high-performance real-time storage and retrieval of vectors. (Coming soon)
 
 ## Install
 
 Install from pip:
```

### Comparing `tair-1.3.3/tair.egg-info/SOURCES.txt` & `tair-1.3.4/tair.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tests/test_from_url.py` & `tair-1.3.4/tests/test_from_url.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tests/test_pipeline.py` & `tair-1.3.4/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tests/test_tairbloom.py` & `tair-1.3.4/tests/test_tairbloom.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tests/test_taircpc.py` & `tair-1.3.4/tests/test_taircpc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tests/test_tairdoc.py` & `tair-1.3.4/tests/test_tairdoc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tests/test_tairgis.py` & `tair-1.3.4/tests/test_tairgis.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tests/test_tairhash.py` & `tair-1.3.4/tests/test_tairhash.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tests/test_tairroaring.py` & `tair-1.3.4/tests/test_tairroaring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tests/test_tairsearch.py` & `tair-1.3.4/tests/test_tairsearch.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tests/test_tairstring.py` & `tair-1.3.4/tests/test_tairstring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tests/test_tairts.py` & `tair-1.3.4/tests/test_tairts.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.3/tests/test_tairvector.py` & `tair-1.3.4/tests/test_tairvector.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             self.assertTrue(k in index)
             self.assertEqual(index[k], str(v))
 
     def test_6_scan_index(self):
         indices = []
         result = client.tvs_scan_index()
         for index in result.iter():
-            indices.append(index)
+            indices.append(index.decode())
         self.assertListEqual(indices, ["test"])
 
     def test_7_scan_index_with_pattern(self):
         indices = []
         result = client.tvs_scan_index(pattern="aaa")
         for index in result.iter():
             indices.append(index)
@@ -185,38 +185,38 @@
         value1 = "value_" + str(uuid.uuid4())
         value2 = "value_" + str(uuid.uuid4())
         ret = client.tvs_hset("test", key, vector=vector, field1=value1, field2=value2)
         self.assertTrue(ret)
         obj = client.tvs_hmget(
             "test", key, Constants.VECTOR_KEY, "field1", "field2", "field3"
         )
-        self.assertEqual(len(obj[0].split(",")), len(vector))
-        self.assertEqual(obj[1], str(value1))
-        self.assertEqual(obj[2], str(value2))
+        self.assertEqual(len(obj[0].split(b",")), len(vector))
+        self.assertEqual(obj[1], bytes(value1, encoding="ascii"))
+        self.assertEqual(obj[2], bytes(value2, encoding="ascii"))
 
     def test_4_scan(self):
         result = client.tvs_scan("test")
         scanned_keys = []
         for k in result.iter():
-            scanned_keys.append(k)
+            scanned_keys.append(k.decode())
         expected_keys = [str(i) for i in range(len(test_vectors))]
         self.assertSetEqual(set(scanned_keys), set(expected_keys))
 
     def test_5_scan_with_pattern(self):
         result = client.tvs_scan("test", pattern="aaa")
         scanned_keys = []
         for k in result.iter():
             scanned_keys.append(k)
         self.assertEqual(scanned_keys, [])
 
         result = client.tvs_scan("test", pattern="0")
         scanned_keys = []
         for k in result.iter():
             scanned_keys.append(k)
-        self.assertEqual(scanned_keys, ["0"])
+        self.assertEqual(scanned_keys, [b"0"])
 
     def test_6_hdel(self):
         for i, attr in enumerate(test_attributes):
             keys = attr.keys()
             self.assertEqual(client.tvs_hdel("test", str(i), *keys), len(keys))
 
     def test_7_delete(self):
@@ -363,15 +363,15 @@
             self.assertTrue(vectorEqual(v, obj[Constants.VECTOR_KEY]))
             del obj[Constants.VECTOR_KEY]
             self.assertDictEqual(obj, test_attributes[i])
 
         result = index.tvs_scan()
         scanned_keys = []
         for k in result.iter():
-            scanned_keys.append(k)
+            scanned_keys.append(k.decode())
         expected_keys = [str(i) for i in range(len(test_vectors))]
         self.assertSetEqual(set(scanned_keys), set(expected_keys))
 
         for i, attr in enumerate(test_attributes):
             keys = attr.keys()
             self.assertEqual(index.tvs_hdel(str(i), *keys), len(keys))
```

### Comparing `tair-1.3.3/tests/test_tairzset.py` & `tair-1.3.4/tests/test_tairzset.py`

 * *Files identical despite different names*

