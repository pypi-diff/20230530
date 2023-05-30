# Comparing `tmp/pymangaj-0.1.4.tar.gz` & `tmp/pymangaj-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymangaj-0.1.4.tar", last modified: Tue May 30 03:55:37 2023, max compression
+gzip compressed data, was "pymangaj-0.1.5.tar", last modified: Tue May 30 04:13:53 2023, max compression
```

## Comparing `pymangaj-0.1.4.tar` & `pymangaj-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 03:55:37.390291 pymangaj-0.1.4/
--rw-rw-rw-   0        0        0     1106 2023-05-02 22:15:56.000000 pymangaj-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      808 2023-05-30 03:55:37.390291 pymangaj-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1425 2023-05-30 03:55:14.000000 pymangaj-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 03:55:37.364327 pymangaj-0.1.4/pymangaj/
--rw-rw-rw-   0        0        0        0 2023-05-30 03:42:56.000000 pymangaj-0.1.4/pymangaj/__init__.py
--rw-rw-rw-   0        0        0     5147 2023-05-30 02:30:14.000000 pymangaj-0.1.4/pymangaj/mangalivre.py
--rw-rw-rw-   0        0        0     1665 2023-05-30 01:42:44.000000 pymangaj-0.1.4/pymangaj/muitomanga.py
--rw-rw-rw-   0        0        0      862 2023-05-30 03:47:25.000000 pymangaj-0.1.4/pymangaj/pymangaj.py
-drwxrwxrwx   0        0        0        0 2023-05-30 03:55:37.388296 pymangaj-0.1.4/pymangaj.egg-info/
--rw-rw-rw-   0        0        0      808 2023-05-30 03:55:37.000000 pymangaj-0.1.4/pymangaj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-30 03:55:37.000000 pymangaj-0.1.4/pymangaj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 03:55:37.000000 pymangaj-0.1.4/pymangaj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 03:55:37.000000 pymangaj-0.1.4/pymangaj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 03:55:37.391292 pymangaj-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      888 2023-05-30 03:55:17.000000 pymangaj-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 04:13:53.151758 pymangaj-0.1.5/
+-rw-rw-rw-   0        0        0     1106 2023-05-02 22:15:56.000000 pymangaj-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      808 2023-05-30 04:13:53.150786 pymangaj-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1386 2023-05-30 04:12:15.000000 pymangaj-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 04:13:53.138758 pymangaj-0.1.5/pymangaj/
+-rw-rw-rw-   0        0        0       41 2023-05-30 04:12:41.000000 pymangaj-0.1.5/pymangaj/__init__.py
+-rw-rw-rw-   0        0        0     5147 2023-05-30 02:30:14.000000 pymangaj-0.1.5/pymangaj/mangalivre.py
+-rw-rw-rw-   0        0        0     1665 2023-05-30 01:42:44.000000 pymangaj-0.1.5/pymangaj/muitomanga.py
+-rw-rw-rw-   0        0        0      862 2023-05-30 04:12:26.000000 pymangaj-0.1.5/pymangaj/pymangaj.py
+drwxrwxrwx   0        0        0        0 2023-05-30 04:13:53.148793 pymangaj-0.1.5/pymangaj.egg-info/
+-rw-rw-rw-   0        0        0      808 2023-05-30 04:13:53.000000 pymangaj-0.1.5/pymangaj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-30 04:13:53.000000 pymangaj-0.1.5/pymangaj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 04:13:53.000000 pymangaj-0.1.5/pymangaj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 04:13:53.000000 pymangaj-0.1.5/pymangaj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 04:13:53.151758 pymangaj-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      888 2023-05-30 04:04:07.000000 pymangaj-0.1.5/setup.py
```

### Comparing `pymangaj-0.1.4/LICENSE` & `pymangaj-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.4/PKG-INFO` & `pymangaj-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymangaj
-Version: 0.1.4
+Version: 0.1.5
 Summary: Search and download mangas.
 Home-page: https://github.com/jjeanjacques10/pymangaj
 Author: Jean Jacques Barros
 Author-email: jjean.jacques10@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pymangaj-0.1.4/README.md` & `pymangaj-0.1.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 ```
 
 ## Getting Started
 
 To use pymangaj, import the `pymangaj` module and call the `search()` method. Pass the manga name, chapter, and the sources you want to search from as arguments. The method will return a list of manga pages.
 
 ``` python
-from pymangaj.pymangaj import pymangaj
-from pymangaj.pymangaj import Sources
+from pymangaj import pymangaj, Sources
 
 pymangaj.search("Naruto", 1, sources=[Sources.MANGA_LIVRE, Sources.MUITO_MANGA])
 ```
 
 ## Sources
 
 pymangaj supports the following manga sources:
```

### Comparing `pymangaj-0.1.4/pymangaj/mangalivre.py` & `pymangaj-0.1.5/pymangaj/mangalivre.py`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.4/pymangaj/muitomanga.py` & `pymangaj-0.1.5/pymangaj/muitomanga.py`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.4/pymangaj/pymangaj.py` & `pymangaj-0.1.5/pymangaj/pymangaj.py`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.4/pymangaj.egg-info/PKG-INFO` & `pymangaj-0.1.5/pymangaj.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymangaj
-Version: 0.1.4
+Version: 0.1.5
 Summary: Search and download mangas.
 Home-page: https://github.com/jjeanjacques10/pymangaj
 Author: Jean Jacques Barros
 Author-email: jjean.jacques10@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pymangaj-0.1.4/setup.py` & `pymangaj-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pymangaj',
-    version='0.1.4',
+    version='0.1.5',
     description='Search and download mangas.',
     long_description='PyMangaj is a Python library for searching and retrieving manga pages from different sources. It provides a simple interface to fetch manga pages from popular manga websites.',
     author='Jean Jacques Barros',
     author_email='jjean.jacques10@gmail.com',
     url='https://github.com/jjeanjacques10/pymangaj',
     packages=find_packages(),
     classifiers=[
```

