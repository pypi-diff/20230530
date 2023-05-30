# Comparing `tmp/artscraper-0.1.1.tar.gz` & `tmp/artscraper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artscraper-0.1.1.tar", last modified: Tue Oct  4 13:17:22 2022, max compression
+gzip compressed data, was "artscraper-0.2.0.tar", last modified: Tue May 30 08:39:31 2023, max compression
```

## Comparing `artscraper-0.1.1.tar` & `artscraper-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 13:17:22.782600 artscraper-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-10-04 13:17:10.000000 artscraper-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-10-04 13:17:22.782600 artscraper-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4644 2022-10-04 13:17:10.000000 artscraper-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 13:17:22.782600 artscraper-0.1.1/artscraper/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-10-04 13:17:10.000000 artscraper-0.1.1/artscraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-10-04 13:17:10.000000 artscraper-0.1.1/artscraper/base.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6645 2022-10-04 13:17:10.000000 artscraper-0.1.1/artscraper/googleart.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7634 2022-10-04 13:17:10.000000 artscraper-0.1.1/artscraper/wikiart.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 13:17:22.782600 artscraper-0.1.1/artscraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-10-04 13:17:22.000000 artscraper-0.1.1/artscraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-10-04 13:17:22.000000 artscraper-0.1.1/artscraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-04 13:17:22.000000 artscraper-0.1.1/artscraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-04 13:17:22.000000 artscraper-0.1.1/artscraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-04 13:17:22.000000 artscraper-0.1.1/artscraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-10-04 13:17:22.782600 artscraper-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-10-04 13:17:10.000000 artscraper-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:39:31.452521 artscraper-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-30 08:39:17.000000 artscraper-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-30 08:39:31.452521 artscraper-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-05-30 08:39:17.000000 artscraper-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:39:31.452521 artscraper-0.2.0/artscraper/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/find_artists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/find_artworks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5688 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/googleart.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7634 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/wikiart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:39:31.452521 artscraper-0.2.0/artscraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-30 08:39:31.000000 artscraper-0.2.0/artscraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-30 08:39:31.000000 artscraper-0.2.0/artscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:39:31.000000 artscraper-0.2.0/artscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 08:39:31.000000 artscraper-0.2.0/artscraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 08:39:31.000000 artscraper-0.2.0/artscraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 08:39:31.452521 artscraper-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-30 08:39:17.000000 artscraper-0.2.0/setup.py
```

### Comparing `artscraper-0.1.1/LICENSE` & `artscraper-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `artscraper-0.1.1/artscraper/base.py` & `artscraper-0.2.0/artscraper/base.py`

 * *Files identical despite different names*

### Comparing `artscraper-0.1.1/artscraper/googleart.py` & `artscraper-0.2.0/artscraper/googleart.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Module for GoogleArtScraper class."""
 
 import json
 import time
 from pathlib import Path
-from random import random
 from time import sleep
 from urllib.parse import urlparse
 
 from bs4 import BeautifulSoup
 from selenium import webdriver
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.common.keys import Keys
 
 from artscraper.base import BaseArtScraper
-
+from artscraper.functions import random_wait_time
 
 class GoogleArtScraper(BaseArtScraper):
     """Class for scraping GoogleArt images.
 
     Parameters
     ----------
     output_dir: Path.pathlib or str, optional
@@ -156,46 +155,7 @@
         if self.skip_existing and img_fp.is_file():
             return
         with open(img_fp, "wb") as f:
             f.write(self.get_image())
 
     def close(self):
         self.driver.close()
-
-
-def random_wait_time(min_wait=5, max_wait=None):
-    """Compute a random wait time.
-
-    This is a probability distribution with non-zero values between
-    min_wait and max_wait. The PDF decreases as a powerlaw (**-1.5) between
-    the two.
-
-    Parameters
-    ----------
-    min_wait: int or float, default=5
-        Minimum waiting time.
-    max_wait: int or float, optional
-        Maximum waiting time. If not supplied, use 3x
-        minimum waiting time.
-
-    Returns
-    -------
-    float:
-        Waiting time between `min_wait` and `max_wait` according to
-        the polynomial PDF.
-    """
-    #  pylint: disable=invalid-name
-    if max_wait is None:
-        max_wait = 3 * min_wait
-    alpha = 1.5
-    beta = alpha - 1
-    b = min_wait
-    c = max_wait
-    a = -beta / (c**-beta - b**-beta)
-
-    # def cdf(x):
-    #     return a / beta * (b**-beta - x**-beta)
-
-    def inv_cdf(x):
-        return (b**-beta - beta * x / a)**(-1 / beta)
-
-    return inv_cdf(random())
```

### Comparing `artscraper-0.1.1/artscraper/wikiart.py` & `artscraper-0.2.0/artscraper/wikiart.py`

 * *Files identical despite different names*

### Comparing `artscraper-0.1.1/setup.py` & `artscraper-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
     
 setup(
     name='artscraper',
-    version='0.1.1',
+    version='0.2.0',
     author='ODISSEI Social Data Science Team',
     description='Package for scraping artworks from WikiArt and GoogleArt',
     long_description='See https://github.com/sodascience/artscraper for examples and usage',
     keywords='artscraper wikiart artsandculture',
     license='MIT',
     url='https://github.com/sodascience/artscraper',
     packages=find_packages(exclude=['data', 'docs', 'tests', 'examples']),
     python_requires='~=3.6',
     install_requires=[
         "requests",
         "selenium",
-        "beautifulsoup4"
+        "beautifulsoup4",
+        "wikipedia-api"
     ]
 )
```

