# Comparing `tmp/pymangaj-0.1.1.tar.gz` & `tmp/pymangaj-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymangaj-0.1.1.tar", last modified: Tue May 30 03:23:37 2023, max compression
+gzip compressed data, was "pymangaj-0.1.2.tar", last modified: Tue May 30 03:29:14 2023, max compression
```

## Comparing `pymangaj-0.1.1.tar` & `pymangaj-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 03:23:37.769443 pymangaj-0.1.1/
--rw-rw-rw-   0        0        0     1106 2023-05-02 22:15:56.000000 pymangaj-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      640 2023-05-30 03:23:37.768442 pymangaj-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1383 2023-05-30 03:06:10.000000 pymangaj-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 03:23:37.749442 pymangaj-0.1.1/pymanga/
--rw-rw-rw-   0        0        0        0 2023-05-29 23:21:17.000000 pymangaj-0.1.1/pymanga/__init__.py
--rw-rw-rw-   0        0        0      891 2023-05-30 03:19:08.000000 pymangaj-0.1.1/pymanga/pymanga.py
--rw-rw-rw-   0        0        0      299 2023-05-30 02:28:57.000000 pymangaj-0.1.1/pymanga/test.py
-drwxrwxrwx   0        0        0        0 2023-05-30 03:23:37.766441 pymangaj-0.1.1/pymangaj.egg-info/
--rw-rw-rw-   0        0        0      640 2023-05-30 03:23:37.000000 pymangaj-0.1.1/pymangaj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-30 03:23:37.000000 pymangaj-0.1.1/pymangaj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 03:23:37.000000 pymangaj-0.1.1/pymangaj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 03:23:37.000000 pymangaj-0.1.1/pymangaj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 03:23:37.770452 pymangaj-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      759 2023-05-30 03:20:14.000000 pymangaj-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:29:14.321131 pymangaj-0.1.2/
+-rw-rw-rw-   0        0        0     1106 2023-05-02 22:15:56.000000 pymangaj-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      769 2023-05-30 03:29:14.320151 pymangaj-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1383 2023-05-30 03:06:10.000000 pymangaj-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 03:29:14.302131 pymangaj-0.1.2/pymanga/
+-rw-rw-rw-   0        0        0        0 2023-05-29 23:21:17.000000 pymangaj-0.1.2/pymanga/__init__.py
+-rw-rw-rw-   0        0        0      877 2023-05-30 03:28:22.000000 pymangaj-0.1.2/pymanga/pymanga.py
+-rw-rw-rw-   0        0        0      299 2023-05-30 02:28:57.000000 pymangaj-0.1.2/pymanga/test.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:29:14.317168 pymangaj-0.1.2/pymangaj.egg-info/
+-rw-rw-rw-   0        0        0      769 2023-05-30 03:29:14.000000 pymangaj-0.1.2/pymangaj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-30 03:29:14.000000 pymangaj-0.1.2/pymangaj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 03:29:14.000000 pymangaj-0.1.2/pymangaj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 03:29:14.000000 pymangaj-0.1.2/pymangaj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 03:29:14.321131 pymangaj-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      888 2023-05-30 03:28:55.000000 pymangaj-0.1.2/setup.py
```

### Comparing `pymangaj-0.1.1/LICENSE` & `pymangaj-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.1/README.md` & `pymangaj-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.1/pymanga/pymanga.py` & `pymangaj-0.1.2/pymanga/pymanga.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
-from pymanga.sources.mangalivre import MangaLivre
-from pymanga.sources.muitomanga import MuitoManga
+from .sources.mangalivre import MangaLivre
+from .sources.muitomanga import MuitoManga
 
 class Sources(Enum):
     MANGA_LIVRE = 'manga_livre'
     MUITO_MANGA = 'muito_manga'
 
 class SourceFactory:
     _value_map = {
```

