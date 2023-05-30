# Comparing `tmp/mysql-oop-0.1.3.tar.gz` & `tmp/mysql-oop-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-oop-0.1.3.tar", last modified: Tue May 30 04:49:05 2023, max compression
+gzip compressed data, was "mysql-oop-0.1.5.tar", last modified: Tue May 30 10:41:33 2023, max compression
```

## Comparing `mysql-oop-0.1.3.tar` & `mysql-oop-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 04:49:05.305676 mysql-oop-0.1.3/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1084 2023-05-28 08:47:28.000000 mysql-oop-0.1.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-30 04:49:05.305676 mysql-oop-0.1.3/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-05-29 08:33:20.000000 mysql-oop-0.1.3/README.md
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      157 2023-05-29 11:46:25.000000 mysql-oop-0.1.3/pyproject.toml
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      608 2023-05-30 04:49:05.305676 mysql-oop-0.1.3/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 04:49:05.301676 mysql-oop-0.1.3/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 04:49:05.305676 mysql-oop-0.1.3/src/mysql_oop.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-30 04:49:05.000000 mysql-oop-0.1.3/src/mysql_oop.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      284 2023-05-30 04:49:05.000000 mysql-oop-0.1.3/src/mysql_oop.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-30 04:49:05.000000 mysql-oop-0.1.3/src/mysql_oop.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-30 04:49:05.000000 mysql-oop-0.1.3/src/mysql_oop.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 04:49:05.305676 mysql-oop-0.1.3/src/mysqloop/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1957 2023-05-30 03:42:27.000000 mysql-oop-0.1.3/src/mysqloop/Model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      153 2023-05-29 08:53:58.000000 mysql-oop-0.1.3/src/mysqloop/Users.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       98 2023-05-30 03:42:13.000000 mysql-oop-0.1.3/src/mysqloop/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    15319 2023-05-30 04:46:41.000000 mysql-oop-0.1.3/src/mysqloop/mysqloop.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 10:41:33.698450 mysql-oop-0.1.5/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1084 2023-05-28 08:47:28.000000 mysql-oop-0.1.5/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-30 10:41:33.698450 mysql-oop-0.1.5/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-05-29 08:33:20.000000 mysql-oop-0.1.5/README.md
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      157 2023-05-29 11:46:25.000000 mysql-oop-0.1.5/pyproject.toml
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      608 2023-05-30 10:41:33.698450 mysql-oop-0.1.5/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 10:41:33.694450 mysql-oop-0.1.5/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 10:41:33.698450 mysql-oop-0.1.5/src/mysql_oop.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-30 10:41:33.000000 mysql-oop-0.1.5/src/mysql_oop.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-05-30 10:41:33.000000 mysql-oop-0.1.5/src/mysql_oop.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-30 10:41:33.000000 mysql-oop-0.1.5/src/mysql_oop.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-30 10:41:33.000000 mysql-oop-0.1.5/src/mysql_oop.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 10:41:33.698450 mysql-oop-0.1.5/src/mysqloop/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      331 2023-05-30 10:23:10.000000 mysql-oop-0.1.5/src/mysqloop/BuildAttrs.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2522 2023-05-30 10:25:57.000000 mysql-oop-0.1.5/src/mysqloop/Model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      153 2023-05-29 08:53:58.000000 mysql-oop-0.1.5/src/mysqloop/Users.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       98 2023-05-30 03:42:13.000000 mysql-oop-0.1.5/src/mysqloop/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    15335 2023-05-30 07:46:13.000000 mysql-oop-0.1.5/src/mysqloop/mysqloop.py
```

### Comparing `mysql-oop-0.1.3/LICENSE` & `mysql-oop-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-oop-0.1.3/PKG-INFO` & `mysql-oop-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-oop
-Version: 0.1.3
+Version: 0.1.5
 Summary: python mysql OOP class
 Home-page: https://github.com/hahadu/mysql-py-oop
 Author: hahadu
 Author-email: mhyzhu@163.com
 Project-URL: Bug Tracker, https://github.com/hahadu/mysql-py-oop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mysql-oop-0.1.3/README.md` & `mysql-oop-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mysql-oop-0.1.3/setup.cfg` & `mysql-oop-0.1.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mysql-oop
