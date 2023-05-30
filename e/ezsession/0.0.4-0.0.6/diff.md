# Comparing `tmp/ezsession-0.0.4.tar.gz` & `tmp/ezsession-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezsession-0.0.4.tar", last modified: Fri May 26 14:45:39 2023, max compression
+gzip compressed data, was "ezsession-0.0.6.tar", last modified: Tue May 30 16:36:26 2023, max compression
```

## Comparing `ezsession-0.0.4.tar` & `ezsession-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:45:39.253608 ezsession-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-26 14:45:39.253608 ezsession-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-26 14:45:28.000000 ezsession-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-26 14:45:28.000000 ezsession-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-26 14:45:39.253608 ezsession-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-26 14:45:28.000000 ezsession-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:45:39.249608 ezsession-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:45:39.249608 ezsession-0.0.4/src/ezsession/
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-26 14:45:28.000000 ezsession-0.0.4/src/ezsession/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:45:39.253608 ezsession-0.0.4/src/ezsession.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-26 14:45:39.000000 ezsession-0.0.4/src/ezsession.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-26 14:45:39.000000 ezsession-0.0.4/src/ezsession.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:45:39.000000 ezsession-0.0.4/src/ezsession.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 14:45:39.000000 ezsession-0.0.4/src/ezsession.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:26.982659 ezsession-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 16:36:13.000000 ezsession-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-30 16:36:26.982659 ezsession-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-30 16:36:13.000000 ezsession-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 16:36:13.000000 ezsession-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 16:36:13.000000 ezsession-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:36:26.982659 ezsession-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-30 16:36:13.000000 ezsession-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:26.982659 ezsession-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:26.982659 ezsession-0.0.6/src/ezsession/
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-30 16:36:13.000000 ezsession-0.0.6/src/ezsession/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:26.982659 ezsession-0.0.6/src/ezsession.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-30 16:36:26.000000 ezsession-0.0.6/src/ezsession.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-30 16:36:26.000000 ezsession-0.0.6/src/ezsession.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:36:26.000000 ezsession-0.0.6/src/ezsession.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 16:36:26.000000 ezsession-0.0.6/src/ezsession.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 16:36:26.000000 ezsession-0.0.6/src/ezsession.egg-info/top_level.txt
```

### Comparing `ezsession-0.0.4/PKG-INFO` & `ezsession-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsession
-Version: 0.0.4
+Version: 0.0.6
 Summary: A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.
 Author: Josh XT
 Author-email: josh@devxt.com
 Description-Content-Type: text/markdown
 
 # ezsession
 A small useful Python module to abstract away the common auth header methods used by different software vendors.  The output is a requests session with the authentication headers built in.
```

### Comparing `ezsession-0.0.4/README.md` & `ezsession-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ezsession-0.0.4/setup.py` & `ezsession-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 import os
 
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
+with open(os.path.join(this_directory, "requirements.txt")) as f:
+    requirements = f.read().splitlines()
+
 setup(
     name="ezsession",
-    version="0.0.4",
+    version="0.0.6",
     description="A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
+    install_requires=requirements,
 )
```

### Comparing `ezsession-0.0.4/src/ezsession/__init__.py` & `ezsession-0.0.6/src/ezsession/__init__.py`

 * *Files identical despite different names*

### Comparing `ezsession-0.0.4/src/ezsession.egg-info/PKG-INFO` & `ezsession-0.0.6/src/ezsession.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsession
-Version: 0.0.4
+Version: 0.0.6
 Summary: A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.
 Author: Josh XT
 Author-email: josh@devxt.com
 Description-Content-Type: text/markdown
 
 # ezsession
 A small useful Python module to abstract away the common auth header methods used by different software vendors.  The output is a requests session with the authentication headers built in.
```

