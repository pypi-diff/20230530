# Comparing `tmp/typed-api-framework-0.0.0.tar.gz` & `tmp/typed-api-framework-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typed-api-framework-0.0.0.tar", last modified: Tue May 30 05:53:16 2023, max compression
+gzip compressed data, was "typed-api-framework-0.0.1a4.tar", last modified: Tue May 30 06:15:39 2023, max compression
```

## Comparing `typed-api-framework-0.0.0.tar` & `typed-api-framework-0.0.1a4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:53:16.559990 typed-api-framework-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-30 05:53:16.559990 typed-api-framework-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 05:53:16.559990 typed-api-framework-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:53:16.555990 typed-api-framework-0.0.0/typedAPI/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:53:16.555990 typed-api-framework-0.0.0/typedAPI/body/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/body/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/body/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/body/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:53:16.555990 typed-api-framework-0.0.0/typedAPI/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/endpoint/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/endpoint/guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/endpoint/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/endpoint/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:53:16.555990 typed-api-framework-0.0.0/typedAPI/headers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/headers/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/headers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/headers/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/headers/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/log_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:53:16.555990 typed-api-framework-0.0.0/typedAPI/resource_path/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/resource_path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/resource_path/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/resource_path/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/resource_path/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:53:16.559990 typed-api-framework-0.0.0/typedAPI/response/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/response/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/response/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/response/factory_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/response/guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/response/guards_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/response/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/response/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/response/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/response/service_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-30 05:53:05.000000 typed-api-framework-0.0.0/typedAPI/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:53:16.559990 typed-api-framework-0.0.0/typed_api_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-30 05:53:16.000000 typed-api-framework-0.0.0/typed_api_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-30 05:53:16.000000 typed-api-framework-0.0.0/typed_api_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 05:53:16.000000 typed-api-framework-0.0.0/typed_api_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 05:53:16.000000 typed-api-framework-0.0.0/typed_api_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:15:39.564857 typed-api-framework-0.0.1a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-30 06:15:39.564857 typed-api-framework-0.0.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:15:39.564857 typed-api-framework-0.0.1a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:15:39.560857 typed-api-framework-0.0.1a4/typedAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:15:39.560857 typed-api-framework-0.0.1a4/typedAPI/body/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/body/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/body/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/body/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:15:39.560857 typed-api-framework-0.0.1a4/typedAPI/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/endpoint/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/endpoint/guards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/endpoint/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/endpoint/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:15:39.560857 typed-api-framework-0.0.1a4/typedAPI/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/headers/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/headers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/headers/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/headers/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/log_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:15:39.560857 typed-api-framework-0.0.1a4/typedAPI/resource_path/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/resource_path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/resource_path/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/resource_path/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/resource_path/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:15:39.560857 typed-api-framework-0.0.1a4/typedAPI/response/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/response/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/response/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/response/factory_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/response/guards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/response/guards_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/response/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/response/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/response/service_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-30 06:15:28.000000 typed-api-framework-0.0.1a4/typedAPI/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:15:39.564857 typed-api-framework-0.0.1a4/typed_api_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-30 06:15:39.000000 typed-api-framework-0.0.1a4/typed_api_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-30 06:15:39.000000 typed-api-framework-0.0.1a4/typed_api_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:15:39.000000 typed-api-framework-0.0.1a4/typed_api_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 06:15:39.000000 typed-api-framework-0.0.1a4/typed_api_framework.egg-info/top_level.txt
```

### Comparing `typed-api-framework-0.0.0/LICENSE` & `typed-api-framework-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/PKG-INFO` & `typed-api-framework-0.0.1a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typed-api-framework
-Version: 0.0.0
+Version: 0.0.1a4
 Summary: A lightweigt package for concisely defining an api.
 Home-page: https://github.com/Digital-Defiance/typed-api
 Author: Rui Filipe de Sousa Campos @ Digital Defiance
 Author-email: mail@ruicampos.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `typed-api-framework-0.0.0/README.md` & `typed-api-framework-0.0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/setup.py` & `typed-api-framework-0.0.1a4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from setuptools import setup, find_packages
 
 import os
 
 VERSION = os.getenv('PACKAGE_VERSION', None)
 
+print(f"{VERSION=}")
+
 if VERSION is None:
   raise RuntimeError('`PACKAGE_VERSION` not defined.')
 
 setup(
     name='typed-api-framework',
     version=VERSION,
     description='A lightweigt package for concisely defining an api.',
```

### Comparing `typed-api-framework-0.0.0/typedAPI/body/service.py` & `typed-api-framework-0.0.1a4/typedAPI/body/service.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/endpoint/schema.py` & `typed-api-framework-0.0.1a4/typedAPI/endpoint/schema.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/endpoint/service.py` & `typed-api-framework-0.0.1a4/typedAPI/endpoint/service.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/headers/factory.py` & `typed-api-framework-0.0.1a4/typedAPI/headers/factory.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/headers/schema.py` & `typed-api-framework-0.0.1a4/typedAPI/headers/schema.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/headers/service.py` & `typed-api-framework-0.0.1a4/typedAPI/headers/service.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/log_config.py` & `typed-api-framework-0.0.1a4/typedAPI/log_config.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/resource_path/service.py` & `typed-api-framework-0.0.1a4/typedAPI/resource_path/service.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/response/data.py` & `typed-api-framework-0.0.1a4/typedAPI/response/data.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/response/factory.py` & `typed-api-framework-0.0.1a4/typedAPI/response/factory.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/response/factory_tests.py` & `typed-api-framework-0.0.1a4/typedAPI/response/factory_tests.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/response/guards.py` & `typed-api-framework-0.0.1a4/typedAPI/response/guards.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/response/guards_tests.py` & `typed-api-framework-0.0.1a4/typedAPI/response/guards_tests.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/response/processors.py` & `typed-api-framework-0.0.1a4/typedAPI/response/processors.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/response/schema.py` & `typed-api-framework-0.0.1a4/typedAPI/response/schema.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/response/service.py` & `typed-api-framework-0.0.1a4/typedAPI/response/service.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/response/service_tests.py` & `typed-api-framework-0.0.1a4/typedAPI/response/service_tests.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typedAPI/server.py` & `typed-api-framework-0.0.1a4/typedAPI/server.py`

 * *Files identical despite different names*

### Comparing `typed-api-framework-0.0.0/typed_api_framework.egg-info/PKG-INFO` & `typed-api-framework-0.0.1a4/typed_api_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typed-api-framework
-Version: 0.0.0
+Version: 0.0.1a4
 Summary: A lightweigt package for concisely defining an api.
 Home-page: https://github.com/Digital-Defiance/typed-api
 Author: Rui Filipe de Sousa Campos @ Digital Defiance
 Author-email: mail@ruicampos.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `typed-api-framework-0.0.0/typed_api_framework.egg-info/SOURCES.txt` & `typed-api-framework-0.0.1a4/typed_api_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

