# Comparing `tmp/airscript-0.0.3.tar.gz` & `tmp/airscript-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airscript-0.0.3.tar", last modified: Tue May 30 07:44:45 2023, max compression
+gzip compressed data, was "airscript-0.0.5.tar", last modified: Tue May 30 09:21:44 2023, max compression
```

## Comparing `airscript-0.0.3.tar` & `airscript-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 07:44:45.765856 airscript-0.0.3/
--rw-rw-rw-   0        0        0      431 2023-05-30 07:44:45.764857 airscript-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-30 06:39:59.000000 airscript-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 07:44:45.755857 airscript-0.0.3/airscript/
--rw-rw-rw-   0        0        0        0 2023-05-30 07:43:45.000000 airscript-0.0.3/airscript/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:44:45.762861 airscript-0.0.3/airscript/action/
--rw-rw-rw-   0        0        0      405 2023-05-30 07:43:59.000000 airscript-0.0.3/airscript/action/__init__.py
--rw-rw-rw-   0        0        0      165 2023-05-30 06:31:48.000000 airscript-0.0.3/airscript/action/touch.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:44:45.763858 airscript-0.0.3/airscript/graphics/
--rw-rw-rw-   0        0        0       85 2023-05-30 06:27:00.000000 airscript-0.0.3/airscript/graphics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:44:45.760858 airscript-0.0.3/airscript.egg-info/
--rw-rw-rw-   0        0        0      431 2023-05-30 07:44:45.000000 airscript-0.0.3/airscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-30 07:44:45.000000 airscript-0.0.3/airscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 07:44:45.000000 airscript-0.0.3/airscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 07:44:45.000000 airscript-0.0.3/airscript.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 07:44:45.765856 airscript-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      692 2023-05-30 07:44:36.000000 airscript-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.671075 airscript-0.0.5/
+-rw-rw-rw-   0        0        0      431 2023-05-30 09:21:44.670077 airscript-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-30 06:39:59.000000 airscript-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.652050 airscript-0.0.5/airscript/
+-rw-rw-rw-   0        0        0        0 2023-05-30 08:18:07.000000 airscript-0.0.5/airscript/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.663075 airscript-0.0.5/airscript/action/
+-rw-rw-rw-   0        0        0      454 2023-05-30 08:07:48.000000 airscript-0.0.5/airscript/action/__init__.py
+-rw-rw-rw-   0        0        0      266 2023-05-30 08:02:07.000000 airscript-0.0.5/airscript/action/gesture.py
+-rw-rw-rw-   0        0        0     1376 2023-05-30 08:11:36.000000 airscript-0.0.5/airscript/action/key.py
+-rw-rw-rw-   0        0        0     1272 2023-05-30 08:04:45.000000 airscript-0.0.5/airscript/action/path.py
+-rw-rw-rw-   0        0        0      165 2023-05-30 06:31:48.000000 airscript-0.0.5/airscript/action/touch.py
+-rw-rw-rw-   0        0        0      157 2023-05-30 09:11:25.000000 airscript-0.0.5/airscript/data.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.664074 airscript-0.0.5/airscript/graphics/
+-rw-rw-rw-   0        0        0       85 2023-05-30 06:27:00.000000 airscript-0.0.5/airscript/graphics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.665074 airscript-0.0.5/airscript/intent/
+-rw-rw-rw-   0        0        0      111 2023-05-30 09:15:39.000000 airscript-0.0.5/airscript/intent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.665074 airscript-0.0.5/airscript/screen/
+-rw-rw-rw-   0        0        0     3960 2023-05-30 08:44:26.000000 airscript-0.0.5/airscript/screen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.666074 airscript-0.0.5/airscript/system/
+-rw-rw-rw-   0        0        0      716 2023-05-30 09:21:23.000000 airscript-0.0.5/airscript/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.668075 airscript-0.0.5/airscript/ui/
+-rw-rw-rw-   0        0        0      631 2023-05-30 09:03:49.000000 airscript-0.0.5/airscript/ui/__init__.py
+-rw-rw-rw-   0        0        0      961 2023-05-30 09:03:44.000000 airscript-0.0.5/airscript/ui/dialog.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.657064 airscript-0.0.5/airscript.egg-info/
+-rw-rw-rw-   0        0        0      431 2023-05-30 09:21:44.000000 airscript-0.0.5/airscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-05-30 09:21:44.000000 airscript-0.0.5/airscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 09:21:44.000000 airscript-0.0.5/airscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 09:21:44.000000 airscript-0.0.5/airscript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 09:21:44.671075 airscript-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      692 2023-05-30 09:21:23.000000 airscript-0.0.5/setup.py
```

### Comparing `airscript-0.0.3/setup.py` & `airscript-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.5'
 DESCRIPTION = 'airscript Type derivation package'
 
 setup(
     name="airscript",
     version=VERSION,
     author="ITisl",
     author_email="1831207432@qq.com",
```

