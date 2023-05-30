# Comparing `tmp/jwt_validate-0.3.5.3.tar.gz` & `tmp/jwt_validate-0.3.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwt_validate-0.3.5.3.tar", max compression
+gzip compressed data, was "jwt_validate-0.3.5.4.tar", max compression
```

## Comparing `jwt_validate-0.3.5.3.tar` & `jwt_validate-0.3.5.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1663 2023-05-30 15:11:58.453236 jwt_validate-0.3.5.3/index.md
--rw-r--r--   0        0        0        0 2023-05-30 15:11:58.453311 jwt_validate-0.3.5.3/jwt_validate/__init__.py
--rw-r--r--   0        0        0      523 2023-05-30 15:11:58.453791 jwt_validate-0.3.5.3/jwt_validate/config.py
--rw-r--r--   0        0        0      437 2023-05-30 15:11:58.453884 jwt_validate-0.3.5.3/jwt_validate/constants.py
--rw-r--r--   0        0        0      934 2023-05-30 15:11:58.453971 jwt_validate-0.3.5.3/jwt_validate/exceptions.py
--rw-r--r--   0        0        0      398 2023-05-30 15:11:58.454246 jwt_validate-0.3.5.3/jwt_validate/generate/generate_jwt.py
--rw-r--r--   0        0        0      243 2023-05-30 15:11:58.454336 jwt_validate-0.3.5.3/jwt_validate/utils.py
--rw-r--r--   0        0        0        0 2023-05-30 15:11:58.454386 jwt_validate-0.3.5.3/jwt_validate/validate/__init__.py
--rw-r--r--   0        0        0     3342 2023-05-30 15:11:58.457774 jwt_validate-0.3.5.3/jwt_validate/validate/validate_jwt.py
--rw-r--r--   0        0        0     2148 2023-05-30 15:21:28.312227 jwt_validate-0.3.5.3/pyproject.toml
--rw-r--r--   0        0        0     2641 1970-01-01 00:00:00.000000 jwt_validate-0.3.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1663 2023-05-30 15:11:58.453236 jwt_validate-0.3.5.4/index.md
+-rw-r--r--   0        0        0        0 2023-05-30 15:11:58.453311 jwt_validate-0.3.5.4/jwt_validate/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-30 15:11:58.453791 jwt_validate-0.3.5.4/jwt_validate/config.py
+-rw-r--r--   0        0        0      437 2023-05-30 15:11:58.453884 jwt_validate-0.3.5.4/jwt_validate/constants.py
+-rw-r--r--   0        0        0      934 2023-05-30 15:11:58.453971 jwt_validate-0.3.5.4/jwt_validate/exceptions.py
+-rw-r--r--   0        0        0      398 2023-05-30 15:11:58.454246 jwt_validate-0.3.5.4/jwt_validate/generate/generate_jwt.py
+-rw-r--r--   0        0        0      243 2023-05-30 15:11:58.454336 jwt_validate-0.3.5.4/jwt_validate/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:11:58.454386 jwt_validate-0.3.5.4/jwt_validate/validate/__init__.py
+-rw-r--r--   0        0        0     3342 2023-05-30 15:11:58.457774 jwt_validate-0.3.5.4/jwt_validate/validate/validate_jwt.py
+-rw-r--r--   0        0        0     2148 2023-05-30 16:34:59.806332 jwt_validate-0.3.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2641 1970-01-01 00:00:00.000000 jwt_validate-0.3.5.4/PKG-INFO
```

### Comparing `jwt_validate-0.3.5.3/index.md` & `jwt_validate-0.3.5.4/index.md`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.5.3/jwt_validate/config.py` & `jwt_validate-0.3.5.4/jwt_validate/config.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.5.3/jwt_validate/exceptions.py` & `jwt_validate-0.3.5.4/jwt_validate/exceptions.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.5.3/jwt_validate/validate/validate_jwt.py` & `jwt_validate-0.3.5.4/jwt_validate/validate/validate_jwt.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.5.3/pyproject.toml` & `jwt_validate-0.3.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jwt-validate"
-version = "0.3.5.3"
+version = "0.3.5.4"
 description = "Library for validation token JWT"
 authors = ["Reinaldo Saraiva do Carmo <reinaldo.carmo@luizalabs.com>"]
 license = "BeerWare"
 readme = "index.md"
 packages = [{include = "jwt_validate"}]
 
 classifiers = [
```

### Comparing `jwt_validate-0.3.5.3/PKG-INFO` & `jwt_validate-0.3.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwt-validate
-Version: 0.3.5.3
+Version: 0.3.5.4
 Summary: Library for validation token JWT
 License: Beerware
 Author: Reinaldo Saraiva do Carmo
 Author-email: reinaldo.carmo@luizalabs.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: FastAPI
```

