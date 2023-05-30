# Comparing `tmp/configzen-0.1.43.tar.gz` & `tmp/configzen-0.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.43.tar", max compression
+gzip compressed data, was "configzen-0.1.44.tar", max compression
```

## Comparing `configzen-0.1.43.tar` & `configzen-0.1.44.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.43/configzen/__init__.py
--rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.1.43/configzen/__main__.py
--rw-r--r--   0        0        0    58987 2023-05-30 00:54:06.267200 configzen-0.1.43/configzen/config.py
--rw-r--r--   0        0        0     2553 2023-05-30 00:29:12.193684 configzen-0.1.43/configzen/errors.py
--rw-r--r--   0        0        0    20820 2023-05-30 00:45:02.555346 configzen-0.1.43/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.43/configzen/py.typed
--rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.1.43/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.43/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-30 00:54:30.991315 configzen-0.1.43/pyproject.toml
--rw-r--r--   0        0        0     7326 2023-05-30 00:29:12.142683 configzen-0.1.43/README.md
--rw-r--r--   0        0        0     7806 1970-01-01 00:00:00.000000 configzen-0.1.43/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.44/configzen/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.1.44/configzen/__main__.py
+-rw-r--r--   0        0        0    58999 2023-05-30 00:59:59.013627 configzen-0.1.44/configzen/config.py
+-rw-r--r--   0        0        0     2553 2023-05-30 00:29:12.193684 configzen-0.1.44/configzen/errors.py
+-rw-r--r--   0        0        0    20820 2023-05-30 00:45:02.555346 configzen-0.1.44/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.44/configzen/py.typed
+-rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.1.44/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.44/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-30 01:00:43.050064 configzen-0.1.44/pyproject.toml
+-rw-r--r--   0        0        0     7326 2023-05-30 00:29:12.142683 configzen-0.1.44/README.md
+-rw-r--r--   0        0        0     7806 1970-01-01 00:00:00.000000 configzen-0.1.44/PKG-INFO
```

### Comparing `configzen-0.1.43/configzen/__main__.py` & `configzen-0.1.44/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.43/configzen/config.py` & `configzen-0.1.44/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1634,18 +1634,18 @@
         )
 
         if kwargs.pop("root", None):
             return type.__new__(cls, name, bases, namespace, **kwargs)
 
         new_class = super().__new__(cls, name, bases, namespace, **kwargs)
         for field in new_class.__fields__.values():
-            if type(field.type_) is ConfigModelMetaclass:
+            if type(field.outer_type_) is ConfigModelMetaclass:
                 if field.pre_validators is None:
                     field.pre_validators = []
-                validator = make_generic_validator(field.type_.__field_setup__)
+                validator = make_generic_validator(field.outer_type_.__field_setup__)
                 field.pre_validators.insert(0, validator)
         new_class.__json_encoder__ = functools.partial(
             _json_encoder,
             new_class.__json_encoder__,
         )
         return cast(type, new_class)
```

### Comparing `configzen-0.1.43/configzen/errors.py` & `configzen-0.1.44/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.43/configzen/processor.py` & `configzen-0.1.44/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.43/configzen/typedefs.py` & `configzen-0.1.44/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.43/LICENSE` & `configzen-0.1.44/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.43/pyproject.toml` & `configzen-0.1.44/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.43"
+version = "0.1.44"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.43/README.md` & `configzen-0.1.44/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.43/PKG-INFO` & `configzen-0.1.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.43
+Version: 0.1.44
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

