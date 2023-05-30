# Comparing `tmp/py_mysql_distill-0.1.1.tar.gz` & `tmp/py_mysql_distill-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_mysql_distill-0.1.1.tar", max compression
+gzip compressed data, was "py_mysql_distill-0.1.2.tar", max compression
```

## Comparing `py_mysql_distill-0.1.1.tar` & `py_mysql_distill-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-29 14:20:55.188677 py_mysql_distill-0.1.1/README.md
--rw-r--r--   0        0        0      215 2023-05-30 02:16:26.920580 py_mysql_distill-0.1.1/mysql_distill/__init__.py
--rw-r--r--   0        0        0      753 2023-05-30 02:16:02.768805 py_mysql_distill-0.1.1/mysql_distill/__main__.py
--rw-r--r--   0        0        0     4369 2023-05-30 02:04:49.365664 py_mysql_distill-0.1.1/mysql_distill/parser.py
--rw-r--r--   0        0        0     7408 2023-05-30 02:31:08.164134 py_mysql_distill-0.1.1/mysql_distill/rewriter.py
--rw-r--r--   0        0        0      449 2023-05-30 04:13:32.405245 py_mysql_distill-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 py_mysql_distill-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-29 14:20:55.188677 py_mysql_distill-0.1.2/README.md
+-rw-r--r--   0        0        0      215 2023-05-30 02:16:26.920580 py_mysql_distill-0.1.2/mysql_distill/__init__.py
+-rw-r--r--   0        0        0      753 2023-05-30 02:16:02.768805 py_mysql_distill-0.1.2/mysql_distill/__main__.py
+-rw-r--r--   0        0        0     4369 2023-05-30 02:04:49.365664 py_mysql_distill-0.1.2/mysql_distill/parser.py
+-rw-r--r--   0        0        0     7646 2023-05-30 05:30:07.234860 py_mysql_distill-0.1.2/mysql_distill/rewriter.py
+-rw-r--r--   0        0        0      449 2023-05-30 05:32:40.796879 py_mysql_distill-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 py_mysql_distill-0.1.2/PKG-INFO
```

### Comparing `py_mysql_distill-0.1.1/mysql_distill/__main__.py` & `py_mysql_distill-0.1.2/mysql_distill/__main__.py`

 * *Files identical despite different names*

### Comparing `py_mysql_distill-0.1.1/mysql_distill/parser.py` & `py_mysql_distill-0.1.2/mysql_distill/parser.py`

 * *Files identical despite different names*

### Comparing `py_mysql_distill-0.1.1/mysql_distill/rewriter.py` & `py_mysql_distill-0.1.2/mysql_distill/rewriter.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,25 +90,29 @@
 def distill(query: str) -> str:
     """
     Distill a query into a canonical form
 
     :param query:
     :return:
     """
+    _logger.info("distill: %s", query)
     verbs, table = distill_verbs(query)
+    _logger.info("distill: verbs=%s, table=%s", verbs, table)
 
     if verbs and _verb_show_re.match(verbs):
         alias_for = {"SCHEMA": "DATABASE", "KEYS": "INDEX", "INDEXES": "INDEX"}
         for alias_for_key, alias_for_value in alias_for.items():
             verbs = verbs.replace(alias_for_key, alias_for_value)
+        _logger.info("distill: show verbs=%s", verbs)
         query = verbs
     elif verbs and _verb_load_data_re.match(verbs):
         return verbs
     else:
         tables = _distill_tables(query, table)
+        _logger.info("distill: query=%s verbs=%s tables=%s", query, verbs, tables)
         query = " ".join([verbs] + tables)
 
     return query
 
 
 def distill_verbs(query: str) -> Tuple[str, str]:
     """
```

