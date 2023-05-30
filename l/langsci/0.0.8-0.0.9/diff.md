# Comparing `tmp/langsci-0.0.8.tar.gz` & `tmp/langsci-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/langsci-0.0.8.tar", last modified: Thu Sep 27 14:06:42 2018, max compression
+gzip compressed data, was "dist/langsci-0.0.9.tar", last modified: Thu Sep 27 14:07:30 2018, max compression
```

## Comparing `langsci-0.0.8.tar` & `langsci-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 snordhoff  (1000) snordhoff  (1000)        0 2018-09-27 14:06:42.000000 langsci-0.0.8/
-drwxrwxr-x   0 snordhoff  (1000) snordhoff  (1000)        0 2018-09-27 14:06:42.000000 langsci-0.0.8/langsci/
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     1154 2018-09-14 09:46:11.000000 langsci-0.0.8/langsci/delatex.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     6699 2018-09-20 09:01:29.000000 langsci-0.0.8/langsci/langsci_tests.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     6628 2018-09-27 12:01:12.000000 langsci-0.0.8/langsci/zenodo.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)        0 2018-09-27 11:45:24.000000 langsci-0.0.8/langsci/sanitycheck.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)    14606 2018-09-27 09:02:44.000000 langsci-0.0.8/langsci/extractaw.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     2896 2018-09-27 13:00:33.000000 langsci-0.0.8/langsci/autoindex.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)    30017 2018-09-27 13:05:34.000000 langsci-0.0.8/langsci/convertertools.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)    12112 2018-09-27 13:22:14.000000 langsci-0.0.8/langsci/sanity.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     2293 2018-09-27 13:10:34.000000 langsci-0.0.8/langsci/normalizebib.py
--rw-r--r--   0 snordhoff  (1000) snordhoff  (1000)      225 2018-09-19 12:15:18.000000 langsci-0.0.8/langsci/__init__.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     1012 2018-09-27 13:09:20.000000 langsci-0.0.8/langsci/fixindex.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     6361 2018-09-27 14:03:21.000000 langsci-0.0.8/langsci/langscibibtex.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)      276 2018-09-27 14:02:24.000000 langsci-0.0.8/langsci/txt2bib.py
--rw-r--r--   0 snordhoff  (1000) snordhoff  (1000)      471 2018-09-27 08:04:05.000000 langsci-0.0.8/langsci/doc2tex.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     2049 2018-09-27 12:06:55.000000 langsci-0.0.8/langsci/indextools.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)   224435 2018-09-20 08:22:14.000000 langsci-0.0.8/langsci/bibnouns.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     1849 2018-09-27 13:19:42.000000 langsci-0.0.8/langsci/registerzenodo.py
--rw-r--r--   0 snordhoff  (1000) snordhoff  (1000)    14551 2018-09-14 09:51:00.000000 langsci-0.0.8/langsci/asciify.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     1490 2018-09-27 11:46:58.000000 langsci-0.0.8/langsci/sanitygit.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     2564 2018-09-18 09:27:51.000000 langsci-0.0.8/langsci/assignproofreaders.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)    16611 2018-09-27 14:06:29.000000 langsci-0.0.8/langsci/bibtools.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)      448 2018-09-27 13:21:50.000000 langsci-0.0.8/langsci/sanitylocal.py
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)      563 2018-09-27 14:06:42.000000 langsci-0.0.8/PKG-INFO
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)      643 2018-09-27 14:06:33.000000 langsci-0.0.8/setup.py
-drwxrwxr-x   0 snordhoff  (1000) snordhoff  (1000)        0 2018-09-27 14:06:42.000000 langsci-0.0.8/langsci.egg-info/
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)        1 2018-09-27 14:06:42.000000 langsci-0.0.8/langsci.egg-info/dependency_links.txt
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)      563 2018-09-27 14:06:42.000000 langsci-0.0.8/langsci.egg-info/PKG-INFO
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)        8 2018-09-27 14:06:42.000000 langsci-0.0.8/langsci.egg-info/top_level.txt
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)      621 2018-09-27 14:06:42.000000 langsci-0.0.8/langsci.egg-info/SOURCES.txt
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)       72 2018-09-18 11:41:51.000000 langsci-0.0.8/README.md
--rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)       38 2018-09-27 14:06:42.000000 langsci-0.0.8/setup.cfg
+drwxrwxr-x   0 snordhoff  (1000) snordhoff  (1000)        0 2018-09-27 14:07:30.000000 langsci-0.0.9/
+drwxrwxr-x   0 snordhoff  (1000) snordhoff  (1000)        0 2018-09-27 14:07:30.000000 langsci-0.0.9/langsci/
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     1154 2018-09-14 09:46:11.000000 langsci-0.0.9/langsci/delatex.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     6699 2018-09-20 09:01:29.000000 langsci-0.0.9/langsci/langsci_tests.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     6628 2018-09-27 12:01:12.000000 langsci-0.0.9/langsci/zenodo.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)        0 2018-09-27 11:45:24.000000 langsci-0.0.9/langsci/sanitycheck.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)    14606 2018-09-27 09:02:44.000000 langsci-0.0.9/langsci/extractaw.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     2896 2018-09-27 13:00:33.000000 langsci-0.0.9/langsci/autoindex.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)    30017 2018-09-27 13:05:34.000000 langsci-0.0.9/langsci/convertertools.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)    12112 2018-09-27 13:22:14.000000 langsci-0.0.9/langsci/sanity.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     2293 2018-09-27 13:10:34.000000 langsci-0.0.9/langsci/normalizebib.py
+-rw-r--r--   0 snordhoff  (1000) snordhoff  (1000)      225 2018-09-19 12:15:18.000000 langsci-0.0.9/langsci/__init__.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     1012 2018-09-27 13:09:20.000000 langsci-0.0.9/langsci/fixindex.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     6361 2018-09-27 14:03:21.000000 langsci-0.0.9/langsci/langscibibtex.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)      276 2018-09-27 14:02:24.000000 langsci-0.0.9/langsci/txt2bib.py
+-rw-r--r--   0 snordhoff  (1000) snordhoff  (1000)      471 2018-09-27 08:04:05.000000 langsci-0.0.9/langsci/doc2tex.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     2049 2018-09-27 12:06:55.000000 langsci-0.0.9/langsci/indextools.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)   224435 2018-09-20 08:22:14.000000 langsci-0.0.9/langsci/bibnouns.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     1849 2018-09-27 13:19:42.000000 langsci-0.0.9/langsci/registerzenodo.py
+-rw-r--r--   0 snordhoff  (1000) snordhoff  (1000)    14551 2018-09-14 09:51:00.000000 langsci-0.0.9/langsci/asciify.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     1490 2018-09-27 11:46:58.000000 langsci-0.0.9/langsci/sanitygit.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)     2564 2018-09-18 09:27:51.000000 langsci-0.0.9/langsci/assignproofreaders.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)    16611 2018-09-27 14:07:23.000000 langsci-0.0.9/langsci/bibtools.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)      448 2018-09-27 13:21:50.000000 langsci-0.0.9/langsci/sanitylocal.py
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)      563 2018-09-27 14:07:30.000000 langsci-0.0.9/PKG-INFO
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)      643 2018-09-27 14:07:27.000000 langsci-0.0.9/setup.py
+drwxrwxr-x   0 snordhoff  (1000) snordhoff  (1000)        0 2018-09-27 14:07:30.000000 langsci-0.0.9/langsci.egg-info/
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)        1 2018-09-27 14:07:30.000000 langsci-0.0.9/langsci.egg-info/dependency_links.txt
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)      563 2018-09-27 14:07:30.000000 langsci-0.0.9/langsci.egg-info/PKG-INFO
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)        8 2018-09-27 14:07:30.000000 langsci-0.0.9/langsci.egg-info/top_level.txt
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)      621 2018-09-27 14:07:30.000000 langsci-0.0.9/langsci.egg-info/SOURCES.txt
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)       72 2018-09-18 11:41:51.000000 langsci-0.0.9/README.md
+-rw-rw-r--   0 snordhoff  (1000) snordhoff  (1000)       38 2018-09-27 14:07:30.000000 langsci-0.0.9/setup.cfg
```

### Comparing `langsci-0.0.8/langsci/delatex.py` & `langsci-0.0.9/langsci/delatex.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/langsci_tests.py` & `langsci-0.0.9/langsci/langsci_tests.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/zenodo.py` & `langsci-0.0.9/langsci/zenodo.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/extractaw.py` & `langsci-0.0.9/langsci/extractaw.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/autoindex.py` & `langsci-0.0.9/langsci/autoindex.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/convertertools.py` & `langsci-0.0.9/langsci/convertertools.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/sanity.py` & `langsci-0.0.9/langsci/sanity.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/normalizebib.py` & `langsci-0.0.9/langsci/normalizebib.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/fixindex.py` & `langsci-0.0.9/langsci/fixindex.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/langscibibtex.py` & `langsci-0.0.9/langsci/langscibibtex.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/indextools.py` & `langsci-0.0.9/langsci/indextools.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/bibnouns.py` & `langsci-0.0.9/langsci/bibnouns.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/registerzenodo.py` & `langsci-0.0.9/langsci/registerzenodo.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/asciify.py` & `langsci-0.0.9/langsci/asciify.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/sanitygit.py` & `langsci-0.0.9/langsci/sanitygit.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/assignproofreaders.py` & `langsci-0.0.9/langsci/assignproofreaders.py`

 * *Files identical despite different names*

### Comparing `langsci-0.0.8/langsci/bibtools.py` & `langsci-0.0.9/langsci/bibtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import argparse
 
 try:
     from asciify import ASCIITRANS, FRENCH_REPLACEMENTS, GERMAN_REPLACEMENTS, ICELANDIC_REPLACEMENTS, asciify
     from bibnouns import LANGUAGENAMES, OCEANNAMES, COUNTRIES, CONTINENTNAMES, CITIES, OCCURREDREPLACEMENTS
     from delatex import dediacriticize
 except ImportError:
