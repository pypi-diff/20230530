# Comparing `tmp/questdb-connect-0.0.54.tar.gz` & `tmp/questdb-connect-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.54.tar", last modified: Tue May 16 18:59:45 2023, max compression
+gzip compressed data, was "questdb-connect-1.0.6.tar", last modified: Mon May 22 17:23:20 2023, max compression
```

## Comparing `questdb-connect-0.0.54.tar` & `questdb-connect-1.0.6.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:59:45.561900 questdb-connect-0.0.54/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.54/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 18:59:45.561771 questdb-connect-0.0.54/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.54/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-16 18:59:26.000000 questdb-connect-0.0.54/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-16 18:59:45.561933 questdb-connect-0.0.54/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:59:45.556198 questdb-connect-0.0.54/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:59:45.558379 questdb-connect-0.0.54/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.54/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.54/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.54/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.54/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.54/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.54/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:59:45.559862 questdb-connect-0.0.54/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.54/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11427 2023-05-16 13:44:28.000000 questdb-connect-0.0.54/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.54/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    12330 2023-05-16 18:58:06.000000 questdb-connect-0.0.54/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.54/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:59:45.560787 questdb-connect-0.0.54/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 18:59:45.000000 questdb-connect-0.0.54/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-16 18:59:45.000000 questdb-connect-0.0.54/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-16 18:59:45.000000 questdb-connect-0.0.54/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-16 18:59:45.000000 questdb-connect-0.0.54/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-16 18:59:45.000000 questdb-connect-0.0.54/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-16 18:59:45.000000 questdb-connect-0.0.54/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:59:45.561397 questdb-connect-0.0.54/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-16 09:28:52.000000 questdb-connect-0.0.54/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.54/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.54/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.838662 questdb-connect-1.0.6/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-1.0.6/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 17:23:20.838526 questdb-connect-1.0.6/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3789 2023-05-22 13:37:39.000000 questdb-connect-1.0.6/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2640 2023-05-22 17:22:05.000000 questdb-connect-1.0.6/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 17:23:20.838703 questdb-connect-1.0.6/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.830250 questdb-connect-1.0.6/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.832518 questdb-connect-1.0.6/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-1.0.6/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-1.0.6/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.835646 questdb-connect-1.0.6/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-22 14:22:42.000000 questdb-connect-1.0.6/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11788 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-1.0.6/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5780 2023-05-22 09:34:56.000000 questdb-connect-1.0.6/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.836689 questdb-connect-1.0.6/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      788 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      160 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      159 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.836808 questdb-connect-1.0.6/src/superset_ext/
+-rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.6/src/superset_ext/__init__.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.837388 questdb-connect-1.0.6/src/superset_ext/db_engine_specs/
+-rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.6/src/superset_ext/db_engine_specs/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12227 2023-05-22 17:20:15.000000 questdb-connect-1.0.6/src/superset_ext/db_engine_specs/questdb.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.838137 questdb-connect-1.0.6/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-22 17:17:07.000000 questdb-connect-1.0.6/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2846 2023-05-22 17:17:07.000000 questdb-connect-1.0.6/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-1.0.6/tests/test_types.py
```

### Comparing `questdb-connect-0.0.54/LICENSE` & `questdb-connect-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.54/PKG-INFO` & `questdb-connect-1.0.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-Metadata-Version: 2.1
-Name: questdb-connect
-Version: 0.0.54
-Summary: SqlAlchemy/Superset libraries.
-Author-email: "questdb.io" <miguel@questdb.io>
-Project-URL: Homepage, https://github.com/questdb/questdb-connect/
-Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
+<a href="https://questdb.io/docs/" target="blank">
+    <img alt="QuestDB Logo" src="https://questdb.io/img/questdb-logo-themed.svg" width="305px"/>
+</a>
+<p></p>
+<a href="https://slack.questdb.io">
+    <img src="https://slack.questdb.io/badge.svg" alt="QuestDB community Slack channel"/>
+</a>
 
 ## QuestDB Connect
 
