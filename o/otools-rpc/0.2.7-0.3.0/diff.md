# Comparing `tmp/otools-rpc-0.2.7.tar.gz` & `tmp/otools-rpc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otools-rpc-0.2.7.tar", last modified: Wed May 24 12:28:39 2023, max compression
+gzip compressed data, was "otools-rpc-0.3.0.tar", last modified: Tue May 30 13:54:57 2023, max compression
```

## Comparing `otools-rpc-0.2.7.tar` & `otools-rpc-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-24 12:28:39.647321 otools-rpc-0.2.7/
--rw-r--r--   0 opennet   (1000) opennet   (1000)     1074 2023-05-22 13:36:09.000000 otools-rpc-0.2.7/LICENSE.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     3458 2023-05-24 12:28:39.647321 otools-rpc-0.2.7/PKG-INFO
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     2837 2023-05-23 14:35:04.000000 otools-rpc-0.2.7/README.md
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-24 12:28:39.647321 otools-rpc-0.2.7/otools_rpc/
--rw-r--r--   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:36:09.000000 otools-rpc-0.2.7/otools_rpc/__init__.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-24 12:28:39.647321 otools-rpc-0.2.7/otools_rpc/db_manager/
--rw-r--r--   0 opennet   (1000) opennet   (1000)       38 2023-05-23 14:35:04.000000 otools-rpc-0.2.7/otools_rpc/db_manager/__init__.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     1115 2023-05-23 14:35:04.000000 otools-rpc-0.2.7/otools_rpc/db_manager/database_utils.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-24 12:28:39.647321 otools-rpc-0.2.7/otools_rpc/external_api/
--rw-r--r--   0 opennet   (1000) opennet   (1000)       37 2023-05-22 13:36:09.000000 otools-rpc-0.2.7/otools_rpc/external_api/__init__.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)      959 2023-05-22 13:36:09.000000 otools-rpc-0.2.7/otools_rpc/external_api/common.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     4812 2023-05-22 13:47:55.000000 otools-rpc-0.2.7/otools_rpc/external_api/environment.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     6390 2023-05-24 12:25:11.000000 otools-rpc-0.2.7/otools_rpc/external_api/recordset.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-24 12:28:39.647321 otools-rpc-0.2.7/otools_rpc.egg-info/
--rw-r--r--   0 opennet   (1000) opennet   (1000)     3458 2023-05-24 12:28:39.000000 otools-rpc-0.2.7/otools_rpc.egg-info/PKG-INFO
--rw-r--r--   0 opennet   (1000) opennet   (1000)      442 2023-05-24 12:28:39.000000 otools-rpc-0.2.7/otools_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 opennet   (1000) opennet   (1000)        1 2023-05-24 12:28:39.000000 otools-rpc-0.2.7/otools_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 opennet   (1000) opennet   (1000)       63 2023-05-24 12:28:39.000000 otools-rpc-0.2.7/otools_rpc.egg-info/requires.txt
--rw-r--r--   0 opennet   (1000) opennet   (1000)       11 2023-05-24 12:28:39.000000 otools-rpc-0.2.7/otools_rpc.egg-info/top_level.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)       38 2023-05-24 12:28:39.647321 otools-rpc-0.2.7/setup.cfg
--rw-r--r--   0 opennet   (1000) opennet   (1000)     1045 2023-05-24 12:26:46.000000 otools-rpc-0.2.7/setup.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-30 13:54:57.795054 otools-rpc-0.3.0/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1326 2023-05-30 13:44:29.000000 otools-rpc-0.3.0/LICENSE.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     4072 2023-05-30 13:54:57.795054 otools-rpc-0.3.0/PKG-INFO
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     3450 2023-05-30 13:44:29.000000 otools-rpc-0.3.0/README.md
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-30 13:54:57.791054 otools-rpc-0.3.0/otools_rpc/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:36:09.000000 otools-rpc-0.3.0/otools_rpc/__init__.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-30 13:54:57.795054 otools-rpc-0.3.0/otools_rpc/db_manager/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       38 2023-05-30 12:59:41.000000 otools-rpc-0.3.0/otools_rpc/db_manager/__init__.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1168 2023-05-30 13:44:29.000000 otools-rpc-0.3.0/otools_rpc/db_manager/database_utils.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-30 13:54:57.795054 otools-rpc-0.3.0/otools_rpc/external_api/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       37 2023-05-22 13:36:09.000000 otools-rpc-0.3.0/otools_rpc/external_api/__init__.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1943 2023-05-30 13:50:43.000000 otools-rpc-0.3.0/otools_rpc/external_api/common.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     5083 2023-05-30 13:50:43.000000 otools-rpc-0.3.0/otools_rpc/external_api/environment.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     6943 2023-05-30 13:50:43.000000 otools-rpc-0.3.0/otools_rpc/external_api/recordset.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-30 13:54:57.795054 otools-rpc-0.3.0/otools_rpc.egg-info/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     4072 2023-05-30 13:54:57.000000 otools-rpc-0.3.0/otools_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 opennet   (1000) opennet   (1000)      442 2023-05-30 13:54:57.000000 otools-rpc-0.3.0/otools_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)        1 2023-05-30 13:54:57.000000 otools-rpc-0.3.0/otools_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       63 2023-05-30 13:54:57.000000 otools-rpc-0.3.0/otools_rpc.egg-info/requires.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       11 2023-05-30 13:54:57.000000 otools-rpc-0.3.0/otools_rpc.egg-info/top_level.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)       38 2023-05-30 13:54:57.795054 otools-rpc-0.3.0/setup.cfg
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1047 2023-05-30 13:50:43.000000 otools-rpc-0.3.0/setup.py
```

### Comparing `otools-rpc-0.2.7/README.md` & `otools-rpc-0.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,46 @@
+Metadata-Version: 2.1
+Name: otools-rpc
+Version: 0.3.0
+Summary: A tool to interact with Odoo's external API.
+Home-page: https://github.com/MrFaBemol/otools-rpc
+Author: Gautier Casabona
+Author-email: gcasabona.pro@gmail.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.txt
+
 # otools-rpc
 
 [![Version](https://img.shields.io/pypi/v/otools-rpc?color=blue&label=version)](https://pypi.org/project/otools-rpc/)
-[![Status](https://img.shields.io/pypi/status/otools-rpc?color=orange.svg)](https://pypi.org/project/otools-rpc/)
+[![LastCommit](https://img.shields.io/github/last-commit/MrFaBemol/otools-rpc?color=green)](https://en.wikipedia.org/wiki/MIT_License)
+[![Status](https://img.shields.io/pypi/status/otools-rpc?color=orange)](https://pypi.org/project/otools-rpc/)
+[![License](https://img.shields.io/github/license/MrFaBemol/otools-rpc?color=blue)](https://en.wikipedia.org/wiki/MIT_License)
+[![Downloads](https://img.shields.io/pypi/dm/otools-rpc?color=blue)](https://pypi.org/project/otools-rpc/)
+
+
+
+
+
 
 otools-rpc is a Python package for interacting with the Odoo ERP system through XML-RPC requests. It provides a convenient way to communicate with Odoo and perform various operations. Please note that the package is currently in the testing/alpha phase, and further improvements and updates are expected.
 
 ## Features
 
 [//]: # (### Environnement Class)
 
-The `Environnement` class represents the environment for interacting with the Odoo ERP system. It provides the following features:
+The `Environment` class represents the environment for interacting with the Odoo ERP system. It provides the following features:
 
 - Authentication: Authenticate with the Odoo system using username and password.
 - Access Models: Access different models (tables) in the Odoo system.
 - Caching: Caching mechanism to improve performance.
 - Logging: Logging capabilities with customizable log levels.
 
 ## Installation
@@ -81,14 +108,19 @@
 
 dbmanager = DBManager(url, master_password)
 
 #Return list of all the available DB in your Odoo ENV
 dbmanager.dbobject.list()
 
 #Duplicating my_odoo to my_new_odoo
-db.manager.duplicate(db='my_odoo', new_name="my_new_odoo")
+dbmanager.duplicate(db='my_odoo', new_name="my_new_odoo")
 
 #Deleting my_new_odoo
-db.manager.drop(db='my_new_odoo')
+dbmanager.drop(db='my_new_odoo')
 ```
 
 More details are coming soon...
+
+
+![Stars](https://img.shields.io/github/stars/MrFaBemol/otools-rpc?style=social)
+![Watchers](https://img.shields.io/github/watchers/MrFaBemol/otools-rpc?style=social)
+![Forks](https://img.shields.io/github/forks/MrFaBemol/otools-rpc?style=social)
```

### Comparing `otools-rpc-0.2.7/otools_rpc/db_manager/database_utils.py` & `otools-rpc-0.3.0/otools_rpc/db_manager/database_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,8 +27,10 @@
     def duplicate(self, db, new_name):
         res = requests.post(self._duplicate_url, data={'master_pwd': self._password, 'name': db, 'new_name': new_name})
         return res
     
     def drop(self, db):
         res = requests.post(self._drop_url, data={'master_pwd': self._password, 'name': db})
         return res
-    
+
+    def list(self):
+        return self.dbobject.list()
```

### Comparing `otools-rpc-0.2.7/otools_rpc/external_api/environment.py` & `otools-rpc-0.3.0/otools_rpc/external_api/environment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 import sys
 import xmlrpc.client
 import re
 import copy
 from typing import Union
-from loguru import logger
+from loguru import logger as loguru_logger
 from .recordset import RecordSet
+from .common import frozendict
 
 
 class Environment(dict):
     # Todo: Add a cache system
 
-    def __init__(self, url: str, username: str, password: str, db: str = None, auto_auth: bool = True, log_level: str = None, **kw):
+    def __init__(
+            self,
+            url: str,
+            username: str,
+            password: str,
+            db: str = None,
+            auto_auth: bool = True,
+            logger: loguru_logger = None,
+            log_level: str = None,
+            **kw
+    ):
         super().__init__(**kw)
 
         self._url = url[:-1] if url[-1] == "/" else url
         self._username = username
         self._password = password
         self._db = db or self._extract_db_from_url()
 
         self.common = xmlrpc.client.ServerProxy(f"{self._url}/xmlrpc/2/common", allow_none=True)
         self.models = None
 
         self.requests = list()
         self.cache = {}
-        self._context = dict()          # Todo: use a frozendict for context things
+        self._context = frozendict()
 
         # Todo: make it an object
         self.user = None
 
-        self.logger = logger
-        self.logger.remove()
-        self.logger.add(sys.stderr, level=log_level or "INFO")
+        self.logger = logger if isinstance(logger, type(loguru_logger)) else loguru_logger
+        if logger is None:
+            self.logger.remove()
+            self.logger.add(sys.stderr, level=log_level or "INFO")
 
         if auto_auth:
             self.authenticate()
 
     def __missing__(self, key):
-        res = RecordSet(key, self)
+        res = RecordSet(key, self, context=self._context)
         if self._has_missing_cache(key):
             self.cache.update({
                 key: {
                     'fields': res.fields_get(),
                     'records': dict(),
                 }
             })
@@ -93,15 +105,15 @@
         module, xml_id = xmlid.split(".")
         res = self['ir.model.data'].check_object_reference(module, xml_id)
         if res:
             return self[res[0]].browse(res[1])
         return None
 
     def with_context(self, **kw):
-        self._context = self._context | kw
+        self._context = self._context.copy(**kw)
         return self
 
 
     def log_request(self, recordset, *args, **kwargs):
         # Todo: add more infos about performance.
         self.logger.trace(f"Executing {args[0]} on {recordset} with args: {args[1:]} / kwargs: {kwargs}")
         self.requests.append({
```

### Comparing `otools-rpc-0.2.7/otools_rpc/external_api/recordset.py` & `otools-rpc-0.3.0/otools_rpc/external_api/recordset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import copy
-from .common import assert_same_model, cache, log_request, model
+import xmlrpc.client
+from .common import assert_same_model, cache, log_request, model, frozendict
 from typing import Union
 
 
 class RecordSet:
-    def __init__(self, name, env, ids: list[int] = None, context: dict = None):
+    def __init__(self, name, env, ids: list[int] = None, context: frozendict = None):
         self._name = name
         self._env = env
         self._curr = -1
         self._ids = self._sanitize_ids(ids or list())
 
         """
         Each recordset has its own context, but inherits it:
             1) from the recordset it was created
             2) from the general environment 
         """
-        self._context = copy.deepcopy(context) or copy.deepcopy(env.context) or dict()
+        self._context = context.copy() if context is not None else frozendict()
 
         self.logger = self._env.logger
 
     def __str__(self):
         return f"{self._name}({', '.join(map(str, self._ids))})"
 
     def __bool__(self):
@@ -31,15 +31,15 @@
     def __iter__(self):
         self._curr = -1
         return self
 
     def __next__(self):
         if self._curr < len(self) - 1:
             self._curr += 1
-            return RecordSet(self._name, self._env, [self._ids[self._curr]])
+            return self._recordset(self._ids[self._curr])
         raise StopIteration
 
     def __getitem__(self, item):
         if isinstance(item, slice):
             return self._recordset(self._ids[item])
         elif isinstance(item, str):
             return getattr(self, item)
@@ -119,15 +119,18 @@
                 self._env.uid,
                 self._env._password,
                 self._name,
                 method,
                 args,
                 kw,
             )
+
         except Exception as e:
+            if isinstance(e, xmlrpc.client.Fault) and 'cannot marshal' in str(e):
+                return None
             self.logger.error(f"Error while executing {self._name}.{method}():")
             self.logger.debug(f"args / kwargs:\n {args} \n {kw}")
             self.logger.error("Odoo API Response:\n" + str(e).replace('\\n', '\n'))
 
     # --------------------------------------------
     #                   ORM
     # --------------------------------------------
@@ -144,15 +147,15 @@
     def check_object_reference(self, module, xml_id):
         # Extra safety check, don't delete (even if nobody should use it directly)
         if self._name != 'ir.model.data':
             return self['ir.model.data'].check_object_reference(module, xml_id)
         return self._execute('check_object_reference', module, xml_id)
 
     def with_context(self, **kw):
-        self._context = self._context | kw
+        self._context = self._context.copy(**kw)
         return self
 
 
     # --- CRUD ---
 
 
     @model
@@ -194,11 +197,22 @@
         return res
 
     def copy(self):
         res_id = self._execute('copy')
         return self._recordset(res_id)
 
 
+    # --- ORM helpers ---
+
+
     def mapped(self, field: str):
         return [getattr(rec, field) for rec in self]
 
+    def filtered(self, func: Union[callable, str]):
+        if isinstance(func, str):
+            name = func
+            func = lambda rec: rec[name]
+            # func = lambda rec: any(rec.mapped(name))      # Odoo behavior
+        return self.browse([rec.id for rec in self if func(rec)])
 
+    def filtered_domain(self, domain: list[tuple]):
+        return self.search([('id', 'in', self.ids)] + domain)
```

### Comparing `otools-rpc-0.2.7/setup.py` & `otools-rpc-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="otools-rpc",
-    version="0.2.7",
+    version="0.3.0",
     description="A tool to interact with Odoo's external API.",
     packages=find_packages(exclude=["tests"]),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MrFaBemol/otools-rpc",
     author="Gautier Casabona",
     author_email="gcasabona.pro@gmail.com",
@@ -20,14 +20,14 @@
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Natural Language :: English"
     ],
     install_requires=[
         "loguru >= 0.7.0",
-        "requests == 2.29.0" #Higher version can break your docker python lib
+        "requests == 2.29.0"  # Higher version can break your docker python lib
     ],
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
     },
     python_requires=">=3.8",
 )
```

