# Comparing `tmp/questdb-connect-1.0.6.tar.gz` & `tmp/questdb-connect-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-1.0.6.tar", last modified: Mon May 22 17:23:20 2023, max compression
+gzip compressed data, was "questdb-connect-1.0.8.tar", last modified: Tue May 30 11:52:59 2023, max compression
```

## Comparing `questdb-connect-1.0.6.tar` & `questdb-connect-1.0.8.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.838662 questdb-connect-1.0.6/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-1.0.6/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 17:23:20.838526 questdb-connect-1.0.6/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3789 2023-05-22 13:37:39.000000 questdb-connect-1.0.6/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2640 2023-05-22 17:22:05.000000 questdb-connect-1.0.6/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 17:23:20.838703 questdb-connect-1.0.6/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.830250 questdb-connect-1.0.6/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.832518 questdb-connect-1.0.6/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-1.0.6/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-1.0.6/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.835646 questdb-connect-1.0.6/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-22 14:22:42.000000 questdb-connect-1.0.6/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11788 2023-05-22 17:17:06.000000 questdb-connect-1.0.6/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-1.0.6/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)     5780 2023-05-22 09:34:56.000000 questdb-connect-1.0.6/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.836689 questdb-connect-1.0.6/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      788 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      160 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      159 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 17:23:20.000000 questdb-connect-1.0.6/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.836808 questdb-connect-1.0.6/src/superset_ext/
--rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.6/src/superset_ext/__init__.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.837388 questdb-connect-1.0.6/src/superset_ext/db_engine_specs/
--rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.6/src/superset_ext/db_engine_specs/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    12227 2023-05-22 17:20:15.000000 questdb-connect-1.0.6/src/superset_ext/db_engine_specs/questdb.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 17:23:20.838137 questdb-connect-1.0.6/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-22 17:17:07.000000 questdb-connect-1.0.6/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2846 2023-05-22 17:17:07.000000 questdb-connect-1.0.6/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-1.0.6/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-30 11:52:59.495148 questdb-connect-1.0.8/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-1.0.8/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4459 2023-05-30 11:52:59.495005 questdb-connect-1.0.8/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3785 2023-05-30 11:44:41.000000 questdb-connect-1.0.8/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2581 2023-05-30 11:52:45.000000 questdb-connect-1.0.8/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-30 11:52:59.495195 questdb-connect-1.0.8/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-30 11:52:59.488167 questdb-connect-1.0.8/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-30 11:52:59.490513 questdb-connect-1.0.8/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1141 2023-05-26 14:30:55.000000 questdb-connect-1.0.8/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1841 2023-05-26 14:30:56.000000 questdb-connect-1.0.8/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2457 2023-05-26 14:30:56.000000 questdb-connect-1.0.8/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2855 2023-05-26 14:30:56.000000 questdb-connect-1.0.8/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3971 2023-05-26 14:30:56.000000 questdb-connect-1.0.8/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2047 2023-05-26 14:30:56.000000 questdb-connect-1.0.8/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-30 11:52:59.492420 questdb-connect-1.0.8/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3215 2023-05-30 11:23:53.000000 questdb-connect-1.0.8/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1548 2023-05-30 11:23:53.000000 questdb-connect-1.0.8/src/questdb_connect/common.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2306 2023-05-26 14:34:24.000000 questdb-connect-1.0.8/src/questdb_connect/compilers.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4932 2023-05-26 14:34:14.000000 questdb-connect-1.0.8/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2446 2023-05-26 14:33:11.000000 questdb-connect-1.0.8/src/questdb_connect/identifier_preparer.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3652 2023-05-30 11:23:53.000000 questdb-connect-1.0.8/src/questdb_connect/inspector.py
+-rw-r--r--   0 marregui   (501) staff       (20)     6305 2023-05-26 14:33:09.000000 questdb-connect-1.0.8/src/questdb_connect/keywords_functions.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2549 2023-05-30 11:23:53.000000 questdb-connect-1.0.8/src/questdb_connect/table_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5460 2023-05-30 11:24:19.000000 questdb-connect-1.0.8/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-30 11:52:59.493331 questdb-connect-1.0.8/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4459 2023-05-30 11:52:59.000000 questdb-connect-1.0.8/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      955 2023-05-30 11:52:59.000000 questdb-connect-1.0.8/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-30 11:52:59.000000 questdb-connect-1.0.8/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      160 2023-05-30 11:52:59.000000 questdb-connect-1.0.8/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      131 2023-05-30 11:52:59.000000 questdb-connect-1.0.8/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       34 2023-05-30 11:52:59.000000 questdb-connect-1.0.8/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-30 11:52:59.493461 questdb-connect-1.0.8/src/superset/
+-rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-26 15:13:18.000000 questdb-connect-1.0.8/src/superset/__init__.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-30 11:52:59.493985 questdb-connect-1.0.8/src/superset/db_engine_specs/
+-rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-26 15:13:18.000000 questdb-connect-1.0.8/src/superset/db_engine_specs/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10881 2023-05-26 15:13:18.000000 questdb-connect-1.0.8/src/superset/db_engine_specs/questdb.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-30 11:52:59.494650 questdb-connect-1.0.8/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)    10194 2023-05-26 14:38:33.000000 questdb-connect-1.0.8/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1243 2023-05-26 15:06:45.000000 questdb-connect-1.0.8/tests/test_examples.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3218 2023-05-26 14:38:05.000000 questdb-connect-1.0.8/tests/test_types.py
```

### Comparing `questdb-connect-1.0.6/LICENSE` & `questdb-connect-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.6/PKG-INFO` & `questdb-connect-1.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 1.0.6
-Summary: SqlAlchemy/Superset library.
+Version: 1.0.8
+Summary: SqlAlchemy library
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
+Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <a href="https://questdb.io/docs/" target="blank">
     <img alt="QuestDB Logo" src="https://questdb.io/img/questdb-logo-themed.svg" width="305px"/>
 </a>
@@ -34,29 +34,28 @@
 
 <a href="https://pypi.org/project/questdb-connect/">
     <img src="https://pypi.org/static/images/logo-small.2a411bc6.svg" alt="PyPi"/>
     https://pypi.org/project/questdb-connect/
 </a>
 <p></p>
 
-_Psycopg2_ is a widely used and trusted Python module for connecting to and working with PostgreSQL databases.
-It provides a comprehensive set of features for interacting with the PostgreSQL database system.
+_Psycopg2_ is a widely used and trusted Python module for connecting to, and working with, QuestDB and other
+PostgreSQL databases.
 
-_SQLAlchemy_ is an open-source SQL toolkit and ORM library for Python. It provides a high-level API for
-communicating with relational databases, including schema creation and modification, an SQL expression
-language, and database connection management. The ORM layer abstracts away the complexities of the
-database, allowing developers to work with Python objects instead of raw SQL statements.
-
-_Apache Superset_ is a popular open-source business intelligence web application that enables users to
-visualize and explore data through customizable dashboards and reports. It provides a rich set of data
-visualizations, including charts, tables, and maps.
+_SQLAlchemy_ is a SQL toolkit and ORM library for Python. It provides a high-level API for communicating with 
+relational databases, including schema creation and modification. The ORM layer abstracts away the complexities 
+of the database, allowing developers to work with Python objects instead of raw SQL statements.
+
+_Apache Superset_ is an open-source business intelligence web application that enables users to visualize and 
+explore data through customizable dashboards and reports. It provides a rich set of data visualizations, including 
+charts, tables, and maps.
 
 ## Requirements
 
