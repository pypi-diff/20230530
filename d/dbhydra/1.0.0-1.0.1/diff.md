# Comparing `tmp/dbhydra-1.0.0.tar.gz` & `tmp/dbhydra-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbhydra-1.0.0.tar", last modified: Thu May 25 14:49:13 2023, max compression
+gzip compressed data, was "dbhydra-1.0.1.tar", last modified: Tue May 30 18:22:21 2023, max compression
```

## Comparing `dbhydra-1.0.0.tar` & `dbhydra-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 14:49:13.151783 dbhydra-1.0.0/
--rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2117 2023-05-25 14:49:13.149788 dbhydra-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 14:49:13.049056 dbhydra-1.0.0/dbhydra/
--rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.0.0/dbhydra/__init__.py
--rw-rw-rw-   0        0        0     1682 2022-10-17 21:58:06.000000 dbhydra-1.0.0/dbhydra/dbhydra_builder.py
--rw-rw-rw-   0        0        0    66388 2023-05-25 14:48:28.000000 dbhydra-1.0.0/dbhydra/dbhydra_core.py
--rw-rw-rw-   0        0        0     2405 2022-10-17 21:58:06.000000 dbhydra-1.0.0/dbhydra/dbhydra_liquibase.py
--rw-rw-rw-   0        0        0      757 2022-10-17 21:58:06.000000 dbhydra-1.0.0/dbhydra/dbhydra_model.py
--rw-rw-rw-   0        0        0      337 2020-12-30 01:44:56.000000 dbhydra-1.0.0/dbhydra/dbhydra_mysql_example - kopie.py
--rw-rw-rw-   0        0        0     3815 2022-10-17 21:58:06.000000 dbhydra-1.0.0/dbhydra/dbhydra_mysql_example.py
--rw-rw-rw-   0        0        0      782 2022-10-17 21:58:06.000000 dbhydra-1.0.0/dbhydra/dbhydra_pandas_framework.py
--rw-rw-rw-   0        0        0     2472 2022-10-17 21:58:06.000000 dbhydra-1.0.0/dbhydra/migrator_example.py
--rw-rw-rw-   0        0        0     1836 2021-09-10 13:04:36.000000 dbhydra-1.0.0/dbhydra/mongo.py
--rw-rw-rw-   0        0        0      448 2021-12-29 18:11:09.000000 dbhydra-1.0.0/dbhydra/test.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:49:13.147794 dbhydra-1.0.0/dbhydra/tests/
--rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.0.0/dbhydra/tests/__init__.py
--rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.0.0/dbhydra/tests/test_cases.py
--rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.0.0/dbhydra/tests/test_mongo.py
--rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.0.0/dbhydra/tests/test_sql.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:49:13.087952 dbhydra-1.0.0/dbhydra.egg-info/
--rw-rw-rw-   0        0        0     2117 2023-05-25 14:49:11.000000 dbhydra-1.0.0/dbhydra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-05-25 14:49:12.000000 dbhydra-1.0.0/dbhydra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 14:49:11.000000 dbhydra-1.0.0/dbhydra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-25 14:49:11.000000 dbhydra-1.0.0/dbhydra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 14:49:12.000000 dbhydra-1.0.0/dbhydra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 14:49:13.152780 dbhydra-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-05-25 14:49:03.000000 dbhydra-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:22:21.397893 dbhydra-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2117 2023-05-30 18:22:21.396895 dbhydra-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 18:22:21.347029 dbhydra-1.0.1/dbhydra/
+-rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.0.1/dbhydra/__init__.py
+-rw-rw-rw-   0        0        0     1682 2022-10-17 21:58:06.000000 dbhydra-1.0.1/dbhydra/dbhydra_builder.py
+-rw-rw-rw-   0        0        0    66894 2023-05-30 18:22:00.000000 dbhydra-1.0.1/dbhydra/dbhydra_core.py
+-rw-rw-rw-   0        0        0     2405 2022-10-17 21:58:06.000000 dbhydra-1.0.1/dbhydra/dbhydra_liquibase.py
+-rw-rw-rw-   0        0        0      757 2022-10-17 21:58:06.000000 dbhydra-1.0.1/dbhydra/dbhydra_model.py
+-rw-rw-rw-   0        0        0      337 2020-12-30 01:44:56.000000 dbhydra-1.0.1/dbhydra/dbhydra_mysql_example - kopie.py
+-rw-rw-rw-   0        0        0     3815 2022-10-17 21:58:06.000000 dbhydra-1.0.1/dbhydra/dbhydra_mysql_example.py
+-rw-rw-rw-   0        0        0      782 2022-10-17 21:58:06.000000 dbhydra-1.0.1/dbhydra/dbhydra_pandas_framework.py
+-rw-rw-rw-   0        0        0     2472 2022-10-17 21:58:06.000000 dbhydra-1.0.1/dbhydra/migrator_example.py
+-rw-rw-rw-   0        0        0     1836 2021-09-10 13:04:36.000000 dbhydra-1.0.1/dbhydra/mongo.py
+-rw-rw-rw-   0        0        0      448 2021-12-29 18:11:09.000000 dbhydra-1.0.1/dbhydra/test.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:22:21.395898 dbhydra-1.0.1/dbhydra/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.0.1/dbhydra/tests/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.0.1/dbhydra/tests/test_cases.py
+-rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.0.1/dbhydra/tests/test_mongo.py
+-rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.0.1/dbhydra/tests/test_sql.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:22:21.371962 dbhydra-1.0.1/dbhydra.egg-info/
+-rw-rw-rw-   0        0        0     2117 2023-05-30 18:22:20.000000 dbhydra-1.0.1/dbhydra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-05-30 18:22:21.000000 dbhydra-1.0.1/dbhydra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 18:22:20.000000 dbhydra-1.0.1/dbhydra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-30 18:22:20.000000 dbhydra-1.0.1/dbhydra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 18:22:20.000000 dbhydra-1.0.1/dbhydra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 18:22:21.397893 dbhydra-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-05-30 18:22:05.000000 dbhydra-1.0.1/setup.py
```

### Comparing `dbhydra-1.0.0/LICENSE` & `dbhydra-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.0/PKG-INFO` & `dbhydra-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.0.0
+Version: 1.0.1
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.0.0/README.md` & `dbhydra-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.0/dbhydra/dbhydra_builder.py` & `dbhydra-1.0.1/dbhydra/dbhydra_builder.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.0/dbhydra/dbhydra_core.py` & `dbhydra-1.0.1/dbhydra/dbhydra_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 """DB Hydra ORM"""
+import sys
 import pymongo
