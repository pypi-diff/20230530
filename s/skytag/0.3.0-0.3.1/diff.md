# Comparing `tmp/skytag-0.3.0.tar.gz` & `tmp/skytag-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytag-0.3.0.tar", last modified: Mon May 29 16:45:52 2023, max compression
+gzip compressed data, was "skytag-0.3.1.tar", last modified: Tue May 30 09:35:07 2023, max compression
```

## Comparing `skytag-0.3.0.tar` & `skytag-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 16:45:52.853198 skytag-0.3.0/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      307 2023-05-29 16:42:07.000000 skytag-0.3.0/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-05-29 16:42:07.000000 skytag-0.3.0/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-05-29 16:42:07.000000 skytag-0.3.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5022 2023-05-29 16:45:52.853198 skytag-0.3.0/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4387 2023-05-29 16:42:07.000000 skytag-0.3.0/README.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-05-29 16:45:52.853198 skytag-0.3.0/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1857 2023-05-29 16:42:07.000000 skytag-0.3.0/setup.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 16:45:52.849198 skytag-0.3.0/skytag/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      119 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4130 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 16:45:52.853198 skytag-0.3.0/skytag/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       94 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/commonutils/getpackagepath.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5118 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/commonutils/prob_at_location.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2059 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/default_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2058 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 16:45:52.853198 skytag-0.3.0/skytag.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5022 2023-05-29 16:45:52.000000 skytag-0.3.0/skytag.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      515 2023-05-29 16:45:52.000000 skytag-0.3.0/skytag.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-29 16:45:52.000000 skytag-0.3.0/skytag.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-05-29 16:45:52.000000 skytag-0.3.0/skytag.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-29 16:45:20.000000 skytag-0.3.0/skytag.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       57 2023-05-29 16:45:52.000000 skytag-0.3.0/skytag.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-05-29 16:45:52.000000 skytag-0.3.0/skytag.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-30 09:35:07.758383 skytag-0.3.1/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      307 2023-05-30 09:31:11.000000 skytag-0.3.1/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-05-30 09:31:11.000000 skytag-0.3.1/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-05-30 09:31:11.000000 skytag-0.3.1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5022 2023-05-30 09:35:07.758383 skytag-0.3.1/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4387 2023-05-30 09:31:11.000000 skytag-0.3.1/README.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-05-30 09:35:07.758383 skytag-0.3.1/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1857 2023-05-30 09:31:11.000000 skytag-0.3.1/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-30 09:35:07.758383 skytag-0.3.1/skytag/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      119 2023-05-30 09:31:11.000000 skytag-0.3.1/skytag/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-05-30 09:31:11.000000 skytag-0.3.1/skytag/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4622 2023-05-30 09:31:11.000000 skytag-0.3.1/skytag/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-30 09:35:07.758383 skytag-0.3.1/skytag/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       94 2023-05-30 09:31:11.000000 skytag-0.3.1/skytag/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-05-30 09:31:11.000000 skytag-0.3.1/skytag/commonutils/getpackagepath.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6449 2023-05-30 09:31:11.000000 skytag-0.3.1/skytag/commonutils/prob_at_location.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2059 2023-05-30 09:31:11.000000 skytag-0.3.1/skytag/default_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-05-30 09:31:11.000000 skytag-0.3.1/skytag/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2058 2023-05-30 09:31:11.000000 skytag-0.3.1/skytag/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-05-30 09:31:11.000000 skytag-0.3.1/skytag/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-30 09:35:07.758383 skytag-0.3.1/skytag.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5022 2023-05-30 09:35:07.000000 skytag-0.3.1/skytag.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      515 2023-05-30 09:35:07.000000 skytag-0.3.1/skytag.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-30 09:35:07.000000 skytag-0.3.1/skytag.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-05-30 09:35:07.000000 skytag-0.3.1/skytag.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-30 09:34:30.000000 skytag-0.3.1/skytag.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       57 2023-05-30 09:35:07.000000 skytag-0.3.1/skytag.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-05-30 09:35:07.000000 skytag-0.3.1/skytag.egg-info/top_level.txt
```

### Comparing `skytag-0.3.0/LICENSE` & `skytag-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skytag-0.3.0/PKG-INFO` & `skytag-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: skytag
-Version: 0.3.0
-Summary: Annotate transient sources or galaxies with the percentage credibility region they reside within on a given HealPix sky map.
-Home-page: https://github.com/thespacedoctor/skytag
-Download-URL: https://github.com/thespacedoctor/skytag/archive/v0.3.0.zip
-Author: David Young
-Author-email: d.r.young@qub.ac.uk
-License: MIT
-Keywords: astronomy
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # skytag
 
 [![](https://zenodo.org/badge/633485720.svg)](https://zenodo.org/badge/latestdoi/633485720) 
 
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/skytag)](https://pypi.org/project/skytag/)
```

### Comparing `skytag-0.3.0/README.md` & `skytag-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: skytag
+Version: 0.3.1
+Summary: Annotate transient sources or galaxies with the percentage credibility region they reside within on a given HealPix sky map.
+Home-page: https://github.com/thespacedoctor/skytag
+Download-URL: https://github.com/thespacedoctor/skytag/archive/v0.3.1.zip
+Author: David Young
+Author-email: d.r.young@qub.ac.uk
+License: MIT
+Keywords: astronomy
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # skytag
 
 [![](https://zenodo.org/badge/633485720.svg)](https://zenodo.org/badge/latestdoi/633485720) 
 
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/skytag)](https://pypi.org/project/skytag/)
```

### Comparing `skytag-0.3.0/setup.py` & `skytag-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `skytag-0.3.0/skytag/cl_utils.py` & `skytag-0.3.1/skytag/cl_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python
 # encoding: utf-8
 """
 Documentation for skytag can be found here: http://skytag.readthedocs.org
 
 Usage:
     skytag init
-    skytag <ra> <dec> <mapPath>
-    skytag <ra> <dec> <mjd> <mapPath>
+    skytag [-d] <ra> <dec> <mapPath>
+    skytag [-d] <ra> <dec> <mjd> <mapPath>
 
 Options:
     init                                   setup the skytag settings file for the first time
     <ra>                                   sky location right-ascension (decimal degrees or sexegesimal)
     <dec>                                  sky location declination (decimal degrees or sexegesimal)
     <mjd>                                  a transient event MJD. If supplied, a time delta from the map event is returned alongside probability.
     <mapPath>                              path to a HealPix skymap
+    -d, --distance                         also return a distance (and error) at the sky location
     -h, --help                             show this help message
     -v, --version                          show version
     -s, --settings <pathToSettingsFile>    the settings file
 """
 from subprocess import Popen, PIPE, STDOUT
 from fundamentals import tools, times
 from docopt import docopt
@@ -86,41 +87,58 @@
             cmd = """start %(filepath)s""" % locals()
             p = Popen(cmd, stdout=PIPE, stderr=PIPE, shell=True)
         except:
             pass
         return
 
     if a["mjd"]:
-        from skytag.commonutils import prob_at_location
-        prob, deltas = prob_at_location(
-            log=log,
-            ra=float(a["ra"]),
-            dec=float(a["dec"]),
-            mjd=float(a["mjd"]),
-            mapPath=a["mapPath"]
-        )
+        mjd = float(a["mjd"])
+    else:
+        mjd = False
+
+    if a["distanceFlag"]:
+        distance = True
+    else:
+        distance = False
+
+    from skytag.commonutils import prob_at_location
+    results = prob_at_location(
+        log=log,
+        ra=float(a["ra"]),
+        dec=float(a["dec"]),
+        mjd=mjd,
+        mapPath=a["mapPath"],
+        distance=distance
+    )
+
+    prob = results[0]
+    reportText = f"This transient is found in the {prob[0]}% credibility region"
 
+    if a["mjd"]:
+        deltas = results[1]
         if deltas[0] < 0.:
             preposition = "before"
         else:
             preposition = "after"
+        reportText += f" and occurred {deltas[0]} days {preposition} the map event."
+    if a["distanceFlag"]:
+        if not a["mjd"]:
+            distance = results[1]
+            reportText += "."
+        else:
+            distance = results[2]
+        if not distance[0][0]:
+            reportText += f" Burst events have no distance localisation."
+        else:
+            reportText += f" At this sky-position the map event is localised to a distance of {distance[0][0]} (±{distance[0][1]}) Mpc."
 
-        print(f"This transient is found in the {prob[0]}% credibility region, and occurred {deltas[0]} days {preposition} the map event.")
-
-    else:
-        # CALL FUNCTIONS/OBJECTS
-        from skytag.commonutils import prob_at_location
-        prob = prob_at_location(
-            log=log,
-            ra=float(a["ra"]),
-            dec=float(a["dec"]),
-            mapPath=a["mapPath"]
-        )[0]
+    if not a["mjd"] and not a["distanceFlag"]:
+        reportText += "."
 
-        print(f"This location is found in the {prob}% credibility region of the map.")
+    print(reportText)
 
     ## FINISH LOGGING ##
     endTime = times.get_now_sql_datetime()
     runningTime = times.calculate_time_difference(startTime, endTime)
     log.info('-- FINISHED ATTEMPT TO RUN THE cl_utils.py AT %s (RUNTIME: %s) --' %
              (endTime, runningTime, ))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `skytag-0.3.0/skytag/default_settings.yaml` & `skytag-0.3.1/skytag/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `skytag-0.3.0/skytag/setup.cfg` & `skytag-0.3.1/skytag/setup.cfg`

 * *Files identical despite different names*

### Comparing `skytag-0.3.0/skytag/test_settings.yaml` & `skytag-0.3.1/skytag/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `skytag-0.3.0/skytag/utKit.py` & `skytag-0.3.1/skytag/utKit.py`

 * *Files identical despite different names*

### Comparing `skytag-0.3.0/skytag.egg-info/PKG-INFO` & `skytag-0.3.1/skytag.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: skytag
-Version: 0.3.0
+Version: 0.3.1
 Summary: Annotate transient sources or galaxies with the percentage credibility region they reside within on a given HealPix sky map.
 Home-page: https://github.com/thespacedoctor/skytag
-Download-URL: https://github.com/thespacedoctor/skytag/archive/v0.3.0.zip
+Download-URL: https://github.com/thespacedoctor/skytag/archive/v0.3.1.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `skytag-0.3.0/skytag.egg-info/SOURCES.txt` & `skytag-0.3.1/skytag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

