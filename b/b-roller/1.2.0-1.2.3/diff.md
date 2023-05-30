# Comparing `tmp/b-roller-1.2.0.tar.gz` & `tmp/b_roller-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b-roller-1.2.0.tar", max compression
+gzip compressed data, was "b_roller-1.2.3.tar", max compression
```

## Comparing `b-roller-1.2.0.tar` & `b_roller-1.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       22 2023-01-21 21:39:16.475309 b-roller-1.2.0/b_roller/__init__.py
--rw-r--r--   0        0        0     2937 2023-01-21 21:39:16.475309 b-roller-1.2.0/b_roller/__main__.py
--rw-r--r--   0        0        0      530 2023-01-21 21:39:16.475309 b-roller-1.2.0/b_roller/credits.py
--rw-r--r--   0        0        0     1218 2023-01-21 21:39:16.475309 b-roller-1.2.0/b_roller/iconfinder.py
--rw-r--r--   0        0        0     1566 2023-01-21 21:39:16.475309 b-roller-1.2.0/b_roller/pexels.py
--rw-r--r--   0        0        0     3932 2023-01-21 21:39:16.475309 b-roller-1.2.0/b_roller/youtube.py
--rw-r--r--   0        0        0     1275 2023-01-21 21:39:16.475309 b-roller-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      511 2023-01-21 21:39:16.475309 b-roller-1.2.0/readme.md
--rw-r--r--   0        0        0     1348 2023-01-21 21:39:43.661258 b-roller-1.2.0/setup.py
--rw-r--r--   0        0        0     1171 2023-01-21 21:39:43.661553 b-roller-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-25 18:28:56.550445 b_roller-1.2.3/b_roller/__init__.py
+-rw-r--r--   0        0        0     2937 2023-05-25 17:54:38.831967 b_roller-1.2.3/b_roller/__main__.py
+-rw-r--r--   0        0        0      530 2023-05-25 17:54:38.832120 b_roller-1.2.3/b_roller/credits.py
+-rw-r--r--   0        0        0     1218 2023-05-25 17:54:38.832239 b_roller-1.2.3/b_roller/iconfinder.py
+-rw-r--r--   0        0        0     1566 2023-05-25 17:54:38.832426 b_roller-1.2.3/b_roller/pexels.py
+-rw-r--r--   0        0        0     3931 2023-05-25 18:27:48.492423 b_roller-1.2.3/b_roller/youtube.py
+-rw-r--r--   0        0        0     1291 2023-05-30 07:46:31.481192 b_roller-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0      511 2023-05-25 17:54:38.833214 b_roller-1.2.3/readme.md
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 b_roller-1.2.3/setup.py
+-rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 b_roller-1.2.3/PKG-INFO
```

### Comparing `b-roller-1.2.0/b_roller/__main__.py` & `b_roller-1.2.3/b_roller/__main__.py`

 * *Files identical despite different names*

### Comparing `b-roller-1.2.0/b_roller/credits.py` & `b_roller-1.2.3/b_roller/credits.py`

 * *Files identical despite different names*

### Comparing `b-roller-1.2.0/b_roller/iconfinder.py` & `b_roller-1.2.3/b_roller/iconfinder.py`

 * *Files identical despite different names*

### Comparing `b-roller-1.2.0/b_roller/pexels.py` & `b_roller-1.2.3/b_roller/pexels.py`

 * *Files identical despite different names*

### Comparing `b-roller-1.2.0/b_roller/youtube.py` & `b_roller-1.2.3/b_roller/youtube.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,14 @@
 def ffmpeg_processing(
     audio_file: Path,
     video_file: Path,
     original_name: str,
     end_time: Optional[str] = None,
     start_time: Optional[str] = None,
 ) -> None:
-
     ffmpeg_arguments = {}
     if start_time:
         ffmpeg_arguments["ss"] = start_time
     if end_time:
         ffmpeg_arguments["to"] = end_time
     input_video = ffmpeg.input(str(video_file), **ffmpeg_arguments)
     input_audio = ffmpeg.input(str(audio_file), **ffmpeg_arguments)
```

### Comparing `b-roller-1.2.0/pyproject.toml` & `b_roller-1.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "b-roller"
-version = "1.2.0"
+version = "1.2.3"
 description = "Download resources from several sources across the web"
 readme = "readme.md"
 authors = ["Antonio Feregrino <antonio.feregrino@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "b_roller" },
 ]
@@ -15,14 +15,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 pytube = "*"
 typer = "*"
 python-slugify = "*"
 requests = "*"
 ffmpeg-python = "^0.2.0"
+urllib3 = "<=2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 black = "*"
 flake8 = "^5.0.4"
 isort = "^5.9.2"
 pyproject-flake8 = "^5.0.4.post1"
```

### Comparing `b-roller-1.2.0/setup.py` & `b_roller-1.2.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 packages = \
 ['b_roller']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['ffmpeg-python>=0.2.0,<0.3.0', 'python-slugify', 'pytube', 'requests', 'typer']
+['ffmpeg-python>=0.2.0,<0.3.0',
+ 'python-slugify',
+ 'pytube',
+ 'requests',
+ 'typer',
+ 'urllib3<=2']
 
 entry_points = \
 {'console_scripts': ['broll = b_roller.__main__:app']}
 
 setup_kwargs = {
     'name': 'b-roller',
-    'version': '1.2.0',
+    'version': '1.2.3',
     'description': 'Download resources from several sources across the web',
     'long_description': '# B-Roller\n\nDownload B-roll footage from YouTube **for fair use purposes**.\n\n## Usage\n\n### Download from YouTube\n\n```\nbroll yt [OPTIONS] URL [START] [END]\n\n  Download content from YouTube\n\nArguments:\n  URL      A video id or a YouTube short/long url  [required]\n  [START]  The desired start of the video in seconds or the format 00:00:00\n  [END]    The desired end of the video in seconds or the format 00:00:00\n```\n\nFor example:\n\n```shell\nbroll yt "https://www.youtube.com/watch?v=QFLiIU8g-R0" 00:10 00:17\n```\n',
     'author': 'Antonio Feregrino',
     'author_email': 'antonio.feregrino@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `b-roller-1.2.0/PKG-INFO` & `b_roller-1.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: b-roller
-Version: 1.2.0
+Version: 1.2.3
 Summary: Download resources from several sources across the web
 License: MIT
 Author: Antonio Feregrino
 Author-email: antonio.feregrino@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: python-slugify
 Requires-Dist: pytube
 Requires-Dist: requests
 Requires-Dist: typer
+Requires-Dist: urllib3 (<=2)
 Description-Content-Type: text/markdown
 
 # B-Roller
 
 Download B-roll footage from YouTube **for fair use purposes**.
 
 ## Usage
```

