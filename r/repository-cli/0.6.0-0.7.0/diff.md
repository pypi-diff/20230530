# Comparing `tmp/repository-cli-0.6.0.tar.gz` & `tmp/repository-cli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repository-cli-0.6.0.tar", last modified: Sun Apr 30 22:39:32 2023, max compression
+gzip compressed data, was "repository-cli-0.7.0.tar", last modified: Tue May 30 08:35:56 2023, max compression
```

## Comparing `repository-cli-0.6.0.tar` & `repository-cli-0.7.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.200523 repository-cli-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-30 22:39:26.000000 repository-cli-0.6.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.196524 repository-cli-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.196524 repository-cli-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-30 22:39:26.000000 repository-cli-0.6.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 22:39:26.000000 repository-cli-0.6.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-30 22:39:26.000000 repository-cli-0.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-30 22:39:26.000000 repository-cli-0.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-30 22:39:26.000000 repository-cli-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-30 22:39:26.000000 repository-cli-0.6.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-30 22:39:26.000000 repository-cli-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-30 22:39:26.000000 repository-cli-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-30 22:39:32.200523 repository-cli-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-30 22:39:26.000000 repository-cli-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.196524 repository-cli-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.200523 repository-cli-0.6.0/repository_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/click_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/click_param_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/records.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.200523 repository-cli-0.6.0/repository_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-30 22:39:26.000000 repository-cli-0.6.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-04-30 22:39:26.000000 repository-cli-0.6.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-30 22:39:32.200523 repository-cli-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-30 22:39:26.000000 repository-cli-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.200523 repository-cli-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-04-30 22:39:26.000000 repository-cli-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-30 22:39:26.000000 repository-cli-0.6.0/tests/test_rdmrecords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-30 22:39:26.000000 repository-cli-0.6.0/tests/test_rdmrecords_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-30 22:39:26.000000 repository-cli-0.6.0/tests/test_rdmrecords_pids.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-30 22:39:26.000000 repository-cli-0.6.0/tests/test_repository_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.657745 repository-cli-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-30 08:35:49.000000 repository-cli-0.7.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.653745 repository-cli-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.653745 repository-cli-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-30 08:35:49.000000 repository-cli-0.7.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-30 08:35:49.000000 repository-cli-0.7.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 08:35:49.000000 repository-cli-0.7.0/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-30 08:35:49.000000 repository-cli-0.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-30 08:35:49.000000 repository-cli-0.7.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-30 08:35:49.000000 repository-cli-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-30 08:35:49.000000 repository-cli-0.7.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-30 08:35:49.000000 repository-cli-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 08:35:49.000000 repository-cli-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-30 08:35:56.657745 repository-cli-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-30 08:35:49.000000 repository-cli-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.657745 repository-cli-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-30 08:35:49.000000 repository-cli-0.7.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.657745 repository-cli-0.7.0/repository_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/click_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/click_param_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-30 08:35:49.000000 repository-cli-0.7.0/repository_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.657745 repository-cli-0.7.0/repository_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 08:35:56.000000 repository-cli-0.7.0/repository_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-30 08:35:49.000000 repository-cli-0.7.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-05-30 08:35:49.000000 repository-cli-0.7.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-30 08:35:56.657745 repository-cli-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 08:35:49.000000 repository-cli-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:35:56.657745 repository-cli-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-05-30 08:35:49.000000 repository-cli-0.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-30 08:35:49.000000 repository-cli-0.7.0/tests/test_rdmrecords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-30 08:35:49.000000 repository-cli-0.7.0/tests/test_rdmrecords_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-30 08:35:49.000000 repository-cli-0.7.0/tests/test_rdmrecords_pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-30 08:35:49.000000 repository-cli-0.7.0/tests/test_repository_cli.py
```

### Comparing `repository-cli-0.6.0/.github/workflows/tests.yml` & `repository-cli-0.7.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `repository-cli-0.6.0/CHANGES.rst` & `repository-cli-0.7.0/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,23 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.7.0 (release 2023-05-30)
+
+- test: fix and pin due flask-babelex
+- records: separate replace-file from add-file
+- fix: black color on black background, bad
+- types: otherwise it is not working with 3.9
+- global: migrate to ruff
+
+
 Version v0.6.0 (release 2023-05-01)
 
 - cli: add command publish
 - cli: add record_id parameter to modify-access
 
 
 Version v0.5.0 (release 2023-03-08)
```

### Comparing `repository-cli-0.6.0/CONTRIBUTING.rst` & `repository-cli-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.6.0/LICENSE` & `repository-cli-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `repository-cli-0.6.0/MANIFEST.in` & `repository-cli-0.7.0/MANIFEST.in`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 recursive-include .github/workflows *.yml
 recursive-include repository_cli/translations *.po *.pot *.mo
 
 # added by check-manifest
 include *.rst
 include *.sh
 include *.txt
+include *.toml
 include LICENSE
 include babel.ini
 include pytest.ini
 recursive-include docs *.bat
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
```

### Comparing `repository-cli-0.6.0/PKG-INFO` & `repository-cli-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-cli
-Version: 0.6.0
+Version: 0.7.0
 Summary: "CLI utilities for TU Graz Repository."
 Home-page: https://github.com/inveniosoftware/repository-cli
 Author: Graz University of Technology
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio repository cli
 Platform: any
@@ -52,14 +52,23 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.7.0 (release 2023-05-30)
+
+- test: fix and pin due flask-babelex
+- records: separate replace-file from add-file
+- fix: black color on black background, bad
+- types: otherwise it is not working with 3.9
+- global: migrate to ruff
+
+
 Version v0.6.0 (release 2023-05-01)
 
 - cli: add command publish
 - cli: add record_id parameter to modify-access
 
 
 Version v0.5.0 (release 2023-03-08)
```

### Comparing `repository-cli-0.6.0/README.rst` & `repository-cli-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.6.0/docs/Makefile` & `repository-cli-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repository-cli-0.6.0/docs/api.rst` & `repository-cli-0.7.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.6.0/docs/conf.py` & `repository-cli-0.7.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -332,8 +332,14 @@
 nitpick_ignore = [
     ("py:class", "flask_principal.Identity"),
     ("py:class", "invenio_drafts_resources.records.api.Draft"),
     ("py:class", "invenio_drafts_resources.records.api.Record"),
     ("py:class", "invenio_rdm_records.services.services.RDMRecordService"),
     ("py:class", "invenio_records_resources.services.records.service.RecordService"),
     ("py:class", "sqlalchemy.orm.decl_api.Model"),
+    ("py:class", "flask.app.Flask"),
+    ("py:class", "RecordService"),
+    ("py:class", "Identity"),
+    ("py:class", "Draft"),
+    ("py:class", "db.Model"),
+    ("py:class", "Record"),
 ]
```

### Comparing `repository-cli-0.6.0/docs/index.rst` & `repository-cli-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.6.0/docs/make.bat` & `repository-cli-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `repository-cli-0.6.0/repository_cli/cli.py` & `repository-cli-0.7.0/repository_cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # Copyright (C) 2021-2023 Graz University of Technology.
 #
 # repository-cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """CLI commands for repository-cli."""
 
-import click
+from click import group
 
 from .records import group_records
 from .users import group_users
 
 
-@click.group()
-def utilities():
+@group()
+def utilities() -> None:
     """Utility commands for TU Graz Repository."""
 
 
 utilities.add_command(group_users)
 utilities.add_command(group_records)
```

### Comparing `repository-cli-0.6.0/repository_cli/click_options.py` & `repository-cli-0.7.0/repository_cli/click_options.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,143 +4,158 @@
 #
 # repository-cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Commonly used options for CLI commands."""
 
 
-import click
+from collections.abc import Callable
+from typing import Any, TypeVar
 
