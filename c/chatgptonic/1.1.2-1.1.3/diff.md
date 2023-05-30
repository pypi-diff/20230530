# Comparing `tmp/chatgptonic-1.1.2.tar.gz` & `tmp/chatgptonic-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgptonic-1.1.2.tar", last modified: Fri May 26 15:33:46 2023, max compression
+gzip compressed data, was "chatgptonic-1.1.3.tar", last modified: Tue May 30 00:27:00 2023, max compression
```

## Comparing `chatgptonic-1.1.2.tar` & `chatgptonic-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-26 15:33:46.641603 chatgptonic-1.1.2/
--rw-r--r--   0 howardmederiros   (501) staff       (20)      537 2023-05-26 15:33:46.641417 chatgptonic-1.1.2/PKG-INFO
--rw-r--r--   0 howardmederiros   (501) staff       (20)      301 2023-03-13 16:03:22.000000 chatgptonic-1.1.2/README.md
-drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-26 15:33:46.640002 chatgptonic-1.1.2/chatgptonic/
--rw-r--r--   0 howardmederiros   (501) staff       (20)       67 2023-05-26 15:31:08.000000 chatgptonic-1.1.2/chatgptonic/__init__.py
--rw-r--r--   0 howardmederiros   (501) staff       (20)     2200 2023-05-26 15:31:08.000000 chatgptonic-1.1.2/chatgptonic/integration.py
-drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-26 15:33:46.641107 chatgptonic-1.1.2/chatgptonic.egg-info/
--rw-r--r--   0 howardmederiros   (501) staff       (20)      537 2023-05-26 15:33:46.000000 chatgptonic-1.1.2/chatgptonic.egg-info/PKG-INFO
--rw-r--r--   0 howardmederiros   (501) staff       (20)      277 2023-05-26 15:33:46.000000 chatgptonic-1.1.2/chatgptonic.egg-info/SOURCES.txt
--rw-r--r--   0 howardmederiros   (501) staff       (20)        1 2023-05-26 15:33:46.000000 chatgptonic-1.1.2/chatgptonic.egg-info/dependency_links.txt
--rw-r--r--   0 howardmederiros   (501) staff       (20)        1 2023-03-13 16:03:25.000000 chatgptonic-1.1.2/chatgptonic.egg-info/not-zip-safe
--rw-r--r--   0 howardmederiros   (501) staff       (20)       88 2023-05-26 15:33:46.000000 chatgptonic-1.1.2/chatgptonic.egg-info/requires.txt
--rw-r--r--   0 howardmederiros   (501) staff       (20)       12 2023-05-26 15:33:46.000000 chatgptonic-1.1.2/chatgptonic.egg-info/top_level.txt
--rw-r--r--   0 howardmederiros   (501) staff       (20)       38 2023-05-26 15:33:46.641676 chatgptonic-1.1.2/setup.cfg
--rw-r--r--   0 howardmederiros   (501) staff       (20)      949 2023-05-26 15:33:02.000000 chatgptonic-1.1.2/setup.py
+drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-30 00:27:00.809827 chatgptonic-1.1.3/
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      537 2023-05-30 00:27:00.809669 chatgptonic-1.1.3/PKG-INFO
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      301 2023-03-13 16:03:22.000000 chatgptonic-1.1.3/README.md
+drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-30 00:27:00.805139 chatgptonic-1.1.3/chatgptonic/
+-rw-r--r--   0 howardmederiros   (501) staff       (20)       67 2023-05-26 15:31:08.000000 chatgptonic-1.1.3/chatgptonic/__init__.py
+-rw-r--r--   0 howardmederiros   (501) staff       (20)     2226 2023-05-30 00:26:35.000000 chatgptonic-1.1.3/chatgptonic/integration.py
+drwxr-xr-x   0 howardmederiros   (501) staff       (20)        0 2023-05-30 00:27:00.808590 chatgptonic-1.1.3/chatgptonic.egg-info/
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      537 2023-05-30 00:27:00.000000 chatgptonic-1.1.3/chatgptonic.egg-info/PKG-INFO
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      277 2023-05-30 00:27:00.000000 chatgptonic-1.1.3/chatgptonic.egg-info/SOURCES.txt
+-rw-r--r--   0 howardmederiros   (501) staff       (20)        1 2023-05-30 00:27:00.000000 chatgptonic-1.1.3/chatgptonic.egg-info/dependency_links.txt
+-rw-r--r--   0 howardmederiros   (501) staff       (20)        1 2023-03-13 16:03:25.000000 chatgptonic-1.1.3/chatgptonic.egg-info/not-zip-safe
+-rw-r--r--   0 howardmederiros   (501) staff       (20)       88 2023-05-30 00:27:00.000000 chatgptonic-1.1.3/chatgptonic.egg-info/requires.txt
+-rw-r--r--   0 howardmederiros   (501) staff       (20)       12 2023-05-30 00:27:00.000000 chatgptonic-1.1.3/chatgptonic.egg-info/top_level.txt
+-rw-r--r--   0 howardmederiros   (501) staff       (20)       38 2023-05-30 00:27:00.811248 chatgptonic-1.1.3/setup.cfg
+-rw-r--r--   0 howardmederiros   (501) staff       (20)      949 2023-05-30 00:26:55.000000 chatgptonic-1.1.3/setup.py
```

### Comparing `chatgptonic-1.1.2/PKG-INFO` & `chatgptonic-1.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgptonic
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package to facilitate integration with chatgpt
 Home-page: https://github.com/how-dev/chatgpython
 Author: Howard Medeiros (howard.medeiros@gmail.com)
 License: UNKNOWN
 Keywords: chatgptonic
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatgptonic-1.1.2/chatgptonic/integration.py` & `chatgptonic-1.1.3/chatgptonic/integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 class ChatGPTMessageException(Exception):
     pass
 
 
 class ChatGPT:
     def __init__(
-        self, api_key: str, chat_model: str = "gpt-3.5-turbo", role: str = "user"
+        self, api_key: str, chat_model: str = "gpt-3.5-turbo", role: str = "user", chat_url: str = "https://api.openai.com/v1/chat/completions"
     ):
         self.api_key: str = api_key
 
         self.chat_model: str = chat_model
         self.role: str = role
-        self.chat_url: str = "https://api.openai.com/v1/chat/completions"
+        self.chat_url: str = chat_url
 
     def _get_headers(self) -> dict:
         return {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}",
         }
```

### Comparing `chatgptonic-1.1.2/chatgptonic.egg-info/PKG-INFO` & `chatgptonic-1.1.3/chatgptonic.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgptonic
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package to facilitate integration with chatgpt
 Home-page: https://github.com/how-dev/chatgpython
 Author: Howard Medeiros (howard.medeiros@gmail.com)
 License: UNKNOWN
 Keywords: chatgptonic
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatgptonic-1.1.2/setup.py` & `chatgptonic-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,10 +23,10 @@
     ],
     include_package_data=True,
     keywords='chatgptonic',
     name='chatgptonic',
     packages=find_packages(include=['chatgptonic', 'chatgptonic.*']),
     test_suite='tests',
     url='https://github.com/how-dev/chatgpython',
-    version='1.1.2',
+    version='1.1.3',
     zip_safe=False,
 )
```

