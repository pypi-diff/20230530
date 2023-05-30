# Comparing `tmp/substrait-0.0.1.tar.gz` & `tmp/substrait-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrait-0.0.1.tar", last modified: Thu May 18 18:44:42 2023, max compression
+gzip compressed data, was "substrait-0.1.0.tar", last modified: Tue May 30 19:42:04 2023, max compression
```

## Comparing `substrait-0.0.1.tar` & `substrait-0.1.0.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxrwxr-x   0 gil       (1000) gil       (1000)        0 2023-05-18 18:44:42.390785 substrait-0.0.1/
--rw-rw-r--   0 gil       (1000) gil       (1000)       45 2023-05-18 18:36:42.000000 substrait-0.0.1/.gitattributes
--rw-rw-r--   0 gil       (1000) gil       (1000)     2020 2023-05-18 18:36:42.000000 substrait-0.0.1/.gitignore
--rw-rw-r--   0 gil       (1000) gil       (1000)      115 2023-05-18 18:36:42.000000 substrait-0.0.1/.gitmodules
--rw-rw-r--   0 gil       (1000) gil       (1000)     1004 2023-05-18 18:36:42.000000 substrait-0.0.1/CONTRIBUTING.md
--rw-rw-r--   0 gil       (1000) gil       (1000)    11357 2023-05-18 18:36:42.000000 substrait-0.0.1/LICENSE
--rw-rw-r--   0 gil       (1000) gil       (1000)     4468 2023-05-18 18:44:42.390785 substrait-0.0.1/PKG-INFO
--rw-rw-r--   0 gil       (1000) gil       (1000)     4153 2023-05-18 18:36:42.000000 substrait-0.0.1/README.md
--rw-rw-r--   0 gil       (1000) gil       (1000)       65 2023-05-18 18:36:42.000000 substrait-0.0.1/buf.gen.yaml
--rw-rw-r--   0 gil       (1000) gil       (1000)       42 2023-05-18 18:36:42.000000 substrait-0.0.1/buf.work.yaml
--rw-rw-r--   0 gil       (1000) gil       (1000)       67 2023-05-18 18:36:42.000000 substrait-0.0.1/buf.yaml
--rw-rw-r--   0 gil       (1000) gil       (1000)      286 2023-05-18 18:36:42.000000 substrait-0.0.1/environment.yml
--rwxrwxr-x   0 gil       (1000) gil       (1000)      637 2023-05-18 18:36:42.000000 substrait-0.0.1/gen_proto.sh
--rw-rw-r--   0 gil       (1000) gil       (1000)      650 2023-05-18 18:39:01.000000 substrait-0.0.1/pyproject.toml
--rw-rw-r--   0 gil       (1000) gil       (1000)       38 2023-05-18 18:44:42.390785 substrait-0.0.1/setup.cfg
-drwxrwxr-x   0 gil       (1000) gil       (1000)        0 2023-05-18 18:44:42.382785 substrait-0.0.1/src/
-drwxrwxr-x   0 gil       (1000) gil       (1000)        0 2023-05-18 18:44:42.386785 substrait-0.0.1/src/substrait/
--rw-rw-r--   0 gil       (1000) gil       (1000)       72 2023-05-18 18:41:51.000000 substrait-0.0.1/src/substrait/__init__.py
--rw-rw-r--   0 gil       (1000) gil       (1000)      160 2023-05-18 18:44:42.000000 substrait-0.0.1/src/substrait/_version.py
-drwxrwxr-x   0 gil       (1000) gil       (1000)        0 2023-05-18 18:44:42.386785 substrait-0.0.1/src/substrait/gen/
--rw-rw-r--   0 gil       (1000) gil       (1000)        0 2023-05-18 18:36:42.000000 substrait-0.0.1/src/substrait/gen/__init__.py
-drwxrwxr-x   0 gil       (1000) gil       (1000)        0 2023-05-18 18:44:42.386785 substrait-0.0.1/src/substrait/gen/proto/
--rw-rw-r--   0 gil       (1000) gil       (1000)        0 2023-05-18 18:36:42.000000 substrait-0.0.1/src/substrait/gen/proto/__init__.py
--rw-rw-r--   0 gil       (1000) gil       (1000)    47948 2023-05-18 18:36:42.000000 substrait-0.0.1/src/substrait/gen/proto/algebra_pb2.py
--rw-rw-r--   0 gil       (1000) gil       (1000)     1527 2023-05-18 18:36:42.000000 substrait-0.0.1/src/substrait/gen/proto/capabilities_pb2.py
--rw-rw-r--   0 gil       (1000) gil       (1000)     2268 2023-05-18 18:36:42.000000 substrait-0.0.1/src/substrait/gen/proto/extended_expression_pb2.py
-drwxrwxr-x   0 gil       (1000) gil       (1000)        0 2023-05-18 18:44:42.390785 substrait-0.0.1/src/substrait/gen/proto/extensions/
--rw-rw-r--   0 gil       (1000) gil       (1000)        0 2023-05-18 18:36:42.000000 substrait-0.0.1/src/substrait/gen/proto/extensions/__init__.py
--rw-rw-r--   0 gil       (1000) gil       (1000)     3127 2023-05-18 18:36:42.000000 substrait-0.0.1/src/substrait/gen/proto/extensions/extensions_pb2.py
--rw-rw-r--   0 gil       (1000) gil       (1000)     7587 2023-05-18 18:36:42.000000 substrait-0.0.1/src/substrait/gen/proto/function_pb2.py
--rw-rw-r--   0 gil       (1000) gil       (1000)     8257 2023-05-18 18:36:42.000000 substrait-0.0.1/src/substrait/gen/proto/parameterized_types_pb2.py
--rw-rw-r--   0 gil       (1000) gil       (1000)     2341 2023-05-18 18:36:42.000000 substrait-0.0.1/src/substrait/gen/proto/plan_pb2.py
--rw-rw-r--   0 gil       (1000) gil       (1000)    10190 2023-05-18 18:36:42.000000 substrait-0.0.1/src/substrait/gen/proto/type_expressions_pb2.py
--rw-rw-r--   0 gil       (1000) gil       (1000)    10975 2023-05-18 18:36:42.000000 substrait-0.0.1/src/substrait/gen/proto/type_pb2.py
-drwxrwxr-x   0 gil       (1000) gil       (1000)        0 2023-05-18 18:44:42.386785 substrait-0.0.1/src/substrait.egg-info/
--rw-rw-r--   0 gil       (1000) gil       (1000)     4468 2023-05-18 18:44:42.000000 substrait-0.0.1/src/substrait.egg-info/PKG-INFO
--rw-rw-r--   0 gil       (1000) gil       (1000)      918 2023-05-18 18:44:42.000000 substrait-0.0.1/src/substrait.egg-info/SOURCES.txt
--rw-rw-r--   0 gil       (1000) gil       (1000)        1 2023-05-18 18:44:42.000000 substrait-0.0.1/src/substrait.egg-info/dependency_links.txt
--rw-rw-r--   0 gil       (1000) gil       (1000)       88 2023-05-18 18:44:42.000000 substrait-0.0.1/src/substrait.egg-info/requires.txt
--rw-rw-r--   0 gil       (1000) gil       (1000)       10 2023-05-18 18:44:42.000000 substrait-0.0.1/src/substrait.egg-info/top_level.txt
-drwxrwxr-x   0 gil       (1000) gil       (1000)        0 2023-05-18 18:44:42.390785 substrait-0.0.1/tests/
--rw-rw-r--   0 gil       (1000) gil       (1000)      660 2023-05-18 18:36:42.000000 substrait-0.0.1/tests/test_proto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.369334 substrait-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 19:41:51.000000 substrait-0.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.353334 substrait-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.361334 substrait-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-30 19:41:51.000000 substrait-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-30 19:41:51.000000 substrait-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-30 19:41:51.000000 substrait-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 19:41:51.000000 substrait-0.1.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-30 19:41:51.000000 substrait-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 19:41:51.000000 substrait-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-30 19:42:04.369334 substrait-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-30 19:41:51.000000 substrait-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-30 19:41:51.000000 substrait-0.1.0/buf.gen.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 19:41:51.000000 substrait-0.1.0/buf.work.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 19:41:51.000000 substrait-0.1.0/buf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-30 19:41:51.000000 substrait-0.1.0/environment.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      637 2023-05-30 19:41:51.000000 substrait-0.1.0/gen_proto.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-30 19:41:51.000000 substrait-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:42:04.369334 substrait-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.357334 substrait-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.361334 substrait-0.1.0/src/substrait/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 19:42:04.000000 substrait-0.1.0/src/substrait/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.365334 substrait-0.1.0/src/substrait/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.369334 substrait-0.1.0/src/substrait/gen/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47948 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/algebra_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/capabilities_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/extended_expression_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.369334 substrait-0.1.0/src/substrait/gen/proto/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/extensions/extensions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/function_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/parameterized_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/plan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/type_expressions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-05-30 19:41:51.000000 substrait-0.1.0/src/substrait/gen/proto/type_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.365334 substrait-0.1.0/src/substrait.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-30 19:42:04.000000 substrait-0.1.0/src/substrait.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-30 19:42:04.000000 substrait-0.1.0/src/substrait.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:42:04.000000 substrait-0.1.0/src/substrait.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 19:42:04.000000 substrait-0.1.0/src/substrait.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 19:42:04.000000 substrait-0.1.0/src/substrait.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:42:04.369334 substrait-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-30 19:41:51.000000 substrait-0.1.0/tests/test_proto.py
```

### Comparing `substrait-0.0.1/.gitignore` & `substrait-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/CONTRIBUTING.md` & `substrait-0.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/LICENSE` & `substrait-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/PKG-INFO` & `substrait-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrait
-Version: 0.0.1
+Version: 0.1.0
 Summary: A python package for Substrait.
 Author-email: Substrait contributors <substrait@googlegroups.com>
 License: Apache-2.0
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: gen_proto
 Provides-Extra: test
