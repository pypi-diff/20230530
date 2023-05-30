# Comparing `tmp/servicex_code_gen_lib-1.1.5.post1.tar.gz` & `tmp/servicex_code_gen_lib-1.1.5.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicex_code_gen_lib-1.1.5.post1.tar", max compression
+gzip compressed data, was "servicex_code_gen_lib-1.1.5.post2.tar", max compression
```

## Comparing `servicex_code_gen_lib-1.1.5.post1.tar` & `servicex_code_gen_lib-1.1.5.post2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1520 2023-05-30 20:22:45.271809 servicex_code_gen_lib-1.1.5.post1/LICENSE
--rw-r--r--   0        0        0      138 2023-05-30 20:22:45.271809 servicex_code_gen_lib-1.1.5.post1/README.md
--rw-r--r--   0        0        0      756 2023-05-30 20:23:04.147741 servicex_code_gen_lib-1.1.5.post1/pyproject.toml
--rw-r--r--   0        0        0     2882 2023-05-30 20:22:45.271809 servicex_code_gen_lib-1.1.5.post1/servicex_codegen/__init__.py
--rw-r--r--   0        0        0     2194 2023-05-30 20:22:45.271809 servicex_code_gen_lib-1.1.5.post1/servicex_codegen/code_generator.py
--rw-r--r--   0        0        0     4797 2023-05-30 20:22:45.271809 servicex_code_gen_lib-1.1.5.post1/servicex_codegen/post_operation.py
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 servicex_code_gen_lib-1.1.5.post1/setup.py
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 servicex_code_gen_lib-1.1.5.post1/PKG-INFO
+-rw-r--r--   0        0        0     1520 2023-05-30 20:37:49.310530 servicex_code_gen_lib-1.1.5.post2/LICENSE
+-rw-r--r--   0        0        0      138 2023-05-30 20:37:49.310530 servicex_code_gen_lib-1.1.5.post2/README.md
+-rw-r--r--   0        0        0      756 2023-05-30 20:38:09.535576 servicex_code_gen_lib-1.1.5.post2/pyproject.toml
+-rw-r--r--   0        0        0     2882 2023-05-30 20:37:49.310530 servicex_code_gen_lib-1.1.5.post2/servicex_codegen/__init__.py
+-rw-r--r--   0        0        0     2194 2023-05-30 20:37:49.310530 servicex_code_gen_lib-1.1.5.post2/servicex_codegen/code_generator.py
+-rw-r--r--   0        0        0     4776 2023-05-30 20:37:49.310530 servicex_code_gen_lib-1.1.5.post2/servicex_codegen/post_operation.py
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 servicex_code_gen_lib-1.1.5.post2/setup.py
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 servicex_code_gen_lib-1.1.5.post2/PKG-INFO
```

### Comparing `servicex_code_gen_lib-1.1.5.post1/LICENSE` & `servicex_code_gen_lib-1.1.5.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `servicex_code_gen_lib-1.1.5.post1/pyproject.toml` & `servicex_code_gen_lib-1.1.5.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicex-code-gen-lib"
-version = "1.1.5-post.1"
+version = "1.1.5-post.2"
 description = "Library for creating ServiceX Code Generators"
 authors = ["Ben Galewsky <bengal1@illinois.edu>"]
 readme = "README.md"
 packages = [{include = "servicex_codegen"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `servicex_code_gen_lib-1.1.5.post1/servicex_codegen/__init__.py` & `servicex_code_gen_lib-1.1.5.post2/servicex_codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex_code_gen_lib-1.1.5.post1/servicex_codegen/code_generator.py` & `servicex_code_gen_lib-1.1.5.post2/servicex_codegen/code_generator.py`

 * *Files identical despite different names*

### Comparing `servicex_code_gen_lib-1.1.5.post1/servicex_codegen/post_operation.py` & `servicex_code_gen_lib-1.1.5.post2/servicex_codegen/post_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 import os
 import zipfile
 from tempfile import TemporaryDirectory
 
-from flask import Response, current_app, request
+from flask import Response, request
 from flask_restful import Resource
 from requests_toolbelt import MultipartEncoder
 
 from servicex_codegen.code_generator import CodeGenerator, GeneratedFileResult
 
 
 class GeneratedCode(Resource):
@@ -88,15 +88,15 @@
                 body = request.get_json()
                 generated_code_result = self.code_generator.generate_code(
                     body["code"], cache_path=tempdir)
 
                 zip_data = self.stream_generated_code(generated_code_result)
                 # code gen transformer returns the default transformer image mentioned in
                 # the config file
-                transformer_image = current_app.config.get("TRANSFORMER_SCIENCE_IMAGE")
+                transformer_image = os.environ.get("TRANSFORMER_SCIENCE_IMAGE")
 
                 # MultipartEncoder library takes multiple types of data fields and merge
                 # them into a multipart mime data type
                 m = MultipartEncoder(
                     fields={'transformer_image': transformer_image,
                             'zip_data': zip_data}
                 )
```

### Comparing `servicex_code_gen_lib-1.1.5.post1/setup.py` & `servicex_code_gen_lib-1.1.5.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'Werkzeug>=2.2.2,<3.0.0',
  'itsdangerous>=2.1.2,<3.0.0',
  'requests-toolbelt>=0.10.1,<0.11.0',
  'urllib3==1.26.15']
 
 setup_kwargs = {
     'name': 'servicex-code-gen-lib',
-    'version': '1.1.5.post1',
+    'version': '1.1.5.post2',
     'description': 'Library for creating ServiceX Code Generators',
     'long_description': '<!-- @format -->\n\n# ServiceX Code Generator Library\n\nThis library provides common code for creating Code Generator services for\nServiceX.\n',
     'author': 'Ben Galewsky',
     'author_email': 'bengal1@illinois.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `servicex_code_gen_lib-1.1.5.post1/PKG-INFO` & `servicex_code_gen_lib-1.1.5.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicex-code-gen-lib
-Version: 1.1.5.post1
+Version: 1.1.5.post2
 Summary: Library for creating ServiceX Code Generators
 Author: Ben Galewsky
 Author-email: bengal1@illinois.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

