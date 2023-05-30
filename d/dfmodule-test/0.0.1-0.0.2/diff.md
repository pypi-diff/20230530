# Comparing `tmp/dfmodule_test-0.0.1.tar.gz` & `tmp/dfmodule_test-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule_test-0.0.1.tar", last modified: Tue May 30 13:30:05 2023, max compression
+gzip compressed data, was "dfmodule_test-0.0.2.tar", last modified: Tue May 30 15:02:08 2023, max compression
```

## Comparing `dfmodule_test-0.0.1.tar` & `dfmodule_test-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 13:30:05.869490 dfmodule_test-0.0.1/
--rw-rw-rw-   0        0        0      524 2023-05-30 13:30:05.869490 dfmodule_test-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-05-30 13:10:52.000000 dfmodule_test-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 13:30:05.868491 dfmodule_test-0.0.1/dfmodule_test.egg-info/
--rw-rw-rw-   0        0        0      524 2023-05-30 13:30:05.000000 dfmodule_test-0.0.1/dfmodule_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-05-30 13:30:05.000000 dfmodule_test-0.0.1/dfmodule_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 13:30:05.000000 dfmodule_test-0.0.1/dfmodule_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-30 13:30:05.000000 dfmodule_test-0.0.1/dfmodule_test.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-30 13:30:05.000000 dfmodule_test-0.0.1/dfmodule_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-30 13:30:05.000000 dfmodule_test-0.0.1/dfmodule_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-30 13:30:05.868491 dfmodule_test-0.0.1/sample/
--rw-rw-rw-   0        0        0       45 2023-05-30 12:59:39.000000 dfmodule_test-0.0.1/sample/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-30 13:30:05.869490 dfmodule_test-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      781 2023-05-30 12:48:46.000000 dfmodule_test-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:02:08.423296 dfmodule_test-0.0.2/
+-rw-rw-rw-   0        0        0      524 2023-05-30 15:02:08.422296 dfmodule_test-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-05-30 13:10:52.000000 dfmodule_test-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 15:02:08.421297 dfmodule_test-0.0.2/dfmodule_test.egg-info/
+-rw-rw-rw-   0        0        0      524 2023-05-30 15:02:08.000000 dfmodule_test-0.0.2/dfmodule_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-30 15:02:08.000000 dfmodule_test-0.0.2/dfmodule_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 15:02:08.000000 dfmodule_test-0.0.2/dfmodule_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-30 13:30:05.000000 dfmodule_test-0.0.2/dfmodule_test.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-30 15:02:08.000000 dfmodule_test-0.0.2/dfmodule_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 15:02:08.000000 dfmodule_test-0.0.2/dfmodule_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 15:02:08.422296 dfmodule_test-0.0.2/sample/
+-rw-rw-rw-   0        0        0       96 2023-05-30 14:52:00.000000 dfmodule_test-0.0.2/sample/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-30 15:02:08.423296 dfmodule_test-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      781 2023-05-30 14:56:46.000000 dfmodule_test-0.0.2/setup.py
```

### Comparing `dfmodule_test-0.0.1/PKG-INFO` & `dfmodule_test-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfmodule_test
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple dfmodule example package
 Home-page: http://github.com/yourusername/sample_package
 Author: Your Name
 Author-email: your.email@example.com
 Keywords: dfmodule_test
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dfmodule_test-0.0.1/dfmodule_test.egg-info/PKG-INFO` & `dfmodule_test-0.0.2/dfmodule_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfmodule-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple dfmodule example package
 Home-page: http://github.com/yourusername/sample_package
 Author: Your Name
 Author-email: your.email@example.com
 Keywords: dfmodule_test
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dfmodule_test-0.0.1/setup.py` & `dfmodule_test-0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dfmodule_test",
-    version="0.0.1",
+    version="0.0.2",
     description="A simple dfmodule example package",
     author="Your Name",
     author_email="your.email@example.com",
     url="http://github.com/yourusername/sample_package",
     install_requires=['pandas', 'numpy'],
     packages=find_packages(exclude=['tests*']),
     keywords=['dfmodule_test'],
```

