# Comparing `tmp/everything2text4prompt-0.0.7.tar.gz` & `tmp/everything2text4prompt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "everything2text4prompt-0.0.7.tar", last modified: Fri May 26 16:20:12 2023, max compression
+gzip compressed data, was "everything2text4prompt-0.0.8.tar", last modified: Tue May 30 15:40:19 2023, max compression
```

## Comparing `everything2text4prompt-0.0.7.tar` & `everything2text4prompt-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 16:20:12.595820 everything2text4prompt-0.0.7/
--rw-rw-rw-   0        0        0     1089 2023-05-18 13:27:55.000000 everything2text4prompt-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1052 2023-05-26 16:20:12.594822 everything2text4prompt-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      658 2023-05-18 13:34:54.000000 everything2text4prompt-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 16:20:12.560448 everything2text4prompt-0.0.7/everything2text4prompt/
--rw-rw-rw-   0        0        0      234 2023-05-26 16:18:10.000000 everything2text4prompt-0.0.7/everything2text4prompt/__init__.py
--rw-rw-rw-   0        0        0     2385 2023-05-26 16:18:53.000000 everything2text4prompt-0.0.7/everything2text4prompt/everything2text4prompt.py
--rw-rw-rw-   0        0        0      452 2023-05-26 16:14:35.000000 everything2text4prompt-0.0.7/everything2text4prompt/pdf_util.py
-drwxrwxrwx   0        0        0        0 2023-05-26 16:20:12.592826 everything2text4prompt-0.0.7/everything2text4prompt/playground/
--rw-rw-rw-   0        0        0      754 2023-05-19 14:34:30.000000 everything2text4prompt-0.0.7/everything2text4prompt/playground/test_split_mp3.py
--rw-rw-rw-   0        0        0      340 2023-05-19 15:00:50.000000 everything2text4prompt-0.0.7/everything2text4prompt/playground/test_whisper.py
--rw-rw-rw-   0        0        0     1183 2023-05-26 16:14:59.000000 everything2text4prompt-0.0.7/everything2text4prompt/podcast_util.py
--rw-rw-rw-   0        0        0     2075 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.7/everything2text4prompt/util.py
--rw-rw-rw-   0        0        0     2444 2023-05-26 16:18:25.000000 everything2text4prompt-0.0.7/everything2text4prompt/youtube_util.py
-drwxrwxrwx   0        0        0        0 2023-05-26 16:20:12.572686 everything2text4prompt-0.0.7/everything2text4prompt.egg-info/
--rw-rw-rw-   0        0        0     1052 2023-05-26 16:20:12.000000 everything2text4prompt-0.0.7/everything2text4prompt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      585 2023-05-26 16:20:12.000000 everything2text4prompt-0.0.7/everything2text4prompt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 16:20:12.000000 everything2text4prompt-0.0.7/everything2text4prompt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-26 16:20:12.000000 everything2text4prompt-0.0.7/everything2text4prompt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-26 16:20:12.000000 everything2text4prompt-0.0.7/everything2text4prompt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 16:20:12.595820 everything2text4prompt-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-05-26 16:19:25.000000 everything2text4prompt-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:40:19.774934 everything2text4prompt-0.0.8/
+-rw-rw-rw-   0        0        0     1089 2023-05-18 13:27:55.000000 everything2text4prompt-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1052 2023-05-30 15:40:19.774934 everything2text4prompt-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-05-18 13:34:54.000000 everything2text4prompt-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 15:40:19.755960 everything2text4prompt-0.0.8/everything2text4prompt/
+-rw-rw-rw-   0        0        0      234 2023-05-26 16:18:10.000000 everything2text4prompt-0.0.8/everything2text4prompt/__init__.py
+-rw-rw-rw-   0        0        0     2423 2023-05-30 15:39:08.000000 everything2text4prompt-0.0.8/everything2text4prompt/everything2text4prompt.py
+-rw-rw-rw-   0        0        0      452 2023-05-26 16:14:35.000000 everything2text4prompt-0.0.8/everything2text4prompt/pdf_util.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:40:19.770919 everything2text4prompt-0.0.8/everything2text4prompt/playground/
+-rw-rw-rw-   0        0        0      754 2023-05-19 14:34:30.000000 everything2text4prompt-0.0.8/everything2text4prompt/playground/test_split_mp3.py
+-rw-rw-rw-   0        0        0      340 2023-05-19 15:00:50.000000 everything2text4prompt-0.0.8/everything2text4prompt/playground/test_whisper.py
+-rw-rw-rw-   0        0        0     1183 2023-05-26 16:14:59.000000 everything2text4prompt-0.0.8/everything2text4prompt/podcast_util.py
+-rw-rw-rw-   0        0        0     2223 2023-05-30 15:31:27.000000 everything2text4prompt-0.0.8/everything2text4prompt/util.py
+-rw-rw-rw-   0        0        0     3682 2023-05-30 15:39:12.000000 everything2text4prompt-0.0.8/everything2text4prompt/youtube_util.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:40:19.765933 everything2text4prompt-0.0.8/everything2text4prompt.egg-info/
+-rw-rw-rw-   0        0        0     1052 2023-05-30 15:40:19.000000 everything2text4prompt-0.0.8/everything2text4prompt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2023-05-30 15:40:19.000000 everything2text4prompt-0.0.8/everything2text4prompt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 15:40:19.000000 everything2text4prompt-0.0.8/everything2text4prompt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-30 15:40:19.000000 everything2text4prompt-0.0.8/everything2text4prompt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-30 15:40:19.000000 everything2text4prompt-0.0.8/everything2text4prompt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 15:40:19.775948 everything2text4prompt-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-05-30 15:40:04.000000 everything2text4prompt-0.0.8/setup.py
```

### Comparing `everything2text4prompt-0.0.7/LICENSE` & `everything2text4prompt-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.7/PKG-INFO` & `everything2text4prompt-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everything2text4prompt
-Version: 0.0.7
+Version: 0.0.8
 Summary: Convert many medium into text, and the text format is specialized for prompt input
 Home-page: https://github.com/michaelthwan/everything2text4prompt
 Author: michaethwan
 Author-email: michaelthwan@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `everything2text4prompt-0.0.7/README.md` & `everything2text4prompt-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.7/everything2text4prompt/everything2text4prompt.py` & `everything2text4prompt-0.0.8/everything2text4prompt/everything2text4prompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,7 +43,8 @@
     # TODO: Not sure why it is not working after chunking
     # 通用人工智能离我们多远，大模型专家访谈 ｜S7E11 硅谷徐老师 x OnBoard！
     # target_source = "https://podcasts.google.com/feed/aHR0cHM6Ly9mZWVkcy5maXJlc2lkZS5mbS9ndWlndXphb3poaWRhby9yc3M/episode/YzIxOWI4ZjktNTZiZi00NGQ3LTg3NjctYWZiNTQzOWZjMTNk?sa=X&ved=0CAUQkfYCahcKEwjwp9icjv_-AhUAAAAAHQAAAAAQLA&hl=zh-TW"
 
     data, is_success, error_msg = converter.convert_text(medium, target_source)
     print(data.shorten_transcript)
     print(is_success, error_msg)
+    # print(data.ts_transcript_list)
```

