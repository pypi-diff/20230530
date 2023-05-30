# Comparing `tmp/uium-0.3.2.tar.gz` & `tmp/uium-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uium-0.3.2.tar", max compression
+gzip compressed data, was "uium-0.3.3.tar", max compression
```

## Comparing `uium-0.3.2.tar` & `uium-0.3.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 uium-0.3.2/LICENSE
--rw-r--r--   0        0        0     1450 2023-05-30 08:04:31.358253 uium-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      596 2023-05-30 02:29:40.011464 uium-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-05-30 05:42:23.658495 uium-0.3.2/uium/__init__.py
--rw-r--r--   0        0        0     1963 1970-01-01 00:00:00.000000 uium-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 uium-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1478 2023-05-30 08:46:00.459841 uium-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      596 2023-05-30 02:29:40.011464 uium-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 05:42:23.658495 uium-0.3.3/uium/__init__.py
+-rw-r--r--   0        0        0     2013 1970-01-01 00:00:00.000000 uium-0.3.3/PKG-INFO
```

### Comparing `uium-0.3.2/LICENSE` & `uium-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uium-0.3.2/pyproject.toml` & `uium-0.3.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uium"
-version = "0.3.2"
+version = "0.3.3"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/uium"
 repository = "https://github.com/MarkHoo/uium"
 classifiers = [
@@ -34,12 +34,12 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/MarkHoo/uium/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 undetected-chromedriver = "^3.4.7"
 selenium = "^4.9.1"
-
+webdriver-manager = "^3.8.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `uium-0.3.2/README.md` & `uium-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `uium-0.3.2/PKG-INFO` & `uium-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uium
-Version: 0.3.2
+Version: 0.3.3
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/uium
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: selenium (>=4.9.1,<5.0.0)
 Requires-Dist: undetected-chromedriver (>=3.4.7,<4.0.0)
+Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0)
 Project-URL: Bug Tracker, https://github.com/MarkHoo/uium/issues
 Project-URL: Repository, https://github.com/MarkHoo/uium
 Description-Content-Type: text/markdown
 
 # uium
 
 #### Installing
```

