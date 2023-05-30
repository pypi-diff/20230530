# Comparing `tmp/influxdb_wrapper-0.0.3.tar.gz` & `tmp/influxdb_wrapper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb_wrapper-0.0.3.tar", last modified: Mon Mar 13 08:03:00 2023, max compression
+gzip compressed data, was "influxdb_wrapper-0.0.4.tar", last modified: Tue May 30 06:25:11 2023, max compression
```

## Comparing `influxdb_wrapper-0.0.3.tar` & `influxdb_wrapper-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:03:00.859569 influxdb_wrapper-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-13 08:03:00.859569 influxdb_wrapper-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-13 08:02:52.000000 influxdb_wrapper-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:03:00.859569 influxdb_wrapper-0.0.3/influxdb_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-13 08:02:52.000000 influxdb_wrapper-0.0.3/influxdb_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-03-13 08:02:52.000000 influxdb_wrapper-0.0.3/influxdb_wrapper/db_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-03-13 08:02:52.000000 influxdb_wrapper-0.0.3/influxdb_wrapper/influxdb_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-13 08:02:52.000000 influxdb_wrapper-0.0.3/influxdb_wrapper/mockdb_conn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:03:00.859569 influxdb_wrapper-0.0.3/influxdb_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-13 08:03:00.000000 influxdb_wrapper-0.0.3/influxdb_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-13 08:03:00.000000 influxdb_wrapper-0.0.3/influxdb_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 08:03:00.000000 influxdb_wrapper-0.0.3/influxdb_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-13 08:03:00.000000 influxdb_wrapper-0.0.3/influxdb_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-13 08:03:00.000000 influxdb_wrapper-0.0.3/influxdb_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 08:03:00.859569 influxdb_wrapper-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-03-13 08:02:52.000000 influxdb_wrapper-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:03:00.859569 influxdb_wrapper-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 08:02:52.000000 influxdb_wrapper-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-13 08:02:52.000000 influxdb_wrapper-0.0.3/tests/test_000.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:11.583121 influxdb_wrapper-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-30 06:25:11.583121 influxdb_wrapper-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:11.579121 influxdb_wrapper-0.0.4/influxdb_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/influxdb_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/influxdb_wrapper/db_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/influxdb_wrapper/influxdb_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/influxdb_wrapper/mockdb_conn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:11.583121 influxdb_wrapper-0.0.4/influxdb_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-30 06:25:11.000000 influxdb_wrapper-0.0.4/influxdb_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-30 06:25:11.000000 influxdb_wrapper-0.0.4/influxdb_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:25:11.000000 influxdb_wrapper-0.0.4/influxdb_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 06:25:11.000000 influxdb_wrapper-0.0.4/influxdb_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 06:25:11.000000 influxdb_wrapper-0.0.4/influxdb_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:25:11.583121 influxdb_wrapper-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:25:11.583121 influxdb_wrapper-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-30 06:24:55.000000 influxdb_wrapper-0.0.4/tests/test_000.py
```

### Comparing `influxdb_wrapper-0.0.3/PKG-INFO` & `influxdb_wrapper-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb_wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: DB management wrapper over influxDB
 Home-page: https://github.com/Phornee/influxdb_wrapper
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `influxdb_wrapper-0.0.3/influxdb_wrapper/db_conn.py` & `influxdb_wrapper-0.0.4/influxdb_wrapper/db_conn.py`

 * *Files identical despite different names*

### Comparing `influxdb_wrapper-0.0.3/influxdb_wrapper/influxdb_conn.py` & `influxdb_wrapper-0.0.4/influxdb_wrapper/influxdb_conn.py`

 * *Files identical despite different names*

### Comparing `influxdb_wrapper-0.0.3/influxdb_wrapper/mockdb_conn.py` & `influxdb_wrapper-0.0.4/influxdb_wrapper/mockdb_conn.py`

 * *Files identical despite different names*

### Comparing `influxdb_wrapper-0.0.3/influxdb_wrapper.egg-info/PKG-INFO` & `influxdb_wrapper-0.0.4/influxdb_wrapper.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb-wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: DB management wrapper over influxDB
 Home-page: https://github.com/Phornee/influxdb_wrapper
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `influxdb_wrapper-0.0.3/setup.py` & `influxdb_wrapper-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="influxdb_wrapper",
-    version="0.0.3",
+    version="0.0.4",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="DB management wrapper over influxDB",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/influxdb_wrapper",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'dnspython>=2.1.0',
+        'dnspython>=1.16.0',
         'influxdb>=5.3.1',
     ],
     python_requires='>=3.6',
 )
```

### Comparing `influxdb_wrapper-0.0.3/tests/test_000.py` & `influxdb_wrapper-0.0.4/tests/test_000.py`

 * *Files identical despite different names*

