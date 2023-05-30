# Comparing `tmp/macrometa-source-collection-0.0.34.tar.gz` & `tmp/macrometa-source-collection-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.34.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.35.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.34.tar` & `macrometa-source-collection-0.0.35.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8969 2023-05-30 05:06:44.643837 macrometa-source-collection-0.0.34/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     8634 2023-05-30 05:06:44.643837 macrometa-source-collection-0.0.34/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1623 2023-05-30 05:06:44.951857 macrometa-source-collection-0.0.34/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.34/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.34/PKG-INFO
+-rw-r--r--   0        0        0     8969 2023-05-30 05:23:36.631533 macrometa-source-collection-0.0.35/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     9054 2023-05-30 05:23:36.631533 macrometa-source-collection-0.0.35/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1623 2023-05-30 05:23:36.887501 macrometa-source-collection-0.0.35/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.35/setup.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.35/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.34/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.35/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.34/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.35/macrometa_source_collection/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,15 +92,16 @@
                     j = json.loads(data.decode("utf8"))
                     j.pop('_id', None)
                     j.pop('_rev', None)
 
                     if props["op"] == "INSERT" or props["op"] == "UPDATE":
                         # skip inserts not having valid schema
                         if len(j.keys() ^ columns) == 0 and all(
-                            j[key] is None or get_singer_data_type(j[key]) in schema_properties[key].type
+                            j[key] is None or (isinstance(schema_properties[key].type, list) and get_singer_data_type(j[key]) in schema_properties[key].type)
+                                                 or (isinstance(schema_properties[key].type, str) and get_singer_data_type(j[key]) == schema_properties[key].type)
                             for key in j.keys()
                         ):
                             j['_sdc_deleted_at'] = None
                             singer_record = self.msg_to_singer_message(stream, j, None, utils.now())
                             singer.write_message(singer_record)
                     elif props["op"] == "DELETE":
                         # Currently, we don't have a way to validate schema here
@@ -129,15 +130,16 @@
                                                stream=True)
         while (not cursor.empty()) or cursor.has_more():
             rec = cursor.next()
             rec.pop('_id', None)
             rec.pop('_rev', None)
             # skip existing data not having valid schema
             if len(rec.keys() ^ columns) == 0 and all(
-                rec[key] is None or get_singer_data_type(rec[key]) in schema_properties[key].type
+                rec[key] is None or (isinstance(schema_properties[key].type, list) and get_singer_data_type(rec[key]) in schema_properties[key].type)
+                                     or (isinstance(schema_properties[key].type, str) and get_singer_data_type(rec[key]) == schema_properties[key].type)
                 for key in rec.keys()
             ):
                 singer_record = self.msg_to_singer_message(stream, rec, None, utils.now())
                 singer.write_message(singer_record)
                 self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(rec))
                 self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
```

### Comparing `macrometa-source-collection-0.0.34/pyproject.toml` & `macrometa-source-collection-0.0.35/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.34'
+version='0.0.35'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.34/setup.py` & `macrometa-source-collection-0.0.35/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.34',
+    'version': '0.0.35',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.34/PKG-INFO` & `macrometa-source-collection-0.0.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.34
+Version: 0.0.35
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