```

### Comparing `substrait-0.0.1/README.md` & `substrait-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/gen_proto.sh` & `substrait-0.1.0/gen_proto.sh`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/pyproject.toml` & `substrait-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 readme = "README.md"
 requires-python = ">=3.8.1"
 dependencies = ["protobuf >= 3.20"]
 dynamic = ["version"]
 
 [tool.setuptools_scm]
 write_to = "src/substrait/_version.py"
+local_scheme = "no-local-version"
 
 [project.optional-dependencies]
 gen_proto = ["protobuf == 3.20.1", "protoletariat >= 2.0.0"]
 test = ["pytest >= 7.0.0"]
 
 [tool.pytest.ini_options]
 pythonpath = "src"
```

### Comparing `substrait-0.0.1/src/substrait/gen/proto/algebra_pb2.py` & `substrait-0.1.0/src/substrait/gen/proto/algebra_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/src/substrait/gen/proto/capabilities_pb2.py` & `substrait-0.1.0/src/substrait/gen/proto/capabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/src/substrait/gen/proto/extended_expression_pb2.py` & `substrait-0.1.0/src/substrait/gen/proto/extended_expression_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/src/substrait/gen/proto/extensions/extensions_pb2.py` & `substrait-0.1.0/src/substrait/gen/proto/extensions/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/src/substrait/gen/proto/function_pb2.py` & `substrait-0.1.0/src/substrait/gen/proto/function_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/src/substrait/gen/proto/parameterized_types_pb2.py` & `substrait-0.1.0/src/substrait/gen/proto/parameterized_types_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/src/substrait/gen/proto/plan_pb2.py` & `substrait-0.1.0/src/substrait/gen/proto/plan_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/src/substrait/gen/proto/type_expressions_pb2.py` & `substrait-0.1.0/src/substrait/gen/proto/type_expressions_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/src/substrait/gen/proto/type_pb2.py` & `substrait-0.1.0/src/substrait/gen/proto/type_pb2.py`

 * *Files identical despite different names*

### Comparing `substrait-0.0.1/src/substrait.egg-info/PKG-INFO` & `substrait-0.1.0/src/substrait.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrait
-Version: 0.0.1
+Version: 0.1.0
 Summary: A python package for Substrait.
 Author-email: Substrait contributors <substrait@googlegroups.com>
 License: Apache-2.0
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: gen_proto
 Provides-Extra: test
```

### Comparing `substrait-0.0.1/src/substrait.egg-info/SOURCES.txt` & `substrait-0.1.0/src/substrait.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 README.md
 buf.gen.yaml
 buf.work.yaml
 buf.yaml
 environment.yml
 gen_proto.sh
 pyproject.toml
+.github/workflows/release.yml
+.github/workflows/test.yml
 src/substrait/__init__.py
 src/substrait/_version.py
 src/substrait.egg-info/PKG-INFO
 src/substrait.egg-info/SOURCES.txt
 src/substrait.egg-info/dependency_links.txt
 src/substrait.egg-info/requires.txt
 src/substrait.egg-info/top_level.txt
```

### Comparing `substrait-0.0.1/tests/test_proto.py` & `substrait-0.1.0/tests/test_proto.py`

 * *Files identical despite different names*

