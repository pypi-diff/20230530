# Comparing `tmp/gkligo-0.1.5.tar.gz` & `tmp/gkligo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gkligo-0.1.5.tar", last modified: Mon May 29 10:38:13 2023, max compression
+gzip compressed data, was "gkligo-0.1.6.tar", last modified: Mon May 29 23:27:01 2023, max compression
```

## Comparing `gkligo-0.1.5.tar` & `gkligo-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 10:38:13.812732 gkligo-0.1.5/
--rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.1.5/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-29 10:38:13.812342 gkligo-0.1.5/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)     1089 2023-05-24 11:09:44.000000 gkligo-0.1.5/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 10:38:13.800592 gkligo-0.1.5/gkligo/
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 14:27:19.000000 gkligo-0.1.5/gkligo/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-05-29 10:37:37.000000 gkligo-0.1.5/gkligo/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 10:38:13.803629 gkligo-0.1.5/gkligo/scripts/
--rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.1.5/gkligo/scripts/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 10:38:13.811121 gkligo-0.1.5/gkligo/scripts/python/
--rw-r--r--   0 kws        (502) staff       (20)        0 2023-05-28 12:23:50.000000 gkligo-0.1.5/gkligo/scripts/python/=
--rw-r--r--   0 kws        (502) staff       (20)       31 2023-04-28 14:27:05.000000 gkligo-0.1.5/gkligo/scripts/python/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.1.5/gkligo/scripts/python/config_download_example.yaml
--rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.1.5/gkligo/scripts/python/config_reports.yaml
--rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.1.5/gkligo/scripts/python/config_reports_example.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)    12905 2023-05-29 10:37:37.000000 gkligo-0.1.5/gkligo/scripts/python/downloadGWAlerts.py
--rwxr-xr-x   0 kws        (502) staff       (20)     5793 2023-05-26 22:32:11.000000 gkligo-0.1.5/gkligo/scripts/python/generateGWReports.py
--rw-r--r--   0 kws        (502) staff       (20)      267 2023-05-26 22:38:03.000000 gkligo-0.1.5/gkligo/scripts/python/test.py
--rw-r--r--   0 kws        (502) staff       (20)     1266 2023-05-23 20:34:59.000000 gkligo-0.1.5/gkligo/scripts/python/test.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.1.5/gkligo/scripts/python/testDaemon.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 10:38:13.803205 gkligo-0.1.5/gkligo.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-29 10:38:13.000000 gkligo-0.1.5/gkligo.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      664 2023-05-29 10:38:13.000000 gkligo-0.1.5/gkligo.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2023-05-29 10:38:13.000000 gkligo-0.1.5/gkligo.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)      147 2023-05-29 10:38:13.000000 gkligo-0.1.5/gkligo.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       85 2023-05-29 10:38:13.000000 gkligo-0.1.5/gkligo.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        7 2023-05-29 10:38:13.000000 gkligo-0.1.5/gkligo.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2023-05-29 10:38:13.812947 gkligo-0.1.5/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.1.5/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 23:27:01.157066 gkligo-0.1.6/
+-rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.1.6/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-29 23:27:01.156579 gkligo-0.1.6/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)     1089 2023-05-24 11:09:44.000000 gkligo-0.1.6/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 23:27:01.143845 gkligo-0.1.6/gkligo/
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 14:27:19.000000 gkligo-0.1.6/gkligo/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-05-29 23:26:40.000000 gkligo-0.1.6/gkligo/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 23:27:01.146783 gkligo-0.1.6/gkligo/scripts/
+-rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.1.6/gkligo/scripts/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 23:27:01.155458 gkligo-0.1.6/gkligo/scripts/python/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2023-05-28 12:23:50.000000 gkligo-0.1.6/gkligo/scripts/python/=
+-rw-r--r--   0 kws        (502) staff       (20)       31 2023-04-28 14:27:05.000000 gkligo-0.1.6/gkligo/scripts/python/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.1.6/gkligo/scripts/python/config_download_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.1.6/gkligo/scripts/python/config_reports.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.1.6/gkligo/scripts/python/config_reports_example.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)    13101 2023-05-29 23:26:40.000000 gkligo-0.1.6/gkligo/scripts/python/downloadGWAlerts.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     5793 2023-05-26 22:32:11.000000 gkligo-0.1.6/gkligo/scripts/python/generateGWReports.py
+-rw-r--r--   0 kws        (502) staff       (20)      267 2023-05-29 14:39:19.000000 gkligo-0.1.6/gkligo/scripts/python/test.py
+-rw-r--r--   0 kws        (502) staff       (20)     1266 2023-05-23 20:34:59.000000 gkligo-0.1.6/gkligo/scripts/python/test.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.1.6/gkligo/scripts/python/testDaemon.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 23:27:01.146362 gkligo-0.1.6/gkligo.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-29 23:27:01.000000 gkligo-0.1.6/gkligo.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      664 2023-05-29 23:27:01.000000 gkligo-0.1.6/gkligo.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2023-05-29 23:27:01.000000 gkligo-0.1.6/gkligo.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      147 2023-05-29 23:27:01.000000 gkligo-0.1.6/gkligo.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       85 2023-05-29 23:27:01.000000 gkligo-0.1.6/gkligo.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        7 2023-05-29 23:27:01.000000 gkligo-0.1.6/gkligo.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2023-05-29 23:27:01.157322 gkligo-0.1.6/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.1.6/setup.py
```

### Comparing `gkligo-0.1.5/PKG-INFO` & `gkligo-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.1.5
+Version: 0.1.6
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # gkligo
         Code to download GW Alert skymaps from Kafka, and optionally write them
