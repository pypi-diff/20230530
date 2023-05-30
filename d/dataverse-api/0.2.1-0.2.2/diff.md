# Comparing `tmp/dataverse_api-0.2.1.tar.gz` & `tmp/dataverse_api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse_api-0.2.1.tar", max compression
+gzip compressed data, was "dataverse_api-0.2.2.tar", max compression
```

## Comparing `dataverse_api-0.2.1.tar` & `dataverse_api-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       61 2023-05-12 18:28:06.104392 dataverse_api-0.2.1/dataverse_api/__init__.py
--rw-r--r--   0        0        0    24199 2023-05-30 13:07:59.598806 dataverse_api-0.2.1/dataverse_api/dataverse.py
--rw-r--r--   0        0        0     8295 2023-05-30 12:51:33.789474 dataverse_api-0.2.1/dataverse_api/utils.py
--rw-r--r--   0        0        0     1093 2023-05-12 18:09:25.896155 dataverse_api-0.2.1/LICENSE
--rw-r--r--   0        0        0      831 2023-05-30 13:08:43.101011 dataverse_api-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3977 2023-05-30 13:12:39.164555 dataverse_api-0.2.1/README.md
--rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 dataverse_api-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-05-12 18:28:06.104392 dataverse_api-0.2.2/dataverse_api/__init__.py
+-rw-r--r--   0        0        0    24199 2023-05-30 13:41:54.658389 dataverse_api-0.2.2/dataverse_api/dataverse.py
+-rw-r--r--   0        0        0     8295 2023-05-30 13:41:54.659390 dataverse_api-0.2.2/dataverse_api/utils.py
+-rw-r--r--   0        0        0     1093 2023-05-12 18:09:25.896155 dataverse_api-0.2.2/LICENSE
+-rw-r--r--   0        0        0      801 2023-05-30 14:37:37.603132 dataverse_api-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3977 2023-05-30 13:41:54.655391 dataverse_api-0.2.2/README.md
+-rw-r--r--   0        0        0     4528 1970-01-01 00:00:00.000000 dataverse_api-0.2.2/PKG-INFO
```

### Comparing `dataverse_api-0.2.1/dataverse_api/dataverse.py` & `dataverse_api-0.2.2/dataverse_api/dataverse.py`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.2.1/dataverse_api/utils.py` & `dataverse_api-0.2.2/dataverse_api/utils.py`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.2.1/LICENSE` & `dataverse_api-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.2.1/pyproject.toml` & `dataverse_api-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "dataverse-api"
-version = "0.2.1"
+version = "0.2.2"
 description = "Abstraction layer for interacting with Microsoft Dataverse in Python. Supports batch operations!"
 authors = ["Marcus Risanger <69350948+MarcusRisanger@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 msal = "^1.22.0"
 msal-requests-auth = "^0.7.0"
 pandas = "^2.0.1"
-requests-toolbelt = "^1.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ipykernel = "^6.22.0"
 python-dotenv = "^1.0.0"
 flake8 = "^6.0.0"
```

### Comparing `dataverse_api-0.2.1/README.md` & `dataverse_api-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.2.1/PKG-INFO` & `dataverse_api-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: dataverse-api
-Version: 0.2.1
+Version: 0.2.2
 Summary: Abstraction layer for interacting with Microsoft Dataverse in Python. Supports batch operations!
 Author: Marcus Risanger
 Author-email: 69350948+MarcusRisanger@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: msal (>=1.22.0,<2.0.0)
 Requires-Dist: msal-requests-auth (>=0.7.0,<0.8.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # `dataverse-api`
 
 [![Build Status](https://github.com/MarcusRisanger/dataverse-api/workflows/release/badge.svg)](https://github.com/MarcusRisanger/dataverse-api/actions)
 [![codecov](https://codecov.io/gh/MarcusRisanger/Dataverse-API/branch/main/graph/badge.svg)](https://codecov.io/gh/MarcusRisanger/Dataverse-API)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

