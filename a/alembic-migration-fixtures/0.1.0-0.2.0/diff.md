# Comparing `tmp/alembic_migration_fixtures-0.1.0.tar.gz` & `tmp/alembic_migration_fixtures-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alembic_migration_fixtures-0.1.0.tar", max compression
+gzip compressed data, was "alembic_migration_fixtures-0.2.0.tar", max compression
```

## Comparing `alembic_migration_fixtures-0.1.0.tar` & `alembic_migration_fixtures-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rwxr-xr-x   0        0        0    11357 2021-07-19 13:06:43.075938 alembic_migration_fixtures-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     3022 2021-07-19 13:06:43.075938 alembic_migration_fixtures-0.1.0/README.md
--rwxr-xr-x   0        0        0        0 2021-07-19 13:06:43.075938 alembic_migration_fixtures-0.1.0/alembic_migration_fixtures/__init__.py
--rwxr-xr-x   0        0        0     3776 2021-07-19 13:06:43.075938 alembic_migration_fixtures-0.1.0/alembic_migration_fixtures/fixtures.py
--rwxr-xr-x   0        0        0      944 2021-07-19 13:06:43.075938 alembic_migration_fixtures-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4087 2021-07-19 13:06:52.077576 alembic_migration_fixtures-0.1.0/setup.py
--rw-r--r--   0        0        0     4030 2021-07-19 13:06:52.077878 alembic_migration_fixtures-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0    11357 2023-05-30 03:37:23.341211 alembic_migration_fixtures-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0     3022 2023-05-30 03:37:23.341211 alembic_migration_fixtures-0.2.0/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-30 03:37:23.341211 alembic_migration_fixtures-0.2.0/alembic_migration_fixtures/__init__.py
+-rwxr-xr-x   0        0        0     3776 2023-05-30 03:37:23.341211 alembic_migration_fixtures-0.2.0/alembic_migration_fixtures/fixtures.py
+-rwxr-xr-x   0        0        0      936 2023-05-30 03:37:23.341211 alembic_migration_fixtures-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 alembic_migration_fixtures-0.2.0/PKG-INFO
```

### Comparing `alembic_migration_fixtures-0.1.0/LICENSE` & `alembic_migration_fixtures-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alembic_migration_fixtures-0.1.0/README.md` & `alembic_migration_fixtures-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alembic_migration_fixtures-0.1.0/alembic_migration_fixtures/fixtures.py` & `alembic_migration_fixtures-0.2.0/alembic_migration_fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `alembic_migration_fixtures-0.1.0/pyproject.toml` & `alembic_migration_fixtures-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alembic_migration_fixtures"
-version = "0.1.0"
+version = "0.2.0"
 description = "Pytest fixtures for tests involving databases managed by alembic migrations"
 
 authors = ["Saulius Beinorius <saulius.beinorius@gmail.com>"]
 maintainers = ["Saulius Beinorius <saulius.beinorius@gmail.com>"]
 
 license = "Apache-2.0"
 readme = "README.md"
@@ -14,20 +14,20 @@
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
-alembic = ">=1.4.2,<1.7"
+alembic = ">=1.4.2,<2"
 pytest = ">=5.2,<7.0"
 SQLAlchemy = ">=1.3.19,<1.5"
 
 [tool.poetry.dev-dependencies]
-black = "^21.7b0"
+black = "*"
 
 [tool.poetry.plugins.pytest11]
 alembic_migration_fixtures = "alembic_migration_fixtures.fixtures"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `alembic_migration_fixtures-0.1.0/PKG-INFO` & `alembic_migration_fixtures-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: alembic-migration-fixtures
-Version: 0.1.0
+Version: 0.2.0
 Summary: Pytest fixtures for tests involving databases managed by alembic migrations
 Home-page: https://github.com/Barbora-Data-Science/alembic-migration-fixtures
 License: Apache-2.0
 Author: Saulius Beinorius
 Author-email: saulius.beinorius@gmail.com
 Maintainer: Saulius Beinorius
 Maintainer-email: saulius.beinorius@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: SQLAlchemy (>=1.3.19,<1.5)
-Requires-Dist: alembic (>=1.4.2,<1.7)
+Requires-Dist: alembic (>=1.4.2,<2)
 Requires-Dist: pytest (>=5.2,<7.0)
 Project-URL: Repository, https://github.com/Barbora-Data-Science/alembic-migration-fixtures
 Description-Content-Type: text/markdown
 
 [![Formatter](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://badge.fury.io/py/alembic-migration-fixtures.svg)](https://pypi.org/project/alembic-migration-fixtures/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/alembic-migration-fixtures)](https://pypi.org/project/alembic-migration-fixtures/)
```

