# Comparing `tmp/oemetadata-1.5.2.tar.gz` & `tmp/oemetadata-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oemetadata-1.5.2.tar", last modified: Fri Nov 18 15:33:08 2022, max compression
+gzip compressed data, was "oemetadata-1.6.0.tar", last modified: Tue May 30 14:11:29 2023, max compression
```

## Comparing `oemetadata-1.5.2.tar` & `oemetadata-1.6.0.tar`

### file list

```diff
@@ -1,123 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.652726 oemetadata-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-11-18 15:32:58.000000 oemetadata-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3123 2022-11-18 15:33:08.652726 oemetadata-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2509 2022-11-18 15:32:58.000000 oemetadata-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.632725 oemetadata-1.5.2/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.632725 oemetadata-1.5.2/metadata/latest/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2289 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/latest/context.json
--rw-r--r--   0 runner    (1001) docker     (121)    14929 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/latest/example.json
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/latest/example.py
--rw-r--r--   0 runner    (1001) docker     (121)    47300 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/latest/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/latest/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     5658 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/latest/template.json
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/latest/template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.632725 oemetadata-1.5.2/metadata/metaschema/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/metaschema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.632725 oemetadata-1.5.2/metadata/metaschema/draft07/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/metaschema/draft07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5806 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/metaschema/draft07/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/metaschema/draft07/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.632725 oemetadata-1.5.2/metadata/v130/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v130/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3554 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v130/example.json
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v130/example.py
--rw-r--r--   0 runner    (1001) docker     (121)    12387 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v130/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v130/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2556 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v130/template.json
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v130/template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.636725 oemetadata-1.5.2/metadata/v140/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v140/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9612 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v140/example.json
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v140/example.py
--rw-r--r--   0 runner    (1001) docker     (121)    34811 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v140/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v140/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     4424 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v140/template.json
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v140/template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.636725 oemetadata-1.5.2/metadata/v141/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v141/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9436 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v141/example.json
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v141/example.py
--rw-r--r--   0 runner    (1001) docker     (121)    34765 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v141/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v141/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     4227 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v141/template.json
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v141/template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.640725 oemetadata-1.5.2/metadata/v150/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v150/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v150/context.json
--rw-r--r--   0 runner    (1001) docker     (121)    10820 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v150/example.json
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v150/example.py
--rw-r--r--   0 runner    (1001) docker     (121)    42880 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v150/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v150/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    36713 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v150/schema_old.json
--rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v150/template.json
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v150/template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.640725 oemetadata-1.5.2/metadata/v151/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v151/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2289 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v151/context.json
--rw-r--r--   0 runner    (1001) docker     (121)    14722 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v151/example.json
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v151/example.py
--rw-r--r--   0 runner    (1001) docker     (121)    47296 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v151/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v151/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     5658 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v151/template.json
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v151/template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.644726 oemetadata-1.5.2/metadata/v152/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v152/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2289 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v152/context.json
--rw-r--r--   0 runner    (1001) docker     (121)    14929 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v152/example.json
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v152/example.py
--rw-r--r--   0 runner    (1001) docker     (121)    47296 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v152/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v152/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     5658 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v152/template.json
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-11-18 15:32:58.000000 oemetadata-1.5.2/metadata/v152/template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.644726 oemetadata-1.5.2/oemetadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3123 2022-11-18 15:33:08.000000 oemetadata-1.5.2/oemetadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2919 2022-11-18 15:33:08.000000 oemetadata-1.5.2/oemetadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 15:33:08.000000 oemetadata-1.5.2/oemetadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-18 15:33:08.000000 oemetadata-1.5.2/oemetadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-18 15:33:08.652726 oemetadata-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-11-18 15:32:58.000000 oemetadata-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.628725 oemetadata-1.5.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.644726 oemetadata-1.5.2/tests/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.644726 oemetadata-1.5.2/tests/metadata/latest/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/latest/test_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/latest/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/latest/test_template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.644726 oemetadata-1.5.2/tests/metadata/metaschema/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/metaschema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.644726 oemetadata-1.5.2/tests/metadata/metaschema/draft07/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/metaschema/draft07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/metaschema/draft07/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.644726 oemetadata-1.5.2/tests/metadata/v130/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v130/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v130/test_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v130/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v130/test_template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.648726 oemetadata-1.5.2/tests/metadata/v140/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v140/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v140/test_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v140/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v140/test_template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.648726 oemetadata-1.5.2/tests/metadata/v141/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v141/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v141/test_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v141/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v141/test_template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.648726 oemetadata-1.5.2/tests/metadata/v150/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v150/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v150/test_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v150/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v150/test_template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.652726 oemetadata-1.5.2/tests/metadata/v151/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v151/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v151/test_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v151/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v151/test_template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:33:08.652726 oemetadata-1.5.2/tests/metadata/v152/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v152/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v152/test_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v152/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-11-18 15:32:58.000000 oemetadata-1.5.2/tests/metadata/v152/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.990414 oemetadata-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-30 14:11:14.000000 oemetadata-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-30 14:11:29.990414 oemetadata-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-30 14:11:14.000000 oemetadata-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.974413 oemetadata-1.6.0/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.974413 oemetadata-1.6.0/metadata/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/latest/context.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/latest/example.json
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/latest/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56121 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/latest/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/latest/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/latest/template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/latest/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.974413 oemetadata-1.6.0/metadata/metaschema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/metaschema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.978413 oemetadata-1.6.0/metadata/metaschema/draft07/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/metaschema/draft07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/metaschema/draft07/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/metaschema/draft07/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.978413 oemetadata-1.6.0/metadata/v130/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v130/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v130/example.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v130/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v130/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v130/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v130/template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v130/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.978413 oemetadata-1.6.0/metadata/v140/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v140/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v140/example.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v140/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34811 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v140/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v140/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v140/template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v140/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.978413 oemetadata-1.6.0/metadata/v141/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v141/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v141/example.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v141/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34765 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v141/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v141/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v141/template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v141/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.982414 oemetadata-1.6.0/metadata/v150/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v150/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v150/context.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v150/example.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v150/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42880 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v150/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v150/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36713 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v150/schema_old.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v150/template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v150/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.982414 oemetadata-1.6.0/metadata/v151/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v151/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v151/context.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14733 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v151/example.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v151/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47296 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v151/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v151/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v151/template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v151/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.982414 oemetadata-1.6.0/metadata/v152/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v152/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v152/context.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v152/example.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v152/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47296 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v152/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v152/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v152/template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v152/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.982414 oemetadata-1.6.0/metadata/v160/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v160/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v160/context.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v160/example.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v160/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56121 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v160/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v160/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v160/template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 14:11:14.000000 oemetadata-1.6.0/metadata/v160/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.986414 oemetadata-1.6.0/oemetadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-30 14:11:29.000000 oemetadata-1.6.0/oemetadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-30 14:11:29.000000 oemetadata-1.6.0/oemetadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:11:29.000000 oemetadata-1.6.0/oemetadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 14:11:29.000000 oemetadata-1.6.0/oemetadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-30 14:11:29.990414 oemetadata-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-30 14:11:14.000000 oemetadata-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.974413 oemetadata-1.6.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.986414 oemetadata-1.6.0/tests/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.986414 oemetadata-1.6.0/tests/metadata/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/latest/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/latest/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/latest/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.986414 oemetadata-1.6.0/tests/metadata/metaschema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/metaschema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.986414 oemetadata-1.6.0/tests/metadata/metaschema/draft07/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/metaschema/draft07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/metaschema/draft07/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.986414 oemetadata-1.6.0/tests/metadata/v130/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v130/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v130/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v130/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v130/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.986414 oemetadata-1.6.0/tests/metadata/v140/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v140/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v140/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v140/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v140/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.986414 oemetadata-1.6.0/tests/metadata/v141/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v141/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v141/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v141/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v141/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.986414 oemetadata-1.6.0/tests/metadata/v150/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v150/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v150/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v150/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v150/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.986414 oemetadata-1.6.0/tests/metadata/v151/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v151/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v151/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v151/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v151/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.990414 oemetadata-1.6.0/tests/metadata/v152/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v152/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v152/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v152/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v152/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:29.990414 oemetadata-1.6.0/tests/metadata/v160/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v160/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v160/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v160/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 14:11:14.000000 oemetadata-1.6.0/tests/metadata/v160/test_template.py
```

### Comparing `oemetadata-1.5.2/LICENSE` & `oemetadata-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/PKG-INFO` & `oemetadata-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oemetadata
-Version: 1.5.2
+Version: 1.6.0
 Summary: Open Energy Platform (OEP) - metadata schemas, examples and templates package
 Home-page: https://github.com/OpenEnergyPlatform/oemetadata
 Author: Alexis Michaltsis
 Author-email: oep_dev@lists.riseup.net
 License: MIT
 Keywords: JSON metadata schema open energy platform oep
 Classifier: Intended Audience :: Developers
