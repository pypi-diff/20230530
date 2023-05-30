# Comparing `tmp/vbarongdatools001-0.0.8.tar.gz` & `tmp/vbarongdatools001-0.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbarongdatools001-0.0.8.tar", last modified: Mon May 29 09:50:43 2023, max compression
+gzip compressed data, was "vbarongdatools001-0.0.9.1.tar", last modified: Tue May 30 06:07:42 2023, max compression
```

## Comparing `vbarongdatools001-0.0.8.tar` & `vbarongdatools001-0.0.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 09:50:43.762139 vbarongdatools001-0.0.8/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 vbarongdatools001-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 vbarongdatools001-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      397 2023-05-29 09:50:43.762139 vbarongdatools001-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 vbarongdatools001-0.0.8/README.md
--rw-rw-rw-   0        0        0      136 2023-05-29 09:50:43.764141 vbarongdatools001-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-05-29 09:44:25.000000 vbarongdatools001-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 09:50:43.750982 vbarongdatools001-0.0.8/vbarongdatools001/
--rw-rw-rw-   0        0        0    53248 2023-05-29 08:40:18.000000 vbarongdatools001-0.0.8/vbarongdatools001/Vbalog.pyd
--rw-rw-rw-   0        0        0     1041 2023-05-29 08:29:49.000000 vbarongdatools001-0.0.8/vbarongdatools001/Vbalogpy.py
--rw-rw-rw-   0        0        0        0 2023-05-26 10:19:22.000000 vbarongdatools001-0.0.8/vbarongdatools001/__init__.py
--rw-rw-rw-   0        0        0    67584 2023-05-29 08:40:27.000000 vbarongdatools001-0.0.8/vbarongdatools001/vbaLogin.pyd
--rw-rw-rw-   0        0        0      156 2023-05-29 09:11:49.000000 vbarongdatools001-0.0.8/vbarongdatools001/vbaloginpy.py
--rw-rw-rw-   0        0        0    48640 2023-05-29 09:47:54.000000 vbarongdatools001-0.0.8/vbarongdatools001/vbarongdatools001.pyd
--rw-rw-rw-   0        0        0   789620 2023-05-29 09:45:24.000000 vbarongdatools001-0.0.8/vbarongdatools001/批量移动或重命名文件、创建文件夹-V0003.xlsm
-drwxrwxrwx   0        0        0        0 2023-05-29 09:50:43.761139 vbarongdatools001-0.0.8/vbarongdatools001.egg-info/
--rw-rw-rw-   0        0        0      397 2023-05-29 09:50:43.000000 vbarongdatools001-0.0.8/vbarongdatools001.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-05-29 09:50:43.000000 vbarongdatools001-0.0.8/vbarongdatools001.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 09:50:43.000000 vbarongdatools001-0.0.8/vbarongdatools001.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-29 09:50:43.000000 vbarongdatools001-0.0.8/vbarongdatools001.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 06:07:42.331210 vbarongdatools001-0.0.9.1/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 vbarongdatools001-0.0.9.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 vbarongdatools001-0.0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      399 2023-05-30 06:07:42.331210 vbarongdatools001-0.0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 vbarongdatools001-0.0.9.1/README.md
+-rw-rw-rw-   0        0        0      136 2023-05-30 06:07:42.332186 vbarongdatools001-0.0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      981 2023-05-30 06:07:36.000000 vbarongdatools001-0.0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:07:42.319184 vbarongdatools001-0.0.9.1/vbarongdatools001/
+-rw-rw-rw-   0        0        0    53248 2023-05-29 08:40:18.000000 vbarongdatools001-0.0.9.1/vbarongdatools001/Vbalog.pyd
+-rw-rw-rw-   0        0        0     1041 2023-05-29 08:29:49.000000 vbarongdatools001-0.0.9.1/vbarongdatools001/Vbalogpy.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 10:19:22.000000 vbarongdatools001-0.0.9.1/vbarongdatools001/__init__.py
+-rw-rw-rw-   0        0        0    67584 2023-05-29 08:40:27.000000 vbarongdatools001-0.0.9.1/vbarongdatools001/vbaLogin.pyd
+-rw-rw-rw-   0        0        0      156 2023-05-29 09:11:49.000000 vbarongdatools001-0.0.9.1/vbarongdatools001/vbaloginpy.py
+-rw-rw-rw-   0        0        0    48640 2023-05-29 09:47:54.000000 vbarongdatools001-0.0.9.1/vbarongdatools001/vbarongdatools001.pyd
+-rw-rw-rw-   0        0        0   789620 2023-05-29 09:45:24.000000 vbarongdatools001-0.0.9.1/vbarongdatools001/批量移动或重命名文件、创建文件夹-V0003.xlsm
+drwxrwxrwx   0        0        0        0 2023-05-30 06:07:42.329185 vbarongdatools001-0.0.9.1/vbarongdatools001.egg-info/
+-rw-rw-rw-   0        0        0      399 2023-05-30 06:07:42.000000 vbarongdatools001-0.0.9.1/vbarongdatools001.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2023-05-30 06:07:42.000000 vbarongdatools001-0.0.9.1/vbarongdatools001.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 06:07:42.000000 vbarongdatools001-0.0.9.1/vbarongdatools001.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-30 06:07:42.000000 vbarongdatools001-0.0.9.1/vbarongdatools001.egg-info/top_level.txt
```

### Comparing `vbarongdatools001-0.0.8/LICENSE.txt` & `vbarongdatools001-0.0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vbarongdatools001-0.0.8/setup.py` & `vbarongdatools001-0.0.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
-PATCH = 8
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
+PATCH = 9
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.1"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "vbarongdatools001",
     version=VERSION,
```

### Comparing `vbarongdatools001-0.0.8/vbarongdatools001/Vbalogpy.py` & `vbarongdatools001-0.0.9.1/vbarongdatools001/Vbalogpy.py`

 * *Files identical despite different names*

### Comparing `vbarongdatools001-0.0.8/vbarongdatools001/批量移动或重命名文件、创建文件夹-V0003.xlsm` & `vbarongdatools001-0.0.9.1/vbarongdatools001/批量移动或重命名文件、创建文件夹-V0003.xlsm`

 * *Files identical despite different names*