-This module offers an implementation of QuestDB's dialect for [SQLAlchemy](https://www.sqlalchemy.org/), 
-as well as an engine specification for [Apache Superset](https://github.com/apache/superset/), using 
+This repository contains an implementation of QuestDB's dialect for [SQLAlchemy](https://www.sqlalchemy.org/),
+as well as an engine specification for [Apache Superset](https://github.com/apache/superset/), using
 [psycopg2](https://www.psycopg.org/) for database connectivity.
 
-Psycopg2 is a widely used and trusted Python module for connecting to and working with PostgreSQL databases. 
+The Python module is available here:
+
+<a href="https://pypi.org/project/questdb-connect/">
+    <img src="https://pypi.org/static/images/logo-small.2a411bc6.svg" alt="PyPi"/>
+    https://pypi.org/project/questdb-connect/
+</a>
+<p></p>
+
+_Psycopg2_ is a widely used and trusted Python module for connecting to and working with PostgreSQL databases.
 It provides a comprehensive set of features for interacting with the PostgreSQL database system.
 
-SQLAlchemy is an open-source SQL toolkit and ORM library for Python. It provides a high-level API for 
-communicating with relational databases, including schema creation and modification, an SQL expression 
-language, and database connection management. The ORM layer abstracts away the complexities of the 
+_SQLAlchemy_ is an open-source SQL toolkit and ORM library for Python. It provides a high-level API for
+communicating with relational databases, including schema creation and modification, an SQL expression
+language, and database connection management. The ORM layer abstracts away the complexities of the
 database, allowing developers to work with Python objects instead of raw SQL statements.
 
-Apache Superset is a popular open-source business intelligence web application that enables users to 
-visualize and explore data through customizable dashboards and reports. It provides a rich set of data 
+_Apache Superset_ is a popular open-source business intelligence web application that enables users to
+visualize and explore data through customizable dashboards and reports. It provides a rich set of data
 visualizations, including charts, tables, and maps.
 
 ## Requirements
 
-* Python from 3.8.x to 3.10.x
-* Psycopg2
-* SQLAlchemy
+* **Python from 3.8.x to 3.10.x** (superset itself use version _3.9.x_)
+* **Psycopg2** `('psycopg2-binary~=2.9.6')`
+* **SQLAlchemy** `('SQLAlchemy<=1.4.47')`
+
+You need to install these packages because questdb-connect depends on them.
 
 ## Installation
 
 You can install this package using pip:
 
 ```shell
 pip install questdb-connect
 ```
 
-## Sample Usage
+## SQLALchemy Sample Usage
 
-Use the QuestDB dialect by specifying it in your SQLAlchemy connection string, 
+Use the QuestDB dialect by specifying it in your SQLAlchemy connection string,
 from that point on use SQLAlchemy:
 
 ```python
 import datetime
 import os
 
 os.environ.setdefault('SQLALCHEMY_SILENCE_UBER_WARNING', '1')
@@ -64,15 +64,15 @@
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base(metadata=MetaData())
 
 
 class Signal(Base):
     __tablename__ = 'signal'
-    __table_args__ = (qdbc.QDBTableEngine('signal', 'ts', qdbc.PartitionBy.HOUR, is_wal=True), )
+    __table_args__ = (qdbc.QDBTableEngine('signal', 'ts', qdbc.PartitionBy.HOUR, is_wal=True),)
     source = Column(qdbc.Symbol)
     value = Column(qdbc.Double)
     ts = Column(qdbc.Timestamp, primary_key=True)
 
 
 def main():
     engine = create_engine('questdb://localhost:8812/main')
@@ -89,12 +89,19 @@
             engine.dispose()
 
 
 if __name__ == '__main__':
     main()
 ```
 
+## Superset Installation
+
+<img alt="QuestDB Logo" src="https://github.com/questdb/questdb-connect/blob/main/docs/superset.png"/>
+
+Follow the instructions available here
+[https://superset.apache.org/docs/installation/installing-superset-from-scratch/](https://superset.apache.org/docs/installation/installing-superset-from-scratch/).
+
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
 please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md)
 if you would like to push a PR.
```

### Comparing `questdb-connect-0.0.54/pyproject.toml` & `questdb-connect-1.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '0.0.54'
+version = '1.0.6'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
-description = "SqlAlchemy/Superset libraries."
+description = "SqlAlchemy/Superset library."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
@@ -42,24 +42,27 @@
 'Homepage' = "https://github.com/questdb/questdb-connect/"
 'Bug Tracker' = "https://github.com/questdb/questdb-connect/issues/"
 
 [project.entry-points.'sqlalchemy.dialects']
 questdb = 'questdb_connect.dialect:QuestDBDialect'
 
 [project.entry-points.'superset.db_engine_specs']
-questdb = 'questdb_connect.superset:QDBEngineSpec'
+questdb = 'superset_ext.db_engine_specs.questdb:QDBEngineSpec'
 
 [project.optional-dependencies]
 test = [
     'psycopg2-binary~=2.9.6',
     'SQLAlchemy<=1.4.47',
     'apache-superset>=2.1.0',
     'sqlparse==0.4.3',
-    'ruff~=0.0.261',
+    'ruff~=0.0.269',
     'pytest~=7.3.0',
+    'black~=23.3.0',
+    'isort~=5.12.0',
+    'bandit~=1.7.5',
 ]
 
 [tool.ruff]
 # https://github.com/charliermarsh/ruff#configuration
 select = ["PL", "RUF", "TCH", "TID", "PT", "C4", "B", "S", "I"]
 line-length = 120
 exclude = [
```

### Comparing `questdb-connect-0.0.54/src/examples/__init__.py` & `questdb-connect-1.0.6/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.54/src/examples/hello_world.py` & `questdb-connect-1.0.6/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.54/src/examples/psycopg2_connect.py` & `questdb-connect-1.0.6/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.54/src/examples/server_utilisation.py` & `questdb-connect-1.0.6/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.54/src/examples/sqlalchemy_orm.py` & `questdb-connect-1.0.6/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.54/src/examples/sqlalchemy_raw.py` & `questdb-connect-1.0.6/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.54/src/questdb_connect/dialect.py` & `questdb-connect-1.0.6/src/questdb_connect/dialect.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,47 +17,46 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import abc
+import logging
 
 import sqlalchemy
 from sqlalchemy import Column, MetaData, text
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
-from sqlalchemy.engine.reflection import Inspector
+from sqlalchemy.engine.reflection import Inspector, cache
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
-from sqlalchemy.sql.compiler import (
-    DDLCompiler,
-    GenericTypeCompiler,
-    IdentifierPreparer,
-    SQLCompiler,
-)
+from sqlalchemy.sql.compiler import DDLCompiler, GenericTypeCompiler, IdentifierPreparer, SQLCompiler
 from sqlalchemy.sql.visitors import Traversible
 
 from . import remove_public_schema
 from .types import *
 
+logger = logging.getLogger(__name__)
+
+
 # ===== SQLAlchemy Dialect ======
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
 
-def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
+def connection_uri(host: str, port: str, username: str, password: str, database: str = 'main'):
     return f'questdb://{username}:{password}@{host}:{port}/{database}'
 
 
 def create_engine(host: str, port: int, username: str, password: str, database: str = 'main'):
     return sqlalchemy.create_engine(
         connection_uri(host, port, username, password, database),
         future=False,
-        hide_parameters=True,
+        hide_parameters=False,
         implicit_returning=False,
-        isolation_level="REPEATABLE READ")
+        isolation_level='REPEATABLE READ')
 
 
 # ===== QUESTDB ENGINE =====
 
 class QDBTableEngine(SchemaEventTarget, Traversible):
     def __init__(
             self,
@@ -141,27 +140,27 @@
         return quote_identifier(value)
 
     def _requires_quotes(self, _value):
         return _value and _has_special_char(_value)
 
     def format_schema(self, name):
         """Prepare a quoted schema name."""
-        return ""
+        return ''
 
     def format_table(self, table, use_schema=True, name=None):
         """Prepare a quoted table and schema name."""
         return quote_identifier(name if name else table.name)
 
 
 class QDBDDLCompiler(DDLCompiler, abc.ABC):
     def visit_create_schema(self, create, **kw):
-        raise Exception('QuestDB does not support SCHEMAS, there is only "public"')
+        raise Exception("QuestDB does not support SCHEMAS, there is only 'public'")
 
     def visit_drop_schema(self, drop, **kw):
-        raise Exception('QuestDB does not support SCHEMAS, there is only "public"')
+        raise Exception("QuestDB does not support SCHEMAS, there is only 'public'")
 
     def visit_create_table(self, create, **kw):
         table = create.element
         create_table = f"CREATE TABLE {quote_identifier(table.fullname)} ("
         create_table += ', '.join([self.get_column_specification(c.element) for c in create.columns])
         return create_table + ') ' + table.engine.get_table_suffix()
 
@@ -225,27 +224,29 @@
             else:
                 table.append_column(Column(col_name, col_type))
         table.engine = QDBTableEngine(table_name, col_ts_name, partition_by, is_wal)
         table.metadata = MetaData()
 
     def get_columns(self, table_name, schema=None, **kw):
         result_set = self.bind.execute(f"table_columns('{table_name}')")
+        return self.format_table_columns(table_name, result_set)
+
+    def get_schema_names(self):
+        return ['public']
+
+    def format_table_columns(self, table_name, result_set):
         if not result_set:
             raise NoResultFound(f"Table '{table_name}' does not exist")
         return [{
             'name': row[0],
             'type': resolve_type_from_name(row[1])(),
             'nullable': True,
             'autoincrement': False,
-            'persisted': True
         } for row in result_set]
 
-    def get_schema_names(self):
-        return ['public']
-
 
 class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
     name = 'questdb'
     psycopg2_version = (2, 9)
     default_schema_name = 'public'
     statement_compiler = QDBSQLCompiler
     ddl_compiler = QDBDDLCompiler
@@ -261,27 +262,38 @@
     supports_multivalues_insert = True
     supports_comments = True
     inline_comments = False
     postfetch_lastrowid = False
     non_native_boolean_check_constraint = False
     max_identifier_length = 255
     _user_defined_max_identifier_length = 255
+    _has_native_hstore = False
     supports_is_distinct_from = False
 
     @classmethod
     def dbapi(cls):
         import questdb_connect as dbapi
         return dbapi
 
     def get_schema_names(self, connection, **kw):
         return ['public']
 
     def get_table_names(self, connection, schema=None, **kw):
         return [row.table for row in connection.execute(text('SHOW TABLES'))]
 
+    def has_table(self, connection, table_name, schema=None):
+        return connection.execute(text(f"tables() WHERE name='{table_name}'")).rowcount == 1
+
+    @cache
+    def get_columns(self, connection, table_name, schema=None, **kw):
+        return self.inspector.format_table_columns(
+            table_name,
+            connection.execute(text(f"table_columns('{table_name}')"))
+        )
+
     def get_pk_constraint(self, connection, table_name, schema=None, **kw):
         return []
 
     def get_foreign_keys(self, connection, table_name, schema=None, postgresql_ignore_search_path=False, **kw):
         return []
 
     def get_temp_table_names(self, connection, **kw):
@@ -301,19 +313,14 @@
 
     def get_unique_constraints(self, connection, table_name, schema=None, **kw):
         return []
 
     def get_check_constraints(self, connection, table_name, schema=None, **kw):
         return []
 
-    def has_table(self, connection, table_name, schema=None):
-        query = f"tables() WHERE name='{table_name}'"
-        result = connection.execute(text(query))
-        return result.rowcount == 1
-
     def has_sequence(self, connection, sequence_name, schema=None, **_kw):
         return False
 
     def do_begin_twophase(self, connection, xid):
         raise NotImplementedError
 
     def do_prepare_twophase(self, connection, xid):
```

### Comparing `questdb-connect-0.0.54/src/questdb_connect/function_names.py` & `questdb-connect-1.0.6/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.54/src/questdb_connect/superset_engine.py` & `questdb-connect-1.0.6/src/superset_ext/db_engine_specs/questdb.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,270 +18,321 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import re
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional
 
 from flask_babel import gettext as __
 from marshmallow import Schema, fields
+from sqlalchemy.engine.interfaces import Dialect
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import (
     BaseEngineSpec,
     BasicParametersMixin,
     BasicParametersType,
 )
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
-from . import remove_public_schema, types
-from .dialect import connection_uri
-from .function_names import FUNCTION_NAMES
+from questdb_connect import remove_public_schema
+from questdb_connect import types as questdb_types
+from questdb_connect.dialect import connection_uri
+from questdb_connect.function_names import FUNCTION_NAMES
 
-# https://superset.apache.org/docs/databases/installing-database-drivers
 # Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
+# https://superset.apache.org/docs/databases/installing-database-drivers
 # https://preset.io/blog/building-database-connector/
+# https://preset.io/blog/improving-apache-superset-integration-database-sqlalchemy/
 
 
 class QDBParametersSchema(Schema):
-    username = fields.String(allow_none=True, description=__('user'))
-    password = fields.String(allow_none=True, description=__('password'))
-    host = fields.String(required=True, description=__('host'))
-    port = fields.Integer(allow_none=True, description=__('port'))
-    database = fields.String(allow_none=True, description=__('database'))
+    username = fields.String(allow_none=True, description=__("user"))
+    password = fields.String(allow_none=True, description=__("password"))
+    host = fields.String(required=True, description=__("host"))
+    port = fields.Integer(allow_none=True, description=__("port"))
+    database = fields.String(allow_none=True, description=__("database"))
 
 
 class QDBEngineSpec(BaseEngineSpec, BasicParametersMixin):
-    engine = 'questdb'
-    engine_name = 'QuestDB Connect'
+    engine = "questdb"
+    engine_name = "QuestDB Connect"
     default_driver = "psycopg2"
     encryption_parameters = {"sslmode": "prefer"}
-    sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname"
+    sqlalchemy_uri_placeholder = "questdb://user:password@host:port/database"
     parameters_schema = QDBParametersSchema()
-    time_groupby_inline = True
+    time_groupby_inline = False
     allows_hidden_cc_in_orderby = True
     time_secondary_columns = True
-    max_column_name_length = 120
     try_remove_schema_from_table_name = True
+    max_column_name_length = 120
     supports_dynamic_schema = False
-    allow_dml = True
-    supports_file_upload = True
     top_keywords = {}
+    # https://en.wikipedia.org/wiki/ISO_8601#Durations
+    # https://questdb.io/docs/reference/function/date-time/#date_trunc
     _time_grain_expressions = {
-        None: '{col}',
-        'PT1S': "date_trunc('second', {col})",
-        'PT5S': "date_trunc('second', {col}) + 5000000",
-        'PT30S': "date_trunc('second', {col}) + 30000000",
-        'PT1M': "date_trunc('minute', {col})",
-        'PT5M': "date_trunc('minute', {col}) + 300000000",
-        'PT10M': "date_trunc('minute', {col}) + 600000000",
-        'PT15M': "date_trunc('minute', {col}) + 900000000",
-        'PT30M': "date_trunc('minute', {col}) + 1800000000",
-        'PT1H': "date_trunc('hour', {col})",
-        'PT6H': "date_trunc('hour', {col})",
-        'PT1D': "date_trunc('day', {col})",
-        'P1W': "date_trunc('week', {col})",
-        'P1M': "date_trunc('month', {col})",
-        'P1Y': "date_trunc('year', {col})",
-        'P3M': "date_trunc('quarter', {col})",
+        None: "{col}",
+        "PT1S": "date_trunc('second', {col})",
+        "PT1M": "date_trunc('minute', {col})",
+        "PT1H": "date_trunc('hour', {col})",
+        "P1D": "date_trunc('day', {col})",
+        "P1W": "date_trunc('week', {col})",
+        "P1M": "date_trunc('month', {col})",
+        "P1Y": "date_trunc('year', {col})",
+        "P3M": "date_trunc('quarter', {col})",
     }
-    _default_column_type_mappings = (
-        (re.compile("^LONG256", re.IGNORECASE), types.Long256, GenericDataType.STRING),
-        (re.compile("^BOOLEAN", re.IGNORECASE), types.Boolean, GenericDataType.BOOLEAN),
-        (re.compile("^BYTE", re.IGNORECASE), types.Byte, GenericDataType.BOOLEAN),
-        (re.compile("^SHORT", re.IGNORECASE), types.Short, GenericDataType.NUMERIC),
-        (re.compile("^INT", re.IGNORECASE), types.Int, GenericDataType.NUMERIC),
-        (re.compile("^LONG", re.IGNORECASE), types.Long, GenericDataType.NUMERIC),
-        (re.compile("^FLOAT", re.IGNORECASE), types.Float, GenericDataType.NUMERIC),
-        (re.compile("^DOUBLE'", re.IGNORECASE), types.Double, GenericDataType.NUMERIC),
-        (re.compile("^SYMBOL", re.IGNORECASE), types.Symbol, GenericDataType.STRING),
-        (re.compile("^STRING", re.IGNORECASE), types.String, GenericDataType.STRING),
-        (re.compile("^UUID", re.IGNORECASE), types.UUID, GenericDataType.STRING),
-        (re.compile("^CHAR", re.IGNORECASE), types.Char, GenericDataType.STRING),
-        (re.compile("^TIMESTAMP", re.IGNORECASE), types.Timestamp, GenericDataType.TEMPORAL),
-        (re.compile("^DATE", re.IGNORECASE), types.Date, GenericDataType.TEMPORAL),
-        (re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE), types.GeohashLong, GenericDataType.STRING),
+    column_type_mappings = (
+        (
+            re.compile("^LONG256", re.IGNORECASE),
+            questdb_types.Long256,
+            GenericDataType.STRING,
+        ),
+        (
+            re.compile("^BOOLEAN", re.IGNORECASE),
+            questdb_types.Boolean,
+            GenericDataType.BOOLEAN,
+        ),
+        (
+            re.compile("^BYTE", re.IGNORECASE),
+            questdb_types.Byte,
+            GenericDataType.NUMERIC,
+        ),
+        (
+            re.compile("^SHORT", re.IGNORECASE),
+            questdb_types.Short,
+            GenericDataType.NUMERIC,
+        ),
+        (re.compile("^INT", re.IGNORECASE), questdb_types.Int, GenericDataType.NUMERIC),
+        (
+            re.compile("^LONG", re.IGNORECASE),
+            questdb_types.Long,
+            GenericDataType.NUMERIC,
+        ),
+        (
+            re.compile("^FLOAT", re.IGNORECASE),
+            questdb_types.Float,
+            GenericDataType.NUMERIC,
+        ),
+        (
+            re.compile("^DOUBLE'", re.IGNORECASE),
+            questdb_types.Double,
+            GenericDataType.NUMERIC,
+        ),
+        (
+            re.compile("^SYMBOL", re.IGNORECASE),
+            questdb_types.Symbol,
+            GenericDataType.STRING,
+        ),
+        (
+            re.compile("^STRING", re.IGNORECASE),
+            questdb_types.String,
+            GenericDataType.STRING,
+        ),
+        (
+            re.compile("^UUID", re.IGNORECASE),
+            questdb_types.UUID,
+            GenericDataType.STRING,
+        ),
+        (
+            re.compile("^CHAR", re.IGNORECASE),
+            questdb_types.Char,
+            GenericDataType.STRING,
+        ),
+        (
+            re.compile("^TIMESTAMP", re.IGNORECASE),
+            questdb_types.Timestamp,
+            GenericDataType.TEMPORAL,
+        ),
+        (
+            re.compile("^DATE", re.IGNORECASE),
+            questdb_types.Date,
+            GenericDataType.TEMPORAL,
+        ),
+        (
+            re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE),
+            questdb_types.GeohashLong,
+            GenericDataType.STRING,
+        ),
     )
-    column_type_mappings = _default_column_type_mappings
 
     @classmethod
     def build_sqlalchemy_uri(
-            cls,
-            parameters: BasicParametersType,
-            encrypted_extra: Optional[Dict[str, str]] = None
+        cls,
+        parameters: BasicParametersType,
+        encrypted_extra: Optional[Dict[str, str]] = None,
     ) -> str:
         return connection_uri(
             parameters.get("host"),
-            int(parameters.get("port")),
+            parameters.get("port"),
             parameters.get("username"),
             parameters.get("password"),
-            parameters.get("database"))
+            parameters.get("database"),
+        )
 
     @classmethod
     def get_default_schema_for_query(cls, database, query) -> Optional[str]:
-        return None
-
-    @classmethod
-    def get_allow_cost_estimate(cls, extra: Dict[str, Any]) -> bool:
-        return False
-
-    @classmethod
-    def get_view_names(cls, database, inspector, schema: Optional[str]):
-        return []
+        return "public"
 
     @classmethod
     def get_text_clause(cls, clause):
         """SQLAlchemy wrapper to ensure text clauses are escaped properly
         :param clause: string clause with potentially unescaped characters
         :return: text clause with escaped characters
         """
         if cls.allows_escaped_colons:
             clause = clause.replace(":", "\\:")
         return text(remove_public_schema(clause))
 
     @classmethod
-    def get_time_grain_expressions(cls) -> Dict[Optional[str], str]:
-        """Return a dict of all supported time grains including any
-        potential added grains but excluding any potentially disabled
-        grains in the config file.
-        :return: All time grain expressions supported by the engine
-        """
-        return cls._time_grain_expressions
-
-    @classmethod
     def epoch_to_dttm(cls) -> str:
-        """SQL expression that converts epoch (seconds) to datetime that can be used in a
-        query. The reference column should be denoted as `{col}` in the return
+        """SQL expression that converts epoch (seconds) to datetime that can be used
+        in a query. The reference column should be denoted as `{col}` in the return
         expression, e.g. "FROM_UNIXTIME({col})"
         :return: SQL Expression
         """
-        return '{col} * 1000000'
+        return "{col} * 1000000"
 
     @classmethod
-    def convert_dttm(cls, target_type: str, dttm: datetime, *_args, **_kwargs) -> Optional[str]:
+    def convert_dttm(
+        cls, target_type: str, dttm: datetime, *_args, **_kwargs
+    ) -> Optional[str]:
         """Convert a Python `datetime` object to a SQL expression.
         :param target_type: The target type of expression
         :param dttm: The datetime object
         :return: The SQL expression
         """
         type_u = target_type.upper()
-        if type_u == 'DATE':
+        if type_u == "DATE":
             return f"TO_DATE('{dttm.date().isoformat()}', 'YYYY-MM-DD')"
-        if type_u in ('DATETIME', 'TIMESTAMP'):
-            dttm_formatted = dttm.isoformat(sep=" ", timespec="microseconds")
+        if type_u in ("DATETIME", "TIMESTAMP"):
+            dttm_formatted = dttm.isoformat(sep="T", timespec="microseconds")
             return f"TO_TIMESTAMP('{dttm_formatted}', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')"
         return None
 
     @classmethod
     def get_datatype(cls, type_code: Any) -> Optional[str]:
         """Change column type code from cursor description to string representation.
         :param type_code: Type code from cursor description
         :return: String representation of type code
         """
-        return type_code.upper() if type_code and isinstance(type_code, str) else 'UNKNOWN'
-
-    @classmethod
-    def get_column_types(
-            cls,
-            column_type: Optional[str],
-    ) -> Optional[Tuple[TypeEngine, GenericDataType]]:
-        """Return a sqlalchemy native column type and generic data type that
-        corresponds to the column type defined in the data source (return None
-        to use default type inferred by SQLAlchemy). Override `column_type_mappings`
-        for specific needs (see MSSQL for example of NCHAR/NVARCHAR handling).
-        :param column_type: Column type returned by inspector
-        :return: SQLAlchemy and generic Superset column types
-        """
-        if not column_type:
-            return None
-        for regex, sqla_type, generic_type in cls._default_column_type_mappings:
-            matching_name = regex.search(column_type)
-            if matching_name:
-                qdbcd_type = types.resolve_type_from_name(sqla_type.__visit_name__)
-                return qdbcd_type.impl, generic_type
-        return None
-
-    @classmethod
-    def get_sqla_column_type(
-            cls,
-            native_type: Optional[str],
-            db_extra: Optional[Dict[str, Any]] = None,
-            source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
-    ) -> Optional[TypeEngine]:
-        """Converts native database type to sqlalchemy column type.
-        :param native_type: Native database type
-        :param db_extra: The database extra object
-        :param source: Type coming from the database table or cursor description
-        :return: ColumnSpec object
-        """
-        if not native_type:
-            return None
-        return types.resolve_type_from_name(native_type).impl
+        if type_code and isinstance(type_code, str):
+            return type_code.upper()
+        return str(type_code)
 
     @classmethod
     def get_column_spec(
-            cls,
-            native_type: Optional[str],
-            db_extra: Optional[Dict[str, Any]] = None,
-            source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
+        cls,
+        native_type: Optional[str],
+        db_extra: Optional[Dict[str, Any]] = None,
+        source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
     ) -> Optional[utils.ColumnSpec]:
         """Get generic type related specs regarding a native column type.
         :param native_type: Native database type
         :param db_extra: The database extra object
         :param source: Type coming from the database table or cursor description
         :return: ColumnSpec object
         """
-        if not native_type:
-            return None
-        sqla_type = types.resolve_type_from_name(native_type)
+        sqla_type = questdb_types.resolve_type_from_name(native_type)
+        if not sqla_type:
+            return BaseEngineSpec.get_column_spec(native_type, db_extra, source)
         name_u = sqla_type.__visit_name__
         generic_type = None
-        if name_u == 'BOOLEAN':
+        if name_u == "BOOLEAN":
             generic_type = GenericDataType.BOOLEAN
-        elif name_u in ('BYTE', 'SHORT', 'INT', 'LONG', 'FLOAT', 'DOUBLE'):
+        elif name_u in ("BYTE", "SHORT", "INT", "LONG", "FLOAT", "DOUBLE"):
             generic_type = GenericDataType.NUMERIC
-        elif name_u in ('SYMBOL', 'STRING', 'CHAR', 'LONG256', 'UUID'):
+        elif name_u in ("SYMBOL", "STRING", "CHAR", "LONG256", "UUID"):
             generic_type = GenericDataType.STRING
-        elif name_u in ('DATE', 'TIMESTAMP'):
+        elif name_u in ("DATE", "TIMESTAMP"):
             generic_type = GenericDataType.TEMPORAL
-        elif 'GEOHASH' in name_u and '(' in name_u and ')' in name_u:
+        elif "GEOHASH" in name_u and "(" in name_u and ")" in name_u:
             generic_type = GenericDataType.STRING
-        return utils.ColumnSpec(sqla_type, generic_type, generic_type == GenericDataType.TEMPORAL)
+        return utils.ColumnSpec(
+            sqla_type, generic_type, generic_type == GenericDataType.TEMPORAL
+        )
+
+    @classmethod
+    def get_sqla_column_type(
+        cls,
+        native_type: Optional[str],
+        db_extra: Optional[Dict[str, Any]] = None,
+        source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
+    ) -> Optional[TypeEngine]:
+        """Converts native database type to sqlalchemy column type.
+        :param native_type: Native database type
+        :param db_extra: The database extra object
+        :param source: Type coming from the database table or cursor description
+        :return: ColumnSpec object
+        """
+        return questdb_types.resolve_type_from_name(native_type).impl
+
+    @classmethod
+    def column_datatype_to_string(
+        cls,
+        sqla_column_type: TypeEngine,
+        dialect: Dialect,
+    ) -> str:
+        """Convert sqlalchemy column type to string representation.
+        By default, removes collation and character encoding info to avoid
+        unnecessarily long datatypes.
+        :param sqla_column_type: SqlAlchemy column type
+        :param dialect: Sqlalchemy dialect
+        :return: Compiled column type
+        """
+        return sqla_column_type.copy().compile(dialect=dialect)
 
     @classmethod
     def select_star(
-            cls,
-            database,
-            table_name: str,
-            engine,
-            schema: Optional[str] = None,
-            limit: int = 100,
-            show_cols: bool = False,
-            indent: bool = True,
-            latest_partition: bool = True,
-            cols: Optional[List[Dict[str, Any]]] = None,
+        cls,
+        database,
+        table_name: str,
+        engine,
+        schema: Optional[str] = None,
+        limit: int = 100,
+        show_cols: bool = False,
+        indent: bool = True,
+        latest_partition: bool = True,
+        cols: Optional[List[Dict[str, Any]]] = None,
     ) -> str:
         """Generate a "SELECT * from table_name" query with appropriate limit.
         :param database: Database instance
         :param table_name: Table name, unquoted
         :param engine: SqlAlchemy Engine instance
         :param schema: Schema, unquoted
         :param limit: limit to impose on query
         :param show_cols: Show columns in query; otherwise use "*"
         :param indent: Add indentation to query
         :param latest_partition: Only query the latest partition
         :param cols: Columns to include in query
         :return: SQL query
         """
-        return super().select_star(database, table_name, engine, None, limit, show_cols, indent, latest_partition, cols)
+        return super().select_star(
+            database,
+            table_name,
+            engine,
+            None,
+            limit,
+            show_cols,
+            indent,
+            latest_partition,
+            cols,
+        )
 
     @classmethod
     def get_function_names(cls, database) -> List[str]:
         """Get a list of function names that are able to be called on the database.
         Used for SQL Lab autocomplete.
         :param database: The database to get functions for
         :return: A list of function names usable in the database
         """
         return FUNCTION_NAMES
+
+    @classmethod
+    def get_allow_cost_estimate(cls, extra: Dict[str, Any]) -> bool:
+        return False
+
+    @classmethod
+    def get_view_names(cls, database, inspector, schema: Optional[str]):
+        return []
```

### Comparing `questdb-connect-0.0.54/src/questdb_connect/types.py` & `questdb-connect-1.0.6/src/questdb_connect/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,21 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-from __future__ import annotations
-
 import enum
 
 import sqlalchemy as sqla
 from sqlalchemy.exc import ArgumentError
 
 # ===== QUESTDB PARTITION TYPE =====
 
-
 class PartitionBy(enum.Enum):
     DAY = 0
     MONTH = 1
     YEAR = 2
     NONE = 3
     HOUR = 4
     WEEK = 5
@@ -96,14 +93,17 @@
     @classmethod
     def matches_type_name(cls, type_name):
         return cls if type_name == cls.__visit_name__ else None
 
     def column_spec(self, column_name):
         return f"{quote_identifier(column_name)} {self.__visit_name__}"
 
+    def compile(self, dialect=None):
+        return self.__visit_name__
+
 
 class Boolean(QDBTypeMixin):
     __visit_name__ = 'BOOLEAN'
     impl = sqla.types.Boolean
     type_code = 1
 
 
@@ -219,14 +219,16 @@
     GeohashInt,
     GeohashShort,
     GeohashLong,
 ]
 
 
 def resolve_type_from_name(type_name):
+    if not type_name:
+        return None
     type_class = _TYPE_CACHE.get(type_name)
     if not type_class:
         for candidate_class in QUESTDB_TYPES:
             type_class = candidate_class.matches_type_name(type_name)
             if type_class:
                 _TYPE_CACHE[type_name] = type_class
                 break
@@ -235,10 +237,8 @@
                 close_p = type_name.index(')')
                 description = type_name[open_p + 1:close_p]
                 g_size = int(description[:-1])
                 if description[-1] in ('C', 'c'):
                     g_size *= 5
                 type_class = geohash_class(g_size)
                 break
-    if not type_class:
-        raise ArgumentError(f'unsupported type: {type_name}')
     return type_class
```

### Comparing `questdb-connect-0.0.54/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-1.0.6/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 src/examples/psycopg2_connect.py
 src/examples/server_utilisation.py
 src/examples/sqlalchemy_orm.py
 src/examples/sqlalchemy_raw.py
 src/questdb_connect/__init__.py
 src/questdb_connect/dialect.py
 src/questdb_connect/function_names.py
-src/questdb_connect/superset_engine.py
 src/questdb_connect/types.py
 src/questdb_connect.egg-info/PKG-INFO
 src/questdb_connect.egg-info/SOURCES.txt
 src/questdb_connect.egg-info/dependency_links.txt
 src/questdb_connect.egg-info/entry_points.txt
 src/questdb_connect.egg-info/requires.txt
 src/questdb_connect.egg-info/top_level.txt
+src/superset_ext/__init__.py
+src/superset_ext/db_engine_specs/__init__.py
+src/superset_ext/db_engine_specs/questdb.py
 tests/test_dialect.py
 tests/test_superset.py
 tests/test_types.py
```

### Comparing `questdb-connect-0.0.54/tests/test_dialect.py` & `questdb-connect-1.0.6/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.54/tests/test_superset.py` & `questdb-connect-1.0.6/tests/test_superset.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,24 +20,21 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import datetime
 from unittest import mock
 
 import pytest
-import sqlalchemy as sqla
-from questdb_connect import types
-from questdb_connect.dialect import QuestDBDialect
-from questdb_connect.superset_engine import QDBEngineSpec
+from superset_ext.db_engine_specs.questdb import QDBEngineSpec
 
 
 def test_build_sqlalchemy_uri():
     request_uri = QDBEngineSpec.build_sqlalchemy_uri({
         'host': 'localhost',
-        'port': 8812,
+        'port': '8812',
         'username': 'admin',
         'password': 'quest',
         'database': 'main',
     })
     assert 'questdb://admin:quest@localhost:8812/main' == request_uri
 
 
@@ -47,20 +44,20 @@
         (
                 "Date",
                 "TO_DATE('2023-04-28', 'YYYY-MM-DD')",
                 datetime.datetime(2023, 4, 28, 23, 55, 59, 281567)
         ),
         (
                 "DateTime",
-                "TO_TIMESTAMP('2023-04-28 23:55:59.281567', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')",
+                "TO_TIMESTAMP('2023-04-28T23:55:59.281567', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')",
                 datetime.datetime(2023, 4, 28, 23, 55, 59, 281567)
         ),
         (
                 "TimeStamp",
-                "TO_TIMESTAMP('2023-04-28 23:55:59.281567', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')",
+                "TO_TIMESTAMP('2023-04-28T23:55:59.281567', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')",
                 datetime.datetime(2023, 4, 28, 23, 55, 59, 281567)
         ),
         ("UnknownType", None, datetime.datetime(2023, 4, 28, 23, 55, 59, 281567)),
     ],
 )
 def test_convert_dttm(target_type, expected_result, dttm) -> None:
     # datetime(year, month, day, hour, minute, second, microsecond)
@@ -80,13 +77,7 @@
 def test_get_table_names():
     inspector = mock.Mock()
     inspector.get_table_names = mock.Mock(return_value=['public.table', 'table_2', '"public.table_3"'])
     pg_result = QDBEngineSpec.get_table_names(
         database=mock.ANY, schema="public", inspector=inspector
     )
     assert pg_result == {'table', '"public.table_3"', 'table_2'}
-
-
-def test_time_exp_literal_no_grain():
-    col = sqla.Column('col_ts', types.Timestamp, primary_key=True)
-    expr = QDBEngineSpec.get_timestamp_expr(col, None, None)
-    assert str(expr.compile(None, dialect=QuestDBDialect())) == 'col_ts'
```

### Comparing `questdb-connect-0.0.54/tests/test_types.py` & `questdb-connect-1.0.6/tests/test_types.py`

 * *Files identical despite different names*

