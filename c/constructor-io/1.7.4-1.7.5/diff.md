# Comparing `tmp/constructor-io-1.7.4.tar.gz` & `tmp/constructor-io-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constructor-io-1.7.4.tar", last modified: Fri May 12 17:11:00 2023, max compression
+gzip compressed data, was "constructor-io-1.7.5.tar", last modified: Tue May 30 17:20:00 2023, max compression
```

## Comparing `constructor-io-1.7.4.tar` & `constructor-io-1.7.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-05-12 17:11:00.988828 constructor-io-1.7.4/
--rw-r--r--   0 enes       (502) staff       (20)     1086 2021-09-21 17:57:12.000000 constructor-io-1.7.4/LICENSE
--rw-r--r--   0 enes       (502) staff       (20)     2562 2023-05-12 17:11:00.988656 constructor-io-1.7.4/PKG-INFO
--rw-r--r--   0 enes       (502) staff       (20)     2198 2022-10-03 13:13:47.000000 constructor-io-1.7.4/README.md
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-05-12 17:11:00.986181 constructor-io-1.7.4/constructor_io/
--rw-r--r--   0 enes       (502) staff       (20)       41 2023-05-12 17:10:46.000000 constructor-io-1.7.4/constructor_io/__init__.py
--rw-r--r--   0 enes       (502) staff       (20)     2324 2023-05-12 17:10:29.000000 constructor-io-1.7.4/constructor_io/constructor_io.py
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-05-12 17:11:00.987321 constructor-io-1.7.4/constructor_io/helpers/
--rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.7.4/constructor_io/helpers/__init__.py
--rw-r--r--   0 enes       (502) staff       (20)      481 2021-11-18 19:33:38.000000 constructor-io-1.7.4/constructor_io/helpers/exception.py
--rw-r--r--   0 enes       (502) staff       (20)     4795 2023-05-10 19:05:41.000000 constructor-io-1.7.4/constructor_io/helpers/utils.py
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-05-12 17:11:00.988435 constructor-io-1.7.4/constructor_io/modules/
--rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.7.4/constructor_io/modules/__init__.py
--rw-r--r--   0 enes       (502) staff       (20)     3976 2022-10-03 13:13:47.000000 constructor-io-1.7.4/constructor_io/modules/autocomplete.py
--rw-r--r--   0 enes       (502) staff       (20)    14881 2022-10-03 13:13:47.000000 constructor-io-1.7.4/constructor_io/modules/browse.py
--rw-r--r--   0 enes       (502) staff       (20)    17262 2022-10-21 17:16:45.000000 constructor-io-1.7.4/constructor_io/modules/catalog.py
--rw-r--r--   0 enes       (502) staff       (20)     6762 2023-04-13 18:25:13.000000 constructor-io-1.7.4/constructor_io/modules/quizzes.py
--rw-r--r--   0 enes       (502) staff       (20)     4167 2022-10-03 13:13:47.000000 constructor-io-1.7.4/constructor_io/modules/recommendations.py
--rw-r--r--   0 enes       (502) staff       (20)     4164 2023-05-10 18:53:45.000000 constructor-io-1.7.4/constructor_io/modules/search.py
--rw-r--r--   0 enes       (502) staff       (20)     3868 2022-11-08 15:58:41.000000 constructor-io-1.7.4/constructor_io/modules/tasks.py
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-05-12 17:11:00.986914 constructor-io-1.7.4/constructor_io.egg-info/
--rw-r--r--   0 enes       (502) staff       (20)     2562 2023-05-12 17:11:00.000000 constructor-io-1.7.4/constructor_io.egg-info/PKG-INFO
--rw-r--r--   0 enes       (502) staff       (20)      660 2023-05-12 17:11:00.000000 constructor-io-1.7.4/constructor_io.egg-info/SOURCES.txt
--rw-r--r--   0 enes       (502) staff       (20)        1 2023-05-12 17:11:00.000000 constructor-io-1.7.4/constructor_io.egg-info/dependency_links.txt
--rw-r--r--   0 enes       (502) staff       (20)       15 2023-05-12 17:11:00.000000 constructor-io-1.7.4/constructor_io.egg-info/requires.txt
--rw-r--r--   0 enes       (502) staff       (20)       15 2023-05-12 17:11:00.000000 constructor-io-1.7.4/constructor_io.egg-info/top_level.txt
--rw-r--r--   0 enes       (502) staff       (20)       38 2023-05-12 17:11:00.988880 constructor-io-1.7.4/setup.cfg
--rw-r--r--   0 enes       (502) staff       (20)      745 2022-01-10 22:25:09.000000 constructor-io-1.7.4/setup.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-05-30 17:20:00.168801 constructor-io-1.7.5/
+-rw-r--r--   0 enes       (502) staff       (20)     1086 2021-09-21 17:57:12.000000 constructor-io-1.7.5/LICENSE
+-rw-r--r--   0 enes       (502) staff       (20)     2562 2023-05-30 17:20:00.168579 constructor-io-1.7.5/PKG-INFO
+-rw-r--r--   0 enes       (502) staff       (20)     2198 2022-10-03 13:13:47.000000 constructor-io-1.7.5/README.md
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-05-30 17:20:00.165478 constructor-io-1.7.5/constructor_io/
+-rw-r--r--   0 enes       (502) staff       (20)       41 2023-05-30 17:19:55.000000 constructor-io-1.7.5/constructor_io/__init__.py
+-rw-r--r--   0 enes       (502) staff       (20)     2324 2023-05-12 17:10:29.000000 constructor-io-1.7.5/constructor_io/constructor_io.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-05-30 17:20:00.166871 constructor-io-1.7.5/constructor_io/helpers/
+-rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.7.5/constructor_io/helpers/__init__.py
+-rw-r--r--   0 enes       (502) staff       (20)      481 2021-11-18 19:33:38.000000 constructor-io-1.7.5/constructor_io/helpers/exception.py
+-rw-r--r--   0 enes       (502) staff       (20)     4795 2023-05-10 19:05:41.000000 constructor-io-1.7.5/constructor_io/helpers/utils.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-05-30 17:20:00.168317 constructor-io-1.7.5/constructor_io/modules/
+-rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.7.5/constructor_io/modules/__init__.py
+-rw-r--r--   0 enes       (502) staff       (20)     3976 2022-10-03 13:13:47.000000 constructor-io-1.7.5/constructor_io/modules/autocomplete.py
+-rw-r--r--   0 enes       (502) staff       (20)    14881 2022-10-03 13:13:47.000000 constructor-io-1.7.5/constructor_io/modules/browse.py
+-rw-r--r--   0 enes       (502) staff       (20)    17262 2022-10-21 17:16:45.000000 constructor-io-1.7.5/constructor_io/modules/catalog.py
+-rw-r--r--   0 enes       (502) staff       (20)     6762 2023-04-13 18:25:13.000000 constructor-io-1.7.5/constructor_io/modules/quizzes.py
+-rw-r--r--   0 enes       (502) staff       (20)     4167 2022-10-03 13:13:47.000000 constructor-io-1.7.5/constructor_io/modules/recommendations.py
+-rw-r--r--   0 enes       (502) staff       (20)     4164 2023-05-10 18:53:45.000000 constructor-io-1.7.5/constructor_io/modules/search.py
+-rw-r--r--   0 enes       (502) staff       (20)     3868 2022-11-08 15:58:41.000000 constructor-io-1.7.5/constructor_io/modules/tasks.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-05-30 17:20:00.166344 constructor-io-1.7.5/constructor_io.egg-info/
+-rw-r--r--   0 enes       (502) staff       (20)     2562 2023-05-30 17:20:00.000000 constructor-io-1.7.5/constructor_io.egg-info/PKG-INFO
+-rw-r--r--   0 enes       (502) staff       (20)      660 2023-05-30 17:20:00.000000 constructor-io-1.7.5/constructor_io.egg-info/SOURCES.txt
+-rw-r--r--   0 enes       (502) staff       (20)        1 2023-05-30 17:20:00.000000 constructor-io-1.7.5/constructor_io.egg-info/dependency_links.txt
+-rw-r--r--   0 enes       (502) staff       (20)       15 2023-05-30 17:20:00.000000 constructor-io-1.7.5/constructor_io.egg-info/requires.txt
+-rw-r--r--   0 enes       (502) staff       (20)       15 2023-05-30 17:20:00.000000 constructor-io-1.7.5/constructor_io.egg-info/top_level.txt
+-rw-r--r--   0 enes       (502) staff       (20)       38 2023-05-30 17:20:00.168876 constructor-io-1.7.5/setup.cfg
+-rw-r--r--   0 enes       (502) staff       (20)      745 2022-01-10 22:25:09.000000 constructor-io-1.7.5/setup.py
```

### Comparing `constructor-io-1.7.4/LICENSE` & `constructor-io-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.4/PKG-INFO` & `constructor-io-1.7.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: constructor-io
-Version: 1.7.4
+Version: 1.7.5
 Summary: Constructor.IO Python Client
 Home-page: https://www.constructor.io
 Author: Constructor.io
 Author-email: info@constructor.io
 License: MIT
-Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.7.4
+Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.7.5
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Constructor.io Python Client
 
 [![Version](https://img.shields.io/pypi/v/constructor-io.svg)](https://pypi.python.org/pypi/constructor-io)
```

### Comparing `constructor-io-1.7.4/README.md` & `constructor-io-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.4/constructor_io/constructor_io.py` & `constructor-io-1.7.5/constructor_io/constructor_io.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.4/constructor_io/helpers/utils.py` & `constructor-io-1.7.5/constructor_io/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.4/constructor_io/modules/autocomplete.py` & `constructor-io-1.7.5/constructor_io/modules/autocomplete.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.4/constructor_io/modules/browse.py` & `constructor-io-1.7.5/constructor_io/modules/browse.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.4/constructor_io/modules/catalog.py` & `constructor-io-1.7.5/constructor_io/modules/catalog.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.4/constructor_io/modules/quizzes.py` & `constructor-io-1.7.5/constructor_io/modules/quizzes.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.4/constructor_io/modules/recommendations.py` & `constructor-io-1.7.5/constructor_io/modules/recommendations.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.4/constructor_io/modules/search.py` & `constructor-io-1.7.5/constructor_io/modules/search.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.4/constructor_io/modules/tasks.py` & `constructor-io-1.7.5/constructor_io/modules/tasks.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.4/constructor_io.egg-info/PKG-INFO` & `constructor-io-1.7.5/constructor_io.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: constructor-io
-Version: 1.7.4
+Version: 1.7.5
 Summary: Constructor.IO Python Client
 Home-page: https://www.constructor.io
 Author: Constructor.io
 Author-email: info@constructor.io
 License: MIT
-Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.7.4
+Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.7.5
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Constructor.io Python Client
 
 [![Version](https://img.shields.io/pypi/v/constructor-io.svg)](https://pypi.python.org/pypi/constructor-io)
```

### Comparing `constructor-io-1.7.4/constructor_io.egg-info/SOURCES.txt` & `constructor-io-1.7.5/constructor_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.4/setup.py` & `constructor-io-1.7.5/setup.py`

 * *Files identical despite different names*

