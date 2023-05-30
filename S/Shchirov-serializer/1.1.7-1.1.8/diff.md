# Comparing `tmp/Shchirov_serializer-1.1.7.tar.gz` & `tmp/Shchirov_serializer-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shchirov_serializer-1.1.7.tar", last modified: Tue May 30 21:38:01 2023, max compression
+gzip compressed data, was "Shchirov_serializer-1.1.8.tar", last modified: Tue May 30 21:52:59 2023, max compression
```

## Comparing `Shchirov_serializer-1.1.7.tar` & `Shchirov_serializer-1.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:38:01.092031 Shchirov_serializer-1.1.7/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:38:01.092031 Shchirov_serializer-1.1.7/PKG-INFO
--rw-r--r--   0 pavel     (1000) pavel     (1000)       66 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.7/README.md
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:38:01.088031 Shchirov_serializer-1.1.7/Shchirov_serializer.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:38:01.000000 Shchirov_serializer-1.1.7/Shchirov_serializer.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      693 2023-05-30 21:38:01.000000 Shchirov_serializer-1.1.7/Shchirov_serializer.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-05-30 21:38:01.000000 Shchirov_serializer-1.1.7/Shchirov_serializer.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        9 2023-05-30 21:38:01.000000 Shchirov_serializer-1.1.7/Shchirov_serializer.egg-info/requires.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       84 2023-05-30 21:38:01.000000 Shchirov_serializer-1.1.7/Shchirov_serializer.egg-info/top_level.txt
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:38:01.088031 Shchirov_serializer-1.1.7/serializers/
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.7/serializers/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:38:01.092031 Shchirov_serializer-1.1.7/serializers/base/
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.7/serializers/base/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     2780 2023-05-30 17:50:06.000000 Shchirov_serializer-1.1.7/serializers/base/constants.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     5479 2023-05-30 19:38:26.000000 Shchirov_serializer-1.1.7/serializers/base/deserialization.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     5488 2023-05-30 20:58:37.000000 Shchirov_serializer-1.1.7/serializers/base/serialization.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)      455 2023-05-30 21:08:16.000000 Shchirov_serializer-1.1.7/serializers/factory.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:38:01.092031 Shchirov_serializer-1.1.7/serializers/json_serializer/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     3210 2023-05-30 21:13:36.000000 Shchirov_serializer-1.1.7/serializers/json_serializer/JsonSerializer.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.7/serializers/json_serializer/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     1313 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.7/serializers/json_serializer/serialization_logic.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:38:01.092031 Shchirov_serializer-1.1.7/serializers/xml_serializer/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     3748 2023-05-30 19:42:12.000000 Shchirov_serializer-1.1.7/serializers/xml_serializer/XmlSerializer.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.7/serializers/xml_serializer/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     1430 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.7/serializers/xml_serializer/serialization_logic.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2023-05-30 21:38:01.092031 Shchirov_serializer-1.1.7/setup.cfg
--rw-r--r--   0 pavel     (1000) pavel     (1000)      612 2023-05-30 21:37:58.000000 Shchirov_serializer-1.1.7/setup.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:38:01.092031 Shchirov_serializer-1.1.7/tests/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     8041 2023-05-30 21:18:45.000000 Shchirov_serializer-1.1.7/tests/tests.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:52:59.196190 Shchirov_serializer-1.1.8/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:52:59.196190 Shchirov_serializer-1.1.8/PKG-INFO
+-rw-r--r--   0 pavel     (1000) pavel     (1000)       66 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.8/README.md
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:52:59.192190 Shchirov_serializer-1.1.8/Shchirov_serializer.egg-info/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:52:59.000000 Shchirov_serializer-1.1.8/Shchirov_serializer.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      693 2023-05-30 21:52:59.000000 Shchirov_serializer-1.1.8/Shchirov_serializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-05-30 21:52:59.000000 Shchirov_serializer-1.1.8/Shchirov_serializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        6 2023-05-30 21:52:59.000000 Shchirov_serializer-1.1.8/Shchirov_serializer.egg-info/requires.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       84 2023-05-30 21:52:59.000000 Shchirov_serializer-1.1.8/Shchirov_serializer.egg-info/top_level.txt
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:52:59.192190 Shchirov_serializer-1.1.8/serializers/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.8/serializers/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:52:59.192190 Shchirov_serializer-1.1.8/serializers/base/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.8/serializers/base/__init__.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     2780 2023-05-30 17:50:06.000000 Shchirov_serializer-1.1.8/serializers/base/constants.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     5479 2023-05-30 19:38:26.000000 Shchirov_serializer-1.1.8/serializers/base/deserialization.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     5488 2023-05-30 20:58:37.000000 Shchirov_serializer-1.1.8/serializers/base/serialization.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)      455 2023-05-30 21:08:16.000000 Shchirov_serializer-1.1.8/serializers/factory.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:52:59.196190 Shchirov_serializer-1.1.8/serializers/json_serializer/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     3210 2023-05-30 21:13:36.000000 Shchirov_serializer-1.1.8/serializers/json_serializer/JsonSerializer.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.8/serializers/json_serializer/__init__.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     1313 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.8/serializers/json_serializer/serialization_logic.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:52:59.196190 Shchirov_serializer-1.1.8/serializers/xml_serializer/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     3748 2023-05-30 19:42:12.000000 Shchirov_serializer-1.1.8/serializers/xml_serializer/XmlSerializer.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.8/serializers/xml_serializer/__init__.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     1430 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.8/serializers/xml_serializer/serialization_logic.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2023-05-30 21:52:59.196190 Shchirov_serializer-1.1.8/setup.cfg
+-rw-r--r--   0 pavel     (1000) pavel     (1000)      597 2023-05-30 21:52:54.000000 Shchirov_serializer-1.1.8/setup.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:52:59.196190 Shchirov_serializer-1.1.8/tests/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     8041 2023-05-30 21:18:45.000000 Shchirov_serializer-1.1.8/tests/tests.py
```

### Comparing `Shchirov_serializer-1.1.7/Shchirov_serializer.egg-info/SOURCES.txt` & `Shchirov_serializer-1.1.8/Shchirov_serializer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.7/serializers/base/constants.py` & `Shchirov_serializer-1.1.8/serializers/base/constants.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.7/serializers/base/deserialization.py` & `Shchirov_serializer-1.1.8/serializers/base/deserialization.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.7/serializers/base/serialization.py` & `Shchirov_serializer-1.1.8/serializers/base/serialization.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.7/serializers/json_serializer/JsonSerializer.py` & `Shchirov_serializer-1.1.8/serializers/json_serializer/JsonSerializer.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.7/serializers/json_serializer/serialization_logic.py` & `Shchirov_serializer-1.1.8/serializers/json_serializer/serialization_logic.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.7/serializers/xml_serializer/XmlSerializer.py` & `Shchirov_serializer-1.1.8/serializers/xml_serializer/XmlSerializer.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.7/serializers/xml_serializer/serialization_logic.py` & `Shchirov_serializer-1.1.8/serializers/xml_serializer/serialization_logic.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.7/setup.py` & `Shchirov_serializer-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import setup
 
 
 setup(
     name="Shchirov_serializer",
-    version="1.1.7",
+    version="1.1.8",
     description="python library for serialization",
     url="https://github.com/PaShampusik/PythonLabs/Lab_3",
     author="PaShampusik",
     author_email="shchirovpavel@gmail.com",
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ],
     install_requires = [
-        'regex', 
-        're'
+        'regex'
     ],
     packages=["serializers/json_serializer", "serializers/base",
               "serializers/xml_serializer", "serializers"],
     include_package_data=True
 )
```

### Comparing `Shchirov_serializer-1.1.7/tests/tests.py` & `Shchirov_serializer-1.1.8/tests/tests.py`

 * *Files identical despite different names*

