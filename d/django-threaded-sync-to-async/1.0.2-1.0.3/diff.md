# Comparing `tmp/django_threaded_sync_to_async-1.0.2.tar.gz` & `tmp/django_threaded_sync_to_async-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_threaded_sync_to_async-1.0.2.tar", last modified: Sun May 28 19:02:24 2023, max compression
+gzip compressed data, was "django_threaded_sync_to_async-1.0.3.tar", last modified: Tue May 30 08:04:25 2023, max compression
```

## Comparing `django_threaded_sync_to_async-1.0.2.tar` & `django_threaded_sync_to_async-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-28 19:02:24.485360 django_threaded_sync_to_async-1.0.2/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1063 2023-05-26 19:21:14.000000 django_threaded_sync_to_async-1.0.2/LICENSE.md
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2656 2023-05-28 19:02:24.485360 django_threaded_sync_to_async-1.0.2/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1250 2023-05-28 09:23:45.000000 django_threaded_sync_to_async-1.0.2/README.md
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-28 19:02:24.485360 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2380 2023-05-28 18:27:08.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2294 2023-05-28 15:11:49.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async/patch.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-28 19:02:24.485360 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2656 2023-05-28 19:02:24.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      389 2023-05-28 19:02:24.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/SOURCES.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-05-28 19:02:24.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/dependency_links.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        8 2023-05-28 19:02:24.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/requires.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       30 2023-05-28 19:02:24.000000 django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/top_level.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       31 2023-05-27 15:17:43.000000 django_threaded_sync_to_async-1.0.2/pyproject.toml
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-05-28 19:02:24.485360 django_threaded_sync_to_async-1.0.2/setup.cfg
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2121 2023-05-28 19:01:38.000000 django_threaded_sync_to_async-1.0.2/setup.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-30 08:04:25.005100 django_threaded_sync_to_async-1.0.3/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1063 2023-05-26 19:21:14.000000 django_threaded_sync_to_async-1.0.3/LICENSE.md
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2656 2023-05-30 08:04:25.005100 django_threaded_sync_to_async-1.0.3/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1250 2023-05-28 09:23:45.000000 django_threaded_sync_to_async-1.0.3/README.md
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-30 08:04:25.005100 django_threaded_sync_to_async-1.0.3/django_threaded_sync_to_async/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2548 2023-05-30 08:02:36.000000 django_threaded_sync_to_async-1.0.3/django_threaded_sync_to_async/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2294 2023-05-30 08:01:17.000000 django_threaded_sync_to_async-1.0.3/django_threaded_sync_to_async/patch.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-30 08:04:25.005100 django_threaded_sync_to_async-1.0.3/django_threaded_sync_to_async.egg-info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2656 2023-05-30 08:04:24.000000 django_threaded_sync_to_async-1.0.3/django_threaded_sync_to_async.egg-info/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      389 2023-05-30 08:04:24.000000 django_threaded_sync_to_async-1.0.3/django_threaded_sync_to_async.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-05-30 08:04:24.000000 django_threaded_sync_to_async-1.0.3/django_threaded_sync_to_async.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        8 2023-05-30 08:04:24.000000 django_threaded_sync_to_async-1.0.3/django_threaded_sync_to_async.egg-info/requires.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       30 2023-05-30 08:04:24.000000 django_threaded_sync_to_async-1.0.3/django_threaded_sync_to_async.egg-info/top_level.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       69 2023-05-30 06:17:44.000000 django_threaded_sync_to_async-1.0.3/pyproject.toml
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-05-30 08:04:25.005100 django_threaded_sync_to_async-1.0.3/setup.cfg
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2122 2023-05-30 08:03:22.000000 django_threaded_sync_to_async-1.0.3/setup.py
```

### Comparing `django_threaded_sync_to_async-1.0.2/LICENSE.md` & `django_threaded_sync_to_async-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_threaded_sync_to_async-1.0.2/PKG-INFO` & `django_threaded_sync_to_async-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_threaded_sync_to_async
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=False, executor=...)`, effectively allowing Django to make calls to database concurrently
 Home-page: https://github.com/excitoon/django_threaded_sync_to_async
 Author: Vladimir Chebotarev
 Author-email: vladimir.chebotarev@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/excitoon/django_threaded_sync_to_async/blob/master/README.md
 Project-URL: Source, https://github.com/excitoon/django_threaded_sync_to_async
```

### Comparing `django_threaded_sync_to_async-1.0.2/README.md` & `django_threaded_sync_to_async-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async/patch.py` & `django_threaded_sync_to_async-1.0.3/django_threaded_sync_to_async/patch.py`

 * *Files identical despite different names*

### Comparing `django_threaded_sync_to_async-1.0.2/django_threaded_sync_to_async.egg-info/PKG-INFO` & `django_threaded_sync_to_async-1.0.3/django_threaded_sync_to_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-threaded-sync-to-async
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=False, executor=...)`, effectively allowing Django to make calls to database concurrently
 Home-page: https://github.com/excitoon/django_threaded_sync_to_async
 Author: Vladimir Chebotarev
 Author-email: vladimir.chebotarev@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/excitoon/django_threaded_sync_to_async/blob/master/README.md
 Project-URL: Source, https://github.com/excitoon/django_threaded_sync_to_async
```

### Comparing `django_threaded_sync_to_async-1.0.2/setup.py` & `django_threaded_sync_to_async-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Setup script."""
 
 import os
+
 import setuptools
 
 
 with open(f"{os.path.dirname(os.path.abspath(__file__))}/requirements.txt") as requirements:
     with open(f"{os.path.dirname(os.path.abspath(__file__))}/README.md") as readme:
         setuptools.setup(
             name="django_threaded_sync_to_async",
-            version="1.0.2",
+            version="1.0.3",
             description="Tools for replacing `sync_to_async` calls to `sync_to_async(thread_sensitive=False, executor=...)`, effectively allowing Django to make calls to database concurrently",
             long_description=readme.read(),
             long_description_content_type="text/markdown",
             author="Vladimir Chebotarev",
             author_email="vladimir.chebotarev@gmail.com",
             license="MIT",
             classifiers=[
```

