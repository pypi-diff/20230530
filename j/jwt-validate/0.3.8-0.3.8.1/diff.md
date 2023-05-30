# Comparing `tmp/jwt_validate-0.3.8.tar.gz` & `tmp/jwt_validate-0.3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwt_validate-0.3.8.tar", max compression
+gzip compressed data, was "jwt_validate-0.3.8.1.tar", max compression
```

## Comparing `jwt_validate-0.3.8.tar` & `jwt_validate-0.3.8.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1663 2023-05-30 15:11:58.453236 jwt_validate-0.3.8/index.md
--rw-r--r--   0        0        0        0 2023-05-30 15:11:58.453311 jwt_validate-0.3.8/jwt_validate/__init__.py
--rw-r--r--   0        0        0      523 2023-05-30 15:11:58.453791 jwt_validate-0.3.8/jwt_validate/config.py
--rw-r--r--   0        0        0      437 2023-05-30 15:11:58.453884 jwt_validate-0.3.8/jwt_validate/constants.py
--rw-r--r--   0        0        0      934 2023-05-30 15:11:58.453971 jwt_validate-0.3.8/jwt_validate/exceptions.py
--rw-r--r--   0        0        0      398 2023-05-30 15:11:58.454246 jwt_validate-0.3.8/jwt_validate/generate/generate_jwt.py
--rw-r--r--   0        0        0      243 2023-05-30 15:11:58.454336 jwt_validate-0.3.8/jwt_validate/utils.py
--rw-r--r--   0        0        0        0 2023-05-30 15:11:58.454386 jwt_validate-0.3.8/jwt_validate/validate/__init__.py
--rw-r--r--   0        0        0     3342 2023-05-30 15:11:58.457774 jwt_validate-0.3.8/jwt_validate/validate/validate_jwt.py
--rw-r--r--   0        0        0     2141 2023-05-30 18:03:09.634525 jwt_validate-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     2638 1970-01-01 00:00:00.000000 jwt_validate-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1663 2023-05-30 15:11:58.453236 jwt_validate-0.3.8.1/index.md
+-rw-r--r--   0        0        0        0 2023-05-30 15:11:58.453311 jwt_validate-0.3.8.1/jwt_validate/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-30 15:11:58.453791 jwt_validate-0.3.8.1/jwt_validate/config.py
+-rw-r--r--   0        0        0      437 2023-05-30 15:11:58.453884 jwt_validate-0.3.8.1/jwt_validate/constants.py
+-rw-r--r--   0        0        0      934 2023-05-30 15:11:58.453971 jwt_validate-0.3.8.1/jwt_validate/exceptions.py
+-rw-r--r--   0        0        0      398 2023-05-30 15:11:58.454246 jwt_validate-0.3.8.1/jwt_validate/generate/generate_jwt.py
+-rw-r--r--   0        0        0      243 2023-05-30 15:11:58.454336 jwt_validate-0.3.8.1/jwt_validate/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:11:58.454386 jwt_validate-0.3.8.1/jwt_validate/validate/__init__.py
+-rw-r--r--   0        0        0     3342 2023-05-30 15:11:58.457774 jwt_validate-0.3.8.1/jwt_validate/validate/validate_jwt.py
+-rw-r--r--   0        0        0     2168 2023-05-30 18:05:59.589916 jwt_validate-0.3.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 jwt_validate-0.3.8.1/PKG-INFO
```

### Comparing `jwt_validate-0.3.8/index.md` & `jwt_validate-0.3.8.1/index.md`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.8/jwt_validate/config.py` & `jwt_validate-0.3.8.1/jwt_validate/config.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.8/jwt_validate/exceptions.py` & `jwt_validate-0.3.8.1/jwt_validate/exceptions.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.8/jwt_validate/validate/validate_jwt.py` & `jwt_validate-0.3.8.1/jwt_validate/validate/validate_jwt.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.8/pyproject.toml` & `jwt_validate-0.3.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jwt-validate"
-version = "0.3.8"
+version = "0.3.8.1"
 description = "Library for validation token JWT"
 authors = ["Reinaldo Saraiva do Carmo <reinaldo.carmo@luizalabs.com>"]
 license = "BeerWare"
 readme = "index.md"
 packages = [{include = "jwt_validate"}]
 
 classifiers = [
@@ -19,14 +19,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = "^0.24.0"
 pyjwt = {extras = ["crypto"], version = "^2.7.0"}
 pytest-env = "^0.8.1"
+python-dotenv = "^1.0.0"
 
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.0"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
```

### Comparing `jwt_validate-0.3.8/PKG-INFO` & `jwt_validate-0.3.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwt-validate
-Version: 0.3.8
+Version: 0.3.8.1
 Summary: Library for validation token JWT
 License: Beerware
 Author: Reinaldo Saraiva do Carmo
 Author-email: reinaldo.carmo@luizalabs.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: FastAPI
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: pyjwt[crypto] (>=2.7.0,<3.0.0)
 Requires-Dist: pytest-env (>=0.8.1,<0.9.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ![logo do projeto](docs/assets/logo.png){width="100" .center}
 # JWT Validation
 
 The Python **jwt-validation library** is a collection of predefined codes and functions that allow users to verify a JWT token's authenticity and integrity. In other words, the library can be used to check if the JWT token is valid and was issued by a trusted source. In addition to decoding the JWT token, the library usually includes methods for verifying its digital signature, and extracting information from its header and payload. Application and system developers can integrate this library into user authentication and data security applications.
```

