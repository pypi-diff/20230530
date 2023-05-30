# Comparing `tmp/eodc-2023.5.0rc1.tar.gz` & `tmp/eodc-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.5.0rc1.tar", max compression
+gzip compressed data, was "eodc-2023.5.1.tar", max compression
```

## Comparing `eodc-2023.5.0rc1.tar` & `eodc-2023.5.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0       62 2023-05-26 08:27:29.080520 eodc-2023.5.0rc1/README.md
--rw-r--r--   0        0        0       30 2023-05-26 08:27:29.080520 eodc-2023.5.0rc1/eodc/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 08:27:29.080520 eodc-2023.5.0rc1/eodc/client.py
--rw-r--r--   0        0        0      125 2023-05-26 08:27:29.080520 eodc-2023.5.0rc1/eodc/config.py
--rw-r--r--   0        0        0        0 2023-05-26 08:27:29.080520 eodc-2023.5.0rc1/eodc/dask_clusters.py
--rw-r--r--   0        0        0      108 2023-05-26 08:27:29.080520 eodc-2023.5.0rc1/eodc/processors.py
--rw-r--r--   0        0        0     1070 2023-05-26 08:27:29.080520 eodc-2023.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 eodc-2023.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-05-30 13:05:38.838561 eodc-2023.5.1/README.md
+-rw-r--r--   0        0        0      213 2023-05-30 13:05:38.838561 eodc-2023.5.1/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-05-30 13:05:38.838561 eodc-2023.5.1/eodc/dask.py
+-rw-r--r--   0        0        0      410 2023-05-30 13:05:38.838561 eodc-2023.5.1/eodc/faas.py
+-rw-r--r--   0        0        0      469 2023-05-30 13:05:38.838561 eodc-2023.5.1/eodc/settings.py
+-rw-r--r--   0        0        0     1114 2023-05-30 13:05:38.838561 eodc-2023.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 eodc-2023.5.1/PKG-INFO
```

### Comparing `eodc-2023.5.0rc1/pyproject.toml` & `eodc-2023.5.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.5.0-rc.1"
+version = "2023.5.1"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 packages = [{include = "eodc"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.12"
 requests = "^2.28.2"
 pydantic = "^1.10.7"
 argo-workflows = "6.3.9"
+dask-gateway = "^2022.11.0"
+eodc-faas-force = "^2023.5.2"
+eodc-faas-sen2like = "^2023.5.0rc0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.0"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 ipykernel = "^6.22.0"
```

