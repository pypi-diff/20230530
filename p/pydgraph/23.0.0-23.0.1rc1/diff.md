# Comparing `tmp/pydgraph-23.0.0.tar.gz` & `tmp/pydgraph-23.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydgraph-23.0.0.tar", last modified: Thu May 25 17:44:20 2023, max compression
+gzip compressed data, was "pydgraph-23.0.1rc1.tar", last modified: Tue May 30 10:07:24 2023, max compression
```

## Comparing `pydgraph-23.0.0.tar` & `pydgraph-23.0.1rc1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:44:20.046277 pydgraph-23.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (122)    10172 2023-05-25 17:42:30.000000 pydgraph-23.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    29505 2023-05-25 17:44:20.046277 pydgraph-23.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17322 2023-05-25 17:42:30.000000 pydgraph-23.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:44:20.042277 pydgraph-23.0.0/pydgraph/
--rwxr-xr-x   0 runner    (1001) docker     (122)      849 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6648 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4662 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/client_stub.py
--rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:44:20.046277 pydgraph-23.0.0/pydgraph/proto/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7961 2023-05-25 17:44:13.000000 pydgraph-23.0.0/pydgraph/proto/api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     7821 2023-05-25 17:44:13.000000 pydgraph-23.0.0/pydgraph/proto/api_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    12606 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/txn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1952 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:44:20.046277 pydgraph-23.0.0/pydgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    29505 2023-05-25 17:44:20.000000 pydgraph-23.0.0/pydgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      698 2023-05-25 17:44:20.000000 pydgraph-23.0.0/pydgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 17:44:20.000000 pydgraph-23.0.0/pydgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-25 17:44:20.000000 pydgraph-23.0.0/pydgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-25 17:44:20.000000 pydgraph-23.0.0/pydgraph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 17:44:20.046277 pydgraph-23.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:44:20.046277 pydgraph-23.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     7787 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_acct_upsert.py
--rw-r--r--   0 runner    (1001) docker     (122)     5185 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_acl.py
--rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     2984 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_client_stub.py
--rw-r--r--   0 runner    (1001) docker     (122)    16449 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     1946 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_essentials.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3882 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (122)    18545 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_txn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_type_system.py
--rw-r--r--   0 runner    (1001) docker     (122)     5986 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_upsert_block.py
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 10:07:24.859842 pydgraph-23.0.1rc1/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10172 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    29295 2023-05-30 10:07:24.859842 pydgraph-23.0.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17109 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 10:07:24.855842 pydgraph-23.0.1rc1/pydgraph/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      849 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/pydgraph/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6648 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/pydgraph/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4662 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/pydgraph/client_stub.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/pydgraph/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/pydgraph/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/pydgraph/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 10:07:24.855842 pydgraph-23.0.1rc1/pydgraph/proto/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/pydgraph/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7961 2023-05-30 10:07:16.000000 pydgraph-23.0.1rc1/pydgraph/proto/api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7821 2023-05-30 10:07:16.000000 pydgraph-23.0.1rc1/pydgraph/proto/api_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12606 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/pydgraph/txn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1952 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/pydgraph/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 10:07:24.855842 pydgraph-23.0.1rc1/pydgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    29295 2023-05-30 10:07:24.000000 pydgraph-23.0.1rc1/pydgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-05-30 10:07:24.000000 pydgraph-23.0.1rc1/pydgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 10:07:24.000000 pydgraph-23.0.1rc1/pydgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-30 10:07:24.000000 pydgraph-23.0.1rc1/pydgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-30 10:07:24.000000 pydgraph-23.0.1rc1/pydgraph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 10:07:24.859842 pydgraph-23.0.1rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 10:07:24.859842 pydgraph-23.0.1rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     7787 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/tests/test_acct_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5185 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/tests/test_acl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2984 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/tests/test_client_stub.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16449 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1946 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/tests/test_essentials.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3882 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18545 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/tests/test_txn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/tests/test_type_system.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5986 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/tests/test_upsert_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-05-30 10:06:41.000000 pydgraph-23.0.1rc1/tests/test_util.py
```

### Comparing `pydgraph-23.0.0/LICENSE` & `pydgraph-23.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/PKG-INFO` & `pydgraph-23.0.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydgraph
-Version: 23.0.0
+Version: 23.0.1rc1
 Summary: Official Dgraph client implementation for Python
 Author-email: Dgraph Labs <contact@dgraph.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -712,22 +712,14 @@
 
 [grpcio-tools]: https://pypi.python.org/pypi/grpcio-tools
 
 ```sh
 python scripts/protogen.py
 ```
 
