# Comparing `tmp/terminusdb-client-10.2.2.tar.gz` & `tmp/terminusdb-client-10.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminusdb-client-10.2.2.tar", last modified: Wed Mar 29 09:18:03 2023, max compression
+gzip compressed data, was "terminusdb-client-10.2.3.tar", last modified: Tue May 30 12:29:31 2023, max compression
```

## Comparing `terminusdb-client-10.2.2.tar` & `terminusdb-client-10.2.3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.538041 terminusdb-client-10.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-03-29 09:18:03.538041 terminusdb-client-10.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-29 09:18:03.542041 terminusdb-client-10.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.534041 terminusdb-client-10.2.2/terminusdb_client/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.534041 terminusdb-client-10.2.2/terminusdb_client/client/
--rw-r--r--   0 runner    (1001) docker     (123)    94773 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/client/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.534041 terminusdb-client-10.2.2/terminusdb_client/query_syntax/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/query_syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/query_syntax/query_syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.534041 terminusdb-client-10.2.2/terminusdb_client/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37919 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/schema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.534041 terminusdb-client-10.2.2/terminusdb_client/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/scripts/schema_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    34318 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/scripts/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.538041 terminusdb-client-10.2.2/terminusdb_client/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/AllServerRecords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/DBRecord.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/ans_cardinality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/ans_doctype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/ans_insert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/ans_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/ans_triple_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/connectCapabilitiesResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/connectionObjDump.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/getSchemaTurtleResponse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.538041 terminusdb-client-10.2.2/terminusdb_client/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/integration_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/integration_tests/mock_jsons.py
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/integration_tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/integration_tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/integration_tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/mockResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/serverRecordsFromCap.py
--rw-r--r--   0 runner    (1001) docker     (123)    26311 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/test_Client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/test_Schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/test_backwardsCompat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/test_woqlCore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/test_woqlExtra.py
--rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/test_woqlQuery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.538041 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlAndJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlCastJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlConcatJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlDeleteJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlDoctypeJson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlExtraJson.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlIdgenJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlJoinSplitJson.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlLimitStar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlMathJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlOptJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlOrJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlReJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlSelectJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlStarJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlTrimJson.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlWhenJson.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/woql_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/woql_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.538041 terminusdb-client-10.2.2/terminusdb_client/woqlclient/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/woqlclient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.538041 terminusdb-client-10.2.2/terminusdb_client/woqldataframe/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/woqldataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/woqldataframe/woqlDataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.538041 terminusdb-client-10.2.2/terminusdb_client/woqlquery/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/woqlquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/woqlquery/woql_core.py
--rw-r--r--   0 runner    (1001) docker     (123)   106610 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/woqlquery/woql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.538041 terminusdb-client-10.2.2/terminusdb_client/woqlschema/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-29 09:17:58.000000 terminusdb-client-10.2.2/terminusdb_client/woqlschema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:18:03.534041 terminusdb-client-10.2.2/terminusdb_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-03-29 09:18:03.000000 terminusdb-client-10.2.2/terminusdb_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-29 09:18:03.000000 terminusdb-client-10.2.2/terminusdb_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 09:18:03.000000 terminusdb-client-10.2.2/terminusdb_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-29 09:18:03.000000 terminusdb-client-10.2.2/terminusdb_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-29 09:18:03.000000 terminusdb-client-10.2.2/terminusdb_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-29 09:18:03.000000 terminusdb-client-10.2.2/terminusdb_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.559061 terminusdb-client-10.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-30 12:29:31.559061 terminusdb-client-10.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-30 12:29:31.559061 terminusdb-client-10.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.547061 terminusdb-client-10.2.3/terminusdb_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.547061 terminusdb-client-10.2.3/terminusdb_client/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    96359 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/client/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.547061 terminusdb-client-10.2.3/terminusdb_client/query_syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/query_syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/query_syntax/query_syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.547061 terminusdb-client-10.2.3/terminusdb_client/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37919 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/schema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.551061 terminusdb-client-10.2.3/terminusdb_client/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/scripts/schema_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34318 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/scripts/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.551061 terminusdb-client-10.2.3/terminusdb_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/AllServerRecords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/DBRecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/ans_cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/ans_doctype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/ans_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/ans_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/ans_triple_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/connectCapabilitiesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/connectionObjDump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/getSchemaTurtleResponse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.555061 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/mock_jsons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/mockResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/serverRecordsFromCap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26316 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_Schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_backwardsCompat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_woqlCore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_woqlExtra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/test_woqlQuery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.555061 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlAndJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlCastJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlConcatJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlDeleteJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlDoctypeJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlExtraJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlIdgenJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlJoinSplitJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlLimitStar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlMathJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlOptJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlOrJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlReJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlSelectJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlStarJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlTrimJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlWhenJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woql_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woql_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.555061 terminusdb-client-10.2.3/terminusdb_client/woqlclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqlclient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.555061 terminusdb-client-10.2.3/terminusdb_client/woqldataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqldataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqldataframe/woqlDataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.559061 terminusdb-client-10.2.3/terminusdb_client/woqlquery/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqlquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqlquery/woql_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106610 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqlquery/woql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.559061 terminusdb-client-10.2.3/terminusdb_client/woqlschema/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-30 12:29:26.000000 terminusdb-client-10.2.3/terminusdb_client/woqlschema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:29:31.547061 terminusdb-client-10.2.3/terminusdb_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-30 12:29:31.000000 terminusdb-client-10.2.3/terminusdb_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-30 12:29:31.000000 terminusdb-client-10.2.3/terminusdb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:29:31.000000 terminusdb-client-10.2.3/terminusdb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-30 12:29:31.000000 terminusdb-client-10.2.3/terminusdb_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 12:29:31.000000 terminusdb-client-10.2.3/terminusdb_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 12:29:31.000000 terminusdb-client-10.2.3/terminusdb_client.egg-info/top_level.txt
```

### Comparing `terminusdb-client-10.2.2/LICENSE` & `terminusdb-client-10.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/PKG-INFO` & `terminusdb-client-10.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 Metadata-Version: 2.1
 Name: terminusdb-client
