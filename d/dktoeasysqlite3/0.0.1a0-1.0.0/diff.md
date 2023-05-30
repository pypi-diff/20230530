# Comparing `tmp/dktoeasysqlite3-0.0.1a0.tar.gz` & `tmp/dktoeasysqlite3-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dktoeasysqlite3-0.0.1a0.tar", last modified: Mon May 29 20:18:03 2023, max compression
+gzip compressed data, was "dktoeasysqlite3-1.0.0.tar", last modified: Tue May 30 21:24:53 2023, max compression
```

## Comparing `dktoeasysqlite3-0.0.1a0.tar` & `dktoeasysqlite3-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 20:18:03.878154 dktoeasysqlite3-0.0.1a0/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      779 2023-05-29 20:18:03.878154 dktoeasysqlite3-0.0.1a0/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)      274 2023-05-29 13:07:42.000000 dktoeasysqlite3-0.0.1a0/README.md
--rw-r--r--   0 pierre    (1000) pierre    (1000)      589 2023-05-29 20:18:03.882154 dktoeasysqlite3-0.0.1a0/setup.cfg
--rw-r--r--   0 pierre    (1000) pierre    (1000)      347 2023-05-29 13:07:42.000000 dktoeasysqlite3-0.0.1a0/setup.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 20:18:03.854154 dktoeasysqlite3-0.0.1a0/src/
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 20:18:03.862154 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3223 2023-05-29 13:07:42.000000 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      530 2023-05-29 13:07:42.000000 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/_add_db.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1321 2023-05-29 13:07:42.000000 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/_execute.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1298 2023-05-29 13:07:42.000000 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/_insert_data.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      390 2023-05-29 13:07:42.000000 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/_request_db.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1170 2023-05-29 13:07:42.000000 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/global_var_storage.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1267 2023-05-29 13:07:42.000000 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/structbdd.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 20:18:03.878154 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3.egg-info/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      779 2023-05-29 20:18:03.000000 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3.egg-info/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)      483 2023-05-29 20:18:03.000000 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3.egg-info/SOURCES.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-05-29 20:18:03.000000 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3.egg-info/dependency_links.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       64 2023-05-29 20:18:03.000000 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3.egg-info/requires.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       16 2023-05-29 20:18:03.000000 dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3.egg-info/top_level.txt
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-30 21:24:53.931908 dktoeasysqlite3-1.0.0/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      839 2023-05-30 21:24:53.935908 dktoeasysqlite3-1.0.0/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      320 2023-05-30 14:13:44.000000 dktoeasysqlite3-1.0.0/README.md
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      588 2023-05-30 21:24:53.935908 dktoeasysqlite3-1.0.0/setup.cfg
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      347 2023-05-29 13:07:42.000000 dktoeasysqlite3-1.0.0/setup.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-30 21:24:53.899908 dktoeasysqlite3-1.0.0/src/
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-30 21:24:53.915908 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3792 2023-05-30 21:20:37.000000 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      530 2023-05-29 13:07:42.000000 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/_add_db.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1327 2023-05-30 15:34:58.000000 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/_execute.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1298 2023-05-29 13:07:42.000000 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/_insert_data.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      394 2023-05-30 15:35:30.000000 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/_request_db.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1170 2023-05-29 13:07:42.000000 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/global_var_storage.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1267 2023-05-29 13:07:42.000000 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/structbdd.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-30 21:24:53.931908 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3.egg-info/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      839 2023-05-30 21:24:53.000000 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3.egg-info/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      483 2023-05-30 21:24:53.000000 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3.egg-info/SOURCES.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-05-30 21:24:53.000000 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3.egg-info/dependency_links.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       64 2023-05-30 21:24:53.000000 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3.egg-info/requires.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       16 2023-05-30 21:24:53.000000 dktoeasysqlite3-1.0.0/src/dktoeasysqlite3.egg-info/top_level.txt
```

### Comparing `dktoeasysqlite3-0.0.1a0/setup.cfg` & `dktoeasysqlite3-1.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dktoeasysqlite3
-version = 0.0.1a
+version = 1.0.0
 author = Pierre
 license = APGL
 description = Some commands to call sqlite3 db easyly
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://discord-catho.frama.io/easysqlite3
 project_urls =
