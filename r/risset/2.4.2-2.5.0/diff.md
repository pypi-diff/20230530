# Comparing `tmp/risset-2.4.2.tar.gz` & `tmp/risset-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risset-2.4.2.tar", last modified: Sat Apr 15 23:15:34 2023, max compression
+gzip compressed data, was "risset-2.5.0.tar", last modified: Tue May 30 17:48:32 2023, max compression
```

## Comparing `risset-2.4.2.tar` & `risset-2.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-15 23:15:34.655872 risset-2.4.2/
--rw-rw-r--   0 em        (1000) em        (1000)     5664 2023-04-15 23:15:34.654872 risset-2.4.2/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     5349 2023-04-13 00:18:38.000000 risset-2.4.2/README.md
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-15 23:15:34.654872 risset-2.4.2/risset.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     5664 2023-04-15 23:15:34.000000 risset-2.4.2/risset.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-15 23:15:34.000000 risset-2.4.2/risset.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-15 23:15:34.000000 risset-2.4.2/risset.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       40 2023-04-15 23:15:34.000000 risset-2.4.2/risset.egg-info/entry_points.txt
--rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-15 23:15:34.000000 risset-2.4.2/risset.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-15 23:15:34.000000 risset-2.4.2/risset.egg-info/top_level.txt
--rwxrwxr-x   0 em        (1000) em        (1000)   108080 2023-04-15 23:08:22.000000 risset-2.4.2/risset.py
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-15 23:15:34.655872 risset-2.4.2/setup.cfg
--rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-12 12:16:30.000000 risset-2.4.2/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-30 17:48:32.253076 risset-2.5.0/
+-rw-rw-r--   0 em        (1000) em        (1000)     5627 2023-05-30 17:48:32.253076 risset-2.5.0/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     5349 2023-04-13 00:18:38.000000 risset-2.5.0/README.md
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-30 17:48:32.253076 risset-2.5.0/risset.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     5627 2023-05-30 17:48:32.000000 risset-2.5.0/risset.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      210 2023-05-30 17:48:32.000000 risset-2.5.0/risset.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-05-30 17:48:32.000000 risset-2.5.0/risset.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       39 2023-05-30 17:48:32.000000 risset-2.5.0/risset.egg-info/entry_points.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       33 2023-05-30 17:48:32.000000 risset-2.5.0/risset.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        7 2023-05-30 17:48:32.000000 risset-2.5.0/risset.egg-info/top_level.txt
+-rwxrwxr-x   0 em        (1000) em        (1000)   108137 2023-05-30 17:48:09.000000 risset-2.5.0/risset.py
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-05-30 17:48:32.253076 risset-2.5.0/setup.cfg
+-rw-rw-r--   0 em        (1000) em        (1000)      915 2023-05-30 17:47:51.000000 risset-2.5.0/setup.py
```

### Comparing `risset-2.4.2/PKG-INFO` & `risset-2.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: risset
-Version: 2.4.2
+Version: 2.5.0
 Summary: A package manager for csound
 Home-page: https://github.com/csound-plugins/risset
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ![risset](assets/risset-title.png)
 
 # risset: a package manager for csound
 
@@ -206,9 +204,7 @@
 
 ## Manifest
 
 Each plugin has an accompanying manifest in the .json format. The name of this file
 is always `risset.json`
 See one of the examples in https://github.com/csound-plugins/csound-plugins/tree/master/src for
 more information about the manifest
-
-
```

### Comparing `risset-2.4.2/README.md` & `risset-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `risset-2.4.2/risset.egg-info/PKG-INFO` & `risset-2.5.0/risset.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: risset
-Version: 2.4.2
+Version: 2.5.0
 Summary: A package manager for csound
 Home-page: https://github.com/csound-plugins/risset
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ![risset](assets/risset-title.png)
 
 # risset: a package manager for csound
 
@@ -206,9 +204,7 @@
 
 ## Manifest
 
 Each plugin has an accompanying manifest in the .json format. The name of this file
 is always `risset.json`
 See one of the examples in https://github.com/csound-plugins/csound-plugins/tree/master/src for
 more information about the manifest
-
-
```

### Comparing `risset-2.4.2/risset.py` & `risset-2.5.0/risset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
-__version__ = "2.4.2"
+__version__ = "2.5.0"
 
 import sys
 
 if (sys.version_info.major, sys.version_info.minor) < (3, 8):
     print("Python 3.8 or higher is needed", file=sys.stderr)
     sys.exit(-1)
 
@@ -2696,14 +2696,15 @@
         lastupdate = 99999999
     else:
         import time
         lastupdate = int((time.time() - picklefile.stat().st_mtime) / 686400)
 
     d = {
         'version': idx.version,
+        'pluginspath': idx.user_plugins_path.as_posix(),
         'rissetroot': RISSET_ROOT.as_posix(),
         'clonespath': RISSET_CLONES_PATH.as_posix(),
         'assetspath': RISSET_ASSETS_PATH.as_posix(),
         'htmldocs': (RISSET_GENERATED_DOCS/"site").as_posix(),
         'manpages': (RISSET_GENERATED_DOCS/"docs/opcodes").as_posix(),
         'datarepo': RISSET_DATAREPO_LOCALPATH.as_posix(),
         'opcodesxml': (RISSET_ROOT / "opcodes.xml").as_posix(),
```

### Comparing `risset-2.4.2/setup.py` & `risset-2.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     long_description_content_type = 'text/markdown',
     py_modules=["risset"],
 
     url="https://github.com/csound-plugins/risset",
 
     install_requires=[
         'pygments',
-        'ctcsound7>=0.3.0'
+        'ctcsound7>=0.3.0',
+        'mkdocs'
     ],
 
     entry_points={
         "console_scripts": [
             "risset=risset:main",
         ]
     }
```