-The generated file `api_pb2_grpc.py` needs to be changed in recent versions of python.
-The required change is outlined below as a diff.
-
-```diff
--import api_pb2 as api__pb2
-+from . import api_pb2 as api__pb2
-```
-
 ### Running tests
 
 To run the tests in your local machine, run:
 
 ```bash
 bash scripts/local-test.sh
 ```
```

### Comparing `pydgraph-23.0.0/README.md` & `pydgraph-23.0.1rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -519,22 +519,14 @@
 
 [grpcio-tools]: https://pypi.python.org/pypi/grpcio-tools
 
 ```sh
 python scripts/protogen.py
 ```
 
-The generated file `api_pb2_grpc.py` needs to be changed in recent versions of python.
-The required change is outlined below as a diff.
-
-```diff
--import api_pb2 as api__pb2
-+from . import api_pb2 as api__pb2
-```
-
 ### Running tests
 
 To run the tests in your local machine, run:
 
 ```bash
 bash scripts/local-test.sh
 ```
```

### Comparing `pydgraph-23.0.0/pydgraph/__init__.py` & `pydgraph-23.0.1rc1/pydgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/pydgraph/client.py` & `pydgraph-23.0.1rc1/pydgraph/client.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/pydgraph/client_stub.py` & `pydgraph-23.0.1rc1/pydgraph/client_stub.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/pydgraph/convert.py` & `pydgraph-23.0.1rc1/pydgraph/convert.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/pydgraph/errors.py` & `pydgraph-23.0.1rc1/pydgraph/errors.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/pydgraph/meta.py` & `pydgraph-23.0.1rc1/pydgraph/meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Metadata about this package."""
 
-VERSION = '23.0.0'
+VERSION = '23.0.1rc1'
```

### Comparing `pydgraph-23.0.0/pydgraph/proto/api_pb2.py` & `pydgraph-23.0.1rc1/pydgraph/proto/api_pb2.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/pydgraph/proto/api_pb2_grpc.py` & `pydgraph-23.0.1rc1/pydgraph/proto/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/pydgraph/txn.py` & `pydgraph-23.0.1rc1/pydgraph/txn.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/pydgraph/util.py` & `pydgraph-23.0.1rc1/pydgraph/util.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/pydgraph.egg-info/PKG-INFO` & `pydgraph-23.0.1rc1/pydgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydgraph
-Version: 23.0.0
+Version: 23.0.1rc1
 Summary: Official Dgraph client implementation for Python
 Author-email: Dgraph Labs <contact@dgraph.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -712,22 +712,14 @@
 
 [grpcio-tools]: https://pypi.python.org/pypi/grpcio-tools
 
 ```sh
 python scripts/protogen.py
 ```
 
-The generated file `api_pb2_grpc.py` needs to be changed in recent versions of python.
-The required change is outlined below as a diff.
-
-```diff
--import api_pb2 as api__pb2
-+from . import api_pb2 as api__pb2
-```
-
 ### Running tests
 
 To run the tests in your local machine, run:
 
 ```bash
 bash scripts/local-test.sh
 ```
```

### Comparing `pydgraph-23.0.0/pydgraph.egg-info/SOURCES.txt` & `pydgraph-23.0.1rc1/pydgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/pyproject.toml` & `pydgraph-23.0.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/tests/test_acct_upsert.py` & `pydgraph-23.0.1rc1/tests/test_acct_upsert.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/tests/test_acl.py` & `pydgraph-23.0.1rc1/tests/test_acl.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/tests/test_async.py` & `pydgraph-23.0.1rc1/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/tests/test_client.py` & `pydgraph-23.0.1rc1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/tests/test_client_stub.py` & `pydgraph-23.0.1rc1/tests/test_client_stub.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/tests/test_convert.py` & `pydgraph-23.0.1rc1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/tests/test_essentials.py` & `pydgraph-23.0.1rc1/tests/test_essentials.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/tests/test_queries.py` & `pydgraph-23.0.1rc1/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/tests/test_txn.py` & `pydgraph-23.0.1rc1/tests/test_txn.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/tests/test_type_system.py` & `pydgraph-23.0.1rc1/tests/test_type_system.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/tests/test_upsert_block.py` & `pydgraph-23.0.1rc1/tests/test_upsert_block.py`

 * *Files identical despite different names*

### Comparing `pydgraph-23.0.0/tests/test_util.py` & `pydgraph-23.0.1rc1/tests/test_util.py`

 * *Files identical despite different names*