@@ -36,15 +36,15 @@
 
 This repository is licensed under [MIT License (MIT)](https://spdx.org/licenses/MIT.html) <br>
 The oemetadata is licensed under [Creative Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) <br>
 The oemetadata example and oemetadata template are licensed under [Creative Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/)
 
 ## Installation
 
-`pip install oep-metadata`
+`pip install oemetadata`
 
 ## Usage Examples
 
 ```
 from metadata.latest.example import OEMETADATA_LATEST_EXAMPLE
 
 print(OEMETADATA_LATEST_EXAMPLE)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oemetadata Version: 1.5.2 Summary: Open Energy
+Metadata-Version: 2.1 Name: oemetadata Version: 1.6.0 Summary: Open Energy
 Platform (OEP) - metadata schemas, examples and templates package Home-page:
 https://github.com/OpenEnergyPlatform/oemetadata Author: Alexis Michaltsis
 Author-email: oep_dev@lists.riseup.net License: MIT Keywords: JSON metadata
 schema open energy platform oep Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
@@ -21,15 +21,15 @@
 example.json) contains a basic metadata example ## License / Copyright This
 repository is licensed under [MIT License (MIT)](https://spdx.org/licenses/
 MIT.html)
 The oemetadata is licensed under [Creative Commons Zero v1.0 Universal](https:/
 /creativecommons.org/publicdomain/zero/1.0/)
 The oemetadata example and oemetadata template are licensed under [Creative
 Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/
-) ## Installation `pip install oep-metadata` ## Usage Examples ``` from
+) ## Installation `pip install oemetadata` ## Usage Examples ``` from
 metadata.latest.example import OEMETADATA_LATEST_EXAMPLE print
 (OEMETADATA_LATEST_EXAMPLE) ``` ``` from metadata.latest.schema import
 OEMETADATA_LATEST_SCHEMA print(OEMETADATA_LATEST_SCHEMA) ``` ``` from
 metadata.latest.template import OEMETADATA_LATEST_TEMPLATE print
 (OEMETADATA_LATEST_TEMPLATE) ``` ## Contributing For further contributing infos
 and conventions see: [CONTRIBUTING.md](./CONTRIBUTING.md) ## Release a new
 version See the complete instructions in the [RELEASE_PROCEDURE](./
```

