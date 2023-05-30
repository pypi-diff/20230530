# Comparing `tmp/xpath_filter-1.0.0.tar.gz` & `tmp/xpath_filter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpath_filter-1.0.0.tar", last modified: Tue May 30 05:34:14 2023, max compression
+gzip compressed data, was "xpath_filter-1.0.1.tar", last modified: Tue May 30 12:53:14 2023, max compression
```

## Comparing `xpath_filter-1.0.0.tar` & `xpath_filter-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 05:34:13.996625 xpath_filter-1.0.0/
--rw-rw-rw-   0        0        0    11558 2023-05-28 23:15:09.000000 xpath_filter-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       17 2023-05-30 05:31:35.000000 xpath_filter-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2798 2023-05-30 05:34:13.996625 xpath_filter-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1782 2023-05-30 05:31:35.000000 xpath_filter-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-30 05:34:13.997623 xpath_filter-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1438 2023-05-30 05:31:35.000000 xpath_filter-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:34:13.975618 xpath_filter-1.0.0/src/
--rw-rw-rw-   0        0        0      377 2023-05-30 05:31:35.000000 xpath_filter-1.0.0/src/__init__.py
--rw-rw-rw-   0        0        0     3316 2023-05-30 05:31:35.000000 xpath_filter-1.0.0/src/xpath_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:34:13.994623 xpath_filter-1.0.0/xpath_filter.egg-info/
--rw-rw-rw-   0        0        0     2798 2023-05-30 05:34:13.000000 xpath_filter-1.0.0/xpath_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-05-30 05:34:13.000000 xpath_filter-1.0.0/xpath_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 05:34:13.000000 xpath_filter-1.0.0/xpath_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-30 05:34:13.000000 xpath_filter-1.0.0/xpath_filter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-30 05:34:13.000000 xpath_filter-1.0.0/xpath_filter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 12:53:14.081458 xpath_filter-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2023-05-28 23:15:09.000000 xpath_filter-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-05-30 05:31:35.000000 xpath_filter-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2796 2023-05-30 12:53:14.080450 xpath_filter-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1780 2023-05-30 12:49:52.000000 xpath_filter-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 12:53:14.081458 xpath_filter-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1438 2023-05-30 05:31:35.000000 xpath_filter-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:53:14.061924 xpath_filter-1.0.1/src/
+-rw-rw-rw-   0        0        0      377 2023-05-30 12:49:44.000000 xpath_filter-1.0.1/src/__init__.py
+-rw-rw-rw-   0        0        0     3316 2023-05-30 05:31:35.000000 xpath_filter-1.0.1/src/xpath_filter.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:53:14.077431 xpath_filter-1.0.1/xpath_filter.egg-info/
+-rw-rw-rw-   0        0        0     2796 2023-05-30 12:53:13.000000 xpath_filter-1.0.1/xpath_filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-05-30 12:53:13.000000 xpath_filter-1.0.1/xpath_filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 12:53:13.000000 xpath_filter-1.0.1/xpath_filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-30 12:53:13.000000 xpath_filter-1.0.1/xpath_filter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-30 12:53:13.000000 xpath_filter-1.0.1/xpath_filter.egg-info/top_level.txt
```

### Comparing `xpath_filter-1.0.0/LICENSE` & `xpath_filter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xpath_filter-1.0.0/PKG-INFO` & `xpath_filter-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpath_filter
-Version: 1.0.0
+Version: 1.0.1
 Summary: XPath filter of HTML files
 Home-page: https://github.com/CarlosAdp/xpath-filter
 Author: Carlos Pinto
 Author-email: carlos.adpinto@gmail.com
 License: Apache License 2.0
 Keywords: xpath html scraping webscraping scraper webscraper
 Classifier: Operating System :: Microsoft :: Windows
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # xpath-filter
 
-[![version](https://img.shields.io/badge/version-1.0.0-blue)](https://pypi.org/project/xpath-filter)
+[![version](https://img.shields.io/badge/version-1.0.1-blue)](https://pypi.org/project/xpath-filter)
 [![tests](https://img.shields.io/badge/tests-passed-green)](tests/test_xpath_filter.py)
 
 Filter HTML files using xpath mappings.
 
 ## Installation
 
 Install `xpath-filter` using pip:
@@ -69,15 +69,15 @@
 ### Filtering HTML file from a YAML xpaths definition.
 
 File at "xpaths.yml":
 
 ```yml
 article:
     xpath: //div[@class="article"]
-    matches: first
+    matches: all
     elements:
         author: './@data-author'
         content: ./p/text()
 ```
 
 Code:
```

### Comparing `xpath_filter-1.0.0/README.md` & `xpath_filter-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # xpath-filter
 
-[![version](https://img.shields.io/badge/version-1.0.0-blue)](https://pypi.org/project/xpath-filter)
+[![version](https://img.shields.io/badge/version-1.0.1-blue)](https://pypi.org/project/xpath-filter)
 [![tests](https://img.shields.io/badge/tests-passed-green)](tests/test_xpath_filter.py)
 
 Filter HTML files using xpath mappings.
 
 ## Installation
 
 Install `xpath-filter` using pip:
@@ -43,15 +43,15 @@
 ### Filtering HTML file from a YAML xpaths definition.
 
 File at "xpaths.yml":
 
 ```yml
 article:
     xpath: //div[@class="article"]
-    matches: first
+    matches: all
     elements:
         author: './@data-author'
         content: ./p/text()
 ```
 
 Code:
```

### Comparing `xpath_filter-1.0.0/setup.py` & `xpath_filter-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `xpath_filter-1.0.0/src/xpath_filter.py` & `xpath_filter-1.0.1/src/xpath_filter.py`

 * *Files identical despite different names*

### Comparing `xpath_filter-1.0.0/xpath_filter.egg-info/PKG-INFO` & `xpath_filter-1.0.1/xpath_filter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpath-filter
-Version: 1.0.0
+Version: 1.0.1
 Summary: XPath filter of HTML files
 Home-page: https://github.com/CarlosAdp/xpath-filter
 Author: Carlos Pinto
 Author-email: carlos.adpinto@gmail.com
 License: Apache License 2.0
 Keywords: xpath html scraping webscraping scraper webscraper
 Classifier: Operating System :: Microsoft :: Windows
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # xpath-filter
 
-[![version](https://img.shields.io/badge/version-1.0.0-blue)](https://pypi.org/project/xpath-filter)
+[![version](https://img.shields.io/badge/version-1.0.1-blue)](https://pypi.org/project/xpath-filter)
 [![tests](https://img.shields.io/badge/tests-passed-green)](tests/test_xpath_filter.py)
 
 Filter HTML files using xpath mappings.
 
 ## Installation
 
 Install `xpath-filter` using pip:
@@ -69,15 +69,15 @@
 ### Filtering HTML file from a YAML xpaths definition.
 
 File at "xpaths.yml":
 
 ```yml
 article:
     xpath: //div[@class="article"]
-    matches: first
+    matches: all
     elements:
         author: './@data-author'
         content: ./p/text()
 ```
 
 Code:
```

