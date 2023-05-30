# Comparing `tmp/psqlpandas-1.0.0.tar.gz` & `tmp/psqlpandas-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psqlpandas-1.0.0.tar", max compression
+gzip compressed data, was "psqlpandas-1.1.0.tar", max compression
```

## Comparing `psqlpandas-1.0.0.tar` & `psqlpandas-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      900 2023-05-29 11:07:32.790702 psqlpandas-1.0.0/LICENSE
--rw-r--r--   0        0        0      199 2023-05-29 11:07:32.790702 psqlpandas-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-29 11:07:32.814702 psqlpandas-1.0.0/psqlpandas/__init__.py
--rw-r--r--   0        0        0       22 2023-05-29 11:07:32.791702 psqlpandas-1.0.0/psqlpandas/__version__.py
--rw-r--r--   0        0        0     7674 2023-05-29 11:07:32.791702 psqlpandas-1.0.0/psqlpandas/postgresql.py
--rw-r--r--   0        0        0       88 2023-05-29 11:07:32.791702 psqlpandas-1.0.0/psqlpandas/scripts/script.py
--rw-r--r--   0        0        0     1909 2023-05-29 11:07:32.791702 psqlpandas-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 psqlpandas-1.0.0/setup.py
--rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 psqlpandas-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-05-30 09:31:06.262635 psqlpandas-1.1.0/LICENSE
+-rw-r--r--   0        0        0      199 2023-05-30 09:31:06.262635 psqlpandas-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 09:31:06.285635 psqlpandas-1.1.0/psqlpandas/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-30 09:31:06.263635 psqlpandas-1.1.0/psqlpandas/__version__.py
+-rw-r--r--   0        0        0     7944 2023-05-30 09:31:06.263635 psqlpandas-1.1.0/psqlpandas/postgresql.py
+-rw-r--r--   0        0        0       88 2023-05-30 09:31:06.263635 psqlpandas-1.1.0/psqlpandas/scripts/script.py
+-rw-r--r--   0        0        0     1909 2023-05-30 09:31:06.263635 psqlpandas-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 psqlpandas-1.1.0/setup.py
+-rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 psqlpandas-1.1.0/PKG-INFO
```

### Comparing `psqlpandas-1.0.0/LICENSE` & `psqlpandas-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psqlpandas-1.0.0/psqlpandas/postgresql.py` & `psqlpandas-1.1.0/psqlpandas/postgresql.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,32 +54,39 @@
             cur.close()
             raise
         else:
             cur.close()
             return data
 
     def read_df(
-        self, query: str, parse_dates: List[str] | str | None = None
+        self,
+        query: str,
+        parse_dates: List[str] | str | None = None,
+        uppercase_colnames: bool = False,
     ) -> pd.DataFrame:
         """
         Reads values from database directly into pandas dataframe
 
         NOTE: generally slower than self.read. But can be usefult for automatic casting of types (including dates).
 
         Args:
             query (str): select query to be executed
             parse_dates (List[str] | str | None, optional): columns to be parsed at dates. Defaults to None.
+            uppercase_colnames (bool): whether to return uppercase colnames. Defaults to False.
 
         Returns:
             pd.DataFrame: dataframe of data retrieved
         """
         try:
-            return pd.read_sql_query(
+            data = pd.read_sql_query(
                 text(query), con=self._sqlalchemy_conn, parse_dates=parse_dates
             )
+            if uppercase_colnames:
+                data.columns = data.columns.str.upper()
+            return data
         except Exception as e:
             logging.error(f"Error while reading query: {query}")
             logging.error(e)
             raise
 
     def execute_sql_query(self, query, row=None):
         cur = self._conn.cursor()
```

### Comparing `psqlpandas-1.0.0/pyproject.toml` & `psqlpandas-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psqlpandas"
-version = "1.0.0"
+version = "1.1.0"
 description = "Utilities to communicate with postgresql database through pandas dataframes."
 authors = ["Mattia Tantardini <mattia.tantardini@gmail.com>"]
 readme = "README.md"
 keywords = ["postgresql", "pandas"]
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Intended Audience :: Developers",
```

### Comparing `psqlpandas-1.0.0/setup.py` & `psqlpandas-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['numpy>=1.24.2,<2.0.0',
  'pandas>=2.0.1,<3.0.0',
  'psycopg2>=2.9.5,<3.0.0',
  'sqlalchemy>=2.0.3,<3.0.0']
 
 setup_kwargs = {
     'name': 'psqlpandas',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': 'Utilities to communicate with postgresql database through pandas dataframes.',
     'long_description': '# psqlpandas\nUtilities to communicate with postgresql database through pandas dataframes.\n\n## Installation\n```\npip install psqlpandas\n```\n\n## Usage\nDescribe how to launch and use psqlpandas project.\n',
     'author': 'Mattia Tantardini',
     'author_email': 'mattia.tantardini@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `psqlpandas-1.0.0/PKG-INFO` & `psqlpandas-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psqlpandas
-Version: 1.0.0
+Version: 1.1.0
 Summary: Utilities to communicate with postgresql database through pandas dataframes.
 Keywords: postgresql,pandas
 Author: Mattia Tantardini
 Author-email: mattia.tantardini@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