### Comparing `oemetadata-1.5.2/README.md` & `oemetadata-1.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 This repository is licensed under [MIT License (MIT)](https://spdx.org/licenses/MIT.html) <br>
 The oemetadata is licensed under [Creative Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) <br>
 The oemetadata example and oemetadata template are licensed under [Creative Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/)
 
 ## Installation
 
-`pip install oep-metadata`
+`pip install oemetadata`
 
 ## Usage Examples
 
 ```
 from metadata.latest.example import OEMETADATA_LATEST_EXAMPLE
 
 print(OEMETADATA_LATEST_EXAMPLE)
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 example.json) contains a basic metadata example ## License / Copyright This
 repository is licensed under [MIT License (MIT)](https://spdx.org/licenses/
 MIT.html)
 The oemetadata is licensed under [Creative Commons Zero v1.0 Universal](https:/
 /creativecommons.org/publicdomain/zero/1.0/)
 The oemetadata example and oemetadata template are licensed under [Creative
 Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/
-) ## Installation `pip install oep-metadata` ## Usage Examples ``` from
+) ## Installation `pip install oemetadata` ## Usage Examples ``` from
 metadata.latest.example import OEMETADATA_LATEST_EXAMPLE print
 (OEMETADATA_LATEST_EXAMPLE) ``` ``` from metadata.latest.schema import
 OEMETADATA_LATEST_SCHEMA print(OEMETADATA_LATEST_SCHEMA) ``` ``` from
 metadata.latest.template import OEMETADATA_LATEST_TEMPLATE print
 (OEMETADATA_LATEST_TEMPLATE) ``` ## Contributing For further contributing infos
 and conventions see: [CONTRIBUTING.md](./CONTRIBUTING.md) ## Release a new
 version See the complete instructions in the [RELEASE_PROCEDURE](./
```

