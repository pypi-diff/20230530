# Comparing `tmp/bqhus-0.1.8.tar.gz` & `tmp/bqhus-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqhus-0.1.8.tar", last modified: Wed Mar 29 05:44:14 2023, max compression
+gzip compressed data, was "bqhus-0.1.9.tar", last modified: Wed Mar 29 08:05:11 2023, max compression
```

## Comparing `bqhus-0.1.8.tar` & `bqhus-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:14.317581 bqhus-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-29 05:44:05.000000 bqhus-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-29 05:44:14.317581 bqhus-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-29 05:44:05.000000 bqhus-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 05:44:14.317581 bqhus-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-29 05:44:05.000000 bqhus-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:14.313581 bqhus-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:14.313581 bqhus-0.1.8/src/bqhus/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-29 05:44:05.000000 bqhus-0.1.8/src/bqhus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-29 05:44:05.000000 bqhus-0.1.8/src/bqhus/bqhus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-03-29 05:44:05.000000 bqhus-0.1.8/src/bqhus/create_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-29 05:44:05.000000 bqhus-0.1.8/src/bqhus/export_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-29 05:44:05.000000 bqhus-0.1.8/src/bqhus/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-03-29 05:44:05.000000 bqhus-0.1.8/src/bqhus/select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:14.313581 bqhus-0.1.8/src/bqhus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-29 05:44:14.000000 bqhus-0.1.8/src/bqhus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-29 05:44:14.000000 bqhus-0.1.8/src/bqhus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 05:44:14.000000 bqhus-0.1.8/src/bqhus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-29 05:44:14.000000 bqhus-0.1.8/src/bqhus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-29 05:44:14.000000 bqhus-0.1.8/src/bqhus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:14.317581 bqhus-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-29 05:44:05.000000 bqhus-0.1.8/tests/test_naming.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-29 05:44:05.000000 bqhus-0.1.8/tests/test_select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:05:11.362741 bqhus-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-29 08:05:02.000000 bqhus-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-29 08:05:11.362741 bqhus-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-29 08:05:02.000000 bqhus-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 08:05:11.362741 bqhus-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-29 08:05:02.000000 bqhus-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:05:11.358741 bqhus-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:05:11.358741 bqhus-0.1.9/src/bqhus/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-29 08:05:02.000000 bqhus-0.1.9/src/bqhus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-29 08:05:02.000000 bqhus-0.1.9/src/bqhus/bqhus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-03-29 08:05:02.000000 bqhus-0.1.9/src/bqhus/create_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-29 08:05:02.000000 bqhus-0.1.9/src/bqhus/export_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-29 08:05:02.000000 bqhus-0.1.9/src/bqhus/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-03-29 08:05:02.000000 bqhus-0.1.9/src/bqhus/select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:05:11.362741 bqhus-0.1.9/src/bqhus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-29 08:05:11.000000 bqhus-0.1.9/src/bqhus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-29 08:05:11.000000 bqhus-0.1.9/src/bqhus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 08:05:11.000000 bqhus-0.1.9/src/bqhus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-29 08:05:11.000000 bqhus-0.1.9/src/bqhus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-29 08:05:11.000000 bqhus-0.1.9/src/bqhus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:05:11.362741 bqhus-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-29 08:05:02.000000 bqhus-0.1.9/tests/test_naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-29 08:05:02.000000 bqhus-0.1.9/tests/test_select.py
```

### Comparing `bqhus-0.1.8/LICENSE` & `bqhus-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bqhus-0.1.8/PKG-INFO` & `bqhus-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqhus
-Version: 0.1.8
+Version: 0.1.9
 Summary: bqhus: BigQuery helper utils.
 Home-page: https://github.com/yokoe/bqhus
 Download-URL: https://github.com/yokoe/bqhus
 Author: yokoe
 Author-email: kreuz45@kreuz45.com
 Maintainer: yokoe
 Maintainer-email: kreuz45@kreuz45.com
