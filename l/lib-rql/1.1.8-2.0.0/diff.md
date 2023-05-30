# Comparing `tmp/lib_rql-1.1.8.tar.gz` & `tmp/lib_rql-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_rql-1.1.8.tar", max compression
+gzip compressed data, was "lib_rql-2.0.0.tar", max compression
```

## Comparing `lib_rql-1.1.8.tar` & `lib_rql-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-03-16 10:56:30.624679 lib_rql-1.1.8/LICENSE
--rw-r--r--   0        0        0     3968 2023-03-16 10:56:30.624679 lib_rql-1.1.8/README.md
--rw-r--r--   0        0        0      347 2023-03-16 10:56:30.624679 lib_rql-1.1.8/py_rql/__init__.py
--rw-r--r--   0        0        0     1068 2023-03-16 10:56:30.624679 lib_rql-1.1.8/py_rql/cast.py
--rw-r--r--   0        0        0     2863 2023-03-16 10:56:30.624679 lib_rql-1.1.8/py_rql/constants.py
--rw-r--r--   0        0        0      941 2023-03-16 10:56:30.624679 lib_rql-1.1.8/py_rql/exceptions.py
--rw-r--r--   0        0        0     3223 2023-03-16 10:56:30.624679 lib_rql-1.1.8/py_rql/filter_cls.py
--rw-r--r--   0        0        0     2375 2023-03-16 10:56:30.624679 lib_rql-1.1.8/py_rql/grammar.py
--rw-r--r--   0        0        0      651 2023-03-16 10:56:30.624679 lib_rql-1.1.8/py_rql/helpers.py
--rw-r--r--   0        0        0     1336 2023-03-16 10:56:30.624679 lib_rql-1.1.8/py_rql/operators.py
--rw-r--r--   0        0        0      957 2023-03-16 10:56:30.624679 lib_rql-1.1.8/py_rql/parser.py
--rw-r--r--   0        0        0     2962 2023-03-16 10:56:30.624679 lib_rql-1.1.8/py_rql/transformer.py
--rw-r--r--   0        0        0     2507 2023-03-16 10:57:07.776587 lib_rql-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     5217 1970-01-01 00:00:00.000000 lib_rql-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 12:20:15.307308 lib_rql-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3968 2023-05-30 12:20:15.307308 lib_rql-2.0.0/README.md
+-rw-r--r--   0        0        0      347 2023-05-30 12:20:15.307308 lib_rql-2.0.0/py_rql/__init__.py
+-rw-r--r--   0        0        0     1068 2023-05-30 12:20:15.307308 lib_rql-2.0.0/py_rql/cast.py
+-rw-r--r--   0        0        0     2863 2023-05-30 12:20:15.307308 lib_rql-2.0.0/py_rql/constants.py
+-rw-r--r--   0        0        0      941 2023-05-30 12:20:15.307308 lib_rql-2.0.0/py_rql/exceptions.py
+-rw-r--r--   0        0        0     3223 2023-05-30 12:20:15.307308 lib_rql-2.0.0/py_rql/filter_cls.py
+-rw-r--r--   0        0        0     2375 2023-05-30 12:20:15.307308 lib_rql-2.0.0/py_rql/grammar.py
+-rw-r--r--   0        0        0      651 2023-05-30 12:20:15.307308 lib_rql-2.0.0/py_rql/helpers.py
+-rw-r--r--   0        0        0     1336 2023-05-30 12:20:15.311308 lib_rql-2.0.0/py_rql/operators.py
+-rw-r--r--   0        0        0      957 2023-05-30 12:20:15.311308 lib_rql-2.0.0/py_rql/parser.py
+-rw-r--r--   0        0        0     2962 2023-05-30 12:20:15.311308 lib_rql-2.0.0/py_rql/transformer.py
+-rw-r--r--   0        0        0     2801 2023-05-30 12:20:49.247774 lib_rql-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4915 1970-01-01 00:00:00.000000 lib_rql-2.0.0/PKG-INFO
```

### Comparing `lib_rql-1.1.8/LICENSE` & `lib_rql-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_rql-1.1.8/README.md` & `lib_rql-2.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -119,20 +119,20 @@
 print(results)
 ```
 
 
 ## Development
 
 
-1. Python 3.7+
+1. Python 3.8+
 0. Install dependencies `pip install poetry && poetry install`
 
 ## Testing
 
-1. Python 3.7+
+1. Python 3.8+
 0. Install dependencies `pip install poetry && poetry install`
 
 Check code style: `poetry run flake8`
 Run tests: `poetry run pytest`
 
 Tests reports are generated in `tests/reports`.
 * `out.xml` - JUnit test results
```

### Comparing `lib_rql-1.1.8/py_rql/cast.py` & `lib_rql-2.0.0/py_rql/cast.py`

 * *Files identical despite different names*