-* **Python from 3.8.x to 3.10.x** (superset itself use version _3.9.x_)
+* **Python from 3.9 to 3.11** (superset itself use version _3.9.x_)
 * **Psycopg2** `('psycopg2-binary~=2.9.6')`
 * **SQLAlchemy** `('SQLAlchemy<=1.4.47')`
 
 You need to install these packages because questdb-connect depends on them.
 
 ## Installation
 
@@ -64,16 +63,22 @@
 
 ```shell
 pip install questdb-connect
 ```
 
 ## SQLALchemy Sample Usage
 
-Use the QuestDB dialect by specifying it in your SQLAlchemy connection string,
-from that point on use SQLAlchemy:
+Use the QuestDB dialect by specifying it in your SQLAlchemy connection string:
+
+```shell
+questdb://admin:quest@localhost:8812/main
+questdb://admin:quest@host.docker.internal:8812/main
+```
+
+From that point on use standard SQLAlchemy:
 
 ```python
 import datetime
 import os
 
 os.environ.setdefault('SQLALCHEMY_SILENCE_UBER_WARNING', '1')
 
@@ -109,17 +114,18 @@
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Superset Installation
 
-<img alt="QuestDB Logo" src="https://github.com/questdb/questdb-connect/blob/main/docs/superset.png"/>
+<a href="https://superset.apache.org/docs/installation/installing-superset-from-scratch/" target="blank">
+    <img alt="Apache Superset" src="https://github.com/questdb/questdb-connect/blob/main/docs/superset.png"/>
+</a>
 
-Follow the instructions available here
-[https://superset.apache.org/docs/installation/installing-superset-from-scratch/](https://superset.apache.org/docs/installation/installing-superset-from-scratch/).
+Follow the instructions available [here](https://superset.apache.org/docs/installation/installing-superset-from-scratch/).
 
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
 please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md)
 if you would like to push a PR.
```

### Comparing `questdb-connect-1.0.6/README.md` & `questdb-connect-1.0.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 
 <a href="https://pypi.org/project/questdb-connect/">
     <img src="https://pypi.org/static/images/logo-small.2a411bc6.svg" alt="PyPi"/>
     https://pypi.org/project/questdb-connect/
 </a>
 <p></p>
 
-_Psycopg2_ is a widely used and trusted Python module for connecting to and working with PostgreSQL databases.
-It provides a comprehensive set of features for interacting with the PostgreSQL database system.
+_Psycopg2_ is a widely used and trusted Python module for connecting to, and working with, QuestDB and other
+PostgreSQL databases.
 
-_SQLAlchemy_ is an open-source SQL toolkit and ORM library for Python. It provides a high-level API for
-communicating with relational databases, including schema creation and modification, an SQL expression
-language, and database connection management. The ORM layer abstracts away the complexities of the
-database, allowing developers to work with Python objects instead of raw SQL statements.
-
-_Apache Superset_ is a popular open-source business intelligence web application that enables users to
-visualize and explore data through customizable dashboards and reports. It provides a rich set of data
-visualizations, including charts, tables, and maps.
+_SQLAlchemy_ is a SQL toolkit and ORM library for Python. It provides a high-level API for communicating with 
+relational databases, including schema creation and modification. The ORM layer abstracts away the complexities 
+of the database, allowing developers to work with Python objects instead of raw SQL statements.
+
+_Apache Superset_ is an open-source business intelligence web application that enables users to visualize and 
+explore data through customizable dashboards and reports. It provides a rich set of data visualizations, including 
+charts, tables, and maps.
 
 ## Requirements
 
-* **Python from 3.8.x to 3.10.x** (superset itself use version _3.9.x_)
+* **Python from 3.9 to 3.11** (superset itself use version _3.9.x_)
 * **Psycopg2** `('psycopg2-binary~=2.9.6')`
 * **SQLAlchemy** `('SQLAlchemy<=1.4.47')`
 
 You need to install these packages because questdb-connect depends on them.
 
 ## Installation
 
@@ -46,16 +45,22 @@
 
 ```shell
 pip install questdb-connect
 ```
 
 ## SQLALchemy Sample Usage
 
-Use the QuestDB dialect by specifying it in your SQLAlchemy connection string,
-from that point on use SQLAlchemy:
+Use the QuestDB dialect by specifying it in your SQLAlchemy connection string:
+
+```shell
+questdb://admin:quest@localhost:8812/main
+questdb://admin:quest@host.docker.internal:8812/main
+```
+
+From that point on use standard SQLAlchemy:
 
 ```python
 import datetime
 import os
 
 os.environ.setdefault('SQLALCHEMY_SILENCE_UBER_WARNING', '1')
 
@@ -91,17 +96,18 @@
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Superset Installation
 
-<img alt="QuestDB Logo" src="https://github.com/questdb/questdb-connect/blob/main/docs/superset.png"/>
+<a href="https://superset.apache.org/docs/installation/installing-superset-from-scratch/" target="blank">
+    <img alt="Apache Superset" src="https://github.com/questdb/questdb-connect/blob/main/docs/superset.png"/>
+</a>
 
-Follow the instructions available here
-[https://superset.apache.org/docs/installation/installing-superset-from-scratch/](https://superset.apache.org/docs/installation/installing-superset-from-scratch/).
+Follow the instructions available [here](https://superset.apache.org/docs/installation/installing-superset-from-scratch/).
 
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
 please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md)
 if you would like to push a PR.
```

### Comparing `questdb-connect-1.0.6/pyproject.toml` & `questdb-connect-1.0.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -19,62 +19,61 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '1.0.6'
+version = '1.0.8'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
-description = "SqlAlchemy/Superset library."
+description = "SqlAlchemy library"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     'Intended Audience :: Developers',
+    'Topic :: Database',
     'License :: OSI Approved :: Apache Software License',
-    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11'
+    'Programming Language :: Python :: 3.11',
 ]
 dependencies = []
 
 [project.urls]
 'Homepage' = "https://github.com/questdb/questdb-connect/"
 'Bug Tracker' = "https://github.com/questdb/questdb-connect/issues/"
 
 [project.entry-points.'sqlalchemy.dialects']
 questdb = 'questdb_connect.dialect:QuestDBDialect'
 
 [project.entry-points.'superset.db_engine_specs']