```

### Comparing `gkligo-0.1.5/README.md` & `gkligo-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.5/gkligo/scripts/python/downloadGWAlerts.py` & `gkligo-0.1.6/gkligo/scripts/python/downloadGWAlerts.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,15 @@
 def writeMeta(options, dataDict, logger):
     #import MySQLdb
     from astropy.io import fits
 
     mjd = None
     distance = None
     distanceStd = None
+    creator = None
     eventMeta = {}
 
     dataDictCopy = deepcopy(dataDict)
     skymap = dataDictCopy['event']['skymap']
 
     areas = {}
     for c in options.contours.split(','):
@@ -183,14 +184,19 @@
         logger.error("The DISTMEAN variable is missing.")
 
     try:
         distanceStd = header['DISTSTD']
     except KeyError as e:
         logger.error("The DISTSTD variable is missing.")
 
+    try:
+        creator = header['CREATOR']
+    except KeyError as e:
+        logger.error("The CREATOR variable is missing.")
+
     # Do NOT write to the database, which could potentially be locked and crash the
     # daemon. Write another script (e.g the reports script) that does that. Just
     # record the metadata for loading.
 
 
     # Remove the skymap from the dictionary.
     try:
@@ -203,15 +209,16 @@
     except KeyError as e:
         pass
 
     eventMeta = {'ALERT': dataDictCopy,
                  'EXTRA': areas,
                  'HEADER': {'MJD-OBS': mjd,
                             'DISTMEAN': distance,
-                            'DISTSTD': distanceStd}}
+                            'DISTSTD': distanceStd,
+                            'CREATOR': creator}}
 
     return eventMeta
 
  
 def listen(options):
     """listen.
```

### Comparing `gkligo-0.1.5/gkligo/scripts/python/generateGWReports.py` & `gkligo-0.1.6/gkligo/scripts/python/generateGWReports.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.5/gkligo/scripts/python/test.yaml` & `gkligo-0.1.6/gkligo/scripts/python/test.yaml`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.5/gkligo/scripts/python/testDaemon.py` & `gkligo-0.1.6/gkligo/scripts/python/testDaemon.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.5/gkligo.egg-info/PKG-INFO` & `gkligo-0.1.6/gkligo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.1.5
+Version: 0.1.6
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # gkligo
         Code to download GW Alert skymaps from Kafka, and optionally write them
```

### Comparing `gkligo-0.1.5/gkligo.egg-info/SOURCES.txt` & `gkligo-0.1.6/gkligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.5/setup.py` & `gkligo-0.1.6/setup.py`

 * *Files identical despite different names*

