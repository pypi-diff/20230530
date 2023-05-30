# Comparing `tmp/airscript-0.0.2.tar.gz` & `tmp/airscript-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airscript-0.0.2.tar", last modified: Tue May 30 07:25:48 2023, max compression
+gzip compressed data, was "airscript-0.0.3.tar", last modified: Tue May 30 07:44:45 2023, max compression
```

## Comparing `airscript-0.0.2.tar` & `airscript-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 07:25:48.312337 airscript-0.0.2/
--rw-rw-rw-   0        0        0      282 2023-05-30 07:25:48.312337 airscript-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-30 06:39:59.000000 airscript-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 07:25:48.305339 airscript-0.0.2/action/
--rw-rw-rw-   0        0        0      390 2023-05-30 07:12:19.000000 airscript-0.0.2/action/__init__.py
--rw-rw-rw-   0        0        0      165 2023-05-30 06:31:48.000000 airscript-0.0.2/action/touch.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:25:48.309336 airscript-0.0.2/airscript.egg-info/
--rw-rw-rw-   0        0        0      282 2023-05-30 07:25:48.000000 airscript-0.0.2/airscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-05-30 07:25:48.000000 airscript-0.0.2/airscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 07:25:48.000000 airscript-0.0.2/airscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-30 07:25:48.000000 airscript-0.0.2/airscript.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-30 07:25:48.310336 airscript-0.0.2/graphics/
--rw-rw-rw-   0        0        0       85 2023-05-30 06:27:00.000000 airscript-0.0.2/graphics/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-30 07:25:48.312337 airscript-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      523 2023-05-30 07:24:17.000000 airscript-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:44:45.765856 airscript-0.0.3/
+-rw-rw-rw-   0        0        0      431 2023-05-30 07:44:45.764857 airscript-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-30 06:39:59.000000 airscript-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 07:44:45.755857 airscript-0.0.3/airscript/
+-rw-rw-rw-   0        0        0        0 2023-05-30 07:43:45.000000 airscript-0.0.3/airscript/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:44:45.762861 airscript-0.0.3/airscript/action/
+-rw-rw-rw-   0        0        0      405 2023-05-30 07:43:59.000000 airscript-0.0.3/airscript/action/__init__.py
+-rw-rw-rw-   0        0        0      165 2023-05-30 06:31:48.000000 airscript-0.0.3/airscript/action/touch.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:44:45.763858 airscript-0.0.3/airscript/graphics/
+-rw-rw-rw-   0        0        0       85 2023-05-30 06:27:00.000000 airscript-0.0.3/airscript/graphics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:44:45.760858 airscript-0.0.3/airscript.egg-info/
+-rw-rw-rw-   0        0        0      431 2023-05-30 07:44:45.000000 airscript-0.0.3/airscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-30 07:44:45.000000 airscript-0.0.3/airscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 07:44:45.000000 airscript-0.0.3/airscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 07:44:45.000000 airscript-0.0.3/airscript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 07:44:45.765856 airscript-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      692 2023-05-30 07:44:36.000000 airscript-0.0.3/setup.py
```

### Comparing `airscript-0.0.2/setup.py` & `airscript-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'airscript Type derivation package'
 
 setup(
     name="airscript",
     version=VERSION,
     author="ITisl",
     author_email="1831207432@qq.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=open('README.md', encoding="UTF8").read(),
     packages=find_packages(),
     keywords=['python', "airscript"],
     license="MIT",
+classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
     url="https://github.com/itisl2220/airscript",
 )
```