+from click import BOOL, STRING, Choice, File, option
 
-def optional_brackets(func):
+T = TypeVar("T")
+
+
+def optional_brackets(func: Callable) -> Callable:
     """With this decorator it is possible to write decorators without ()."""
 
-    def wrapper(*args, **kwargs):
+    def wrapper(*args: dict, **kwargs: dict) -> Any:  # noqa: ANN401
         if len(args) >= 1 and callable(args[0]):
             return func()(args[0])
         return func(*args, **kwargs)
 
     return wrapper
 
 
 @optional_brackets
-def option_quiet():
+def option_quiet() -> Callable[[T], T]:
     """Get parameter option for quiet."""
-    return click.option(
+    return option(
         "--quiet",
         is_flag=True,
         default=False,
-        type=click.BOOL,
+        type=BOOL,
     )
 
 
 @optional_brackets
-def option_jq_filter():
+def option_jq_filter() -> Callable[[T], T]:
     """Get parameter option for jq filter."""
-    return click.option(
+    return option(
         "--jq-filter",
         default=".",
-        type=click.STRING,
+        type=STRING,
         required=False,
         help="filter for jq",
     )
 
 
 @optional_brackets
-def option_data_model():
+def option_data_model() -> Callable[[T], T]:
     """Get parameter option for data model."""
-    return click.option(
+    return option(
         "--data-model",
-        type=click.Choice(["rdm", "marc21"]),
+        type=Choice(["rdm", "marc21"]),
         default="rdm",
     )
 
 
 @optional_brackets
-def option_record_type():
+def option_record_type() -> Callable[[T], T]:
     """Get parameter option for record type."""
-    return click.option(
+    return option(
         "--record-type",
-        type=click.Choice(["record", "draft"], case_sensitive=True),
+        type=Choice(["record", "draft"], case_sensitive=True),
         default="record",
     )
 
 
 @optional_brackets
-def option_identifier(required: bool = True):
+def option_identifier(
+    required: bool = True,  # noqa: FBT001, FBT002
+) -> Callable[[T], T]:
     """Get parameter options for metadata identifier.
 
     Sample use: --identifier '{ "identifier": "10.48436/fcze8-4vx33", "scheme": "doi"}'
     """
-    return click.option(
+    return option(
         "--identifier",
         "-i",
         required=required,
         help="metadata identifier as JSON",
     )
 
 
 # TODO. rename to option_pid
 @optional_brackets
-def option_pid_identifier(required: bool = True):
+def option_pid_identifier(
+    required: bool = True,  # noqa: FBT001, FBT002
+) -> Callable[[T], T]:
     """Get parameter options for metadata identifier.
 
     Sample use: --pid-identifier '{"doi": {"identifier": "10.48436/fcze8-4vx33",
                                            "provider": "unmanaged"}}'
     """
-    return click.option(
+    return option(
         "--pid-identifier",
         required=required,
         help="pid identifier as JSON",
     )
 
 
 # TODO: rename to option_id, refactore to true concept of the used id
 @optional_brackets
-def option_pid(required: bool = True):
+def option_pid(
+    required: bool = True,  # noqa: FBT001, FBT002
+) -> Callable[[T], T]:
     """Get parameter options for record PID.
 
     Sample use: --pid "fcze8-4vx33"
     """
-    return click.option(
+    return option(
         "--pid",
         "-p",
         metavar="PID_VALUE",
         required=required,
         help="persistent identifier of the object to operate on",
     )
 
 
 @optional_brackets
 def option_input_file(
-    required: bool = True,
-    type_=click.File("r"),
-    name="input_file",
-    help_="name of file to read from",
-):
+    required: bool = True,  # noqa: FBT001, FBT002
+    type_: File = None,
+    name: str = "input_file",
+    help_: str = "name of file to read from",
+) -> Callable[[T], T]:
     """Get parameter options for input file.
 
     Sample use: --input-file "input.json"
     """
-    return click.option(
+    if not type_:
+        type_ = File("r")
+    return option(
         "--input-file",
         name,
         metavar="string",
         required=required,
         help=help_,
         type=type_,
     )
 
 
 @optional_brackets
-def option_output_file(required: bool = True):
+def option_output_file(
+    required: bool = True,  # noqa: FBT001, FBT002
+) -> Callable[[T], T]:
     """Get parameter options for output file.
 
     Sample use: --output-file "output.json"
     """
-    return click.option(
+    return option(
         "--output-file",
         metavar="string",
         required=required,
         help="name of file to write to",
-        type=click.File("w"),
+        type=File("w"),
     )
```

### Comparing `repository-cli-0.6.0/repository_cli/click_param_types.py` & `repository-cli-0.7.0/repository_cli/click_param_types.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,33 +6,40 @@
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Commonly used param types for CLI commands."""
 
 
 import sys
 from json import JSONDecodeError, load
-from os.path import isfile
+from pathlib import Path
+from typing import Any, Optional
 
-from click import ParamType, secho
+from click import Context, Parameter, ParamType, secho
 
 from .types import Color
 
 
 class JSON(ParamType):
     """JSON provides the ability to load a json from a string or a file."""
 
     name = "JSON"
 
-    def convert(self, value, param, ctx):
-        """This method converts the json-file to the dictionary representation."""
-        if not isfile(value):
+    def convert(
+        self,
+        value: Any,  # noqa: ANN401
+        param: Optional["Parameter"],  # noqa: ARG002
+        ctx: Optional["Context"],  # noqa: ARG002
+    ) -> Any:  # noqa: ANN401
+        """The method converts the json-file to the dictionary representation."""
+        if not Path(value).is_file():
             secho("ERROR - please look up if the file path is correct.", fg=Color.error)
             sys.exit()
 
         try:
-            with open(value, "r", encoding="utf8") as file_pointer:
+            with Path(value).open("r", encoding="utf8") as file_pointer:
                 obj = load(file_pointer)
-            return obj
         except JSONDecodeError as error:
             secho("ERROR - Invalid JSON provided.", fg=Color.error)
             secho(f"  error: {error.args[0]}", fg=Color.error)
             sys.exit()
+        else:
+            return obj
```

### Comparing `repository-cli-0.6.0/repository_cli/ext.py` & `repository-cli-0.7.0/repository_cli/ext.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 # Copyright (C) 2021-2023 Graz University of Technology.
 #
 # repository-cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """CLI utilities for TU Graz Repository."""
 
+from flask import Flask
+
 
 class RepositoryCli:
     """repository-cli extension."""
 
-    def __init__(self, app=None):
+    def __init__(self, app: Flask = None) -> None:
         """Extension initialization."""
         if app:
             self.init_app(app)
 
-    def init_app(self, app):
+    def init_app(self, app: Flask) -> None:
         """Flask application initialization."""
         app.extensions["repository-cli"] = self
```

### Comparing `repository-cli-0.6.0/repository_cli/records.py` & `repository-cli-0.7.0/repository_cli/records.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 #
 # repository-cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Management commands for records."""
 
 import json
-import os
 from copy import deepcopy
-from io import SEEK_END, SEEK_SET
+from pathlib import Path
 from typing import TextIO
 
-import click
 import jq
-from click import secho
+from click import STRING, Choice, File, group, option, secho
 from flask.cli import with_appcontext
 from invenio_db import db
 from invenio_pidstore.errors import PIDDoesNotExistError
 
 from .click_options import (
     option_data_model,
     option_identifier,
@@ -41,24 +39,24 @@
     get_metadata_model,
     get_record_or_draft,
     get_records_service,
     update_record,
 )
 
 
-@click.group("records")
-def group_records():
+@group("records")
+def group_records() -> None:
     """Management commands for records."""
 
 
 @group_records.command("count")
 @option_data_model
 @option_record_type
 @with_appcontext
-def count_records(data_model, record_type):
+def count_records(data_model: str, record_type: str) -> None:
     """Count number of record's.
 
     example call:
         invenio repository records count
     """
     model = get_metadata_model(data_model, record_type)
     records = model.query.filter_by(is_deleted=False)
@@ -70,16 +68,20 @@
 @option_output_file(required=False)
 @option_data_model
 @option_quiet
 @option_jq_filter
 @option_record_type
 @with_appcontext
 def list_records(
-    output_file: TextIO, data_model: str, quiet: bool, jq_filter: str, record_type: str
-):
+    output_file: TextIO,
+    data_model: str,
+    quiet: bool,  # noqa: FBT001
+    jq_filter: str,
+    record_type: str,
+) -> None:
     """List record's.
 
     example call:
         invenio repository records list [--output-file out.json]
         invenio repository records list --record-type draft \
                                            --data-model marc21 \
                                            --output-file /dev/stdout \
@@ -123,15 +125,15 @@
         secho(output_msg, fg=Color.success)
 
 
 @group_records.command("update")
 @option_input_file(type_=JSON(), name="records")
 @option_data_model
 @with_appcontext
-def update_records(records: list, data_model):
+def update_records(records: list, data_model: str) -> None:
     """Update records specified in input file.
 
     example call:
         invenio repository records update --input-file in.json
 
     Description:
       the record could be replaced completelly by the given json
@@ -163,15 +165,15 @@
         secho(f"'{pid}', successfully updated", fg=Color.success)
 
 
 @group_records.command("add-metadata")
 @option_input_file(type_=JSON(), name="records")
 @option_data_model
 @with_appcontext
-def add_metadata_to_records(records: list, data_model):
+def add_metadata_to_records(records: list, data_model: str) -> None:
     """Add metadata to records.
 
     example call:
         invenio repository records update --input-file in.json [--data-model marc21]
 
     Description:
       file should look like:
@@ -197,17 +199,16 @@
         except RuntimeError as error:
             secho(str(error), fg=Color.error)
             continue
 
         if data_model == "marc21":
             new_data = add_metadata_to_marc21_record(deepcopy(old_data), record)
         else:
-            raise RuntimeError(
-                "Only marc21 is implemented for adding metadata to record."
-            )
+            msg = "Only marc21 is implemented for adding metadata to record."
+            raise RuntimeError(msg)
 
         try:
             update_record(service, pid, identity, new_data, old_data)
         except Exception as error:
             secho(
                 f"'{pid}', an error occured on updating the record, {error}",
                 fg=Color.error,
@@ -216,15 +217,15 @@
 
         secho(f"'{pid}', successfully updated", fg=Color.success)
 
 
 @group_records.command("delete")
 @option_pid
 @with_appcontext
-def delete_record(pid: str):
+def delete_record(pid: str) -> None:
     """Delete record.
 
     example call:
         invenio repository records delete -p "fcze8-4vx33"
     """
     service = get_records_service()
     identity = get_identity(permission_name="system_process", role_name="admin")
@@ -236,15 +237,15 @@
     service.delete(id_=pid, identity=identity)
     secho(f"'{pid}', soft-deleted", fg=Color.success)
 
 
 @group_records.command("delete-draft")
 @option_pid
 @with_appcontext
-def delete_draft(pid: str):
+def delete_draft(pid: str) -> None:
     """Delete draft.
 
     example call:
         invenio repository records delete-draft -p "fcze8-4vx33"
     """
     service = get_records_service()
     identity = get_identity(permission_name="system_process", role_name="admin")
@@ -259,22 +260,22 @@
         return
 
     service.delete_draft(id_=pid, identity=identity)
     secho(f"'{pid}', deleted draft", fg=Color.success)
 
 
 @group_records.group("pids")
-def group_pids():
+def group_pids() -> None:
     """Management commands for record pids."""
 
 
 @group_pids.command("list")
 @option_pid
 @with_appcontext
-def list_pids(pid: str):
+def list_pids(pid: str) -> None:
     """List record's pids.
 
     example call:
         invenio repository records pids list -p <pid>
     """
     service = get_records_service()
     identity = get_identity()
@@ -293,15 +294,15 @@
         secho(json.dumps(current_pid, indent=2), fg=Color.alternate[index % 2])
 
 
 @group_pids.command("replace")
 @option_pid
 @option_pid_identifier
 @with_appcontext
-def replace_pid(pid: str, pid_identifier: str):
+def replace_pid(pid: str, pid_identifier: str) -> None:
     """Update pid doi to unmanaged.
 
     example call:
         invenio repository records pids replace -p "fcze8-4vx33"
         --pid-identifier ' { "doi": {
         "identifier": "10.48436/fcze8-4vx33", "provider": "unmanaged" }}'
     """
@@ -337,22 +338,22 @@
         secho(f"'{pid}', problem during update, {error}", fg=Color.error)
         return
 
     secho(f"'{pid}', successfully updated", fg=Color.success)
 
 
 @group_records.group("identifiers")
-def group_identifiers():
+def group_identifiers() -> None:
     """Management commands for record identifiers."""
 
 
 @group_identifiers.command("list")
 @option_pid
 @with_appcontext
-def list_identifiers(pid: str):
+def list_identifiers(pid: str) -> None:
     """List record's identifiers.
 
     example call:
         invenio repository records identifiers list -p <pid>
     """
     service = get_records_service()
     identity = get_identity()
@@ -371,15 +372,15 @@
         secho(json.dumps(identifier, indent=2), fg=Color.alternate[index % 2])
 
 
 @group_identifiers.command("add")
 @option_identifier
 @option_pid
 @with_appcontext
-def add_identifier(identifier: str, pid: str):
+def add_identifier(identifier: str, pid: str) -> None:
     """Update the specified record's identifiers.
 
     example call:
         invenio repository records identifiers add -p "fcze8-4vx33"
         -i '{ "identifier": "10.48436/fcze8-4vx33", "scheme": "doi"}'
     """
     try:
@@ -419,15 +420,15 @@
     return
 
 
 @group_identifiers.command("replace")
 @option_identifier
 @option_pid
 @with_appcontext
-def replace_identifier(identifier: str, pid: str):
+def replace_identifier(identifier: str, pid: str) -> None:
     """Update the specified record's identifiers.
 
     example call:
         invenio repository records identifiers replace -p "fcze8-4vx33"
         -i '{ "identifier": "10.48436/fcze8-4vx33", "scheme": "doi"}'
     """
     try:
@@ -466,111 +467,140 @@
     except Exception as error:
         secho(f"'{pid}', problem during update, {error}", fg=Color.error)
         return
 
     secho(f"Identifier for '{pid}' replaced.", fg=Color.success)
 
 
-@group_records.command("add-file")
-@option_pid
+@group_records.command("replace-file")
 @option_data_model
-@option_input_file(type_=click.File("rb"))
-@click.option("--replace-existing", "-f", is_flag=True, default=False)
-@click.option("--enable-files", is_flag=True, default=False)
+@option_pid
+@option_input_file(type_=File("rb"))
+@option("--override-name-match-check", is_flag=True, default=False)
 @with_appcontext
-def add_file(pid, input_file, replace_existing, data_model, enable_files):
-    """Add a new file to a published record."""
+def replace_file(
+    data_model: str,
+    pid: str,
+    input_file: File,
+    override_name_match_check: bool,  # noqa: FBT001
+) -> None:
+    """Replace the file."""
     identity = get_identity("system_process", role_name="admin")
     service = get_records_service(data_model=data_model)
 
     try:
-        # pylint: disable=protected-access
-        record = service.read(identity=identity, id_=pid)._record
+        record = service.read(identity=identity, id_=pid)._record  # noqa: SLF001
     except PIDDoesNotExistError as error:
-        secho(
-            f"Record with type '{error.pid_type}' and id '{error.pid_value}' does not exist.",
-            fg=Color.error,
-        )
+        msg = f"Record id '{error.pid_value} ({data_model})' does not exist."
+        secho(msg, fg=Color.error)
         return
 
     files = record.files
-    bucket = files.bucket
-
-    filename = os.path.basename(input_file.name)
+    filename = Path(input_file.name).name  # Path().name gets the filename only
     obj = None
+
     try:
         obj = files[filename]
     except KeyError:
-        secho("File does not yet exist.", fg=Color.neutral)
+        if override_name_match_check and len(files) == 1:
+            filename = list(files)[0]
+            obj = files[filename]
+        elif len(files) > 1:
+            msg = "There is more than 1 file and no matching found, specify filename."
+            secho(msg, fg=Color.error)
+            return
+        else:
+            secho(
+                "There is only one file but the filename does not match, "
+                "maybe use parameter --override-name-match-check.",
+                fg=Color.error,
+            )
+            return
 
-    if obj is not None and not replace_existing:
-        secho(
-            f"Use --replace-existing to overwrite existing {filename} file",
-            fg=Color.error,
-        )
+    files.unlock()
+    files.delete(obj.key)
+    files.create(filename, stream=input_file)
+    files.lock()
+
+    record.commit()
+    db.session.commit()
+    secho("File replaced successfully.", fg=Color.success)
+
+
+@group_records.command("add-file")
+@option_pid
+@option_data_model
+@option_input_file(type_=File("rb"))
+@option("--enable-files", is_flag=True, default=False)
+@with_appcontext
+def add_file(
+    pid: str,
+    input_file: File,
+    data_model: str,
+    enable_files: bool,  # noqa: FBT001
+) -> None:
+    """Add a new file to a published record."""
+    identity = get_identity("system_process", role_name="admin")
+    service = get_records_service(data_model=data_model)
+
+    try:
+        record = service.read(identity=identity, id_=pid)._record  # noqa: SLF001
+    except PIDDoesNotExistError as error:
+        msg = f"Record id '{error.pid_value} ({data_model})' does not exist."
+        secho(msg, fg=Color.error)
         return
 
+    files = record.files
+    filename = Path(input_file.name).name
+
+    if files.enabled:
+        obj = files.get(filename, None)
+        if obj is not None:
+            secho(
+                "File already exists if you want to replace use argument replace-file",
+                fg=Color.neutral,
+            )
+            return
+
     if not files.enabled and not enable_files:
         secho(
             "Use --enable-files to add files to (metadata-only) record",
             fg=Color.error,
         )
         return
 
-    input_file.seek(SEEK_SET, SEEK_END)
-    size = input_file.tell()
-    input_file.seek(SEEK_SET)
-
-    title = record.get("metadata", {}).get("title")
-    messages = {
-        "Will add the following file:": Color.neutral,
-        f"  filename: {filename}\n  bucket: {bucket}\n  size: {size}": Color.success,
-        "to record:": Color.neutral,
-        f"  Title: {title}\n  ID: {record['id']}\n  UUID: {record.id}": Color.success,
-    }
-
-    for message, color in messages.items():
-        secho(message, fg=color)
-
-    if replace_existing and obj is not None:
-        secho("and remove the file:\n", fg=Color.neutral)
-        secho(
-            f"  filename: {obj.key}\n  bucket: {bucket}\n  size: {obj.file.size}",
-            fg=Color.success,
-        )
-
-    if click.confirm("Continue?"):
-        files.enabled = True  # this allows to also add files to metadata only records
-        files.unlock()
-        if obj is not None and replace_existing:
-            files.delete(obj.key)
-        files.create(filename, stream=input_file)
-        files.lock()
-
-        record.commit()
-        db.session.commit()  # pylint: disable=no-member
-        secho("File added successfully.", fg=Color.success)
-    else:
-        secho("File addition aborted.", fg=Color.abort)
+    files.enabled = True  # this allows to also add files to metadata only records
+    files.unlock()
+    files.create(filename, stream=input_file)
+    files.lock()
+
+    record.commit()
+    db.session.commit()
+    secho("File added successfully.", fg=Color.success)
 
 
 @group_records.command("modify-access")
 @option_data_model
 @option_input_file(
-    type_=JSON(), name="record_ids", help_="json array of ids", required=False
-)
-@click.option("--record-id", type=click.STRING)
-@click.option(
-    "--access-record", default=None, type=click.Choice(["public", "restricted"])
+    type_=JSON(),
+    name="record_ids",
+    help_="json array of ids",
+    required=False,
 )
-@click.option(
-    "--access-file", default=None, type=click.Choice(["public", "restricted"])
-)
-@with_appcontext
-def modify_access(data_model, record_ids, record_id, access_record, access_file):
+@option("--record-id", type=STRING)
+@option("--access-record", default=None, type=Choice(["public", "restricted"]))
+@option("--access-file", default=None, type=Choice(["public", "restricted"]))
+@with_appcontext
+def modify_access(
+    data_model: str,
+    record_ids: list,
+    record_id: str,
+    access_record: str,
+    access_file: str,
+) -> None:
     """Modify the access object within the record."""
     identity = get_identity("system_process", role_name="admin")
     service = get_records_service(data_model=data_model)
 
     if not record_ids and record_id:
         record_ids = [record_id]
 
@@ -586,19 +616,22 @@
         service.update_draft(id_=rec_id, identity=identity, data=data)
         service.publish(id_=rec_id, identity=identity)
 
 
 @group_records.command("publish")
 @option_data_model
 @option_input_file(
-    type_=JSON(), name="record_ids", help_="json array of ids", required=False
+    type_=JSON(),
+    name="record_ids",
+    help_="json array of ids",
+    required=False,
 )
-@click.option("--record-id", type=click.STRING)
+@option("--record-id", type=STRING)
 @with_appcontext
-def publish(data_model, record_ids, record_id):
+def publish(data_model: str, record_ids: list, record_id: str) -> None:
     """Publish all records."""
     identity = get_identity("system_process", role_name="admin")
     service = get_records_service(data_model=data_model)
 
     if not record_ids and record_id:
         record_ids = [record_id]
```

### Comparing `repository-cli-0.6.0/repository_cli/users.py` & `repository-cli-0.7.0/repository_cli/users.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 # Copyright (C) 2021-2023 Graz University of Technology.
 #
 # repository-cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Management commands for users."""
 
-import click
+from click import group
 from flask.cli import with_appcontext
 from invenio_accounts.models import User
 from tabulate import tabulate
 
 
-@click.group("users")
-def group_users():
+@group("users")
+def group_users() -> None:
     """Management commands for users."""
 
 
 @group_users.command("list")
 @with_appcontext
-def list_users():
+def list_users() -> None:
     """List registered users.
 
     example call:
         invenio repository users list
     """
     users = []
 
     for user in User.query:
         active = "YES" if user.active else "NO"
 
         users.append([user.id, user.email, active, user.confirmed_at])
 
-    print(tabulate(users, headers=["id", "email", "active", "confirmed"]))
+    print(tabulate(users, headers=["id", "email", "active", "confirmed"]))  # noqa: T201
```

### Comparing `repository-cli-0.6.0/repository_cli/utils.py` & `repository-cli-0.7.0/repository_cli/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,44 @@
 #
 # Copyright (C) 2021-2023 Graz University of Technology.
 #
 # repository-cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Commonly used utility functions."""
-from typing import Optional, Union
+from __future__ import annotations
+
+from contextlib import suppress
+from typing import TYPE_CHECKING
 
 from flask_principal import Identity, RoleNeed
 from invenio_access.permissions import any_user, system_process
 from invenio_accounts import current_accounts
-from invenio_db import db
-from invenio_drafts_resources.records.api import Draft, Record
 from invenio_rdm_records.proxies import current_rdm_records
 from invenio_rdm_records.records.models import RDMDraftMetadata, RDMRecordMetadata
 from invenio_records_marc21 import Marc21Metadata, current_records_marc21
 from invenio_records_marc21.records import DraftMetadata as Marc21DraftMetadata
 from invenio_records_marc21.records import RecordMetadata as Marc21RecordMetadata
-from invenio_records_resources.services import RecordService
+
+if TYPE_CHECKING:
+    from invenio_db import db
+    from invenio_drafts_resources.records.api import Draft, Record
+    from invenio_records_resources.services import RecordService
+
+
+BELOW_CONTROLFIELD = 10
+
+
+class IdentityNotFoundError(Exception):
+    """Identity not found exception."""
+
+    def __init__(self, role: str) -> None:
+        """Construct IdentityNotFound."""
+        msg = f"Role {role} does not exist"
+        super().__init__(msg)
 
 
 def get_identity(permission_name: str = "any_user", role_name: str = None) -> Identity:
     """Get an identity to perform tasks.
 
     Default permission is "any_user"
     """
@@ -32,63 +49,65 @@
         permission = system_process
 
     if role_name:
         role = current_accounts.datastore.find_role(role_name)
         if role:
             identity.provides.add(RoleNeed(role_name))
         else:
-            raise Exception(f"Role {role_name} does not exist")
+            raise IdentityNotFoundError(role=role_name)
 
     identity.provides.add(permission)
     return identity
 
 
-def get_draft(service: RecordService, pid: str, identity: Identity) -> Optional[Draft]:
+def get_draft(service: RecordService, pid: str, identity: Identity) -> Draft | None:
     """Get current draft of record.
 
     None will be returned if there is no draft.
     """
     # check if record exists
     service.read(id_=pid, identity=identity)
 
     draft = None
-    try:
+    with suppress(Exception):
         draft = service.read_draft(id_=pid, identity=identity)
-    except Exception:
-        pass
 
     return draft
 
 
 def get_record_or_draft(
-    service: RecordService, pid: str, identity: Identity
-) -> Union[Draft, Record]:
+    service: RecordService,
+    pid: str,
+    identity: Identity,
+) -> Draft | Record:
     """Get record or draft."""
     try:
         old_data = service.read(id_=pid, identity=identity).data
     except Exception as exc:
         try:
             old_data = service.read_draft(id_=pid, identity=identity).data
         except Exception:
-            raise RuntimeError(f"Record ({pid}) does not exists") from exc
+            msg = f"Record ({pid}) does not exists"
+            raise RuntimeError(msg) from exc
     return old_data
 
 
-def get_records_service(data_model="rdm") -> RecordService:
+def get_records_service(data_model: str = "rdm") -> RecordService:
     """Get records service."""
     available_services = {
         "rdm": current_rdm_records.records_service,
         "marc21": current_records_marc21.records_service,
     }
 
     return available_services.get(data_model, current_rdm_records.records_service)
 
 
 def get_metadata_model(
-    data_model: str = "rdm", record_type: str = "record"
+    data_model: str = "rdm",
+    record_type: str = "record",
 ) -> db.Model:
     """Get the record model."""
     available_models = {
         "record": {
             "rdm": RDMRecordMetadata,
             "marc21": Marc21RecordMetadata,
         },
@@ -108,15 +127,19 @@
         return _type.get(data_model)
     except KeyError as exc:
         msg = "the used data_model should be of the list [rdm, marc21]"
         raise RuntimeError(msg) from exc
 
 
 def update_record(
-    service: RecordService, pid: str, identity: Identity, new_data: dict, old_data: dict
+    service: RecordService,
+    pid: str,
+    identity: Identity,
+    new_data: dict,
+    old_data: dict,
 ) -> None:
     """Update record with new data.
 
     If there is an error during publishing, the record will be set back
     WARNING: If there is an unpublished draft, the data of it will be lost.
     """
     do_publish = False
@@ -126,23 +149,23 @@
 
     try:
         service.update_draft(id_=pid, identity=identity, data=new_data)
         if do_publish:
             service.publish(id_=pid, identity=identity)
     except Exception as error:
         service.update_draft(id_=pid, identity=identity, data=old_data)
-        raise error
+        raise error  # noqa: TRY201
 
 
 def add_metadata_to_marc21_record(metadata: dict, addition: dict) -> dict:
     """Add fields to marc21 record."""
     marc21 = Marc21Metadata(json=metadata["metadata"])
 
     for field_number, fields in addition["metadata"]["fields"].items():
-        if int(field_number) < 10:
+        if int(field_number) < BELOW_CONTROLFIELD:
             marc21.emplace_controlfield(field_number, fields)
         else:
             for field in fields:
                 selector = f"{field_number}.{field['ind1']}.{field['ind2']}."
                 marc21.emplace_datafield(selector, subfs=field["subfields"])
 
     metadata.update(marc21.json)
```

### Comparing `repository-cli-0.6.0/repository_cli.egg-info/PKG-INFO` & `repository-cli-0.7.0/repository_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-cli
-Version: 0.6.0
+Version: 0.7.0
 Summary: "CLI utilities for TU Graz Repository."
 Home-page: https://github.com/inveniosoftware/repository-cli
 Author: Graz University of Technology
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio repository cli
 Platform: any
@@ -52,14 +52,23 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.7.0 (release 2023-05-30)
+
+- test: fix and pin due flask-babelex
+- records: separate replace-file from add-file
+- fix: black color on black background, bad
+- types: otherwise it is not working with 3.9
+- global: migrate to ruff
+
+
 Version v0.6.0 (release 2023-05-01)
 
 - cli: add command publish
 - cli: add record_id parameter to modify-access
 
 
 Version v0.5.0 (release 2023-03-08)
```

### Comparing `repository-cli-0.6.0/repository_cli.egg-info/SOURCES.txt` & `repository-cli-0.7.0/repository_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .git-blame-ignore-revs
+.ruff.toml
 AUTHORS.rst
 CHANGES.rst
 CONTRIBUTING.rst
 INSTALL.rst
 LICENSE
 MANIFEST.in
 README.rst
```

### Comparing `repository-cli-0.6.0/run-tests.sh` & `repository-cli-0.7.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `repository-cli-0.6.0/setup.cfg` & `repository-cli-0.7.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.9
 zip_safe = False
 install_requires = 
 	click>=7.1.1
-	invenio-rdm-records[opensearch2]>=0.39.2
+	invenio-rdm-records[opensearch2]>=0.39.2,<2.0.0
 	invenio-records-marc21>=0.9
 	jq>=1.4.0
 	tabulate>=0.9.0
 
 [options.extras_require]
 tests = 
 	pytest-invenio>=1.4.0
 	pytest-black>=0.3.0
-	pytest-pylint>=0.18.0
-	pytest-bandit>=0.6.1
+	invenio-i18n<2.0.0 # only because of flask-babelex
 	invenio-app>=1.3.0
 	invenio-search[opensearch2]>=2.1.0
 	invenio-cache>=1.1.1
 	Sphinx>=4.5
 	sphinx-click>=2.5.0
+	ruff>=0.0.270
 
 [options.entry_points]
 flask.commands = 
 	repository = repository_cli.cli:utilities
 invenio_base.apps = 
 	repository_cli = repository_cli:RepositoryCli
 
@@ -48,28 +48,22 @@
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
 
 [bdist_wheel]
 universal = 1
 
-[pydocstyle]
-add_ignore = D401
-
 [tool:isort]
 profile = black
 
 [check-manifest]
 ignore = 
 	*-requirements.txt
 
-[pylint.messages_control]
-disable = fixme, broad-exception-caught, broad-exception-raised, too-few-public-methods, too-many-locals
-
 [tool:pytest]
-addopts = --pylint --bandit --black --isort --pydocstyle --doctest-glob="*.rst" --doctest-modules --cov=repository_cli --cov-report=term-missing
+addopts = --black --doctest-glob="*.rst" --doctest-modules --cov=repository_cli --cov-report=term-missing
 testpaths = tests repository_cli
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `repository-cli-0.6.0/tests/conftest.py` & `repository-cli-0.7.0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,115 +1,125 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 Graz University of Technology.
+# Copyright (C) 2021-2023 Graz University of Technology.
 #
 # repository-cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Pytest configuration.
 
 See https://pytest-invenio.readthedocs.io/ for documentation on which test
 fixtures are available.
 """
 
 import os
 import shutil
+from pathlib import Path
 
 import pytest
 from faker import Faker
+from flask import Flask
 from flask_principal import Identity
 from invenio_access.cli import allow_action
 from invenio_access.permissions import system_identity, system_process
 from invenio_accounts.cli import roles_create
 from invenio_app.factory import create_api as _create_api
 from invenio_db import db
 from invenio_files_rest.models import Location
-from invenio_rdm_records.cli import create_fake_record
+from invenio_rdm_records.fixtures.demo import create_fake_record
 from invenio_rdm_records.proxies import current_rdm_records
+from invenio_records_resources.services.records.results import RecordItem
 from invenio_vocabularies.proxies import current_service as vocabulary_service
 from invenio_vocabularies.records.api import Vocabulary
+from invenio_vocabularies.records.models import VocabularyType
 
 
 @pytest.fixture(scope="module", name="app_config")
-def fixture_app_config(app_config):
+def fixture_app_config(app_config: dict) -> dict:
     """Mimic an instance's configuration."""
     app_config["JSONSCHEMAS_HOST"] = "no-use"
     app_config["BABEL_DEFAULT_LOCALE"] = "en"
     app_config["I18N_LANGUAGES"] = [("en", "English"), ("de", "German")]
     app_config[
         "RECORDS_REFRESOLVER_CLS"
     ] = "invenio_records.resolver.InvenioRefResolver"
     app_config[
         "RECORDS_REFRESOLVER_STORE"
     ] = "invenio_jsonschemas.proxies.current_refresolver_store"
 
     app_config["SQLALCHEMY_DATABASE_URI"] = os.getenv(
-        "SQLALCHEMY_DATABASE_URI", "sqlite://"
+        "SQLALCHEMY_DATABASE_URI",
+        "sqlite://",
     )
     app_config["SQLALCHEMY_TRACK_MODIFICATIONS"] = False
     app_config["DATADIR"] = "data"
 
     return app_config
 
 
 @pytest.fixture(scope="module")
-def create_app():
+def create_app() -> Flask:
     """Application factory fixture."""
     return _create_api
 
 
 @pytest.fixture(scope="module", name="app_initialized")
-def fixture_app_initialized(app, resource_type_item):  # pylint: disable=unused-argument
+def fixture_app_initialized(
+    app: Flask,
+    resource_type_item: str,  # noqa: ARG001
+) -> Flask:
     """Flask application with data added."""
     datadir = app.config["DATADIR"]
-    if os.path.exists(datadir):
+    if Path(datadir).exists():
         shutil.rmtree(datadir)
-        os.makedirs(datadir)
+        Path(datadir).makedir()
 
     loc = Location(name="local", uri=datadir, default=True)
-    db.session.add(loc)  # pylint: disable=no-member
-    db.session.commit()  # pylint: disable=no-member
+    db.session.add(loc)
+    db.session.commit()
 
     runner = app.test_cli_runner()
     runner.invoke(roles_create, ["admin"])
     runner.invoke(allow_action, ["superuser-access", "role", "admin"])
 
     return app
 
 
 @pytest.fixture(name="create_record")
-def fixture_create_record(app_initialized):  # pylint: disable=unused-argument
+def fixture_create_record(app_initialized: Flask) -> RecordItem:  # noqa: ARG001
     """Create and publish new record."""
     record_service = current_rdm_records.records_service
     identity = Identity(1)
     identity.provides.add(system_process)
 
     record_json = minimal_record()
     record_json["metadata"]["identifiers"] = [
-        {"identifier": "ark:/123/456", "scheme": "ark"}
+        {"identifier": "ark:/123/456", "scheme": "ark"},
     ]
 
     rec = record_service.create(data=record_json, identity=identity)
     record_service.publish(id_=rec.id, identity=identity)
 
     return rec
 
 
 @pytest.fixture()
-def create_draft(app_initialized, create_record):  # pylint: disable=unused-argument
+def create_draft(
+    app_initialized: Flask,  # noqa: ARG001
+    create_record: RecordItem,
+) -> RecordItem:
     """Create draft for record."""
     record_service = current_rdm_records.records_service
     identity = Identity(1)
     identity.provides.add(system_process)
 
-    draft = record_service.edit(id_=create_record.id, identity=identity)
-    return draft
+    return record_service.edit(id_=create_record.id, identity=identity)
 
 
-def minimal_record():
+def minimal_record() -> dict:
     """Minimal record data as dict coming from the external world.
 
     https://github.com/inveniosoftware/invenio-rdm-records/blob/aa575a4f8b1beb4d24a448067b649d6f0b8c085e/tests/conftest.py#L279
     """
     return {
         "pids": {},
         "access": {
@@ -124,67 +134,68 @@
             "resource_type": {"id": "image-photo"},
             "creators": [
                 {
                     "person_or_org": {
                         "family_name": "Brown",
                         "given_name": "Troy",
                         "type": "personal",
-                    }
+                    },
                 },
                 {
                     "person_or_org": {
                         "name": "Troy Inc.",
                         "type": "organizational",
                     },
                 },
             ],
             "title": "A Romans story",
         },
     }
 
 
-def fake_record():
+def fake_record() -> dict:
     """Create fake record and replace date.
 
     As date ranges (e.g. 1968-08-20/2020-11) don't work yet.
     """
     record_json = create_fake_record()
     fake = Faker()
     date_pattern = ["%Y", "%m", "%d"]
     new_date = fake.date("-".join(date_pattern))
     record_json["metadata"]["publication_date"] = new_date
 
     return record_json
 
 
 @pytest.fixture()
-def identifier():
+def identifier() -> dict:
     """Create identifier for test cases."""
     return {"identifier": "10.48436/fcze8-4vx33", "scheme": "doi"}
 
 
 @pytest.fixture()
-def pid_identifier():
+def pid_identifier() -> dict:
     """Create pid identifier for test cases."""
     return {"doi": {"identifier": "10.48436/fcze8-4vx33", "provider": "unmanaged"}}
 
 
 @pytest.fixture(scope="module", name="resource_type_type")
-def fixture_resource_type_type(app):  # pylint: disable=unused-argument
+def fixture_resource_type_type(app: Flask) -> VocabularyType:  # noqa: ARG001
     """Resource type vocabulary type.
 
     https://github.com/inveniosoftware/invenio-rdm-records/blob/aa575a4f8b1beb4d24a448067b649d6f0b8c085e/tests/conftest.py#L398
     """
     return vocabulary_service.create_type(system_identity, "resourcetypes", "rsrct")
 
 
 @pytest.fixture(scope="module", name="resource_type_item")
 def fixture_resource_type_item(
-    app, resource_type_type
-):  # pylint: disable=unused-argument
+    app: Flask,  # noqa: ARG001
+    resource_type_type: str,  # noqa: ARG001
+) -> VocabularyType:
     """Resource type vocabulary record.
 
     https://github.com/inveniosoftware/invenio-rdm-records/blob/aa575a4f8b1beb4d24a448067b649d6f0b8c085e/tests/conftest.py#L405
     """
     vocab = vocabulary_service.create(
         system_identity,
         {
```

### Comparing `repository-cli-0.6.0/tests/test_rdmrecords.py` & `repository-cli-0.7.0/tests/test_rdmrecords.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,124 +7,130 @@
 
 """Pytest configuration.
 
 See https://pytest-invenio.readthedocs.io/ for documentation on which test
 fixtures are available.
 """
 
-import os
+from pathlib import Path
+
+from flask import Flask
+from invenio_records_resources.services.records.results import RecordItem
 
 from repository_cli.records import (
     count_records,
     delete_draft,
     delete_record,
     group_records,
     list_records,
     update_records,
 )
 
 
-def test_base_command(app):
+def test_base_command(app: Flask) -> None:
     """Test base command."""
     runner = app.test_cli_runner()
     response = runner.invoke(group_records)
     assert response.exit_code == 0
 
 
 def test_count_with_entries(
-    app_initialized,
-    create_record,  # pylint: disable=unused-argument
-):
+    app_initialized: Flask,
+    create_record: RecordItem,  # noqa: ARG001
+) -> None:
     """Test count with entries."""
     runner = app_initialized.test_cli_runner()
     response = runner.invoke(count_records)
     assert response.exit_code == 0
     assert "0 records" not in response.output
 
 
-def test_list_with_entries(app_initialized, create_record):
+def test_list_with_entries(app_initialized: Flask, create_record: RecordItem) -> None:
     """Test list with entries."""
     runner = app_initialized.test_cli_runner()
     record = create_record
     r_id = record.id
     title = record.data["metadata"]["title"]
     response = runner.invoke(list_records)
     assert response.exit_code == 0
     assert "0 records" not in response.output
     assert f"{ r_id }" in response.output
     assert f"{ title }" in response.output
 
 
-def test_list_output_file(app_initialized):
+def test_list_output_file(app_initialized: Flask) -> None:
     """Test list output file."""
     filename = "out.json"
     runner = app_initialized.test_cli_runner()
     response = runner.invoke(list_records, ["--output-file", filename])
-    os.remove(filename)
+    Path(filename).unlink()
     assert response.exit_code == 0
     assert "0 records" not in response.output
     assert f"records to {filename}" in response.output
 
 
-def test_update(app_initialized):
+def test_update(app_initialized: Flask) -> None:
     """Test update."""
     filename = "out.json"
     runner = app_initialized.test_cli_runner()
     response = runner.invoke(list_records, ["--output-file", filename])
     assert response.exit_code == 0
     assert f"records to {filename}" in response.output
 
     response = runner.invoke(update_records, ["--input-file", filename])
-    os.remove(filename)
+    Path(filename).unlink()
     assert response.exit_code == 0
     assert "successfully updated" in response.output
 
 
-def test_update_ill_formatted_file(app_initialized):
+def test_update_ill_formatted_file(app_initialized: Flask) -> None:
     """Test update ill formatted file."""
     filename = "out.json"
-    with open(filename, mode="w", encoding="utf8") as file_pointer:
+    with Path(filename).open(mode="w", encoding="utf8") as file_pointer:
         file_pointer.write("not a valid JSON representation")
 
     runner = app_initialized.test_cli_runner()
     response = runner.invoke(update_records, ["--input-file", filename])
 
-    os.remove(filename)
+    Path(filename).unlink()
 
     assert response.exit_code == 0
     assert "ERROR - Invalid JSON provided." in response.output
 
 
-def test_delete(app_initialized, create_record):
+def test_delete(app_initialized: Flask, create_record: RecordItem) -> None:
     """Test delete."""
     r_id = create_record.id
     runner = app_initialized.test_cli_runner()
     response = runner.invoke(delete_record, ["--pid", r_id])
     assert response.exit_code == 0
     assert f"'{r_id}', soft-deleted" in response.output
 
 
-def test_delete_draft_success(app_initialized, create_draft):
+def test_delete_draft_success(app_initialized: Flask, create_draft: RecordItem) -> None:
     """Test delete draft success."""
     r_id = create_draft.id
     runner = app_initialized.test_cli_runner()
     response = runner.invoke(delete_draft, ["--pid", r_id])
     assert response.exit_code == 0
     assert f"'{r_id}', deleted draft" in response.output
 
 
-def test_delete_draft_no_draft(app_initialized, create_record):
+def test_delete_draft_no_draft(
+    app_initialized: Flask,
+    create_record: RecordItem,
+) -> None:
     """Test delete draft no draft."""
     r_id = create_record.id
     runner = app_initialized.test_cli_runner()
     response = runner.invoke(delete_draft, ["--pid", r_id])
     assert response.exit_code == 0
     assert f"'{r_id}', does not have a draft" in response.output
 
 
-def test_delete_draft_pid_does_not_exist(app_initialized):
+def test_delete_draft_pid_does_not_exist(app_initialized: Flask) -> None:
     """Test delete draft pid does not exist."""
     r_id = "himbeere"
     runner = app_initialized.test_cli_runner()
     response = runner.invoke(delete_draft, ["--pid", r_id])
     assert response.exit_code == 0
     assert f"'{r_id}', does not exist" in response.output
```

### Comparing `repository-cli-0.6.0/tests/test_rdmrecords_identifiers.py` & `repository-cli-0.7.0/tests/test_rdmrecords_identifiers.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,125 +9,155 @@
 
 See https://pytest-invenio.readthedocs.io/ for documentation on which test
 fixtures are available.
 """
 
 import json
 
+from flask import Flask
+from invenio_records_resources.services.records.results import RecordItem
+
 from repository_cli.records import add_identifier, list_identifiers, replace_identifier
 
 
-def test_list_identifiers(app_initialized, create_record):
+def test_list_identifiers(app_initialized: Flask, create_record: RecordItem) -> None:
     """Test list identifiers."""
     runner = app_initialized.test_cli_runner()
     r_id = create_record.id
     response = runner.invoke(list_identifiers, ["--pid", r_id])
     assert response.exit_code == 0
     assert "scheme" in response.output
     assert "identifier" in response.output
 
 
-def test_list_identifiers_record_not_found(app_initialized):
+def test_list_identifiers_record_not_found(app_initialized: Flask) -> None:
     """Test list identifier record not found."""
     runner = app_initialized.test_cli_runner()
     r_id = "this does not exist"
     response = runner.invoke(list_identifiers, ["--pid", r_id])
     assert response.exit_code == 0
     assert "does not exist or is deleted" in response.output
 
 
-def test_add_identifier(app_initialized, identifier, create_record):
+def test_add_identifier(
+    app_initialized: Flask,
+    identifier: dict,
+    create_record: RecordItem,
+) -> None:
     """Test add identifier."""
     runner = app_initialized.test_cli_runner()
     r_id = create_record.id
     response = runner.invoke(
-        add_identifier, ["--pid", r_id, "--identifier", json.dumps(identifier)]
+        add_identifier,
+        ["--pid", r_id, "--identifier", json.dumps(identifier)],
     )
     assert response.exit_code == 0
     assert f"Identifier for '{r_id}' added" in response.output
 
 
-def test_add_identifier_scheme_exists(app_initialized, identifier, create_record):
+def test_add_identifier_scheme_exists(
+    app_initialized: Flask,
+    identifier: dict,
+    create_record: RecordItem,
+) -> None:
     """Test add identifier scheme exists."""
     runner = app_initialized.test_cli_runner()
     r_id = create_record.id
     response = runner.invoke(
-        add_identifier, ["--pid", r_id, "--identifier", json.dumps(identifier)]
+        add_identifier,
+        ["--pid", r_id, "--identifier", json.dumps(identifier)],
     )
     assert response.exit_code == 0
     assert f"Identifier for '{r_id}' added" in response.output
     response = runner.invoke(
-        add_identifier, ["--pid", r_id, "--identifier", json.dumps(identifier)]
+        add_identifier,
+        ["--pid", r_id, "--identifier", json.dumps(identifier)],
     )
     assert response.exit_code == 0
     assert f"scheme '{identifier['scheme']}' already in identifiers" in response.output
 
 
-def test_add_identifier_wrong_identifier_type(app_initialized, create_record):
+def test_add_identifier_wrong_identifier_type(
+    app_initialized: Flask,
+    create_record: RecordItem,
+) -> None:
     """Test add identifier wrong identifier type."""
     runner = app_initialized.test_cli_runner()
     r_id = create_record.id
     response = runner.invoke(
-        add_identifier, ["--pid", r_id, "--identifier", "this is not a dict"]
+        add_identifier,
+        ["--pid", r_id, "--identifier", "this is not a dict"],
     )
     assert response.exit_code == 0
     assert "identifier is not valid JSON" in response.output
 
 
-def test_add_identifiers_record_not_found(app_initialized, identifier):
+def test_add_identifiers_record_not_found(
+    app_initialized: Flask,
+    identifier: dict,
+) -> None:
     """Test add identifiers record not found."""
     runner = app_initialized.test_cli_runner()
     r_id = "this does not exist"
     response = runner.invoke(
-        add_identifier, ["--pid", r_id, "--identifier", json.dumps(identifier)]
+        add_identifier,
+        ["--pid", r_id, "--identifier", json.dumps(identifier)],
     )
     assert response.exit_code == 0
     assert "does not exist or is deleted" in response.output
 
 
-def test_replace_identifier(app_initialized, create_record):
+def test_replace_identifier(app_initialized: Flask, create_record: RecordItem) -> None:
     """Test replace identifier."""
     runner = app_initialized.test_cli_runner()
     r_id = create_record.id
     new_identifier = create_record["metadata"]["identifiers"][0]
     response = runner.invoke(
         replace_identifier,
         ["--pid", r_id, "--identifier", json.dumps(new_identifier)],
     )
     assert response.exit_code == 0
     assert f"Identifier for '{r_id}' replaced" in response.output
 
 
 def test_replace_identifier_scheme_does_not_exist(
-    app_initialized, identifier, create_record
-):
+    app_initialized: Flask,
+    identifier: dict,
+    create_record: RecordItem,
+) -> None:
     """Test replace identifier scheme does not exist."""
     runner = app_initialized.test_cli_runner()
     r_id = create_record.id
     response = runner.invoke(
         replace_identifier,
         ["--pid", r_id, "--identifier", json.dumps(identifier)],
     )
     assert response.exit_code == 0
     assert f"scheme '{identifier['scheme']}' not in identifiers" in response.output
 
 
-def test_replace_identifier_wrong_identifier_type(app_initialized, create_record):
+def test_replace_identifier_wrong_identifier_type(
+    app_initialized: Flask,
+    create_record: RecordItem,
+) -> None:
     """Test replace identifier wrong identifier type."""
     runner = app_initialized.test_cli_runner()
     r_id = create_record.id
     response = runner.invoke(
         replace_identifier,
         ["--pid", r_id, "--identifier", "this is not a dict"],
     )
     assert response.exit_code == 0
     assert "identifier is not valid JSON" in response.output
 
 
-def test_replace_identifiers_record_not_found(app_initialized, identifier):
+def test_replace_identifiers_record_not_found(
+    app_initialized: Flask,
+    identifier: dict,
+) -> None:
     """Test replace identifiers record not found."""
     runner = app_initialized.test_cli_runner()
     r_id = "this does not exist"
     response = runner.invoke(
         replace_identifier,
         ["--pid", r_id, "--identifier", json.dumps(identifier)],
     )
```

### Comparing `repository-cli-0.6.0/tests/test_rdmrecords_pids.py` & `repository-cli-0.7.0/tests/test_rdmrecords_pids.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,75 +9,78 @@
 
 See https://pytest-invenio.readthedocs.io/ for documentation on which test
 fixtures are available.
 """
 
 import json
 
+from flask import Flask
+from invenio_records_resources.services.records.results import RecordItem
+
 from repository_cli.records import list_pids, replace_pid
 
 
-def test_list_pids_with_entries(app_initialized, create_record):
+def test_list_pids_with_entries(
+    app_initialized: Flask,
+    create_record: RecordItem,
+) -> None:
     """Test list pids with entries."""
     runner = app_initialized.test_cli_runner()
     r_id = create_record.id
     response = runner.invoke(list_pids, ["--pid", r_id])
     assert response.exit_code == 0
 
 
-def test_list_pids_record_not_found(app_initialized):
+def test_list_pids_record_not_found(app_initialized: Flask) -> None:
     """Test list pids record not found."""
     runner = app_initialized.test_cli_runner()
     r_id = "this does not exist"
     response = runner.invoke(list_pids, ["--pid", r_id])
     assert response.exit_code == 0
     assert "does not exist or is deleted" in response.output
 
 
-# TODO:
-# this should work, but it does not. It seams that the error is,
-# that the original record does not have a doi.
-# def test_replace_pid(app_initialized, pid_identifier, create_record):
-#     runner = app_initialized.test_cli_runner()
-#     r_id = create_record.id
-#     response = runner.invoke(
-#         replace_pid,
-#         ["--pid", r_id, "--pid-identifier", json.dumps(pid_identifier)],
-#     )
-#     assert response.exit_code == 0
-#     assert f"'{r_id}', successfully updated" in response.output
-
-
-def test_replace_pid_pid_does_not_exist(app_initialized, pid_identifier, create_record):
+def test_replace_pid_pid_does_not_exist(
+    app_initialized: Flask,
+    pid_identifier: dict,
+    create_record: RecordItem,
+) -> None:
     """Test replace pid pid does not exist."""
     runner = app_initialized.test_cli_runner()
     r_id = create_record.id
     pid_identifier["unknown_identifier"] = pid_identifier.pop(
-        list(pid_identifier.keys())[0]
+        list(pid_identifier.keys())[0],
     )
     response = runner.invoke(
         replace_pid,
         ["--pid", r_id, "--pid-identifier", json.dumps(pid_identifier)],
     )
     assert response.exit_code == 0
     assert "does not have pid identifier" in response.output
 
 
-def test_replace_pid_wrong_identifier_type(app_initialized, create_record):
+def test_replace_pid_wrong_identifier_type(
+    app_initialized: Flask,
+    create_record: RecordItem,
+) -> None:
     """Test replace pid wrong identifier type."""
     runner = app_initialized.test_cli_runner()
     r_id = create_record.id
     response = runner.invoke(
-        replace_pid, ["--pid", r_id, "--pid-identifier", "this is not a dict"]
+        replace_pid,
+        ["--pid", r_id, "--pid-identifier", "this is not a dict"],
     )
     assert response.exit_code == 0
     assert "pid_identifier is not valid JSON" in response.output
 
 
-def test_replace_pid_record_not_found(app_initialized, pid_identifier):
+def test_replace_pid_record_not_found(
+    app_initialized: Flask,
+    pid_identifier: dict,
+) -> None:
     """Test replace pid record not found."""
     runner = app_initialized.test_cli_runner()
     r_id = "this does not exist"
     response = runner.invoke(
         replace_pid,
         ["--pid", r_id, "--pid-identifier", json.dumps(pid_identifier)],
     )
```

