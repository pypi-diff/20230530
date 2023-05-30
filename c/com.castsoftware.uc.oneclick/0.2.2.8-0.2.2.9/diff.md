# Comparing `tmp/com.castsoftware.uc.oneclick-0.2.2.8.tar.gz` & `tmp/com.castsoftware.uc.oneclick-0.2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.2.8.tar", last modified: Mon May 15 20:37:26 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.2.9.tar", last modified: Tue May 16 01:57:42 2023, max compression
```

## Comparing `com.castsoftware.uc.oneclick-0.2.2.8.tar` & `com.castsoftware.uc.oneclick-0.2.2.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 20:37:26.067985 com.castsoftware.uc.oneclick-0.2.2.8/
--rw-rw-rw-   0        0        0      517 2023-05-15 20:37:26.056528 com.castsoftware.uc.oneclick-0.2.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-15 20:37:25.745651 com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/
--rw-rw-rw-   0        0        0      517 2023-05-15 20:37:25.000000 com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      836 2023-05-15 20:37:25.000000 com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 20:37:25.000000 com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-05-15 20:37:25.000000 com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-15 20:37:25.000000 com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 20:37:25.890416 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/
--rw-rw-rw-   0        0        0        2 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:37:25.947856 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/__init__.py
--rw-rw-rw-   0        0        0     2736 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/aip_analysis.py
--rw-rw-rw-   0        0        0     1231 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/analysis.py
--rw-rw-rw-   0        0        0     3914 2023-05-13 12:48:37.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/highlight_analysis.py
--rw-rw-rw-   0        0        0     4706 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/trackAnalysis.py
--rw-rw-rw-   0        0        0    19803 2023-05-15 16:57:12.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/config.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:37:26.047175 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/
--rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/__init__.py
--rw-rw-rw-   0        0        0     4432 2023-05-13 21:26:47.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/cleanup.py
--rw-rw-rw-   0        0        0     7052 2023-05-13 21:24:21.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/cloc.py
--rw-rw-rw-   0        0        0     8411 2023-05-15 20:34:04.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/discoveryReport.py
--rw-rw-rw-   0        0        0     3472 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/prep.py
--rw-rw-rw-   0        0        0      491 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/sourceValidation.py
--rw-rw-rw-   0        0        0     6835 2023-05-13 12:48:23.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/sqlDiscovery.py
--rw-rw-rw-   0        0        0     2251 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/unzip.py
--rw-rw-rw-   0        0        0      305 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/exceptions.py
--rw-rw-rw-   0        0        0    10978 2023-05-13 14:37:06.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/main.py
--rw-rw-rw-   0        0        0     2152 2023-05-15 16:56:38.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/runArg.py
--rw-rw-rw-   0        0        0     2098 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/sendEmail.py
--rw-rw-rw-   0        0        0     6003 2023-05-15 13:33:19.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/setup.py
--rw-rw-rw-   0        0        0      752 2023-05-15 20:36:44.000000 com.castsoftware.uc.oneclick-0.2.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 20:37:26.068987 com.castsoftware.uc.oneclick-0.2.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 01:57:42.169070 com.castsoftware.uc.oneclick-0.2.2.9/
+-rw-rw-rw-   0        0        0      517 2023-05-16 01:57:42.159360 com.castsoftware.uc.oneclick-0.2.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 01:57:41.871522 com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-05-16 01:57:41.000000 com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      836 2023-05-16 01:57:41.000000 com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 01:57:41.000000 com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-05-16 01:57:41.000000 com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 01:57:41.000000 com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 01:57:42.004331 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/
+-rw-rw-rw-   0        0        0        2 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:57:42.057857 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/__init__.py
+-rw-rw-rw-   0        0        0     2736 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/aip_analysis.py
+-rw-rw-rw-   0        0        0     1231 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/analysis.py
+-rw-rw-rw-   0        0        0     3914 2023-05-13 12:48:37.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/highlight_analysis.py
+-rw-rw-rw-   0        0        0     4706 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/trackAnalysis.py
+-rw-rw-rw-   0        0        0    19803 2023-05-15 16:57:12.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/config.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:57:42.146823 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/
+-rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/__init__.py
+-rw-rw-rw-   0        0        0     4432 2023-05-13 21:26:47.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/cleanup.py
+-rw-rw-rw-   0        0        0     7052 2023-05-13 21:24:21.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/cloc.py
+-rw-rw-rw-   0        0        0     8411 2023-05-15 20:34:04.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/discoveryReport.py
+-rw-rw-rw-   0        0        0     3472 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/prep.py
+-rw-rw-rw-   0        0        0      491 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/sourceValidation.py
+-rw-rw-rw-   0        0        0     6835 2023-05-13 12:48:23.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/sqlDiscovery.py
+-rw-rw-rw-   0        0        0     2251 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/unzip.py
+-rw-rw-rw-   0        0        0      305 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/exceptions.py
+-rw-rw-rw-   0        0        0    10978 2023-05-13 14:37:06.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/main.py
+-rw-rw-rw-   0        0        0     2152 2023-05-15 16:56:38.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/runArg.py
+-rw-rw-rw-   0        0        0     2098 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/sendEmail.py
+-rw-rw-rw-   0        0        0     6003 2023-05-15 13:33:19.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/setup.py
+-rw-rw-rw-   0        0        0      752 2023-05-16 01:57:16.000000 com.castsoftware.uc.oneclick-0.2.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 01:57:42.169070 com.castsoftware.uc.oneclick-0.2.2.9/setup.cfg
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2.8
+Version: 0.2.2.9
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2.8
+Version: 0.2.2.9
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt` & `com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/aip_analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/aip_analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/highlight_analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/highlight_analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/trackAnalysis.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/trackAnalysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/config.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/config.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/cleanup.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/cleanup.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/cloc.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/cloc.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/discoveryReport.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/discoveryReport.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/prep.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/prep.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/sqlDiscovery.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/sqlDiscovery.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/unzip.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/unzip.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/main.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/main.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/runArg.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/runArg.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/sendEmail.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/sendEmail.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/setup.py` & `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/setup.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.8/pyproject.toml` & `com.castsoftware.uc.oneclick-0.2.2.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name='com.castsoftware.uc.oneclick'
 description="Assessment Generator"
-version='0.2.2.8' #prod version
+version='0.2.2.9' #prod version
 dependencies = [
     'pandas==1.4.0','python-pptx==0.6.18','python-docx','argparse_formatter',
     'django',
-    'com.castsoftware.uc.python.common==1.0.1',
+    'com.castsoftware.uc.python.common==1.0.2',
     'com.castsoftware.uc.action-plan',
     'com.castsoftware.uc.arg'
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

