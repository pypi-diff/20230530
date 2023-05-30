# Comparing `tmp/dbt-clickzetta-0.1.2.tar.gz` & `tmp/dbt-clickzetta-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickzetta-0.1.2.tar", last modified: Mon May 29 09:01:31 2023, max compression
+gzip compressed data, was "dbt-clickzetta-0.1.3.tar", last modified: Mon May 29 13:36:32 2023, max compression
```

## Comparing `dbt-clickzetta-0.1.2.tar` & `dbt-clickzetta-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:01:31.876385 dbt-clickzetta-0.1.2/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-29 09:01:31.876261 dbt-clickzetta-0.1.2/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/README.md
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:01:31.871162 dbt-clickzetta-0.1.2/dbt/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:01:31.870426 dbt-clickzetta-0.1.2/dbt/adapters/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:01:31.872144 dbt-clickzetta-0.1.2/dbt/adapters/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/adapters/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/adapters/clickzetta/__version__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1425 2023-05-28 10:16:48.000000 dbt-clickzetta-0.1.2/dbt/adapters/clickzetta/column.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7138 2023-05-29 03:50:21.000000 dbt-clickzetta-0.1.2/dbt/adapters/clickzetta/connections.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6709 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/adapters/clickzetta/impl.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1184 2023-05-28 14:31:37.000000 dbt-clickzetta-0.1.2/dbt/adapters/clickzetta/relation.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:01:31.870517 dbt-clickzetta-0.1.2/dbt/include/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:01:31.872607 dbt-clickzetta-0.1.2/dbt/include/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/dbt_project.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:01:31.872810 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14278 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/adapters.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:01:31.873305 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:01:31.873817 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/incremental/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2651 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/seed.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/snapshot.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/table.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/view.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:01:31.875523 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/any_value.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/array_append.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/array_concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/array_construct.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/assert_not_null.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/bool_or.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/dateadd.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/datediff.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/listagg.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/split_part.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/timestamps.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.2/dbt/include/clickzetta/profile_template.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:01:31.876105 dbt-clickzetta-0.1.2/dbt_clickzetta.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-29 09:01:31.000000 dbt-clickzetta-0.1.2/dbt_clickzetta.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-05-29 09:01:31.000000 dbt-clickzetta-0.1.2/dbt_clickzetta.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 09:01:31.000000 dbt-clickzetta-0.1.2/dbt_clickzetta.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 09:01:31.000000 dbt-clickzetta-0.1.2/dbt_clickzetta.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-05-29 09:01:31.000000 dbt-clickzetta-0.1.2/dbt_clickzetta.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-05-29 09:01:31.000000 dbt-clickzetta-0.1.2/dbt_clickzetta.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-29 09:01:31.876421 dbt-clickzetta-0.1.2/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-05-29 09:01:29.000000 dbt-clickzetta-0.1.2/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 13:36:32.018341 dbt-clickzetta-0.1.3/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-29 13:36:32.018218 dbt-clickzetta-0.1.3/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/README.md
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 13:36:32.012802 dbt-clickzetta-0.1.3/dbt/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 13:36:32.012062 dbt-clickzetta-0.1.3/dbt/adapters/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 13:36:32.013800 dbt-clickzetta-0.1.3/dbt/adapters/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/adapters/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/adapters/clickzetta/__version__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1425 2023-05-28 10:16:48.000000 dbt-clickzetta-0.1.3/dbt/adapters/clickzetta/column.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7138 2023-05-29 03:50:21.000000 dbt-clickzetta-0.1.3/dbt/adapters/clickzetta/connections.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6709 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/adapters/clickzetta/impl.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1184 2023-05-28 14:31:37.000000 dbt-clickzetta-0.1.3/dbt/adapters/clickzetta/relation.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 13:36:32.012156 dbt-clickzetta-0.1.3/dbt/include/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 13:36:32.014266 dbt-clickzetta-0.1.3/dbt/include/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/dbt_project.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 13:36:32.014481 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14278 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/adapters.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 13:36:32.015010 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 13:36:32.015505 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/incremental/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2651 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/seed.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/snapshot.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/table.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/view.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 13:36:32.017352 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/any_value.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/array_append.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/array_concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/array_construct.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/assert_not_null.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/bool_or.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/dateadd.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/datediff.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/listagg.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/split_part.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/timestamps.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.3/dbt/include/clickzetta/profile_template.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 13:36:32.018055 dbt-clickzetta-0.1.3/dbt_clickzetta.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-29 13:36:31.000000 dbt-clickzetta-0.1.3/dbt_clickzetta.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-05-29 13:36:32.000000 dbt-clickzetta-0.1.3/dbt_clickzetta.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 13:36:31.000000 dbt-clickzetta-0.1.3/dbt_clickzetta.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 13:36:31.000000 dbt-clickzetta-0.1.3/dbt_clickzetta.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-05-29 13:36:31.000000 dbt-clickzetta-0.1.3/dbt_clickzetta.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-05-29 13:36:31.000000 dbt-clickzetta-0.1.3/dbt_clickzetta.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-29 13:36:32.018376 dbt-clickzetta-0.1.3/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-05-29 13:36:27.000000 dbt-clickzetta-0.1.3/setup.py
```

### Comparing `dbt-clickzetta-0.1.2/PKG-INFO` & `dbt-clickzetta-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickzetta
-Version: 0.1.2
+Version: 0.1.3
 Summary: The ClickZetta adapter plugin for dbt
 Home-page: 
 Author: clickzetta
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `dbt-clickzetta-0.1.2/dbt/adapters/clickzetta/__init__.py` & `dbt-clickzetta-0.1.3/dbt/adapters/clickzetta/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/adapters/clickzetta/column.py` & `dbt-clickzetta-0.1.3/dbt/adapters/clickzetta/column.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/adapters/clickzetta/connections.py` & `dbt-clickzetta-0.1.3/dbt/adapters/clickzetta/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/adapters/clickzetta/impl.py` & `dbt-clickzetta-0.1.3/dbt/adapters/clickzetta/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/adapters/clickzetta/relation.py` & `dbt-clickzetta-0.1.3/dbt/adapters/clickzetta/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/adapters.sql` & `dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql` & `dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql` & `dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql` & `dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/incremental/validate.sql` & `dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/seed.sql` & `dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/snapshot.sql` & `dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/materializations/table.sql` & `dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/dateadd.sql` & `dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/datediff.sql` & `dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/listagg.sql` & `dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt/include/clickzetta/macros/utils/split_part.sql` & `dbt-clickzetta-0.1.3/dbt/include/clickzetta/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/dbt_clickzetta.egg-info/PKG-INFO` & `dbt-clickzetta-0.1.3/dbt_clickzetta.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickzetta
-Version: 0.1.2
+Version: 0.1.3
 Summary: The ClickZetta adapter plugin for dbt
 Home-page: 
 Author: clickzetta
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `dbt-clickzetta-0.1.2/dbt_clickzetta.egg-info/SOURCES.txt` & `dbt-clickzetta-0.1.3/dbt_clickzetta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.1.2/setup.py` & `dbt-clickzetta-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-clickzetta"
-package_version = "0.1.2"
+package_version = "0.1.3"
 dbt_core_version = _get_dbt_core_version()
 description = """The ClickZetta adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
@@ -64,15 +64,15 @@
     author="clickzetta",
     author_email="",
     url="",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-core~={}".format(dbt_core_version),
-        "clickzetta-connector~=0.8.0",
+        "clickzetta-connector~=0.8.2",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
```

