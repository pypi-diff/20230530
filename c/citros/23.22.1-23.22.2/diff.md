# Comparing `tmp/citros-23.22.1.tar.gz` & `tmp/citros-23.22.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.22.1.tar", last modified: Mon May 29 19:04:08 2023, max compression
+gzip compressed data, was "citros-23.22.2.tar", last modified: Tue May 30 10:47:03 2023, max compression
```

## Comparing `citros-23.22.1.tar` & `citros-23.22.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:04:08.784710 citros-23.22.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 19:03:53.000000 citros-23.22.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-29 19:04:08.780710 citros-23.22.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-29 19:03:53.000000 citros-23.22.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:04:08.780710 citros-23.22.1/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-05-29 19:03:53.000000 citros-23.22.1/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:04:08.780710 citros-23.22.1/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-29 19:03:53.000000 citros-23.22.1/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-05-29 19:03:53.000000 citros-23.22.1/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    13838 2023-05-29 19:03:53.000000 citros-23.22.1/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-29 19:03:53.000000 citros-23.22.1/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-29 19:03:53.000000 citros-23.22.1/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-05-29 19:03:53.000000 citros-23.22.1/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-05-29 19:03:53.000000 citros-23.22.1/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-29 19:03:53.000000 citros-23.22.1/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:04:08.780710 citros-23.22.1/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-29 19:03:53.000000 citros-23.22.1/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-29 19:03:53.000000 citros-23.22.1/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:04:08.780710 citros-23.22.1/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-29 19:03:53.000000 citros-23.22.1/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-29 19:03:53.000000 citros-23.22.1/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-29 19:03:53.000000 citros-23.22.1/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:04:08.780710 citros-23.22.1/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-29 19:03:53.000000 citros-23.22.1/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 19:03:53.000000 citros-23.22.1/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18298 2023-05-29 19:03:53.000000 citros-23.22.1/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:04:08.780710 citros-23.22.1/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-29 19:03:53.000000 citros-23.22.1/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-29 19:03:53.000000 citros-23.22.1/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-29 19:03:53.000000 citros-23.22.1/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-29 19:03:53.000000 citros-23.22.1/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:04:08.780710 citros-23.22.1/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-29 19:04:08.000000 citros-23.22.1/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-29 19:04:08.000000 citros-23.22.1/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:04:08.000000 citros-23.22.1/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-29 19:04:08.000000 citros-23.22.1/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 19:04:08.000000 citros-23.22.1/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-29 19:03:53.000000 citros-23.22.1/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:04:08.784710 citros-23.22.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-29 19:03:53.000000 citros-23.22.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:04:08.780710 citros-23.22.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:03:53.000000 citros-23.22.1/tests/test_parse_ros_project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:03:53.000000 citros-23.22.1/tests/test_uplosd_to_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 10:46:45.000000 citros-23.22.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-30 10:47:03.120994 citros-23.22.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-30 10:46:45.000000 citros-23.22.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.116994 citros-23.22.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-05-30 10:46:45.000000 citros-23.22.2/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-30 10:46:45.000000 citros-23.22.2/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13838 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-30 10:46:45.000000 citros-23.22.2/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-30 10:46:45.000000 citros-23.22.2/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-30 10:46:45.000000 citros-23.22.2/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-30 10:46:45.000000 citros-23.22.2/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-30 10:46:45.000000 citros-23.22.2/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-30 10:46:45.000000 citros-23.22.2/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 10:46:45.000000 citros-23.22.2/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18298 2023-05-30 10:46:45.000000 citros-23.22.2/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-30 10:46:45.000000 citros-23.22.2/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-30 10:46:45.000000 citros-23.22.2/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-30 10:46:45.000000 citros-23.22.2/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-30 10:46:45.000000 citros-23.22.2/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-30 10:47:03.000000 citros-23.22.2/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-30 10:47:03.000000 citros-23.22.2/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:47:03.000000 citros-23.22.2/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-30 10:47:03.000000 citros-23.22.2/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 10:47:03.000000 citros-23.22.2/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-30 10:46:45.000000 citros-23.22.2/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:47:03.120994 citros-23.22.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-30 10:46:45.000000 citros-23.22.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:46:45.000000 citros-23.22.2/tests/test_parse_ros_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:46:45.000000 citros-23.22.2/tests/test_uplosd_to_server.py
```

### Comparing `citros-23.22.1/LICENSE` & `citros-23.22.2/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/PKG-INFO` & `citros-23.22.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.22.1
+Version: 23.22.2
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.22.1/README.md` & `citros-23.22.2/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/bin/citros` & `citros-23.22.2/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/__init__.py` & `citros-23.22.2/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/citros.py` & `citros-23.22.2/citros/citros.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,20 @@
         # if self.init: # init only once. 
         #     return
         # self.init = True
         
         self.CONFIG_DIR = ".citros"
                     
         self._user = None
