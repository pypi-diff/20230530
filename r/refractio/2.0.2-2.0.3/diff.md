# Comparing `tmp/refractio-2.0.2.tar.gz` & `tmp/refractio-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-2.0.2.tar", last modified: Fri May 26 11:31:36 2023, max compression
+gzip compressed data, was "refractio-2.0.3.tar", last modified: Tue May 30 09:32:44 2023, max compression
```

## Comparing `refractio-2.0.2.tar` & `refractio-2.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-26 11:31:36.375791 refractio-2.0.2/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7440 2023-05-26 11:31:36.375791 refractio-2.0.2/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6771 2023-05-26 11:30:32.000000 refractio-2.0.2/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-26 11:31:36.373791 refractio-2.0.2/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      319 2023-05-23 10:14:58.000000 refractio-2.0.2/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-05-23 10:14:58.000000 refractio-2.0.2/refractio/amazons3.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-05-23 10:14:58.000000 refractio-2.0.2/refractio/azure.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4707 2023-05-19 12:16:37.000000 refractio-2.0.2/refractio/hive.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3875 2023-05-19 12:16:37.000000 refractio-2.0.2/refractio/manager.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4407 2023-05-19 12:16:26.000000 refractio-2.0.2/refractio/mysql.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    13446 2023-05-19 12:16:26.000000 refractio-2.0.2/refractio/refractio.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-05-19 12:16:37.000000 refractio-2.0.2/refractio/sftp.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5335 2023-05-19 12:16:26.000000 refractio-2.0.2/refractio/snowflake.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-26 11:31:36.375791 refractio-2.0.2/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7440 2023-05-26 11:31:36.000000 refractio-2.0.2/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      367 2023-05-26 11:31:36.000000 refractio-2.0.2/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-26 11:31:36.000000 refractio-2.0.2/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      483 2023-05-26 11:31:36.000000 refractio-2.0.2/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-26 11:31:36.000000 refractio-2.0.2/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-26 11:31:36.376791 refractio-2.0.2/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1807 2023-05-26 11:28:00.000000 refractio-2.0.2/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-30 09:32:44.233870 refractio-2.0.3/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7440 2023-05-30 09:32:44.233870 refractio-2.0.3/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6771 2023-05-30 09:31:33.000000 refractio-2.0.3/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-30 09:32:44.232870 refractio-2.0.3/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      319 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/amazons3.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/azure.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4717 2023-05-30 09:31:33.000000 refractio-2.0.3/refractio/hive.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3875 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/manager.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4407 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/mysql.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    13446 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/refractio.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/sftp.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5335 2023-05-30 09:31:19.000000 refractio-2.0.3/refractio/snowflake.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-30 09:32:44.232870 refractio-2.0.3/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7440 2023-05-30 09:32:43.000000 refractio-2.0.3/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      367 2023-05-30 09:32:43.000000 refractio-2.0.3/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-30 09:32:43.000000 refractio-2.0.3/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      483 2023-05-30 09:32:43.000000 refractio-2.0.3/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-30 09:32:43.000000 refractio-2.0.3/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-30 09:32:44.233870 refractio-2.0.3/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1807 2023-05-30 09:31:33.000000 refractio-2.0.3/setup.py
```

### Comparing `refractio-2.0.2/PKG-INFO` & `refractio-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.2
+Version: 2.0.3
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.2/README.md` & `refractio-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `refractio-2.0.2/refractio/amazons3.py` & `refractio-2.0.3/refractio/amazons3.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.2/refractio/azure.py` & `refractio-2.0.3/refractio/azure.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.2/refractio/hive.py` & `refractio-2.0.3/refractio/hive.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,18 @@
             print(f"Connection details fetched: {self.__connection_details}")
             print(f"Ex: {ex}")
             raise Exception(f"Exception occurred in creating hive connection: "
                             f"{self.__connection_details.get('detailMessage')}")
 
     def get_connection(self, connection_name=None, user_id="1001"):
         try:
-            # Getting connection
-            if self.con_obj is None or not self.con_obj.open:   # todo: need to check, how to validate live connection.
+            # Getting connection.
+            # connection.close() is not working in hive and there seems to be no attribute to validate whether the
+            # connection is live in hive connection object.
+            if self.con_obj is None:
                 # Getting default connection name
                 if connection_name is None:
                     connection_name = default_connection_name("HIVE")
                     if not connection_name:
                         raise Exception("Could not get the default connection name,"
                                         "please create/pass an active hive connection name.")
                 self.__connection_details = get_conn_details_from_conn_name(
@@ -75,15 +77,15 @@
             return data_frame
         except Exception as ex:
             print(f"Exception occurred in reading data_frame from hive connection: {ex}")
 
     def execute_query(self, query, connection_name=None, user_id="1001"):
         try:
             # Getting connection object
-            if self.con_obj is None or not self.con_obj.open:   # todo: need to check, how to validate live connection.
+            if self.con_obj is None:
                 self.get_connection(connection_name, user_id=user_id)
 
             data_frame = pd.read_sql(query, self.con_obj)   # Fetch all records in pandas dataframe
 
             self.con_obj.close()    # Closing the connection
             return data_frame
         except Exception as ex:
```

### Comparing `refractio-2.0.2/refractio/manager.py` & `refractio-2.0.3/refractio/manager.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.2/refractio/mysql.py` & `refractio-2.0.3/refractio/mysql.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.2/refractio/refractio.py` & `refractio-2.0.3/refractio/refractio.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.2/refractio/sftp.py` & `refractio-2.0.3/refractio/sftp.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.2/refractio/snowflake.py` & `refractio-2.0.3/refractio/snowflake.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.2/refractio.egg-info/PKG-INFO` & `refractio-2.0.3/refractio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.2
+Version: 2.0.3
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.2/setup.py` & `refractio-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.2'
+VERSION = '2.0.3'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.0.2",
         "boto3==1.26.116",
         "azure==4.0.0",
```

