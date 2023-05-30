# Comparing `tmp/dbhydra-1.0.1.tar.gz` & `tmp/dbhydra-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbhydra-1.0.1.tar", last modified: Tue May 30 18:22:21 2023, max compression
+gzip compressed data, was "dbhydra-1.0.2.tar", last modified: Tue May 30 18:30:18 2023, max compression
```

## Comparing `dbhydra-1.0.1.tar` & `dbhydra-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 18:22:21.397893 dbhydra-1.0.1/
--rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2117 2023-05-30 18:22:21.396895 dbhydra-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 18:22:21.347029 dbhydra-1.0.1/dbhydra/
--rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.0.1/dbhydra/__init__.py
--rw-rw-rw-   0        0        0     1682 2022-10-17 21:58:06.000000 dbhydra-1.0.1/dbhydra/dbhydra_builder.py
--rw-rw-rw-   0        0        0    66894 2023-05-30 18:22:00.000000 dbhydra-1.0.1/dbhydra/dbhydra_core.py
--rw-rw-rw-   0        0        0     2405 2022-10-17 21:58:06.000000 dbhydra-1.0.1/dbhydra/dbhydra_liquibase.py
--rw-rw-rw-   0        0        0      757 2022-10-17 21:58:06.000000 dbhydra-1.0.1/dbhydra/dbhydra_model.py
--rw-rw-rw-   0        0        0      337 2020-12-30 01:44:56.000000 dbhydra-1.0.1/dbhydra/dbhydra_mysql_example - kopie.py
--rw-rw-rw-   0        0        0     3815 2022-10-17 21:58:06.000000 dbhydra-1.0.1/dbhydra/dbhydra_mysql_example.py
--rw-rw-rw-   0        0        0      782 2022-10-17 21:58:06.000000 dbhydra-1.0.1/dbhydra/dbhydra_pandas_framework.py
--rw-rw-rw-   0        0        0     2472 2022-10-17 21:58:06.000000 dbhydra-1.0.1/dbhydra/migrator_example.py
--rw-rw-rw-   0        0        0     1836 2021-09-10 13:04:36.000000 dbhydra-1.0.1/dbhydra/mongo.py
--rw-rw-rw-   0        0        0      448 2021-12-29 18:11:09.000000 dbhydra-1.0.1/dbhydra/test.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:22:21.395898 dbhydra-1.0.1/dbhydra/tests/
--rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.0.1/dbhydra/tests/__init__.py
--rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.0.1/dbhydra/tests/test_cases.py
--rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.0.1/dbhydra/tests/test_mongo.py
--rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.0.1/dbhydra/tests/test_sql.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:22:21.371962 dbhydra-1.0.1/dbhydra.egg-info/
--rw-rw-rw-   0        0        0     2117 2023-05-30 18:22:20.000000 dbhydra-1.0.1/dbhydra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-05-30 18:22:21.000000 dbhydra-1.0.1/dbhydra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 18:22:20.000000 dbhydra-1.0.1/dbhydra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-30 18:22:20.000000 dbhydra-1.0.1/dbhydra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 18:22:20.000000 dbhydra-1.0.1/dbhydra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 18:22:21.397893 dbhydra-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-05-30 18:22:05.000000 dbhydra-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:30:18.860805 dbhydra-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2020-12-30 01:44:56.000000 dbhydra-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2117 2023-05-30 18:30:18.859805 dbhydra-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1636 2021-12-29 21:54:01.000000 dbhydra-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 18:30:18.826894 dbhydra-1.0.2/dbhydra/
+-rw-rw-rw-   0        0        0        0 2020-12-30 01:44:56.000000 dbhydra-1.0.2/dbhydra/__init__.py
+-rw-rw-rw-   0        0        0     1682 2022-10-17 21:58:06.000000 dbhydra-1.0.2/dbhydra/dbhydra_builder.py
+-rw-rw-rw-   0        0        0    67310 2023-05-30 18:29:17.000000 dbhydra-1.0.2/dbhydra/dbhydra_core.py
+-rw-rw-rw-   0        0        0     2405 2022-10-17 21:58:06.000000 dbhydra-1.0.2/dbhydra/dbhydra_liquibase.py
+-rw-rw-rw-   0        0        0      757 2022-10-17 21:58:06.000000 dbhydra-1.0.2/dbhydra/dbhydra_model.py
+-rw-rw-rw-   0        0        0      337 2020-12-30 01:44:56.000000 dbhydra-1.0.2/dbhydra/dbhydra_mysql_example - kopie.py
+-rw-rw-rw-   0        0        0     3815 2022-10-17 21:58:06.000000 dbhydra-1.0.2/dbhydra/dbhydra_mysql_example.py
+-rw-rw-rw-   0        0        0      782 2022-10-17 21:58:06.000000 dbhydra-1.0.2/dbhydra/dbhydra_pandas_framework.py
+-rw-rw-rw-   0        0        0     2472 2022-10-17 21:58:06.000000 dbhydra-1.0.2/dbhydra/migrator_example.py
+-rw-rw-rw-   0        0        0     1836 2021-09-10 13:04:36.000000 dbhydra-1.0.2/dbhydra/mongo.py
+-rw-rw-rw-   0        0        0      448 2021-12-29 18:11:09.000000 dbhydra-1.0.2/dbhydra/test.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:30:18.857811 dbhydra-1.0.2/dbhydra/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-12 23:52:29.000000 dbhydra-1.0.2/dbhydra/tests/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-03-12 23:52:29.000000 dbhydra-1.0.2/dbhydra/tests/test_cases.py
+-rw-rw-rw-   0        0        0     1979 2023-03-12 23:52:29.000000 dbhydra-1.0.2/dbhydra/tests/test_mongo.py
+-rw-rw-rw-   0        0        0     3126 2023-03-12 23:52:29.000000 dbhydra-1.0.2/dbhydra/tests/test_sql.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:30:18.851827 dbhydra-1.0.2/dbhydra.egg-info/
+-rw-rw-rw-   0        0        0     2117 2023-05-30 18:30:17.000000 dbhydra-1.0.2/dbhydra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-05-30 18:30:18.000000 dbhydra-1.0.2/dbhydra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 18:30:18.000000 dbhydra-1.0.2/dbhydra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-30 18:30:18.000000 dbhydra-1.0.2/dbhydra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 18:30:18.000000 dbhydra-1.0.2/dbhydra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 18:30:18.860805 dbhydra-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-05-30 18:29:50.000000 dbhydra-1.0.2/setup.py
```

### Comparing `dbhydra-1.0.1/LICENSE` & `dbhydra-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.1/PKG-INFO` & `dbhydra-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.0.1
+Version: 1.0.2
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.0.1/README.md` & `dbhydra-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.1/dbhydra/dbhydra_builder.py` & `dbhydra-1.0.2/dbhydra/dbhydra_builder.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.1/dbhydra/dbhydra_core.py` & `dbhydra-1.0.2/dbhydra/dbhydra_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,27 +30,27 @@
 POSTGRES_TO_MYSQL_DATA_MAPPING = {
     "int": "int",
     "integer": "int",
     "bigint": "bigint",
     "smallint": "smallint",
     "character varying": "varchar",
     "text": "longtext",
-    "boolean": "tinyint",
+    "boolean": "bit",
     "double precision": "double",
     "real": "float",
     "numeric": "decimal",
     "date": "date",
     "timestamp": "timestamp"
 }
 
 PYTHON_TO_MYSQL_DATA_MAPPING = {
     'int': "int",
     'float': "double",
     'str': "varchar(255)",
-    'bool': "tinyint",
+    'bool': "bit",
     'datetime': "datetime"
 }
 
 def read_file(file):
     """Reads txt file -> list"""
 
     with open(file, "r") as f:
