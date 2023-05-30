# Comparing `tmp/duptextfinder-0.1.tar.gz` & `tmp/duptextfinder-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duptextfinder-0.1.tar", last modified: Tue May 30 09:20:37 2023, max compression
+gzip compressed data, was "duptextfinder-0.2.tar", last modified: Tue May 30 09:26:34 2023, max compression
```

## Comparing `duptextfinder-0.1.tar` & `duptextfinder-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 obirot   (668440) heka     (201783)        0 2023-05-30 09:20:37.580149 duptextfinder-0.1/
--rw-r--r--   0 obirot   (668440) heka     (201783)     2989 2023-05-30 09:20:37.580149 duptextfinder-0.1/PKG-INFO
--rw-r--r--   0 obirot   (668440) heka     (201783)     2161 2023-05-30 09:16:48.000000 duptextfinder-0.1/README.md
-drwxr-xr-x   0 obirot   (668440) heka     (201783)        0 2023-05-30 09:20:37.580149 duptextfinder-0.1/duptextfinder/
--rw-r--r--   0 obirot   (668440) heka     (201783)      215 2023-05-30 09:10:29.000000 duptextfinder-0.1/duptextfinder/__init__.py
--rw-r--r--   0 obirot   (668440) heka     (201783)     7946 2023-05-30 09:10:29.000000 duptextfinder-0.1/duptextfinder/char_fingerprint_builder.py
--rw-r--r--   0 obirot   (668440) heka     (201783)    33753 2023-05-30 09:10:29.000000 duptextfinder-0.1/duptextfinder/duplicate_finder.py
--rw-r--r--   0 obirot   (668440) heka     (201783)      822 2023-05-30 08:48:39.000000 duptextfinder-0.1/duptextfinder/span.py
--rw-r--r--   0 obirot   (668440) heka     (201783)     8803 2023-05-30 09:10:29.000000 duptextfinder-0.1/duptextfinder/word_fingerprint_builder.py
-drwxr-xr-x   0 obirot   (668440) heka     (201783)        0 2023-05-30 09:20:37.580149 duptextfinder-0.1/duptextfinder.egg-info/
--rw-r--r--   0 obirot   (668440) heka     (201783)     2989 2023-05-30 09:20:37.000000 duptextfinder-0.1/duptextfinder.egg-info/PKG-INFO
--rw-r--r--   0 obirot   (668440) heka     (201783)      378 2023-05-30 09:20:37.000000 duptextfinder-0.1/duptextfinder.egg-info/SOURCES.txt
--rw-r--r--   0 obirot   (668440) heka     (201783)        1 2023-05-30 09:20:37.000000 duptextfinder-0.1/duptextfinder.egg-info/dependency_links.txt
--rw-r--r--   0 obirot   (668440) heka     (201783)       91 2023-05-30 09:20:37.000000 duptextfinder-0.1/duptextfinder.egg-info/requires.txt
--rw-r--r--   0 obirot   (668440) heka     (201783)       14 2023-05-30 09:20:37.000000 duptextfinder-0.1/duptextfinder.egg-info/top_level.txt
--rw-r--r--   0 obirot   (668440) heka     (201783)       79 2023-05-30 09:20:37.580149 duptextfinder-0.1/setup.cfg
--rw-r--r--   0 obirot   (668440) heka     (201783)      684 2023-05-30 09:16:17.000000 duptextfinder-0.1/setup.py
+drwxr-xr-x   0 obirot   (668440) heka     (201783)        0 2023-05-30 09:26:34.300162 duptextfinder-0.2/
+-rw-r--r--   0 obirot   (668440) heka     (201783)     3171 2023-05-30 09:26:34.300162 duptextfinder-0.2/PKG-INFO
+-rw-r--r--   0 obirot   (668440) heka     (201783)     2279 2023-05-30 09:23:28.000000 duptextfinder-0.2/README.md
+drwxr-xr-x   0 obirot   (668440) heka     (201783)        0 2023-05-30 09:26:34.300162 duptextfinder-0.2/duptextfinder/
+-rw-r--r--   0 obirot   (668440) heka     (201783)      215 2023-05-30 09:10:29.000000 duptextfinder-0.2/duptextfinder/__init__.py
+-rw-r--r--   0 obirot   (668440) heka     (201783)     7946 2023-05-30 09:10:29.000000 duptextfinder-0.2/duptextfinder/char_fingerprint_builder.py
+-rw-r--r--   0 obirot   (668440) heka     (201783)    33753 2023-05-30 09:10:29.000000 duptextfinder-0.2/duptextfinder/duplicate_finder.py
+-rw-r--r--   0 obirot   (668440) heka     (201783)      822 2023-05-30 08:48:39.000000 duptextfinder-0.2/duptextfinder/span.py
+-rw-r--r--   0 obirot   (668440) heka     (201783)     8803 2023-05-30 09:10:29.000000 duptextfinder-0.2/duptextfinder/word_fingerprint_builder.py
+drwxr-xr-x   0 obirot   (668440) heka     (201783)        0 2023-05-30 09:26:34.300162 duptextfinder-0.2/duptextfinder.egg-info/
+-rw-r--r--   0 obirot   (668440) heka     (201783)     3171 2023-05-30 09:26:34.000000 duptextfinder-0.2/duptextfinder.egg-info/PKG-INFO
+-rw-r--r--   0 obirot   (668440) heka     (201783)      378 2023-05-30 09:26:34.000000 duptextfinder-0.2/duptextfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 obirot   (668440) heka     (201783)        1 2023-05-30 09:26:34.000000 duptextfinder-0.2/duptextfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 obirot   (668440) heka     (201783)       91 2023-05-30 09:26:34.000000 duptextfinder-0.2/duptextfinder.egg-info/requires.txt
+-rw-r--r--   0 obirot   (668440) heka     (201783)       14 2023-05-30 09:26:34.000000 duptextfinder-0.2/duptextfinder.egg-info/top_level.txt
+-rw-r--r--   0 obirot   (668440) heka     (201783)       79 2023-05-30 09:26:34.300162 duptextfinder-0.2/setup.cfg
+-rw-r--r--   0 obirot   (668440) heka     (201783)      684 2023-05-30 09:25:25.000000 duptextfinder-0.2/setup.py
```

### Comparing `duptextfinder-0.1/PKG-INFO` & `duptextfinder-0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 Metadata-Version: 2.1
 Name: duptextfinder