-import pyodbc
+
+#! Disabled on macOS --> problematic import
+if sys.platform != "darwin":
+    import pyodbc
+    
 import pandas as pd
 import numpy as np
 import pymysql as MySQLdb
 from sys import platform
 if platform != "linux" and platform != "linux2":
     # linux
     import psycopg2 # disable dependency for server (Temporary)
@@ -105,14 +110,16 @@
         function(instance, *args, **kw)
 
     return (new_function)
 
 
 # class DataMigrator:
 
+class DbHydraException(Exception):
+    """Raise for db_hydra specific exceptions such as 'pyodbc can't be used on macOS as it's not supported'."""
 
 
 class Migrator:
     def __init__(self, db=None):
         self.db = db
         self.migration_number = 1
         self.migration_list = []
@@ -376,28 +383,33 @@
 
     # TODO, execute, close
 
 
 # AWFUL NAME, SHOULD BE RENAMED WITH MAJOR RELEASE (This connects basic SQL i suppose)
 class db(AbstractDB):
     def connect_remotely(self):
+        if sys.platform == "darwin":
+            raise DbHydraException("pyodbc library (MSSQL) not supported on macOS.")
 
         self.connection = pyodbc.connect(
             r'DRIVER={' + self.DB_DRIVER + '};'
                                            r'SERVER=' + self.DB_SERVER + ';'
                                                                          r'DATABASE=' + self.DB_DATABASE + ';'
                                                                                                            r'UID=' + self.DB_USERNAME + ';'
                                                                                                                                         r'PWD=' + self.DB_PASSWORD + '',
             timeout=1
 
         )
         self.cursor = self.connection.cursor()
         print("DB connection established")
 
     def connect_locally(self):
+        if sys.platform == "darwin":
+            raise DbHydraException("pyodbc library (MSSQL) not supported on macOS.")
+        
         self.connection = pyodbc.connect(
             r'DRIVER={' + self.DB_DRIVER + '};'
                                            r'SERVER=' + self.DB_SERVER + ';'
                                                                          r'DATABASE=' + self.DB_DATABASE + ';'
                                                                                                            r'TRUSTED_CONNECTION=yes;',
             timeout=1
             # r'PWD=' + self.DB_PASSWORD + '')
```

### Comparing `dbhydra-1.0.0/dbhydra/dbhydra_liquibase.py` & `dbhydra-1.0.1/dbhydra/dbhydra_liquibase.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.0/dbhydra/dbhydra_model.py` & `dbhydra-1.0.1/dbhydra/dbhydra_model.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.0/dbhydra/dbhydra_mysql_example.py` & `dbhydra-1.0.1/dbhydra/dbhydra_mysql_example.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.0/dbhydra/dbhydra_pandas_framework.py` & `dbhydra-1.0.1/dbhydra/dbhydra_pandas_framework.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.0/dbhydra/migrator_example.py` & `dbhydra-1.0.1/dbhydra/migrator_example.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.0/dbhydra/mongo.py` & `dbhydra-1.0.1/dbhydra/mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.0/dbhydra/tests/test_mongo.py` & `dbhydra-1.0.1/dbhydra/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.0/dbhydra/tests/test_sql.py` & `dbhydra-1.0.1/dbhydra/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.0/dbhydra.egg-info/PKG-INFO` & `dbhydra-1.0.1/dbhydra.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.0.0
+Version: 1.0.1
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.0.0/dbhydra.egg-info/SOURCES.txt` & `dbhydra-1.0.1/dbhydra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.0/setup.py` & `dbhydra-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='dbhydra',
-    version='1.0.0',
+    version='1.0.1',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Data science friendly ORM combining Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/dbhydra',
     packages=setuptools.find_packages(),
```