```

### Comparing `dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/__init__.py` & `dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,24 +37,43 @@
         self.lock=lock_in
 
         if db_path:
             self.db_path = db_path
         #endIf
 
         if self.db_path is not None and os.path.exists(self.db_path):
-
             pass
 
         elif createIfNotExists is not None:
 
+            try:
+
+                conn = sqlite3.connect(self.db_path)
+
+            except sqlite3.OperationalError:
+
+                os.makedirs(os.path.dirname(self.db_path), exist_ok=True) # exist_ok : ne pas lever d'erreur si existe
+                sys.stderr.write(f"! WARNING : path for DATABASE not exist, create a directory:\n{os.path.dirname(self.db_path)}\n")
+
+            finally:
+
+                conn = sqlite3.connect(self.db_path)
+
+            #endTry
+
             sys.stderr.write(f"! WARNING : path for DATABASE not exist, create a database:\n{self.db_path}\n")
-            conn = sqlite3.connect(self.db_path)
             cursor = conn.cursor()
-            print("DBG", createIfNotExists)
-            if isinstance(createIfNotExists, str):
+
+            if isinstance(createIfNotExists, bool) and createIfNotExists:
+
+                conn.commit()
+                conn.close()
+                return
+
+            elif isinstance(createIfNotExists, str):
                 createIfNotExists = [createIfNotExists,]
             #endIf
 
             if isinstance(createIfNotExists, list) or isinstance(createIfNotExists, tuple):
                 createIfNotExists = {e:{"useless_col":"INTEGER"} for e in createIfNotExists}
             #endIf
 
@@ -84,14 +103,15 @@
         self.conn = sqlite3.connect(f"{self.db_path}")
 
     #endDef
 
     from ._request_db import request_db
     from ._add_db import add_db
     from ._insert_data import insert_data
+    from ._execute import execute
 
     def commit(self):
         with self.lock:
             self.conn.commit()
         #endWith
 
     def end_conn(self):
```

### Comparing `dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/_add_db.py` & `dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/_add_db.py`

 * *Files identical despite different names*

### Comparing `dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/_execute.py` & `dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/_execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         c.execute( query, datas )
     else:
         c.execute( query )
     #endIf
 
     return c
 
-def execute(query:str, datas:list=[], lock:bool=False):
+def execute(self, query:str, datas:list=[], lock:bool=False):
     """
     :param str query: Query
     :param list|tuple datas: List of arguments (same number as '?' in the query)
 
     :param book lock: enable/disable lock
 
     :raise ValueError: query not a string
@@ -37,15 +37,15 @@
     if not isinstance(datas, list) and not isinstance(datas, tuple):
         sys.stderr.write(f"datas: {datas}\n")
         raise ValueError(f"datas is expected to be a list, not {type(datas)}")
     #endIf
 
     if lock and self.lock:
         with self.lock:
-            return _execute(self.lock, query, datas)
+            return _execute(self.conn, query, datas)
         #EndWith
     else:
-        return _execute(self.lock, query, datas)
+        return _execute(self.conn, query, datas)
     #endIf
 
     return None
 #endDef
```

### Comparing `dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/_insert_data.py` & `dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/_insert_data.py`

 * *Files identical despite different names*

### Comparing `dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/global_var_storage.py` & `dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/global_var_storage.py`

 * *Files identical despite different names*

### Comparing `dktoeasysqlite3-0.0.1a0/src/dktoeasysqlite3/structbdd.py` & `dktoeasysqlite3-1.0.0/src/dktoeasysqlite3/structbdd.py`

 * *Files identical despite different names*

