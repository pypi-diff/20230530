# Comparing `tmp/ezmail-0.1.0.tar.gz` & `tmp/ezmail-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezmail-0.1.0.tar", last modified: Tue May 30 04:44:55 2023, max compression
+gzip compressed data, was "ezmail-0.1.1.tar", last modified: Tue May 30 04:47:07 2023, max compression
```

## Comparing `ezmail-0.1.0.tar` & `ezmail-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 04:44:55.673949 ezmail-0.1.0/
--rw-r--r--   0 alex       (501) staff       (20)    35149 2023-05-30 04:28:26.000000 ezmail-0.1.0/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)      491 2023-05-30 04:44:55.673601 ezmail-0.1.0/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)       41 2023-05-30 04:28:26.000000 ezmail-0.1.0/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 04:44:55.665744 ezmail-0.1.0/ezmail/
--rw-r--r--   0 alex       (501) staff       (20)       29 2023-05-30 04:23:23.000000 ezmail-0.1.0/ezmail/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     4231 2023-05-30 04:43:32.000000 ezmail-0.1.0/ezmail/ezmail.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 04:44:55.672859 ezmail-0.1.0/ezmail.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      491 2023-05-30 04:44:55.000000 ezmail-0.1.0/ezmail.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      211 2023-05-30 04:44:55.000000 ezmail-0.1.0/ezmail.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-05-30 04:44:55.000000 ezmail-0.1.0/ezmail.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       14 2023-05-30 04:44:55.000000 ezmail-0.1.0/ezmail.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)        7 2023-05-30 04:44:55.000000 ezmail-0.1.0/ezmail.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-05-30 04:44:55.674068 ezmail-0.1.0/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      735 2023-05-30 04:37:31.000000 ezmail-0.1.0/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 04:47:07.637692 ezmail-0.1.1/
+-rw-r--r--   0 alex       (501) staff       (20)    35149 2023-05-30 04:28:26.000000 ezmail-0.1.1/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)      491 2023-05-30 04:47:07.637091 ezmail-0.1.1/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)       41 2023-05-30 04:28:26.000000 ezmail-0.1.1/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 04:47:07.628706 ezmail-0.1.1/ezmail/
+-rw-r--r--   0 alex       (501) staff       (20)       30 2023-05-30 04:46:48.000000 ezmail-0.1.1/ezmail/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     4231 2023-05-30 04:43:32.000000 ezmail-0.1.1/ezmail/ezmail.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 04:47:07.636257 ezmail-0.1.1/ezmail.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      491 2023-05-30 04:47:07.000000 ezmail-0.1.1/ezmail.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      211 2023-05-30 04:47:07.000000 ezmail-0.1.1/ezmail.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-05-30 04:47:07.000000 ezmail-0.1.1/ezmail.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       14 2023-05-30 04:47:07.000000 ezmail-0.1.1/ezmail.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)        7 2023-05-30 04:47:07.000000 ezmail-0.1.1/ezmail.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-05-30 04:47:07.637830 ezmail-0.1.1/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      735 2023-05-30 04:47:01.000000 ezmail-0.1.1/setup.py
```

### Comparing `ezmail-0.1.0/LICENSE` & `ezmail-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezmail-0.1.0/ezmail/ezmail.py` & `ezmail-0.1.1/ezmail/ezmail.py`

 * *Files identical despite different names*

### Comparing `ezmail-0.1.0/setup.py` & `ezmail-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ezmail",
-    version="0.1.0",
+    version="0.1.1",
     author="Alex Rodriguez",
     author_email="alex.rodriguez.oro@gmail.com",
     description="easily send out emails via SMTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Alex23rodriguez/ezmail",
     packages=setuptools.find_packages(),
```