-questdb = 'superset_ext.db_engine_specs.questdb:QDBEngineSpec'
+questdb = 'superset.db_engine_specs.questdb:QuestDbEngineSpec'
 
 [project.optional-dependencies]
 test = [
     'psycopg2-binary~=2.9.6',
     'SQLAlchemy<=1.4.47',
     'apache-superset>=2.1.0',
     'sqlparse==0.4.3',
-    'ruff~=0.0.269',
     'pytest~=7.3.0',
     'black~=23.3.0',
-    'isort~=5.12.0',
-    'bandit~=1.7.5',
+    'ruff~=0.0.269',
 ]
 
 [tool.ruff]
 # https://github.com/charliermarsh/ruff#configuration
 select = ["PL", "RUF", "TCH", "TID", "PT", "C4", "B", "S", "I"]
 line-length = 120
 exclude = [
     ".pytest_cache",
     ".questdb_data",
     ".git",
     ".ruff_cache",
     "venv",
+    "dist",
     "questdb_connect.egg-info",
 ]
 
 [tool.ruff.pylint]
 max-branches = 20
 max-args = 10
```

### Comparing `questdb-connect-1.0.6/src/examples/__init__.py` & `questdb-connect-1.0.8/src/examples/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import os
 
 CONNECTION_ATTRS = {
-    'host': os.environ.get('QUESTDB_CONNECT_HOST', 'localhost'),
-    'port': int(os.environ.get('QUESTDB_CONNECT_PORT', '8812')),
-    'username': os.environ.get('QUESTDB_CONNECT_USER', 'admin'),
-    'password': os.environ.get('QUESTDB_CONNECT_PASSWORD', 'quest')
+    "host": os.environ.get("QUESTDB_CONNECT_HOST", "localhost"),
+    "port": int(os.environ.get("QUESTDB_CONNECT_PORT", "8812")),
+    "username": os.environ.get("QUESTDB_CONNECT_USER", "admin"),
+    "password": os.environ.get("QUESTDB_CONNECT_PASSWORD", "quest"),
 }
```

### Comparing `questdb-connect-1.0.6/src/examples/hello_world.py` & `questdb-connect-1.0.8/src/questdb_connect/compilers.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,48 +16,45 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-import datetime
-import os
+import abc
 
-os.environ.setdefault('SQLALCHEMY_SILENCE_UBER_WARNING', '1')
+import sqlalchemy
 
-import questdb_connect.dialect as qdbc
-from sqlalchemy import Column, MetaData, create_engine, insert
-from sqlalchemy.orm import declarative_base
-
-Base = declarative_base(metadata=MetaData())
-
-
-class Signal(Base):
-    __tablename__ = 'signal'
-    __table_args__ = (qdbc.QDBTableEngine(
-        'signal',
-        'ts',
-        qdbc.PartitionBy.HOUR,
-        is_wal=True),)
-    source = Column(qdbc.Symbol)
-    value = Column(qdbc.Double)
-    ts = Column(qdbc.Timestamp, primary_key=True)
-
-
-def main():
-    engine = create_engine('questdb://localhost:8812/main')
-    try:
-        Base.metadata.create_all(engine)
-        with engine.connect() as conn:
-            conn.execute(insert(Signal).values(
-                source='coconut',
-                value=16.88993244,
-                ts=datetime.datetime.utcnow()
-            ))
-    finally:
-        if engine:
-            engine.dispose()
+from .common import quote_identifier, remove_public_schema
+from .types import QDBTypeMixin
 
 
-if __name__ == '__main__':
-    main()
+class QDBDDLCompiler(sqlalchemy.sql.compiler.DDLCompiler, abc.ABC):
+    def visit_create_schema(self, create, **kw):
+        raise Exception("QuestDB does not support SCHEMAS, there is only 'public'")
+
+    def visit_drop_schema(self, drop, **kw):
+        raise Exception("QuestDB does not support SCHEMAS, there is only 'public'")
+
+    def visit_create_table(self, create, **kw):
+        table = create.element
+        create_table = f"CREATE TABLE {quote_identifier(table.fullname)} ("
+        create_table += ", ".join(
+            [self.get_column_specification(c.element) for c in create.columns]
+        )
+        return create_table + ") " + table.engine.get_table_suffix()
+
+    def get_column_specification(self, column: sqlalchemy.Column, **_):
+        if not isinstance(column.type, QDBTypeMixin):
+            raise sqlalchemy.exc.ArgumentError(
+                "Column type is not a valid QuestDB type"
+            )
+        return column.type.column_spec(column.name)
+
+
+class QDBSQLCompiler(sqlalchemy.sql.compiler.SQLCompiler, abc.ABC):
+    def _is_safe_for_fast_insert_values_helper(self):
+        return True
+
+    def visit_textclause(self, textclause, add_to_result_map=None, **kw):
+        textclause.text = remove_public_schema(textclause.text)
+        return super().visit_textclause(textclause, add_to_result_map, **kw)
```

### Comparing `questdb-connect-1.0.6/src/examples/psycopg2_connect.py` & `questdb-connect-1.0.8/src/examples/psycopg2_connect.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,43 +33,45 @@
 from questdb_connect import connect
 
 from examples import CONNECTION_ATTRS
 
 
 def print_partition(row):
     p_index, p_by, _, min_ts, max_ts, num_rows, _, p_size, *_ = row
-    print(f' - Partition {p_index} by {p_by} [{min_ts}, {max_ts}] {num_rows} rows {p_size}')
+    print(
+        f" - Partition {p_index} by {p_by} [{min_ts}, {max_ts}] {num_rows} rows {p_size}"
+    )
 
 
 def print_table(row):
     table_id, table_name, ts_column, p_by, _, _, is_wal, dir_name = row
-    msg = ', '.join((
-        f'Table id:{table_id}',
-        f'name:{table_name}',
-        f'ts-col:{ts_column}',
-        f'partition-by:{p_by}',
-        f'is-wal:{is_wal}',
-        f'dir-name:{dir_name}'))
+    msg = ", ".join(
+        (
+            f"Table id:{table_id}",
+            f"name:{table_name}",
+            f"ts-col:{ts_column}",
+            f"partition-by:{p_by}",
+            f"is-wal:{is_wal}",
+            f"dir-name:{dir_name}",
+        )
+    )
     print(msg)
 
 
 def print_server_info(dsn_parameters):
-    print(f'QuestDB server information: {json.dumps(dsn_parameters, indent=4)}')
+    print(f"QuestDB server information: {json.dumps(dsn_parameters, indent=4)}")
 
 
 def main():
     with connect(**CONNECTION_ATTRS) as conn:
         print_server_info(conn.get_dsn_parameters())
