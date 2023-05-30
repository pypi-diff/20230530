# Comparing `tmp/serializer_Konchik-0.1.7.tar.gz` & `tmp/serializer_Konchik-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializer_Konchik-0.1.7.tar", last modified: Thu May 25 17:53:58 2023, max compression
+gzip compressed data, was "serializer_Konchik-0.1.8.tar", last modified: Tue May 30 19:18:59 2023, max compression
```

## Comparing `serializer_Konchik-0.1.7.tar` & `serializer_Konchik-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 17:53:58.217330 serializer_Konchik-0.1.7/
--rw-rw-rw-   0        0        0      262 2023-05-25 17:53:58.217330 serializer_Konchik-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-25 17:53:58.189362 serializer_Konchik-0.1.7/serializer_Konchik/
--rw-rw-rw-   0        0        0      176 2023-05-25 17:45:04.000000 serializer_Konchik-0.1.7/serializer_Konchik/__init__.py
--rw-rw-rw-   0        0        0     2740 2023-05-24 17:05:42.000000 serializer_Konchik-0.1.7/serializer_Konchik/constants.py
--rw-rw-rw-   0        0        0      116 2023-05-24 17:50:50.000000 serializer_Konchik-0.1.7/serializer_Konchik/is_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:53:58.211408 serializer_Konchik-0.1.7/serializer_Konchik/packer/
--rw-rw-rw-   0        0        0      110 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.7/serializer_Konchik/packer/__init__.py
--rw-rw-rw-   0        0        0     5514 2023-05-25 17:46:37.000000 serializer_Konchik-0.1.7/serializer_Konchik/packer/packer.py
--rw-rw-rw-   0        0        0     5477 2023-05-24 17:46:20.000000 serializer_Konchik-0.1.7/serializer_Konchik/packer/unpacker.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:53:58.216329 serializer_Konchik-0.1.7/serializer_Konchik/serializer/
--rw-rw-rw-   0        0        0      226 2023-05-25 17:45:28.000000 serializer_Konchik-0.1.7/serializer_Konchik/serializer/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-05-22 16:01:32.000000 serializer_Konchik-0.1.7/serializer_Konchik/serializer/base_serializer.py
--rw-rw-rw-   0        0        0     3331 2023-05-25 17:45:51.000000 serializer_Konchik-0.1.7/serializer_Konchik/serializer/json_serializer.py
--rw-rw-rw-   0        0        0      732 2023-05-25 17:46:20.000000 serializer_Konchik-0.1.7/serializer_Konchik/serializer/serializer_factory.py
--rw-rw-rw-   0        0        0     3884 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.7/serializer_Konchik/serializer/xml_serializer.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:53:58.208366 serializer_Konchik-0.1.7/serializer_Konchik.egg-info/
--rw-rw-rw-   0        0        0      262 2023-05-25 17:53:58.000000 serializer_Konchik-0.1.7/serializer_Konchik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      667 2023-05-25 17:53:58.000000 serializer_Konchik-0.1.7/serializer_Konchik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 17:53:58.000000 serializer_Konchik-0.1.7/serializer_Konchik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-25 17:53:58.000000 serializer_Konchik-0.1.7/serializer_Konchik.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-25 17:53:58.000000 serializer_Konchik-0.1.7/serializer_Konchik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 17:53:58.217330 serializer_Konchik-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      595 2023-05-25 17:48:59.000000 serializer_Konchik-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:18:59.575880 serializer_Konchik-0.1.8/
+-rw-rw-rw-   0        0        0      287 2023-05-30 19:18:59.575880 serializer_Konchik-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 19:18:59.545880 serializer_Konchik-0.1.8/serializer_Konchik/
+-rw-rw-rw-   0        0        0      176 2023-05-25 17:45:04.000000 serializer_Konchik-0.1.8/serializer_Konchik/__init__.py
+-rw-rw-rw-   0        0        0     2740 2023-05-30 19:08:58.000000 serializer_Konchik-0.1.8/serializer_Konchik/constants.py
+-rw-rw-rw-   0        0        0      116 2023-05-24 17:50:50.000000 serializer_Konchik-0.1.8/serializer_Konchik/is_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:18:59.561880 serializer_Konchik-0.1.8/serializer_Konchik/packer/
+-rw-rw-rw-   0        0        0      110 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.8/serializer_Konchik/packer/__init__.py
+-rw-rw-rw-   0        0        0     5514 2023-05-30 19:07:21.000000 serializer_Konchik-0.1.8/serializer_Konchik/packer/packer.py
+-rw-rw-rw-   0        0        0     5477 2023-05-30 19:09:04.000000 serializer_Konchik-0.1.8/serializer_Konchik/packer/unpacker.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:18:59.574880 serializer_Konchik-0.1.8/serializer_Konchik/serializer/
+-rw-rw-rw-   0        0        0      226 2023-05-25 17:45:28.000000 serializer_Konchik-0.1.8/serializer_Konchik/serializer/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-05-22 16:01:32.000000 serializer_Konchik-0.1.8/serializer_Konchik/serializer/base_serializer.py
+-rw-rw-rw-   0        0        0     3333 2023-05-30 14:24:01.000000 serializer_Konchik-0.1.8/serializer_Konchik/serializer/json_serializer.py
+-rw-rw-rw-   0        0        0      732 2023-05-25 17:46:20.000000 serializer_Konchik-0.1.8/serializer_Konchik/serializer/serializer_factory.py
+-rw-rw-rw-   0        0        0     3884 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.8/serializer_Konchik/serializer/xml_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:18:59.559894 serializer_Konchik-0.1.8/serializer_Konchik.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-05-30 19:18:59.000000 serializer_Konchik-0.1.8/serializer_Konchik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2023-05-30 19:18:59.000000 serializer_Konchik-0.1.8/serializer_Konchik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 19:18:59.000000 serializer_Konchik-0.1.8/serializer_Konchik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 19:18:59.000000 serializer_Konchik-0.1.8/serializer_Konchik.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-30 19:18:59.000000 serializer_Konchik-0.1.8/serializer_Konchik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 19:18:59.575880 serializer_Konchik-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      626 2023-05-30 19:18:17.000000 serializer_Konchik-0.1.8/setup.py
```

### Comparing `serializer_Konchik-0.1.7/serializer_Konchik/constants.py` & `serializer_Konchik-0.1.8/serializer_Konchik/constants.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.7/serializer_Konchik/packer/packer.py` & `serializer_Konchik-0.1.8/serializer_Konchik/packer/packer.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.7/serializer_Konchik/packer/unpacker.py` & `serializer_Konchik-0.1.8/serializer_Konchik/packer/unpacker.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.7/serializer_Konchik/serializer/base_serializer.py` & `serializer_Konchik-0.1.8/serializer_Konchik/serializer/base_serializer.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.7/serializer_Konchik/serializer/json_serializer.py` & `serializer_Konchik-0.1.8/serializer_Konchik/serializer/json_serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 
         packed: dict = self._deconvert(string)
         return Unpacker.unpack(packed)
 
     def _convert(self, obj: dict) -> str:
         """
         Convert dictionary that represents object
-        to a string of 'XML' format
+        to a string of 'JSON' format
 
         :param obj: Dictionary that represents object.
         :type obj: dict
 
-        :return: String of 'XML' format.
+        :return: String of 'JSON' format.
         :rtype: str
         """
 
         if isinstance(obj, PRIMITIVES):
             if isinstance(obj, str):
                 return '"' + obj.replace("\\", "\\\\").replace('"', "\"").replace("'", "\'") + '"'
             else:
```

### Comparing `serializer_Konchik-0.1.7/serializer_Konchik/serializer/serializer_factory.py` & `serializer_Konchik-0.1.8/serializer_Konchik/serializer/serializer_factory.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.7/serializer_Konchik/serializer/xml_serializer.py` & `serializer_Konchik-0.1.8/serializer_Konchik/serializer/xml_serializer.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.7/serializer_Konchik.egg-info/SOURCES.txt` & `serializer_Konchik-0.1.8/serializer_Konchik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.7/setup.py` & `serializer_Konchik-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Always prefer setuptools over distutils
 from setuptools import setup
 
 # This call to setup() does all the work
 setup(
     name="serializer_Konchik",
-    version="0.1.7",
+    version="0.1.8",
     description="JSON / XML serializer",
     author="Denis Konchik",
     author_email="denis.pptx@gmail.com",
     license="MIT",
     classifiers=[
         "Programming Language :: Python",
         "Operating System :: OS Independent"
     ],
+    python_requires='>=3.11',
     packages=["serializer_Konchik", "serializer_Konchik.packer", "serializer_Konchik.serializer"],
     include_package_data=True,
     install_requires=["regex"]
 )
```

