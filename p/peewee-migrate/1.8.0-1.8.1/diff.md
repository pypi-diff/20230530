# Comparing `tmp/peewee_migrate-1.8.0.tar.gz` & `tmp/peewee_migrate-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_migrate-1.8.0.tar", max compression
+gzip compressed data, was "peewee_migrate-1.8.1.tar", max compression
```

## Comparing `peewee_migrate-1.8.0.tar` & `peewee_migrate-1.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     4456 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/README.rst
--rw-r--r--   0        0        0      146 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/__init__.py
--rw-r--r--   0        0        0       78 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/__main__.py
--rw-r--r--   0        0        0    12050 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/auto.py
--rw-r--r--   0        0        0     6597 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/cli.py
--rw-r--r--   0        0        0      146 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/logs.py
--rw-r--r--   0        0        0    19498 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/migrator.py
--rw-r--r--   0        0        0      461 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/models.py
--rw-r--r--   0        0        0        0 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/py.typed
--rw-r--r--   0        0        0    12235 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/router.py
--rw-r--r--   0        0        0     1802 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/template.py
--rw-r--r--   0        0        0      249 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/types.py
--rw-r--r--   0        0        0      325 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/utils.py
--rw-r--r--   0        0        0     1589 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4456 2023-05-30 14:09:43.371776 peewee_migrate-1.8.1/README.rst
+-rw-r--r--   0        0        0      146 2023-05-30 14:09:43.371776 peewee_migrate-1.8.1/peewee_migrate/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-30 14:09:43.371776 peewee_migrate-1.8.1/peewee_migrate/__main__.py
+-rw-r--r--   0        0        0    12050 2023-05-30 14:09:43.371776 peewee_migrate-1.8.1/peewee_migrate/auto.py
+-rw-r--r--   0        0        0     6597 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/cli.py
+-rw-r--r--   0        0        0      146 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/logs.py
+-rw-r--r--   0        0        0    19578 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/migrator.py
+-rw-r--r--   0        0        0      461 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/models.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/py.typed
+-rw-r--r--   0        0        0    12235 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/router.py
+-rw-r--r--   0        0        0     1802 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/template.py
+-rw-r--r--   0        0        0      249 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/types.py
+-rw-r--r--   0        0        0      325 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/peewee_migrate/utils.py
+-rw-r--r--   0        0        0     1589 2023-05-30 14:09:43.375776 peewee_migrate-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.8.1/PKG-INFO
```

### Comparing `peewee_migrate-1.8.0/README.rst` & `peewee_migrate-1.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.8.0/peewee_migrate/auto.py` & `peewee_migrate-1.8.1/peewee_migrate/auto.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.8.0/peewee_migrate/cli.py` & `peewee_migrate-1.8.1/peewee_migrate/cli.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.8.0/peewee_migrate/migrator.py` & `peewee_migrate-1.8.1/peewee_migrate/migrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Run migrations."""
 
 from __future__ import annotations
 
+from contextlib import suppress
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Union, cast, overload
 
 import peewee as pw
 from playhouse.migrate import (
     SQL,
     Context,
     MySQLDatabase,
@@ -186,15 +187,15 @@
 
         :param model: Model class or table name
         :param pw_db(true): Change fields in database
 
         >> migrator.change_fields(Model, name=pw.CharField(null=True))
         """
         model = self.__get_model__(model)
-        meta = model._meta  # type: ignore[]
+        meta: pw.Metadata = model._meta  # type: ignore[]
         for name, field in fields.items():
             old_field = meta.fields.get(name, field)
             old_column_name = old_field and old_field.column_name
 
             meta.add_field(name, field)
 
             if pw_db:
@@ -238,15 +239,16 @@
 
             if field.unique:
                 index = (field.column_name,), field.unique
                 meta.indexes.append(index)
                 self.__process__(self.__migrator__.add_index(meta.table_name, *index), db=pw_db)
             else:
                 index = field.column_name
-                meta.indexes.remove(((field.column_name,), old_field.unique))
+                with suppress(ValueError):
+                    meta.indexes.remove(((field.column_name,), True))
                 self.__process__(self.__migrator__.drop_index(meta.table_name, index), db=pw_db)
 
         return model
 
     change_columns = depricated_method(change_fields, "change_columns")
 
     def remove_fields(
```

### Comparing `peewee_migrate-1.8.0/peewee_migrate/router.py` & `peewee_migrate-1.8.1/peewee_migrate/router.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.8.0/peewee_migrate/template.py` & `peewee_migrate-1.8.1/peewee_migrate/template.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.8.0/pyproject.toml` & `peewee_migrate-1.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-migrate"
-version = "1.8.0"
+version = "1.8.1"
 homepage = "https://github.com/klen/peewee_migrate"
 repository = "https://github.com/klen/peewee_migrate"
 description = "Support for migrations in Peewee ORM"
 readme = "README.rst"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["peewee", "migrations", "orm"]
```

### Comparing `peewee_migrate-1.8.0/PKG-INFO` & `peewee_migrate-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-migrate
-Version: 1.8.0
+Version: 1.8.1
 Summary: Support for migrations in Peewee ORM
 Home-page: https://github.com/klen/peewee_migrate
 License: MIT
 Keywords: peewee,migrations,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