-        with (
-            conn.cursor() as tables_cur,
-            conn.cursor() as partitions_cur
-        ):
+        with conn.cursor() as tables_cur, conn.cursor() as partitions_cur:
             tables_cur.execute("tables()")
             for table_row in tables_cur.fetchall():
                 print_table(table_row)
                 partitions_cur.execute(f"table_partitions('{table_row[1]}')")
                 for partition_row in partitions_cur.fetchall():
                     print_partition(partition_row)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `questdb-connect-1.0.6/src/examples/server_utilisation.py` & `questdb-connect-1.0.8/src/examples/server_utilisation.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 #
 import datetime
 import enum
 import os
 import random
 import time
 
-os.environ.setdefault('SQLALCHEMY_SILENCE_UBER_WARNING', '1')
+os.environ.setdefault("SQLALCHEMY_SILENCE_UBER_WARNING", "1")
 
-import questdb_connect.dialect as qdbc
+import questdb_connect as qdbc
 from sqlalchemy import Column, MetaData, create_engine
 from sqlalchemy.orm import Session, declarative_base
 
 
 class BaseEnum(enum.Enum):
     @classmethod
     def rand(cls):
@@ -52,43 +52,41 @@
     NETWORK = 4
 
 
 Base = declarative_base(metadata=MetaData())
 
 
 class NodeMetrics(Base):
-    __tablename__ = 'node_metrics'
-    __table_args__ = (qdbc.QDBTableEngine(
-        'node_metrics',
-        'ts',
-        qdbc.PartitionBy.HOUR,
-        is_wal=True),)
+    __tablename__ = "node_metrics"
+    __table_args__ = (
+        qdbc.QDBTableEngine("node_metrics", "ts", qdbc.PartitionBy.HOUR, is_wal=True),
+    )
     source = Column(qdbc.Symbol)  # Nodes
     attr_name = Column(qdbc.Symbol)  # Metrics
     attr_value = Column(qdbc.Double)
     ts = Column(qdbc.Timestamp, primary_key=True)
 
 
-def main():
-    end_time = time.time() + 10.0
-    engine = create_engine('questdb://localhost:8812/main')
+def main(duration_sec: float = 10.0):
+    end_time = time.time() + max(duration_sec - 0.5, 2.0)
+    engine = create_engine("questdb://localhost:8812/main")
     session = Session(engine)
     max_batch_size = 3000
     try:
         Base.metadata.drop_all(engine)
         Base.metadata.create_all(engine)
         batch_size = 0
         while time.time() < end_time:
             node = Nodes.rand()
             session.add(
                 NodeMetrics(
                     source=node.name,
                     attr_name=Metrics.rand().name,
                     attr_value=random.random() * node.value * random.randint(1, 100),
-                    ts=datetime.datetime.utcnow()
+                    ts=datetime.datetime.utcnow(),
                 )
             )
             batch_size += 1
             if batch_size > max_batch_size:
                 session.commit()
                 batch_size = 0
         if batch_size > 0:
@@ -96,9 +94,9 @@
     finally:
         if session:
             session.close()
         if engine:
             engine.dispose()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `questdb-connect-1.0.6/src/examples/sqlalchemy_orm.py` & `questdb-connect-1.0.8/src/examples/sqlalchemy_orm.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,30 +21,31 @@
 #  limitations under the License.
 #
 import datetime
 import json
 import os
 import time
 
-os.environ.setdefault('SQLALCHEMY_SILENCE_UBER_WARNING', '1')
+os.environ.setdefault("SQLALCHEMY_SILENCE_UBER_WARNING", "1")
 
-import questdb_connect.dialect as qdbc
+import questdb_connect as qdbc
 from sqlalchemy import Column, MetaData, insert, text
 from sqlalchemy.orm import declarative_base
 
 from examples import CONNECTION_ATTRS
 
 Base = declarative_base(metadata=MetaData())
-table_name = 'all_types'
+table_name = "all_types"
 
 
 class MyTable(Base):
     __tablename__ = table_name
     __table_args__ = (
-        qdbc.QDBTableEngine(table_name, 'col_ts', qdbc.PartitionBy.DAY, is_wal=True),)
+        qdbc.QDBTableEngine(table_name, "col_ts", qdbc.PartitionBy.DAY, is_wal=True),
+    )
     col_boolean = Column(qdbc.Boolean)
     col_byte = Column(qdbc.Byte)
     col_short = Column(qdbc.Short)
     col_int = Column(qdbc.Int)
     col_long = Column(qdbc.Long)
     col_float = Column(qdbc.Float)
     col_double = Column(qdbc.Double)
@@ -77,39 +78,41 @@
         # create the 'all_types' table
         Base.metadata.create_all(engine)
 
         # connect with QuestDB
         with engine.connect() as conn:
             # insert a fully populated row
             now = datetime.datetime(2023, 4, 22, 18, 10, 10, 765123)
-            conn.execute(insert(MyTable).values(
-                col_boolean=True,
-                col_byte=8,
-                col_short=12,
-                col_int=13,
-                col_long=14,
-                col_float=15.234,
-                col_double=16.88993244,
-                col_symbol='coconut',
-                col_string='banana',
-                col_char='C',
-                col_uuid='6d5eb038-63d1-4971-8484-30c16e13de5b',
-                col_date=now.date(),
-                col_ts=now,
-                col_geohash='dfvgsj2vptwu',
-                col_long256='0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a'
-            ))
+            conn.execute(
+                insert(MyTable).values(
+                    col_boolean=True,
+                    col_byte=8,
+                    col_short=12,
+                    col_int=13,
+                    col_long=14,
+                    col_float=15.234,
+                    col_double=16.88993244,
+                    col_symbol="coconut",
+                    col_string="banana",
+                    col_char="C",
+                    col_uuid="6d5eb038-63d1-4971-8484-30c16e13de5b",
+                    col_date=now.date(),
+                    col_ts=now,
+                    col_geohash="dfvgsj2vptwu",
+                    col_long256="0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a",
+                )
+            )
             columns = [col.name for col in MyTable.__table__.columns]
             while True:
-                rs = conn.execute(text('all_types'))
+                rs = conn.execute(text("all_types"))
                 if rs.rowcount:
