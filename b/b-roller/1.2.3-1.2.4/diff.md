# Comparing `tmp/b_roller-1.2.3.tar.gz` & `tmp/b_roller-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b_roller-1.2.3.tar", max compression
+gzip compressed data, was "b_roller-1.2.4.tar", max compression
```

## Comparing `b_roller-1.2.3.tar` & `b_roller-1.2.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       22 2023-05-25 18:28:56.550445 b_roller-1.2.3/b_roller/__init__.py
--rw-r--r--   0        0        0     2937 2023-05-25 17:54:38.831967 b_roller-1.2.3/b_roller/__main__.py
--rw-r--r--   0        0        0      530 2023-05-25 17:54:38.832120 b_roller-1.2.3/b_roller/credits.py
--rw-r--r--   0        0        0     1218 2023-05-25 17:54:38.832239 b_roller-1.2.3/b_roller/iconfinder.py
--rw-r--r--   0        0        0     1566 2023-05-25 17:54:38.832426 b_roller-1.2.3/b_roller/pexels.py
--rw-r--r--   0        0        0     3931 2023-05-25 18:27:48.492423 b_roller-1.2.3/b_roller/youtube.py
--rw-r--r--   0        0        0     1291 2023-05-30 07:46:31.481192 b_roller-1.2.3/pyproject.toml
--rw-r--r--   0        0        0      511 2023-05-25 17:54:38.833214 b_roller-1.2.3/readme.md
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 b_roller-1.2.3/setup.py
--rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 b_roller-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-30 07:53:09.739147 b_roller-1.2.4/b_roller/__init__.py
+-rw-r--r--   0        0        0     2937 2023-05-30 07:53:09.739147 b_roller-1.2.4/b_roller/__main__.py
+-rw-r--r--   0        0        0      530 2023-05-30 07:53:09.739147 b_roller-1.2.4/b_roller/credits.py
+-rw-r--r--   0        0        0     1218 2023-05-30 07:53:09.739147 b_roller-1.2.4/b_roller/iconfinder.py
+-rw-r--r--   0        0        0     1566 2023-05-30 07:53:09.739147 b_roller-1.2.4/b_roller/pexels.py
+-rw-r--r--   0        0        0     3931 2023-05-30 07:53:09.739147 b_roller-1.2.4/b_roller/youtube.py
+-rw-r--r--   0        0        0     1291 2023-05-30 07:53:09.739147 b_roller-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0      511 2023-05-30 07:53:09.739147 b_roller-1.2.4/readme.md
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 b_roller-1.2.4/setup.py
+-rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 b_roller-1.2.4/PKG-INFO
```

### Comparing `b_roller-1.2.3/b_roller/__main__.py` & `b_roller-1.2.4/b_roller/__main__.py`

 * *Files identical despite different names*

### Comparing `b_roller-1.2.3/b_roller/credits.py` & `b_roller-1.2.4/b_roller/credits.py`

 * *Files identical despite different names*

### Comparing `b_roller-1.2.3/b_roller/iconfinder.py` & `b_roller-1.2.4/b_roller/iconfinder.py`

 * *Files identical despite different names*

### Comparing `b_roller-1.2.3/b_roller/pexels.py` & `b_roller-1.2.4/b_roller/pexels.py`

 * *Files identical despite different names*

### Comparing `b_roller-1.2.3/b_roller/youtube.py` & `b_roller-1.2.4/b_roller/youtube.py`

 * *Files identical despite different names*

### Comparing `b_roller-1.2.3/pyproject.toml` & `b_roller-1.2.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "b-roller"
-version = "1.2.3"
+version = "1.2.4"
 description = "Download resources from several sources across the web"
 readme = "readme.md"
 authors = ["Antonio Feregrino <antonio.feregrino@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "b_roller" },
 ]
```

### Comparing `b_roller-1.2.3/setup.py` & `b_roller-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'urllib3<=2']
 
 entry_points = \
 {'console_scripts': ['broll = b_roller.__main__:app']}
 
 setup_kwargs = {
     'name': 'b-roller',
-    'version': '1.2.3',
+    'version': '1.2.4',
     'description': 'Download resources from several sources across the web',
     'long_description': '# B-Roller\n\nDownload B-roll footage from YouTube **for fair use purposes**.\n\n## Usage\n\n### Download from YouTube\n\n```\nbroll yt [OPTIONS] URL [START] [END]\n\n  Download content from YouTube\n\nArguments:\n  URL      A video id or a YouTube short/long url  [required]\n  [START]  The desired start of the video in seconds or the format 00:00:00\n  [END]    The desired end of the video in seconds or the format 00:00:00\n```\n\nFor example:\n\n```shell\nbroll yt "https://www.youtube.com/watch?v=QFLiIU8g-R0" 00:10 00:17\n```\n',
     'author': 'Antonio Feregrino',
     'author_email': 'antonio.feregrino@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `b_roller-1.2.3/PKG-INFO` & `b_roller-1.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b-roller
-Version: 1.2.3
+Version: 1.2.4
 Summary: Download resources from several sources across the web
 License: MIT
 Author: Antonio Feregrino
 Author-email: antonio.feregrino@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

