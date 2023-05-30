# Comparing `tmp/jsonxmlsatsiuk2-0.1.1.tar.gz` & `tmp/jsonxmlsatsiuk2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonxmlsatsiuk2-0.1.1.tar", last modified: Tue May 30 14:43:26 2023, max compression
+gzip compressed data, was "jsonxmlsatsiuk2-0.1.2.tar", last modified: Tue May 30 14:48:20 2023, max compression
```

## Comparing `jsonxmlsatsiuk2-0.1.1.tar` & `jsonxmlsatsiuk2-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 stanislav   (501) staff       (20)        0 2023-05-30 14:43:26.174797 jsonxmlsatsiuk2-0.1.1/
--rw-r--r--   0 stanislav   (501) staff       (20)      415 2023-05-30 14:43:26.174644 jsonxmlsatsiuk2-0.1.1/PKG-INFO
-drwxr-xr-x   0 stanislav   (501) staff       (20)        0 2023-05-30 14:43:26.172191 jsonxmlsatsiuk2-0.1.1/jsonxmlsatsiuk2.egg-info/
--rw-r--r--   0 stanislav   (501) staff       (20)      415 2023-05-30 14:43:26.000000 jsonxmlsatsiuk2-0.1.1/jsonxmlsatsiuk2.egg-info/PKG-INFO
--rw-r--r--   0 stanislav   (501) staff       (20)      419 2023-05-30 14:43:26.000000 jsonxmlsatsiuk2-0.1.1/jsonxmlsatsiuk2.egg-info/SOURCES.txt
--rw-r--r--   0 stanislav   (501) staff       (20)        1 2023-05-30 14:43:26.000000 jsonxmlsatsiuk2-0.1.1/jsonxmlsatsiuk2.egg-info/dependency_links.txt
--rw-r--r--   0 stanislav   (501) staff       (20)        6 2023-05-30 14:43:26.000000 jsonxmlsatsiuk2-0.1.1/jsonxmlsatsiuk2.egg-info/requires.txt
--rw-r--r--   0 stanislav   (501) staff       (20)       12 2023-05-30 14:43:26.000000 jsonxmlsatsiuk2-0.1.1/jsonxmlsatsiuk2.egg-info/top_level.txt
-drwxr-xr-x   0 stanislav   (501) staff       (20)        0 2023-05-30 14:43:26.173835 jsonxmlsatsiuk2-0.1.1/serializers/
--rw-rw-r--   0 stanislav   (501) staff       (20)      521 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.1/serializers/__init__.py
--rw-rw-r--   0 stanislav   (501) staff       (20)     1209 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.1/serializers/consts.py
--rw-rw-r--   0 stanislav   (501) staff       (20)      347 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.1/serializers/factory.py
--rw-rw-r--   0 stanislav   (501) staff       (20)     9368 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.1/serializers/packing_tool.py
--rw-rw-r--   0 stanislav   (501) staff       (20)      357 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.1/serializers/serializer.py
--rw-rw-r--   0 stanislav   (501) staff       (20)     3863 2023-05-24 15:08:52.000000 jsonxmlsatsiuk2-0.1.1/serializers/serializer_json.py
--rw-rw-r--   0 stanislav   (501) staff       (20)     4070 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.1/serializers/serializer_xml.py
--rw-r--r--   0 stanislav   (501) staff       (20)       38 2023-05-30 14:43:26.174843 jsonxmlsatsiuk2-0.1.1/setup.cfg
--rw-rw-r--   0 stanislav   (501) staff       (20)      557 2023-05-30 14:43:12.000000 jsonxmlsatsiuk2-0.1.1/setup.py
-drwxr-xr-x   0 stanislav   (501) staff       (20)        0 2023-05-30 14:43:26.174327 jsonxmlsatsiuk2-0.1.1/test/
--rw-rw-r--   0 stanislav   (501) staff       (20)     2276 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.1/test/test_value.py
--rw-rw-r--   0 stanislav   (501) staff       (20)     3988 2023-05-24 15:31:57.000000 jsonxmlsatsiuk2-0.1.1/test/tests.py
+drwxr-xr-x   0 stanislav   (501) staff       (20)        0 2023-05-30 14:48:20.722859 jsonxmlsatsiuk2-0.1.2/
+-rw-r--r--   0 stanislav   (501) staff       (20)      415 2023-05-30 14:48:20.722703 jsonxmlsatsiuk2-0.1.2/PKG-INFO
+drwxr-xr-x   0 stanislav   (501) staff       (20)        0 2023-05-30 14:48:20.720366 jsonxmlsatsiuk2-0.1.2/jsonxmlsatsiuk2.egg-info/
+-rw-r--r--   0 stanislav   (501) staff       (20)      415 2023-05-30 14:48:20.000000 jsonxmlsatsiuk2-0.1.2/jsonxmlsatsiuk2.egg-info/PKG-INFO
+-rw-r--r--   0 stanislav   (501) staff       (20)      473 2023-05-30 14:48:20.000000 jsonxmlsatsiuk2-0.1.2/jsonxmlsatsiuk2.egg-info/SOURCES.txt
+-rw-r--r--   0 stanislav   (501) staff       (20)        1 2023-05-30 14:48:20.000000 jsonxmlsatsiuk2-0.1.2/jsonxmlsatsiuk2.egg-info/dependency_links.txt
+-rw-r--r--   0 stanislav   (501) staff       (20)     7576 2023-05-30 14:43:26.000000 jsonxmlsatsiuk2-0.1.2/jsonxmlsatsiuk2.egg-info/jsonxmlsatsiuk2-0.1.2.tar.gz
+-rw-r--r--   0 stanislav   (501) staff       (20)        6 2023-05-30 14:48:20.000000 jsonxmlsatsiuk2-0.1.2/jsonxmlsatsiuk2.egg-info/requires.txt
+-rw-r--r--   0 stanislav   (501) staff       (20)       12 2023-05-30 14:48:20.000000 jsonxmlsatsiuk2-0.1.2/jsonxmlsatsiuk2.egg-info/top_level.txt
+drwxr-xr-x   0 stanislav   (501) staff       (20)        0 2023-05-30 14:48:20.721931 jsonxmlsatsiuk2-0.1.2/serializers/
+-rw-rw-r--   0 stanislav   (501) staff       (20)      521 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.2/serializers/__init__.py
+-rw-rw-r--   0 stanislav   (501) staff       (20)     1209 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.2/serializers/consts.py
+-rw-rw-r--   0 stanislav   (501) staff       (20)      347 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.2/serializers/factory.py
+-rw-rw-r--   0 stanislav   (501) staff       (20)     9368 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.2/serializers/packing_tool.py
+-rw-rw-r--   0 stanislav   (501) staff       (20)      357 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.2/serializers/serializer.py
+-rw-rw-r--   0 stanislav   (501) staff       (20)     3863 2023-05-24 15:08:52.000000 jsonxmlsatsiuk2-0.1.2/serializers/serializer_json.py
+-rw-rw-r--   0 stanislav   (501) staff       (20)     4070 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.2/serializers/serializer_xml.py
+-rw-r--r--   0 stanislav   (501) staff       (20)       38 2023-05-30 14:48:20.722901 jsonxmlsatsiuk2-0.1.2/setup.cfg
+-rw-rw-r--   0 stanislav   (501) staff       (20)      557 2023-05-30 14:47:48.000000 jsonxmlsatsiuk2-0.1.2/setup.py
+drwxr-xr-x   0 stanislav   (501) staff       (20)        0 2023-05-30 14:48:20.722403 jsonxmlsatsiuk2-0.1.2/test/
+-rw-rw-r--   0 stanislav   (501) staff       (20)     2276 2023-05-11 20:15:11.000000 jsonxmlsatsiuk2-0.1.2/test/test_value.py
+-rw-rw-r--   0 stanislav   (501) staff       (20)     3988 2023-05-24 15:31:57.000000 jsonxmlsatsiuk2-0.1.2/test/tests.py
```

### Comparing `jsonxmlsatsiuk2-0.1.1/serializers/__init__.py` & `jsonxmlsatsiuk2-0.1.2/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonxmlsatsiuk2-0.1.1/serializers/consts.py` & `jsonxmlsatsiuk2-0.1.2/serializers/consts.py`

 * *Files identical despite different names*

### Comparing `jsonxmlsatsiuk2-0.1.1/serializers/packing_tool.py` & `jsonxmlsatsiuk2-0.1.2/serializers/packing_tool.py`

 * *Files identical despite different names*

### Comparing `jsonxmlsatsiuk2-0.1.1/serializers/serializer_json.py` & `jsonxmlsatsiuk2-0.1.2/serializers/serializer_json.py`

 * *Files identical despite different names*

### Comparing `jsonxmlsatsiuk2-0.1.1/serializers/serializer_xml.py` & `jsonxmlsatsiuk2-0.1.2/serializers/serializer_xml.py`

 * *Files identical despite different names*

### Comparing `jsonxmlsatsiuk2-0.1.1/setup.py` & `jsonxmlsatsiuk2-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="jsonxmlsatsiuk2",
-    version="0.1.1",
+    version="0.1.2",
     description="Library for python (de)serialization in Json and Xml",
     url="https://github.com/panton8/igi-labs/tree/lab3",
     author="stady09",
     author_email="stassatsiukgg@gmail.com",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
```

### Comparing `jsonxmlsatsiuk2-0.1.1/test/test_value.py` & `jsonxmlsatsiuk2-0.1.2/test/test_value.py`

 * *Files identical despite different names*

### Comparing `jsonxmlsatsiuk2-0.1.1/test/tests.py` & `jsonxmlsatsiuk2-0.1.2/test/tests.py`

 * *Files identical despite different names*