```

### Comparing `bqhus-0.1.8/README.md` & `bqhus-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `bqhus-0.1.8/setup.py` & `bqhus-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 DESCRIPTION = "bqhus: BigQuery helper utils."
 NAME = "bqhus"
 AUTHOR = "yokoe"
 AUTHOR_EMAIL = "kreuz45@kreuz45.com"
 URL = "https://github.com/yokoe/bqhus"
 LICENSE = "MIT"
 DOWNLOAD_URL = URL
-VERSION = "0.1.8"
-PYTHON_REQUIRES = ">=3.6"
+VERSION = "0.1.9"
+PYTHON_REQUIRES = ">=3.9"
 INSTALL_REQUIRES = [
     "google-cloud-bigquery>=3.4.0",
     "Jinja2>=3.0.0",
     "pandas>=1.4.0",
     "db-dtypes>=1.0.5",
 ]
 PACKAGES = ["bqhus"]
```

### Comparing `bqhus-0.1.8/src/bqhus/create_table.py` & `bqhus-0.1.9/src/bqhus/create_table.py`

 * *Files identical despite different names*

### Comparing `bqhus-0.1.8/src/bqhus/export_table.py` & `bqhus-0.1.9/src/bqhus/export_table.py`

 * *Files identical despite different names*

### Comparing `bqhus-0.1.8/src/bqhus/select.py` & `bqhus-0.1.9/src/bqhus/select.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from google.cloud import bigquery
 from jinja2 import Template, Environment, FileSystemLoader
 from .create_table import create_table
+import google.cloud.bigquery
 
 
 class SelectTask:
     def __init__(self, client, query):
         self.client = client
         self.query = query
         self.query_parameters = []
@@ -54,19 +55,23 @@
             client=self.client,
         )
 
     def to_dataframe(self):
         return self.job().to_dataframe()
 
 
-def select(query, query_parameters=[], client=None):
+def select(
+    query: str,
+    query_parameters=[],
+    client: google.cloud.bigquery.Client = None,
+):
     return SelectTask(client=client, query=query).params(query_parameters)
 
 
 def select_with_template(
-    template_dir, template_name, template_parameters={}, client=None
+    template_dir: str, template_name: str, template_parameters={}, client=None
 ):
     env = Environment(loader=FileSystemLoader(template_dir, encoding="utf8"))
     tmpl = env.get_template(template_name)
     query = tmpl.render(template_parameters)
 
-    return select(query, client)
+    return select(query=query, query_parameters=[], client=client)
```

### Comparing `bqhus-0.1.8/src/bqhus.egg-info/PKG-INFO` & `bqhus-0.1.9/src/bqhus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqhus
-Version: 0.1.8
+Version: 0.1.9
 Summary: bqhus: BigQuery helper utils.
 Home-page: https://github.com/yokoe/bqhus
 Download-URL: https://github.com/yokoe/bqhus
 Author: yokoe
 Author-email: kreuz45@kreuz45.com
 Maintainer: yokoe
 Maintainer-email: kreuz45@kreuz45.com
```

### Comparing `bqhus-0.1.8/tests/test_select.py` & `bqhus-0.1.9/tests/test_select.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,22 @@
         self.assertEqual(query, task.query)
 
     def test_select(self):
         query = "SELECT word FROM `bigquery-public-data.samples.shakespeare` order by rand() limit 5"
         words = bqhus.select(query).as_dicts()
         self.assertEqual(len(words), 5)
 
+    def test_select_with_template(self):
+        words = (
+            bqhus.select_with_template("./tests/templates", "shakespeare.j2")
+            .int64_param("max_count", 3)
+            .as_dicts()
+        )
+        self.assertEqual(len(words), 3)
+
     def test_select_to_dataframe(self):
         query = "SELECT word FROM `bigquery-public-data.samples.shakespeare` order by rand() limit 5"
         df = bqhus.select(query).to_dataframe()
         self.assertEqual(len(df.index), 5)
 
     def test_select_int64_param(self):
         query = "SELECT word FROM `bigquery-public-data.samples.shakespeare` order by rand() limit @max_count"
```

