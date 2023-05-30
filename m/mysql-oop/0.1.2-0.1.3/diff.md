# Comparing `tmp/mysql-oop-0.1.2.tar.gz` & `tmp/mysql-oop-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-oop-0.1.2.tar", last modified: Tue May 30 03:55:25 2023, max compression
+gzip compressed data, was "mysql-oop-0.1.3.tar", last modified: Tue May 30 04:49:05 2023, max compression
```

## Comparing `mysql-oop-0.1.2.tar` & `mysql-oop-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 03:55:25.688883 mysql-oop-0.1.2/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1084 2023-05-28 08:47:28.000000 mysql-oop-0.1.2/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-30 03:55:25.688883 mysql-oop-0.1.2/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-05-29 08:33:20.000000 mysql-oop-0.1.2/README.md
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      157 2023-05-29 11:46:25.000000 mysql-oop-0.1.2/pyproject.toml
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      608 2023-05-30 03:55:25.688883 mysql-oop-0.1.2/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 03:55:25.684882 mysql-oop-0.1.2/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 03:55:25.688883 mysql-oop-0.1.2/src/mysql_oop.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-30 03:55:25.000000 mysql-oop-0.1.2/src/mysql_oop.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      284 2023-05-30 03:55:25.000000 mysql-oop-0.1.2/src/mysql_oop.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-30 03:55:25.000000 mysql-oop-0.1.2/src/mysql_oop.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-30 03:55:25.000000 mysql-oop-0.1.2/src/mysql_oop.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 03:55:25.688883 mysql-oop-0.1.2/src/mysqloop/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1957 2023-05-30 03:42:27.000000 mysql-oop-0.1.2/src/mysqloop/Model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      153 2023-05-29 08:53:58.000000 mysql-oop-0.1.2/src/mysqloop/Users.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       98 2023-05-30 03:42:13.000000 mysql-oop-0.1.2/src/mysqloop/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    15079 2023-05-30 03:11:28.000000 mysql-oop-0.1.2/src/mysqloop/mysqloop.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 04:49:05.305676 mysql-oop-0.1.3/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1084 2023-05-28 08:47:28.000000 mysql-oop-0.1.3/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-30 04:49:05.305676 mysql-oop-0.1.3/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-05-29 08:33:20.000000 mysql-oop-0.1.3/README.md
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      157 2023-05-29 11:46:25.000000 mysql-oop-0.1.3/pyproject.toml
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      608 2023-05-30 04:49:05.305676 mysql-oop-0.1.3/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 04:49:05.301676 mysql-oop-0.1.3/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 04:49:05.305676 mysql-oop-0.1.3/src/mysql_oop.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-30 04:49:05.000000 mysql-oop-0.1.3/src/mysql_oop.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      284 2023-05-30 04:49:05.000000 mysql-oop-0.1.3/src/mysql_oop.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-30 04:49:05.000000 mysql-oop-0.1.3/src/mysql_oop.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-30 04:49:05.000000 mysql-oop-0.1.3/src/mysql_oop.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 04:49:05.305676 mysql-oop-0.1.3/src/mysqloop/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1957 2023-05-30 03:42:27.000000 mysql-oop-0.1.3/src/mysqloop/Model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      153 2023-05-29 08:53:58.000000 mysql-oop-0.1.3/src/mysqloop/Users.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       98 2023-05-30 03:42:13.000000 mysql-oop-0.1.3/src/mysqloop/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    15319 2023-05-30 04:46:41.000000 mysql-oop-0.1.3/src/mysqloop/mysqloop.py
```

### Comparing `mysql-oop-0.1.2/LICENSE` & `mysql-oop-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-oop-0.1.2/PKG-INFO` & `mysql-oop-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-oop
-Version: 0.1.2
+Version: 0.1.3
 Summary: python mysql OOP class
 Home-page: https://github.com/hahadu/mysql-py-oop
 Author: hahadu
 Author-email: mhyzhu@163.com
 Project-URL: Bug Tracker, https://github.com/hahadu/mysql-py-oop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mysql-oop-0.1.2/README.md` & `mysql-oop-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mysql-oop-0.1.2/setup.cfg` & `mysql-oop-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mysql-oop
-version = 0.1.2
+version = 0.1.3
 author = hahadu
 author_email = mhyzhu@163.com
 description = python mysql OOP class
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hahadu/mysql-py-oop
 project_urls =
```

### Comparing `mysql-oop-0.1.2/src/mysql_oop.egg-info/PKG-INFO` & `mysql-oop-0.1.3/src/mysql_oop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-oop
-Version: 0.1.2
+Version: 0.1.3
 Summary: python mysql OOP class
 Home-page: https://github.com/hahadu/mysql-py-oop
 Author: hahadu
 Author-email: mhyzhu@163.com
 Project-URL: Bug Tracker, https://github.com/hahadu/mysql-py-oop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mysql-oop-0.1.2/src/mysqloop/Model.py` & `mysql-oop-0.1.3/src/mysqloop/Model.py`

 * *Files identical despite different names*

### Comparing `mysql-oop-0.1.2/src/mysqloop/mysqloop.py` & `mysql-oop-0.1.3/src/mysqloop/mysqloop.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,30 +33,38 @@
     __operators = [
         "<=>", "=", "!=", "<>", ">", "<", ">=", "<=", "!<", "!>", "!",
         "AND", "BETWEEN", "NOT BETWEEN", "IN", "NOT IN", "LIKE", "EXISTS",
         "GLOB", "NOT", "OR", "XOR", "IS NULL", "IS", "IS NOT", "||", "UNIQUE",
         "REGEXP", "RLIKE",
     ]
     __config = {
-        "db_host": os.getenv("DB_HOST"),
-        "db_port": os.getenv("DB_PORT"),
-        "db_user": os.getenv("DB_USER"),
-        "db_password": os.getenv("DB_PASSWORD"),
-        "db_name": os.getenv("DB_NAME")
+        "db_host": None,
+        "db_port": None,
+        "db_user": None,
+        "db_password": None,
+        "db_name": None
     }
 
     db = None
 
     def __init__(self, config=None):
         """
         :param config:
         """
 
         if config is not None:
             self.__config.update(config)
+        else:
+            self.__config.update({
+                "db_host": os.getenv("DB_HOST"),
+                "db_port": os.getenv("DB_PORT"),
+                "db_user": os.getenv("DB_USER"),
+                "db_password": os.getenv("DB_PASSWORD"),
+                "db_name": os.getenv("DB_NAME")
+            })
         try:
             self.db = connector.connect(host=self.__config['db_host'], port=self.__config['db_port'],
                                         user=self.__config['db_user'], password=self.__config['db_password'],
                                         database=self.__config['db_name'])
         except Exception as e:
             raise Exception(e)
     def connect(self, db_host="127.0.0.1", db_port=3306, db_user="root", db_password=None, db_name="root"):
```