+        # do not access directly, only via get/set token.
         self._jwt_token = None
         
         # GQL
         self._gql_client = None
+        self._token_changed = False
         
         # for logger
         self.batch_run_id = batch_run_id
         self.simulation_run_id = simulation_run_id    
         
         self.CITROS_DOMAIN = config("CITROS_DOMAIN", "https://citros.io")
         print(f"--- using self.CITROS_DOMAIN = {self.CITROS_DOMAIN}")
@@ -92,14 +94,15 @@
         self._set_token(None)
         
     def _set_token(self, jwt_token):
         #TODO: check token validity
         # print(f"jwt_token [{jwt_token}]")
         if not jwt_token or jwt_token == '':
             self._jwt_token = None
+            self._token_changed = True
             try:
                 os.remove(f"{self.CONFIG_DIR}/auth")
                 return
             except FileNotFoundError as e:
                 return # its ok that there is no file.                
             except Exception as e:
                 self.log.exception(e)       
@@ -116,25 +119,27 @@
         except FileNotFoundError as e:
             self.log.exception(e)
             traceback.print_exc()
         except Exception as e:
             self.log.exception(e)
             traceback.print_exc()
         finally:
-            self._jwt_token = jwt_token                        
+            self._jwt_token = jwt_token
+            self._token_changed = True                        
         
         return self._jwt_token
     
     def _get_token(self):
         try:
             if self._jwt_token:
                 return self._jwt_token
             
             with open(f"{self.CONFIG_DIR}/auth", mode='r') as file:            
                 self._jwt_token = file.read()
+                self._token_changed = True
         except FileNotFoundError as e:
             # Key file wasn't found. assuming the user is not logged in...
             self._jwt_token = None
             return None
         except Exception as e:
             self.log.exception(e)
             traceback.print_exc()
@@ -350,19 +355,20 @@
         if self.isAuthenticated():
             transport.headers = {
                 "Authorization": f"Bearer {self._get_token()}"
             }
         return transport
 
     def _get_gql_client(self):
-        if self._gql_client:
+        if self._gql_client and not self._token_changed:
             return self._gql_client
         # https://gql.readthedocs.io/en/v3.0.0a6/intro.html
         transport = self._get_transport()
         self._gql_client = Client(transport=transport, fetch_schema_from_transport=False)
+        self._token_changed = False
         return self._gql_client
         
     def gql_execute(self, query, variable_values=None):
         """_summary_
 
         Args:
             query (gql): gql query
```

### Comparing `citros-23.22.1/citros/citros_bag.py` & `citros-23.22.2/citros/citros_bag.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/citros_batch.py` & `citros-23.22.2/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/citros_events.py` & `citros-23.22.2/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/citros_integration.py` & `citros-23.22.2/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/citros_params.py` & `citros-23.22.2/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/citros_utils.py` & `citros-23.22.2/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/launches/__init__.py` & `citros-23.22.2/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/launches/launch.py` & `citros-23.22.2/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/logger/__init__.py` & `citros-23.22.2/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/logger/logger.py` & `citros-23.22.2/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/logger/logger_pg_handler.py` & `citros-23.22.2/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/parsers/__init__.py` & `citros-23.22.2/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/parsers/parser_ros2.py` & `citros-23.22.2/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/rosbag/__init__.py` & `citros-23.22.2/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/rosbag/reader_base.py` & `citros-23.22.2/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/rosbag/reader_mcap.py` & `citros-23.22.2/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros/rosbag/reader_sqlite.py` & `citros-23.22.2/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/citros.egg-info/PKG-INFO` & `citros-23.22.2/citros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.22.1
+Version: 23.22.2
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.22.1/citros.egg-info/SOURCES.txt` & `citros-23.22.2/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.22.1/setup.py` & `citros-23.22.2/setup.py`

 * *Files identical despite different names*

