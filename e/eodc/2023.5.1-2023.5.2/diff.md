# Comparing `tmp/eodc-2023.5.1.tar.gz` & `tmp/eodc-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.5.1.tar", max compression
+gzip compressed data, was "eodc-2023.5.2.tar", max compression
```

## Comparing `eodc-2023.5.1.tar` & `eodc-2023.5.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      513 2023-05-30 13:05:38.838561 eodc-2023.5.1/README.md
--rw-r--r--   0        0        0      213 2023-05-30 13:05:38.838561 eodc-2023.5.1/eodc/__init__.py
--rw-r--r--   0        0        0     1102 2023-05-30 13:05:38.838561 eodc-2023.5.1/eodc/dask.py
--rw-r--r--   0        0        0      410 2023-05-30 13:05:38.838561 eodc-2023.5.1/eodc/faas.py
--rw-r--r--   0        0        0      469 2023-05-30 13:05:38.838561 eodc-2023.5.1/eodc/settings.py
--rw-r--r--   0        0        0     1114 2023-05-30 13:05:38.838561 eodc-2023.5.1/pyproject.toml
--rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 eodc-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-05-30 19:27:13.728942 eodc-2023.5.2/README.md
+-rw-r--r--   0        0        0      213 2023-05-30 19:27:13.728942 eodc-2023.5.2/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-05-30 19:27:13.728942 eodc-2023.5.2/eodc/dask.py
+-rw-r--r--   0        0        0      590 2023-05-30 19:27:13.728942 eodc-2023.5.2/eodc/faas.py
+-rw-r--r--   0        0        0      469 2023-05-30 19:27:13.728942 eodc-2023.5.2/eodc/settings.py
+-rw-r--r--   0        0        0     1114 2023-05-30 19:27:13.728942 eodc-2023.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 eodc-2023.5.2/PKG-INFO
```

### Comparing `eodc-2023.5.1/README.md` & `eodc-2023.5.2/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2023.5.1/eodc/dask.py` & `eodc-2023.5.2/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.5.1/pyproject.toml` & `eodc-2023.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.5.1"
+version = "2023.5.2"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
@@ -21,15 +21,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 requests = "^2.28.2"
 pydantic = "^1.10.7"
 argo-workflows = "6.3.9"
 dask-gateway = "^2022.11.0"
-eodc-faas-force = "^2023.5.2"
+eodc-faas-force = "^2023.5.3"
 eodc-faas-sen2like = "^2023.5.0rc0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.0"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 ipykernel = "^6.22.0"
```

### Comparing `eodc-2023.5.1/PKG-INFO` & `eodc-2023.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: argo-workflows (==6.3.9)
 Requires-Dist: dask-gateway (>=2022.11.0,<2023.0.0)
-Requires-Dist: eodc-faas-force (>=2023.5.2,<2024.0.0)
+Requires-Dist: eodc-faas-force (>=2023.5.3,<2024.0.0)
 Requires-Dist: eodc-faas-sen2like (>=2023.5.0rc0,<2024.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/eodcgmbh/eodc-sdk
 Description-Content-Type: text/markdown
 
 # EODC SDK
```

