# Comparing `tmp/mobilevids-dl-1.0.2.tar.gz` & `tmp/mobilevids-dl-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobilevids-dl-1.0.2.tar", last modified: Tue Apr  4 13:48:50 2023, max compression
+gzip compressed data, was "mobilevids-dl-1.0.3.tar", last modified: Tue May 30 21:21:30 2023, max compression
```

## Comparing `mobilevids-dl-1.0.2.tar` & `mobilevids-dl-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:48:50.305006 mobilevids-dl-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-04 13:48:39.000000 mobilevids-dl-1.0.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-04 13:48:39.000000 mobilevids-dl-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-04 13:48:39.000000 mobilevids-dl-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-04-04 13:48:50.305006 mobilevids-dl-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-04 13:48:39.000000 mobilevids-dl-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:48:50.301006 mobilevids-dl-1.0.2/mobilevids/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-04 13:48:39.000000 mobilevids-dl-1.0.2/mobilevids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-04 13:48:39.000000 mobilevids-dl-1.0.2/mobilevids/define.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1121 2023-04-04 13:48:39.000000 mobilevids-dl-1.0.2/mobilevids/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-04 13:48:39.000000 mobilevids-dl-1.0.2/mobilevids/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-04 13:48:39.000000 mobilevids-dl-1.0.2/mobilevids/imagetoascii.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-04 13:48:39.000000 mobilevids-dl-1.0.2/mobilevids/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-04 13:48:39.000000 mobilevids-dl-1.0.2/mobilevids/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:48:50.305006 mobilevids-dl-1.0.2/mobilevids_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-04-04 13:48:50.000000 mobilevids-dl-1.0.2/mobilevids_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-04 13:48:50.000000 mobilevids-dl-1.0.2/mobilevids_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 13:48:50.000000 mobilevids-dl-1.0.2/mobilevids_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-04 13:48:50.000000 mobilevids-dl-1.0.2/mobilevids_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-04 13:48:50.000000 mobilevids-dl-1.0.2/mobilevids_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-04 13:48:50.000000 mobilevids-dl-1.0.2/mobilevids_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-04 13:48:39.000000 mobilevids-dl-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 13:48:50.305006 mobilevids-dl-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-04 13:48:39.000000 mobilevids-dl-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:21:30.175266 mobilevids-dl-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-30 21:21:30.171265 mobilevids-dl-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:21:30.171265 mobilevids-dl-1.0.3/mobilevids/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/define.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1121 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/imagetoascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:21:30.171265 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-30 21:21:30.000000 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-30 21:21:30.000000 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:21:30.000000 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 21:21:30.000000 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-30 21:21:30.000000 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 21:21:30.000000 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:21:30.175266 mobilevids-dl-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/setup.py
```

### Comparing `mobilevids-dl-1.0.2/AUTHORS.md` & `mobilevids-dl-1.0.3/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.2/LICENSE` & `mobilevids-dl-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.2/PKG-INFO` & `mobilevids-dl-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobilevids-dl
-Version: 1.0.2
+Version: 1.0.3
 Summary: Script for downloading Movies and Shows from mobilevids.org
 Home-page: https://github.com/ahron-maslin/mobilevids-dl
 Maintainer: Aharon Maslin
 Maintainer-email: aronmas613@gmail.com
 License: LGPL
 Keywords: mpbilevids-dl,mobilevids,download,entertainment,video
 Platform: any
```

### Comparing `mobilevids-dl-1.0.2/README.rst` & `mobilevids-dl-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.2/mobilevids/define.py` & `mobilevids-dl-1.0.3/mobilevids/define.py`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.2/mobilevids/dispatcher.py` & `mobilevids-dl-1.0.3/mobilevids/dispatcher.py`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.2/mobilevids/downloader.py` & `mobilevids-dl-1.0.3/mobilevids/downloader.py`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.2/mobilevids/imagetoascii.py` & `mobilevids-dl-1.0.3/mobilevids/imagetoascii.py`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.2/mobilevids/network.py` & `mobilevids-dl-1.0.3/mobilevids/network.py`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.2/mobilevids/options.py` & `mobilevids-dl-1.0.3/mobilevids/options.py`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.2/mobilevids_dl.egg-info/PKG-INFO` & `mobilevids-dl-1.0.3/mobilevids_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobilevids-dl
-Version: 1.0.2
+Version: 1.0.3
 Summary: Script for downloading Movies and Shows from mobilevids.org
 Home-page: https://github.com/ahron-maslin/mobilevids-dl
 Maintainer: Aharon Maslin
 Maintainer-email: aronmas613@gmail.com
 License: LGPL
 Keywords: mpbilevids-dl,mobilevids,download,entertainment,video
 Platform: any
```

### Comparing `mobilevids-dl-1.0.2/setup.py` & `mobilevids-dl-1.0.3/setup.py`

 * *Files identical despite different names*

