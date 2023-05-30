# Comparing `tmp/ansq-0.2.0.tar.gz` & `tmp/ansq-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansq-0.2.0.tar", last modified: Tue Jan 24 22:35:19 2023, max compression
+gzip compressed data, was "ansq-0.2.1.tar", last modified: Tue May 30 13:26:05 2023, max compression
```

## Comparing `ansq-0.2.0.tar` & `ansq-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,51 @@
-drwxr-xr-x   0 os         (501) staff       (20)        0 2023-01-24 22:35:19.359445 ansq-0.2.0/
--rw-r--r--   0 os         (501) staff       (20)     1133 2022-05-31 08:29:33.000000 ansq-0.2.0/LICENSE
--rw-r--r--   0 os         (501) staff       (20)     2980 2023-01-24 22:35:19.362142 ansq-0.2.0/PKG-INFO
--rw-r--r--   0 os         (501) staff       (20)     2198 2023-01-24 15:58:25.000000 ansq-0.2.0/README.md
-drwxr-xr-x   0 os         (501) staff       (20)        0 2023-01-24 22:35:19.345241 ansq-0.2.0/ansq/
--rw-r--r--   0 os         (501) staff       (20)      313 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/__init__.py
-drwxr-xr-x   0 os         (501) staff       (20)        0 2023-01-24 22:35:19.348232 ansq-0.2.0/ansq/http/
--rw-r--r--   0 os         (501) staff       (20)      111 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/http/__init__.py
--rw-r--r--   0 os         (501) staff       (20)     2241 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/http/base.py
--rw-r--r--   0 os         (501) staff       (20)     1210 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/http/http_exceptions.py
--rw-r--r--   0 os         (501) staff       (20)     2916 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/http/lookupd.py
--rw-r--r--   0 os         (501) staff       (20)     4386 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/http/writer.py
-drwxr-xr-x   0 os         (501) staff       (20)        0 2023-01-24 22:35:19.354986 ansq-0.2.0/ansq/tcp/
--rw-r--r--   0 os         (501) staff       (20)        0 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/tcp/__init__.py
--rw-r--r--   0 os         (501) staff       (20)    21127 2023-01-24 15:58:25.000000 ansq-0.2.0/ansq/tcp/connection.py
--rw-r--r--   0 os         (501) staff       (20)      245 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/tcp/consts.py
--rw-r--r--   0 os         (501) staff       (20)     2271 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/tcp/exceptions.py
--rw-r--r--   0 os         (501) staff       (20)     5483 2023-01-24 15:58:25.000000 ansq-0.2.0/ansq/tcp/protocol.py
--rw-r--r--   0 os         (501) staff       (20)    11956 2023-01-24 15:58:25.000000 ansq-0.2.0/ansq/tcp/reader.py
-drwxr-xr-x   0 os         (501) staff       (20)        0 2023-01-24 22:35:19.359279 ansq-0.2.0/ansq/tcp/types/
--rw-r--r--   0 os         (501) staff       (20)      584 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/tcp/types/__init__.py
--rw-r--r--   0 os         (501) staff       (20)     2388 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/tcp/types/client.py
--rw-r--r--   0 os         (501) staff       (20)      332 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/tcp/types/commands.py
--rw-r--r--   0 os         (501) staff       (20)     9900 2023-01-24 15:58:25.000000 ansq-0.2.0/ansq/tcp/types/connection.py
--rw-r--r--   0 os         (501) staff       (20)      790 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/tcp/types/connection_status.py
--rw-r--r--   0 os         (501) staff       (20)      347 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/tcp/types/frame_type.py
--rw-r--r--   0 os         (501) staff       (20)     4241 2023-01-24 15:58:25.000000 ansq-0.2.0/ansq/tcp/types/message.py
--rw-r--r--   0 os         (501) staff       (20)     2486 2023-01-24 15:58:25.000000 ansq-0.2.0/ansq/tcp/types/response_schemas.py
--rw-r--r--   0 os         (501) staff       (20)     2181 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/tcp/writer.py
--rw-r--r--   0 os         (501) staff       (20)      281 2022-05-31 08:29:33.000000 ansq-0.2.0/ansq/typedefs.py
--rw-r--r--   0 os         (501) staff       (20)     5386 2023-01-24 15:58:25.000000 ansq-0.2.0/ansq/utils.py
-drwxr-xr-x   0 os         (501) staff       (20)        0 2023-01-24 22:35:19.346410 ansq-0.2.0/ansq.egg-info/
--rw-r--r--   0 os         (501) staff       (20)     2980 2023-01-24 22:35:19.000000 ansq-0.2.0/ansq.egg-info/PKG-INFO
--rw-r--r--   0 os         (501) staff       (20)      712 2023-01-24 22:35:19.000000 ansq-0.2.0/ansq.egg-info/SOURCES.txt
--rw-r--r--   0 os         (501) staff       (20)        1 2023-01-24 22:35:19.000000 ansq-0.2.0/ansq.egg-info/dependency_links.txt
--rw-r--r--   0 os         (501) staff       (20)      129 2023-01-24 22:35:19.000000 ansq-0.2.0/ansq.egg-info/requires.txt
--rw-r--r--   0 os         (501) staff       (20)        5 2023-01-24 22:35:19.000000 ansq-0.2.0/ansq.egg-info/top_level.txt
--rw-r--r--   0 os         (501) staff       (20)     1508 2023-01-24 22:35:19.365516 ansq-0.2.0/setup.cfg
--rw-r--r--   0 os         (501) staff       (20)       38 2022-05-31 08:29:33.000000 ansq-0.2.0/setup.py
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.032036 ansq-0.2.1/
+-rw-r--r--   0 os         (501) staff       (20)     1133 2022-05-31 08:29:33.000000 ansq-0.2.1/LICENSE
+-rw-r--r--   0 os         (501) staff       (20)     2960 2023-05-30 13:26:05.032122 ansq-0.2.1/PKG-INFO
+-rw-r--r--   0 os         (501) staff       (20)     2198 2023-01-24 15:58:25.000000 ansq-0.2.1/README.md
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.026155 ansq-0.2.1/ansq/
+-rw-r--r--   0 os         (501) staff       (20)      313 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/__init__.py
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.027793 ansq-0.2.1/ansq/http/
+-rw-r--r--   0 os         (501) staff       (20)      111 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/http/__init__.py
+-rw-r--r--   0 os         (501) staff       (20)     2241 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/http/base.py
+-rw-r--r--   0 os         (501) staff       (20)     1210 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/http/http_exceptions.py
+-rw-r--r--   0 os         (501) staff       (20)     2916 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/http/lookupd.py
+-rw-r--r--   0 os         (501) staff       (20)     4386 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/http/writer.py
+-rw-r--r--   0 os         (501) staff       (20)        0 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/py.typed
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.029019 ansq-0.2.1/ansq/tcp/
+-rw-r--r--   0 os         (501) staff       (20)        0 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/__init__.py
+-rw-r--r--   0 os         (501) staff       (20)    21127 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/tcp/connection.py
+-rw-r--r--   0 os         (501) staff       (20)      245 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/consts.py
+-rw-r--r--   0 os         (501) staff       (20)     2271 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/exceptions.py
+-rw-r--r--   0 os         (501) staff       (20)     5483 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/tcp/protocol.py
+-rw-r--r--   0 os         (501) staff       (20)    11956 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/tcp/reader.py
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.030419 ansq-0.2.1/ansq/tcp/types/
+-rw-r--r--   0 os         (501) staff       (20)      584 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/types/__init__.py
+-rw-r--r--   0 os         (501) staff       (20)     2388 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/types/client.py
+-rw-r--r--   0 os         (501) staff       (20)      332 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/types/commands.py
+-rw-r--r--   0 os         (501) staff       (20)     9900 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/tcp/types/connection.py
+-rw-r--r--   0 os         (501) staff       (20)      862 2023-05-30 13:05:57.000000 ansq-0.2.1/ansq/tcp/types/connection_status.py
+-rw-r--r--   0 os         (501) staff       (20)      362 2023-05-30 13:05:57.000000 ansq-0.2.1/ansq/tcp/types/frame_type.py
+-rw-r--r--   0 os         (501) staff       (20)     4241 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/tcp/types/message.py
+-rw-r--r--   0 os         (501) staff       (20)     2486 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/tcp/types/response_schemas.py
+-rw-r--r--   0 os         (501) staff       (20)     2181 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/tcp/writer.py
+-rw-r--r--   0 os         (501) staff       (20)      281 2022-05-31 08:29:33.000000 ansq-0.2.1/ansq/typedefs.py
+-rw-r--r--   0 os         (501) staff       (20)     5386 2023-01-24 15:58:25.000000 ansq-0.2.1/ansq/utils.py
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.027013 ansq-0.2.1/ansq.egg-info/
+-rw-r--r--   0 os         (501) staff       (20)     2960 2023-05-30 13:26:05.000000 ansq-0.2.1/ansq.egg-info/PKG-INFO
+-rw-r--r--   0 os         (501) staff       (20)      999 2023-05-30 13:26:05.000000 ansq-0.2.1/ansq.egg-info/SOURCES.txt
+-rw-r--r--   0 os         (501) staff       (20)        1 2023-05-30 13:26:05.000000 ansq-0.2.1/ansq.egg-info/dependency_links.txt
+-rw-r--r--   0 os         (501) staff       (20)      129 2023-05-30 13:26:05.000000 ansq-0.2.1/ansq.egg-info/requires.txt
+-rw-r--r--   0 os         (501) staff       (20)        5 2023-05-30 13:26:05.000000 ansq-0.2.1/ansq.egg-info/top_level.txt
+-rw-r--r--   0 os         (501) staff       (20)     1508 2023-05-30 13:26:05.032544 ansq-0.2.1/setup.cfg
+-rw-r--r--   0 os         (501) staff       (20)       38 2022-05-31 08:29:33.000000 ansq-0.2.1/setup.py
+drwxr-xr-x   0 os         (501) staff       (20)        0 2023-05-30 13:26:05.031912 ansq-0.2.1/tests/
+-rw-r--r--   0 os         (501) staff       (20)     3118 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_connection.py
+-rw-r--r--   0 os         (501) staff       (20)     3447 2022-05-31 08:29:33.000000 ansq-0.2.1/tests/test_convert_to_bytes.py
+-rw-r--r--   0 os         (501) staff       (20)     2362 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_http_writer.py
+-rw-r--r--   0 os         (501) staff       (20)     7287 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_read_messages.py
+-rw-r--r--   0 os         (501) staff       (20)     2712 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_reader.py
+-rw-r--r--   0 os         (501) staff       (20)     3118 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_reader_lookupd.py
+-rw-r--r--   0 os         (501) staff       (20)     2728 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_send_commands.py
+-rw-r--r--   0 os         (501) staff       (20)      930 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_utils.py
+-rw-r--r--   0 os         (501) staff       (20)      893 2022-05-31 08:29:33.000000 ansq-0.2.1/tests/test_validation_topic_channel_name.py
+-rw-r--r--   0 os         (501) staff       (20)     2110 2023-01-24 15:58:25.000000 ansq-0.2.1/tests/test_writer.py
```

### Comparing `ansq-0.2.0/LICENSE` & `ansq-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/PKG-INFO` & `ansq-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ansq
-Version: 0.2.0
+Version: 0.2.1
 Summary: Written with native Asyncio NSQ package
 Home-page: https://github.com/list-family/ansq
 Author: LiST
 Author-email: info@list.family
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -127,9 +126,7 @@
 ```
 
 Run tests.
 
 ```bash
 pytest
 ```
-
-
```

