# Comparing `tmp/stups-kio-0.1.8.tar.gz` & `tmp/stups-kio-0.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stups-kio-0.1.8.tar", last modified: Fri Nov 20 09:54:26 2015, max compression
+gzip compressed data, was "dist/stups-kio-0.1.post3.tar", last modified: Wed Nov 11 11:14:19 2015, max compression
```

## Comparing `stups-kio-0.1.8.tar` & `stups-kio-0.1.post3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 hjacobs   (1000) hjacobs   (1000)        0 2015-11-20 09:54:26.000000 stups-kio-0.1.8/
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)       67 2015-11-19 20:38:22.000000 stups-kio-0.1.8/requirements.txt
-drwxrwxr-x   0 hjacobs   (1000) hjacobs   (1000)        0 2015-11-20 09:54:26.000000 stups-kio-0.1.8/stups_kio.egg-info/
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)        4 2015-11-20 09:54:26.000000 stups-kio-0.1.8/stups_kio.egg-info/top_level.txt
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)     2427 2015-11-20 09:54:26.000000 stups-kio-0.1.8/stups_kio.egg-info/PKG-INFO
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)      314 2015-11-20 09:54:26.000000 stups-kio-0.1.8/stups_kio.egg-info/SOURCES.txt
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)       67 2015-11-20 09:54:26.000000 stups-kio-0.1.8/stups_kio.egg-info/requires.txt
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)       38 2015-11-20 09:54:26.000000 stups-kio-0.1.8/stups_kio.egg-info/entry_points.txt
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)        1 2015-11-20 09:54:26.000000 stups-kio-0.1.8/stups_kio.egg-info/dependency_links.txt
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)       55 2015-11-10 13:14:15.000000 stups-kio-0.1.8/MANIFEST.in
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)     2427 2015-11-20 09:54:26.000000 stups-kio-0.1.8/PKG-INFO
-drwxrwxr-x   0 hjacobs   (1000) hjacobs   (1000)        0 2015-11-20 09:54:26.000000 stups-kio-0.1.8/kio/
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)       22 2015-11-20 09:54:22.000000 stups-kio-0.1.8/kio/__init__.py
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)     7410 2015-11-19 20:38:03.000000 stups-kio-0.1.8/kio/cli.py
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)     1908 2015-11-13 12:27:35.000000 stups-kio-0.1.8/kio/time.py
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)       64 2015-11-10 13:18:03.000000 stups-kio-0.1.8/kio/__main__.py
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)      430 2015-09-14 13:50:34.000000 stups-kio-0.1.8/kio/api.py
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)     4432 2015-11-10 13:17:03.000000 stups-kio-0.1.8/setup.py
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)     1169 2015-11-10 13:16:32.000000 stups-kio-0.1.8/README.rst
--rw-rw-r--   0 hjacobs   (1000) hjacobs   (1000)       59 2015-11-20 09:54:26.000000 stups-kio-0.1.8/setup.cfg
+drwxrwxr-x   0 go         (106) go         (111)        0 2015-11-11 11:14:19.000000 stups-kio-0.1.post3/
+drwxrwxr-x   0 go         (106) go         (111)        0 2015-11-11 11:14:19.000000 stups-kio-0.1.post3/kio/
+-rw-rw-r--   0 go         (106) go         (111)      430 2015-11-11 11:14:14.000000 stups-kio-0.1.post3/kio/api.py
+-rw-rw-r--   0 go         (106) go         (111)       22 2015-11-11 11:14:16.000000 stups-kio-0.1.post3/kio/__init__.py
+-rw-rw-r--   0 go         (106) go         (111)       64 2015-11-11 11:14:14.000000 stups-kio-0.1.post3/kio/__main__.py
+-rw-rw-r--   0 go         (106) go         (111)     1889 2015-11-11 11:14:14.000000 stups-kio-0.1.post3/kio/time.py
+-rw-rw-r--   0 go         (106) go         (111)     4544 2015-11-11 11:14:14.000000 stups-kio-0.1.post3/kio/cli.py
+-rw-rw-r--   0 go         (106) go         (111)       65 2015-11-11 11:14:14.000000 stups-kio-0.1.post3/requirements.txt
+-rw-rw-r--   0 go         (106) go         (111)       55 2015-11-11 11:14:14.000000 stups-kio-0.1.post3/MANIFEST.in
+-rw-rw-r--   0 go         (106) go         (111)       59 2015-11-11 11:14:19.000000 stups-kio-0.1.post3/setup.cfg
+drwxrwxr-x   0 go         (106) go         (111)        0 2015-11-11 11:14:19.000000 stups-kio-0.1.post3/stups_kio.egg-info/
+-rw-rw-r--   0 go         (106) go         (111)       65 2015-11-11 11:14:19.000000 stups-kio-0.1.post3/stups_kio.egg-info/requires.txt
+-rw-rw-r--   0 go         (106) go         (111)       38 2015-11-11 11:14:19.000000 stups-kio-0.1.post3/stups_kio.egg-info/entry_points.txt
+-rw-rw-r--   0 go         (106) go         (111)      314 2015-11-11 11:14:19.000000 stups-kio-0.1.post3/stups_kio.egg-info/SOURCES.txt
+-rw-rw-r--   0 go         (106) go         (111)        1 2015-11-11 11:14:19.000000 stups-kio-0.1.post3/stups_kio.egg-info/dependency_links.txt
+-rw-rw-r--   0 go         (106) go         (111)        4 2015-11-11 11:14:19.000000 stups-kio-0.1.post3/stups_kio.egg-info/top_level.txt
+-rw-rw-r--   0 go         (106) go         (111)     2431 2015-11-11 11:14:19.000000 stups-kio-0.1.post3/stups_kio.egg-info/PKG-INFO
+-rw-rw-r--   0 go         (106) go         (111)     2431 2015-11-11 11:14:19.000000 stups-kio-0.1.post3/PKG-INFO
+-rw-rw-r--   0 go         (106) go         (111)     1169 2015-11-11 11:14:14.000000 stups-kio-0.1.post3/README.rst
+-rw-rw-r--   0 go         (106) go         (111)     4432 2015-11-11 11:14:14.000000 stups-kio-0.1.post3/setup.py
```

### Comparing `stups-kio-0.1.8/stups_kio.egg-info/PKG-INFO` & `stups-kio-0.1.post3/stups_kio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: stups-kio
-Version: 0.1.8
+Version: 0.1.post3
 Summary: Simple command line utility to manage Kio applications and application versions
 Home-page: https://github.com/zalando-stups/kio-cli
 Author: Henning Jacobs
 Author-email: henning.jacobs@zalando.de
 License: Apache License 2.0
 Description: =======
         Kio CLI
