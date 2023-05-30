# Comparing `tmp/jwt_validate-0.3.5.tar.gz` & `tmp/jwt_validate-0.3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwt_validate-0.3.5.tar", max compression
+gzip compressed data, was "jwt_validate-0.3.5.1.tar", max compression
```

## Comparing `jwt_validate-0.3.5.tar` & `jwt_validate-0.3.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1663 2023-05-19 12:12:52.897568 jwt_validate-0.3.5/index.md
--rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152260 jwt_validate-0.3.5/jwt_validate/__init__.py
--rw-r--r--   0        0        0      492 2023-05-19 17:00:39.522115 jwt_validate-0.3.5/jwt_validate/config.py
--rw-r--r--   0        0        0      437 2023-05-16 20:05:04.152451 jwt_validate-0.3.5/jwt_validate/constants.py
--rw-r--r--   0        0        0      934 2023-05-16 20:05:04.152530 jwt_validate-0.3.5/jwt_validate/exceptions.py
--rw-r--r--   0        0        0      395 2023-05-16 20:05:04.152650 jwt_validate-0.3.5/jwt_validate/generate/generate_jwt.py
--rw-r--r--   0        0        0      243 2023-05-16 20:05:04.152823 jwt_validate-0.3.5/jwt_validate/utils.py
--rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152895 jwt_validate-0.3.5/jwt_validate/validate/__init__.py
--rw-r--r--   0        0        0     3362 2023-05-19 17:03:52.093642 jwt_validate-0.3.5/jwt_validate/validate/validate_jwt.py
--rw-r--r--   0        0        0     2122 2023-05-23 11:59:22.547719 jwt_validate-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2638 1970-01-01 00:00:00.000000 jwt_validate-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1663 2023-05-19 12:12:52.897568 jwt_validate-0.3.5.1/index.md
+-rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152260 jwt_validate-0.3.5.1/jwt_validate/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-23 12:55:20.177338 jwt_validate-0.3.5.1/jwt_validate/config.py
+-rw-r--r--   0        0        0      437 2023-05-16 20:05:04.152451 jwt_validate-0.3.5.1/jwt_validate/constants.py
+-rw-r--r--   0        0        0      934 2023-05-16 20:05:04.152530 jwt_validate-0.3.5.1/jwt_validate/exceptions.py
+-rw-r--r--   0        0        0      398 2023-05-23 12:55:26.294712 jwt_validate-0.3.5.1/jwt_validate/generate/generate_jwt.py
+-rw-r--r--   0        0        0      243 2023-05-16 20:05:04.152823 jwt_validate-0.3.5.1/jwt_validate/utils.py
+-rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152895 jwt_validate-0.3.5.1/jwt_validate/validate/__init__.py
+-rw-r--r--   0        0        0     3342 2023-05-30 12:39:18.873959 jwt_validate-0.3.5.1/jwt_validate/validate/validate_jwt.py
+-rw-r--r--   0        0        0     2054 2023-05-30 13:23:30.690366 jwt_validate-0.3.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 jwt_validate-0.3.5.1/PKG-INFO
```

### Comparing `jwt_validate-0.3.5/index.md` & `jwt_validate-0.3.5.1/index.md`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.5/jwt_validate/exceptions.py` & `jwt_validate-0.3.5.1/jwt_validate/exceptions.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.5/jwt_validate/validate/validate_jwt.py` & `jwt_validate-0.3.5.1/jwt_validate/validate/validate_jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from fastapi import (
     Depends,
     HTTPException,
 )
 from fastapi.security import (
     HTTPBearer,
     OAuth2PasswordBearer,
-    SecurityScopes,
 )
 from jwt.exceptions import (
     DecodeError,
     ExpiredSignatureError,
 )
 
 from jwt_validate.config import settings
```

### Comparing `jwt_validate-0.3.5/pyproject.toml` & `jwt_validate-0.3.5.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jwt-validate"
-version = "0.3.5"
+version = "0.3.5.1"
 description = "Library for validation token JWT"
 authors = ["Reinaldo Saraiva do Carmo <reinaldo.carmo@luizalabs.com>"]
 license = "BeerWare"
 readme = "index.md"
 packages = [{include = "jwt_validate"}]
 
 classifiers = [
@@ -15,18 +15,15 @@
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
-httpx = "^0.24.0"
-pytest-mock = "^3.10.0"
-pytest-asyncio = "^0.21.0"
+python = "^3.8"
 pyjwt = {extras = ["crypto"], version = "^2.7.0"}
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.0"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
```

### Comparing `jwt_validate-0.3.5/PKG-INFO` & `jwt_validate-0.3.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: jwt-validate
-Version: 0.3.5
+Version: 0.3.5.1
 Summary: Library for validation token JWT
 License: Beerware
 Author: Reinaldo Saraiva do Carmo
 Author-email: reinaldo.carmo@luizalabs.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: pyjwt[crypto] (>=2.7.0,<3.0.0)
-Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
-Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 ![logo do projeto](docs/assets/logo.png){width="100" .center}
 # JWT Validation
 
 The Python **jwt-validation library** is a collection of predefined codes and functions that allow users to verify a JWT token's authenticity and integrity. In other words, the library can be used to check if the JWT token is valid and was issued by a trusted source. In addition to decoding the JWT token, the library usually includes methods for verifying its digital signature, and extracting information from its header and payload. Application and system developers can integrate this library into user authentication and data security applications.
```