@@ -457,18 +457,18 @@
 
 class Mysqldb(AbstractDB):
 
     python_database_type_mapping = PYTHON_TO_MYSQL_DATA_MAPPING = \
     {
     'int': "int",
     'float': "double",
-    'str': "varchar(255)",
-    'list': "varchar(255)",
-    'dict': "varchar(255)",
-    'bool': "tinyint",
+    'str': "nvarchar(255)",
+    'list': "nvarchar(255)",
+    'dict': "nvarchar(255)",
+    'bool': "bit",
     'datetime': "datetime"
     }
 
     def connect_locally(self):
         self.connection = MySQLdb.connect(host=self.DB_SERVER, user=self.DB_USERNAME, password=self.DB_PASSWORD,
                                           database=self.DB_DATABASE)
         self.cursor = self.connection.cursor()
@@ -802,22 +802,28 @@
 
         if adjust_df:
             df = self._adjust_df(df, debug_mode)
 
         if insert_id:
             assert len(df.columns) == len(self.columns)
             assert set(df.columns) == set(self.columns)
+            
+            inserted_columns=self.columns
+            
         else:
             assert len(df.columns) + 1 == len(self.columns) # +1 because of id column
-            sql_columns = set(self.columns)
-            sql_columns.remove('id')
-            assert set(df.columns) == sql_columns
-
-        df = df[self.columns]
-
+            
+            inserted_columns=list(dict.fromkeys(self.columns)) #DEDUPLICATION preserving order -> better than inserted_columns = set(self.columns) 
+            id_index=inserted_columns.index("id")
+            inserted_columns.pop(id_index)
+            print(inserted_columns,df.columns)
+            
+            assert set(df.columns) == set(inserted_columns) #elements are matchin
+            #df = df[inserted_columns]
+        df = df[inserted_columns]
 
         pd_nullable_dtypes = {pd.Int8Dtype(), pd.Int16Dtype(), pd.Int32Dtype(), pd.Int64Dtype(),
                               pd.UInt8Dtype(), pd.UInt16Dtype(), pd.UInt32Dtype(), pd.UInt64Dtype(),
                               pd.Float32Dtype(), pd.Float64Dtype()}
         pd_nullable_columns = df.dtypes.isin(pd_nullable_dtypes)
 
         # cast pd nullable columns to float - changing to 'NULL' then proceeds without an error.
