# Comparing `tmp/hertz_packet-1.0.0.tar.gz` & `tmp/hertz_packet-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hertz_packet-1.0.0.tar", last modified: Fri May 12 02:38:54 2023, max compression
+gzip compressed data, was "hertz_packet-1.1.0.tar", last modified: Tue May 30 14:39:13 2023, max compression
```

## Comparing `hertz_packet-1.0.0.tar` & `hertz_packet-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 02:38:54.533985 hertz_packet-1.0.0/
--rw-rw-rw-   0        0        0     1082 2023-05-12 02:13:36.000000 hertz_packet-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      610 2023-05-12 02:38:54.530994 hertz_packet-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       49 2023-05-12 02:13:36.000000 hertz_packet-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 02:38:54.507057 hertz_packet-1.0.0/hertz_packet/
--rw-rw-rw-   0        0        0      150 2023-05-12 02:34:21.000000 hertz_packet-1.0.0/hertz_packet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:38:54.528001 hertz_packet-1.0.0/hertz_packet/notice/
--rw-rw-rw-   0        0        0      564 2023-05-12 02:34:21.000000 hertz_packet-1.0.0/hertz_packet/notice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:38:54.525009 hertz_packet-1.0.0/hertz_packet.egg-info/
--rw-rw-rw-   0        0        0      610 2023-05-12 02:38:54.000000 hertz_packet-1.0.0/hertz_packet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-12 02:38:54.000000 hertz_packet-1.0.0/hertz_packet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 02:38:54.000000 hertz_packet-1.0.0/hertz_packet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-12 02:38:54.000000 hertz_packet-1.0.0/hertz_packet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-12 02:38:54.000000 hertz_packet-1.0.0/hertz_packet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 02:38:54.533985 hertz_packet-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      942 2023-05-12 02:28:48.000000 hertz_packet-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:39:13.341162 hertz_packet-1.1.0/
+-rw-rw-rw-   0        0        0     1082 2023-05-20 05:12:59.000000 hertz_packet-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      610 2023-05-30 14:39:13.340162 hertz_packet-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2023-05-20 05:12:59.000000 hertz_packet-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 14:39:13.327157 hertz_packet-1.1.0/hertz_packet/
+-rw-rw-rw-   0        0        0      150 2023-05-20 05:12:59.000000 hertz_packet-1.1.0/hertz_packet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:39:13.334162 hertz_packet-1.1.0/hertz_packet/notice/
+-rw-rw-rw-   0        0        0      582 2023-05-20 05:58:04.000000 hertz_packet-1.1.0/hertz_packet/notice/__init__.py
+-rw-rw-rw-   0        0        0     1393 2023-05-30 12:04:34.000000 hertz_packet-1.1.0/hertz_packet/notice/log.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:39:13.336162 hertz_packet-1.1.0/hertz_packet/recall/
+-rw-rw-rw-   0        0        0      153 2023-05-20 05:58:04.000000 hertz_packet-1.1.0/hertz_packet/recall/__init__.py
+-rw-rw-rw-   0        0        0     2090 2023-05-30 12:04:34.000000 hertz_packet-1.1.0/hertz_packet/recall/mysql.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:39:13.332163 hertz_packet-1.1.0/hertz_packet.egg-info/
+-rw-rw-rw-   0        0        0      610 2023-05-30 14:39:13.000000 hertz_packet-1.1.0/hertz_packet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-05-30 14:39:13.000000 hertz_packet-1.1.0/hertz_packet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 14:39:13.000000 hertz_packet-1.1.0/hertz_packet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-30 14:39:13.000000 hertz_packet-1.1.0/hertz_packet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-30 14:39:13.000000 hertz_packet-1.1.0/hertz_packet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 14:39:13.341162 hertz_packet-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      969 2023-05-30 14:38:32.000000 hertz_packet-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:39:13.337162 hertz_packet-1.1.0/test/
+-rw-rw-rw-   0        0        0      153 2023-05-30 12:04:34.000000 hertz_packet-1.1.0/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:39:13.339162 hertz_packet-1.1.0/test/notice/
+-rw-rw-rw-   0        0        0      153 2023-05-30 12:04:34.000000 hertz_packet-1.1.0/test/notice/__init__.py
+-rw-rw-rw-   0        0        0      230 2023-05-30 12:04:34.000000 hertz_packet-1.1.0/test/notice/log_t1.py
```

### Comparing `hertz_packet-1.0.0/LICENSE` & `hertz_packet-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hertz_packet-1.0.0/PKG-INFO` & `hertz_packet-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hertz_packet
-Version: 1.0.0
+Version: 1.1.0
 Summary: release Hertz
 Home-page: https://github.com/luke1879012/hertz_packet
 Author: luke9012
 Author-email: luke781520097@163.com
 License: MIT
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `hertz_packet-1.0.0/hertz_packet/notice/__init__.py` & `hertz_packet-1.1.0/hertz_packet/notice/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
 @Project : hertz_packet 
 @File    : __init__.py
 @Date    : 2023/5/12 10:31:05
 @Author  : zhchen
-@Desc    : 
+@Desc    : 发送一些消息
 """
 import json
 
 import requests
 
 
 def send_note(_k, _v, _memo: dict = None):
```

### Comparing `hertz_packet-1.0.0/hertz_packet.egg-info/PKG-INFO` & `hertz_packet-1.1.0/hertz_packet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hertz-packet
-Version: 1.0.0
+Version: 1.1.0
 Summary: release Hertz
 Home-page: https://github.com/luke1879012/hertz_packet
 Author: luke9012
 Author-email: luke781520097@163.com
 License: MIT
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `hertz_packet-1.0.0/setup.py` & `hertz_packet-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='hertz_packet',  # 包名
-    version='1.0.0',  # 版本号
+    version='1.1.0',  # 版本号
     description='release Hertz',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='luke9012',
     author_email='luke781520097@163.com',
     url='https://github.com/luke1879012/hertz_packet',
     install_requires=[
         'requests~=2.27.1',
+        'pymysql~=1.0.3',
     ],
     license='MIT',
     packages=find_packages(),
     platforms=["all"],
     python_requires='>=3.6',
     classifiers=[
         'Intended Audience :: Developers',
```