-                    print(f'rows: {rs.rowcount}')
+                    print(f"rows: {rs.rowcount}")
                     for row in rs:
                         print(json.dumps(dict(zip(columns, map(str, row))), indent=4))
                     break
     finally:
         if engine:
             engine.dispose()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `questdb-connect-1.0.6/src/questdb_connect/types.py` & `questdb-connect-1.0.8/src/questdb_connect/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,164 +18,143 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import enum
 
-import sqlalchemy as sqla
-from sqlalchemy.exc import ArgumentError
+import sqlalchemy
 
-# ===== QUESTDB PARTITION TYPE =====
+from .common import quote_identifier
 
-class PartitionBy(enum.Enum):
-    DAY = 0
-    MONTH = 1
-    YEAR = 2
-    NONE = 3
-    HOUR = 4
-    WEEK = 5
-
-
-# ===== QUESTDB DATA TYPES =====
-
-_QUOTES = ("'", '"')
 _GEOHASH_BYTE_MAX = 8
 _GEOHASH_SHORT_MAX = 16
 _GEOHASH_INT_MAX = 32
 _GEOHASH_LONG_BITS = 60
 _TYPE_CACHE = {
     # key:   '__visit_name__' of the implementor of QDBTypeMixin
     # value: implementor class itself
 }
 
 
 def geohash_type_name(bits):
     if not isinstance(bits, int) or bits < 0 or bits > _GEOHASH_LONG_BITS:
-        raise ArgumentError(f'geohash precision must be int [0, {_GEOHASH_LONG_BITS}]')
+        raise sqlalchemy.exc.ArgumentError(
+            f"geohash precision must be int [0, {_GEOHASH_LONG_BITS}]"
+        )
     if 0 < bits <= _GEOHASH_BYTE_MAX:
-        return f'GEOHASH(8b)'
+        return f"GEOHASH(8b)"
     elif _GEOHASH_BYTE_MAX < bits <= _GEOHASH_SHORT_MAX:
-        return 'GEOHASH(3c)'
+        return "GEOHASH(3c)"
     elif _GEOHASH_SHORT_MAX < bits <= _GEOHASH_INT_MAX:
-        return 'GEOHASH(6c)'
-    return f'GEOHASH(12c)'
+        return "GEOHASH(6c)"
+    return f"GEOHASH(12c)"
 
 
 def geohash_class(bits):
     if not isinstance(bits, int) or bits < 0 or bits > _GEOHASH_LONG_BITS:
-        raise ArgumentError(f'geohash precision must be int [0, {_GEOHASH_LONG_BITS}]')
+        raise sqlalchemy.exc.ArgumentError(
+            f"geohash precision must be int [0, {_GEOHASH_LONG_BITS}]"
+        )
     if 0 < bits <= _GEOHASH_BYTE_MAX:
         return GeohashByte
     elif _GEOHASH_BYTE_MAX < bits <= _GEOHASH_SHORT_MAX:
         return GeohashShort
     elif _GEOHASH_SHORT_MAX < bits <= _GEOHASH_INT_MAX:
         return GeohashInt
     return GeohashLong
 
 
-def quote_identifier(identifier: str):
-    if not identifier:
-        return None
-    first = 0
-    last = len(identifier)
-    if identifier[first] in _QUOTES:
-        first += 1
-    if identifier[last - 1] in _QUOTES:
-        last -= 1
-    return f'"{identifier[first:last]}"'
-
-
-class QDBTypeMixin(sqla.types.TypeDecorator):
-    __visit_name__ = 'QDBTypeMixin'
-    impl = sqla.types.String
+class QDBTypeMixin(sqlalchemy.types.TypeDecorator):
+    __visit_name__ = "QDBTypeMixin"
+    impl = sqlalchemy.types.String
     cache_ok = True
 
     @classmethod
     def matches_type_name(cls, type_name):
         return cls if type_name == cls.__visit_name__ else None
 
     def column_spec(self, column_name):
         return f"{quote_identifier(column_name)} {self.__visit_name__}"
 
     def compile(self, dialect=None):
         return self.__visit_name__
 
 
 class Boolean(QDBTypeMixin):
-    __visit_name__ = 'BOOLEAN'
-    impl = sqla.types.Boolean
+    __visit_name__ = "BOOLEAN"
+    impl = sqlalchemy.types.Boolean
     type_code = 1
 
 
 class Byte(QDBTypeMixin):
-    __visit_name__ = 'BYTE'
-    impl = sqla.types.Integer
+    __visit_name__ = "BYTE"
+    impl = sqlalchemy.types.Integer
     type_code = 2
 
 
 class Short(QDBTypeMixin):
-    __visit_name__ = 'SHORT'
+    __visit_name__ = "SHORT"
     type_code = 3
-    impl = sqla.types.Integer
+    impl = sqlalchemy.types.Integer
 
 
 class Char(QDBTypeMixin):
-    __visit_name__ = 'CHAR'
+    __visit_name__ = "CHAR"
     type_code = 4
 
 
 class Int(QDBTypeMixin):
-    __visit_name__ = 'INT'
+    __visit_name__ = "INT"
     type_code = 5
-    impl = sqla.types.Integer
+    impl = sqlalchemy.types.Integer
 
 
 class Long(QDBTypeMixin):
-    __visit_name__ = 'LONG'
+    __visit_name__ = "LONG"
     type_code = 6
-    impl = sqla.types.Integer
+    impl = sqlalchemy.types.Integer
 
 
 class Date(QDBTypeMixin):
-    __visit_name__ = 'DATE'
+    __visit_name__ = "DATE"
     type_code = 7
-    impl = sqla.types.Date
+    impl = sqlalchemy.types.Date
 
 
 class Timestamp(QDBTypeMixin):
-    __visit_name__ = 'TIMESTAMP'
+    __visit_name__ = "TIMESTAMP"
     type_code = 8
-    impl = sqla.types.DateTime
+    impl = sqlalchemy.types.DateTime
 
 
 class Float(QDBTypeMixin):
-    __visit_name__ = 'FLOAT'
+    __visit_name__ = "FLOAT"
     type_code = 9
-    impl = sqla.types.Float
+    impl = sqlalchemy.types.Float
 
 
 class Double(QDBTypeMixin):
-    __visit_name__ = 'DOUBLE'
+    __visit_name__ = "DOUBLE"
     type_code = 10
-    impl = sqla.types.Float
+    impl = sqlalchemy.types.Float
 
 
 class String(QDBTypeMixin):
-    __visit_name__ = 'STRING'
+    __visit_name__ = "STRING"
     type_code = 11
 
 
 class Symbol(QDBTypeMixin):
-    __visit_name__ = 'SYMBOL'
+    __visit_name__ = "SYMBOL"
     type_code = 12
 
 
 class Long256(QDBTypeMixin):
-    __visit_name__ = 'LONG256'
+    __visit_name__ = "LONG256"
     type_code = 13
 
 
 class GeohashByte(QDBTypeMixin):
     __visit_name__ = geohash_type_name(8)
     type_code = 14
 
@@ -192,15 +171,15 @@
 
 class GeohashLong(QDBTypeMixin):
     __visit_name__ = geohash_type_name(60)
     type_code = 17
 
 
 class UUID(QDBTypeMixin):
-    __visit_name__ = 'UUID'
+    __visit_name__ = "UUID"
     type_code = 19
 
 
 QUESTDB_TYPES = [
     Long256,
     Boolean,
     Byte,
@@ -228,17 +207,19 @@
     type_class = _TYPE_CACHE.get(type_name)
     if not type_class:
         for candidate_class in QUESTDB_TYPES:
             type_class = candidate_class.matches_type_name(type_name)
             if type_class:
                 _TYPE_CACHE[type_name] = type_class
                 break
-            elif 'GEOHASH' in type_name.upper() and '(' in type_name and ')' in type_name:
-                open_p = type_name.index('(')
-                close_p = type_name.index(')')
-                description = type_name[open_p + 1:close_p]
+            elif (
+                "GEOHASH" in type_name.upper() and "(" in type_name and ")" in type_name
+            ):
+                open_p = type_name.index("(")
+                close_p = type_name.index(")")
+                description = type_name[open_p + 1 : close_p]
                 g_size = int(description[:-1])
-                if description[-1] in ('C', 'c'):
+                if description[-1] in ("C", "c"):
                     g_size *= 5
                 type_class = geohash_class(g_size)
                 break
     return type_class
```

### Comparing `questdb-connect-1.0.6/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-1.0.8/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 1.0.6
-Summary: SqlAlchemy/Superset library.
+Version: 1.0.8
+Summary: SqlAlchemy library
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
+Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <a href="https://questdb.io/docs/" target="blank">
     <img alt="QuestDB Logo" src="https://questdb.io/img/questdb-logo-themed.svg" width="305px"/>
 </a>
@@ -34,29 +34,28 @@
 
 <a href="https://pypi.org/project/questdb-connect/">
     <img src="https://pypi.org/static/images/logo-small.2a411bc6.svg" alt="PyPi"/>
     https://pypi.org/project/questdb-connect/
 </a>
 <p></p>
 
