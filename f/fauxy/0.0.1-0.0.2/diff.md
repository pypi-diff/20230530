# Comparing `tmp/fauxy-0.0.1.tar.gz` & `tmp/fauxy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fauxy-0.0.1.tar", max compression
+gzip compressed data, was "fauxy-0.0.2.tar", max compression
```

## Comparing `fauxy-0.0.1.tar` & `fauxy-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2414 2023-05-30 11:09:54.375169 fauxy-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-29 17:24:04.586514 fauxy-0.0.1/fauxy/__init__.py
--rw-r--r--   0        0        0     2457 2023-05-30 10:30:38.822741 fauxy-0.0.1/fauxy/app.py
--rw-r--r--   0        0        0     2123 2023-05-30 10:31:24.669237 fauxy-0.0.1/fauxy/library.py
--rw-r--r--   0        0        0     4208 2023-05-29 17:24:58.210842 fauxy-0.0.1/fauxy/record.py
--rw-r--r--   0        0        0      426 2023-05-29 10:39:39.176834 fauxy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 fauxy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2697 2023-05-30 13:47:04.695510 fauxy-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 17:24:04.586514 fauxy-0.0.2/fauxy/__init__.py
+-rw-r--r--   0        0        0     2457 2023-05-30 10:30:38.822741 fauxy-0.0.2/fauxy/app.py
+-rw-r--r--   0        0        0     2123 2023-05-30 10:31:24.669237 fauxy-0.0.2/fauxy/library.py
+-rw-r--r--   0        0        0     4208 2023-05-29 17:24:58.210842 fauxy-0.0.2/fauxy/record.py
+-rw-r--r--   0        0        0      473 2023-05-30 13:48:25.053036 fauxy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3364 1970-01-01 00:00:00.000000 fauxy-0.0.2/PKG-INFO
```

### Comparing `fauxy-0.0.1/README.md` & `fauxy-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Fauxy is an ASGI webapp that will proxy requests to a remote server.
 The first time it sees a request, it records the response to disk and returns it.
 From then on, it can return the recorded response whenever it sees the same request.
 
 # Running
 Fauxy can be run by any ASGI server.
-[example.py](example.py) runs fauxy using [uvicorn](https://www.uvicorn.org/).
+[example.py](https://github.com/groves/fauxy/blob/main/example.py) runs fauxy using [uvicorn](https://www.uvicorn.org/).
 If you've installed fauxy, you can run it with `python example.py`.
 
 # Matching requests
 To decide if a given request matches any recordings, fauxy creates a 'key' for the request.
 It takes a `key_maker` function to do this.
 The key maker function takes in a Starlette Request object and returns a JSON key.
 Any request that produces identical JSON will be considered a match by fauxy.
@@ -35,7 +35,14 @@
 For our /1/2/3 example, if the library directory is `recordings`, fauxy could produce the directory `recordings/1/2/3/ba8d9c9d`.
 In that example, `ba8d9c9d` is the hash of the key JSON bytes.
 When looking for a recording matching a request, fauxy produces the hash, walks the library directory, and returns the first matching hash directory it finds.
 
 While the request path is part of the created directory structure, it doesn't constrain matching.
 As long as the hash matches, fauxy will return a response.
 If you include the requested path in the key JSON, the hash will be determined by the path, but if you don't, it won't affect it.
+
+# Todo
+* Processing responses before saving
+* Optionally record requests
+* TUI for viewing requests and responses
+* Hosting multiple reloading proxies on separate ports from a single parent
+* Content-adressed response content deduplication
```

### Comparing `fauxy-0.0.1/fauxy/app.py` & `fauxy-0.0.2/fauxy/app.py`

 * *Files identical despite different names*

### Comparing `fauxy-0.0.1/fauxy/library.py` & `fauxy-0.0.2/fauxy/library.py`

 * *Files identical despite different names*

### Comparing `fauxy-0.0.1/fauxy/record.py` & `fauxy-0.0.2/fauxy/record.py`

 * *Files identical despite different names*

### Comparing `fauxy-0.0.1/PKG-INFO` & `fauxy-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: fauxy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Faux responses from proxying
+Home-page: https://github.com/groves/fauxy
 License: Apache-2.0
 Author: Charlie Groves
 Author-email: c@sevorg.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: starlette (>=0.26.1,<0.27.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
+Project-URL: Repository, https://github.com/groves/fauxy
 Description-Content-Type: text/markdown
 
 Fauxy is an ASGI webapp that will proxy requests to a remote server.
 The first time it sees a request, it records the response to disk and returns it.
 From then on, it can return the recorded response whenever it sees the same request.
 
 # Running
 Fauxy can be run by any ASGI server.
-[example.py](example.py) runs fauxy using [uvicorn](https://www.uvicorn.org/).
+[example.py](https://github.com/groves/fauxy/blob/main/example.py) runs fauxy using [uvicorn](https://www.uvicorn.org/).
 If you've installed fauxy, you can run it with `python example.py`.
 
 # Matching requests
 To decide if a given request matches any recordings, fauxy creates a 'key' for the request.
 It takes a `key_maker` function to do this.
 The key maker function takes in a Starlette Request object and returns a JSON key.
 Any request that produces identical JSON will be considered a match by fauxy.
@@ -53,7 +55,14 @@
 In that example, `ba8d9c9d` is the hash of the key JSON bytes.
 When looking for a recording matching a request, fauxy produces the hash, walks the library directory, and returns the first matching hash directory it finds.
 
 While the request path is part of the created directory structure, it doesn't constrain matching.
 As long as the hash matches, fauxy will return a response.
 If you include the requested path in the key JSON, the hash will be determined by the path, but if you don't, it won't affect it.
 
+# Todo
+* Processing responses before saving
+* Optionally record requests
+* TUI for viewing requests and responses
+* Hosting multiple reloading proxies on separate ports from a single parent
+* Content-adressed response content deduplication
+
```

