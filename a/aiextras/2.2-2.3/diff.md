# Comparing `tmp/aiextras-2.2.tar.gz` & `tmp/aiextras-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aiextras-2.2.tar", last modified: Tue May 30 02:29:51 2023, max compression
+gzip compressed data, was "dist\aiextras-2.3.tar", last modified: Tue May 30 02:31:31 2023, max compression
```

## Comparing `aiextras-2.2.tar` & `aiextras-2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 02:29:51.000000 aiextras-2.2/
--rw-rw-rw-   0        0        0        0 2023-05-22 03:45:14.000000 aiextras-2.2/LICENSE
--rw-rw-rw-   0        0        0      336 2023-05-30 02:29:51.000000 aiextras-2.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-20 09:12:45.000000 aiextras-2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 02:29:51.000000 aiextras-2.2/aiextras/
-drwxrwxrwx   0        0        0        0 2023-05-30 02:29:51.000000 aiextras-2.2/aiextras/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 02:29:51.000000 aiextras-2.2/aiextras/src/aiextras.egg-info/
--rw-rw-rw-   0        0        0      336 2023-05-30 02:29:51.000000 aiextras-2.2/aiextras/src/aiextras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-05-30 02:29:51.000000 aiextras-2.2/aiextras/src/aiextras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 02:29:51.000000 aiextras-2.2/aiextras/src/aiextras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 02:29:51.000000 aiextras-2.2/aiextras/src/aiextras.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    82951 2023-05-30 02:29:41.000000 aiextras-2.2/aiextras/src/aiextras.py
--rw-rw-rw-   0        0        0       86 2023-05-30 02:29:51.000000 aiextras-2.2/setup.cfg
--rw-rw-rw-   0        0        0     1204 2023-05-30 02:29:47.000000 aiextras-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:31:31.000000 aiextras-2.3/
+-rw-rw-rw-   0        0        0        0 2023-05-22 03:45:14.000000 aiextras-2.3/LICENSE
+-rw-rw-rw-   0        0        0      336 2023-05-30 02:31:31.000000 aiextras-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-20 09:12:45.000000 aiextras-2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 02:31:31.000000 aiextras-2.3/aiextras/
+drwxrwxrwx   0        0        0        0 2023-05-30 02:31:31.000000 aiextras-2.3/aiextras/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 02:31:31.000000 aiextras-2.3/aiextras/src/aiextras.egg-info/
+-rw-rw-rw-   0        0        0      336 2023-05-30 02:31:31.000000 aiextras-2.3/aiextras/src/aiextras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-05-30 02:31:31.000000 aiextras-2.3/aiextras/src/aiextras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 02:31:31.000000 aiextras-2.3/aiextras/src/aiextras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 02:31:31.000000 aiextras-2.3/aiextras/src/aiextras.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    82930 2023-05-30 02:31:16.000000 aiextras-2.3/aiextras/src/aiextras.py
+-rw-rw-rw-   0        0        0       86 2023-05-30 02:31:31.000000 aiextras-2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1204 2023-05-30 02:31:28.000000 aiextras-2.3/setup.py
```

### Comparing `aiextras-2.2/aiextras/src/aiextras.py` & `aiextras-2.3/aiextras/src/aiextras.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import srp as srp
-
 srp_exp1a = '''
 from numpy import median
 from sklearn.ensemble import GradientBoostingClassifier
 from sklearn.ensemble import RandomForestClassifier
 from sklearn import svm
 from sklearn.linear_model import LogisticRegression
 from sklearn import metrics
```

### Comparing `aiextras-2.2/setup.py` & `aiextras-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiextras",                     # This is the name of the package
-    version="2.2",                        # The initial release version
+    version="2.3",                        # The initial release version
     author="AnupamKris",                     # Full name of the author
     description="AI2LAB Programs",
     # Long description read from the the readme file
     long_description=long_description,
     long_description_content_type="text/markdown",
     # List of all python modules to be installed
     packages=setuptools.find_packages(),
```