-Version: 10.2.2
+Version: 10.2.3
 Summary: Python client for Terminus DB
 Home-page: https://github.com/terminusdb/terminusdb-client-python
 Author: TerminusDB group
 Author-email: terminusdatabase@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dataframe
 License-File: LICENSE
 
 [![TerminusDB Python Client](https://assets.terminusdb.com/readmes/terminusdb-client-python/header.gif)][terminusdb-client-python-docs]
 
-[terminusdb-client-python-docs]: https://terminusdb.github.io/terminusdb-client-python/
+[terminusdb-client-python-docs]: https://terminusdb.com/docs/guides/reference-guides/python-client-reference
 
 ---
 
 [![Discord](https://img.shields.io/discord/689805612053168129?label=Discord&logo=Discord&style=plastic)](https://discord.gg/yTJKAma)
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/TerminusDB?style=social)](https://www.reddit.com/r/TerminusDB/)
 [![Twitter](https://img.shields.io/twitter/follow/terminusdb?color=skyblue&label=Follow%20on%20Twitter&logo=twitter&style=flat)](https://twitter.com/TerminusDB)
 
 [![release version](https://img.shields.io/pypi/v/terminusdb-client.svg?logo=pypi)](https://pypi.python.org/pypi/terminusdb-client/)
 [![downloads](https://img.shields.io/pypi/dm/terminusdb-client.svg?logo=pypi)](https://pypi.python.org/pypi/terminusdb-client/)
 
 [![build status](https://img.shields.io/github/workflow/status/terminusdb/terminusdb-client-python/Python%20package?logo=github)](https://github.com/terminusdb/terminusdb-client-python/actions)
-[![documentation](https://img.shields.io/github/deployments/terminusdb/terminusdb-client-python/github-pages?label=documentation&logo=github)](https://terminusdb.github.io/terminusdb-client-python/)
+[![documentation](https://img.shields.io/github/deployments/terminusdb/terminusdb-client-python/github-pages?label=documentation&logo=github)](https://terminusdb.com/docs/guides/reference-guides/python-client-reference)
 [![code coverage](https://codecov.io/gh/terminusdb/terminusdb-client-python/branch/main/graph/badge.svg?token=BclAUaOPnQ)](https://codecov.io/gh/terminusdb/terminusdb-client-python)
 [![license](https://img.shields.io/github/license/terminusdb/terminusdb-client-python?color=pink&logo=apache)](https://github.com/terminusdb/terminusdb-client-python/blob/main/LICENSE)
 
-> Python client for TerminusDB and TerminusX.
+> Python client for TerminusDB and TerminusCMS.
 
 [**TerminusDB**][terminusdb] is an [open-source][terminusdb-repo] graph database
 and document store. It allows you to link JSON documents in a powerful knowledge
 graph all through a simple document API.
 
 [terminusdb]: https://terminusdb.com/
 [terminusdb-docs]: https://terminusdb.com/docs/
 [terminusdb-repo]: https://github.com/terminusdb/terminusdb
 
-**TerminusX** is TerminusDB as a service. SOC 2 certified hosting. Build your beta and get to market fast. Scale up and deploy your own instance. [Sign up now][dashboard].
+[**TerminusCMS**](https://terminusdb.com/terminuscms/) is a hosted headless content management system. It is built upon TerminusDB and is a developer focused data management platform for complex data and content infrastructure. [Sign up and clone a demo project to see how it works][dashboard].
 
 [dashboard]: https://dashboard.terminusdb.com/
 
 ## Requirements
 
 - [TerminusDB v10.0](https://github.com/terminusdb/terminusdb-server)
 - [Python >=3.7](https://www.python.org/downloads)
 
 ## Release Notes and Previous Versions
 
-TerminusDB Client v10.0 works with TerminusDB v10.0 and TerminusX. Please check the [Release Notes](https://github.com/terminusdb/terminusdb-client-python/blob/master/RELEASE_NOTES.md) to find out what has changed.
+TerminusDB Client v10.0 works with TerminusDB v10.0 and TerminusCMS. Please check the [Release Notes](https://github.com/terminusdb/terminusdb-client-python/blob/master/RELEASE_NOTES.md) to find out what has changed.
 
 ## Installation
 -  TerminusDB Client can be downloaded form PyPI using pip:
 `python -m pip install terminusdb-client`
 
 This only includes the core Python Client (Client) and WOQLQuery.
 
@@ -87,17 +87,17 @@
 ```Python
 from terminusdb_client import Client
 
 client = Client("http://127.0.0.1:6363/")
 client.connect()
 ```
 
-Connect to TerminusX
+Connect to TerminusCMS
 
-*check documentation for TerminusX about how to add the API token to the environment variable*
+*check documentation for TerminusCMS about how to add the [API token](https://terminusdb.com/docs/terminuscms/get-api-key) to the environment variable*
 
 
 ```Python
 from terminusdb_client import Client
 
 team="MyTeam"
 client = Client(f"https://dashboard.terminusdb.com/{team}/")
@@ -196,19 +196,19 @@
 
 ```bash
 $ tdbpy deletedb
 Do you want to delete 'mydb'? WARNING: This opertation is non-reversible. [y/N]: y
 mydb deleted.
 ```
 
-### Please check the [full Documentation](https://terminusdb.github.io/terminusdb-client-python/) for more information.
+### Please check the [full Documentation](https://terminusdb.com/docs/guides/reference-guides/python-client-reference) for more information.
 
-## Tutorials
+## Guides & Tutorials
 
-There is a [list of examples](https://terminusdb.github.io/terminusdb-client-python/tutorials.html) that uses the Python client in our [tutorial repo](https://github.com/terminusdb/terminus-tutorials/). As a start, we would recommend having a look at [create TerminusDB graph with Python client using Jupyter notebook](https://github.com/terminusdb/terminusdb-tutorials/blob/master/bike-tutorial/python/Create%20TerminusDB%20Graph%20with%20Python%20Client.ipynb)
+Visit our documentation for a range of short how to guides, [how-to use the Python Client](https://terminusdb.com/docs/guides/how-to-guides/use-the-python-client) and [how to use the collaboration features with the Python Client](https://terminusdb.com/docs/guides/how-to-guides/use-collaboration-features/with-the-python-client). Alternatively, undertake the  [Getting Started with the Python Client Tutorial Series.](https://github.com/terminusdb/terminusdb-tutorials/blob/main/getting_started/python-client/README.md).
 
 ## Testing
 
 1. Clone this repository
 `git clone https://github.com/terminusdb/terminusdb-client-python.git`
 
 2. Install all development dependencies using poetry
```

### Comparing `terminusdb-client-10.2.2/README.md` & `terminusdb-client-10.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 [![TerminusDB Python Client](https://assets.terminusdb.com/readmes/terminusdb-client-python/header.gif)][terminusdb-client-python-docs]
 
-[terminusdb-client-python-docs]: https://terminusdb.github.io/terminusdb-client-python/
+[terminusdb-client-python-docs]: https://terminusdb.com/docs/guides/reference-guides/python-client-reference
 
 ---
 
 [![Discord](https://img.shields.io/discord/689805612053168129?label=Discord&logo=Discord&style=plastic)](https://discord.gg/yTJKAma)
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/TerminusDB?style=social)](https://www.reddit.com/r/TerminusDB/)
 [![Twitter](https://img.shields.io/twitter/follow/terminusdb?color=skyblue&label=Follow%20on%20Twitter&logo=twitter&style=flat)](https://twitter.com/TerminusDB)
 
 [![release version](https://img.shields.io/pypi/v/terminusdb-client.svg?logo=pypi)](https://pypi.python.org/pypi/terminusdb-client/)
 [![downloads](https://img.shields.io/pypi/dm/terminusdb-client.svg?logo=pypi)](https://pypi.python.org/pypi/terminusdb-client/)
 
 [![build status](https://img.shields.io/github/workflow/status/terminusdb/terminusdb-client-python/Python%20package?logo=github)](https://github.com/terminusdb/terminusdb-client-python/actions)
-[![documentation](https://img.shields.io/github/deployments/terminusdb/terminusdb-client-python/github-pages?label=documentation&logo=github)](https://terminusdb.github.io/terminusdb-client-python/)
+[![documentation](https://img.shields.io/github/deployments/terminusdb/terminusdb-client-python/github-pages?label=documentation&logo=github)](https://terminusdb.com/docs/guides/reference-guides/python-client-reference)
 [![code coverage](https://codecov.io/gh/terminusdb/terminusdb-client-python/branch/main/graph/badge.svg?token=BclAUaOPnQ)](https://codecov.io/gh/terminusdb/terminusdb-client-python)
 [![license](https://img.shields.io/github/license/terminusdb/terminusdb-client-python?color=pink&logo=apache)](https://github.com/terminusdb/terminusdb-client-python/blob/main/LICENSE)
 
-> Python client for TerminusDB and TerminusX.
+> Python client for TerminusDB and TerminusCMS.
 
 [**TerminusDB**][terminusdb] is an [open-source][terminusdb-repo] graph database
 and document store. It allows you to link JSON documents in a powerful knowledge
 graph all through a simple document API.
 
 [terminusdb]: https://terminusdb.com/
 [terminusdb-docs]: https://terminusdb.com/docs/
 [terminusdb-repo]: https://github.com/terminusdb/terminusdb
 
-**TerminusX** is TerminusDB as a service. SOC 2 certified hosting. Build your beta and get to market fast. Scale up and deploy your own instance. [Sign up now][dashboard].
+[**TerminusCMS**](https://terminusdb.com/terminuscms/) is a hosted headless content management system. It is built upon TerminusDB and is a developer focused data management platform for complex data and content infrastructure. [Sign up and clone a demo project to see how it works][dashboard].
 
 [dashboard]: https://dashboard.terminusdb.com/
 
 ## Requirements
 
 - [TerminusDB v10.0](https://github.com/terminusdb/terminusdb-server)
 - [Python >=3.7](https://www.python.org/downloads)
 
 ## Release Notes and Previous Versions
 
-TerminusDB Client v10.0 works with TerminusDB v10.0 and TerminusX. Please check the [Release Notes](RELEASE_NOTES.md) to find out what has changed.
+TerminusDB Client v10.0 works with TerminusDB v10.0 and TerminusCMS. Please check the [Release Notes](RELEASE_NOTES.md) to find out what has changed.
 
 ## Installation
 -  TerminusDB Client can be downloaded form PyPI using pip:
 `python -m pip install terminusdb-client`
 
 This only includes the core Python Client (Client) and WOQLQuery.
 
@@ -72,17 +72,17 @@
 ```Python
 from terminusdb_client import Client
 
 client = Client("http://127.0.0.1:6363/")
 client.connect()
 ```
 
-Connect to TerminusX
+Connect to TerminusCMS
 
-*check documentation for TerminusX about how to add the API token to the environment variable*
+*check documentation for TerminusCMS about how to add the [API token](https://terminusdb.com/docs/terminuscms/get-api-key) to the environment variable*
 
 
 ```Python
 from terminusdb_client import Client
 
 team="MyTeam"
 client = Client(f"https://dashboard.terminusdb.com/{team}/")
@@ -181,19 +181,19 @@
 
 ```bash
 $ tdbpy deletedb
 Do you want to delete 'mydb'? WARNING: This opertation is non-reversible. [y/N]: y
 mydb deleted.
 ```
 
-### Please check the [full Documentation](https://terminusdb.github.io/terminusdb-client-python/) for more information.
+### Please check the [full Documentation](https://terminusdb.com/docs/guides/reference-guides/python-client-reference) for more information.
 
-## Tutorials
+## Guides & Tutorials
 
-There is a [list of examples](https://terminusdb.github.io/terminusdb-client-python/tutorials.html) that uses the Python client in our [tutorial repo](https://github.com/terminusdb/terminus-tutorials/). As a start, we would recommend having a look at [create TerminusDB graph with Python client using Jupyter notebook](https://github.com/terminusdb/terminusdb-tutorials/blob/master/bike-tutorial/python/Create%20TerminusDB%20Graph%20with%20Python%20Client.ipynb)
+Visit our documentation for a range of short how to guides, [how-to use the Python Client](https://terminusdb.com/docs/guides/how-to-guides/use-the-python-client) and [how to use the collaboration features with the Python Client](https://terminusdb.com/docs/guides/how-to-guides/use-collaboration-features/with-the-python-client). Alternatively, undertake the  [Getting Started with the Python Client Tutorial Series.](https://github.com/terminusdb/terminusdb-tutorials/blob/main/getting_started/python-client/README.md).
 
 ## Testing
 
 1. Clone this repository
 `git clone https://github.com/terminusdb/terminusdb-client-python.git`
 
 2. Install all development dependencies using poetry
```

### Comparing `terminusdb-client-10.2.2/pyproject.toml` & `terminusdb-client-10.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "terminusdb-client"
-version = "10.2.2"
+version = "10.2.3"
 description = "Python client for Terminus DB"
 authors = ["TerminusDB group"]
 license = "Apache Software License"
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4.0"
-requests = "*"
+requests = "<2.29.2"
 shed = "*"
 numpydoc = "*"
 typeguard = "~2.13.3"
 tqdm = "*"
 click = ">=8.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `terminusdb-client-10.2.2/setup.cfg` & `terminusdb-client-10.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/setup.py` & `terminusdb-client-10.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 requires = ["requests", "numpydoc", "click<9.0,>=7.0", "shed", "typeguard>=2,<3", "tqdm"]
 
 extras_require = {"dataframe": ["numpy >= 1.13.0", "pandas >= 0.23.0"]}
 
 setuptools.setup(
     name="terminusdb-client",
-    version="10.2.2",
+    version="10.2.3",
     author="TerminusDB group",
     author_email="terminusdatabase@gmail.com",
     description="Python client for Terminus DB",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"": ["LICENSE"]},
     url="https://github.com/terminusdb/terminusdb-client-python",
```

### Comparing `terminusdb-client-10.2.2/terminusdb_client/client/Client.py` & `terminusdb-client-10.2.3/terminusdb_client/client/Client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Client.py
 Client is the Python public API for TerminusDB"""
+import base64
 import copy
 import gzip
 import json
 import os
 import urllib.parse as urlparse
 import warnings
 from collections.abc import Iterable
@@ -265,27 +266,24 @@
             self._repo = value
 
     @property
     def ref(self):
         return self._ref
 
     @ref.setter
-    def ref(self, value):
-        if isinstance(value, str):
+    def ref(self, value: Optional[str]):
+        if value is not None:
             value = value.lower()
-        if value in ["local", "remote", None]:
-            self._ref = value
-        else:
-            raise ValueError("ref can only be 'local' or 'remote'")
+        self._ref = value
 
     def connect(
         self,
         team: str = "admin",
         db: Optional[str] = None,
-        remote_auth: str = None,
+        remote_auth: Optional[dict] = None,
         use_token: bool = False,
         jwt_token: Optional[str] = None,
         api_token: Optional[str] = None,
         key: str = "root",
         user: str = "admin",
         branch: str = "main",
         ref: Optional[str] = None,
@@ -298,15 +296,15 @@
 
         Parameters
         ----------
         team: str
             Name of the team, default to be "admin"
         db: optional, str
             Name of the database connected
-        remote_auth: optional, str
+        remote_auth: optional, dict
             Remote Auth setting
         key: optional, str
             API key for connecting, default to be "root"
         user: optional, str
             Name of the user, default to be "admin"
         use_token: bool
             Use token to connect. If both `jwt_token` and `api_token` is not provided (None), then it will use the ENV variable TERMINUSDB_ACCESS_TOKEN to connect as the API token
@@ -327,18 +325,21 @@
         --------
         >>> client = Client("http://127.0.0.1:6363")
         >>> client.connect(key="root", team="admin", user="admin", db="example_db")
         """
 
         self.team = team
         self.db = db
-        self._remote_auth = remote_auth
+        self._remote_auth_dict = remote_auth
         self._key = key
         self.user = user
-        self._use_token = use_token
+        if api_token:
+            self._use_token = True
+        else:
+            self._use_token = use_token
         self._jwt_token = jwt_token
         self._api_token = api_token
         self.branch = branch
         self.ref = ref
         self.repo = repo
         self._session = requests.Session()
         self._connected = True
@@ -619,15 +620,15 @@
 
         if team is None:
             team = self.team
 
         return self.connect(
             team=team,
             db=dbid,
-            remote_auth=self._remote_auth,
+            remote_auth=self._remote_auth_dict,
             key=self._key,
             user=self.user,
             branch=self.branch,
             ref=self.ref,
             repo=self.repo,
         )
 
@@ -933,15 +934,15 @@
         **kwargs,
     ) -> dict:
         """Retrieves the document of the iri_id
 
         Parameters
         ----------
         iri_id : str
-            Iri id for the docuemnt that is retriving
+            Iri id for the document that is to be retrieved
         graph_type : GraphType
             Graph type, either GraphType.INSTANCE or GraphType.SCHEMA.
         get_data_version: bool
             If the data version of the document(s) should be obtained. If True, the method return the result and the version as a tuple.
         kwargs:
             Additional boolean flags for retriving. Currently avaliable: "prefixed", "minimized", "unfold"
 
@@ -1670,15 +1671,17 @@
             headers=self._default_headers,
             json=rc_args,
             auth=self._auth(),
         )
 
         return json.loads(_finish_response(result))
 
-    def fetch(self, remote_id: str) -> dict:
+    def fetch(self, remote_id: str,
+              remote_auth: Optional[dict] = None,
+              ) -> dict:
         """Fatch the brach from a remote
 
         Parameters
         ----------
         remote_id: str
             id of the remote
 
@@ -1698,27 +1701,30 @@
 
     def push(
         self,
         remote: str = "origin",
         remote_branch: Optional[str] = None,
         message: Optional[str] = None,
         author: Optional[str] = None,
+        remote_auth: Optional[dict] = None,
     ) -> dict:
         """Push changes from a branch to a remote repo
 
         Parameters
         ----------
         remote: str
             remote to push to, default "origin"
         remote_branch: str, optional
             remote branch to push to, default to be your current barnch
         message: str, optional
             optional commit message
         author: str, optional
             option to overide the author of the operation
+        remote_auth: dict, optional
+            optional remote authorization (uses client remote auth otherwise)
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a database
 
         Examples
@@ -1740,18 +1746,21 @@
             )
         rc_args = {
             "remote": remote,
             "remote_branch": remote_branch,
             "author": author,
             "message": message,
         }
+        if self._remote_auth_dict or remote_auth:
+            headers = {'Authorization-Remote' : self._generate_remote_header(remote_auth) if remote_auth else self._remote_auth()}
+        headers.update(self._default_headers)
 
         result = self._session.post(
             self._push_url(),
-            headers=self._default_headers,
+            headers=headers,
             json=rc_args,
             auth=self._auth(),
         )
 
         return json.loads(_finish_response(result))
 
     def rebase(
@@ -2228,46 +2237,53 @@
                 json=request_dict,
                 auth=self._auth(),
             )
         )
         return json.loads(result)
 
     def clonedb(
-        self, clone_source: str, newid: str, description: Optional[str] = None
+            self, clone_source: str, newid: str, description: Optional[str] = None,
+            remote_auth: Optional[dict] = None
     ) -> None:
         """Clone a remote repository and create a local copy.
 
         Parameters
         ----------
         clone_source : str
             The source url of the repo to be cloned.
         newid : str
             Identifier of the new repository to create.
         Description : str, optional
             Optional description about the cloned database.
+        remote_auth : str, optional
+            Optional remote authorization (uses client remote auth otherwise)
 
         Raises
         ------
         InterfaceError
             if the client does not connect to a database
 
         Examples
         --------
         >>> client = Client("http://127.0.0.1:6363/")
         >>> client.clonedb("http://terminusdb.com/some_user/test_db", "my_test_db")
         """
-        self._check_connection()
+        self._check_connection(check_db=False)
         if description is None:
             description = f"New database {newid}"
+
+        if self._remote_auth_dict or remote_auth:
+            headers = {'Authorization-Remote' : self._generate_remote_header(remote_auth) if remote_auth else self._remote_auth()}
+        headers.update(self._default_headers)
         rc_args = {"remote_url": clone_source, "label": newid, "comment": description}
 
         _finish_response(
             self._session.post(
                 self._clone_url(newid),
-                headers=self._default_headers,
+                headers=headers,
                 json=rc_args,
                 auth=self._auth(),
             )
         )
 
     def _generate_commit(
         self, msg: Optional[str] = None, author: Optional[str] = None
@@ -2308,15 +2324,33 @@
             return JWTAuth(self._jwt_token)
         elif self._connected and self._api_token is not None:
             return APITokenAuth(self._api_token)
         elif self._connected:
             return APITokenAuth(os.environ["TERMINUSDB_ACCESS_TOKEN"])
         else:
             raise RuntimeError("Client not connected.")
-        # TODO: remote_auth
+
+    def _remote_auth(self):
+        if self._remote_auth_dict:
+            return self._generate_remote_header(self._remote_auth_dict)
+        elif "TERMINUSDB_REMOTE_ACCESS_TOKEN" in os.environ:
+            token = os.environ["TERMINUSDB_REMOTE_ACCESS_TOKEN"]
+            return f"Token {token}"
+
+    def _generate_remote_header(self, remote_auth: dict):
+        key_type = remote_auth['type']
+        key = remote_auth['key']
+        if key_type == 'http_basic':
+            username = remote_auth['username']
+            http_basic_creds = base64.b64encode(f"{username}:{key}".encode('utf-8'))
+            return f"Basic {http_basic_creds}"
+        elif key_type == 'token':
+            return f"Token {key}"
+        # JWT is the only key type remaining
+        return f"Bearer {key}"
 
     def create_organization(self, org: str) -> Optional[dict]:
         """
         Add a new organization
 
         Parameters
         ----------
```

### Comparing `terminusdb-client-10.2.2/terminusdb_client/errors.py` & `terminusdb-client-10.2.3/terminusdb_client/errors.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/query_syntax/query_syntax.py` & `terminusdb-client-10.2.3/terminusdb_client/query_syntax/query_syntax.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/schema/schema.py` & `terminusdb-client-10.2.3/terminusdb_client/schema/schema.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/scripts/schema_template.py` & `terminusdb-client-10.2.3/terminusdb_client/scripts/schema_template.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/scripts/scripts.py` & `terminusdb-client-10.2.3/terminusdb_client/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/AllServerRecords.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/AllServerRecords.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/DBRecord.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/DBRecord.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/ans_cardinality.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/ans_cardinality.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/ans_doctype.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/ans_doctype.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/ans_insert.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/ans_insert.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/ans_property.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/ans_property.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/ans_triple_quad.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/ans_triple_quad.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/conftest.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/connectCapabilitiesResponse.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/connectCapabilitiesResponse.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/connectionObjDump.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/connectionObjDump.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/getSchemaTurtleResponse.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/getSchemaTurtleResponse.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/integration_tests/conftest.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/integration_tests/mock_jsons.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/mock_jsons.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/integration_tests/test_client.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/integration_tests/test_schema.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/integration_tests/test_scripts.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/integration_tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/mockResponse.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/mockResponse.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/serverRecordsFromCap.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/serverRecordsFromCap.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/test_Client.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/test_Client.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
 @mock.patch.object(requests.Session, 'get', side_effect=mocked_request_success)
 def test_remote_auth(mocked_requests):
     client = Client("http://localhost:6363")
     auth_setting = {"type": "jwt", "user": "admin", "key": "<token>"}
     client.connect(
         user="admin", team="admin", key="root", remote_auth=auth_setting
     )
-    result = client._remote_auth
+    result = client._remote_auth_dict
     assert result == auth_setting
 
 
 @mock.patch.object(requests.Session, 'head', side_effect=mocked_request_success)
 @mock.patch.object(requests.Session, 'get', side_effect=mocked_request_success)
 def test_set_db(mocked_requests, mocked_requests2):
     client = Client("http://localhost:6363")
```

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/test_Schema.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/test_Schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,14 +202,35 @@
     )
     client = Client("http://127.0.0.1:6366")
     result = client._convert_document(gavin, 'instance')
     # Finds the internal object and splays it out properly
     assert (len(result) == 2)
 
 
+def test_person_sys_json():
+    schema_json = {
+        "@id": "PersonJSONTest",
+        "@key": {
+            "@type": "Random"
+        },
+        "@type": "Class",
+        "metadata": {
+            "@class": "sys:JSON",
+            "@type": "Optional"
+        }
+    }
+    schema = Schema()
+    test_result = schema._construct_class(schema_json)
+    result = {'@id': 'PersonJSONTest',
+              '@key': {'@type': 'Random'},
+              '@type': 'Class',
+              'metadata': {'@class': 'sys:JSON', '@type': 'Optional'}}
+    assert test_result._to_dict() == result
+
+
 def test_id_and_capture(test_schema):
     my_schema = test_schema
     Person = my_schema.object.get("Person")
     Country = my_schema.object.get("Country")
     Address = my_schema.object.get("Address")
 
     ireland = Country()
```

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/test_backwardsCompat.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/test_backwardsCompat.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/test_scripts.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/test_woqlExtra.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/test_woqlExtra.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/test_woqlQuery.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/test_woqlQuery.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlAndJson.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlAndJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlDeleteJson.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlDeleteJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlDoctypeJson.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlDoctypeJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlExtraJson.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlExtraJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlIdgenJson.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlIdgenJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlJoinSplitJson.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlJoinSplitJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlJson.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlMathJson.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlMathJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlOrJson.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlOrJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/tests/woqljson/woqlSelectJson.py` & `terminusdb-client-10.2.3/terminusdb_client/tests/woqljson/woqlSelectJson.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/woql_type.py` & `terminusdb-client-10.2.3/terminusdb_client/woql_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import ForwardRef, List, Optional, Set, Union
 
 CONVERT_TYPE = {
     str: "xsd:string",
     bool: "xsd:boolean",
     float: "xsd:double",
     int: "xsd:integer",
+    dict: "sys:JSON",
     dt.datetime: "xsd:dateTime",
     dt.date: "xsd:date",
     dt.time: "xsd:time",
     dt.timedelta: "xsd:duration",
 }
```

### Comparing `terminusdb-client-10.2.2/terminusdb_client/woql_utils.py` & `terminusdb-client-10.2.3/terminusdb_client/woql_utils.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/woqldataframe/woqlDataframe.py` & `terminusdb-client-10.2.3/terminusdb_client/woqldataframe/woqlDataframe.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/woqlquery/woql_core.py` & `terminusdb-client-10.2.3/terminusdb_client/woqlquery/woql_core.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client/woqlquery/woql_query.py` & `terminusdb-client-10.2.3/terminusdb_client/woqlquery/woql_query.py`

 * *Files identical despite different names*

### Comparing `terminusdb-client-10.2.2/terminusdb_client.egg-info/PKG-INFO` & `terminusdb-client-10.2.3/terminusdb_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 Metadata-Version: 2.1
 Name: terminusdb-client
-Version: 10.2.2
+Version: 10.2.3
 Summary: Python client for Terminus DB
 Home-page: https://github.com/terminusdb/terminusdb-client-python
 Author: TerminusDB group
 Author-email: terminusdatabase@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dataframe
 License-File: LICENSE
 
 [![TerminusDB Python Client](https://assets.terminusdb.com/readmes/terminusdb-client-python/header.gif)][terminusdb-client-python-docs]
 
-[terminusdb-client-python-docs]: https://terminusdb.github.io/terminusdb-client-python/
+[terminusdb-client-python-docs]: https://terminusdb.com/docs/guides/reference-guides/python-client-reference
 
 ---
 
 [![Discord](https://img.shields.io/discord/689805612053168129?label=Discord&logo=Discord&style=plastic)](https://discord.gg/yTJKAma)
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/TerminusDB?style=social)](https://www.reddit.com/r/TerminusDB/)
 [![Twitter](https://img.shields.io/twitter/follow/terminusdb?color=skyblue&label=Follow%20on%20Twitter&logo=twitter&style=flat)](https://twitter.com/TerminusDB)
 
 [![release version](https://img.shields.io/pypi/v/terminusdb-client.svg?logo=pypi)](https://pypi.python.org/pypi/terminusdb-client/)
 [![downloads](https://img.shields.io/pypi/dm/terminusdb-client.svg?logo=pypi)](https://pypi.python.org/pypi/terminusdb-client/)
 
 [![build status](https://img.shields.io/github/workflow/status/terminusdb/terminusdb-client-python/Python%20package?logo=github)](https://github.com/terminusdb/terminusdb-client-python/actions)
-[![documentation](https://img.shields.io/github/deployments/terminusdb/terminusdb-client-python/github-pages?label=documentation&logo=github)](https://terminusdb.github.io/terminusdb-client-python/)
+[![documentation](https://img.shields.io/github/deployments/terminusdb/terminusdb-client-python/github-pages?label=documentation&logo=github)](https://terminusdb.com/docs/guides/reference-guides/python-client-reference)
 [![code coverage](https://codecov.io/gh/terminusdb/terminusdb-client-python/branch/main/graph/badge.svg?token=BclAUaOPnQ)](https://codecov.io/gh/terminusdb/terminusdb-client-python)
 [![license](https://img.shields.io/github/license/terminusdb/terminusdb-client-python?color=pink&logo=apache)](https://github.com/terminusdb/terminusdb-client-python/blob/main/LICENSE)
 
-> Python client for TerminusDB and TerminusX.
+> Python client for TerminusDB and TerminusCMS.
 
 [**TerminusDB**][terminusdb] is an [open-source][terminusdb-repo] graph database
 and document store. It allows you to link JSON documents in a powerful knowledge
 graph all through a simple document API.
 
 [terminusdb]: https://terminusdb.com/
 [terminusdb-docs]: https://terminusdb.com/docs/
 [terminusdb-repo]: https://github.com/terminusdb/terminusdb
 
-**TerminusX** is TerminusDB as a service. SOC 2 certified hosting. Build your beta and get to market fast. Scale up and deploy your own instance. [Sign up now][dashboard].
+[**TerminusCMS**](https://terminusdb.com/terminuscms/) is a hosted headless content management system. It is built upon TerminusDB and is a developer focused data management platform for complex data and content infrastructure. [Sign up and clone a demo project to see how it works][dashboard].
 
 [dashboard]: https://dashboard.terminusdb.com/
 
 ## Requirements
 
 - [TerminusDB v10.0](https://github.com/terminusdb/terminusdb-server)
 - [Python >=3.7](https://www.python.org/downloads)
 
 ## Release Notes and Previous Versions
 
-TerminusDB Client v10.0 works with TerminusDB v10.0 and TerminusX. Please check the [Release Notes](https://github.com/terminusdb/terminusdb-client-python/blob/master/RELEASE_NOTES.md) to find out what has changed.
+TerminusDB Client v10.0 works with TerminusDB v10.0 and TerminusCMS. Please check the [Release Notes](https://github.com/terminusdb/terminusdb-client-python/blob/master/RELEASE_NOTES.md) to find out what has changed.
 
 ## Installation
 -  TerminusDB Client can be downloaded form PyPI using pip:
 `python -m pip install terminusdb-client`
 
 This only includes the core Python Client (Client) and WOQLQuery.
 
@@ -87,17 +87,17 @@
 ```Python
 from terminusdb_client import Client
 
 client = Client("http://127.0.0.1:6363/")
 client.connect()
 ```
 
-Connect to TerminusX
+Connect to TerminusCMS
 
-*check documentation for TerminusX about how to add the API token to the environment variable*
+*check documentation for TerminusCMS about how to add the [API token](https://terminusdb.com/docs/terminuscms/get-api-key) to the environment variable*
 
 
 ```Python
 from terminusdb_client import Client
 
 team="MyTeam"
 client = Client(f"https://dashboard.terminusdb.com/{team}/")
@@ -196,19 +196,19 @@
 
 ```bash
 $ tdbpy deletedb
 Do you want to delete 'mydb'? WARNING: This opertation is non-reversible. [y/N]: y
 mydb deleted.
 ```
 
-### Please check the [full Documentation](https://terminusdb.github.io/terminusdb-client-python/) for more information.
+### Please check the [full Documentation](https://terminusdb.com/docs/guides/reference-guides/python-client-reference) for more information.
 
-## Tutorials
+## Guides & Tutorials
 
-There is a [list of examples](https://terminusdb.github.io/terminusdb-client-python/tutorials.html) that uses the Python client in our [tutorial repo](https://github.com/terminusdb/terminus-tutorials/). As a start, we would recommend having a look at [create TerminusDB graph with Python client using Jupyter notebook](https://github.com/terminusdb/terminusdb-tutorials/blob/master/bike-tutorial/python/Create%20TerminusDB%20Graph%20with%20Python%20Client.ipynb)
+Visit our documentation for a range of short how to guides, [how-to use the Python Client](https://terminusdb.com/docs/guides/how-to-guides/use-the-python-client) and [how to use the collaboration features with the Python Client](https://terminusdb.com/docs/guides/how-to-guides/use-collaboration-features/with-the-python-client). Alternatively, undertake the  [Getting Started with the Python Client Tutorial Series.](https://github.com/terminusdb/terminusdb-tutorials/blob/main/getting_started/python-client/README.md).
 
 ## Testing
 
 1. Clone this repository
 `git clone https://github.com/terminusdb/terminusdb-client-python.git`
 
 2. Install all development dependencies using poetry
```

### Comparing `terminusdb-client-10.2.2/terminusdb_client.egg-info/SOURCES.txt` & `terminusdb-client-10.2.3/terminusdb_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