### Comparing `oemetadata-1.5.2/metadata/latest/context.json` & `oemetadata-1.6.0/metadata/latest/context.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/latest/example.json` & `oemetadata-1.6.0/metadata/v152/example.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'@context'": "'https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/develop/metadata/latest/context.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "@context": "https://github.com/OpenEnergyPlatform/oemetadata/blob/master/metadata/latest/context.json",
+    "@context": "https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/develop/metadata/latest/context.json",
     "@id": "https://databus.dbpedia.org/kurzum/mastr/bnetza-mastr/01.04.00",
     "_comment": {
         "dates": "Dates and time must follow the ISO8601 including time zone (YYYY-MM-DD or YYYY-MM-DDThh:mm:ss\u00b1hh)",
         "languages": "Languages must follow the IETF (BCP47) format (en-GB, en-US, de-DE)",
         "licenses": "License name must follow the SPDX License List (https://spdx.org/licenses/)",
         "metadata": "Metadata documentation and explanation (https://github.com/OpenEnergyPlatform/oemetadata)",
         "null": "If not applicable use: null",
```

### Comparing `oemetadata-1.5.2/metadata/latest/schema.json` & `oemetadata-1.6.0/metadata/v152/schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/master/metadata/v152/schema.json'",*

 * * "'description'": "'Open Energy Plaftorm (OEP) metadata schema v1.5.2'"}*

```diff
@@ -1,12 +1,12 @@
 {
-    "$id": "https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/master/oemetadata/latest/schema.json",
+    "$id": "https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/master/metadata/v152/schema.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
-    "description": "Open Energy Plaftorm (OEP) metadata schema latest",
+    "description": "Open Energy Plaftorm (OEP) metadata schema v1.5.2",
     "properties": {
         "@context": {
             "description": "Explanation of metadata keys in ontology terms. Example: https://raw.githubusercontent.com/LOD-GEOSS/databus-snippets/master/oep_metadata/context.jsonld",
             "title": "@context",
             "type": [
                 "string",
                 "null"
```

### Comparing `oemetadata-1.5.2/metadata/latest/template.json` & `oemetadata-1.6.0/metadata/latest/template.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'@context'": "'https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/develop/metadata/latest/context.json'",*

 * * "'metaMetadata'": "{'metadataVersion': 'OEP-1.6.0'}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "@context": null,
