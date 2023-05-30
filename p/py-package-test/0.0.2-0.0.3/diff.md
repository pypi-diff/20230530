# Comparing `tmp/py_package_test-0.0.2.tar.gz` & `tmp/py_package_test-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_package_test-0.0.2.tar", last modified: Tue May 30 00:33:33 2023, max compression
+gzip compressed data, was "py_package_test-0.0.3.tar", last modified: Tue May 30 00:58:56 2023, max compression
```

## Comparing `py_package_test-0.0.2.tar` & `py_package_test-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 00:33:33.352779 py_package_test-0.0.2/
--rw-rw-rw-   0        0        0      524 2023-05-30 00:33:33.352779 py_package_test-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 00:33:33.322779 py_package_test-0.0.2/py_package_test/
--rw-rw-rw-   0        0        0        0 2023-05-30 00:32:04.000000 py_package_test-0.0.2/py_package_test/__init__.py
--rw-rw-rw-   0        0        0       33 2023-05-30 00:13:18.000000 py_package_test-0.0.2/py_package_test/add.py
-drwxrwxrwx   0        0        0        0 2023-05-30 00:33:33.349780 py_package_test-0.0.2/py_package_test/extras/
--rw-rw-rw-   0        0        0       56 2023-05-30 00:12:28.000000 py_package_test-0.0.2/py_package_test/extras/__init__.py
--rw-rw-rw-   0        0        0       36 2023-05-30 00:14:01.000000 py_package_test-0.0.2/py_package_test/extras/divide.py
--rw-rw-rw-   0        0        0       38 2023-05-30 00:14:06.000000 py_package_test-0.0.2/py_package_test/extras/multiply.py
--rw-rw-rw-   0        0        0       33 2023-05-30 00:13:33.000000 py_package_test-0.0.2/py_package_test/sub.py
-drwxrwxrwx   0        0        0        0 2023-05-30 00:33:33.340781 py_package_test-0.0.2/py_package_test.egg-info/
--rw-rw-rw-   0        0        0      524 2023-05-30 00:33:33.000000 py_package_test-0.0.2/py_package_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-30 00:33:33.000000 py_package_test-0.0.2/py_package_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 00:33:33.000000 py_package_test-0.0.2/py_package_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-30 00:33:33.000000 py_package_test-0.0.2/py_package_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 00:33:33.353783 py_package_test-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1051 2023-05-30 00:33:28.000000 py_package_test-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:58:56.294697 py_package_test-0.0.3/
+-rw-rw-rw-   0        0        0      524 2023-05-30 00:58:56.292729 py_package_test-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 00:58:56.248736 py_package_test-0.0.3/py_package_test/
+-rw-rw-rw-   0        0        0       42 2023-05-30 00:58:36.000000 py_package_test-0.0.3/py_package_test/__init__.py
+-rw-rw-rw-   0        0        0       33 2023-05-30 00:57:33.000000 py_package_test-0.0.3/py_package_test/add.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:58:56.287723 py_package_test-0.0.3/py_package_test/extras/
+-rw-rw-rw-   0        0        0       56 2023-05-30 00:12:28.000000 py_package_test-0.0.3/py_package_test/extras/__init__.py
+-rw-rw-rw-   0        0        0       36 2023-05-30 00:14:01.000000 py_package_test-0.0.3/py_package_test/extras/divide.py
+-rw-rw-rw-   0        0        0       38 2023-05-30 00:14:06.000000 py_package_test-0.0.3/py_package_test/extras/multiply.py
+-rw-rw-rw-   0        0        0       33 2023-05-30 00:57:43.000000 py_package_test-0.0.3/py_package_test/sub.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:58:56.272700 py_package_test-0.0.3/py_package_test.egg-info/
+-rw-rw-rw-   0        0        0      524 2023-05-30 00:58:55.000000 py_package_test-0.0.3/py_package_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-30 00:58:56.000000 py_package_test-0.0.3/py_package_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 00:58:55.000000 py_package_test-0.0.3/py_package_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-30 00:58:55.000000 py_package_test-0.0.3/py_package_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 00:58:56.294697 py_package_test-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1051 2023-05-30 00:58:48.000000 py_package_test-0.0.3/setup.py
```

### Comparing `py_package_test-0.0.2/PKG-INFO` & `py_package_test-0.0.3/py_package_test.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_package_test
-Version: 0.0.2
+Name: py-package-test
+Version: 0.0.3
 Summary: Py package test
 Author: Sanjay
 Author-email: youremail@email.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `py_package_test-0.0.2/py_package_test.egg-info/PKG-INFO` & `py_package_test-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-package-test
-Version: 0.0.2
+Name: py_package_test
+Version: 0.0.3
 Summary: Py package test
 Author: Sanjay
 Author-email: youremail@email.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `py_package_test-0.0.2/setup.py` & `py_package_test-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'Py package test'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="py_package_test",
```

