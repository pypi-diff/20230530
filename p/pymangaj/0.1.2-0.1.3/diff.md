# Comparing `tmp/pymangaj-0.1.2.tar.gz` & `tmp/pymangaj-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymangaj-0.1.2.tar", last modified: Tue May 30 03:29:14 2023, max compression
+gzip compressed data, was "pymangaj-0.1.3.tar", last modified: Tue May 30 03:45:27 2023, max compression
```

## Comparing `pymangaj-0.1.2.tar` & `pymangaj-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 03:29:14.321131 pymangaj-0.1.2/
--rw-rw-rw-   0        0        0     1106 2023-05-02 22:15:56.000000 pymangaj-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      769 2023-05-30 03:29:14.320151 pymangaj-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1383 2023-05-30 03:06:10.000000 pymangaj-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 03:29:14.302131 pymangaj-0.1.2/pymanga/
--rw-rw-rw-   0        0        0        0 2023-05-29 23:21:17.000000 pymangaj-0.1.2/pymanga/__init__.py
--rw-rw-rw-   0        0        0      877 2023-05-30 03:28:22.000000 pymangaj-0.1.2/pymanga/pymanga.py
--rw-rw-rw-   0        0        0      299 2023-05-30 02:28:57.000000 pymangaj-0.1.2/pymanga/test.py
-drwxrwxrwx   0        0        0        0 2023-05-30 03:29:14.317168 pymangaj-0.1.2/pymangaj.egg-info/
--rw-rw-rw-   0        0        0      769 2023-05-30 03:29:14.000000 pymangaj-0.1.2/pymangaj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-30 03:29:14.000000 pymangaj-0.1.2/pymangaj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 03:29:14.000000 pymangaj-0.1.2/pymangaj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 03:29:14.000000 pymangaj-0.1.2/pymangaj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 03:29:14.321131 pymangaj-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      888 2023-05-30 03:28:55.000000 pymangaj-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:45:27.247449 pymangaj-0.1.3/
+-rw-rw-rw-   0        0        0     1106 2023-05-02 22:15:56.000000 pymangaj-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      808 2023-05-30 03:45:27.246449 pymangaj-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1386 2023-05-30 03:44:53.000000 pymangaj-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 03:45:27.223446 pymangaj-0.1.3/pymangaj/
+-rw-rw-rw-   0        0        0        0 2023-05-30 03:42:56.000000 pymangaj-0.1.3/pymangaj/__init__.py
+-rw-rw-rw-   0        0        0     5147 2023-05-30 02:30:14.000000 pymangaj-0.1.3/pymangaj/mangalivre.py
+-rw-rw-rw-   0        0        0     1665 2023-05-30 01:42:44.000000 pymangaj-0.1.3/pymangaj/muitomanga.py
+-rw-rw-rw-   0        0        0      860 2023-05-30 03:44:20.000000 pymangaj-0.1.3/pymangaj/pymangaj.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:45:27.244484 pymangaj-0.1.3/pymangaj.egg-info/
+-rw-rw-rw-   0        0        0      808 2023-05-30 03:45:27.000000 pymangaj-0.1.3/pymangaj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-30 03:45:27.000000 pymangaj-0.1.3/pymangaj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 03:45:27.000000 pymangaj-0.1.3/pymangaj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 03:45:27.000000 pymangaj-0.1.3/pymangaj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 03:45:27.247449 pymangaj-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      888 2023-05-30 03:45:07.000000 pymangaj-0.1.3/setup.py
```

### Comparing `pymangaj-0.1.2/LICENSE` & `pymangaj-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.2/PKG-INFO` & `pymangaj-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: pymangaj
-Version: 0.1.2
+Version: 0.1.3
 Summary: Search and download mangas.
 Home-page: https://github.com/jjeanjacques10/pymangaj
 Author: Jean Jacques Barros
 Author-email: jjean.jacques10@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 
 PyMangaj is a Python library for searching and retrieving manga pages from different sources. It provides a simple interface to fetch manga pages from popular manga websites.
+
```

### Comparing `pymangaj-0.1.2/README.md` & `pymangaj-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # PyMangaJ
 
-pymangaj is a Python library for searching and retrieving manga pages from different sources. It provides a simple interface to fetch manga pages from popular manga websites.
+Pymangaj is a Python library for searching and retrieving manga pages from different sources. It provides a simple interface to fetch manga pages from popular manga websites.
 
 ## Installation
 
 You can install pymangaj using pip:
 
 ``` bash
 pip install pymangaj
 ```
 
 ## Getting Started
 
-To use pymangaj, import the `pymanga` module and call the `search()` method. Pass the manga name, chapter, and the sources you want to search from as arguments. The method will return a list of manga pages.
+To use pymangaj, import the `pymangaj` module and call the `search()` method. Pass the manga name, chapter, and the sources you want to search from as arguments. The method will return a list of manga pages.
 
 ``` python
-from pymangaj import pymanga, Sources
+from pymangaj import pymangaj, Sources
 
-pymanga.search("Naruto", 1, sources=[Sources.MANGA_LIVRE, Sources.MUITO_MANGA])
+pymangaj.search("Naruto", 1, sources=[Sources.MANGA_LIVRE, Sources.MUITO_MANGA])
 ```
 
 ## Sources
 
 pymangaj supports the following manga sources:
 
 |          Source                       | Language | Status |
```

### Comparing `pymangaj-0.1.2/pymanga/pymanga.py` & `pymangaj-0.1.3/pymangaj/pymangaj.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
-from .sources.mangalivre import MangaLivre
-from .sources.muitomanga import MuitoManga
+from mangalivre import MangaLivre
+from muitomanga import MuitoManga
 
 class Sources(Enum):
     MANGA_LIVRE = 'manga_livre'
     MUITO_MANGA = 'muito_manga'
 
 class SourceFactory:
     _value_map = {
@@ -14,15 +14,15 @@
 
     @staticmethod
     def get_source(value, manga_name, chapter):
         cls = SourceFactory._value_map[value]
         return cls(manga_name, chapter)
 
 
-class pymanga:
+class pymangaj:
     
     @staticmethod
     # Get mangas by sources
     def search(manga_name, chapter, **sources):
         result = []
         for source in sources['sources']:
             manga_downloader = SourceFactory.get_source(source, manga_name, chapter)
```

### Comparing `pymangaj-0.1.2/pymangaj.egg-info/PKG-INFO` & `pymangaj-0.1.3/pymangaj.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: pymangaj
-Version: 0.1.2
+Version: 0.1.3
 Summary: Search and download mangas.
 Home-page: https://github.com/jjeanjacques10/pymangaj
 Author: Jean Jacques Barros
 Author-email: jjean.jacques10@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 
 PyMangaj is a Python library for searching and retrieving manga pages from different sources. It provides a simple interface to fetch manga pages from popular manga websites.
+
```

### Comparing `pymangaj-0.1.2/setup.py` & `pymangaj-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pymangaj',
-    version='0.1.2',
+    version='0.1.3',
     description='Search and download mangas.',
     long_description='PyMangaj is a Python library for searching and retrieving manga pages from different sources. It provides a simple interface to fetch manga pages from popular manga websites.',
     author='Jean Jacques Barros',
     author_email='jjean.jacques10@gmail.com',
     url='https://github.com/jjeanjacques10/pymangaj',
     packages=find_packages(),
     classifiers=[
```

