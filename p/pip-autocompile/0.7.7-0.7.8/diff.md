# Comparing `tmp/pip_autocompile-0.7.7.tar.gz` & `tmp/pip_autocompile-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_autocompile-0.7.7.tar", max compression
+gzip compressed data, was "pip_autocompile-0.7.8.tar", max compression
```

## Comparing `pip_autocompile-0.7.7.tar` & `pip_autocompile-0.7.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1076 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/LICENSE
--rw-r--r--   0        0        0     1572 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/README.md
--rw-r--r--   0        0        0       33 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/examples/docker/Dockerfile
--rw-r--r--   0        0        0        6 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/examples/docker/requirements/50_base.in
--rw-r--r--   0        0        0       26 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/examples/docker/requirements/60_dev.in
--rw-r--r--   0        0        0       24 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/examples/docker/requirements/61_prod.in
--rw-r--r--   0        0        0      429 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/examples/docker_ssh_agent/Dockerfile
--rw-r--r--   0        0        0       49 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/examples/docker_ssh_agent/requirements/pip-autocompile.in
--rw-r--r--   0        0        0        6 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/examples/requirements.in
--rw-r--r--   0        0        0     1985 2023-03-15 20:42:22.496410 pip_autocompile-0.7.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/src/pipautocompile/__init__.py
--rw-r--r--   0        0        0      379 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/src/pipautocompile/git.py
--rw-r--r--   0        0        0      771 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/src/pipautocompile/io.py
--rw-r--r--   0        0        0      261 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/src/pipautocompile/logging.py
--rw-r--r--   0        0        0     6027 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/src/pipautocompile/main.py
--rw-r--r--   0        0        0        0 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/src/pipautocompile/py.typed
--rw-r--r--   0        0        0      229 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/src/pipautocompile/utils.py
--rw-r--r--   0        0        0        0 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/tests/__init__.py
--rw-r--r--   0        0        0     2533 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/tests/conftest.py
--rw-r--r--   0        0        0     1626 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/tests/test_git.py
--rw-r--r--   0        0        0     4448 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/tests/test_io.py
--rw-r--r--   0        0        0     2400 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/tests/test_logging.py
--rw-r--r--   0        0        0     5104 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/tests/test_main.py
--rw-r--r--   0        0        0     1232 2023-03-15 20:42:21.572393 pip_autocompile-0.7.7/tests/test_utils.py
--rw-r--r--   0        0        0     2819 1970-01-01 00:00:00.000000 pip_autocompile-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/LICENSE
+-rw-r--r--   0        0        0     1572 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/README.md
+-rw-r--r--   0        0        0       33 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/docker/Dockerfile
+-rw-r--r--   0        0        0        6 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/docker/requirements/50_base.in
+-rw-r--r--   0        0        0       26 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/docker/requirements/60_dev.in
+-rw-r--r--   0        0        0       24 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/docker/requirements/61_prod.in
+-rw-r--r--   0        0        0      429 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/docker_ssh_agent/Dockerfile
+-rw-r--r--   0        0        0       49 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/docker_ssh_agent/requirements/pip-autocompile.in
+-rw-r--r--   0        0        0        6 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/requirements.in
+-rw-r--r--   0        0        0     1985 2023-05-30 11:08:15.280207 pip_autocompile-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/__init__.py
+-rw-r--r--   0        0        0      379 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/git.py
+-rw-r--r--   0        0        0      771 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/io.py
+-rw-r--r--   0        0        0      261 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/logging.py
+-rw-r--r--   0        0        0     6027 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/main.py
+-rw-r--r--   0        0        0        0 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/py.typed
+-rw-r--r--   0        0        0      229 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/__init__.py
+-rw-r--r--   0        0        0     2533 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/conftest.py
+-rw-r--r--   0        0        0     1626 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/test_git.py
+-rw-r--r--   0        0        0     4448 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/test_io.py
+-rw-r--r--   0        0        0     2400 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/test_logging.py
+-rw-r--r--   0        0        0     5104 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/test_main.py
+-rw-r--r--   0        0        0     1232 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/test_utils.py
+-rw-r--r--   0        0        0     2819 1970-01-01 00:00:00.000000 pip_autocompile-0.7.8/PKG-INFO
```

### Comparing `pip_autocompile-0.7.7/LICENSE` & `pip_autocompile-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.7/README.md` & `pip_autocompile-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.7/pyproject.toml` & `pip_autocompile-0.7.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pip-autocompile"
-version = "0.7.7"
+version = "0.7.8"
 description = "Automate pip-compile for multiple environments."
 license = "MIT"
 authors = ["Konstantinos Smanis <konstantinos.smanis@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/KSmanis/pip-autocompile"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -24,26 +24,26 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 click = "^8.1.3"
 pygit2 = [
     { version = "~1.10.1", python = "~3.7" },
     { version = "^1.11.1", python = "^3.8" },
 ]
-python-on-whales = "^0.59.0"
+python-on-whales = "^0.60.1"
 
 [tool.poetry.group.lint.dependencies]
 pre-commit = [
     { version = "~2.21.0", python = "~3.7" },
     { version = "^3.0.0", python = "^3.8" },
 ]
-mypy = "^1.1.1"
+mypy = "^1.3.0"
 
 [tool.poetry.group.test.dependencies]
-pip-tools = "^6.12.3"
-pytest-cov = "^4.0.0"
+pip-tools = "^6.13.0"
+pytest-cov = "^4.1.0"
 
 [tool.poetry.scripts]
 pip-autocompile = "pipautocompile.main:cli"
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
```

### Comparing `pip_autocompile-0.7.7/src/pipautocompile/io.py` & `pip_autocompile-0.7.8/src/pipautocompile/io.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.7/src/pipautocompile/main.py` & `pip_autocompile-0.7.8/src/pipautocompile/main.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.7/tests/conftest.py` & `pip_autocompile-0.7.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.7/tests/test_git.py` & `pip_autocompile-0.7.8/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.7/tests/test_io.py` & `pip_autocompile-0.7.8/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.7/tests/test_logging.py` & `pip_autocompile-0.7.8/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.7/tests/test_main.py` & `pip_autocompile-0.7.8/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.7/tests/test_utils.py` & `pip_autocompile-0.7.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.7/PKG-INFO` & `pip_autocompile-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-autocompile
-Version: 0.7.7
+Version: 0.7.8
 Summary: Automate pip-compile for multiple environments.
 Home-page: https://github.com/KSmanis/pip-autocompile
 License: MIT
 Author: Konstantinos Smanis
 Author-email: konstantinos.smanis@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pygit2 (>=1.10.1,<1.11.0) ; python_version >= "3.7" and python_version < "3.8"
 Requires-Dist: pygit2 (>=1.11.1,<2.0.0) ; python_version >= "3.8" and python_version < "4.0"
-Requires-Dist: python-on-whales (>=0.59.0,<0.60.0)
+Requires-Dist: python-on-whales (>=0.60.1,<0.61.0)
 Project-URL: Repository, https://github.com/KSmanis/pip-autocompile
 Description-Content-Type: text/markdown
 
 # pip-autocompile
 
 [![build](https://github.com/KSmanis/pip-autocompile/actions/workflows/build.yml/badge.svg)](https://github.com/KSmanis/pip-autocompile/actions/workflows/build.yml)
 [![PyPI version](https://img.shields.io/pypi/v/pip-autocompile.svg)](https://pypi.org/project/pip-autocompile/)
```

