# Comparing `tmp/ardilla-0.3.2b0.tar.gz` & `tmp/ardilla-0.3.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardilla-0.3.2b0.tar", last modified: Mon May 29 14:38:14 2023, max compression
+gzip compressed data, was "ardilla-0.3.3b0.tar", last modified: Tue May 30 13:37:24 2023, max compression
```

## Comparing `ardilla-0.3.2b0.tar` & `ardilla-0.3.3b0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 14:38:14.898011 ardilla-0.3.2b0/
--rw-rw-rw-   0        0        0     1084 2023-05-21 21:48:03.000000 ardilla-0.3.2b0/LICENCE
--rw-rw-rw-   0        0        0      898 2023-05-29 14:38:14.889013 ardilla-0.3.2b0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-29 14:38:14.704012 ardilla-0.3.2b0/ardilla/
--rw-rw-rw-   0        0        0      145 2023-05-22 03:22:06.000000 ardilla-0.3.2b0/ardilla/__init__.py
--rw-rw-rw-   0        0        0     4877 2023-05-28 06:26:40.000000 ardilla-0.3.2b0/ardilla/abc.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:38:14.859013 ardilla-0.3.2b0/ardilla/asyncio/
--rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.3.2b0/ardilla/asyncio/__init__.py
--rw-rw-rw-   0        0        0     8771 2023-05-29 01:20:30.000000 ardilla-0.3.2b0/ardilla/asyncio/crud.py
--rw-rw-rw-   0        0        0     2074 2023-05-28 13:12:38.000000 ardilla-0.3.2b0/ardilla/asyncio/engine.py
--rw-rw-rw-   0        0        0     8808 2023-05-29 13:48:04.000000 ardilla-0.3.2b0/ardilla/crud.py
--rw-rw-rw-   0        0        0     2232 2023-05-29 14:34:14.000000 ardilla-0.3.2b0/ardilla/engine.py
--rw-rw-rw-   0        0        0      508 2023-05-28 05:57:28.000000 ardilla-0.3.2b0/ardilla/errors.py
--rw-rw-rw-   0        0        0     2586 2023-05-25 17:47:32.000000 ardilla-0.3.2b0/ardilla/fields.py
--rw-rw-rw-   0        0        0      222 2023-05-22 17:13:39.000000 ardilla-0.3.2b0/ardilla/logging.py
--rw-rw-rw-   0        0        0     2846 2023-05-28 13:16:48.000000 ardilla-0.3.2b0/ardilla/models.py
--rw-rw-rw-   0        0        0     1082 2023-05-18 22:33:35.000000 ardilla-0.3.2b0/ardilla/ordering.py
--rw-rw-rw-   0        0        0     6518 2023-05-29 14:36:16.000000 ardilla-0.3.2b0/ardilla/queries.py
--rw-rw-rw-   0        0        0     5680 2023-05-29 13:53:23.000000 ardilla-0.3.2b0/ardilla/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:38:14.841017 ardilla-0.3.2b0/ardilla.egg-info/
--rw-rw-rw-   0        0        0      898 2023-05-29 14:38:14.000000 ardilla-0.3.2b0/ardilla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2023-05-29 14:38:14.000000 ardilla-0.3.2b0/ardilla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 14:38:14.000000 ardilla-0.3.2b0/ardilla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      208 2023-05-29 14:38:14.000000 ardilla-0.3.2b0/ardilla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-29 14:38:14.000000 ardilla-0.3.2b0/ardilla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1216 2023-05-29 13:53:31.000000 ardilla-0.3.2b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 14:38:14.901023 ardilla-0.3.2b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 14:38:14.885017 ardilla-0.3.2b0/tests/
--rw-rw-rw-   0        0        0     6628 2023-05-28 05:57:28.000000 ardilla-0.3.2b0/tests/test_async.py
--rw-rw-rw-   0        0        0     2174 2023-05-28 13:21:08.000000 ardilla-0.3.2b0/tests/test_models.py
--rw-rw-rw-   0        0        0     5907 2023-05-28 05:57:28.000000 ardilla-0.3.2b0/tests/test_sync.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:37:24.204930 ardilla-0.3.3b0/
+-rw-rw-rw-   0        0        0     1084 2023-05-21 21:48:03.000000 ardilla-0.3.3b0/LICENCE
+-rw-rw-rw-   0        0        0     5203 2023-05-30 13:37:24.201930 ardilla-0.3.3b0/PKG-INFO
+-rw-rw-rw-   0        0        0     4301 2023-05-30 13:33:05.000000 ardilla-0.3.3b0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 13:37:24.017932 ardilla-0.3.3b0/ardilla/
+-rw-rw-rw-   0        0        0      145 2023-05-22 03:22:06.000000 ardilla-0.3.3b0/ardilla/__init__.py
+-rw-rw-rw-   0        0        0     5064 2023-05-30 13:32:37.000000 ardilla-0.3.3b0/ardilla/abc.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:37:24.176930 ardilla-0.3.3b0/ardilla/asyncio/
+-rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.3.3b0/ardilla/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     8771 2023-05-29 01:20:30.000000 ardilla-0.3.3b0/ardilla/asyncio/crud.py
+-rw-rw-rw-   0        0        0     2622 2023-05-30 13:35:24.000000 ardilla-0.3.3b0/ardilla/asyncio/engine.py
+-rw-rw-rw-   0        0        0     8808 2023-05-29 13:48:04.000000 ardilla-0.3.3b0/ardilla/crud.py
+-rw-rw-rw-   0        0        0     2730 2023-05-30 13:34:32.000000 ardilla-0.3.3b0/ardilla/engine.py
+-rw-rw-rw-   0        0        0      508 2023-05-28 05:57:28.000000 ardilla-0.3.3b0/ardilla/errors.py
+-rw-rw-rw-   0        0        0     2586 2023-05-25 17:47:32.000000 ardilla-0.3.3b0/ardilla/fields.py
+-rw-rw-rw-   0        0        0      222 2023-05-22 17:13:39.000000 ardilla-0.3.3b0/ardilla/logging.py
+-rw-rw-rw-   0        0        0     2846 2023-05-28 13:16:48.000000 ardilla-0.3.3b0/ardilla/models.py
+-rw-rw-rw-   0        0        0     1082 2023-05-18 22:33:35.000000 ardilla-0.3.3b0/ardilla/ordering.py
+-rw-rw-rw-   0        0        0     6518 2023-05-29 14:36:16.000000 ardilla-0.3.3b0/ardilla/queries.py
+-rw-rw-rw-   0        0        0     5680 2023-05-29 13:53:23.000000 ardilla-0.3.3b0/ardilla/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:37:24.153928 ardilla-0.3.3b0/ardilla.egg-info/
+-rw-rw-rw-   0        0        0     5203 2023-05-30 13:37:23.000000 ardilla-0.3.3b0/ardilla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-05-30 13:37:23.000000 ardilla-0.3.3b0/ardilla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 13:37:23.000000 ardilla-0.3.3b0/ardilla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      208 2023-05-30 13:37:23.000000 ardilla-0.3.3b0/ardilla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 13:37:23.000000 ardilla-0.3.3b0/ardilla.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1216 2023-05-30 13:30:50.000000 ardilla-0.3.3b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 13:37:24.205930 ardilla-0.3.3b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 13:37:24.197929 ardilla-0.3.3b0/tests/
+-rw-rw-rw-   0        0        0     6628 2023-05-28 05:57:28.000000 ardilla-0.3.3b0/tests/test_async.py
+-rw-rw-rw-   0        0        0     2174 2023-05-28 13:21:08.000000 ardilla-0.3.3b0/tests/test_models.py
+-rw-rw-rw-   0        0        0     5907 2023-05-28 05:57:28.000000 ardilla-0.3.3b0/tests/test_sync.py
```

### Comparing `ardilla-0.3.2b0/LICENCE` & `ardilla-0.3.3b0/LICENCE`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.2b0/ardilla/abc.py` & `ardilla-0.3.3b0/ardilla/abc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 import sqlite3
-from typing import Any, Literal, TypeVar, Optional
+from typing import Any, Literal, TypeVar, Optional, Union
 from abc import abstractmethod, ABC
 from sqlite3 import Row
 
 from .models import M, Model as BaseModel
 
 E = TypeVar("E")  # Engine Type
 
@@ -27,36 +27,43 @@
     def check_connection(self) -> bool:
         """Checks if the engine's connection is alive
         works for both the sync and async classes
 
         Returns:
             bool: if the connection is fine
         """
+        con: Union[Connection, None] = getattr(self, 'con', None)
         try:
-            if isinstance(self.con, sqlite3.Connection):
-                self.con.cursor()
+            if isinstance(con, sqlite3.Connection):
+                con.cursor()
                 return True
-            else:
+            elif con is not None:
                 # should be aiosqlite
                 # we don't import it here to prevent import errors 
                 # in case there's missing dependency of aiosqlite
-                return self.con._running and self.con._connection                
+                return con._running and con._connection
+            else:
+                return None
         except:
             return False
 
     def __init__(
         self,
         path: str,
         enable_foreing_keys: bool = False,
     ):
         self.path = path
         self.schemas: set[str] = set()
         self.tables_created: set[str] = set()
         self._cruds: dict[type[M], CrudType] = {}
         self.enable_foreing_keys = enable_foreing_keys
+    
+    @abstractmethod
+    def get_connection(self) -> Connection:
+        ...
         
     @abstractmethod
     def connect(self) -> Connection:
         ...
         
     @abstractmethod
     def close(self) -> None:
```