@@ -825,19 +831,21 @@
         df = df.copy()
         df.loc[:, pd_nullable_columns] = df.loc[:, pd_nullable_columns].astype(float)
 
         # TODO: handling nan values -> change to NULL
         for column in list(df.columns):
             df.loc[pd.isna(df[column]), column] = "NULL"
 
+        # rows = df.values.tolist()
+        # for i, row in enumerate(rows):
+        #     for j, record in enumerate(row):
+        #         if type(record) == str:
+        #             rows[i][j] = "'" + record + "'"
+        #print(rows)
         rows = df.values.tolist()
-        for i, row in enumerate(rows):
-            for j, record in enumerate(row):
-                if type(record) == str:
-                    rows[i][j] = "'" + record + "'"
         self.insert(rows, batch=batch, try_mode=try_mode, debug_mode=False, insert_id=insert_id)
 
     #TODO: need to solve inserting in different column_order
     #check df column names, permute if needed
     def insert_from_column_value_dict(self, dict, insert_id=False):
         df = pd.DataFrame(dict, index=[0])
         self.insert_from_df(df, insert_id=insert_id)
@@ -850,15 +858,14 @@
 
     def delete(self, where=None):
 
         if where is None:
             query = "DELETE FROM " + self.name
         else:
             query = "DELETE FROM " + self.name + " WHERE " + where
-        print(query)
         self.db1.execute(query)
 
 
 class PostgresTable(AbstractTable):
     def __init__(self, db1, name, columns=None, types=None):
         super().__init__(db1, name, columns)
         self.types = types
```

### Comparing `dbhydra-1.0.1/dbhydra/dbhydra_liquibase.py` & `dbhydra-1.0.2/dbhydra/dbhydra_liquibase.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.1/dbhydra/dbhydra_model.py` & `dbhydra-1.0.2/dbhydra/dbhydra_model.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.1/dbhydra/dbhydra_mysql_example.py` & `dbhydra-1.0.2/dbhydra/dbhydra_mysql_example.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.1/dbhydra/dbhydra_pandas_framework.py` & `dbhydra-1.0.2/dbhydra/dbhydra_pandas_framework.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.1/dbhydra/migrator_example.py` & `dbhydra-1.0.2/dbhydra/migrator_example.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.1/dbhydra/mongo.py` & `dbhydra-1.0.2/dbhydra/mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.1/dbhydra/tests/test_mongo.py` & `dbhydra-1.0.2/dbhydra/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.1/dbhydra/tests/test_sql.py` & `dbhydra-1.0.2/dbhydra/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.1/dbhydra.egg-info/PKG-INFO` & `dbhydra-1.0.2/dbhydra.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 1.0.1
+Version: 1.0.2
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dbhydra-1.0.1/dbhydra.egg-info/SOURCES.txt` & `dbhydra-1.0.2/dbhydra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbhydra-1.0.1/setup.py` & `dbhydra-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='dbhydra',
-    version='1.0.1',
+    version='1.0.2',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Data science friendly ORM combining Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/dbhydra',
     packages=setuptools.find_packages(),
```