-    langsci.from asciify import ASCIITRANS, FRENCH_REPLACEMENTS, GERMAN_REPLACEMENTS, ICELANDIC_REPLACEMENTS, asciify
-    langsci.from bibnouns import LANGUAGENAMES, OCEANNAMES, COUNTRIES, CONTINENTNAMES, CITIES, OCCURREDREPLACEMENTS
-    langsci.from delatex import dediacriticize
+    from langsci.asciify import ASCIITRANS, FRENCH_REPLACEMENTS, GERMAN_REPLACEMENTS, ICELANDIC_REPLACEMENTS, asciify
+    from langsci.bibnouns import LANGUAGENAMES, OCEANNAMES, COUNTRIES, CONTINENTNAMES, CITIES, OCCURREDREPLACEMENTS
+    from langsci.delatex import dediacriticize
 
 keys = {} #store for all bibtex keys
 #The following fields will not be included in the normalizedfile
 excludefields = ['abstract', 
                  'language', 
                  'date-added',
                  'date-modified',
```

### Comparing `langsci-0.0.8/PKG-INFO` & `langsci-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langsci
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for open access books used at Language Science Press
 Home-page: https://github.com/langsci/pypi
 Author: Sebastian Nordhoff
 Author-email: sebastian.nordhoff@langsci-press.org
 License: UNKNOWN
 Description: # LangSci
```

### Comparing `langsci-0.0.8/setup.py` & `langsci-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="langsci",
-    version="0.0.8",
+    version="0.0.9",
     author="Sebastian Nordhoff",
     author_email="sebastian.nordhoff@langsci-press.org",
     description="Tools for open access books used at Language Science Press",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/langsci/pypi",
     packages=["langsci"],
```

### Comparing `langsci-0.0.8/langsci.egg-info/PKG-INFO` & `langsci-0.0.9/langsci.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langsci
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for open access books used at Language Science Press
 Home-page: https://github.com/langsci/pypi
 Author: Sebastian Nordhoff
 Author-email: sebastian.nordhoff@langsci-press.org
 License: UNKNOWN
 Description: # LangSci
```

### Comparing `langsci-0.0.8/langsci.egg-info/SOURCES.txt` & `langsci-0.0.9/langsci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