### Comparing `lib_rql-1.1.8/py_rql/constants.py` & `lib_rql-2.0.0/py_rql/constants.py`

 * *Files identical despite different names*

### Comparing `lib_rql-1.1.8/py_rql/exceptions.py` & `lib_rql-2.0.0/py_rql/exceptions.py`

 * *Files identical despite different names*

### Comparing `lib_rql-1.1.8/py_rql/filter_cls.py` & `lib_rql-2.0.0/py_rql/filter_cls.py`

 * *Files identical despite different names*

### Comparing `lib_rql-1.1.8/py_rql/grammar.py` & `lib_rql-2.0.0/py_rql/grammar.py`

 * *Files identical despite different names*

### Comparing `lib_rql-1.1.8/py_rql/helpers.py` & `lib_rql-2.0.0/py_rql/helpers.py`

 * *Files identical despite different names*

### Comparing `lib_rql-1.1.8/py_rql/operators.py` & `lib_rql-2.0.0/py_rql/operators.py`

 * *Files identical despite different names*

### Comparing `lib_rql-1.1.8/py_rql/parser.py` & `lib_rql-2.0.0/py_rql/parser.py`

 * *Files identical despite different names*

### Comparing `lib_rql-1.1.8/py_rql/transformer.py` & `lib_rql-2.0.0/py_rql/transformer.py`

 * *Files identical despite different names*

### Comparing `lib_rql-1.1.8/pyproject.toml` & `lib_rql-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [tool.poetry]
 name = "lib-rql"
-version = "1.1.8"
+version = "2.0.0"
 description = "Python RQL Filtering"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "py_rql" }
 ]
 readme = "./README.md"
 homepage = "https://connect.cloudblue.com/community/api/rql/"
 repository = "https://github.com/cloudblue/lib-rql"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: Unix",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Text Processing :: Filters"
 ]
 keywords = [
     "rql",
     "filter",
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4"
+python = ">=3.8,<4"
 lark-parser = "0.11.0"
 cachetools = ">=4.2.4"
 python-dateutil = ">=2.8.2"
 
 [tool.poetry.group.test.dependencies]
 ipython = ">=7.10.0"
 pytest = ">=6.1.2,<8"
@@ -41,16 +40,17 @@
 pytest-mock = "^3.3.1"
 coverage = {extras = ["toml"], version = ">=5.3,<7"}
 flake8 = ">=3.8,<6"
 flake8-bugbear = ">=20,<23"
 flake8-cognitive-complexity = "^0.1"
 flake8-commas = "~2.1"
 flake8-future-import = "~0.4"
-flake8-isort = "^5.0"
+flake8-isort = "^6.0"
 flake8-broken-line = ">=0.3,<0.7"
+flake8-pyproject = "^1.2.3"
 isort = "^5.10"
 importlib-metadata = "<5"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = ">=1.4"
 mkdocs-material = ">=9"
 mkdocs-glightbox = "^0.3.1"
@@ -95,7 +95,26 @@
 multi_line_output = 3
 force_grid_wrap = 4
 combine_as_imports = true
 use_parentheses = true
 include_trailing_comma = true
 line_length = 100
 lines_after_imports = 2
+
+[tool.flake8]
+exclude = [
+    ".idea",
+    ".vscode",
+    ".git",
+    "pg_data",
+    "venv",
+    "*.eggs",
+    "*.egg",
+    "tests/fixtures",
+    "setup.py",
+    "resources",
+    "docs/*",
+]
+show-source = true
+max-line-length = 100
+max-cognitive-complexity = 20
+ignore = ["FI1", "I100", "W503", "W605", "B008"]
```

### Comparing `lib_rql-1.1.8/PKG-INFO` & `lib_rql-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 Metadata-Version: 2.1
 Name: lib-rql
-Version: 1.1.8
+Version: 2.0.0
 Summary: Python RQL Filtering
 Home-page: https://connect.cloudblue.com/community/api/rql/
 License: Apache-2.0
 Keywords: rql,filter
 Author: CloudBlue LLC
-Requires-Python: >=3.7,<4
+Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Text Processing :: Filters
 Requires-Dist: cachetools (>=4.2.4)
 Requires-Dist: lark-parser (==0.11.0)
 Requires-Dist: python-dateutil (>=2.8.2)
 Project-URL: Repository, https://github.com/cloudblue/lib-rql
 Description-Content-Type: text/markdown
 
@@ -150,20 +144,20 @@
 print(results)
 ```
 
 
 ## Development
 
 
-1. Python 3.7+
+1. Python 3.8+
 0. Install dependencies `pip install poetry && poetry install`
 
 ## Testing
 
-1. Python 3.7+
+1. Python 3.8+
 0. Install dependencies `pip install poetry && poetry install`
 
 Check code style: `poetry run flake8`
 Run tests: `poetry run pytest`
 
 Tests reports are generated in `tests/reports`.
 * `out.xml` - JUnit test results
```

