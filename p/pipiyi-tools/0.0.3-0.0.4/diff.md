# Comparing `tmp/pipiyi_tools-0.0.3.tar.gz` & `tmp/pipiyi_tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pipiyi_tools-0.0.3.tar", last modified: Tue May 30 09:29:52 2023, max compression
+gzip compressed data, was "dist/pipiyi_tools-0.0.4.tar", last modified: Tue May 30 09:42:36 2023, max compression
```

## Comparing `pipiyi_tools-0.0.3.tar` & `pipiyi_tools-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-05-30 09:29:52.000000 pipiyi_tools-0.0.3/
--rw-r--r--   0 xiaopipi   (501) staff       (20)      918 2023-05-30 09:29:52.000000 pipiyi_tools-0.0.3/PKG-INFO
--rw-r--r--   0 xiaopipi   (501) staff       (20)      288 2023-05-30 08:07:51.000000 pipiyi_tools-0.0.3/README.md
-drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-05-30 09:29:52.000000 pipiyi_tools-0.0.3/pipiyi-tools/
--rw-r--r--   0 xiaopipi   (501) staff       (20)     2589 2023-05-23 08:46:36.000000 pipiyi_tools-0.0.3/pipiyi-tools/EpubSpliter.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1058 2023-05-25 05:43:31.000000 pipiyi_tools-0.0.3/pipiyi-tools/FileOperation.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1134 2023-05-26 09:22:54.000000 pipiyi_tools-0.0.3/pipiyi-tools/ListQueue.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1928 2023-05-26 09:49:22.000000 pipiyi_tools-0.0.3/pipiyi-tools/Log.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     2070 2023-05-23 06:29:36.000000 pipiyi_tools-0.0.3/pipiyi-tools/MyRequest.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     6711 2023-05-28 14:14:08.000000 pipiyi_tools-0.0.3/pipiyi-tools/PooledBase.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)      972 2023-05-23 04:18:08.000000 pipiyi_tools-0.0.3/pipiyi-tools/Storage.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)       19 2023-05-30 09:29:39.000000 pipiyi_tools-0.0.3/pipiyi-tools/__init__.py
-drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-05-30 09:29:52.000000 pipiyi_tools-0.0.3/pipiyi_tools.egg-info/
--rw-r--r--   0 xiaopipi   (501) staff       (20)      918 2023-05-30 09:29:52.000000 pipiyi_tools-0.0.3/pipiyi_tools.egg-info/PKG-INFO
--rw-r--r--   0 xiaopipi   (501) staff       (20)      403 2023-05-30 09:29:52.000000 pipiyi_tools-0.0.3/pipiyi_tools.egg-info/SOURCES.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)        1 2023-05-30 09:29:52.000000 pipiyi_tools-0.0.3/pipiyi_tools.egg-info/dependency_links.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)       43 2023-05-30 09:29:52.000000 pipiyi_tools-0.0.3/pipiyi_tools.egg-info/requires.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)       13 2023-05-30 09:29:52.000000 pipiyi_tools-0.0.3/pipiyi_tools.egg-info/top_level.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)       38 2023-05-30 09:29:52.000000 pipiyi_tools-0.0.3/setup.cfg
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1003 2023-05-30 09:29:45.000000 pipiyi_tools-0.0.3/setup.py
+drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-05-30 09:42:36.000000 pipiyi_tools-0.0.4/
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      918 2023-05-30 09:42:36.000000 pipiyi_tools-0.0.4/PKG-INFO
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      288 2023-05-30 08:07:51.000000 pipiyi_tools-0.0.4/README.md
+drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-05-30 09:42:36.000000 pipiyi_tools-0.0.4/pipiyi-tools/
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     2589 2023-05-23 08:46:36.000000 pipiyi_tools-0.0.4/pipiyi-tools/EpubSpliter.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1058 2023-05-25 05:43:31.000000 pipiyi_tools-0.0.4/pipiyi-tools/FileOperation.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1134 2023-05-26 09:22:54.000000 pipiyi_tools-0.0.4/pipiyi-tools/ListQueue.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1928 2023-05-26 09:49:22.000000 pipiyi_tools-0.0.4/pipiyi-tools/Log.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     2070 2023-05-23 06:29:36.000000 pipiyi_tools-0.0.4/pipiyi-tools/MyRequest.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     6711 2023-05-28 14:14:08.000000 pipiyi_tools-0.0.4/pipiyi-tools/PooledBase.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      972 2023-05-23 04:18:08.000000 pipiyi_tools-0.0.4/pipiyi-tools/Storage.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)       19 2023-05-30 09:29:39.000000 pipiyi_tools-0.0.4/pipiyi-tools/__init__.py
+drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-05-30 09:42:36.000000 pipiyi_tools-0.0.4/pipiyi_tools.egg-info/
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      918 2023-05-30 09:42:36.000000 pipiyi_tools-0.0.4/pipiyi_tools.egg-info/PKG-INFO
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      403 2023-05-30 09:42:36.000000 pipiyi_tools-0.0.4/pipiyi_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)        1 2023-05-30 09:42:36.000000 pipiyi_tools-0.0.4/pipiyi_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)       43 2023-05-30 09:42:36.000000 pipiyi_tools-0.0.4/pipiyi_tools.egg-info/requires.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)       13 2023-05-30 09:42:36.000000 pipiyi_tools-0.0.4/pipiyi_tools.egg-info/top_level.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)       38 2023-05-30 09:42:36.000000 pipiyi_tools-0.0.4/setup.cfg
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      989 2023-05-30 09:42:29.000000 pipiyi_tools-0.0.4/setup.py
```

### Comparing `pipiyi_tools-0.0.3/PKG-INFO` & `pipiyi_tools-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipiyi_tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Personal tool library
 Home-page: UNKNOWN
 Author: pipiyi
 Author-email: smallpoliao@gmail.com
 License: UNKNOWN
 Description: 
         # 一个小工具合集
