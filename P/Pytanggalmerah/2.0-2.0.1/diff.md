# Comparing `tmp/Pytanggalmerah-2.0.tar.gz` & `tmp/Pytanggalmerah-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pytanggalmerah-2.0.tar", last modified: Thu Mar 24 16:33:57 2022, max compression
+gzip compressed data, was "Pytanggalmerah-2.0.1.tar", last modified: Fri Mar 25 03:08:48 2022, max compression
```

## Comparing `Pytanggalmerah-2.0.tar` & `Pytanggalmerah-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-24 16:33:57.940349 Pytanggalmerah-2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2022-03-24 16:33:47.000000 Pytanggalmerah-2.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1861 2022-03-24 16:33:57.939432 Pytanggalmerah-2.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-24 16:33:57.938516 Pytanggalmerah-2.0/Pytanggalmerah.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1861 2022-03-24 16:33:57.000000 Pytanggalmerah-2.0/Pytanggalmerah.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      348 2022-03-24 16:33:57.000000 Pytanggalmerah-2.0/Pytanggalmerah.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-24 16:33:57.000000 Pytanggalmerah-2.0/Pytanggalmerah.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-03-24 16:33:57.000000 Pytanggalmerah-2.0/Pytanggalmerah.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2022-03-24 16:33:57.000000 Pytanggalmerah-2.0/Pytanggalmerah.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1488 2022-03-24 16:33:47.000000 Pytanggalmerah-2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      495 2022-03-24 16:33:47.000000 Pytanggalmerah-2.0/harilibur
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-24 16:33:57.939432 Pytanggalmerah-2.0/pytanggalmerah/
--rw-rw-rw-   0 root         (0) root         (0)     1545 2022-03-24 16:33:57.000000 Pytanggalmerah-2.0/pytanggalmerah/TanggalMerah.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-03-24 16:33:57.000000 Pytanggalmerah-2.0/pytanggalmerah/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2022-03-24 16:33:57.000000 Pytanggalmerah-2.0/pytanggalmerah/myrequests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-24 16:33:57.939432 Pytanggalmerah-2.0/pytanggalmerahcache/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-24 16:33:47.000000 Pytanggalmerah-2.0/pytanggalmerahcache/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-24 16:33:57.940349 Pytanggalmerah-2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      827 2022-03-24 16:33:57.000000 Pytanggalmerah-2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 03:08:48.627195 Pytanggalmerah-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2022-03-25 03:08:38.000000 Pytanggalmerah-2.0.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1863 2022-03-25 03:08:48.627195 Pytanggalmerah-2.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 03:08:48.625194 Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1863 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      348 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2022-03-25 03:08:38.000000 Pytanggalmerah-2.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      495 2022-03-25 03:08:38.000000 Pytanggalmerah-2.0.1/harilibur
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 03:08:48.626195 Pytanggalmerah-2.0.1/pytanggalmerah/
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/pytanggalmerah/TanggalMerah.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/pytanggalmerah/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2022-03-25 03:08:47.000000 Pytanggalmerah-2.0.1/pytanggalmerah/myrequests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 03:08:48.627195 Pytanggalmerah-2.0.1/pytanggalmerahcache/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-25 03:08:38.000000 Pytanggalmerah-2.0.1/pytanggalmerahcache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2022-03-25 03:08:48.627195 Pytanggalmerah-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      829 2022-03-25 03:08:47.000000 Pytanggalmerah-2.0.1/setup.py
```

### Comparing `Pytanggalmerah-2.0/LICENSE.txt` & `Pytanggalmerah-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Pytanggalmerah-2.0/PKG-INFO` & `Pytanggalmerah-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytanggalmerah
-Version: 2.0
+Version: 2.0.1
 Summary: python module to check indonesia holiday calendar (include sunday)
 Home-page: https://github.com/guangrei/pytanggalmerah
 Author: guangrei
 Author-email: myawn@pm.me
 License: MIT
 Keywords: holiday indonesia calendar sunday
 Platform: UNKNOWN
```

### Comparing `Pytanggalmerah-2.0/Pytanggalmerah.egg-info/PKG-INFO` & `Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytanggalmerah
-Version: 2.0
+Version: 2.0.1
 Summary: python module to check indonesia holiday calendar (include sunday)
 Home-page: https://github.com/guangrei/pytanggalmerah
 Author: guangrei
 Author-email: myawn@pm.me
 License: MIT
 Keywords: holiday indonesia calendar sunday
 Platform: UNKNOWN
```

### Comparing `Pytanggalmerah-2.0/README.md` & `Pytanggalmerah-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Pytanggalmerah-2.0/pytanggalmerah/TanggalMerah.py` & `Pytanggalmerah-2.0.1/pytanggalmerah/TanggalMerah.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import json
 
 
 class TanggalMerah:
     def __init__(self, cache_path=None, cache_time=600):
         self.event = set([])
         self.date = datetime.now(timezone("Asia/Jakarta"))
-        req = MyRequests("https://github.com/guangrei/Json-Indonesia-holidays/raw/master/calendar.json",
+        req = MyRequests("https://github.com/guangrei/Json-Indonesia-holidays/raw/master/calendar.min.json",
                          cache_path=cache_path, cache_time=cache_time)
         self.data = json.loads(req.response)
 
     # end __init_()
 
     def set_timezone(self, tz):
         self.date = datetime.now(timezone(tz))
```

### Comparing `Pytanggalmerah-2.0/pytanggalmerah/myrequests.py` & `Pytanggalmerah-2.0.1/pytanggalmerah/myrequests.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,11 +27,11 @@
             else:
                 self.response = cache.get(u_en+"_offline")
                 self.is_loaded_from_cache = True
 
     def makeRequest(self, url):
 
         try:
-            req = requests.get(url, verify=False)
+            req = requests.get(url)
             return req.text
         except:
             return False
```

### Comparing `Pytanggalmerah-2.0/setup.py` & `Pytanggalmerah-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='Pytanggalmerah',
-    version='2.0',
+    version='2.0.1',
     packages=['pytanggalmerah', 'pytanggalmerahcache'],
     scripts=["harilibur"],
     license='MIT',
     author="guangrei",
     author_email="myawn@pm.me",
     description="python module to check indonesia holiday calendar (include sunday)",
     long_description=long_description,
```

