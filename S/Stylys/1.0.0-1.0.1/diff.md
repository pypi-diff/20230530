# Comparing `tmp/Stylys-1.0.0.tar.gz` & `tmp/Stylys-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Stylys-1.0.0.tar", last modified: Tue May 30 13:24:34 2023, max compression
+gzip compressed data, was "Stylys-1.0.1.tar", last modified: Tue May 30 14:16:56 2023, max compression
```

## Comparing `Stylys-1.0.0.tar` & `Stylys-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 13:24:34.453019 Stylys-1.0.0/
--rw-rw-rw-   0        0        0     1233 2023-05-29 15:27:23.000000 Stylys-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      601 2023-05-30 13:24:34.453019 Stylys-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-05-29 15:37:20.000000 Stylys-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 13:24:34.445025 Stylys-1.0.0/Stylys.egg-info/
--rw-rw-rw-   0        0        0      601 2023-05-30 13:24:33.000000 Stylys-1.0.0/Stylys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      165 2023-05-30 13:24:34.000000 Stylys-1.0.0/Stylys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 13:24:33.000000 Stylys-1.0.0/Stylys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-30 13:24:33.000000 Stylys-1.0.0/Stylys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 13:24:34.457021 Stylys-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      670 2023-05-29 15:27:49.000000 Stylys-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:24:34.449021 Stylys-1.0.0/stylys/
--rw-rw-rw-   0        0        0     1491 2023-05-29 17:49:08.000000 Stylys-1.0.0/stylys/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:16:56.667473 Stylys-1.0.1/
+-rw-rw-rw-   0        0        0     1233 2023-05-29 15:27:23.000000 Stylys-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      902 2023-05-30 14:16:56.667473 Stylys-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-05-29 15:37:20.000000 Stylys-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 14:16:56.655366 Stylys-1.0.1/Stylys.egg-info/
+-rw-rw-rw-   0        0        0      902 2023-05-30 14:16:56.000000 Stylys-1.0.1/Stylys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2023-05-30 14:16:56.000000 Stylys-1.0.1/Stylys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 14:16:56.000000 Stylys-1.0.1/Stylys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 14:16:56.000000 Stylys-1.0.1/Stylys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 14:16:56.667473 Stylys-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      837 2023-05-30 14:07:20.000000 Stylys-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:16:56.663963 Stylys-1.0.1/stylys/
+-rw-rw-rw-   0        0        0     1491 2023-05-30 14:07:26.000000 Stylys-1.0.1/stylys/__init__.py
```

### Comparing `Stylys-1.0.0/LICENSE` & `Stylys-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Stylys-1.0.0/setup.py` & `Stylys-1.0.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from setuptools import setup
 
+with open('README.md') as readme:
+    long_description = readme.read()
+
 setup(
     name='Stylys',
-    version='1.0.0',
+    version='1.0.1',
     description='Just a next text styling library for Python.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author='Ivulka',
     url='https://github.com/IvulkaCZ/Stylys',
     packages=['stylys'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: The Unlicense (Unlicense)',
```

### Comparing `Stylys-1.0.0/stylys/__init__.py` & `Stylys-1.0.1/stylys/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ### Stylys ###
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 # Reset the style
 reset = '\u001b[0m'
 
 # Styling like bold, italic, etc.
 class style:
     def sgr(sgr: str or int or list):
```