-Version: 0.1
+Version: 0.2
 Summary: Detect duplicated zones in (clinical) text
 Home-page: https://github.com/equipe22/duplicatedZoneInClinicalText
 License: GPLv3
 Description: # Duplicate Text Finder
         
-        A python library to detect duplicated zones in text. Primarily meant to detect
+        `duptextfinder` is a python library to detect duplicated zones in text. Primarily meant to detect
         copy/paste across medical documents. Should be faster than python's built-in
         `difflib` algorithm and more robust to whitespace, newlines and other irrelevant
         characters.
         
+        ## Installation
+        
+        `duptextfinder` can be installed through pip:
+        
+        ```
+        pip install duptextfinder
+        ```
+        
         ## Usage
         
         ```python3
         
         from pathlib import Path
         from duptextfinder import CharFingerprintBuilder, DuplicateFinder
```

### Comparing `duptextfinder-0.1/README.md` & `duptextfinder-0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Duplicate Text Finder
 
-A python library to detect duplicated zones in text. Primarily meant to detect
+`duptextfinder` is a python library to detect duplicated zones in text. Primarily meant to detect
 copy/paste across medical documents. Should be faster than python's built-in
 `difflib` algorithm and more robust to whitespace, newlines and other irrelevant
 characters.
 
+## Installation
+
+`duptextfinder` can be installed through pip:
+
+```
+pip install duptextfinder
+```
+
 ## Usage
 
 ```python3
 
 from pathlib import Path
 from duptextfinder import CharFingerprintBuilder, DuplicateFinder
```

### Comparing `duptextfinder-0.1/duptextfinder/char_fingerprint_builder.py` & `duptextfinder-0.2/duptextfinder/char_fingerprint_builder.py`

 * *Files identical despite different names*

### Comparing `duptextfinder-0.1/duptextfinder/duplicate_finder.py` & `duptextfinder-0.2/duptextfinder/duplicate_finder.py`

 * *Files identical despite different names*

### Comparing `duptextfinder-0.1/duptextfinder/span.py` & `duptextfinder-0.2/duptextfinder/span.py`

 * *Files identical despite different names*

### Comparing `duptextfinder-0.1/duptextfinder/word_fingerprint_builder.py` & `duptextfinder-0.2/duptextfinder/word_fingerprint_builder.py`

 * *Files identical despite different names*

### Comparing `duptextfinder-0.1/duptextfinder.egg-info/PKG-INFO` & `duptextfinder-0.2/duptextfinder.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 Metadata-Version: 2.1
 Name: duptextfinder
-Version: 0.1
+Version: 0.2
 Summary: Detect duplicated zones in (clinical) text
 Home-page: https://github.com/equipe22/duplicatedZoneInClinicalText
 License: GPLv3
 Description: # Duplicate Text Finder
         
-        A python library to detect duplicated zones in text. Primarily meant to detect
+        `duptextfinder` is a python library to detect duplicated zones in text. Primarily meant to detect
         copy/paste across medical documents. Should be faster than python's built-in
         `difflib` algorithm and more robust to whitespace, newlines and other irrelevant
         characters.
         
+        ## Installation
+        
+        `duptextfinder` can be installed through pip:
+        
+        ```
+        pip install duptextfinder
+        ```
+        
         ## Usage
         
         ```python3
         
         from pathlib import Path
         from duptextfinder import CharFingerprintBuilder, DuplicateFinder
```

### Comparing `duptextfinder-0.1/setup.py` & `duptextfinder-0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,13 +9,13 @@
     license="GPLv3",
     packages=["duptextfinder"],
     extras_require = {
         "tests": ["pytest", "pytest-mock"],
         "ncls":  ["ncls>=0.0.66", "numpy"],
         "intervaltree":  ["intervaltree>=3.0.0"],
     },
-    version="0.1",
+    version="0.2",
     keywords = ["TEXT", "DUPLICATION", "DUPLICATE", "CLINICAL"],
     url="https://github.com/equipe22/duplicatedZoneInClinicalText",
     long_description=long_description,
     long_description_content_type="text/markdown"
 )
```