```

### Comparing `stups-kio-0.1.8/PKG-INFO` & `stups-kio-0.1.post3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: stups-kio
-Version: 0.1.8
+Version: 0.1.post3
 Summary: Simple command line utility to manage Kio applications and application versions
 Home-page: https://github.com/zalando-stups/kio-cli
 Author: Henning Jacobs
 Author-email: henning.jacobs@zalando.de
 License: Apache License 2.0
 Description: =======
         Kio CLI
```

### Comparing `stups-kio-0.1.8/kio/time.py` & `stups-kio-0.1.post3/kio/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 import re
 
 TIME_UNITS = {
     's': 'seconds',
     'm': 'minutes',
     'h': 'hours',
     'd': 'days',
-    'w': 'weeks',
 }
 
 TIME_PATTERN = \
     re.compile(r"""
     (?x)
     ^
     (?:
         (?P<magnitude> [+-]? \d+ )
-        (?P<unit> [smhdw] )
+        (?P<unit> [smhd] )
     |
         (?P<isodate> \d{4} - \d{2} - \d{2} (?: [ ] \d{2} : \d{2} : \d{2} (?: \. \d+)? ) )
     )
     $
     """
                )
```

### Comparing `stups-kio-0.1.8/setup.py` & `stups-kio-0.1.post3/setup.py`

 * *Files identical despite different names*

### Comparing `stups-kio-0.1.8/README.rst` & `stups-kio-0.1.post3/README.rst`

 * *Files identical despite different names*