-version = 0.1.3
+version = 0.1.5
 author = hahadu
 author_email = mhyzhu@163.com
 description = python mysql OOP class
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hahadu/mysql-py-oop
 project_urls =
```

### Comparing `mysql-oop-0.1.3/src/mysql_oop.egg-info/PKG-INFO` & `mysql-oop-0.1.5/src/mysql_oop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-oop
-Version: 0.1.3
+Version: 0.1.5
 Summary: python mysql OOP class
 Home-page: https://github.com/hahadu/mysql-py-oop
 Author: hahadu
 Author-email: mhyzhu@163.com
 Project-URL: Bug Tracker, https://github.com/hahadu/mysql-py-oop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mysql-oop-0.1.3/src/mysqloop/Model.py` & `mysql-oop-0.1.5/src/mysqloop/Model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-from .mysqloop import mysqloop
-
 from re import sub as re_sub
 
+from .mysqloop import mysqloop
+from .BuildAttrs import BuildAttrs
 
 class Model(mysqloop):
-    _table_name = ''
 
     def _re_underline_table_name(self, Upstr):
         """
         将大写驼峰转为下划线的表名
         """
         return re_sub('(?<=[a-z])[A-Z]|(?<!^)[A-Z](?=[a-z])', '_\g<0>', Upstr).lower()
 
     def __init__(self, config=None):
         super().__init__(config)
         self.get_table_name()
-        self._set_cursor()
 
     def get_table_name(self):
-        self._table_name = self._table_name if self._table_name is None else self._re_underline_table_name(
-            self.__class__.__name__.split('.')[-1])
-        return self._table_name
+        self.set_table_name(self._re_underline_table_name(
+            self.__class__.__name__.split('.')[-1]))
+        return super().get_table_name()
 
     def set_table_name(self, table_name):
-        self._table_name = table_name
+        self.table(table_name)
 
     def where(self, column, op=None, value=None, _boolean=" AND"):
         if isinstance(column, dict):
             for cl in column:
                 val = column[cl]
                 super().where(cl, '=', val)
         elif isinstance(column, list):
@@ -51,7 +49,30 @@
 
     def updateOrCreate(self, attributes, values: dict):
 
         if self.where(attributes).exists():
             return self.where(attributes).update(values)
         else:
             return self.create(attributes.update(values))
+
+    def save(self):
+
+        attrs = {}
+        for attr_column in vars(self).keys():
+            if attr_column[:1] != "_":
+                attrs.update({attr_column: self.__dict__[attr_column]})
+        return self.create(attrs)
+
+    def get(self, columns="*"):
+        attrList = []
+        datas = super().select(columns=columns)
+        for data in datas:
+            attrs = BuildAttrs()
+
+            for item in data:
+                # print(data[item])
+                # print(item)
+                setattr(attrs, item, data[item])
+            print(attrs.toJson())
+            #print(attrs.id)
+
+        print(datas)
```

### Comparing `mysql-oop-0.1.3/src/mysqloop/mysqloop.py` & `mysql-oop-0.1.5/src/mysqloop/mysqloop.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         "db_host": None,
         "db_port": None,
         "db_user": None,
         "db_password": None,
         "db_name": None
     }
 
-    db = None
+    _db = None
 
     def __init__(self, config=None):
         """
         :param config:
         """
 
         if config is not None:
@@ -58,21 +58,21 @@
                 "db_host": os.getenv("DB_HOST"),
                 "db_port": os.getenv("DB_PORT"),
                 "db_user": os.getenv("DB_USER"),
                 "db_password": os.getenv("DB_PASSWORD"),
                 "db_name": os.getenv("DB_NAME")
             })
         try:
