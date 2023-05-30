# Comparing `tmp/peewee_migrate-1.7.9.tar.gz` & `tmp/peewee_migrate-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_migrate-1.7.9.tar", max compression
+gzip compressed data, was "peewee_migrate-1.8.0.tar", max compression
```

## Comparing `peewee_migrate-1.7.9.tar` & `peewee_migrate-1.8.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     4456 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/README.rst
--rw-r--r--   0        0        0      146 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/__init__.py
--rw-r--r--   0        0        0       78 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/__main__.py
--rw-r--r--   0        0        0    11862 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/auto.py
--rw-r--r--   0        0        0     6597 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/cli.py
--rw-r--r--   0        0        0      146 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/logs.py
--rw-r--r--   0        0        0    17190 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/migrator.py
--rw-r--r--   0        0        0      461 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/models.py
--rw-r--r--   0        0        0        0 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/py.typed
--rw-r--r--   0        0        0    12235 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/router.py
--rw-r--r--   0        0        0     1802 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/template.py
--rw-r--r--   0        0        0      249 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/types.py
--rw-r--r--   0        0        0     1589 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/pyproject.toml
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.7.9/PKG-INFO
+-rw-r--r--   0        0        0     4456 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/README.rst
+-rw-r--r--   0        0        0      146 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/__main__.py
+-rw-r--r--   0        0        0    12050 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/auto.py
+-rw-r--r--   0        0        0     6597 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/cli.py
+-rw-r--r--   0        0        0      146 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/logs.py
+-rw-r--r--   0        0        0    19498 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/migrator.py
+-rw-r--r--   0        0        0      461 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/models.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/py.typed
+-rw-r--r--   0        0        0    12235 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/router.py
+-rw-r--r--   0        0        0     1802 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/template.py
+-rw-r--r--   0        0        0      249 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/types.py
+-rw-r--r--   0        0        0      325 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/peewee_migrate/utils.py
+-rw-r--r--   0        0        0     1589 2023-05-30 13:53:43.405809 peewee_migrate-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.8.0/PKG-INFO
```

### Comparing `peewee_migrate-1.7.9/README.rst` & `peewee_migrate-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.9/peewee_migrate/auto.py` & `peewee_migrate-1.8.0/peewee_migrate/auto.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,17 +56,17 @@
 
     return params
 
 
 FIELD_TO_PARAMS: Dict[Type[pw.Field], Callable[[Any], TParams]] = {
     pw.CharField: lambda f: {"max_length": f.max_length},
     pw.DecimalField: lambda f: {
-        "max_digits": f.max_digits,
-        "decimal_places": f.decimal_places,
         "auto_round": f.auto_round,
+        "decimal_places": f.decimal_places,
+        "max_digits": f.max_digits,
         "rounding": f.rounding,
     },
     pw.ForeignKeyField: fk_to_params,
     pw.DateTimeField: dtf_to_params,
 }
 
 
@@ -83,14 +83,15 @@
             field.null,
             primary_key=field.primary_key,
             column_name=field.column_name,
             index=field.index,
             unique=field.unique,
             **kwargs,
         )
+        self.field = field
 
         if self.field_class in FIELD_TO_PARAMS:
             if self.extra_parameters is None:  # type: ignore[has-type]
                 self.extra_parameters = {}
 
             self.extra_parameters.update(FIELD_TO_PARAMS[self.field_class](field))
 
@@ -120,14 +121,17 @@
         params.pop("backref", None)
         if change:
             params["unique"] = bool(params.pop("unique", False))
             params["index"] = bool(params.pop("index", False)) or params["unique"]
             params.pop("on_delete", None)
             params.pop("on_update", None)
 
+        elif self.field.default is not None and not callable(self.field.default):
+            params["default"] = repr(self.field.db_value(self.field.default))
+
         return params
 
 
 def diff_one(model1: TModelType, model2: TModelType, **kwargs) -> List[str]:  # noqa:
     """Find difference between given peewee models."""
     changes = []
```

### Comparing `peewee_migrate-1.7.9/peewee_migrate/cli.py` & `peewee_migrate-1.8.0/peewee_migrate/cli.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.9/peewee_migrate/router.py` & `peewee_migrate-1.8.0/peewee_migrate/router.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.9/peewee_migrate/template.py` & `peewee_migrate-1.8.0/peewee_migrate/template.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.9/pyproject.toml` & `peewee_migrate-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-migrate"
-version = "1.7.9"
+version = "1.8.0"
 homepage = "https://github.com/klen/peewee_migrate"
 repository = "https://github.com/klen/peewee_migrate"
 description = "Support for migrations in Peewee ORM"
 readme = "README.rst"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["peewee", "migrations", "orm"]
```

### Comparing `peewee_migrate-1.7.9/PKG-INFO` & `peewee_migrate-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-migrate
-Version: 1.7.9
+Version: 1.8.0
 Summary: Support for migrations in Peewee ORM
 Home-page: https://github.com/klen/peewee_migrate
 License: MIT
 Keywords: peewee,migrations,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

