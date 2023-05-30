# Comparing `tmp/trino-0.325.0.tar.gz` & `tmp/trino-0.326.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trino-0.325.0.tar", last modified: Fri May 26 07:12:43 2023, max compression
+gzip compressed data, was "trino-0.326.0.tar", last modified: Tue May 30 12:40:14 2023, max compression
```

## Comparing `trino-0.325.0.tar` & `trino-0.326.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:12:43.769862 trino-0.325.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-26 07:12:27.000000 trino-0.325.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-26 07:12:43.769862 trino-0.325.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-05-26 07:12:27.000000 trino-0.325.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-26 07:12:43.769862 trino-0.325.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3532 2023-05-26 07:12:27.000000 trino-0.325.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:12:43.765862 trino-0.325.0/trino/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-26 07:12:30.000000 trino-0.325.0/trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-26 07:12:27.000000 trino-0.325.0/trino/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    46886 2023-05-26 07:12:27.000000 trino-0.325.0/trino/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-26 07:12:27.000000 trino-0.325.0/trino/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25846 2023-05-26 07:12:27.000000 trino-0.325.0/trino/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-26 07:12:27.000000 trino-0.325.0/trino/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-26 07:12:27.000000 trino-0.325.0/trino/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:12:43.769862 trino-0.325.0/trino/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-26 07:12:27.000000 trino-0.325.0/trino/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-26 07:12:27.000000 trino-0.325.0/trino/sqlalchemy/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-05-26 07:12:27.000000 trino-0.325.0/trino/sqlalchemy/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-05-26 07:12:27.000000 trino-0.325.0/trino/sqlalchemy/dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-26 07:12:27.000000 trino-0.325.0/trino/sqlalchemy/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-26 07:12:27.000000 trino-0.325.0/trino/sqlalchemy/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-26 07:12:27.000000 trino-0.325.0/trino/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:12:43.769862 trino-0.325.0/trino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-26 07:12:43.000000 trino-0.325.0/trino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-26 07:12:43.000000 trino-0.325.0/trino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:12:43.000000 trino-0.325.0/trino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-26 07:12:43.000000 trino-0.325.0/trino.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-26 07:12:43.000000 trino-0.325.0/trino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 07:12:43.000000 trino-0.325.0/trino.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:40:14.982991 trino-0.326.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 12:40:00.000000 trino-0.326.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-30 12:40:14.982991 trino-0.326.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-05-30 12:40:00.000000 trino-0.326.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-30 12:40:14.982991 trino-0.326.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3532 2023-05-30 12:40:00.000000 trino-0.326.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:40:14.982991 trino-0.326.0/trino/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-30 12:40:02.000000 trino-0.326.0/trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-30 12:40:00.000000 trino-0.326.0/trino/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46886 2023-05-30 12:40:00.000000 trino-0.326.0/trino/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-30 12:40:00.000000 trino-0.326.0/trino/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-05-30 12:40:00.000000 trino-0.326.0/trino/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-30 12:40:00.000000 trino-0.326.0/trino/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-30 12:40:00.000000 trino-0.326.0/trino/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:40:14.982991 trino-0.326.0/trino/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-30 12:40:00.000000 trino-0.326.0/trino/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-30 12:40:00.000000 trino-0.326.0/trino/sqlalchemy/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-05-30 12:40:00.000000 trino-0.326.0/trino/sqlalchemy/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-05-30 12:40:00.000000 trino-0.326.0/trino/sqlalchemy/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-30 12:40:00.000000 trino-0.326.0/trino/sqlalchemy/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-30 12:40:00.000000 trino-0.326.0/trino/sqlalchemy/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-30 12:40:00.000000 trino-0.326.0/trino/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:40:14.982991 trino-0.326.0/trino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-30 12:40:14.000000 trino-0.326.0/trino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-30 12:40:14.000000 trino-0.326.0/trino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:40:14.000000 trino-0.326.0/trino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-30 12:40:14.000000 trino-0.326.0/trino.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-30 12:40:14.000000 trino-0.326.0/trino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 12:40:14.000000 trino-0.326.0/trino.egg-info/top_level.txt
```

### Comparing `trino-0.325.0/LICENSE` & `trino-0.326.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/PKG-INFO` & `trino-0.326.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trino
-Version: 0.325.0
+Version: 0.326.0
 Summary: Client for the Trino distributed SQL Engine
 Home-page: https://github.com/trinodb/trino-python-client
 Author: Trino Team
 Author-email: python-client@trino.io
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trino-0.325.0/README.md` & `trino-0.326.0/README.md`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/setup.py` & `trino-0.326.0/setup.py`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/trino/__init__.py` & `trino-0.326.0/trino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from . import auth, client, constants, dbapi, exceptions, logging
 
 __all__ = ['auth', 'dbapi', 'client', 'constants', 'exceptions', 'logging']
 
