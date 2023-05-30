# Comparing `tmp/casaconfig-0.0.8.tar.gz` & `tmp/casaconfig-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casaconfig-0.0.8.tar", last modified: Tue Oct 26 20:56:53 2021, max compression
+gzip compressed data, was "casaconfig-0.0.9.tar", last modified: Thu Oct 28 14:38:25 2021, max compression
```

## Comparing `casaconfig-0.0.8.tar` & `casaconfig-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 raba      (1000) raba      (1000)        0 2021-10-26 20:56:53.108431 casaconfig-0.0.8/
--rw-rw-r--   0 raba      (1000) raba      (1000)    11358 2021-10-19 17:29:59.000000 casaconfig-0.0.8/LICENSE
--rw-rw-r--   0 raba      (1000) raba      (1000)       39 2021-10-19 18:16:42.000000 casaconfig-0.0.8/MANIFEST.in
--rw-rw-r--   0 raba      (1000) raba      (1000)      583 2021-10-26 20:56:53.108431 casaconfig-0.0.8/PKG-INFO
--rw-rw-r--   0 raba      (1000) raba      (1000)      249 2021-10-19 17:29:59.000000 casaconfig-0.0.8/README.md
-drwxrwxr-x   0 raba      (1000) raba      (1000)        0 2021-10-26 20:56:53.100431 casaconfig-0.0.8/casaconfig/
--rw-rw-r--   0 raba      (1000) raba      (1000)    46036 2021-10-19 17:29:59.000000 casaconfig-0.0.8/casaconfig/JPLephem_reader2.py
-drwxrwxr-x   0 raba      (1000) raba      (1000)        0 2021-10-26 20:56:53.108431 casaconfig-0.0.8/casaconfig/__data__/
--rw-rw-r--   0 raba      (1000) raba      (1000)      295 2021-10-19 17:29:59.000000 casaconfig-0.0.8/casaconfig/__data__/README.txt
--rw-rw-r--   0 raba      (1000) raba      (1000)      379 2021-10-19 22:58:57.000000 casaconfig-0.0.8/casaconfig/__init__.py
--rw-rw-r--   0 raba      (1000) raba      (1000)     1555 2021-10-26 18:54:15.000000 casaconfig-0.0.8/casaconfig/config.py
--rw-rw-r--   0 raba      (1000) raba      (1000)     1021 2021-10-19 17:52:24.000000 casaconfig-0.0.8/casaconfig/get_data_dir.py
--rw-rw-r--   0 raba      (1000) raba      (1000)    18637 2021-10-19 17:29:59.000000 casaconfig-0.0.8/casaconfig/jplephem_request.py
--rw-rw-r--   0 raba      (1000) raba      (1000)     1254 2021-10-26 15:43:04.000000 casaconfig-0.0.8/casaconfig/measures_available.py
--rw-rw-r--   0 raba      (1000) raba      (1000)     4145 2021-10-26 18:37:06.000000 casaconfig-0.0.8/casaconfig/measures_update.py
--rw-rw-r--   0 raba      (1000) raba      (1000)     2459 2021-10-26 18:26:26.000000 casaconfig-0.0.8/casaconfig/pull_data.py
--rw-rw-r--   0 raba      (1000) raba      (1000)     1861 2021-10-19 18:04:29.000000 casaconfig-0.0.8/casaconfig/set_casacore_path.py
--rw-rw-r--   0 raba      (1000) raba      (1000)     4699 2021-10-26 20:55:55.000000 casaconfig-0.0.8/casaconfig/table_open.py
--rw-rw-r--   0 raba      (1000) raba      (1000)     1802 2021-10-19 23:10:38.000000 casaconfig-0.0.8/casaconfig/write_default_config.py
-drwxrwxr-x   0 raba      (1000) raba      (1000)        0 2021-10-26 20:56:53.104431 casaconfig-0.0.8/casaconfig.egg-info/
--rw-rw-r--   0 raba      (1000) raba      (1000)      583 2021-10-26 20:56:52.000000 casaconfig-0.0.8/casaconfig.egg-info/PKG-INFO
--rw-rw-r--   0 raba      (1000) raba      (1000)      550 2021-10-26 20:56:52.000000 casaconfig-0.0.8/casaconfig.egg-info/SOURCES.txt
--rw-rw-r--   0 raba      (1000) raba      (1000)        1 2021-10-26 20:56:52.000000 casaconfig-0.0.8/casaconfig.egg-info/dependency_links.txt
--rw-rw-r--   0 raba      (1000) raba      (1000)       73 2021-10-26 20:56:52.000000 casaconfig-0.0.8/casaconfig.egg-info/requires.txt
--rw-rw-r--   0 raba      (1000) raba      (1000)       11 2021-10-26 20:56:52.000000 casaconfig-0.0.8/casaconfig.egg-info/top_level.txt
--rw-rw-r--   0 raba      (1000) raba      (1000)       38 2021-10-26 20:56:53.108431 casaconfig-0.0.8/setup.cfg
--rw-rw-r--   0 raba      (1000) raba      (1000)      809 2021-10-26 20:44:25.000000 casaconfig-0.0.8/setup.py
+drwxrwxr-x   0 raba      (1000) raba      (1000)        0 2021-10-28 14:38:25.897653 casaconfig-0.0.9/
+-rw-rw-r--   0 raba      (1000) raba      (1000)    11358 2021-10-19 17:29:59.000000 casaconfig-0.0.9/LICENSE
+-rw-rw-r--   0 raba      (1000) raba      (1000)       39 2021-10-19 18:16:42.000000 casaconfig-0.0.9/MANIFEST.in
+-rw-rw-r--   0 raba      (1000) raba      (1000)      583 2021-10-28 14:38:25.897653 casaconfig-0.0.9/PKG-INFO
+-rw-rw-r--   0 raba      (1000) raba      (1000)      249 2021-10-19 17:29:59.000000 casaconfig-0.0.9/README.md
+drwxrwxr-x   0 raba      (1000) raba      (1000)        0 2021-10-28 14:38:25.897653 casaconfig-0.0.9/casaconfig/
+-rw-rw-r--   0 raba      (1000) raba      (1000)    46036 2021-10-19 17:29:59.000000 casaconfig-0.0.9/casaconfig/JPLephem_reader2.py
+drwxrwxr-x   0 raba      (1000) raba      (1000)        0 2021-10-28 14:38:25.897653 casaconfig-0.0.9/casaconfig/__data__/
+-rw-rw-r--   0 raba      (1000) raba      (1000)      295 2021-10-19 17:29:59.000000 casaconfig-0.0.9/casaconfig/__data__/README.txt
+-rw-rw-r--   0 raba      (1000) raba      (1000)      471 2021-10-28 14:26:44.000000 casaconfig-0.0.9/casaconfig/__init__.py
+-rw-rw-r--   0 raba      (1000) raba      (1000)     1555 2021-10-26 18:54:15.000000 casaconfig-0.0.9/casaconfig/config.py
+-rw-rw-r--   0 raba      (1000) raba      (1000)     1021 2021-10-19 17:52:24.000000 casaconfig-0.0.9/casaconfig/get_data_dir.py
+-rw-rw-r--   0 raba      (1000) raba      (1000)    18637 2021-10-19 17:29:59.000000 casaconfig-0.0.9/casaconfig/jplephem_request.py
+-rw-rw-r--   0 raba      (1000) raba      (1000)     1254 2021-10-26 15:43:04.000000 casaconfig-0.0.9/casaconfig/measures_available.py
+-rw-rw-r--   0 raba      (1000) raba      (1000)     4145 2021-10-26 18:37:06.000000 casaconfig-0.0.9/casaconfig/measures_update.py
+-rw-rw-r--   0 raba      (1000) raba      (1000)     2459 2021-10-26 18:26:26.000000 casaconfig-0.0.9/casaconfig/pull_data.py
+-rw-rw-r--   0 raba      (1000) raba      (1000)     1861 2021-10-19 18:04:29.000000 casaconfig-0.0.9/casaconfig/set_casacore_path.py
+-rw-rw-r--   0 raba      (1000) raba      (1000)     4699 2021-10-26 20:55:55.000000 casaconfig-0.0.9/casaconfig/table_open.py
+-rw-rw-r--   0 raba      (1000) raba      (1000)     1802 2021-10-19 23:10:38.000000 casaconfig-0.0.9/casaconfig/write_default_config.py
+drwxrwxr-x   0 raba      (1000) raba      (1000)        0 2021-10-28 14:38:25.897653 casaconfig-0.0.9/casaconfig.egg-info/
+-rw-rw-r--   0 raba      (1000) raba      (1000)      583 2021-10-28 14:38:25.000000 casaconfig-0.0.9/casaconfig.egg-info/PKG-INFO
+-rw-rw-r--   0 raba      (1000) raba      (1000)      550 2021-10-28 14:38:25.000000 casaconfig-0.0.9/casaconfig.egg-info/SOURCES.txt
+-rw-rw-r--   0 raba      (1000) raba      (1000)        1 2021-10-28 14:38:25.000000 casaconfig-0.0.9/casaconfig.egg-info/dependency_links.txt
+-rw-rw-r--   0 raba      (1000) raba      (1000)       73 2021-10-28 14:38:25.000000 casaconfig-0.0.9/casaconfig.egg-info/requires.txt
+-rw-rw-r--   0 raba      (1000) raba      (1000)       11 2021-10-28 14:38:25.000000 casaconfig-0.0.9/casaconfig.egg-info/top_level.txt
+-rw-rw-r--   0 raba      (1000) raba      (1000)       38 2021-10-28 14:38:25.897653 casaconfig-0.0.9/setup.cfg
+-rw-rw-r--   0 raba      (1000) raba      (1000)      809 2021-10-28 14:38:09.000000 casaconfig-0.0.9/setup.py
```

### Comparing `casaconfig-0.0.8/LICENSE` & `casaconfig-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.8/PKG-INFO` & `casaconfig-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casaconfig
-Version: 0.0.8
+Version: 0.0.9
 Summary: CASA Operational Configuration Package
 Home-page: https://github.com/casangi/casadata
 Author: National Radio Astronomy Observatory
 Author-email: casa-feedback@nrao.edu
 License: Apache-2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `casaconfig-0.0.8/casaconfig/JPLephem_reader2.py` & `casaconfig-0.0.9/casaconfig/JPLephem_reader2.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.8/casaconfig/config.py` & `casaconfig-0.0.9/casaconfig/config.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.8/casaconfig/get_data_dir.py` & `casaconfig-0.0.9/casaconfig/get_data_dir.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.8/casaconfig/jplephem_request.py` & `casaconfig-0.0.9/casaconfig/jplephem_request.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.8/casaconfig/measures_available.py` & `casaconfig-0.0.9/casaconfig/measures_available.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.8/casaconfig/measures_update.py` & `casaconfig-0.0.9/casaconfig/measures_update.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.8/casaconfig/pull_data.py` & `casaconfig-0.0.9/casaconfig/pull_data.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.8/casaconfig/set_casacore_path.py` & `casaconfig-0.0.9/casaconfig/set_casacore_path.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.8/casaconfig/table_open.py` & `casaconfig-0.0.9/casaconfig/table_open.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.8/casaconfig/write_default_config.py` & `casaconfig-0.0.9/casaconfig/write_default_config.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.8/casaconfig.egg-info/PKG-INFO` & `casaconfig-0.0.9/casaconfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casaconfig
-Version: 0.0.8
+Version: 0.0.9
 Summary: CASA Operational Configuration Package
 Home-page: https://github.com/casangi/casadata
 Author: National Radio Astronomy Observatory
 Author-email: casa-feedback@nrao.edu
 License: Apache-2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `casaconfig-0.0.8/casaconfig.egg-info/SOURCES.txt` & `casaconfig-0.0.9/casaconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.8/setup.py` & `casaconfig-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from glob import glob
 
 with open('README.md', "r") as fid:   #encoding='utf-8'
     long_description = fid.read()
 
 setup(
     name='casaconfig',
-    version='0.0.8',
+    version='0.0.9',
     description='CASA Operational Configuration Package',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='National Radio Astronomy Observatory',
     author_email='casa-feedback@nrao.edu',
     url='https://github.com/casangi/casadata',
     license='Apache-2.0',
```

