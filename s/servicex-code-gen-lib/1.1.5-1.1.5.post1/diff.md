# Comparing `tmp/servicex_code_gen_lib-1.1.5.tar.gz` & `tmp/servicex_code_gen_lib-1.1.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicex_code_gen_lib-1.1.5.tar", max compression
+gzip compressed data, was "servicex_code_gen_lib-1.1.5.post1.tar", max compression
```

## Comparing `servicex_code_gen_lib-1.1.5.tar` & `servicex_code_gen_lib-1.1.5.post1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1520 2023-05-18 18:00:53.213698 servicex_code_gen_lib-1.1.5/LICENSE
--rw-r--r--   0        0        0      138 2023-05-18 18:00:53.213698 servicex_code_gen_lib-1.1.5/README.md
--rw-r--r--   0        0        0      749 2023-05-18 18:01:16.277930 servicex_code_gen_lib-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     2882 2023-05-18 18:00:53.213698 servicex_code_gen_lib-1.1.5/servicex_codegen/__init__.py
--rw-r--r--   0        0        0     2194 2023-05-18 18:00:53.213698 servicex_code_gen_lib-1.1.5/servicex_codegen/code_generator.py
--rw-r--r--   0        0        0     4797 2023-05-18 18:00:53.213698 servicex_code_gen_lib-1.1.5/servicex_codegen/post_operation.py
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 servicex_code_gen_lib-1.1.5/setup.py
--rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 servicex_code_gen_lib-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1520 2023-05-30 20:22:45.271809 servicex_code_gen_lib-1.1.5.post1/LICENSE
+-rw-r--r--   0        0        0      138 2023-05-30 20:22:45.271809 servicex_code_gen_lib-1.1.5.post1/README.md
+-rw-r--r--   0        0        0      756 2023-05-30 20:23:04.147741 servicex_code_gen_lib-1.1.5.post1/pyproject.toml
+-rw-r--r--   0        0        0     2882 2023-05-30 20:22:45.271809 servicex_code_gen_lib-1.1.5.post1/servicex_codegen/__init__.py
+-rw-r--r--   0        0        0     2194 2023-05-30 20:22:45.271809 servicex_code_gen_lib-1.1.5.post1/servicex_codegen/code_generator.py
+-rw-r--r--   0        0        0     4797 2023-05-30 20:22:45.271809 servicex_code_gen_lib-1.1.5.post1/servicex_codegen/post_operation.py
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 servicex_code_gen_lib-1.1.5.post1/setup.py
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 servicex_code_gen_lib-1.1.5.post1/PKG-INFO
```

### Comparing `servicex_code_gen_lib-1.1.5/LICENSE` & `servicex_code_gen_lib-1.1.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `servicex_code_gen_lib-1.1.5/pyproject.toml` & `servicex_code_gen_lib-1.1.5.post1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicex-code-gen-lib"
-version = "1.1.5"
+version = "1.1.5-post.1"
 description = "Library for creating ServiceX Code Generators"
 authors = ["Ben Galewsky <bengal1@illinois.edu>"]
 readme = "README.md"
 packages = [{include = "servicex_codegen"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `servicex_code_gen_lib-1.1.5/servicex_codegen/__init__.py` & `servicex_code_gen_lib-1.1.5.post1/servicex_codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex_code_gen_lib-1.1.5/servicex_codegen/code_generator.py` & `servicex_code_gen_lib-1.1.5.post1/servicex_codegen/code_generator.py`

 * *Files identical despite different names*

### Comparing `servicex_code_gen_lib-1.1.5/servicex_codegen/post_operation.py` & `servicex_code_gen_lib-1.1.5.post1/servicex_codegen/post_operation.py`

 * *Files identical despite different names*

### Comparing `servicex_code_gen_lib-1.1.5/setup.py` & `servicex_code_gen_lib-1.1.5.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'Werkzeug>=2.2.2,<3.0.0',
  'itsdangerous>=2.1.2,<3.0.0',
  'requests-toolbelt>=0.10.1,<0.11.0',
  'urllib3==1.26.15']
 
 setup_kwargs = {
     'name': 'servicex-code-gen-lib',
-    'version': '1.1.5',
+    'version': '1.1.5.post1',
     'description': 'Library for creating ServiceX Code Generators',
     'long_description': '<!-- @format -->\n\n# ServiceX Code Generator Library\n\nThis library provides common code for creating Code Generator services for\nServiceX.\n',
     'author': 'Ben Galewsky',
     'author_email': 'bengal1@illinois.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `servicex_code_gen_lib-1.1.5/PKG-INFO` & `servicex_code_gen_lib-1.1.5.post1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicex-code-gen-lib
-Version: 1.1.5
+Version: 1.1.5.post1
 Summary: Library for creating ServiceX Code Generators
 Author: Ben Galewsky
 Author-email: bengal1@illinois.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

