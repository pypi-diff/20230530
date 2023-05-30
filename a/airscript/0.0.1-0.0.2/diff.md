# Comparing `tmp/airscript-0.0.1.tar.gz` & `tmp/airscript-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airscript-0.0.1.tar", last modified: Tue May 30 06:42:18 2023, max compression
+gzip compressed data, was "airscript-0.0.2.tar", last modified: Tue May 30 07:25:48 2023, max compression
```

## Comparing `airscript-0.0.1.tar` & `airscript-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 06:42:18.206447 airscript-0.0.1/
--rw-rw-rw-   0        0        0      282 2023-05-30 06:42:18.206447 airscript-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-30 06:39:59.000000 airscript-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 06:42:18.198272 airscript-0.0.1/action/
--rw-rw-rw-   0        0        0      385 2023-05-30 06:34:12.000000 airscript-0.0.1/action/__init__.py
--rw-rw-rw-   0        0        0      165 2023-05-30 06:31:48.000000 airscript-0.0.1/action/touch.py
-drwxrwxrwx   0        0        0        0 2023-05-30 06:42:18.203447 airscript-0.0.1/airscript.egg-info/
--rw-rw-rw-   0        0        0      282 2023-05-30 06:42:18.000000 airscript-0.0.1/airscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-05-30 06:42:18.000000 airscript-0.0.1/airscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 06:42:18.000000 airscript-0.0.1/airscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-30 06:42:18.000000 airscript-0.0.1/airscript.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-30 06:42:18.204446 airscript-0.0.1/graphics/
--rw-rw-rw-   0        0        0       85 2023-05-30 06:27:00.000000 airscript-0.0.1/graphics/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-30 06:42:18.206447 airscript-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      523 2023-05-30 06:39:39.000000 airscript-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:25:48.312337 airscript-0.0.2/
+-rw-rw-rw-   0        0        0      282 2023-05-30 07:25:48.312337 airscript-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-30 06:39:59.000000 airscript-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 07:25:48.305339 airscript-0.0.2/action/
+-rw-rw-rw-   0        0        0      390 2023-05-30 07:12:19.000000 airscript-0.0.2/action/__init__.py
+-rw-rw-rw-   0        0        0      165 2023-05-30 06:31:48.000000 airscript-0.0.2/action/touch.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:25:48.309336 airscript-0.0.2/airscript.egg-info/
+-rw-rw-rw-   0        0        0      282 2023-05-30 07:25:48.000000 airscript-0.0.2/airscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-05-30 07:25:48.000000 airscript-0.0.2/airscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 07:25:48.000000 airscript-0.0.2/airscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-30 07:25:48.000000 airscript-0.0.2/airscript.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 07:25:48.310336 airscript-0.0.2/graphics/
+-rw-rw-rw-   0        0        0       85 2023-05-30 06:27:00.000000 airscript-0.0.2/graphics/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-30 07:25:48.312337 airscript-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      523 2023-05-30 07:24:17.000000 airscript-0.0.2/setup.py
```

### Comparing `airscript-0.0.1/setup.py` & `airscript-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'airscript Type derivation package'
 
 setup(
     name="airscript",
     version=VERSION,
     author="ITisl",
     author_email="1831207432@qq.com",
```

