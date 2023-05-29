# Comparing `tmp/IMDBTraktSyncer-1.3.6.tar.gz` & `tmp/IMDBTraktSyncer-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.3.6.tar", last modified: Mon May 29 23:51:47 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.3.7.tar", last modified: Mon May 29 23:54:34 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.3.6.tar` & `IMDBTraktSyncer-1.3.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 23:51:47.634969 IMDBTraktSyncer-1.3.6/
-drwxrwxrwx   0        0        0        0 2023-05-29 23:51:47.601962 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    23224 2023-05-29 23:47:18.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4440 2023-05-28 13:20:16.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4207 2023-05-24 23:10:07.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3858 2023-05-28 12:08:18.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     7844 2023-05-29 23:40:21.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     6982 2023-05-28 12:08:00.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-29 23:51:47.631975 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    11969 2023-05-29 23:51:47.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-05-29 23:51:47.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 23:51:47.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-29 23:51:47.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-29 23:51:47.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-29 23:51:47.000000 IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.3.6/LICENSE
--rw-rw-rw-   0        0        0    11969 2023-05-29 23:51:47.633976 IMDBTraktSyncer-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0    11226 2023-05-29 23:50:45.000000 IMDBTraktSyncer-1.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 23:51:47.634969 IMDBTraktSyncer-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-05-29 23:51:10.000000 IMDBTraktSyncer-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 23:54:34.263412 IMDBTraktSyncer-1.3.7/
+drwxrwxrwx   0        0        0        0 2023-05-29 23:54:34.240860 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    23158 2023-05-29 23:53:46.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4440 2023-05-28 13:20:16.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4207 2023-05-24 23:10:07.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3858 2023-05-28 12:08:18.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     7844 2023-05-29 23:40:21.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     6982 2023-05-28 12:08:00.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-29 23:54:34.260413 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    11969 2023-05-29 23:54:34.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-05-29 23:54:34.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 23:54:34.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-29 23:54:34.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-29 23:54:34.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-29 23:54:34.000000 IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.3.7/LICENSE
+-rw-rw-rw-   0        0        0    11969 2023-05-29 23:54:34.261414 IMDBTraktSyncer-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11226 2023-05-29 23:50:45.000000 IMDBTraktSyncer-1.3.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 23:54:34.263412 IMDBTraktSyncer-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-05-29 23:54:31.000000 IMDBTraktSyncer-1.3.7/setup.py
```

### Comparing `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.common.exceptions import SessionNotCreatedException
-from selenium.webdriver.common.action_chains import ActionChains
 try:
     from IMDBTraktSyncer import checkChromedriver
     from IMDBTraktSyncer import verifyCredentials as VC
     from IMDBTraktSyncer import traktData
     from IMDBTraktSyncer import imdbData
     from IMDBTraktSyncer import errorHandling as EH
 except ImportError:
```

### Comparing `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/imdbData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.3.6
+Version: 1.3.7
 Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.3.6/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.3.7/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.6/LICENSE` & `IMDBTraktSyncer-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.6/PKG-INFO` & `IMDBTraktSyncer-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.3.6
+Version: 1.3.7
 Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.3.6/README.md` & `IMDBTraktSyncer-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.3.6/setup.py` & `IMDBTraktSyncer-1.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.3.6'
+VERSION = '1.3.7'
 DESCRIPTION = 'This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