### Comparing `ardilla-0.3.2b0/ardilla/asyncio/crud.py` & `ardilla-0.3.3b0/ardilla/asyncio/crud.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.2b0/ardilla/asyncio/engine.py` & `ardilla-0.3.3b0/ardilla/asyncio/engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 from __future__ import annotations
+from ctypes import Union
 
 import aiosqlite
 
 from ..abc import BaseEngine
 from ..models import M
 from ..errors import DisconnectedEngine
 
 from .crud import AsyncCrud
 
 class AsyncEngine(BaseEngine):
     """Async Engine that uses `aiosqlite.Connection` and `aiosqlite.Cursor`
     """
     con: aiosqlite.Connection
+
+    async def get_connection(self) -> aiosqlite.Connection:
+        """Gets the connections or makes a new one but it doesn't set it as an attrib
+
+        Returns:
+            sqlite3.Connection: the connection
+        """
+        con: Union[aiosqlite.Connection, None] = getattr(self, 'con', None)
+        if not self.check_connection():
+            con: aiosqlite.Connection = await aiosqlite.connect(self.path)
+            con.row_factory = aiosqlite.Row
+            
+            if self.enable_foreing_keys:
+                await con.execute("PRAGMA foreign_keys = on;")
+            
+            return con
+        else:
+            return self.con
     
     async def connect(self) -> aiosqlite.Connection:
         """
         Stablishes a connection to the database
         Returns:
             The connection
         """
         await self.close()
