# Comparing `tmp/tableautransformer-1.0.1.tar.gz` & `tmp/tableautransformer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableautransformer-1.0.1.tar", last modified: Thu May 11 13:30:43 2023, max compression
+gzip compressed data, was "tableautransformer-1.0.2.tar", last modified: Tue May 30 14:12:11 2023, max compression
```

## Comparing `tableautransformer-1.0.1.tar` & `tableautransformer-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 13:30:43.410040 tableautransformer-1.0.1/
--rw-rw-rw-   0        0        0     1091 2022-12-21 16:48:30.000000 tableautransformer-1.0.1/LICENCE
--rw-rw-rw-   0        0        0     8485 2023-05-11 13:30:43.410040 tableautransformer-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8135 2023-05-11 13:29:50.000000 tableautransformer-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 13:30:43.410040 tableautransformer-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-05-11 13:30:23.000000 tableautransformer-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 13:30:43.362043 tableautransformer-1.0.1/tableautransformer/
--rw-rw-rw-   0        0        0        0 2022-12-22 15:23:56.000000 tableautransformer-1.0.1/tableautransformer/__init__.py
--rw-rw-rw-   0        0        0      189 2022-12-22 15:56:40.000000 tableautransformer-1.0.1/tableautransformer/backbone.py
--rw-rw-rw-   0        0        0     4590 2023-05-11 13:27:31.000000 tableautransformer-1.0.1/tableautransformer/datawrangling.py
-drwxrwxrwx   0        0        0        0 2023-05-11 13:30:43.410040 tableautransformer-1.0.1/tableautransformer.egg-info/
--rw-rw-rw-   0        0        0     8485 2023-05-11 13:30:42.000000 tableautransformer-1.0.1/tableautransformer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-11 13:30:43.000000 tableautransformer-1.0.1/tableautransformer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 13:30:42.000000 tableautransformer-1.0.1/tableautransformer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-11 13:30:42.000000 tableautransformer-1.0.1/tableautransformer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 14:12:11.269900 tableautransformer-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2022-12-21 16:48:30.000000 tableautransformer-1.0.2/LICENCE
+-rw-rw-rw-   0        0        0     8485 2023-05-30 14:12:11.267902 tableautransformer-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8135 2023-05-11 13:29:50.000000 tableautransformer-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 14:12:11.269900 tableautransformer-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-05-30 14:11:35.000000 tableautransformer-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:12:11.198899 tableautransformer-1.0.2/tableautransformer/
+-rw-rw-rw-   0        0        0        0 2022-12-22 15:23:56.000000 tableautransformer-1.0.2/tableautransformer/__init__.py
+-rw-rw-rw-   0        0        0      189 2022-12-22 15:56:40.000000 tableautransformer-1.0.2/tableautransformer/backbone.py
+-rw-rw-rw-   0        0        0     4636 2023-05-30 14:11:09.000000 tableautransformer-1.0.2/tableautransformer/datawrangling.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:12:11.262901 tableautransformer-1.0.2/tableautransformer.egg-info/
+-rw-rw-rw-   0        0        0     8485 2023-05-30 14:12:09.000000 tableautransformer-1.0.2/tableautransformer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-30 14:12:10.000000 tableautransformer-1.0.2/tableautransformer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 14:12:09.000000 tableautransformer-1.0.2/tableautransformer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-30 14:12:10.000000 tableautransformer-1.0.2/tableautransformer.egg-info/top_level.txt
```

### Comparing `tableautransformer-1.0.1/LICENCE` & `tableautransformer-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `tableautransformer-1.0.1/PKG-INFO` & `tableautransformer-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableautransformer
-Version: 1.0.1
+Version: 1.0.2
 Summary: ETL tooling for tableau seed data
 Home-page: https://pypi.org/project/tableautransformer
 Author: Josh Teixeira
 Author-email: jteixeira@cppib.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `tableautransformer-1.0.1/README.md` & `tableautransformer-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tableautransformer-1.0.1/tableautransformer/datawrangling.py` & `tableautransformer-1.0.2/tableautransformer/datawrangling.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,16 +83,18 @@
 
 def cast(df, target_col, value):
     df[target_col] = value
     return df
 
 def export(file_name, tables):
     with pd.ExcelWriter(file_name) as writer:
-        for tab_name, df_name in tables.items():
-            df_name.to_excel(writer, sheet_name=tab_name, index=False)
+        for key in tables.keys():
+            tab_name = key
+            tab_df = tables[key]
+            tab_df.to_excel(writer, sheet_name=tab_name, index=False)
     return print(f"Data written too {file_name}")
 
 def create_row(): # might not be needed, if so it will be a create row with filter and col_ops
     pass
 
 def bucket(df, column, bucket_col_name, intervals): # need to add in operand for both lower and upper bounds
     interval_values = []
```

### Comparing `tableautransformer-1.0.1/tableautransformer.egg-info/PKG-INFO` & `tableautransformer-1.0.2/tableautransformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableautransformer
-Version: 1.0.1
+Version: 1.0.2
 Summary: ETL tooling for tableau seed data
 Home-page: https://pypi.org/project/tableautransformer
 Author: Josh Teixeira
 Author-email: jteixeira@cppib.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