-__version__ = "0.325.0"
+__version__ = "0.326.0"
```

### Comparing `trino-0.325.0/trino/auth.py` & `trino-0.326.0/trino/auth.py`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/trino/client.py` & `trino-0.326.0/trino/client.py`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/trino/constants.py` & `trino-0.326.0/trino/constants.py`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/trino/dbapi.py` & `trino-0.326.0/trino/dbapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,20 +279,21 @@
         value = must_use_legacy_prepared_statements.get((self.host, self.port))
         if value is None:
             try:
                 query = trino.client.TrinoQuery(
                     self._create_request(),
                     query="EXECUTE IMMEDIATE 'SELECT 1'")
                 query.execute()
+                value = False
             except Exception as e:
                 logger.warning(
                     "EXECUTE IMMEDIATE not available for %s:%s; defaulting to legacy prepared statements (%s)",
                     self.host, self.port, e)
                 value = True
-                must_use_legacy_prepared_statements.put((self.host, self.port), value)
+            must_use_legacy_prepared_statements.put((self.host, self.port), value)
         return value
 
 
 class DescribeOutput(NamedTuple):
     name: str
     catalog: str
     schema: str
```

### Comparing `trino-0.325.0/trino/exceptions.py` & `trino-0.326.0/trino/exceptions.py`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/trino/logging.py` & `trino-0.326.0/trino/logging.py`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/trino/sqlalchemy/__init__.py` & `trino-0.326.0/trino/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/trino/sqlalchemy/compiler.py` & `trino-0.326.0/trino/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/trino/sqlalchemy/datatype.py` & `trino-0.326.0/trino/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/trino/sqlalchemy/dialect.py` & `trino-0.326.0/trino/sqlalchemy/dialect.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         if "client_tags" in url.query:
             kwargs["client_tags"] = json.loads(unquote_plus(url.query["client_tags"]))
 
         if "legacy_primitive_types" in url.query:
             kwargs["legacy_primitive_types"] = json.loads(unquote_plus(url.query["legacy_primitive_types"]))
 
         if "legacy_prepared_statements" in url.query:
-            kwargs["legacy_prepared_statements"] = unquote_plus(url.query["legacy_prepared_statements"])
+            kwargs["legacy_prepared_statements"] = json.loads(unquote_plus(url.query["legacy_prepared_statements"]))
 
         if "verify" in url.query:
             kwargs["verify"] = json.loads(unquote_plus(url.query["verify"]))
 
         if "roles" in url.query:
             kwargs["roles"] = json.loads(url.query["roles"])
```

### Comparing `trino-0.325.0/trino/sqlalchemy/error.py` & `trino-0.326.0/trino/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/trino/sqlalchemy/util.py` & `trino-0.326.0/trino/sqlalchemy/util.py`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/trino/transaction.py` & `trino-0.326.0/trino/transaction.py`

 * *Files identical despite different names*

### Comparing `trino-0.325.0/trino.egg-info/PKG-INFO` & `trino-0.326.0/trino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trino
-Version: 0.325.0
+Version: 0.326.0
 Summary: Client for the Trino distributed SQL Engine
 Home-page: https://github.com/trinodb/trino-python-client
 Author: Trino Team
 Author-email: python-client@trino.io
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trino-0.325.0/trino.egg-info/SOURCES.txt` & `trino-0.326.0/trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

