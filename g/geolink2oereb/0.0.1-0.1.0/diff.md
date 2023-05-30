# Comparing `tmp/geolink2oereb-0.0.1.tar.gz` & `tmp/geolink2oereb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolink2oereb-0.0.1.tar", last modified: Tue May 30 11:25:46 2023, max compression
+gzip compressed data, was "geolink2oereb-0.1.0.tar", last modified: Tue May 30 14:36:01 2023, max compression
```

## Comparing `geolink2oereb-0.0.1.tar` & `geolink2oereb-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:25:46.800384 geolink2oereb-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-30 11:25:46.800384 geolink2oereb-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-30 11:25:46.800384 geolink2oereb-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:25:46.796384 geolink2oereb-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:25:46.796384 geolink2oereb-0.0.1/src/geolink2oereb/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/src/geolink2oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/src/geolink2oereb/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:25:46.796384 geolink2oereb-0.0.1/src/geolink2oereb/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/src/geolink2oereb/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:25:46.796384 geolink2oereb-0.0.1/src/geolink2oereb/lib/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/src/geolink2oereb/lib/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:25:46.796384 geolink2oereb-0.0.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:25:46.800384 geolink2oereb-0.0.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:25:46.800384 geolink2oereb-0.0.1/src/geolink2oereb/lib/interfaces/pyramid_oereb/
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-30 11:25:14.000000 geolink2oereb-0.0.1/src/geolink2oereb/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:25:46.796384 geolink2oereb-0.0.1/src/geolink2oereb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-30 11:25:46.000000 geolink2oereb-0.0.1/src/geolink2oereb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-30 11:25:46.000000 geolink2oereb-0.0.1/src/geolink2oereb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:25:46.000000 geolink2oereb-0.0.1/src/geolink2oereb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 11:25:46.000000 geolink2oereb-0.0.1/src/geolink2oereb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:25:46.000000 geolink2oereb-0.0.1/src/geolink2oereb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-30 11:25:46.000000 geolink2oereb-0.0.1/src/geolink2oereb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 11:25:46.000000 geolink2oereb-0.0.1/src/geolink2oereb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:36:01.057296 geolink2oereb-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-30 14:36:01.057296 geolink2oereb-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-30 14:36:01.057296 geolink2oereb-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:36:01.053296 geolink2oereb-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:36:01.053296 geolink2oereb-0.1.0/src/geolink2oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/src/geolink2oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/src/geolink2oereb/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:36:01.057296 geolink2oereb-0.1.0/src/geolink2oereb/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/src/geolink2oereb/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:36:01.057296 geolink2oereb-0.1.0/src/geolink2oereb/lib/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/src/geolink2oereb/lib/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:36:01.057296 geolink2oereb-0.1.0/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:36:01.057296 geolink2oereb-0.1.0/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2034125 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:36:01.057296 geolink2oereb-0.1.0/src/geolink2oereb/lib/interfaces/pyramid_oereb/
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-30 14:35:27.000000 geolink2oereb-0.1.0/src/geolink2oereb/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:36:01.053296 geolink2oereb-0.1.0/src/geolink2oereb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-30 14:36:01.000000 geolink2oereb-0.1.0/src/geolink2oereb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-30 14:36:01.000000 geolink2oereb-0.1.0/src/geolink2oereb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:36:01.000000 geolink2oereb-0.1.0/src/geolink2oereb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 14:36:01.000000 geolink2oereb-0.1.0/src/geolink2oereb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:36:01.000000 geolink2oereb-0.1.0/src/geolink2oereb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 14:36:01.000000 geolink2oereb-0.1.0/src/geolink2oereb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 14:36:01.000000 geolink2oereb-0.1.0/src/geolink2oereb.egg-info/top_level.txt
```

### Comparing `geolink2oereb-0.0.1/LICENSE` & `geolink2oereb-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.0.1/README.md` & `geolink2oereb-0.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,13 @@
 OEREBlex geoLink Formatter
 ==========================
 
