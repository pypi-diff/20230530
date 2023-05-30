# Comparing `tmp/searchcode-cli-2.1.2.tar.gz` & `tmp/searchcode-cli-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchcode-cli-2.1.2.tar", last modified: Sun May 21 04:40:49 2023, max compression
+gzip compressed data, was "searchcode-cli-2.1.3.tar", last modified: Tue May 30 08:58:29 2023, max compression
```

## Comparing `searchcode-cli-2.1.2.tar` & `searchcode-cli-2.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43192 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/searchcode/
--rw-r--r--   0 runner    (1001) docker     (123)    26906 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/searchcode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/searchcode/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/searchcode/miscellaneous.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/searchcode_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43192 2023-05-21 04:40:49.000000 searchcode-cli-2.1.2/searchcode_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-21 04:40:49.000000 searchcode-cli-2.1.2/searchcode_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 04:40:49.000000 searchcode-cli-2.1.2/searchcode_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 04:40:49.000000 searchcode-cli-2.1.2/searchcode_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:58:29.185176 searchcode-cli-2.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:58:29.185176 searchcode-cli-2.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:58:29.185176 searchcode-cli-2.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-30 08:58:17.000000 searchcode-cli-2.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-30 08:58:17.000000 searchcode-cli-2.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-30 08:58:17.000000 searchcode-cli-2.1.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:58:29.185176 searchcode-cli-2.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-30 08:58:17.000000 searchcode-cli-2.1.3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-30 08:58:17.000000 searchcode-cli-2.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-30 08:58:17.000000 searchcode-cli-2.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-30 08:58:17.000000 searchcode-cli-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43192 2023-05-30 08:58:29.185176 searchcode-cli-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-30 08:58:17.000000 searchcode-cli-2.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-30 08:58:17.000000 searchcode-cli-2.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:58:29.185176 searchcode-cli-2.1.3/searchcode/
+-rw-r--r--   0 runner    (1001) docker     (123)    26898 2023-05-30 08:58:17.000000 searchcode-cli-2.1.3/searchcode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-30 08:58:17.000000 searchcode-cli-2.1.3/searchcode/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-05-30 08:58:17.000000 searchcode-cli-2.1.3/searchcode/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:58:29.185176 searchcode-cli-2.1.3/searchcode_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43192 2023-05-30 08:58:29.000000 searchcode-cli-2.1.3/searchcode_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-30 08:58:29.000000 searchcode-cli-2.1.3/searchcode_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:58:29.000000 searchcode-cli-2.1.3/searchcode_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 08:58:29.000000 searchcode-cli-2.1.3/searchcode_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:58:29.185176 searchcode-cli-2.1.3/setup.cfg
```

### Comparing `searchcode-cli-2.1.2/.github/ISSUE_TEMPLATE/bug_report.md` & `searchcode-cli-2.1.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `searchcode-cli-2.1.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.2/.github/workflows/codeql.yml` & `searchcode-cli-2.1.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.2/.github/workflows/python-publish.yml` & `searchcode-cli-2.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.2/.gitignore` & `searchcode-cli-2.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.2/LICENSE` & `searchcode-cli-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.2/PKG-INFO` & `searchcode-cli-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchcode-cli
-Version: 2.1.2
+Version: 2.1.3
 Summary: A Python wrapper around the searchcode API
 Author-email: Richard Mwewa <rly0nheart@duck.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `searchcode-cli-2.1.2/README.md` & `searchcode-cli-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.2/pyproject.toml` & `searchcode-cli-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "searchcode-cli"
-version = "2.1.2"
+version = "2.1.3"
 description = "A Python wrapper around the searchcode API"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["searchcode", "search-engine", "codesearch", "api-wrapper"]
 authors = [{name = "Richard Mwewa", email = "rly0nheart@duck.com"}]
 classifiers = [
```

### Comparing `searchcode-cli-2.1.2/searchcode/__init__.py` & `searchcode-cli-2.1.3/searchcode/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Search code api endpoints
 from typing import Union, Literal
 from searchcode.connection import __api_handler
-from searchcode.miscellaneous import __code_sources, __code_languages, __api_endpoints  # searchcode API endpoints
+from searchcode.utils import __code_sources, __code_languages, __api_endpoints  # searchcode API endpoints
 
 
 def __join_parameters(names, sources) -> str:
     """
     Returns a single string of joined parameters for the given list of filter names and sources.
 
     Parameters:
```

### Comparing `searchcode-cli-2.1.2/searchcode/connection.py` & `searchcode-cli-2.1.3/searchcode/connection.py`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.2/searchcode/miscellaneous.py` & `searchcode-cli-2.1.3/searchcode/utils.py`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.2/searchcode_cli.egg-info/PKG-INFO` & `searchcode-cli-2.1.3/searchcode_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchcode-cli
-Version: 2.1.2
+Version: 2.1.3
 Summary: A Python wrapper around the searchcode API
 Author-email: Richard Mwewa <rly0nheart@duck.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

