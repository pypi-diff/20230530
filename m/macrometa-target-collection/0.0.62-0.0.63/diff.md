# Comparing `tmp/macrometa-target-collection-0.0.62.tar.gz` & `tmp/macrometa-target-collection-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.62.tar", last modified: Fri May 26 07:05:05 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.63.tar", last modified: Tue May 30 04:21:16 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.62.tar` & `macrometa-target-collection-0.0.63.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:05.863687 macrometa-target-collection-0.0.62/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-26 07:04:39.000000 macrometa-target-collection-0.0.62/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-26 07:05:05.863687 macrometa-target-collection-0.0.62/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-26 07:04:39.000000 macrometa-target-collection-0.0.62/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:05.863687 macrometa-target-collection-0.0.62/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-26 07:04:39.000000 macrometa-target-collection-0.0.62/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14458 2023-05-26 07:04:39.000000 macrometa-target-collection-0.0.62/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:05.863687 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-26 07:05:05.000000 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-26 07:05:05.000000 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:05:05.000000 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 07:05:05.000000 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-26 07:05:05.000000 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 07:05:05.000000 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-26 07:04:39.000000 macrometa-target-collection-0.0.62/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-26 07:05:05.867687 macrometa-target-collection-0.0.62/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:21:16.330926 macrometa-target-collection-0.0.63/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-30 04:20:52.000000 macrometa-target-collection-0.0.63/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-30 04:21:16.330926 macrometa-target-collection-0.0.63/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-30 04:20:52.000000 macrometa-target-collection-0.0.63/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:21:16.330926 macrometa-target-collection-0.0.63/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-30 04:20:52.000000 macrometa-target-collection-0.0.63/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14459 2023-05-30 04:20:52.000000 macrometa-target-collection-0.0.63/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:21:16.330926 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-30 04:21:16.000000 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-30 04:21:16.000000 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 04:21:16.000000 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-30 04:21:16.000000 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-30 04:21:16.000000 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 04:21:16.000000 macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-30 04:20:52.000000 macrometa-target-collection-0.0.63/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 04:21:16.330926 macrometa-target-collection-0.0.63/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.62/LICENSE` & `macrometa-target-collection-0.0.63/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.62/PKG-INFO` & `macrometa-target-collection-0.0.63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.62
+Version: 0.0.63
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.62/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.63/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.62/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.63/macrometa_target_collection/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
             try:
                 validators[stream].validate((o['record']))
             except jsonschema.ValidationError as e:
                 # Increment ingest_errors metric
                 ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 logger.error(f"Failed parsing the json schema for stream: {stream}.")
-                raise e
+                continue
 
             try:
                 rec = o['record']
                 if 'time_extracted' in o:
                     rec["time_extracted"] = ensure_datetime(o["time_extracted"])
                 else:
                     rec["time_extracted"] = ensure_datetime(record_batch.last_executed_time)
```

### Comparing `macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.63/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.62
+Version: 0.0.63
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.62/pyproject.toml` & `macrometa-target-collection-0.0.63/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.62"
+version = "0.0.63"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

