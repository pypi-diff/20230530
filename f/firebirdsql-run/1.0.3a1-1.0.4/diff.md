# Comparing `tmp/firebirdsql_run-1.0.3a1.tar.gz` & `tmp/firebirdsql_run-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebirdsql_run-1.0.3a1.tar", max compression
+gzip compressed data, was "firebirdsql_run-1.0.4.tar", max compression
```

## Comparing `firebirdsql_run-1.0.3a1.tar` & `firebirdsql_run-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-05-25 16:26:17.636545 firebirdsql_run-1.0.3a1/LICENSE
--rw-r--r--   0        0        0     2067 2023-05-25 16:26:17.636545 firebirdsql_run-1.0.3a1/README.md
--rw-r--r--   0        0        0     2245 2023-05-25 16:26:40.428232 firebirdsql_run-1.0.3a1/pyproject.toml
--rw-r--r--   0        0        0     3123 2023-05-25 16:26:17.636545 firebirdsql_run-1.0.3a1/src/firebirdsql_run/__init__.py
--rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 firebirdsql_run-1.0.3a1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-30 19:49:31.605746 firebirdsql_run-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2152 2023-05-30 19:49:31.605746 firebirdsql_run-1.0.4/README.md
+-rw-r--r--   0        0        0     2239 2023-05-30 19:49:44.869787 firebirdsql_run-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      241 2023-05-30 19:49:31.605746 firebirdsql_run-1.0.4/src/firebirdsql_run/__init__.py
+-rw-r--r--   0        0        0     2851 2023-05-30 19:49:31.605746 firebirdsql_run-1.0.4/src/firebirdsql_run/main.py
+-rw-r--r--   0        0        0      429 2023-05-30 19:49:31.605746 firebirdsql_run-1.0.4/src/firebirdsql_run/type.py
+-rw-r--r--   0        0        0      357 2023-05-30 19:49:31.605746 firebirdsql_run-1.0.4/src/firebirdsql_run/util.py
+-rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 firebirdsql_run-1.0.4/PKG-INFO
```

### Comparing `firebirdsql_run-1.0.3a1/LICENSE` & `firebirdsql_run-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `firebirdsql_run-1.0.3a1/README.md` & `firebirdsql_run-1.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # firebirdsql-run
 
 > [Firebirdsql](https://github.com/nakagami/pyfirebirdsql/) wrapper inspired by [subprocess.run](https://docs.python.org/3/library/subprocess.html#subprocess.run)
 
 [![PyPI version](https://img.shields.io/pypi/v/firebirdsql-run)](https://pypi.org/project/firebirdsql-run)
-[![CI/CD](https://github.com/DeadNews/firebirdsql-run/actions/workflows/python-app.yml/badge.svg)](https://github.com/DeadNews/firebirdsql-run/actions/workflows/python-app.yml)
+[![Main](https://github.com/DeadNews/firebirdsql-run/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/firebirdsql-run/actions/workflows/main.yml)
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/firebirdsql-run/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/firebirdsql-run/main)
 [![codecov](https://codecov.io/gh/DeadNews/firebirdsql-run/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/firebirdsql-run)
 
 ## Installation
 
 ```sh
 pip install firebirdsql-run
 ```
 
 ## Examples
 
-### Execute
+### Table
 
 | maker | model | type |
 | ----- | ----- | ---- |
 | B     | 1121  | PC   |
 | A     | 1232  | PC   |
 
+### Execute
+
 ```py
 result = execute(
     query="SELECT * FROM TABLE",
     host="localhost",
     db="fdb",
     user="sysdba",
-    passwd=getenv("FB_PASSWORD"),
 )
 
 if result.returncode != 0:
     log.error(result)
 else:
     log.info(result)
 ```
 
-- `Info`
+### Info result example
 
 ```py
 CompletedTransaction(
     host="localhost",
     db="fdb",
     user="sysdba",
     returncode=0,
@@ -51,15 +52,15 @@
     data=[
         {"maker": "B", "model": 1121, "type": "PC"},
         {"maker": "A", "model": 1232, "type": "PC"},
     ],
 )
 ```
 
-- `Error`
+### Error result example
 
 ```py
 CompletedTransaction(
     host="localhost",
     db="fdb",
     user="sysdba",
     returncode=1,
@@ -69,21 +70,24 @@
     data=[],
 )
 ```
 
 ### Reuse connection
 
 ```py
-conn = connection(
-    host="localhost",
-    db="fdb",
-    user="sysdba",
-    passwd=getenv("FB_PASSWORD"),
-)
+conn = connection(host="localhost", db="fdb", user="sysdba")
 
 execute(use_conn=conn, query="SELECT * FROM TABLE")
 ...
 callproc(use_conn=conn, procname="PROCNAME", params=(...))
 ...
 
 conn.close()
 ```
+
+## Env variables
+
+```ini
+FIREBIRD_KEY=
+```
+
+The `FIREBIRD_KEY` environment variable can be overridden with the function argument `passwd`.
```

