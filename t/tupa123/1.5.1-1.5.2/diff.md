# Comparing `tmp/tupa123-1.5.1.tar.gz` & `tmp/tupa123-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.5.1.tar", last modified: Mon May 29 20:44:41 2023, max compression
+gzip compressed data, was "tupa123-1.5.2.tar", last modified: Tue May 30 20:23:43 2023, max compression
```

## Comparing `tupa123-1.5.1.tar` & `tupa123-1.5.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 20:44:41.000449 tupa123-1.5.1/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-05-29 20:44:41.000449 tupa123-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 20:44:41.000449 tupa123-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0      837 2023-05-29 20:43:58.000000 tupa123-1.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:44:40.990447 tupa123-1.5.1/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.5.1/tupa123/__init__.py
--rw-rw-rw-   0        0        0   172319 2023-05-29 13:46:41.000000 tupa123-1.5.1/tupa123/machine1.txt
--rw-rw-rw-   0        0        0    89844 2023-05-29 20:11:26.000000 tupa123-1.5.1/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:44:41.000449 tupa123-1.5.1/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-05-29 20:44:40.000000 tupa123-1.5.1/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-29 20:44:40.000000 tupa123-1.5.1/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 20:44:40.000000 tupa123-1.5.1/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-29 20:44:40.000000 tupa123-1.5.1/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-29 20:44:40.000000 tupa123-1.5.1/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 20:23:43.149899 tupa123-1.5.2/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-05-30 20:23:43.149899 tupa123-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 20:23:43.149899 tupa123-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      833 2023-05-30 20:23:25.000000 tupa123-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:23:43.149899 tupa123-1.5.2/tupa123/
+-rw-rw-rw-   0        0        0       47 2023-05-30 20:06:06.000000 tupa123-1.5.2/tupa123/__init__.py
+-rw-rw-rw-   0        0        0   172319 2023-05-29 13:46:41.000000 tupa123-1.5.2/tupa123/machine1.txt
+-rw-rw-rw-   0        0        0    50672 2023-05-30 19:47:13.000000 tupa123-1.5.2/tupa123/tupa12.py
+-rw-rw-rw-   0        0        0    89844 2023-05-29 20:11:26.000000 tupa123-1.5.2/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:23:43.149899 tupa123-1.5.2/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-05-30 20:23:42.000000 tupa123-1.5.2/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-30 20:23:43.000000 tupa123-1.5.2/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 20:23:42.000000 tupa123-1.5.2/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-30 20:23:42.000000 tupa123-1.5.2/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 20:23:42.000000 tupa123-1.5.2/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.5.1/LICENSE.txt` & `tupa123-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.1/PKG-INFO` & `tupa123-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.5.1
+Version: 1.5.2
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.5.1/README.md` & `tupa123-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.1/setup.py` & `tupa123-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.5.1',
+    version='1.5.2',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
-    packages=['tupa123'],    
+    packages=['tupa123'],
     package_data={'tupa123': ['machine1.txt'],},    
     install_requires=['numpy','matplotlib','pandas','opencv-python'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `tupa123-1.5.1/tupa123/machine1.txt` & `tupa123-1.5.2/tupa123/machine1.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.1/tupa123/tupa123.py` & `tupa123-1.5.2/tupa123/tupa123.py`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.1/tupa123.egg-info/PKG-INFO` & `tupa123-1.5.2/tupa123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.5.1
+Version: 1.5.2
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

