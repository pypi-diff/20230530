# Comparing `tmp/ezmail-0.2.0.tar.gz` & `tmp/ezmail-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezmail-0.2.0.tar", last modified: Tue May 30 04:56:18 2023, max compression
+gzip compressed data, was "ezmail-1.0.0.tar", last modified: Tue May 30 20:20:03 2023, max compression
```

## Comparing `ezmail-0.2.0.tar` & `ezmail-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 04:56:18.599642 ezmail-0.2.0/
--rw-r--r--   0 alex       (501) staff       (20)    35149 2023-05-30 04:28:26.000000 ezmail-0.2.0/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)      491 2023-05-30 04:56:18.599171 ezmail-0.2.0/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)       41 2023-05-30 04:28:26.000000 ezmail-0.2.0/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 04:56:18.596202 ezmail-0.2.0/ezmail/
--rw-r--r--   0 alex       (501) staff       (20)       30 2023-05-30 04:46:48.000000 ezmail-0.2.0/ezmail/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1107 2023-05-30 04:54:44.000000 ezmail-0.2.0/ezmail/__main__.py
--rw-r--r--   0 alex       (501) staff       (20)     4231 2023-05-30 04:43:32.000000 ezmail-0.2.0/ezmail/ezmail.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 04:56:18.598681 ezmail-0.2.0/ezmail.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      491 2023-05-30 04:56:18.000000 ezmail-0.2.0/ezmail.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      230 2023-05-30 04:56:18.000000 ezmail-0.2.0/ezmail.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-05-30 04:56:18.000000 ezmail-0.2.0/ezmail.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       14 2023-05-30 04:56:18.000000 ezmail-0.2.0/ezmail.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)        7 2023-05-30 04:56:18.000000 ezmail-0.2.0/ezmail.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-05-30 04:56:18.599857 ezmail-0.2.0/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      735 2023-05-30 04:55:41.000000 ezmail-0.2.0/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 20:20:03.104018 ezmail-1.0.0/
+-rw-r--r--   0 alex       (501) staff       (20)    35149 2023-05-30 04:28:26.000000 ezmail-1.0.0/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)     3831 2023-05-30 20:20:03.103546 ezmail-1.0.0/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     3381 2023-05-30 20:18:56.000000 ezmail-1.0.0/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 20:20:03.098398 ezmail-1.0.0/ezmail/
+-rw-r--r--   0 alex       (501) staff       (20)       30 2023-05-30 04:46:48.000000 ezmail-1.0.0/ezmail/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1107 2023-05-30 04:54:44.000000 ezmail-1.0.0/ezmail/__main__.py
+-rw-r--r--   0 alex       (501) staff       (20)     4231 2023-05-30 04:43:32.000000 ezmail-1.0.0/ezmail/ezmail.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 20:20:03.102588 ezmail-1.0.0/ezmail.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     3831 2023-05-30 20:20:02.000000 ezmail-1.0.0/ezmail.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      230 2023-05-30 20:20:03.000000 ezmail-1.0.0/ezmail.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-05-30 20:20:02.000000 ezmail-1.0.0/ezmail.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       14 2023-05-30 20:20:02.000000 ezmail-1.0.0/ezmail.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)        7 2023-05-30 20:20:02.000000 ezmail-1.0.0/ezmail.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-05-30 20:20:03.104201 ezmail-1.0.0/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      735 2023-05-30 20:19:33.000000 ezmail-1.0.0/setup.py
```

### Comparing `ezmail-0.2.0/LICENSE` & `ezmail-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezmail-0.2.0/ezmail/__main__.py` & `ezmail-1.0.0/ezmail/__main__.py`

 * *Files identical despite different names*

### Comparing `ezmail-0.2.0/ezmail/ezmail.py` & `ezmail-1.0.0/ezmail/ezmail.py`

 * *Files identical despite different names*

### Comparing `ezmail-0.2.0/setup.py` & `ezmail-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ezmail",
-    version="0.2.0",
+    version="1.0.0",
     author="Alex Rodriguez",
     author_email="alex.rodriguez.oro@gmail.com",
     description="easily send out emails via SMTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Alex23rodriguez/ezmail",
     packages=setuptools.find_packages(),
```