+    "@context": "https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/develop/metadata/latest/context.json",
     "@id": null,
     "_comment": {
         "dates": "Dates and time must follow the ISO8601 including time zone (YYYY-MM-DD or YYYY-MM-DDThh:mm:ss\u00b1hh)",
         "languages": "Languages must follow the IETF (BCP47) format (en-GB, en-US, de-DE)",
         "licenses": "License name must follow the SPDX License List (https://spdx.org/licenses/)",
         "metadata": "Metadata documentation and explanation (https://github.com/OpenEnergyPlatform/oemetadata)",
         "null": "If not applicable use: null",
@@ -49,15 +49,15 @@
     ],
     "metaMetadata": {
         "metadataLicense": {
             "name": "CC0-1.0",
             "path": "https://creativecommons.org/publicdomain/zero/1.0/",
             "title": "Creative Commons Zero v1.0 Universal"
         },
-        "metadataVersion": "OEP-1.5.2"
+        "metadataVersion": "OEP-1.6.0"
     },
     "name": null,
     "publicationDate": null,
     "resources": [
         {
             "dialect": {
                 "decimalSeparator": ".",
```

### Comparing `oemetadata-1.5.2/metadata/metaschema/draft07/schema.json` & `oemetadata-1.6.0/metadata/metaschema/draft07/schema.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v130/example.json` & `oemetadata-1.6.0/metadata/v130/example.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v130/schema.json` & `oemetadata-1.6.0/metadata/v130/schema.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v130/template.json` & `oemetadata-1.6.0/metadata/v130/template.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v140/example.json` & `oemetadata-1.6.0/metadata/v140/example.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v140/schema.json` & `oemetadata-1.6.0/metadata/v140/schema.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v140/template.json` & `oemetadata-1.6.0/metadata/v140/template.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v141/example.json` & `oemetadata-1.6.0/metadata/v141/example.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v141/schema.json` & `oemetadata-1.6.0/metadata/v141/schema.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v141/template.json` & `oemetadata-1.6.0/metadata/v141/template.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v150/context.json` & `oemetadata-1.6.0/metadata/v150/context.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v150/example.json` & `oemetadata-1.6.0/metadata/v150/example.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v150/schema.json` & `oemetadata-1.6.0/metadata/v150/schema.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v150/schema_old.json` & `oemetadata-1.6.0/metadata/v150/schema_old.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v150/template.json` & `oemetadata-1.6.0/metadata/v150/template.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v151/context.json` & `oemetadata-1.6.0/metadata/v151/context.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v151/example.json` & `oemetadata-1.6.0/metadata/v151/example.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'@context'": "'https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/develop/metadata/latest/context.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "@context": "https://github.com/OpenEnergyPlatform/oemetadata/blob/master/metadata/latest/context.json",
+    "@context": "https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/develop/metadata/latest/context.json",
     "@id": "https://databus.dbpedia.org/kurzum/mastr/bnetza-mastr/01.04.00",
     "_comment": {
         "dates": "Dates and time must follow the ISO8601 including time zone (YYYY-MM-DD or YYYY-MM-DDThh:mm:ss\u00b1hh)",
         "languages": "Languages must follow the IETF (BCP47) format (en-GB, en-US, de-DE)",
         "licenses": "License name must follow the SPDX License List (https://spdx.org/licenses/)",
         "metadata": "Metadata documentation and explanation (https://github.com/OpenEnergyPlatform/oemetadata)",
         "null": "If not applicable use: null",
```

### Comparing `oemetadata-1.5.2/metadata/v151/schema.json` & `oemetadata-1.6.0/metadata/v151/schema.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v151/template.json` & `oemetadata-1.6.0/metadata/v160/template.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'@context'": "'https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/develop/metadata/latest/context.json'",*

 * * "'metaMetadata'": "{'metadataVersion': 'OEP-1.6.0'}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "@context": null,
+    "@context": "https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/develop/metadata/latest/context.json",
     "@id": null,
     "_comment": {
         "dates": "Dates and time must follow the ISO8601 including time zone (YYYY-MM-DD or YYYY-MM-DDThh:mm:ss\u00b1hh)",
         "languages": "Languages must follow the IETF (BCP47) format (en-GB, en-US, de-DE)",
         "licenses": "License name must follow the SPDX License List (https://spdx.org/licenses/)",
         "metadata": "Metadata documentation and explanation (https://github.com/OpenEnergyPlatform/oemetadata)",
         "null": "If not applicable use: null",
@@ -49,15 +49,15 @@
     ],
     "metaMetadata": {
         "metadataLicense": {
             "name": "CC0-1.0",
             "path": "https://creativecommons.org/publicdomain/zero/1.0/",
             "title": "Creative Commons Zero v1.0 Universal"
         },
-        "metadataVersion": "OEP-1.5.1"
+        "metadataVersion": "OEP-1.6.0"
     },
     "name": null,
     "publicationDate": null,
     "resources": [
         {
             "dialect": {
                 "decimalSeparator": ".",
```

### Comparing `oemetadata-1.5.2/metadata/v152/context.json` & `oemetadata-1.6.0/metadata/v152/context.json`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/metadata/v152/example.json` & `oemetadata-1.6.0/metadata/latest/example.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888627819548873%*

 * *Differences: {"'@context'": "'https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/develop/metadata/latest/context.json'",*

 * * "'contributors'": "{insert: [(18, OrderedDict([('title', 'christian-rli'), ('email', None), "*

 * *                   "('date', '2023-05-30'), ('object', 'metadata'), ('comment', 'Release metadata "*

 * *                   "version OEP-1.6.0')]))]}",*

 * * "'id'": "'http://openenergyplatform.org/dataedit/view/model_draft/oep_metadata_table_example_v160'",*

 * * "'metaMetadata'": "{'metadataVersion': 'OEP-1. […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "@context": "https://github.com/OpenEnergyPlatform/oemetadata/blob/master/metadata/latest/context.json",
+    "@context": "https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/develop/metadata/latest/context.json",
     "@id": "https://databus.dbpedia.org/kurzum/mastr/bnetza-mastr/01.04.00",
     "_comment": {
         "dates": "Dates and time must follow the ISO8601 including time zone (YYYY-MM-DD or YYYY-MM-DDThh:mm:ss\u00b1hh)",
         "languages": "Languages must follow the IETF (BCP47) format (en-GB, en-US, de-DE)",
         "licenses": "License name must follow the SPDX License List (https://spdx.org/licenses/)",
         "metadata": "Metadata documentation and explanation (https://github.com/OpenEnergyPlatform/oemetadata)",
         "null": "If not applicable use: null",
@@ -143,18 +143,25 @@
         },
         {
             "comment": "Release metadata version OEP-1.5.2",
             "date": "2022-11-18",
             "email": null,
             "object": "metadata",
             "title": "jh-RLI"
+        },
+        {
+            "comment": "Release metadata version OEP-1.6.0",
+            "date": "2023-05-30",
+            "email": null,
+            "object": "metadata",
+            "title": "christian-rli"
         }
     ],
     "description": "This is an metadata example for example data. There is a corresponding table on the OEP for each metadata version.",
-    "id": "http://openenergyplatform.org/dataedit/view/model_draft/oep_metadata_table_example_v152",
+    "id": "http://openenergyplatform.org/dataedit/view/model_draft/oep_metadata_table_example_v160",
     "keywords": [
         "energy",
         "example",
         "template",
         "test"
     ],
     "language": [
@@ -174,28 +181,28 @@
     ],
     "metaMetadata": {
         "metadataLicense": {
             "name": "CC0-1.0",
             "path": "https://creativecommons.org/publicdomain/zero/1.0/",
             "title": "Creative Commons Zero v1.0 Universal"
         },
-        "metadataVersion": "OEP-1.5.2"
+        "metadataVersion": "OEP-1.6.0"
     },
-    "name": "oep_metadata_table_example_v152",
+    "name": "oep_metadata_table_example_v160",
     "publicationDate": "2022-02-15",
     "resources": [
         {
             "dialect": {
                 "decimalSeparator": ".",
                 "delimiter": null
             },
             "encoding": "UTF-8",
             "format": "PostgreSQL",
-            "name": "model_draft.oep_metadata_table_example_v152",
-            "path": "http://openenergyplatform.org/dataedit/view/model_draft/oep_metadata_table_example_v152",
+            "name": "model_draft.oep_metadata_table_example_v160",
+            "path": "http://openenergyplatform.org/dataedit/view/model_draft/oep_metadata_table_example_v160",
             "profile": "tabular-data-resource",
             "schema": {
                 "fields": [
                     {
                         "description": "Unique identifier",
                         "isAbout": [
                             {
@@ -398,9 +405,9 @@
                 "alignment": "right",
                 "end": "2019-06-01T23:00+01",
                 "resolution": "15 min",
                 "start": "2018-01-01T00:00+01"
             }
         ]
     },
-    "title": "Example title for metadata example - Version 1.5.2"
+    "title": "Example title for metadata example - Version 1.6.0"
 }
```

### Comparing `oemetadata-1.5.2/metadata/v152/template.json` & `oemetadata-1.6.0/metadata/v151/template.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'@context'": "'https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/develop/metadata/latest/context.json'",*

 * * "'metaMetadata'": "{'metadataVersion': 'OEP-1.5.1'}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "@context": null,
+    "@context": "https://raw.githubusercontent.com/OpenEnergyPlatform/oemetadata/develop/metadata/latest/context.json",
     "@id": null,
     "_comment": {
         "dates": "Dates and time must follow the ISO8601 including time zone (YYYY-MM-DD or YYYY-MM-DDThh:mm:ss\u00b1hh)",
         "languages": "Languages must follow the IETF (BCP47) format (en-GB, en-US, de-DE)",
         "licenses": "License name must follow the SPDX License List (https://spdx.org/licenses/)",
         "metadata": "Metadata documentation and explanation (https://github.com/OpenEnergyPlatform/oemetadata)",
         "null": "If not applicable use: null",
@@ -49,15 +49,15 @@
     ],
     "metaMetadata": {
         "metadataLicense": {
             "name": "CC0-1.0",
             "path": "https://creativecommons.org/publicdomain/zero/1.0/",
             "title": "Creative Commons Zero v1.0 Universal"
         },
-        "metadataVersion": "OEP-1.5.2"
+        "metadataVersion": "OEP-1.5.1"
     },
     "name": null,
     "publicationDate": null,
     "resources": [
         {
             "dialect": {
                 "decimalSeparator": ".",
```

### Comparing `oemetadata-1.5.2/oemetadata.egg-info/PKG-INFO` & `oemetadata-1.6.0/oemetadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oemetadata
-Version: 1.5.2
+Version: 1.6.0
 Summary: Open Energy Platform (OEP) - metadata schemas, examples and templates package
 Home-page: https://github.com/OpenEnergyPlatform/oemetadata
 Author: Alexis Michaltsis
 Author-email: oep_dev@lists.riseup.net
 License: MIT
 Keywords: JSON metadata schema open energy platform oep
 Classifier: Intended Audience :: Developers
@@ -36,15 +36,15 @@
 
 This repository is licensed under [MIT License (MIT)](https://spdx.org/licenses/MIT.html) <br>
 The oemetadata is licensed under [Creative Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) <br>
 The oemetadata example and oemetadata template are licensed under [Creative Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/)
 
 ## Installation
 
-`pip install oep-metadata`
+`pip install oemetadata`
 
 ## Usage Examples
 
 ```
 from metadata.latest.example import OEMETADATA_LATEST_EXAMPLE
 
 print(OEMETADATA_LATEST_EXAMPLE)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oemetadata Version: 1.5.2 Summary: Open Energy
+Metadata-Version: 2.1 Name: oemetadata Version: 1.6.0 Summary: Open Energy
 Platform (OEP) - metadata schemas, examples and templates package Home-page:
 https://github.com/OpenEnergyPlatform/oemetadata Author: Alexis Michaltsis
 Author-email: oep_dev@lists.riseup.net License: MIT Keywords: JSON metadata
 schema open energy platform oep Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
@@ -21,15 +21,15 @@
 example.json) contains a basic metadata example ## License / Copyright This
 repository is licensed under [MIT License (MIT)](https://spdx.org/licenses/
 MIT.html)
 The oemetadata is licensed under [Creative Commons Zero v1.0 Universal](https:/
 /creativecommons.org/publicdomain/zero/1.0/)
 The oemetadata example and oemetadata template are licensed under [Creative
 Commons Zero v1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/
-) ## Installation `pip install oep-metadata` ## Usage Examples ``` from
+) ## Installation `pip install oemetadata` ## Usage Examples ``` from
 metadata.latest.example import OEMETADATA_LATEST_EXAMPLE print
 (OEMETADATA_LATEST_EXAMPLE) ``` ``` from metadata.latest.schema import
 OEMETADATA_LATEST_SCHEMA print(OEMETADATA_LATEST_SCHEMA) ``` ``` from
 metadata.latest.template import OEMETADATA_LATEST_TEMPLATE print
 (OEMETADATA_LATEST_TEMPLATE) ``` ## Contributing For further contributing infos
 and conventions see: [CONTRIBUTING.md](./CONTRIBUTING.md) ## Release a new
 version See the complete instructions in the [RELEASE_PROCEDURE](./
```

### Comparing `oemetadata-1.5.2/oemetadata.egg-info/SOURCES.txt` & `oemetadata-1.6.0/oemetadata.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,22 @@
 metadata/v152/context.json
 metadata/v152/example.json
 metadata/v152/example.py
 metadata/v152/schema.json
 metadata/v152/schema.py
 metadata/v152/template.json
 metadata/v152/template.py
+metadata/v160/__init__.py
+metadata/v160/context.json
+metadata/v160/example.json
+metadata/v160/example.py
+metadata/v160/schema.json
+metadata/v160/schema.py
+metadata/v160/template.json
+metadata/v160/template.py
 oemetadata.egg-info/PKG-INFO
 oemetadata.egg-info/SOURCES.txt
 oemetadata.egg-info/dependency_links.txt
 oemetadata.egg-info/top_level.txt
 tests/metadata/__init__.py
 tests/metadata/latest/__init__.py
 tests/metadata/latest/test_example.py
@@ -92,8 +100,12 @@
 tests/metadata/v151/__init__.py
 tests/metadata/v151/test_example.py
 tests/metadata/v151/test_schema.py
 tests/metadata/v151/test_template.py
 tests/metadata/v152/__init__.py
 tests/metadata/v152/test_example.py
 tests/metadata/v152/test_schema.py
-tests/metadata/v152/test_template.py
+tests/metadata/v152/test_template.py
+tests/metadata/v160/__init__.py
+tests/metadata/v160/test_example.py
+tests/metadata/v160/test_schema.py
+tests/metadata/v160/test_template.py
```

### Comparing `oemetadata-1.5.2/setup.py` & `oemetadata-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="oemetadata",
-    version="1.5.2",
+    version="1.6.0",
     description="Open Energy Platform (OEP) - metadata schemas, examples and templates package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OpenEnergyPlatform/oemetadata",
     author="Alexis Michaltsis",
     author_email="oep_dev@lists.riseup.net",
     license="MIT",
```

### Comparing `oemetadata-1.5.2/tests/metadata/latest/test_schema.py` & `oemetadata-1.6.0/tests/metadata/latest/test_schema.py`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/tests/metadata/metaschema/draft07/test_schema.py` & `oemetadata-1.6.0/tests/metadata/metaschema/draft07/test_schema.py`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/tests/metadata/v130/test_schema.py` & `oemetadata-1.6.0/tests/metadata/v130/test_schema.py`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/tests/metadata/v140/test_schema.py` & `oemetadata-1.6.0/tests/metadata/v140/test_schema.py`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/tests/metadata/v141/test_schema.py` & `oemetadata-1.6.0/tests/metadata/v141/test_schema.py`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/tests/metadata/v150/test_schema.py` & `oemetadata-1.6.0/tests/metadata/v150/test_schema.py`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/tests/metadata/v151/test_schema.py` & `oemetadata-1.6.0/tests/metadata/v151/test_schema.py`

 * *Files identical despite different names*

### Comparing `oemetadata-1.5.2/tests/metadata/v152/test_schema.py` & `oemetadata-1.6.0/tests/metadata/v152/test_schema.py`

 * *Files identical despite different names*

