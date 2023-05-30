# Comparing `tmp/Shchirov_serializer-1.1.4.tar.gz` & `tmp/Shchirov_serializer-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shchirov_serializer-1.1.4.tar", last modified: Tue May 30 21:19:22 2023, max compression
+gzip compressed data, was "Shchirov_serializer-1.1.5.tar", last modified: Tue May 30 21:23:35 2023, max compression
```

## Comparing `Shchirov_serializer-1.1.4.tar` & `Shchirov_serializer-1.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/PKG-INFO
--rw-r--r--   0 pavel     (1000) pavel     (1000)       66 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/README.md
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/Shchirov_serializer.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:19:22.000000 Shchirov_serializer-1.1.4/Shchirov_serializer.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      651 2023-05-30 21:19:22.000000 Shchirov_serializer-1.1.4/Shchirov_serializer.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-05-30 21:19:22.000000 Shchirov_serializer-1.1.4/Shchirov_serializer.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       84 2023-05-30 21:19:22.000000 Shchirov_serializer-1.1.4/Shchirov_serializer.egg-info/top_level.txt
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/serializers/
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/serializers/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/serializers/base/
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/serializers/base/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     2780 2023-05-30 17:50:06.000000 Shchirov_serializer-1.1.4/serializers/base/constants.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     5479 2023-05-30 19:38:26.000000 Shchirov_serializer-1.1.4/serializers/base/deserialization.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     5488 2023-05-30 20:58:37.000000 Shchirov_serializer-1.1.4/serializers/base/serialization.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)      455 2023-05-30 21:08:16.000000 Shchirov_serializer-1.1.4/serializers/factory.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/serializers/json_serializer/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     3210 2023-05-30 21:13:36.000000 Shchirov_serializer-1.1.4/serializers/json_serializer/JsonSerializer.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/serializers/json_serializer/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     1313 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/serializers/json_serializer/serialization_logic.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/serializers/xml_serializer/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     3748 2023-05-30 19:42:12.000000 Shchirov_serializer-1.1.4/serializers/xml_serializer/XmlSerializer.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/serializers/xml_serializer/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     1430 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.4/serializers/xml_serializer/serialization_logic.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/setup.cfg
--rw-r--r--   0 pavel     (1000) pavel     (1000)      549 2023-05-30 21:19:21.000000 Shchirov_serializer-1.1.4/setup.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:19:22.884149 Shchirov_serializer-1.1.4/tests/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     8041 2023-05-30 21:18:45.000000 Shchirov_serializer-1.1.4/tests/tests.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:23:35.870314 Shchirov_serializer-1.1.5/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:23:35.866314 Shchirov_serializer-1.1.5/PKG-INFO
+-rw-r--r--   0 pavel     (1000) pavel     (1000)       66 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.5/README.md
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:23:35.866314 Shchirov_serializer-1.1.5/Shchirov_serializer.egg-info/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      320 2023-05-30 21:23:35.000000 Shchirov_serializer-1.1.5/Shchirov_serializer.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      651 2023-05-30 21:23:35.000000 Shchirov_serializer-1.1.5/Shchirov_serializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-05-30 21:23:35.000000 Shchirov_serializer-1.1.5/Shchirov_serializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       84 2023-05-30 21:23:35.000000 Shchirov_serializer-1.1.5/Shchirov_serializer.egg-info/top_level.txt
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:23:35.866314 Shchirov_serializer-1.1.5/serializers/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.5/serializers/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:23:35.866314 Shchirov_serializer-1.1.5/serializers/base/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.5/serializers/base/__init__.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     2780 2023-05-30 17:50:06.000000 Shchirov_serializer-1.1.5/serializers/base/constants.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     5479 2023-05-30 19:38:26.000000 Shchirov_serializer-1.1.5/serializers/base/deserialization.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     5488 2023-05-30 20:58:37.000000 Shchirov_serializer-1.1.5/serializers/base/serialization.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)      455 2023-05-30 21:08:16.000000 Shchirov_serializer-1.1.5/serializers/factory.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:23:35.866314 Shchirov_serializer-1.1.5/serializers/json_serializer/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     3210 2023-05-30 21:13:36.000000 Shchirov_serializer-1.1.5/serializers/json_serializer/JsonSerializer.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.5/serializers/json_serializer/__init__.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     1313 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.5/serializers/json_serializer/serialization_logic.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:23:35.866314 Shchirov_serializer-1.1.5/serializers/xml_serializer/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     3748 2023-05-30 19:42:12.000000 Shchirov_serializer-1.1.5/serializers/xml_serializer/XmlSerializer.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.5/serializers/xml_serializer/__init__.py
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     1430 2023-05-30 17:05:21.000000 Shchirov_serializer-1.1.5/serializers/xml_serializer/serialization_logic.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2023-05-30 21:23:35.870314 Shchirov_serializer-1.1.5/setup.cfg
+-rw-r--r--   0 pavel     (1000) pavel     (1000)      549 2023-05-30 21:23:33.000000 Shchirov_serializer-1.1.5/setup.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-05-30 21:23:35.866314 Shchirov_serializer-1.1.5/tests/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     8041 2023-05-30 21:18:45.000000 Shchirov_serializer-1.1.5/tests/tests.py
```

### Comparing `Shchirov_serializer-1.1.4/Shchirov_serializer.egg-info/SOURCES.txt` & `Shchirov_serializer-1.1.5/Shchirov_serializer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.4/serializers/base/constants.py` & `Shchirov_serializer-1.1.5/serializers/base/constants.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.4/serializers/base/deserialization.py` & `Shchirov_serializer-1.1.5/serializers/base/deserialization.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.4/serializers/base/serialization.py` & `Shchirov_serializer-1.1.5/serializers/base/serialization.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.4/serializers/json_serializer/JsonSerializer.py` & `Shchirov_serializer-1.1.5/serializers/json_serializer/JsonSerializer.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.4/serializers/json_serializer/serialization_logic.py` & `Shchirov_serializer-1.1.5/serializers/json_serializer/serialization_logic.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.4/serializers/xml_serializer/XmlSerializer.py` & `Shchirov_serializer-1.1.5/serializers/xml_serializer/XmlSerializer.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.4/serializers/xml_serializer/serialization_logic.py` & `Shchirov_serializer-1.1.5/serializers/xml_serializer/serialization_logic.py`

 * *Files identical despite different names*

### Comparing `Shchirov_serializer-1.1.4/setup.py` & `Shchirov_serializer-1.1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="Shchirov_serializer",
-    version="1.1.4",
+    version="1.1.5",
     description="python library for serialization",
     url="https://github.com/PaShampusik/PythonLabs/Lab_3",
     author="PaShampusik",
     author_email="shchirovpavel@gmail.com",
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
```

### Comparing `Shchirov_serializer-1.1.4/tests/tests.py` & `Shchirov_serializer-1.1.5/tests/tests.py`

 * *Files identical despite different names*