```

### Comparing `pipiyi_tools-0.0.3/pipiyi-tools/EpubSpliter.py` & `pipiyi_tools-0.0.4/pipiyi-tools/EpubSpliter.py`

 * *Files identical despite different names*

### Comparing `pipiyi_tools-0.0.3/pipiyi-tools/FileOperation.py` & `pipiyi_tools-0.0.4/pipiyi-tools/FileOperation.py`

 * *Files identical despite different names*

### Comparing `pipiyi_tools-0.0.3/pipiyi-tools/ListQueue.py` & `pipiyi_tools-0.0.4/pipiyi-tools/ListQueue.py`

 * *Files identical despite different names*

### Comparing `pipiyi_tools-0.0.3/pipiyi-tools/Log.py` & `pipiyi_tools-0.0.4/pipiyi-tools/Log.py`

 * *Files identical despite different names*

### Comparing `pipiyi_tools-0.0.3/pipiyi-tools/MyRequest.py` & `pipiyi_tools-0.0.4/pipiyi-tools/MyRequest.py`

 * *Files identical despite different names*

### Comparing `pipiyi_tools-0.0.3/pipiyi-tools/PooledBase.py` & `pipiyi_tools-0.0.4/pipiyi-tools/PooledBase.py`

 * *Files identical despite different names*

### Comparing `pipiyi_tools-0.0.3/pipiyi-tools/Storage.py` & `pipiyi_tools-0.0.4/pipiyi-tools/Storage.py`

 * *Files identical despite different names*

### Comparing `pipiyi_tools-0.0.3/pipiyi_tools.egg-info/PKG-INFO` & `pipiyi_tools-0.0.4/pipiyi_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipiyi-tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Personal tool library
 Home-page: UNKNOWN
 Author: pipiyi
 Author-email: smallpoliao@gmail.com
 License: UNKNOWN
 Description: 
         # 一个小工具合集
```

### Comparing `pipiyi_tools-0.0.3/setup.py` & `pipiyi_tools-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Personal tool library'
 
 # Setting up
 setup(
     name="pipiyi_tools",
     version=VERSION,
     author="pipiyi",
     author_email="smallpoliao@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
-    packages=find_packages(),
+    packages=['pipiyi-tools'],
     install_requires=['requests', 'ebooklib', 'colorlog','dbutils','pymysql'],
     keywords=['python'],
     setup_requires=['wheel'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