-_Psycopg2_ is a widely used and trusted Python module for connecting to and working with PostgreSQL databases.
-It provides a comprehensive set of features for interacting with the PostgreSQL database system.
+_Psycopg2_ is a widely used and trusted Python module for connecting to, and working with, QuestDB and other
+PostgreSQL databases.
 
-_SQLAlchemy_ is an open-source SQL toolkit and ORM library for Python. It provides a high-level API for
-communicating with relational databases, including schema creation and modification, an SQL expression
-language, and database connection management. The ORM layer abstracts away the complexities of the
-database, allowing developers to work with Python objects instead of raw SQL statements.
-
-_Apache Superset_ is a popular open-source business intelligence web application that enables users to
-visualize and explore data through customizable dashboards and reports. It provides a rich set of data
-visualizations, including charts, tables, and maps.
+_SQLAlchemy_ is a SQL toolkit and ORM library for Python. It provides a high-level API for communicating with 
+relational databases, including schema creation and modification. The ORM layer abstracts away the complexities 
+of the database, allowing developers to work with Python objects instead of raw SQL statements.
+
+_Apache Superset_ is an open-source business intelligence web application that enables users to visualize and 
+explore data through customizable dashboards and reports. It provides a rich set of data visualizations, including 
+charts, tables, and maps.
 
 ## Requirements
 
-* **Python from 3.8.x to 3.10.x** (superset itself use version _3.9.x_)
+* **Python from 3.9 to 3.11** (superset itself use version _3.9.x_)
 * **Psycopg2** `('psycopg2-binary~=2.9.6')`
 * **SQLAlchemy** `('SQLAlchemy<=1.4.47')`
 
 You need to install these packages because questdb-connect depends on them.
 
 ## Installation
 
@@ -64,16 +63,22 @@
 
 ```shell
 pip install questdb-connect
 ```
 
 ## SQLALchemy Sample Usage
 
-Use the QuestDB dialect by specifying it in your SQLAlchemy connection string,
-from that point on use SQLAlchemy:
+Use the QuestDB dialect by specifying it in your SQLAlchemy connection string:
+
+```shell
+questdb://admin:quest@localhost:8812/main
+questdb://admin:quest@host.docker.internal:8812/main
+```
+
+From that point on use standard SQLAlchemy:
 
 ```python
 import datetime
 import os
 
 os.environ.setdefault('SQLALCHEMY_SILENCE_UBER_WARNING', '1')
 
@@ -109,17 +114,18 @@
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Superset Installation
 
-<img alt="QuestDB Logo" src="https://github.com/questdb/questdb-connect/blob/main/docs/superset.png"/>
+<a href="https://superset.apache.org/docs/installation/installing-superset-from-scratch/" target="blank">
+    <img alt="Apache Superset" src="https://github.com/questdb/questdb-connect/blob/main/docs/superset.png"/>
+</a>
 
-Follow the instructions available here
-[https://superset.apache.org/docs/installation/installing-superset-from-scratch/](https://superset.apache.org/docs/installation/installing-superset-from-scratch/).
+Follow the instructions available [here](https://superset.apache.org/docs/installation/installing-superset-from-scratch/).
 
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
 please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md)
 if you would like to push a PR.
```

### Comparing `questdb-connect-1.0.6/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-1.0.8/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,27 @@
 src/examples/__init__.py
 src/examples/hello_world.py
 src/examples/psycopg2_connect.py
 src/examples/server_utilisation.py
 src/examples/sqlalchemy_orm.py
 src/examples/sqlalchemy_raw.py
 src/questdb_connect/__init__.py
+src/questdb_connect/common.py
+src/questdb_connect/compilers.py
 src/questdb_connect/dialect.py
-src/questdb_connect/function_names.py
+src/questdb_connect/identifier_preparer.py
+src/questdb_connect/inspector.py
+src/questdb_connect/keywords_functions.py
+src/questdb_connect/table_engine.py
 src/questdb_connect/types.py
 src/questdb_connect.egg-info/PKG-INFO
 src/questdb_connect.egg-info/SOURCES.txt
 src/questdb_connect.egg-info/dependency_links.txt
 src/questdb_connect.egg-info/entry_points.txt
 src/questdb_connect.egg-info/requires.txt
 src/questdb_connect.egg-info/top_level.txt
-src/superset_ext/__init__.py
-src/superset_ext/db_engine_specs/__init__.py
-src/superset_ext/db_engine_specs/questdb.py
+src/superset/__init__.py
+src/superset/db_engine_specs/__init__.py
+src/superset/db_engine_specs/questdb.py
 tests/test_dialect.py
-tests/test_superset.py
+tests/test_examples.py
 tests/test_types.py
```

### Comparing `questdb-connect-1.0.6/src/superset_ext/__init__.py` & `questdb-connect-1.0.8/src/superset/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.6/src/superset_ext/db_engine_specs/__init__.py` & `questdb-connect-1.0.8/src/superset/db_engine_specs/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.6/src/superset_ext/db_engine_specs/questdb.py` & `questdb-connect-1.0.8/src/superset/db_engine_specs/questdb.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,206 +1,198 @@
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
 #
-#     ___                  _   ____  ____
-#    / _ \ _   _  ___  ___| |_|  _ \| __ )
-#   | | | | | | |/ _ \/ __| __| | | |  _ \
-#   | |_| | |_| |  __/\__ \ |_| |_| | |_) |
-#    \__\_\\__,_|\___||___/\__|____/|____/
-#
-#  Copyright (c) 2014-2019 Appsicle
-#  Copyright (c) 2019-2023 QuestDB
-#
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#  http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
 import re
 from datetime import datetime
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Set
 
+import questdb_connect.types as qdbc_types
 from flask_babel import gettext as __
-from marshmallow import Schema, fields
-from sqlalchemy.engine.interfaces import Dialect
-from sqlalchemy.sql import text
+from marshmallow import fields, Schema
+from sqlalchemy.engine.base import Engine
+from sqlalchemy.engine.reflection import Inspector
 from sqlalchemy.types import TypeEngine
+
 from superset.db_engine_specs.base import (
     BaseEngineSpec,
     BasicParametersMixin,
     BasicParametersType,
 )
+from superset.models.core import Database
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
-from questdb_connect import remove_public_schema
-from questdb_connect import types as questdb_types
-from questdb_connect.dialect import connection_uri
-from questdb_connect.function_names import FUNCTION_NAMES
-
-# Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
-# https://superset.apache.org/docs/databases/installing-database-drivers
-# https://preset.io/blog/building-database-connector/
-# https://preset.io/blog/improving-apache-superset-integration-database-sqlalchemy/
-
-
-class QDBParametersSchema(Schema):
-    username = fields.String(allow_none=True, description=__("user"))
-    password = fields.String(allow_none=True, description=__("password"))
-    host = fields.String(required=True, description=__("host"))
-    port = fields.Integer(allow_none=True, description=__("port"))
-    database = fields.String(allow_none=True, description=__("database"))
 
