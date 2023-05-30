# Comparing `tmp/methodism-0.1.0.tar.gz` & `tmp/methodism-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodism-0.1.0.tar", last modified: Tue May 30 07:16:33 2023, max compression
+gzip compressed data, was "methodism-0.1.1.tar", last modified: Tue May 30 07:22:00 2023, max compression
```

## Comparing `methodism-0.1.0.tar` & `methodism-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 07:16:33.296627 methodism-0.1.0/
--rw-rw-rw-   0        0        0     3953 2023-05-30 07:16:33.296627 methodism-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3471 2023-05-30 06:58:48.000000 methodism-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 07:16:33.281012 methodism-0.1.0/methodism/
--rw-rw-rw-   0        0        0      399 2023-05-29 07:36:13.000000 methodism-0.1.0/methodism/__init__.py
--rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.1.0/methodism/costumizing.py
--rw-rw-rw-   0        0        0      856 2023-05-30 07:16:02.000000 methodism-0.1.0/methodism/decors.py
--rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.1.0/methodism/error_messages.py
--rw-rw-rw-   0        0        0     2192 2023-05-29 07:11:47.000000 methodism-0.1.0/methodism/helper.py
--rw-rw-rw-   0        0        0     6883 2023-05-30 06:51:39.000000 methodism-0.1.0/methodism/main.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:16:33.296627 methodism-0.1.0/methodism.egg-info/
--rw-rw-rw-   0        0        0     3953 2023-05-30 07:16:33.000000 methodism-0.1.0/methodism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-30 07:16:33.000000 methodism-0.1.0/methodism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 07:16:33.000000 methodism-0.1.0/methodism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 07:16:33.000000 methodism-0.1.0/methodism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      603 2023-05-30 06:43:18.000000 methodism-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      546 2023-05-30 07:16:33.296627 methodism-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 07:22:00.647364 methodism-0.1.1/
+-rw-rw-rw-   0        0        0     3953 2023-05-30 07:22:00.647364 methodism-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3471 2023-05-30 06:58:48.000000 methodism-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 07:22:00.629334 methodism-0.1.1/methodism/
+-rw-rw-rw-   0        0        0      449 2023-05-30 07:21:18.000000 methodism-0.1.1/methodism/__init__.py
+-rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.1.1/methodism/costumizing.py
+-rw-rw-rw-   0        0        0      856 2023-05-30 07:16:02.000000 methodism-0.1.1/methodism/decors.py
+-rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.1.1/methodism/error_messages.py
+-rw-rw-rw-   0        0        0     2192 2023-05-29 07:11:47.000000 methodism-0.1.1/methodism/helper.py
+-rw-rw-rw-   0        0        0     6883 2023-05-30 06:51:39.000000 methodism-0.1.1/methodism/main.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:22:00.645367 methodism-0.1.1/methodism.egg-info/
+-rw-rw-rw-   0        0        0     3953 2023-05-30 07:22:00.000000 methodism-0.1.1/methodism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-30 07:22:00.000000 methodism-0.1.1/methodism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 07:22:00.000000 methodism-0.1.1/methodism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 07:22:00.000000 methodism-0.1.1/methodism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      604 2023-05-30 07:21:31.000000 methodism-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      546 2023-05-30 07:22:00.654885 methodism-0.1.1/setup.cfg
```

### Comparing `methodism-0.1.0/PKG-INFO` & `methodism-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.1.0
+Version: 0.1.1
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `methodism-0.1.0/README.md` & `methodism-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `methodism-0.1.0/methodism/costumizing.py` & `methodism-0.1.1/methodism/costumizing.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.0/methodism/decors.py` & `methodism-0.1.1/methodism/decors.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.0/methodism/error_messages.py` & `methodism-0.1.1/methodism/error_messages.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.0/methodism/helper.py` & `methodism-0.1.1/methodism/helper.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.0/methodism/main.py` & `methodism-0.1.1/methodism/main.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.0/methodism.egg-info/PKG-INFO` & `methodism-0.1.1/methodism.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.1.0
+Version: 0.1.1
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `methodism-0.1.0/pyproject.toml` & `methodism-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "djangorestframework>=3.14.0",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "methodism"
-version = "0.1.0"
+version = "0.1.01"
 authors = [
   { name="xudikk", email="xudikk.1@gmail.com" },
 ]
 description = "Help to build APIs Faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `methodism-0.1.0/setup.cfg` & `methodism-0.1.1/setup.cfg`

 * *Files identical despite different names*