### Comparing `firebirdsql_run-1.0.3a1/pyproject.toml` & `firebirdsql_run-1.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "firebirdsql-run"
-version = "1.0.3-alpha.1"
+version = "1.0.4"
 description = "Firebirdsql wrapper inspired by subprocess.run"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/firebirdsql-run"
 repository = "https://github.com/DeadNews/firebirdsql-run"
 keywords = ["firebird", "sql", "api"]
 classifiers = ["Operating System :: OS Independent", "Topic :: Database"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 firebirdsql = "^1.2.2"
 
-[tool.poetry.group.ci.dependencies]
+[tool.poetry.group.lint.dependencies]
 black = "^23.3.0"
 mypy = "^1.2.0"
 poethepoet = "^0.20.0"
 ruff = "^0.0.270"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
```

### Comparing `firebirdsql_run-1.0.3a1/src/firebirdsql_run/__init__.py` & `firebirdsql_run-1.0.4/src/firebirdsql_run/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,16 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 """Firebirdsql wrapper inspired by subprocess.run."""
-from datetime import datetime
 from pathlib import Path
 from socket import getfqdn
-from typing import NamedTuple
 
 from firebirdsql import Connection, connect
 
-FBTypes = str | float | datetime | None
-Dataset = list[dict[str, FBTypes]]
-
-
-class CompletedTransaction(NamedTuple):
-    """The return value from execute(), representing a transaction that has finished."""
-
-    host: str
-    db: str
-    user: str
-    returncode: int
-    error: str
-    query: str
-    params: tuple
-    data: Dataset
+from firebirdsql_run.type import CompletedTransaction
+from firebirdsql_run.util import get_env
 
 
 class ExecuteError(Exception):
     """Exception raised for execute transaction errors."""
 
 
 def connection(
@@ -37,15 +22,15 @@
 ) -> Connection:
     """Create a connection to the database."""
     return connect(
         host=getfqdn(host),
         database=f"{db}",
         port=port,
         user=user,
-        password=passwd,
+        password=passwd or get_env("FIREBIRD_KEY"),
     )
 
 
 def execute(
     query: str,
     params: tuple = (),
     db: Path | str = "",
```

### Comparing `firebirdsql_run-1.0.3a1/PKG-INFO` & `firebirdsql_run-1.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebirdsql-run
-Version: 1.0.3a1
+Version: 1.0.4
 Summary: Firebirdsql wrapper inspired by subprocess.run
 Home-page: https://github.com/DeadNews/firebirdsql-run
 License: MIT
 Keywords: firebird,sql,api
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
@@ -19,49 +19,50 @@
 Description-Content-Type: text/markdown
 
 # firebirdsql-run
 
 > [Firebirdsql](https://github.com/nakagami/pyfirebirdsql/) wrapper inspired by [subprocess.run](https://docs.python.org/3/library/subprocess.html#subprocess.run)
 
 [![PyPI version](https://img.shields.io/pypi/v/firebirdsql-run)](https://pypi.org/project/firebirdsql-run)
-[![CI/CD](https://github.com/DeadNews/firebirdsql-run/actions/workflows/python-app.yml/badge.svg)](https://github.com/DeadNews/firebirdsql-run/actions/workflows/python-app.yml)
+[![Main](https://github.com/DeadNews/firebirdsql-run/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/firebirdsql-run/actions/workflows/main.yml)
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/firebirdsql-run/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/firebirdsql-run/main)
 [![codecov](https://codecov.io/gh/DeadNews/firebirdsql-run/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/firebirdsql-run)
 
 ## Installation
 
 ```sh
 pip install firebirdsql-run
 ```
 
 ## Examples
 
-### Execute
+### Table
 
 | maker | model | type |
 | ----- | ----- | ---- |
 | B     | 1121  | PC   |
 | A     | 1232  | PC   |
 
+### Execute
+
 ```py
 result = execute(
     query="SELECT * FROM TABLE",
     host="localhost",
     db="fdb",
     user="sysdba",
-    passwd=getenv("FB_PASSWORD"),
 )
 
 if result.returncode != 0:
     log.error(result)
 else:
     log.info(result)
 ```
 
-- `Info`
+### Info result example
 
 ```py
 CompletedTransaction(
     host="localhost",
     db="fdb",
     user="sysdba",
     returncode=0,
@@ -71,15 +72,15 @@
     data=[
         {"maker": "B", "model": 1121, "type": "PC"},
         {"maker": "A", "model": 1232, "type": "PC"},
     ],
 )
 ```
 
-- `Error`
+### Error result example
 
 ```py
 CompletedTransaction(
     host="localhost",
     db="fdb",
     user="sysdba",
     returncode=1,
@@ -89,22 +90,25 @@
     data=[],
 )
 ```
 
 ### Reuse connection
 
 ```py
-conn = connection(
-    host="localhost",
-    db="fdb",
-    user="sysdba",
-    passwd=getenv("FB_PASSWORD"),
-)
+conn = connection(host="localhost", db="fdb", user="sysdba")
 
 execute(use_conn=conn, query="SELECT * FROM TABLE")
 ...
 callproc(use_conn=conn, procname="PROCNAME", params=(...))
 ...
 
 conn.close()
 ```
 
+## Env variables
+
+```ini
+FIREBIRD_KEY=
+```
+
+The `FIREBIRD_KEY` environment variable can be overridden with the function argument `passwd`.
+
```