+class QuestDbParametersSchema(Schema):
+    username = fields.String(
+        description=__("user"),
+        dump_default="admin",
+        load_default="admin",
+    )
+    password = fields.String(
+        description=__("password"),
+        dump_default="quest",
+        load_default="quest",
+    )
+    host = fields.String(
+        description=__("host"),
+        dump_default="host.docker.internal",
+        load_default="host.docker.internal",
+    )
+    port = fields.Integer(
+        description=__("port"),
+        dump_default="8812",
+        load_default="8812",
+    )
+    database = fields.String(
+        description=__("database"),
+        dump_default="main",
+        load_default="main",
+    )
 
-class QDBEngineSpec(BaseEngineSpec, BasicParametersMixin):
+
+class QuestDbEngineSpec(BaseEngineSpec, BasicParametersMixin):
     engine = "questdb"
-    engine_name = "QuestDB Connect"
+    engine_name = "QuestDB"
     default_driver = "psycopg2"
     encryption_parameters = {"sslmode": "prefer"}
     sqlalchemy_uri_placeholder = "questdb://user:password@host:port/database"
-    parameters_schema = QDBParametersSchema()
+    parameters_schema = QuestDbParametersSchema()
     time_groupby_inline = False
     allows_hidden_cc_in_orderby = True
     time_secondary_columns = True
     try_remove_schema_from_table_name = True
     max_column_name_length = 120
     supports_dynamic_schema = False
-    top_keywords = {}
+    top_keywords: Set[str] = set({})
     # https://en.wikipedia.org/wiki/ISO_8601#Durations
     # https://questdb.io/docs/reference/function/date-time/#date_trunc
     _time_grain_expressions = {
         None: "{col}",
-        "PT1S": "date_trunc('second', {col})",
-        "PT1M": "date_trunc('minute', {col})",
-        "PT1H": "date_trunc('hour', {col})",
-        "P1D": "date_trunc('day', {col})",
-        "P1W": "date_trunc('week', {col})",
-        "P1M": "date_trunc('month', {col})",
-        "P1Y": "date_trunc('year', {col})",
-        "P3M": "date_trunc('quarter', {col})",
+        "PT1S": "DATE_TRUNC('second', {col})",
+        "PT1M": "DATE_TRUNC('minute', {col})",
+        "PT1H": "DATE_TRUNC('hour', {col})",
+        "P1D": "DATE_TRUNC('day', {col})",
+        "P1W": "DATE_TRUNC('week', {col})",
+        "P1M": "DATE_TRUNC('month', {col})",
+        "P1Y": "DATE_TRUNC('year', {col})",
+        "P3M": "DATE_TRUNC('quarter', {col})",
     }
     column_type_mappings = (
         (
             re.compile("^LONG256", re.IGNORECASE),
-            questdb_types.Long256,
+            qdbc_types.Long256,
             GenericDataType.STRING,
         ),
         (
             re.compile("^BOOLEAN", re.IGNORECASE),
-            questdb_types.Boolean,
+            qdbc_types.Boolean,
             GenericDataType.BOOLEAN,
         ),
         (
             re.compile("^BYTE", re.IGNORECASE),
-            questdb_types.Byte,
+            qdbc_types.Byte,
             GenericDataType.NUMERIC,
         ),
         (
             re.compile("^SHORT", re.IGNORECASE),
-            questdb_types.Short,
+            qdbc_types.Short,
             GenericDataType.NUMERIC,
         ),
-        (re.compile("^INT", re.IGNORECASE), questdb_types.Int, GenericDataType.NUMERIC),
+        (re.compile("^INT", re.IGNORECASE), qdbc_types.Int, GenericDataType.NUMERIC),
         (
             re.compile("^LONG", re.IGNORECASE),
-            questdb_types.Long,
+            qdbc_types.Long,
             GenericDataType.NUMERIC,
         ),
         (
             re.compile("^FLOAT", re.IGNORECASE),
-            questdb_types.Float,
+            qdbc_types.Float,
             GenericDataType.NUMERIC,
         ),
         (
             re.compile("^DOUBLE'", re.IGNORECASE),
-            questdb_types.Double,
+            qdbc_types.Double,
             GenericDataType.NUMERIC,
         ),
         (
             re.compile("^SYMBOL", re.IGNORECASE),
-            questdb_types.Symbol,
+            qdbc_types.Symbol,
             GenericDataType.STRING,
         ),
         (
             re.compile("^STRING", re.IGNORECASE),
-            questdb_types.String,
+            qdbc_types.String,
             GenericDataType.STRING,
         ),
         (
             re.compile("^UUID", re.IGNORECASE),
-            questdb_types.UUID,
+            qdbc_types.UUID,
             GenericDataType.STRING,
         ),
         (
             re.compile("^CHAR", re.IGNORECASE),
-            questdb_types.Char,
+            qdbc_types.Char,
             GenericDataType.STRING,
         ),
         (
             re.compile("^TIMESTAMP", re.IGNORECASE),
-            questdb_types.Timestamp,
+            qdbc_types.Timestamp,
             GenericDataType.TEMPORAL,
         ),
         (
             re.compile("^DATE", re.IGNORECASE),
-            questdb_types.Date,
+            qdbc_types.Date,
             GenericDataType.TEMPORAL,
         ),
         (
             re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE),
-            questdb_types.GeohashLong,
+            qdbc_types.GeohashLong,
             GenericDataType.STRING,
         ),
     )
 
     @classmethod
     def build_sqlalchemy_uri(
         cls,
         parameters: BasicParametersType,
         encrypted_extra: Optional[Dict[str, str]] = None,
     ) -> str:
-        return connection_uri(
-            parameters.get("host"),
-            parameters.get("port"),
-            parameters.get("username"),
-            parameters.get("password"),
-            parameters.get("database"),
-        )
-
-    @classmethod
-    def get_default_schema_for_query(cls, database, query) -> Optional[str]:
-        return "public"
-
-    @classmethod
-    def get_text_clause(cls, clause):
-        """SQLAlchemy wrapper to ensure text clauses are escaped properly
-        :param clause: string clause with potentially unescaped characters
-        :return: text clause with escaped characters
-        """
-        if cls.allows_escaped_colons:
-            clause = clause.replace(":", "\\:")
-        return text(remove_public_schema(clause))
+        host = parameters.get("host")
+        port = parameters.get("port")
+        username = parameters.get("username")
+        password = parameters.get("password")
+        database = parameters.get("database")
+        return f"questdb://{username}:{password}@{host}:{port}/{database}"
 
     @classmethod
     def epoch_to_dttm(cls) -> str:
         """SQL expression that converts epoch (seconds) to datetime that can be used
         in a query. The reference column should be denoted as `{col}` in the return
         expression, e.g. "FROM_UNIXTIME({col})"
         :return: SQL Expression
         """
         return "{col} * 1000000"
 
     @classmethod
     def convert_dttm(
-        cls, target_type: str, dttm: datetime, *_args, **_kwargs
+        cls, target_type: str, dttm: datetime, db_extra: Optional[Dict[str, Any]] = None
     ) -> Optional[str]:
         """Convert a Python `datetime` object to a SQL expression.
         :param target_type: The target type of expression
         :param dttm: The datetime object
         :return: The SQL expression
         """
         type_u = target_type.upper()
