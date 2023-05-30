# Comparing `tmp/dit_activity_stream-0.2.0.tar.gz` & `tmp/dit_activity_stream-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dit_activity_stream-0.2.0.tar", max compression
+gzip compressed data, was "dit_activity_stream-0.2.1.tar", max compression
```

## Comparing `dit_activity_stream-0.2.0.tar` & `dit_activity_stream-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1091 2022-11-17 16:47:15.957768 dit_activity_stream-0.2.0/LICENSE
--rw-r--r--   0        0        0     2678 2022-11-21 11:56:33.916206 dit_activity_stream-0.2.0/README.md
--rw-r--r--   0        0        0        0 2022-11-17 16:47:15.958280 dit_activity_stream-0.2.0/dit_activity_stream/__init__.py
--rw-r--r--   0        0        0     5272 2022-11-17 16:47:15.958448 dit_activity_stream-0.2.0/dit_activity_stream/client.py
--rw-r--r--   0        0        0        0 2022-11-17 16:47:15.958505 dit_activity_stream-0.2.0/dit_activity_stream/py.typed
--rw-r--r--   0        0        0        0 2022-11-17 16:47:15.958646 dit_activity_stream-0.2.0/dit_activity_stream/test_app/__init__.py
--rw-r--r--   0        0        0      257 2022-11-17 16:47:15.958783 dit_activity_stream-0.2.0/dit_activity_stream/test_app/apps.py
--rw-r--r--   0        0        0     1118 2022-11-17 16:47:15.958923 dit_activity_stream-0.2.0/dit_activity_stream/test_app/client.py
--rw-r--r--   0        0        0      321 2022-11-17 16:47:15.959043 dit_activity_stream-0.2.0/dit_activity_stream/test_app/factories.py
--rw-r--r--   0        0        0      336 2022-11-17 16:47:15.959163 dit_activity_stream-0.2.0/dit_activity_stream/test_app/models.py
--rw-r--r--   0        0        0     1398 2022-11-17 16:47:15.959307 dit_activity_stream-0.2.0/dit_activity_stream/test_app/settings.py
--rw-r--r--   0        0        0      128 2022-11-17 16:47:15.959434 dit_activity_stream-0.2.0/dit_activity_stream/test_app/urls.py
--rw-r--r--   0        0        0     1218 2022-11-17 16:47:15.959555 dit_activity_stream-0.2.0/dit_activity_stream/test_app/utils.py
--rw-r--r--   0        0        0        0 2022-11-17 16:47:15.959678 dit_activity_stream-0.2.0/dit_activity_stream/tests/__init__.py
--rw-r--r--   0        0        0      634 2022-11-17 16:47:15.959809 dit_activity_stream-0.2.0/dit_activity_stream/tests/test_client.py
--rw-r--r--   0        0        0     3869 2022-11-17 16:47:15.959944 dit_activity_stream-0.2.0/dit_activity_stream/tests/test_views.py
--rw-r--r--   0        0        0      168 2022-11-17 16:47:15.960056 dit_activity_stream-0.2.0/dit_activity_stream/urls.py
--rw-r--r--   0        0        0     1374 2022-11-18 13:29:28.471899 dit_activity_stream-0.2.0/dit_activity_stream/views.py
--rw-r--r--   0        0        0      788 2023-04-19 10:28:56.039099 dit_activity_stream-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 dit_activity_stream-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-11-17 16:47:15.957768 dit_activity_stream-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2678 2022-11-21 11:56:33.916206 dit_activity_stream-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2022-11-17 16:47:15.958280 dit_activity_stream-0.2.1/dit_activity_stream/__init__.py
+-rw-r--r--   0        0        0     5272 2022-11-17 16:47:15.958448 dit_activity_stream-0.2.1/dit_activity_stream/client.py
+-rw-r--r--   0        0        0        0 2022-11-17 16:47:15.958505 dit_activity_stream-0.2.1/dit_activity_stream/py.typed
+-rw-r--r--   0        0        0        0 2022-11-17 16:47:15.958646 dit_activity_stream-0.2.1/dit_activity_stream/test_app/__init__.py
+-rw-r--r--   0        0        0      257 2022-11-17 16:47:15.958783 dit_activity_stream-0.2.1/dit_activity_stream/test_app/apps.py
+-rw-r--r--   0        0        0     1118 2022-11-17 16:47:15.958923 dit_activity_stream-0.2.1/dit_activity_stream/test_app/client.py
+-rw-r--r--   0        0        0      321 2022-11-17 16:47:15.959043 dit_activity_stream-0.2.1/dit_activity_stream/test_app/factories.py
+-rw-r--r--   0        0        0      336 2022-11-17 16:47:15.959163 dit_activity_stream-0.2.1/dit_activity_stream/test_app/models.py
+-rw-r--r--   0        0        0     1398 2022-11-17 16:47:15.959307 dit_activity_stream-0.2.1/dit_activity_stream/test_app/settings.py
+-rw-r--r--   0        0        0      128 2022-11-17 16:47:15.959434 dit_activity_stream-0.2.1/dit_activity_stream/test_app/urls.py
+-rw-r--r--   0        0        0     1218 2022-11-17 16:47:15.959555 dit_activity_stream-0.2.1/dit_activity_stream/test_app/utils.py
+-rw-r--r--   0        0        0        0 2022-11-17 16:47:15.959678 dit_activity_stream-0.2.1/dit_activity_stream/tests/__init__.py
+-rw-r--r--   0        0        0      634 2022-11-17 16:47:15.959809 dit_activity_stream-0.2.1/dit_activity_stream/tests/test_client.py
+-rw-r--r--   0        0        0     3869 2022-11-17 16:47:15.959944 dit_activity_stream-0.2.1/dit_activity_stream/tests/test_views.py
+-rw-r--r--   0        0        0      168 2022-11-17 16:47:15.960056 dit_activity_stream-0.2.1/dit_activity_stream/urls.py
+-rw-r--r--   0        0        0     1374 2022-11-18 13:29:28.471899 dit_activity_stream-0.2.1/dit_activity_stream/views.py
+-rw-r--r--   0        0        0      788 2023-05-30 13:59:07.756204 dit_activity_stream-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 dit_activity_stream-0.2.1/PKG-INFO
```

### Comparing `dit_activity_stream-0.2.0/LICENSE` & `dit_activity_stream-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.2.0/README.md` & `dit_activity_stream-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.2.0/dit_activity_stream/client.py` & `dit_activity_stream-0.2.1/dit_activity_stream/client.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.2.0/dit_activity_stream/test_app/client.py` & `dit_activity_stream-0.2.1/dit_activity_stream/test_app/client.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.2.0/dit_activity_stream/test_app/settings.py` & `dit_activity_stream-0.2.1/dit_activity_stream/test_app/settings.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.2.0/dit_activity_stream/test_app/utils.py` & `dit_activity_stream-0.2.1/dit_activity_stream/test_app/utils.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.2.0/dit_activity_stream/tests/test_client.py` & `dit_activity_stream-0.2.1/dit_activity_stream/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.2.0/dit_activity_stream/tests/test_views.py` & `dit_activity_stream-0.2.1/dit_activity_stream/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.2.0/dit_activity_stream/views.py` & `dit_activity_stream-0.2.1/dit_activity_stream/views.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.2.0/pyproject.toml` & `dit_activity_stream-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "dit-activity-stream"
-version = "0.2.0"
+version = "0.2.1"
 description = "DIT Activity Stream"
 authors = [
     "Cameron Lamb <live.services@digital.trade.gov.uk>"
 ]
 license = "MIT"
 readme = "README.md"
 keywords = [
```

### Comparing `dit_activity_stream-0.2.0/PKG-INFO` & `dit_activity_stream-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dit-activity-stream
-Version: 0.2.0
+Version: 0.2.1
 Summary: DIT Activity Stream
 Home-page: https://github.com/uktrade/dit-activity-stream
 License: MIT
 Keywords: django
 Author: Cameron Lamb
 Author-email: live.services@digital.trade.gov.uk
 Requires-Python: >=3.7,<4.0
```