### Comparing `ansq-0.2.0/README.md` & `ansq-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/http/base.py` & `ansq-0.2.1/ansq/http/base.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/http/http_exceptions.py` & `ansq-0.2.1/ansq/http/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/http/lookupd.py` & `ansq-0.2.1/ansq/http/lookupd.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/http/writer.py` & `ansq-0.2.1/ansq/http/writer.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/tcp/connection.py` & `ansq-0.2.1/ansq/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/tcp/exceptions.py` & `ansq-0.2.1/ansq/tcp/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/tcp/protocol.py` & `ansq-0.2.1/ansq/tcp/protocol.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/tcp/reader.py` & `ansq-0.2.1/ansq/tcp/reader.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/tcp/types/__init__.py` & `ansq-0.2.1/ansq/tcp/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/tcp/types/client.py` & `ansq-0.2.1/ansq/tcp/types/client.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/tcp/types/connection.py` & `ansq-0.2.1/ansq/tcp/types/connection.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/tcp/types/message.py` & `ansq-0.2.1/ansq/tcp/types/message.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/tcp/types/response_schemas.py` & `ansq-0.2.1/ansq/tcp/types/response_schemas.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/tcp/writer.py` & `ansq-0.2.1/ansq/tcp/writer.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq/utils.py` & `ansq-0.2.1/ansq/utils.py`

 * *Files identical despite different names*

### Comparing `ansq-0.2.0/ansq.egg-info/PKG-INFO` & `ansq-0.2.1/ansq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ansq
-Version: 0.2.0
+Version: 0.2.1
 Summary: Written with native Asyncio NSQ package
 Home-page: https://github.com/list-family/ansq
 Author: LiST
 Author-email: info@list.family
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -127,9 +126,7 @@
 ```
 
 Run tests.
 
 ```bash
 pytest
 ```
-
-
```

### Comparing `ansq-0.2.0/setup.cfg` & `ansq-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ansq
-version = 0.2.0
+version = 0.2.1
 description = Written with native Asyncio NSQ package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/list-family/ansq
 author = LiST
 author_email = info@list.family
 license = MIT
```

