# Comparing `tmp/e6data-python-connector-1.0.6.tar.gz` & `tmp/e6data-python-connector-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e6data-python-connector-1.0.6.tar", last modified: Mon May 22 20:22:43 2023, max compression
+gzip compressed data, was "e6data-python-connector-1.0.7.tar", last modified: Tue May 30 07:52:31 2023, max compression
```

## Comparing `e6data-python-connector-1.0.6.tar` & `e6data-python-connector-1.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-22 20:22:43.949553 e6data-python-connector-1.0.6/
--rw-r--r--   0 vishalanand   (501) staff       (20)    11357 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/LICENSE
--rw-r--r--   0 vishalanand   (501) staff       (20)       55 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/MANIFEST.in
--rw-r--r--   0 vishalanand   (501) staff       (20)     7301 2023-05-22 20:22:43.949700 e6data-python-connector-1.0.6/PKG-INFO
--rw-r--r--   0 vishalanand   (501) staff       (20)     5189 2023-05-22 20:22:22.000000 e6data-python-connector-1.0.6/README.md
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-22 20:22:43.932635 e6data-python-connector-1.0.6/e6data_python_connector.egg-info/
--rw-r--r--   0 vishalanand   (501) staff       (20)     7301 2023-05-22 20:22:43.000000 e6data-python-connector-1.0.6/e6data_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 vishalanand   (501) staff       (20)      632 2023-05-22 20:22:43.000000 e6data-python-connector-1.0.6/e6data_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)        1 2023-05-22 20:22:43.000000 e6data-python-connector-1.0.6/e6data_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)       63 2023-05-22 20:22:43.000000 e6data-python-connector-1.0.6/e6data_python_connector.egg-info/entry_points.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)       66 2023-05-22 20:22:43.000000 e6data-python-connector-1.0.6/e6data_python_connector.egg-info/requires.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)        6 2023-05-22 20:22:43.000000 e6data-python-connector-1.0.6/e6data_python_connector.egg-info/top_level.txt
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-22 20:22:43.945434 e6data-python-connector-1.0.6/e6xdb/
--rw-r--r--   0 vishalanand   (501) staff       (20)      334 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/e6xdb/__init__.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     9958 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/e6xdb/common.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      682 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/e6xdb/constants.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     6052 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/e6xdb/datainputstream.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    13623 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/e6xdb/date_time_utils.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    16837 2023-05-22 20:22:22.000000 e6data-python-connector-1.0.6/e6xdb/e6x.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      382 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/e6xdb/exceptions.py
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-22 20:22:43.949162 e6data-python-connector-1.0.6/e6xdb/server/
--rw-r--r--   0 vishalanand   (501) staff       (20)   191597 2023-05-22 18:51:52.000000 e6data-python-connector-1.0.6/e6xdb/server/QueryEngineService.py
--rw-r--r--   0 vishalanand   (501) staff       (20)       56 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/e6xdb/server/__init__.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      366 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/e6xdb/server/constants.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    12609 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/e6xdb/server/ttypes.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    11833 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/e6xdb/sqlalchemy_e6x.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     1777 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/e6xdb/typeId.py
--rw-r--r--   0 vishalanand   (501) staff       (20)       64 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.6/pyproject.toml
--rw-r--r--   0 vishalanand   (501) staff       (20)       73 2023-05-22 20:22:43.951306 e6data-python-connector-1.0.6/setup.cfg
--rw-r--r--   0 vishalanand   (501) staff       (20)     1925 2023-05-22 20:22:22.000000 e6data-python-connector-1.0.6/setup.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-30 07:52:31.152654 e6data-python-connector-1.0.7/
+-rw-r--r--   0 vishalanand   (501) staff       (20)    11357 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/LICENSE
+-rw-r--r--   0 vishalanand   (501) staff       (20)       55 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/MANIFEST.in
+-rw-r--r--   0 vishalanand   (501) staff       (20)     7301 2023-05-30 07:52:31.153050 e6data-python-connector-1.0.7/PKG-INFO
+-rw-r--r--   0 vishalanand   (501) staff       (20)     5189 2023-05-30 06:22:51.000000 e6data-python-connector-1.0.7/README.md
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-30 07:52:31.098571 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/
+-rw-r--r--   0 vishalanand   (501) staff       (20)     7301 2023-05-30 07:52:30.000000 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 vishalanand   (501) staff       (20)      632 2023-05-30 07:52:30.000000 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)        1 2023-05-30 07:52:30.000000 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       63 2023-05-30 07:52:30.000000 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/entry_points.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       66 2023-05-30 07:52:30.000000 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/requires.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)        6 2023-05-30 07:52:30.000000 e6data-python-connector-1.0.7/e6data_python_connector.egg-info/top_level.txt
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-30 07:52:31.118765 e6data-python-connector-1.0.7/e6xdb/
+-rw-r--r--   0 vishalanand   (501) staff       (20)      334 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     9958 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/common.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      682 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/constants.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     6052 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/datainputstream.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    13623 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/date_time_utils.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    18483 2023-05-30 07:49:42.000000 e6data-python-connector-1.0.7/e6xdb/e6x.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      382 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/exceptions.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-30 07:52:31.150871 e6data-python-connector-1.0.7/e6xdb/server/
+-rw-r--r--   0 vishalanand   (501) staff       (20)   206971 2023-05-30 06:20:46.000000 e6data-python-connector-1.0.7/e6xdb/server/QueryEngineService.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)       56 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/server/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      366 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/server/constants.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    21227 2023-05-30 06:20:46.000000 e6data-python-connector-1.0.7/e6xdb/server/ttypes.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    11833 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/sqlalchemy_e6x.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     1777 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/e6xdb/typeId.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)       64 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.7/pyproject.toml
+-rw-r--r--   0 vishalanand   (501) staff       (20)       73 2023-05-30 07:52:31.156686 e6data-python-connector-1.0.7/setup.cfg
+-rw-r--r--   0 vishalanand   (501) staff       (20)     1925 2023-05-30 06:22:52.000000 e6data-python-connector-1.0.7/setup.py
```

### Comparing `e6data-python-connector-1.0.6/LICENSE` & `e6data-python-connector-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.6/PKG-INFO` & `e6data-python-connector-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: e6data-python-connector
-Version: 1.0.6
+Version: 1.0.7
 Summary: Client for the e6data distributed SQL Engine.
 Home-page: https://github.com/e6x-labs/e6data-python-connector
 Author: Uniphi, Inc.
 Author-email: info@e6data.com
 License: Apache 2.0
 Description: # e6data Python Connector
         