### Comparing `everything2text4prompt-0.0.7/everything2text4prompt/playground/test_split_mp3.py` & `everything2text4prompt-0.0.8/everything2text4prompt/playground/test_split_mp3.py`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.7/everything2text4prompt/podcast_util.py` & `everything2text4prompt-0.0.8/everything2text4prompt/podcast_util.py`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.7/everything2text4prompt/util.py` & `everything2text4prompt-0.0.8/everything2text4prompt/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,29 @@
     def shorten_text(self, text: str) -> str:
         if text is None or len(text) < 120:
             return text
         return text[:50] + " ... " + text[-50:]
 
 
 class YoutubeData(BaseData):
-    def __init__(self, transcript, title, description):
+    def __init__(self, transcript, title, description, ts_transcript_list):
         super().__init__(transcript)
         self.title = title
         self.description = description
         self.shorten_transcript = self.shorten_text(transcript)
+        self.ts_transcript_list = ts_transcript_list
 
 
 class PodcastData(BaseData):
-    def __init__(self, transcript, title, description):
+    def __init__(self, transcript, title, description, ts_transcript_list):
         super().__init__(transcript)
         self.title = title
         self.description = description
         self.shorten_transcript = self.shorten_text(transcript)
+        self.ts_transcript_list = ts_transcript_list
 
 
 def chunk_mp3(file_path: str) -> list:
     chunk_size = 20 * 1024 * 1024  # 20MB
 
     with open(file_path, "rb") as f:
         data = f.read()  # Read the file as binary data
```

### Comparing `everything2text4prompt-0.0.7/everything2text4prompt.egg-info/PKG-INFO` & `everything2text4prompt-0.0.8/everything2text4prompt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everything2text4prompt
-Version: 0.0.7
+Version: 0.0.8
 Summary: Convert many medium into text, and the text format is specialized for prompt input
 Home-page: https://github.com/michaelthwan/everything2text4prompt
 Author: michaethwan
 Author-email: michaelthwan@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `everything2text4prompt-0.0.7/everything2text4prompt.egg-info/SOURCES.txt` & `everything2text4prompt-0.0.8/everything2text4prompt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.7/setup.py` & `everything2text4prompt-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="everything2text4prompt",
-    version="0.0.7",
+    version="0.0.8",
     description="Convert many medium into text, and the text format is specialized for prompt input",
     # package_dir={'': 'everything2text4prompt'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/michaelthwan/everything2text4prompt",
     author="michaethwan",
```