-            self.db = connector.connect(host=self.__config['db_host'], port=self.__config['db_port'],
-                                        user=self.__config['db_user'], password=self.__config['db_password'],
-                                        database=self.__config['db_name'])
+            self._db = connector.connect(host=self.__config['db_host'], port=self.__config['db_port'],
+                                         user=self.__config['db_user'], password=self.__config['db_password'],
+                                         database=self.__config['db_name'])
         except Exception as e:
             raise Exception(e)
     def connect(self, db_host="127.0.0.1", db_port=3306, db_user="root", db_password=None, db_name="root"):
-        self.db = connector.connect(
+        self._db = connector.connect(
             host=db_host,
             port=db_port,
             user=db_user,
             passwd=db_password,
             database=db_name
         )
         return self
@@ -84,15 +84,15 @@
         :return:
         """
         self._table_name = table_name
         self._set_cursor()
         return self
 
     def _set_cursor(self):
-        self._cursor = self.db.cursor()
+        self._cursor = self._db.cursor()
 
     def get_table_name(self):
         return self._table_name
 
     def __is_tablename(self):
         if len(self._table_name) == 0:
             return "No query form is specified 亲，叫个表吧，求你了！"
@@ -257,37 +257,37 @@
         :return:
         """
         # print(type(type(columns)))
         if not isinstance(columns, (list, dict)):
             raise Exception("columns type must be (list or dict )")
         if isinstance(columns, dict):
             self.__instert_o(columns)
-            self.db.commit()
+            self._db.commit()
             last_id = self._cursor.lastrowid
             return self.where("id", str(last_id)).find()
         else:
             for item in columns:
                 self.__instert_o(item)
-            self.db.commit()
-            if self.db.total_changes > 0:
+            self._db.commit()
+            if self._db.total_changes > 0:
                 return True
             else:
                 return False
 
     def create(self, data: dict):
         """
         创建单条数据
         :param data:
         :return:
         """
         if not isinstance(data, dict):
             raise Exception("columns type must be dict")
         else:
             self.__instert_o(data)
-            self.db.commit()
+            self._db.commit()
             last_id = self._cursor.lastrowid
             return self.where("id", str(last_id)).find()
 
     def __instert_o(self, columns):
         """
         set insert sql
         :param columns:
@@ -346,26 +346,26 @@
         update += self.SPACE_CHARACTER
         update += "SET"
         update += self.SPACE_CHARACTER
         update += update_string
         update += self.SPACE_CHARACTER
         update += self.__base_where_clause_string
         self._cursor.execute(update)
-        self.db.commit()
+        self._db.commit()
         return self._cursor.rowcount
 
     def delete(self):
         delete_data = "DELETE FROM"
         delete_data += self.SPACE_CHARACTER
         delete_data += self._table_name
         delete_data += self.SPACE_CHARACTER
         delete_data += self.__base_where_clause_string
         delete_data += self.SEMICOLON_CHARACTER
         self._cursor.execute(delete_data)
-        self.db.commit()
+        self._db.commit()
 
         return self._cursor.rowcount
 
     def create_table(self, create_columns: dict, primary_key=None):
         """
         创建数据表
         :param create_columns:
@@ -393,25 +393,25 @@
         if primary_key is not None:
             created += ", PRIMARY KEY ( "
             created += primary_key
             created += " )"
         created += " )ENGINE=InnoDB DEFAULT CHARSET=utf8; "
         try:
             self._cursor.execute(created)
-            self.db.commit()
+            self._db.commit()
             return self.desc_table()
         except ValueError:
             raise Exception("create table fail!")
 
     def delete_table(self):
         delete_table = "DROP TABLE"
         delete_table += self.SPACE_CHARACTER
         delete_table += self._table_name
         self._cursor.execute(delete_table)
-        self.db.commit()
+        self._db.commit()
         if not self.is_table():
             return True
         else:
             return False
 
     def desc_table(self):
         if not self.is_table():
@@ -440,14 +440,14 @@
         count = len(self.show_table())
         if count > 0:
             return True
         else:
             return False
 
     def close(self):
-        self.db.close()
+        self._db.close()
 
     def __del__(self):
-        if self.db is not None:
+        if self._db is not None:
             self.close()
         else:
             raise Exception('mysql failed to connect')
```