-        ![version](https://img.shields.io/badge/version-1.0.6-blue.svg)
+        ![version](https://img.shields.io/badge/version-1.0.7-blue.svg)
         
         ## Introduction
         
         The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
         
         To install the Python package, use the command below:
         ```shell
```

### Comparing `e6data-python-connector-1.0.6/README.md` & `e6data-python-connector-1.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # e6data Python Connector
 
-![version](https://img.shields.io/badge/version-1.0.6-blue.svg)
+![version](https://img.shields.io/badge/version-1.0.7-blue.svg)
 
 ## Introduction
 
 The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
 
 To install the Python package, use the command below:
 ```shell
```

### Comparing `e6data-python-connector-1.0.6/e6data_python_connector.egg-info/PKG-INFO` & `e6data-python-connector-1.0.7/e6data_python_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: e6data-python-connector
-Version: 1.0.6
+Version: 1.0.7
 Summary: Client for the e6data distributed SQL Engine.
 Home-page: https://github.com/e6x-labs/e6data-python-connector
 Author: Uniphi, Inc.
 Author-email: info@e6data.com
 License: Apache 2.0
 Description: # e6data Python Connector
         
-        ![version](https://img.shields.io/badge/version-1.0.6-blue.svg)
+        ![version](https://img.shields.io/badge/version-1.0.7-blue.svg)
         
         ## Introduction
         
         The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
         
         To install the Python package, use the command below:
         ```shell
```

### Comparing `e6data-python-connector-1.0.6/e6data_python_connector.egg-info/SOURCES.txt` & `e6data-python-connector-1.0.7/e6data_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.6/e6xdb/common.py` & `e6data-python-connector-1.0.7/e6xdb/common.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.6/e6xdb/constants.py` & `e6data-python-connector-1.0.7/e6xdb/constants.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.6/e6xdb/datainputstream.py` & `e6data-python-connector-1.0.7/e6xdb/datainputstream.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.6/e6xdb/date_time_utils.py` & `e6data-python-connector-1.0.7/e6xdb/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.6/e6xdb/e6x.py` & `e6data-python-connector-1.0.7/e6xdb/e6x.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,17 +200,32 @@
     def get_tables(self, database):
         return self._client.getTables(sessionId=self.get_session_id, schema=database)
 
     def get_tables_v2(self, catalog_name, database):
         return self._client.getTablesV2(sessionId=self.get_session_id, catalogName=catalog_name, schema=database)
 
     def get_columns(self, database, table):
-        catalog_name = ''
-        return self._client.getColumns(sessionId=self.get_session_id, catalogName=catalog_name, schema=database,
-                                       table=table)
+        return self._client.getColumns(sessionId=self.get_session_id, schema=database, table=table)
+
+    def status(self, query_id):
+        return self._client.status(sessionId=self.get_session_id, queryId=query_id)
+
+    def get_add_catalog_response(self):
+        """
+        Response Type:
+            AddCatalogsResponse(status='success', failures=[])
+        Usage:
+            response.status: success, in_progress, failed
+
+        Error Usage:
+            response = conn.get_add_catalog_response()
+            if response.status == 'error'
+                print(response.failures[0].reason)
+        """
+        return self._client.getAddCatalogsResponse(sessionId=self.get_session_id)
 
     def get_columns_v2(self, catalog_name, database, table):
         return self._client.getColumnsV2(
             sessionId=self.get_session_id,
             catalogName=catalog_name,
             schema=database,
             table=table
@@ -497,7 +512,49 @@
 #
 # Type Objects and Constructors
 #
 
 for type_id in PRIMITIVE_TYPES:
     name = TypeId._VALUES_TO_NAMES[type_id]
     setattr(sys.modules[__name__], name, DBAPITypeObject([name]))
+
+
+if __name__ == '__main__':
+    ip = '54.205.255.188'
+    conn = Connection(
+        host=ip,
+        username='admin',
+        password='admin',
+        port=9000
+    )
+    catalogs = {'catalogs': [{
+        "type": 'HIVE',
+        "name": 'hive',
+        "hive_ip": '18.233.112.169',
+        "hive_port": 9084,
+        "included_schemas": [],
+        "excluded_schemas": [],
+        "included_tables": [],
+        "excluded_tables": [],
+        "included_columns": [],
+        "excluded_columns": [],
+        "is_assumed_role": False,
+        "assumed_role_arn": '',
+        "default": True
+    }]}
+    import json
+    import time
+    start = time.time()
+    # print(conn.add_catalogs(json.dumps(catalogs)))
+    add_cat_time = time.time()
+    print('Add catalog time', add_cat_time - start)
+    status = 'in_progress'
+    res = conn.get_add_catalog_response()
+    print(res)
+    print(res.failures[0].reason)
+    # while status == 'in_progress':
+    #     res = conn.get_add_catalog_response()
+    #     status = res.status
+    #     print(res)
+    #     time.sleep(5)
+    print('get_add_catalog_response time', time.time() - add_cat_time)
+
```

### Comparing `e6data-python-connector-1.0.6/e6xdb/server/QueryEngineService.py` & `e6data-python-connector-1.0.7/e6xdb/server/QueryEngineService.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,19 +174,18 @@
         Parameters:
          - sessionId
          - catalogName
 
         """
         pass
 
-    def getColumns(self, sessionId, catalogName, schema, table):
+    def getColumns(self, sessionId, schema, table):
         """
         Parameters:
          - sessionId
-         - catalogName
          - schema
          - table
 
         """
         pass
 
     def getColumnsV2(self, sessionId, catalogName, schema, table):
@@ -213,23 +212,40 @@
         Parameters:
          - sessionId
          - propMap
 
         """
         pass
 
+    def status(self, sessionId, queryId):
+        """
+        Parameters:
+         - sessionId
+         - queryId
+
+        """
+        pass
+
     def addCatalogs(self, sessionId, jsonString):
         """
         Parameters:
          - sessionId
          - jsonString
 
         """
         pass
 
+    def getAddCatalogsResponse(self, sessionId):
+        """
+        Parameters:
+         - sessionId
+
+        """
+        pass
+
 
 class Client(Iface):
     def __init__(self, iprot, oprot=None):
         self._iprot = self._oprot = iprot
         if oprot is not None:
             self._oprot = oprot
         self._seqid = 0
@@ -880,31 +896,29 @@
             return result.success
         if result.error1 is not None:
             raise result.error1
         if result.error2 is not None:
             raise result.error2
         raise TApplicationException(TApplicationException.MISSING_RESULT, "getSchemaNamesV2 failed: unknown result")
 
-    def getColumns(self, sessionId, catalogName, schema, table):
+    def getColumns(self, sessionId, schema, table):
         """
         Parameters:
          - sessionId
-         - catalogName
          - schema
          - table
 
         """
-        self.send_getColumns(sessionId, catalogName, schema, table)
+        self.send_getColumns(sessionId, schema, table)
         return self.recv_getColumns()
 
-    def send_getColumns(self, sessionId, catalogName, schema, table):
+    def send_getColumns(self, sessionId, schema, table):
         self._oprot.writeMessageBegin('getColumns', TMessageType.CALL, self._seqid)
         args = getColumns_args()
         args.sessionId = sessionId
-        args.catalogName = catalogName
         args.schema = schema
         args.table = table
         args.write(self._oprot)
         self._oprot.writeMessageEnd()
         self._oprot.trans.flush()
 
     def recv_getColumns(self):
@@ -1032,14 +1046,52 @@
         result = setProps_result()
         result.read(iprot)
         iprot.readMessageEnd()
         if result.error2 is not None:
             raise result.error2
         return
 
+    def status(self, sessionId, queryId):
+        """
+        Parameters:
+         - sessionId
+         - queryId
+
+        """
+        self.send_status(sessionId, queryId)
+        return self.recv_status()
+
+    def send_status(self, sessionId, queryId):
+        self._oprot.writeMessageBegin('status', TMessageType.CALL, self._seqid)
+        args = status_args()
+        args.sessionId = sessionId
+        args.queryId = queryId
+        args.write(self._oprot)
+        self._oprot.writeMessageEnd()
+        self._oprot.trans.flush()
+
+    def recv_status(self):
+        iprot = self._iprot
+        (fname, mtype, rseqid) = iprot.readMessageBegin()
+        if mtype == TMessageType.EXCEPTION:
+            x = TApplicationException()
+            x.read(iprot)
+            iprot.readMessageEnd()
+            raise x
+        result = status_result()
+        result.read(iprot)
+        iprot.readMessageEnd()
+        if result.success is not None:
+            return result.success
+        if result.error1 is not None:
+            raise result.error1
+        if result.error2 is not None:
+            raise result.error2
+        raise TApplicationException(TApplicationException.MISSING_RESULT, "status failed: unknown result")
+
     def addCatalogs(self, sessionId, jsonString):
         """
         Parameters:
          - sessionId
          - jsonString
 
         """
@@ -1068,14 +1120,50 @@
         iprot.readMessageEnd()
         if result.error1 is not None:
             raise result.error1
         if result.error2 is not None:
             raise result.error2
         return
 
+    def getAddCatalogsResponse(self, sessionId):
+        """
+        Parameters:
+         - sessionId
+
+        """
+        self.send_getAddCatalogsResponse(sessionId)
+        return self.recv_getAddCatalogsResponse()
+
+    def send_getAddCatalogsResponse(self, sessionId):
+        self._oprot.writeMessageBegin('getAddCatalogsResponse', TMessageType.CALL, self._seqid)
+        args = getAddCatalogsResponse_args()
+        args.sessionId = sessionId
+        args.write(self._oprot)
+        self._oprot.writeMessageEnd()
+        self._oprot.trans.flush()
+
+    def recv_getAddCatalogsResponse(self):
+        iprot = self._iprot
+        (fname, mtype, rseqid) = iprot.readMessageBegin()
+        if mtype == TMessageType.EXCEPTION:
+            x = TApplicationException()
+            x.read(iprot)
+            iprot.readMessageEnd()
+            raise x
+        result = getAddCatalogsResponse_result()
+        result.read(iprot)
+        iprot.readMessageEnd()
+        if result.success is not None:
+            return result.success
+        if result.error1 is not None:
+            raise result.error1
+        if result.error2 is not None:
+            raise result.error2
+        raise TApplicationException(TApplicationException.MISSING_RESULT, "getAddCatalogsResponse failed: unknown result")
+
 
 class Processor(Iface, TProcessor):
     def __init__(self, handler):
         self._handler = handler
         self._processMap = {}
         self._processMap["clear"] = Processor.process_clear
         self._processMap["cancelQuery"] = Processor.process_cancelQuery
@@ -1094,15 +1182,17 @@
         self._processMap["getTablesV2"] = Processor.process_getTablesV2
         self._processMap["getSchemaNames"] = Processor.process_getSchemaNames
         self._processMap["getSchemaNamesV2"] = Processor.process_getSchemaNamesV2
         self._processMap["getColumns"] = Processor.process_getColumns
         self._processMap["getColumnsV2"] = Processor.process_getColumnsV2
         self._processMap["updateUsers"] = Processor.process_updateUsers
         self._processMap["setProps"] = Processor.process_setProps
+        self._processMap["status"] = Processor.process_status
         self._processMap["addCatalogs"] = Processor.process_addCatalogs
+        self._processMap["getAddCatalogsResponse"] = Processor.process_getAddCatalogsResponse
         self._on_message_begin = None
 
     def on_message_begin(self, func):
         self._on_message_begin = func
 
     def process(self, iprot, oprot):
         (name, type, seqid) = iprot.readMessageBegin()
@@ -1613,15 +1703,15 @@
 
     def process_getColumns(self, seqid, iprot, oprot):
         args = getColumns_args()
         args.read(iprot)
         iprot.readMessageEnd()
         result = getColumns_result()
         try:
-            result.success = self._handler.getColumns(args.sessionId, args.catalogName, args.schema, args.table)
+            result.success = self._handler.getColumns(args.sessionId, args.schema, args.table)
             msg_type = TMessageType.REPLY
         except TTransport.TTransportException:
             raise
         except QueryProcessingException as error1:
             msg_type = TMessageType.REPLY
             result.error1 = error1
         except AccessDeniedException as error2:
@@ -1720,14 +1810,43 @@
             msg_type = TMessageType.EXCEPTION
             result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
         oprot.writeMessageBegin("setProps", msg_type, seqid)
         result.write(oprot)
         oprot.writeMessageEnd()
         oprot.trans.flush()
 
+    def process_status(self, seqid, iprot, oprot):
+        args = status_args()
+        args.read(iprot)
+        iprot.readMessageEnd()
+        result = status_result()
+        try:
+            result.success = self._handler.status(args.sessionId, args.queryId)
+            msg_type = TMessageType.REPLY
+        except TTransport.TTransportException:
+            raise
+        except QueryProcessingException as error1:
+            msg_type = TMessageType.REPLY
+            result.error1 = error1
+        except AccessDeniedException as error2:
+            msg_type = TMessageType.REPLY
+            result.error2 = error2
+        except TApplicationException as ex:
+            logging.exception('TApplication exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = ex
+        except Exception:
+            logging.exception('Unexpected exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
+        oprot.writeMessageBegin("status", msg_type, seqid)
+        result.write(oprot)
+        oprot.writeMessageEnd()
+        oprot.trans.flush()
+
     def process_addCatalogs(self, seqid, iprot, oprot):
         args = addCatalogs_args()
         args.read(iprot)
         iprot.readMessageEnd()
         result = addCatalogs_result()
         try:
             self._handler.addCatalogs(args.sessionId, args.jsonString)
@@ -1749,14 +1868,43 @@
             msg_type = TMessageType.EXCEPTION
             result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
         oprot.writeMessageBegin("addCatalogs", msg_type, seqid)
         result.write(oprot)
         oprot.writeMessageEnd()
         oprot.trans.flush()
 
+    def process_getAddCatalogsResponse(self, seqid, iprot, oprot):
+        args = getAddCatalogsResponse_args()
+        args.read(iprot)
+        iprot.readMessageEnd()
+        result = getAddCatalogsResponse_result()
+        try:
+            result.success = self._handler.getAddCatalogsResponse(args.sessionId)
+            msg_type = TMessageType.REPLY
+        except TTransport.TTransportException:
+            raise
+        except QueryProcessingException as error1:
+            msg_type = TMessageType.REPLY
+            result.error1 = error1
+        except AccessDeniedException as error2:
+            msg_type = TMessageType.REPLY
+            result.error2 = error2
+        except TApplicationException as ex:
+            logging.exception('TApplication exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = ex
+        except Exception:
+            logging.exception('Unexpected exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
+        oprot.writeMessageBegin("getAddCatalogsResponse", msg_type, seqid)
+        result.write(oprot)
+        oprot.writeMessageEnd()
+        oprot.trans.flush()
+
 # HELPER FUNCTIONS AND STRUCTURES
 
 
 class clear_args(object):
     """
     Attributes:
      - sessionId
@@ -3947,18 +4095,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype10, _size7) = iprot.readListBegin()
-                    for _i11 in range(_size7):
-                        _elem12 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.success.append(_elem12)
+                    (_etype17, _size14) = iprot.readListBegin()
+                    for _i18 in range(_size14):
+                        _elem19 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.success.append(_elem19)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.error1 = QueryProcessingException.read(iprot)
                 else:
@@ -3977,16 +4125,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('getTables_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter13 in self.success:
-                oprot.writeString(iter13.encode('utf-8') if sys.version_info[0] == 2 else iter13)
+            for iter20 in self.success:
+                oprot.writeString(iter20.encode('utf-8') if sys.version_info[0] == 2 else iter20)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.error1 is not None:
             oprot.writeFieldBegin('error1', TType.STRUCT, 1)
             self.error1.write(oprot)
             oprot.writeFieldEnd()
         if self.error2 is not None:
@@ -4126,18 +4274,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype17, _size14) = iprot.readListBegin()
-                    for _i18 in range(_size14):
-                        _elem19 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.success.append(_elem19)
+                    (_etype24, _size21) = iprot.readListBegin()
+                    for _i25 in range(_size21):
+                        _elem26 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.success.append(_elem26)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.error1 = QueryProcessingException.read(iprot)
                 else:
@@ -4156,16 +4304,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('getTablesV2_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter20 in self.success:
-                oprot.writeString(iter20.encode('utf-8') if sys.version_info[0] == 2 else iter20)
+            for iter27 in self.success:
+                oprot.writeString(iter27.encode('utf-8') if sys.version_info[0] == 2 else iter27)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.error1 is not None:
             oprot.writeFieldBegin('error1', TType.STRUCT, 1)
             self.error1.write(oprot)
             oprot.writeFieldEnd()
         if self.error2 is not None:
@@ -4281,18 +4429,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype24, _size21) = iprot.readListBegin()
-                    for _i25 in range(_size21):
-                        _elem26 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.success.append(_elem26)
+                    (_etype31, _size28) = iprot.readListBegin()
+                    for _i32 in range(_size28):
+                        _elem33 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.success.append(_elem33)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.error1 = QueryProcessingException.read(iprot)
                 else:
@@ -4311,16 +4459,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('getSchemaNames_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter27 in self.success:
-                oprot.writeString(iter27.encode('utf-8') if sys.version_info[0] == 2 else iter27)
+            for iter34 in self.success:
+                oprot.writeString(iter34.encode('utf-8') if sys.version_info[0] == 2 else iter34)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.error1 is not None:
             oprot.writeFieldBegin('error1', TType.STRUCT, 1)
             self.error1.write(oprot)
             oprot.writeFieldEnd()
         if self.error2 is not None:
@@ -4448,18 +4596,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype31, _size28) = iprot.readListBegin()
-                    for _i32 in range(_size28):
-                        _elem33 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.success.append(_elem33)
+                    (_etype38, _size35) = iprot.readListBegin()
+                    for _i39 in range(_size35):
+                        _elem40 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.success.append(_elem40)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.error1 = QueryProcessingException.read(iprot)
                 else:
@@ -4478,16 +4626,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('getSchemaNamesV2_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter34 in self.success:
-                oprot.writeString(iter34.encode('utf-8') if sys.version_info[0] == 2 else iter34)
+            for iter41 in self.success:
+                oprot.writeString(iter41.encode('utf-8') if sys.version_info[0] == 2 else iter41)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.error1 is not None:
             oprot.writeFieldBegin('error1', TType.STRUCT, 1)
             self.error1.write(oprot)
             oprot.writeFieldEnd()
         if self.error2 is not None:
@@ -4518,24 +4666,22 @@
 )
 
 
 class getColumns_args(object):
     """
     Attributes:
      - sessionId
-     - catalogName
      - schema
      - table
 
     """
 
 
-    def __init__(self, sessionId=None, catalogName=None, schema=None, table=None,):
+    def __init__(self, sessionId=None, schema=None, table=None,):
         self.sessionId = sessionId
-        self.catalogName = catalogName
         self.schema = schema
         self.table = table
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
@@ -4547,23 +4693,18 @@
             if fid == 1:
                 if ftype == TType.STRING:
                     self.sessionId = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRING:
-                    self.catalogName = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                else:
-                    iprot.skip(ftype)
-            elif fid == 3:
-                if ftype == TType.STRING:
                     self.schema = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
-            elif fid == 4:
+            elif fid == 3:
                 if ftype == TType.STRING:
                     self.table = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
@@ -4574,24 +4715,20 @@
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('getColumns_args')
         if self.sessionId is not None:
             oprot.writeFieldBegin('sessionId', TType.STRING, 1)
             oprot.writeString(self.sessionId.encode('utf-8') if sys.version_info[0] == 2 else self.sessionId)
             oprot.writeFieldEnd()
-        if self.catalogName is not None:
-            oprot.writeFieldBegin('catalogName', TType.STRING, 2)
-            oprot.writeString(self.catalogName.encode('utf-8') if sys.version_info[0] == 2 else self.catalogName)
-            oprot.writeFieldEnd()
         if self.schema is not None:
-            oprot.writeFieldBegin('schema', TType.STRING, 3)
+            oprot.writeFieldBegin('schema', TType.STRING, 2)
             oprot.writeString(self.schema.encode('utf-8') if sys.version_info[0] == 2 else self.schema)
             oprot.writeFieldEnd()
         if self.table is not None:
-            oprot.writeFieldBegin('table', TType.STRING, 4)
+            oprot.writeFieldBegin('table', TType.STRING, 3)
             oprot.writeString(self.table.encode('utf-8') if sys.version_info[0] == 2 else self.table)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4606,17 +4743,16 @@
 
     def __ne__(self, other):
         return not (self == other)
 all_structs.append(getColumns_args)
 getColumns_args.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'sessionId', 'UTF8', None, ),  # 1
-    (2, TType.STRING, 'catalogName', 'UTF8', None, ),  # 2
-    (3, TType.STRING, 'schema', 'UTF8', None, ),  # 3
-    (4, TType.STRING, 'table', 'UTF8', None, ),  # 4
+    (2, TType.STRING, 'schema', 'UTF8', None, ),  # 2
+    (3, TType.STRING, 'table', 'UTF8', None, ),  # 3
 )
 
 
 class getColumns_result(object):
     """
     Attributes:
      - success
@@ -4639,19 +4775,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype38, _size35) = iprot.readListBegin()
-                    for _i39 in range(_size35):
-                        _elem40 = TFieldInfo()
-                        _elem40.read(iprot)
-                        self.success.append(_elem40)
+                    (_etype45, _size42) = iprot.readListBegin()
+                    for _i46 in range(_size42):
+                        _elem47 = TFieldInfo()
+                        _elem47.read(iprot)
+                        self.success.append(_elem47)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.error1 = QueryProcessingException.read(iprot)
                 else:
@@ -4670,16 +4806,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('getColumns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter41 in self.success:
-                iter41.write(oprot)
+            for iter48 in self.success:
+                iter48.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.error1 is not None:
             oprot.writeFieldBegin('error1', TType.STRUCT, 1)
             self.error1.write(oprot)
             oprot.writeFieldEnd()
         if self.error2 is not None:
@@ -4831,19 +4967,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype45, _size42) = iprot.readListBegin()
-                    for _i46 in range(_size42):
-                        _elem47 = TFieldInfo()
-                        _elem47.read(iprot)
-                        self.success.append(_elem47)
+                    (_etype52, _size49) = iprot.readListBegin()
+                    for _i53 in range(_size49):
+                        _elem54 = TFieldInfo()
+                        _elem54.read(iprot)
+                        self.success.append(_elem54)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.error1 = QueryProcessingException.read(iprot)
                 else:
@@ -4862,16 +4998,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('getColumnsV2_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter48 in self.success:
-                iter48.write(oprot)
+            for iter55 in self.success:
+                iter55.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.error1 is not None:
             oprot.writeFieldBegin('error1', TType.STRUCT, 1)
             self.error1.write(oprot)
             oprot.writeFieldEnd()
         if self.error2 is not None:
@@ -5170,14 +5306,174 @@
 all_structs.append(setProps_result)
 setProps_result.thrift_spec = (
     None,  # 0
     (1, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 1
 )
 
 
+class status_args(object):
+    """
+    Attributes:
+     - sessionId
+     - queryId
+
+    """
+
+
+    def __init__(self, sessionId=None, queryId=None,):
+        self.sessionId = sessionId
+        self.queryId = queryId
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRING:
+                    self.sessionId = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRING:
+                    self.queryId = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('status_args')
+        if self.sessionId is not None:
+            oprot.writeFieldBegin('sessionId', TType.STRING, 1)
+            oprot.writeString(self.sessionId.encode('utf-8') if sys.version_info[0] == 2 else self.sessionId)
+            oprot.writeFieldEnd()
+        if self.queryId is not None:
+            oprot.writeFieldBegin('queryId', TType.STRING, 2)
+            oprot.writeString(self.queryId.encode('utf-8') if sys.version_info[0] == 2 else self.queryId)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(status_args)
+status_args.thrift_spec = (
+    None,  # 0
+    (1, TType.STRING, 'sessionId', 'UTF8', None, ),  # 1
+    (2, TType.STRING, 'queryId', 'UTF8', None, ),  # 2
+)
+
+
+class status_result(object):
+    """
+    Attributes:
+     - success
+     - error1
+     - error2
+
+    """
+
+
+    def __init__(self, success=None, error1=None, error2=None,):
+        self.success = success
+        self.error1 = error1
+        self.error2 = error2
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 0:
+                if ftype == TType.STRUCT:
+                    self.success = Status()
+                    self.success.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 1:
+                if ftype == TType.STRUCT:
+                    self.error1 = QueryProcessingException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRUCT:
+                    self.error2 = AccessDeniedException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('status_result')
+        if self.success is not None:
+            oprot.writeFieldBegin('success', TType.STRUCT, 0)
+            self.success.write(oprot)
+            oprot.writeFieldEnd()
+        if self.error1 is not None:
+            oprot.writeFieldBegin('error1', TType.STRUCT, 1)
+            self.error1.write(oprot)
+            oprot.writeFieldEnd()
+        if self.error2 is not None:
+            oprot.writeFieldBegin('error2', TType.STRUCT, 2)
+            self.error2.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(status_result)
+status_result.thrift_spec = (
+    (0, TType.STRUCT, 'success', [Status, None], None, ),  # 0
+    (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
+    (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
+)
+
+
 class addCatalogs_args(object):
     """
     Attributes:
      - sessionId
      - jsonString
 
     """
@@ -5316,9 +5612,157 @@
         return not (self == other)
 all_structs.append(addCatalogs_result)
 addCatalogs_result.thrift_spec = (
     None,  # 0
     (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
     (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
 )
+
+
+class getAddCatalogsResponse_args(object):
+    """
+    Attributes:
+     - sessionId
+
+    """
+
+
+    def __init__(self, sessionId=None,):
+        self.sessionId = sessionId
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRING:
+                    self.sessionId = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('getAddCatalogsResponse_args')
+        if self.sessionId is not None:
+            oprot.writeFieldBegin('sessionId', TType.STRING, 1)
+            oprot.writeString(self.sessionId.encode('utf-8') if sys.version_info[0] == 2 else self.sessionId)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(getAddCatalogsResponse_args)
+getAddCatalogsResponse_args.thrift_spec = (
+    None,  # 0
+    (1, TType.STRING, 'sessionId', 'UTF8', None, ),  # 1
+)
+
+
+class getAddCatalogsResponse_result(object):
+    """
+    Attributes:
+     - success
+     - error1
+     - error2
+
+    """
+
+
+    def __init__(self, success=None, error1=None, error2=None,):
+        self.success = success
+        self.error1 = error1
+        self.error2 = error2
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 0:
+                if ftype == TType.STRUCT:
+                    self.success = AddCatalogsResponse()
+                    self.success.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 1:
+                if ftype == TType.STRUCT:
+                    self.error1 = QueryProcessingException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRUCT:
+                    self.error2 = AccessDeniedException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('getAddCatalogsResponse_result')
+        if self.success is not None:
+            oprot.writeFieldBegin('success', TType.STRUCT, 0)
+            self.success.write(oprot)
+            oprot.writeFieldEnd()
+        if self.error1 is not None:
+            oprot.writeFieldBegin('error1', TType.STRUCT, 1)
+            self.error1.write(oprot)
+            oprot.writeFieldEnd()
+        if self.error2 is not None:
+            oprot.writeFieldBegin('error2', TType.STRUCT, 2)
+            self.error2.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(getAddCatalogsResponse_result)
+getAddCatalogsResponse_result.thrift_spec = (
+    (0, TType.STRUCT, 'success', [AddCatalogsResponse, None], None, ),  # 0
+    (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
+    (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
+)
 fix_spec(all_structs)
 del all_structs
```

### Comparing `e6data-python-connector-1.0.6/e6xdb/server/ttypes.py` & `e6data-python-connector-1.0.7/e6xdb/server/ttypes.py`

 * *Files 24% similar despite different names*

```diff
@@ -324,14 +324,238 @@
         return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
 
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
+
+
+class Status(object):
+    """
+    Attributes:
+     - status
+     - rowCount
+
+    """
+
+
+    def __init__(self, status=None, rowCount=None,):
+        self.status = status
+        self.rowCount = rowCount
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BOOL:
+                    self.status = iprot.readBool()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I64:
+                    self.rowCount = iprot.readI64()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('Status')
+        if self.status is not None:
+            oprot.writeFieldBegin('status', TType.BOOL, 1)
+            oprot.writeBool(self.status)
+            oprot.writeFieldEnd()
+        if self.rowCount is not None:
+            oprot.writeFieldBegin('rowCount', TType.I64, 2)
+            oprot.writeI64(self.rowCount)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FailedSchemaElement(object):
+    """
+    Attributes:
+     - name
+     - type
+     - reason
+
+    """
+
+
+    def __init__(self, name=None, type=None, reason=None,):
+        self.name = name
+        self.type = type
+        self.reason = reason
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRING:
+                    self.name = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRING:
+                    self.type = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.STRING:
+                    self.reason = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FailedSchemaElement')
+        if self.name is not None:
+            oprot.writeFieldBegin('name', TType.STRING, 1)
+            oprot.writeString(self.name.encode('utf-8') if sys.version_info[0] == 2 else self.name)
+            oprot.writeFieldEnd()
+        if self.type is not None:
+            oprot.writeFieldBegin('type', TType.STRING, 2)
+            oprot.writeString(self.type.encode('utf-8') if sys.version_info[0] == 2 else self.type)
+            oprot.writeFieldEnd()
+        if self.reason is not None:
+            oprot.writeFieldBegin('reason', TType.STRING, 3)
+            oprot.writeString(self.reason.encode('utf-8') if sys.version_info[0] == 2 else self.reason)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class AddCatalogsResponse(object):
+    """
+    Attributes:
+     - status
+     - failures
+
+    """
+
+
+    def __init__(self, status=None, failures=None,):
+        self.status = status
+        self.failures = failures
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRING:
+                    self.status = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.LIST:
+                    self.failures = []
+                    (_etype10, _size7) = iprot.readListBegin()
+                    for _i11 in range(_size7):
+                        _elem12 = FailedSchemaElement()
+                        _elem12.read(iprot)
+                        self.failures.append(_elem12)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('AddCatalogsResponse')
+        if self.status is not None:
+            oprot.writeFieldBegin('status', TType.STRING, 1)
+            oprot.writeString(self.status.encode('utf-8') if sys.version_info[0] == 2 else self.status)
+            oprot.writeFieldEnd()
+        if self.failures is not None:
+            oprot.writeFieldBegin('failures', TType.LIST, 2)
+            oprot.writeListBegin(TType.STRUCT, len(self.failures))
+            for iter13 in self.failures:
+                iter13.write(oprot)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
 all_structs.append(QueryProcessingException)
 QueryProcessingException.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'reason', 'UTF8', None, ),  # 1
     (2, TType.STRING, 'queryId', 'UTF8', None, ),  # 2
 )
 all_structs.append(AccessDeniedException)
@@ -348,9 +572,28 @@
 all_structs.append(UserAccessInfo)
 UserAccessInfo.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'uuid', 'UTF8', None, ),  # 1
     (2, TType.STRING, 'userName', 'UTF8', None, ),  # 2
     (3, TType.LIST, 'tokens', (TType.STRING, 'UTF8', False), None, ),  # 3
 )
+all_structs.append(Status)
+Status.thrift_spec = (
+    None,  # 0
+    (1, TType.BOOL, 'status', None, None, ),  # 1
+    (2, TType.I64, 'rowCount', None, None, ),  # 2
+)
+all_structs.append(FailedSchemaElement)
+FailedSchemaElement.thrift_spec = (
+    None,  # 0
+    (1, TType.STRING, 'name', 'UTF8', None, ),  # 1
+    (2, TType.STRING, 'type', 'UTF8', None, ),  # 2
+    (3, TType.STRING, 'reason', 'UTF8', None, ),  # 3
+)
+all_structs.append(AddCatalogsResponse)
+AddCatalogsResponse.thrift_spec = (
+    None,  # 0
+    (1, TType.STRING, 'status', 'UTF8', None, ),  # 1
+    (2, TType.LIST, 'failures', (TType.STRUCT, [FailedSchemaElement, None], False), None, ),  # 2
+)
 fix_spec(all_structs)
 del all_structs
```

### Comparing `e6data-python-connector-1.0.6/e6xdb/sqlalchemy_e6x.py` & `e6data-python-connector-1.0.7/e6xdb/sqlalchemy_e6x.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.6/e6xdb/typeId.py` & `e6data-python-connector-1.0.7/e6xdb/typeId.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.6/setup.py` & `e6data-python-connector-1.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import os
 
 import setuptools
 
 envstring = lambda var: os.environ.get(var) or ""
 
-VERSION = [1, 0, 6]
+VERSION = [1, 0, 7]
 
 
 def get_long_desc():
     with open("README.md", "r") as fh:
         long_description = fh.read()
     return long_description
```

