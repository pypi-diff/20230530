# Comparing `tmp/macrometa-source-collection-0.0.33.tar.gz` & `tmp/macrometa-source-collection-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.33.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.34.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.33.tar` & `macrometa-source-collection-0.0.34.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8945 2023-05-30 04:19:31.664195 macrometa-source-collection-0.0.33/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     8634 2023-05-30 04:19:31.664195 macrometa-source-collection-0.0.33/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1623 2023-05-30 04:19:31.928199 macrometa-source-collection-0.0.33/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.33/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.33/PKG-INFO
+-rw-r--r--   0        0        0     8969 2023-05-30 05:06:44.643837 macrometa-source-collection-0.0.34/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     8634 2023-05-30 05:06:44.643837 macrometa-source-collection-0.0.34/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1623 2023-05-30 05:06:44.951857 macrometa-source-collection-0.0.34/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.34/setup.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.34/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.33/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.34/macrometa_source_collection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         host=config["gdn_host"],
         port=443,
         geofabric=config["fabric"],
         apikey=config["api_key"]
     ), collection_name, 50)
     schema_properties = {
         k: SingerSchema(
-            type=['null', v] if v != 'null' else ['null', 'string', 'integer', 'number', 'boolean', 'array', 'object'],
+            type=['null', 'string', 'integer', 'number', 'boolean', 'array', 'object'] if v == 'null' else (v if k == '_key' else ['null', v]),
             format=None
         )
         for k, v in schema.items()
     }
     # inject `_sdc_deleted_at` prop to the schema.
     schema_properties['_sdc_deleted_at'] = SingerSchema(type=['null', 'string'], format='date-time')
     singer_schema = SingerSchema(type='object', properties=schema_properties)
```

### Comparing `macrometa-source-collection-0.0.33/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.34/macrometa_source_collection/client.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.33/pyproject.toml` & `macrometa-source-collection-0.0.34/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.33'
+version='0.0.34'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.33/setup.py` & `macrometa-source-collection-0.0.34/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.33',
+    'version': '0.0.34',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.33/PKG-INFO` & `macrometa-source-collection-0.0.34/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.33
+Version: 0.0.34
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

