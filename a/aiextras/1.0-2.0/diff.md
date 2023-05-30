# Comparing `tmp/aiextras-1.0.tar.gz` & `tmp/aiextras-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aiextras-1.0.tar", last modified: Mon May 22 04:55:55 2023, max compression
+gzip compressed data, was "dist\aiextras-2.0.tar", last modified: Tue May 30 02:22:58 2023, max compression
```

## Comparing `aiextras-1.0.tar` & `aiextras-2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 04:55:55.000000 aiextras-1.0/
--rw-rw-rw-   0        0        0        0 2023-05-22 03:45:14.000000 aiextras-1.0/LICENSE
--rw-rw-rw-   0        0        0      336 2023-05-22 04:55:55.000000 aiextras-1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-20 09:12:45.000000 aiextras-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 04:55:55.000000 aiextras-1.0/aiextras/
-drwxrwxrwx   0        0        0        0 2023-05-22 04:55:55.000000 aiextras-1.0/aiextras/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 04:55:55.000000 aiextras-1.0/aiextras/src/aiextras.egg-info/
--rw-rw-rw-   0        0        0      336 2023-05-22 04:55:55.000000 aiextras-1.0/aiextras/src/aiextras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-05-22 04:55:55.000000 aiextras-1.0/aiextras/src/aiextras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 04:55:55.000000 aiextras-1.0/aiextras/src/aiextras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 04:55:55.000000 aiextras-1.0/aiextras/src/aiextras.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    25007 2023-05-22 04:55:22.000000 aiextras-1.0/aiextras/src/aiextras.py
--rw-rw-rw-   0        0        0       86 2023-05-22 04:55:55.000000 aiextras-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1204 2023-05-22 04:55:49.000000 aiextras-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:22:58.000000 aiextras-2.0/
+-rw-rw-rw-   0        0        0        0 2023-05-22 03:45:14.000000 aiextras-2.0/LICENSE
+-rw-rw-rw-   0        0        0      336 2023-05-30 02:22:58.000000 aiextras-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-20 09:12:45.000000 aiextras-2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 02:22:58.000000 aiextras-2.0/aiextras/
+drwxrwxrwx   0        0        0        0 2023-05-30 02:22:58.000000 aiextras-2.0/aiextras/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 02:22:58.000000 aiextras-2.0/aiextras/src/aiextras.egg-info/
+-rw-rw-rw-   0        0        0      336 2023-05-30 02:22:58.000000 aiextras-2.0/aiextras/src/aiextras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-05-30 02:22:58.000000 aiextras-2.0/aiextras/src/aiextras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 02:22:58.000000 aiextras-2.0/aiextras/src/aiextras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 02:22:58.000000 aiextras-2.0/aiextras/src/aiextras.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    25007 2023-05-22 04:55:22.000000 aiextras-2.0/aiextras/src/aiextras.py
+-rw-rw-rw-   0        0        0       86 2023-05-30 02:22:58.000000 aiextras-2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1204 2023-05-30 02:22:47.000000 aiextras-2.0/setup.py
```

### Comparing `aiextras-1.0/aiextras/src/aiextras.py` & `aiextras-2.0/aiextras/src/aiextras.py`

 * *Files identical despite different names*

### Comparing `aiextras-1.0/setup.py` & `aiextras-2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiextras",                     # This is the name of the package
-    version="1.0",                        # The initial release version
+    version="2.0",                        # The initial release version
     author="AnupamKris",                     # Full name of the author
     description="AI2LAB Programs",
     # Long description read from the the readme file
     long_description=long_description,
     long_description_content_type="text/markdown",
     # List of all python modules to be installed
     packages=setuptools.find_packages(),
```