-|license| |python version| |format| |status| |build status| |coverage report| |dependencies| |code quality|
+|![license](https://img.shields.io/pypi/l/geolink2oereb.svg)|![python version](https://img.shields.io/pypi/pyversions/geolink2oereb.svg)|![format](https://img.shields.io/pypi/format/geolink2oereb.svg)|![status](https://img.shields.io/pypi/status/geolink2oereb.svg)|![build status](https://github.com/openoereb/geolink2oereb/actions/workflows/ci.yml/badge.svg)|![coverage report](https://codecov.io/gh/openoereb/geolink2oereb/branch/master/graph/badge.svg)|![dependencies](https://img.shields.io/librariesio/github/openoereb/geolink2oereb.svg)|![code quality](https://app.codacy.com/project/badge/Grade/2ac4dbc1dd3e4c7f8d9f97c195a07c24)|
 
-This is a small library, meant to be used in combination with OEREBlex. It is capable of parsing a received
-geoLink response (XML) and converting it to multiple formats, such as HTML, which can be styled for
-presentation.
+This is a small library, meant to be used in combination with OEREBlex. It uses 
+[geolink_formatter](https://pypi.org/search/?q=geolink_formatter) and
+[pyramid_oereb](https://pypi.org/project/pyramid-oereb/) as proven libs to handle
+configuration and connection to ÖREBlex. On top, it provides a decent way to transform received ÖREBlex
+documents into the OeREBKRMtrsfr structure objects for further handling.
 
-For detailed information, please refer to the online documentation:
-
-https://openoereb.github.io/geolink2oereb/
-
-.. |license| image:: https://img.shields.io/pypi/l/geolink2oereb.svg
-   :target: https://pypi.org/project/geolink2oereb/
-.. |python version| image:: https://img.shields.io/pypi/pyversions/geolink2oereb.svg
-   :target: https://pypi.org/project/geolink2oereb/
-.. |format| image:: https://img.shields.io/pypi/format/geolink2oereb.svg
-   :target: https://pypi.org/project/geolink2oereb/
-.. |status| image:: https://img.shields.io/pypi/status/geolink2oereb.svg
-   :target: https://pypi.org/project/geolink2oereb/
-.. |build status| image:: https://travis-ci.org/openoereb/geolink2oereb.svg?branch=master
-   :target: https://travis-ci.org/openoereb/geolink2oereb
-.. |coverage report| image:: https://codecov.io/gh/openoereb/geolink2oereb/branch/master/graph/badge.svg
-   :target: https://codecov.io/gh/openoereb/geolink2oereb
-.. |dependencies| image:: https://img.shields.io/librariesio/github/openoereb/geolink2oereb.svg
-   :target: https://libraries.io/github/openoereb/geolink2oereb
-.. |code quality| image:: https://api.codacy.com/project/badge/Grade/d2bb03f17bf3438cb295c0b5ea131ac8
-   :target: https://www.codacy.com/app/openoereb/geolink2oereb?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=openoereb/geolink2oereb&amp;utm_campaign=Badge_Grade
+For detailed information, please refer to the online
+[documentation](https://openoereb.github.io/geolink2oereb/).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geolink2oereb-0.0.1/setup.py` & `geolink2oereb-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,18 +20,19 @@
     'WebTest >= 1.3.1',  # py3 compat
     'pytest',  # includes virtualenv
     'pytest-cov'
 ]
 
 setup(
     name='geolink2oereb',
-    version='0.0.1',
+    version='0.1.0',
     description='Transforms a geolink to OeREBKRMtrsfr_V2_0 document entities',
     license='BSD',
     long_description='{readme}\n\n{changelog}'.format(readme=readme, changelog=changelog),
+    long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.10",
```

### Comparing `geolink2oereb-0.0.1/src/geolink2oereb/cli.py` & `geolink2oereb-0.1.0/src/geolink2oereb/cli.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.0.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py` & `geolink2oereb-0.1.0/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/classes.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.0.1/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py` & `geolink2oereb-0.1.0/src/geolink2oereb/lib/interfaces/oerebkrmtrsfr/v2_0/generators.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.0.1/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py` & `geolink2oereb-0.1.0/src/geolink2oereb/lib/interfaces/pyramid_oereb/__init__.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.0.1/src/geolink2oereb/transform.py` & `geolink2oereb-0.1.0/src/geolink2oereb/transform.py`

 * *Files identical despite different names*

### Comparing `geolink2oereb-0.0.1/src/geolink2oereb.egg-info/SOURCES.txt` & `geolink2oereb-0.1.0/src/geolink2oereb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