-        con = await aiosqlite.connect(self.path)
-        con.row_factory = aiosqlite.Row
-        if self.enable_foreing_keys:
-            await con.execute('PRAGMA foreign_keys = ON;')
-        self.con = con
-        return con
+        
+        self.con = await self.get_connection()
+        return self.con
 
     async def close(self) -> None:
         if self.check_connection():
             await self.con.close()
         self._cruds.clear()
 
     async def __aenter__(self) -> AsyncEngine:
```

### Comparing `ardilla-0.3.2b0/ardilla/crud.py` & `ardilla-0.3.3b0/ardilla/crud.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.2b0/ardilla/engine.py` & `ardilla-0.3.3b0/ardilla/engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import sqlite3
+from typing import Union
 
 from .models import M
 from .crud import Crud
 from .abc import BaseEngine
 from .errors import DisconnectedEngine
 
 class Engine(BaseEngine):
@@ -19,31 +20,44 @@
         tables_created (set[str]): the tables that have been setup by the engine
         enable_foreing_keys (bool): if True, the engine enables the pragma on all connections
     """
     con: sqlite3.Connection
     
     def __init__(self, path: str, enable_foreing_keys: bool = False):
         super().__init__(path, enable_foreing_keys)
+    
+    def get_connection(self) -> sqlite3.Connection:
+        """Gets the connections or makes a new one but it doesn't set it as an attrib
+
+        Returns:
+            sqlite3.Connection: the connection
+        """
+        con: Union[sqlite3.Connection, None] = getattr(self, 'con', None)
+        if not self.check_connection():
+            con = sqlite3.connect(self.path)
+            con.row_factory = sqlite3.Row
+            
+            if self.enable_foreing_keys:
+                con.execute("PRAGMA foreign_keys = on;")
+            
+            return con
+        else:
+            return self.con
         
     def __enter__(self):
         self.connect()
         return self
     
     def __exit__(self, *_):
         self.close()
-    
+        
     def connect(self) -> sqlite3.Connection:
         self.close()
-        con = sqlite3.connect(self.path)
-        con.row_factory = sqlite3.Row
-        
-        if self.enable_foreing_keys:
-            con.execute("PRAGMA foreign_keys = on;")
-        self.con = con
-        return con
+        self.con = self.get_connection()
+        return self.con
 
     def close(self) -> None:
         if self.check_connection():
             self.con.close()
         self._cruds.clear()
     
     def crud(self, Model: type[M]) -> Crud[M]:
```

### Comparing `ardilla-0.3.2b0/ardilla/fields.py` & `ardilla-0.3.3b0/ardilla/fields.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.2b0/ardilla/models.py` & `ardilla-0.3.3b0/ardilla/models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.2b0/ardilla/ordering.py` & `ardilla-0.3.3b0/ardilla/ordering.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.2b0/ardilla/queries.py` & `ardilla-0.3.3b0/ardilla/queries.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.2b0/ardilla/schemas.py` & `ardilla-0.3.3b0/ardilla/schemas.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.2b0/ardilla.egg-info/SOURCES.txt` & `ardilla-0.3.3b0/ardilla.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENCE
+README.md
 pyproject.toml
 ardilla/__init__.py
 ardilla/abc.py
 ardilla/crud.py
 ardilla/engine.py
 ardilla/errors.py
 ardilla/fields.py
```

### Comparing `ardilla-0.3.2b0/pyproject.toml` & `ardilla-0.3.3b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ardilla"
-version = "0.3.2-beta"
+version = "0.3.3-beta"
 authors = [
   { name="ChrisDewa", email="chrisdewa@duck.com" },
 ]
 description = "Ardilla ORM. Easy to use, fast to implement, with sync and async flavors"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ardilla-0.3.2b0/tests/test_async.py` & `ardilla-0.3.3b0/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.2b0/tests/test_models.py` & `ardilla-0.3.3b0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.2b0/tests/test_sync.py` & `ardilla-0.3.3b0/tests/test_sync.py`

 * *Files identical despite different names*