@@ -230,31 +222,33 @@
     ) -> Optional[utils.ColumnSpec]:
         """Get generic type related specs regarding a native column type.
         :param native_type: Native database type
         :param db_extra: The database extra object
         :param source: Type coming from the database table or cursor description
         :return: ColumnSpec object
         """
-        sqla_type = questdb_types.resolve_type_from_name(native_type)
+        sqla_type = qdbc_types.resolve_type_from_name(native_type)
         if not sqla_type:
             return BaseEngineSpec.get_column_spec(native_type, db_extra, source)
         name_u = sqla_type.__visit_name__
-        generic_type = None
+        generic_type = GenericDataType.STRING
         if name_u == "BOOLEAN":
             generic_type = GenericDataType.BOOLEAN
         elif name_u in ("BYTE", "SHORT", "INT", "LONG", "FLOAT", "DOUBLE"):
             generic_type = GenericDataType.NUMERIC
         elif name_u in ("SYMBOL", "STRING", "CHAR", "LONG256", "UUID"):
             generic_type = GenericDataType.STRING
         elif name_u in ("DATE", "TIMESTAMP"):
             generic_type = GenericDataType.TEMPORAL
         elif "GEOHASH" in name_u and "(" in name_u and ")" in name_u:
             generic_type = GenericDataType.STRING
         return utils.ColumnSpec(
-            sqla_type, generic_type, generic_type == GenericDataType.TEMPORAL
+            sqla_type,
+            generic_type,
+            generic_type == GenericDataType.TEMPORAL,
         )
 
     @classmethod
     def get_sqla_column_type(
         cls,
         native_type: Optional[str],
         db_extra: Optional[Dict[str, Any]] = None,
@@ -262,37 +256,22 @@
     ) -> Optional[TypeEngine]:
         """Converts native database type to sqlalchemy column type.
         :param native_type: Native database type
         :param db_extra: The database extra object
         :param source: Type coming from the database table or cursor description
         :return: ColumnSpec object
         """
-        return questdb_types.resolve_type_from_name(native_type).impl
+        return qdbc_types.resolve_type_from_name(native_type).impl
 
     @classmethod
-    def column_datatype_to_string(
+    def select_star(  # pylint: disable=too-many-arguments
         cls,
-        sqla_column_type: TypeEngine,
-        dialect: Dialect,
-    ) -> str:
-        """Convert sqlalchemy column type to string representation.
-        By default, removes collation and character encoding info to avoid
-        unnecessarily long datatypes.
-        :param sqla_column_type: SqlAlchemy column type
-        :param dialect: Sqlalchemy dialect
-        :return: Compiled column type
-        """
-        return sqla_column_type.copy().compile(dialect=dialect)
-
-    @classmethod
-    def select_star(
-        cls,
-        database,
+        database: Database,
         table_name: str,
-        engine,
+        engine: Engine,
         schema: Optional[str] = None,
         limit: int = 100,
         show_cols: bool = False,
         indent: bool = True,
         latest_partition: bool = True,
         cols: Optional[List[Dict[str, Any]]] = None,
     ) -> str:
@@ -317,22 +296,18 @@
             show_cols,
             indent,
             latest_partition,
             cols,
         )
 
     @classmethod
-    def get_function_names(cls, database) -> List[str]:
-        """Get a list of function names that are able to be called on the database.
-        Used for SQL Lab autocomplete.
-        :param database: The database to get functions for
-        :return: A list of function names usable in the database
-        """
-        return FUNCTION_NAMES
-
-    @classmethod
     def get_allow_cost_estimate(cls, extra: Dict[str, Any]) -> bool:
         return False
 
     @classmethod
-    def get_view_names(cls, database, inspector, schema: Optional[str]):
-        return []
+    def get_view_names(
+        cls,
+        database: Database,
+        inspector: Inspector,
+        schema: Optional[str],
+    ) -> Set[str]:
+        return set({})
```

### Comparing `questdb-connect-1.0.6/tests/test_dialect.py` & `questdb-connect-1.0.8/tests/test_dialect.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import datetime
 
+import questdb_connect as qdbc
 import sqlalchemy as sqla
-from questdb_connect import types
 from sqlalchemy.orm import Session
 
 from tests.conftest import ALL_TYPES_TABLE_NAME, collect_select_all, collect_select_all_raw_connection
 
 
 def test_insert(test_engine, test_model):
     with test_engine.connect() as conn:
@@ -108,29 +108,29 @@
     finally:
         if session:
             session.close()
     metadata = sqla.MetaData()
     table = sqla.Table(ALL_TYPES_TABLE_NAME, metadata, autoload_with=test_engine)
     table_columns = str([(col.name, col.type, col.primary_key) for col in table.columns])
     assert table_columns == str([
-        ('col_boolean', types.Boolean(), False),
-        ('col_byte', types.Byte(), False),
-        ('col_short', types.Short(), False),
-        ('col_int', types.Int(), False),
-        ('col_long', types.Long(), False),
-        ('col_float', types.Float(), False),
-        ('col_double', types.Double(), False),
-        ('col_symbol', types.Symbol(), False),
-        ('col_string', types.String(), False),
-        ('col_char', types.Char(), False),
-        ('col_uuid', types.UUID(), False),
-        ('col_date', types.Date(), False),
-        ('col_ts', types.Timestamp(), True),
-        ('col_geohash', types.GeohashInt(), False),
-        ('col_long256', types.Long256(), False)
+        ('col_boolean', qdbc.Boolean(), False),
+        ('col_byte', qdbc.Byte(), False),
+        ('col_short', qdbc.Short(), False),
+        ('col_int', qdbc.Int(), False),
+        ('col_long', qdbc.Long(), False),
+        ('col_float', qdbc.Float(), False),
+        ('col_double', qdbc.Double(), False),
+        ('col_symbol', qdbc.Symbol(), False),
+        ('col_string', qdbc.String(), False),
+        ('col_char', qdbc.Char(), False),
+        ('col_uuid', qdbc.UUID(), False),
+        ('col_date', qdbc.Date(), False),
+        ('col_ts', qdbc.Timestamp(), True),
+        ('col_geohash', qdbc.GeohashInt(), False),
+        ('col_long256', qdbc.Long256(), False)
     ])
 
 
 def test_multiple_insert(test_engine, test_model):
     now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
     now_date = now.date()
     session = Session(test_engine)
@@ -214,7 +214,19 @@
         session.bulk_save_objects(models)
         session.commit()
         assert collect_select_all(session, expected_rows=num_rows) == expected
     finally:
         if session:
             session.close()
         assert collect_select_all_raw_connection(test_engine, expected_rows=num_rows) == expected
+
+
+def test_functions(test_engine):
+    with test_engine.connect() as conn:
+        expected = [row[0] for row in conn.execute("SELECT name FROM functions()").fetchall()]
+        assert qdbc.get_functions_list() == expected
+
+
+def test_keywords(test_engine):
+    with test_engine.connect() as conn:
+        expected = [row[0] for row in conn.execute("SELECT keyword FROM keywords()").fetchall()]
+        assert qdbc.get_keywords_list() == expected
```

