# Comparing `tmp/spetlr-1.1.89.tar.gz` & `tmp/spetlr-1.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spetlr-1.1.89.tar", last modified: Wed May 24 08:42:41 2023, max compression
+gzip compressed data, was "spetlr-1.1.94.tar", last modified: Tue May 30 11:12:43 2023, max compression
```

## Comparing `spetlr-1.1.89.tar` & `spetlr-1.1.94.tar`

### file list

```diff
@@ -1,276 +1,255 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.861817 spetlr-1.1.89/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-24 08:42:28.000000 spetlr-1.1.89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 08:42:28.000000 spetlr-1.1.89/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-24 08:42:41.861817 spetlr-1.1.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-24 08:42:28.000000 spetlr-1.1.89/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-24 08:42:28.000000 spetlr-1.1.89/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-24 08:42:41.865817 spetlr-1.1.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 08:42:28.000000 spetlr-1.1.89/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.821817 spetlr-1.1.89/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.829817 spetlr-1.1.89/src/spetlr/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/alias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.833817 spetlr-1.1.89/src/spetlr/cache/
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/cache/CachedLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/cache/CachedLoaderParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.833817 spetlr-1.1.89/src/spetlr/config_master/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/config_master/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.833817 spetlr-1.1.89/src/spetlr/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.833817 spetlr-1.1.89/src/spetlr/configurator/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/_cli/generate_keys_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    15383 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.833817 spetlr-1.1.89/src/spetlr/configurator/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/StatementBlocks.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/init_sqlparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/parse_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.837817 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.837817 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/engine/filter_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/engine/grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/engine/statement_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.837817 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/filters/aligned_indent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/filters/others.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/filters/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/filters/reindent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/filters/right_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/filters/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20547 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/sqlparse/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/substructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/configurator/sql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.837817 spetlr-1.1.89/src/spetlr/cosmos/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/cosmos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/cosmos/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/cosmos/cosmos_base_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/cosmos/cosmos_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/db_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.837817 spetlr-1.1.89/src/spetlr/delta/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/delta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/delta/db_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/delta/delta_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.841817 spetlr-1.1.89/src/spetlr/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/eh/EventHubCapture.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/eh/EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/eh/EventHubJsonPublisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/eh/EventHubStream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/eh/PartitionSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/eh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/eh/eh_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.841817 spetlr-1.1.89/src/spetlr/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/entry_points/generalized_task_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/entry_points/task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.841817 spetlr-1.1.89/src/spetlr/etl/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.841817 spetlr-1.1.89/src/spetlr/etl/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/extractors/incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/extractors/schema_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/extractors/simple_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.845817 spetlr-1.1.89/src/spetlr/etl/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/loaders/DeleteDataLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/loaders/UpsertLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/loaders/simple_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/loaders/simple_sql_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/etl/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.845817 spetlr-1.1.89/src/spetlr/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/exceptions/cli_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/exceptions/configurator_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.845817 spetlr-1.1.89/src/spetlr/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/extractors/eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.845817 spetlr-1.1.89/src/spetlr/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/formatting/git_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.845817 spetlr-1.1.89/src/spetlr/mount/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/mount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/mount/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.845817 spetlr-1.1.89/src/spetlr/orchestrators/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/orchestrators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.845817 spetlr-1.1.89/src/spetlr/orchestrators/eh2bronze/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/orchestrators/eh2bronze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.845817 spetlr-1.1.89/src/spetlr/orchestrators/eh2silver/
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/orchestrators/eh2silver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.845817 spetlr-1.1.89/src/spetlr/orchestrators/ehjson2delta/
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/orchestrators/ehjson2delta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.845817 spetlr-1.1.89/src/spetlr/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/reporting/JobReflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/reporting/SlackNotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.845817 spetlr-1.1.89/src/spetlr/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/schema_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/schema_manager/schema_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/schema_manager/spark_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.849817 spetlr-1.1.89/src/spetlr/singleton/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/singleton/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/spark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.849817 spetlr-1.1.89/src/spetlr/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/sql/BaseExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/sql/CommonBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/sql/SqlBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/sql/SqlExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/sql/SqlServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/sql/SqlServerBaseOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/sql/sql_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.849817 spetlr-1.1.89/src/spetlr/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/tables/TableHandle.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/tables/ThMaker.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.853817 spetlr-1.1.89/src/spetlr/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/dropColumnsTransformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/drop_oldest_duplicate_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/selectColumnsTransformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/simple_sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/timezone_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/union_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/transformers/validfromto_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.853817 spetlr-1.1.89/src/spetlr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/utils/CheckDfMerge.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/utils/CleanupTestDatabases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/utils/DataframeCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/utils/DropOldestDuplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/utils/GetMergeStatement.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/utils/MockExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/utils/MockLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/utils/SelectAndCastColumns.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 08:42:28.000000 spetlr-1.1.89/src/spetlr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.829817 spetlr-1.1.89/src/spetlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-24 08:42:41.000000 spetlr-1.1.89/src/spetlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-05-24 08:42:41.000000 spetlr-1.1.89/src/spetlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:42:41.000000 spetlr-1.1.89/src/spetlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-24 08:42:41.000000 spetlr-1.1.89/src/spetlr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:42:41.000000 spetlr-1.1.89/src/spetlr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-24 08:42:41.000000 spetlr-1.1.89/src/spetlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 08:42:41.000000 spetlr-1.1.89/src/spetlr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.825817 spetlr-1.1.89/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.825817 spetlr-1.1.89/tests/cluster/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.853817 spetlr-1.1.89/tests/cluster/cache/
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/cache/test_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.853817 spetlr-1.1.89/tests/cluster/cosmos/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/cosmos/test_cosmos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.853817 spetlr-1.1.89/tests/cluster/db/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/db/test_db_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.853817 spetlr-1.1.89/tests/cluster/delta/
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/delta/test_cleanup_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/delta/test_delta_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.853817 spetlr-1.1.89/tests/cluster/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/eh/test_eh_json_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/eh/test_eh_json_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/eh/test_eh_saving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.857817 spetlr-1.1.89/tests/cluster/etl/
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/etl/test_delete_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/etl/test_deltaupsert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/etl/test_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/etl/test_incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/etl/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/etl/test_orchestrator_etl_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/etl/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/etl/test_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/etl/test_upsertloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.857817 spetlr-1.1.89/tests/cluster/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.857817 spetlr-1.1.89/tests/cluster/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.857817 spetlr-1.1.89/tests/cluster/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/sql/test_deliveryexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/sql/test_deliverysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/sql/test_deliverysqlspn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/sql/test_simple_sql_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/sql/test_sqlhandle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.857817 spetlr-1.1.89/tests/cluster/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/transformations/test_merge_df_into_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/cluster/transformations/test_union_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.857817 spetlr-1.1.89/tests/local/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.857817 spetlr-1.1.89/tests/local/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/configurator/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/configurator/test_configurator_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.857817 spetlr-1.1.89/tests/local/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/eh/test_EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/eh/test_ehto_bronze_and_silver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/eh/test_ehtodeltabronze_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/eh/test_ehtodeltabronze_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/eh/test_ehtodeltasilver_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.857817 spetlr-1.1.89/tests/local/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/entry_points/test_task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.857817 spetlr-1.1.89/tests/local/etl/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/etl/test_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.857817 spetlr-1.1.89/tests/local/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/extractors/test_eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.857817 spetlr-1.1.89/tests/local/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.861817 spetlr-1.1.89/tests/local/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.861817 spetlr-1.1.89/tests/local/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/sql/test_SqlExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/test_get_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/test_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/test_sqlServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/test_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.861817 spetlr-1.1.89/tests/local/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/transformers/test_concat_df.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/transformers/test_drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/transformers/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/transformers/test_fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/transformers/test_join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/transformers/test_select_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/transformers/test_simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/transformers/test_timezone_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/transformers/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/transformers/test_union_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/transformers/test_validfromto_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:42:41.861817 spetlr-1.1.89/tests/local/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/utils/test_cleandatabases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/utils/test_dataframe_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/utils/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/utils/test_getmergestatement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/utils/test_mock_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-05-24 08:42:28.000000 spetlr-1.1.89/tests/local/utils/test_selectandcastcolumns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.055467 spetlr-1.1.94/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 11:12:30.000000 spetlr-1.1.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 11:12:30.000000 spetlr-1.1.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-30 11:12:43.055467 spetlr-1.1.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-30 11:12:30.000000 spetlr-1.1.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-30 11:12:30.000000 spetlr-1.1.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-30 11:12:43.059467 spetlr-1.1.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:12:30.000000 spetlr-1.1.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.027467 spetlr-1.1.94/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.039467 spetlr-1.1.94/src/spetlr/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/alias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.039467 spetlr-1.1.94/src/spetlr/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/cache/CachedLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/cache/CachedLoaderParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.039467 spetlr-1.1.94/src/spetlr/config_master/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/config_master/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.039467 spetlr-1.1.94/src/spetlr/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.039467 spetlr-1.1.94/src/spetlr/configurator/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/_cli/generate_keys_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15383 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.043467 spetlr-1.1.94/src/spetlr/configurator/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/sql/StatementBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/sql/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/sql/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/sql/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/sql/init_sqlparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/sql/parse_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/sql/substructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/sql/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/configurator/sql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.043467 spetlr-1.1.94/src/spetlr/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/cosmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/cosmos/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/cosmos/cosmos_base_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/cosmos/cosmos_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/db_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.043467 spetlr-1.1.94/src/spetlr/delta/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/delta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/delta/db_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/delta/delta_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.043467 spetlr-1.1.94/src/spetlr/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/eh/EventHubCapture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/eh/EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/eh/EventHubJsonPublisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/eh/EventHubStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/eh/PartitionSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/eh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/eh/eh_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.043467 spetlr-1.1.94/src/spetlr/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/entry_points/generalized_task_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/entry_points/task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.043467 spetlr-1.1.94/src/spetlr/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.043467 spetlr-1.1.94/src/spetlr/etl/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/extractors/incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/extractors/schema_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/extractors/simple_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.043467 spetlr-1.1.94/src/spetlr/etl/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/loaders/DeleteDataLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/loaders/UpsertLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/loaders/simple_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/loaders/simple_sql_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/etl/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.047467 spetlr-1.1.94/src/spetlr/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/exceptions/cli_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/exceptions/configurator_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.047467 spetlr-1.1.94/src/spetlr/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/extractors/eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.047467 spetlr-1.1.94/src/spetlr/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/formatting/git_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.047467 spetlr-1.1.94/src/spetlr/mount/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/mount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/mount/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.047467 spetlr-1.1.94/src/spetlr/orchestrators/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/orchestrators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.047467 spetlr-1.1.94/src/spetlr/orchestrators/eh2bronze/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/orchestrators/eh2bronze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.047467 spetlr-1.1.94/src/spetlr/orchestrators/eh2silver/
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/orchestrators/eh2silver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.047467 spetlr-1.1.94/src/spetlr/orchestrators/ehjson2delta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/orchestrators/ehjson2delta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.047467 spetlr-1.1.94/src/spetlr/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/reporting/JobReflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/reporting/SlackNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.047467 spetlr-1.1.94/src/spetlr/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/schema_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/schema_manager/schema_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/schema_manager/spark_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.047467 spetlr-1.1.94/src/spetlr/singleton/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/singleton/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/spark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.047467 spetlr-1.1.94/src/spetlr/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/sql/BaseExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/sql/CommonBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/sql/SqlBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/sql/SqlExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/sql/SqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/sql/SqlServerBaseOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/sql/sql_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.047467 spetlr-1.1.94/src/spetlr/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/tables/TableHandle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/tables/ThMaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.051468 spetlr-1.1.94/src/spetlr/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/country_to_alphacode_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/dropColumnsTransformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/drop_oldest_duplicate_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/selectColumnsTransformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/simple_sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/timezone_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/union_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/transformers/validfromto_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.051468 spetlr-1.1.94/src/spetlr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/utils/CheckDfMerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/utils/CleanupTestDatabases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/utils/DataframeCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/utils/DropOldestDuplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/utils/GetMergeStatement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/utils/MockExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/utils/MockLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/utils/SelectAndCastColumns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 11:12:30.000000 spetlr-1.1.94/src/spetlr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.039467 spetlr-1.1.94/src/spetlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-30 11:12:42.000000 spetlr-1.1.94/src/spetlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-05-30 11:12:42.000000 spetlr-1.1.94/src/spetlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:12:42.000000 spetlr-1.1.94/src/spetlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 11:12:42.000000 spetlr-1.1.94/src/spetlr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:12:42.000000 spetlr-1.1.94/src/spetlr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-30 11:12:42.000000 spetlr-1.1.94/src/spetlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 11:12:42.000000 spetlr-1.1.94/src/spetlr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.035467 spetlr-1.1.94/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.035467 spetlr-1.1.94/tests/cluster/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.051468 spetlr-1.1.94/tests/cluster/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/cache/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.051468 spetlr-1.1.94/tests/cluster/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/cosmos/test_cosmos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.051468 spetlr-1.1.94/tests/cluster/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/db/test_db_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.051468 spetlr-1.1.94/tests/cluster/delta/
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/delta/test_cleanup_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/delta/test_delta_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/delta/test_sparkexecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.051468 spetlr-1.1.94/tests/cluster/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/eh/test_eh_json_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/eh/test_eh_json_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/eh/test_eh_saving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.051468 spetlr-1.1.94/tests/cluster/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/etl/test_delete_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/etl/test_deltaupsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/etl/test_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/etl/test_incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/etl/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/etl/test_orchestrator_etl_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/etl/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/etl/test_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/etl/test_upsertloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.051468 spetlr-1.1.94/tests/cluster/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.051468 spetlr-1.1.94/tests/cluster/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.051468 spetlr-1.1.94/tests/cluster/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/sql/test_deliveryexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/sql/test_deliverysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/sql/test_deliverysqlspn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/sql/test_simple_sql_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/sql/test_sqlhandle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.051468 spetlr-1.1.94/tests/cluster/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/transformations/test_merge_df_into_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/cluster/transformations/test_union_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.055467 spetlr-1.1.94/tests/local/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.055467 spetlr-1.1.94/tests/local/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/configurator/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/configurator/test_configurator_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.055467 spetlr-1.1.94/tests/local/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/eh/test_EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/eh/test_ehto_bronze_and_silver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/eh/test_ehtodeltabronze_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/eh/test_ehtodeltabronze_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/eh/test_ehtodeltasilver_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.055467 spetlr-1.1.94/tests/local/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/entry_points/test_task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.055467 spetlr-1.1.94/tests/local/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/etl/test_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.055467 spetlr-1.1.94/tests/local/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/extractors/test_eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.055467 spetlr-1.1.94/tests/local/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.055467 spetlr-1.1.94/tests/local/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.055467 spetlr-1.1.94/tests/local/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/sql/test_SqlExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/test_get_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/test_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/test_sqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/test_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.055467 spetlr-1.1.94/tests/local/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_concat_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_country_to_alphacode_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_select_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_timezone_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_union_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/transformers/test_validfromto_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:12:43.055467 spetlr-1.1.94/tests/local/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/utils/test_cleandatabases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/utils/test_dataframe_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/utils/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/utils/test_getmergestatement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/utils/test_mock_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-05-30 11:12:30.000000 spetlr-1.1.94/tests/local/utils/test_selectandcastcolumns.py
```

### Comparing `spetlr-1.1.89/LICENSE` & `spetlr-1.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/PKG-INFO` & `spetlr-1.1.94/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: spetlr
-Version: 1.1.89
-Summary: A python SPark ETL libRary (SPETLR) for Databricks.
-Home-page: https://github.com/atc-net/atc-dataplatform
+Version: 1.1.94
+Summary: A python ETL libRary (SPETLR) for Databricks powered by Apache SPark.
+Home-page: https://github.com/spetlr-org/spetlr
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr/issues
 Project-URL: Source Code, https://github.com/spetlr-org/spetlr
 Description: # spetlr
-        A python SPark ETL libRary (SPETLR) for Databricks. 
+        A python ETL libRary (SPETLR) for Databricks powered by Apache SPark. 
         
         Visit SPETLR official webpage: [https://spetlr.com/](https://spetlr.com/)
         
         ## Important Notes
         
         This package can not be run or tested without access to pyspark.
         However, installing pyspark as part of our installer gave issues when
```

### Comparing `spetlr-1.1.89/README.md` & `spetlr-1.1.94/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # spetlr
-A python SPark ETL libRary (SPETLR) for Databricks. 
+A python ETL libRary (SPETLR) for Databricks powered by Apache SPark. 
 
 Visit SPETLR official webpage: [https://spetlr.com/](https://spetlr.com/)
 
 ## Important Notes
 
 This package can not be run or tested without access to pyspark.
 However, installing pyspark as part of our installer gave issues when
```

### Comparing `spetlr-1.1.89/setup.cfg` & `spetlr-1.1.94/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = spetlr
 author = Spetlr.Org
 version = file: src/VERSION.txt
-description = A python SPark ETL libRary (SPETLR) for Databricks.
+description = A python ETL libRary (SPETLR) for Databricks powered by Apache SPark.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author_email = spetlr.org@gmail.com
-url = https://github.com/atc-net/atc-dataplatform
+url = https://github.com/spetlr-org/spetlr
 keywords = databricks, pyspark
 license_files = LICENSE
 project_urls = 
 	Documentation = https://github.com/spetlr-org/spetlr
 	Bug Reports = https://github.com/spetlr-org/spetlr/issues
 	Source Code = https://github.com/spetlr-org/spetlr
 classifiers = 
@@ -36,14 +36,15 @@
 	Deprecated
 	pyodbc
 	databricks-api
 	importlib-metadata
 	azure-cosmos
 	timezonefinder==6.0.2
 	more_itertools
+	pycountry
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	python3 = spetlr.alias:python3
```

### Comparing `spetlr-1.1.89/src/spetlr/cache/CachedLoader.py` & `spetlr-1.1.94/src/spetlr/cache/CachedLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/cache/CachedLoaderParameters.py` & `spetlr-1.1.94/src/spetlr/cache/CachedLoaderParameters.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/configurator/_cli/__init__.py` & `spetlr-1.1.94/src/spetlr/configurator/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/configurator/_cli/generate_keys_file.py` & `spetlr-1.1.94/src/spetlr/configurator/_cli/generate_keys_file.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/configurator/configurator.py` & `spetlr-1.1.94/src/spetlr/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/configurator/sql/StatementBlocks.py` & `spetlr-1.1.94/src/spetlr/configurator/sql/StatementBlocks.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/configurator/sql/comments.py` & `spetlr-1.1.94/src/spetlr/configurator/sql/comments.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 from typing import Dict, List
 
+import sqlparse
 import yaml
-
-from . import sqlparse
-from .sqlparse.sql import Statement
+from sqlparse.sql import Statement
 
 _magic_comment_start = "-- spetlr.configurator "
 
 
 def _extract_comment_attributes(stmt: Statement) -> Dict:
     _magic_comment_start_re = re.compile(_magic_comment_start, re.IGNORECASE)
     collected_lines = []
```

### Comparing `spetlr-1.1.89/src/spetlr/configurator/sql/create.py` & `spetlr-1.1.94/src/spetlr/configurator/sql/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict
 
+import sqlparse
 from more_itertools import peekable
 
-from spetlr.configurator.sql import sqlparse
 from spetlr.configurator.sql.db import _walk_db_statement
 from spetlr.configurator.sql.table import _walk_table_statement
 from spetlr.configurator.sql.utils import _meaningful_token_iter
 
 
 def _walk_create_statement(statement: sqlparse.sql.Statement) -> Dict:
     # create an iterator over all tokens in the statement
```

### Comparing `spetlr-1.1.89/src/spetlr/configurator/sql/db.py` & `spetlr-1.1.94/src/spetlr/configurator/sql/db.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/configurator/sql/init_sqlparse.py` & `spetlr-1.1.94/src/spetlr/configurator/sql/init_sqlparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
-from .sqlparse import engine, keywords, tokens
-from .sqlparse.engine import grouping
-from .sqlparse.lexer import Lexer
-from .sqlparse.sql import Statement
+from sqlparse import engine, keywords, tokens
+from sqlparse.engine import grouping
+from sqlparse.lexer import Lexer
+from sqlparse.sql import Statement
 
 lex = Lexer.get_default_instance()
 my_regex = [
     (r"IF\s+NOT\s+EXISTS\b", tokens.Keyword),
     (r"ZORDER\s+BY\b", tokens.Keyword),
     (r"PARTITIONED\s+BY\b", tokens.Keyword),
     (r"SORTED\s+BY\b", tokens.Keyword),
```

### Comparing `spetlr-1.1.89/src/spetlr/configurator/sql/parse_sql.py` & `spetlr-1.1.94/src/spetlr/configurator/sql/parse_sql.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/configurator/sql/substructures.py` & `spetlr-1.1.94/src/spetlr/configurator/sql/substructures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Generator, List, Tuple
 
+import sqlparse
+
 from spetlr.exceptions.configurator_exceptions import (
     SpetlrConfiguratorInvalidSqlException,
 )
 
-from . import sqlparse
 from .StatementBlocks import ENUM_DESC, SortingCol
 from .types import _PeekableTokenList
 from .utils import _meaningful_token_iter
 
 
 def _unpack_comma_separated_list_in_parens(
     stmt: _PeekableTokenList,
```

### Comparing `spetlr-1.1.89/src/spetlr/configurator/sql/table.py` & `spetlr-1.1.94/src/spetlr/configurator/sql/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
 from typing import Dict
 
+import sqlparse
+
 from spetlr.exceptions.configurator_exceptions import (
     SpetlrConfiguratorInvalidSqlException,
 )
 
-from . import sqlparse
 from .exceptions import _UnpackAttemptFailed
 from .StatementBlocks import ClusteredBy, StatementBlocks
 from .substructures import (
     _unpack_list_of_single_variables,
     _unpack_list_of_sorting_statements,
     _unpack_options,
 )
```

### Comparing `spetlr-1.1.89/src/spetlr/cosmos/cosmos.py` & `spetlr-1.1.94/src/spetlr/cosmos/cosmos.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/cosmos/cosmos_base_server.py` & `spetlr-1.1.94/src/spetlr/cosmos/cosmos_base_server.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/cosmos/cosmos_handle.py` & `spetlr-1.1.94/src/spetlr/cosmos/cosmos_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/db_auto.py` & `spetlr-1.1.94/src/spetlr/db_auto.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/delta/db_handle.py` & `spetlr-1.1.94/src/spetlr/delta/db_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/delta/delta_handle.py` & `spetlr-1.1.94/src/spetlr/delta/delta_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/eh/EventHubCapture.py` & `spetlr-1.1.94/src/spetlr/eh/EventHubCapture.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/eh/EventHubCaptureExtractor.py` & `spetlr-1.1.94/src/spetlr/eh/EventHubCaptureExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/eh/EventHubJsonPublisher.py` & `spetlr-1.1.94/src/spetlr/eh/EventHubJsonPublisher.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/eh/EventHubStream.py` & `spetlr-1.1.94/src/spetlr/eh/EventHubStream.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/eh/PartitionSpec.py` & `spetlr-1.1.94/src/spetlr/eh/PartitionSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/entry_points/generalized_task_entry_point.py` & `spetlr-1.1.94/src/spetlr/entry_points/generalized_task_entry_point.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/entry_points/task_entry_point.py` & `spetlr-1.1.94/src/spetlr/entry_points/task_entry_point.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/etl/extractor.py` & `spetlr-1.1.94/src/spetlr/etl/extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/etl/extractors/incremental_extractor.py` & `spetlr-1.1.94/src/spetlr/etl/extractors/incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/etl/extractors/schema_extractor.py` & `spetlr-1.1.94/src/spetlr/etl/extractors/schema_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/etl/loader.py` & `spetlr-1.1.94/src/spetlr/etl/loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/etl/loaders/DeleteDataLoader.py` & `spetlr-1.1.94/src/spetlr/etl/loaders/DeleteDataLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/etl/loaders/UpsertLoader.py` & `spetlr-1.1.94/src/spetlr/etl/loaders/UpsertLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/etl/loaders/simple_loader.py` & `spetlr-1.1.94/src/spetlr/etl/loaders/simple_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/etl/orchestrator.py` & `spetlr-1.1.94/src/spetlr/etl/orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/etl/transformer.py` & `spetlr-1.1.94/src/spetlr/etl/transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/etl/transformer_nc.py` & `spetlr-1.1.94/src/spetlr/etl/transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/exceptions/__init__.py` & `spetlr-1.1.94/src/spetlr/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/extractors/eventhub_stream_extractor.py` & `spetlr-1.1.94/src/spetlr/extractors/eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/formatting/git_hooks.py` & `spetlr-1.1.94/src/spetlr/formatting/git_hooks.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/functions.py` & `spetlr-1.1.94/src/spetlr/functions.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/mount/main.py` & `spetlr-1.1.94/src/spetlr/mount/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py` & `spetlr-1.1.94/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py` & `spetlr-1.1.94/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py` & `spetlr-1.1.94/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py` & `spetlr-1.1.94/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py` & `spetlr-1.1.94/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py` & `spetlr-1.1.94/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/reporting/JobReflection.py` & `spetlr-1.1.94/src/spetlr/reporting/JobReflection.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/reporting/SlackNotifier.py` & `spetlr-1.1.94/src/spetlr/reporting/SlackNotifier.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/schema_manager/schema_manager.py` & `spetlr-1.1.94/src/spetlr/schema_manager/schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/schema_manager/spark_schema.py` & `spetlr-1.1.94/src/spetlr/schema_manager/spark_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/spark.py` & `spetlr-1.1.94/src/spetlr/spark.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/sql/CommonBaseServer.py` & `spetlr-1.1.94/src/spetlr/sql/CommonBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/sql/SqlBaseServer.py` & `spetlr-1.1.94/src/spetlr/sql/SqlBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/sql/SqlExecutor.py` & `spetlr-1.1.94/src/spetlr/sql/SqlExecutor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import itertools
 import re
 from importlib import resources as ir
 from pathlib import Path
 from types import ModuleType
 from typing import Dict, List, Optional, Union
 
+import sqlparse
+
 from spetlr.configurator.configurator import Configurator
-from spetlr.configurator.sql import sqlparse
 from spetlr.configurator.sql.init_sqlparse import parse
 from spetlr.schema_manager import SchemaManager
 from spetlr.spark import Spark
 from spetlr.sql import BaseExecutor
 
 
 class SqlExecutor:
@@ -61,33 +62,99 @@
         exclude_pattern: str = None,
         replacements: Dict[str, str] = None,
     ):
         """
         NB: This sql parser can be challenged in parsing sql statements
         which do not use semicolon as a query separator only.
         """
+        for conts in self._get_raw_contents(
+            file_pattern=file_pattern, exclude_pattern=exclude_pattern
+        ):
+            for statement in self.chop_and_substitute(conts, replacements=replacements):
+                yield statement
 
-        # prepare arguments:
-        file_pattern = self._wildcard_string_to_regexp(file_pattern)
-        if exclude_pattern is not None:
-            exclude_pattern = self._wildcard_string_to_regexp(exclude_pattern)
+    def chop_and_substitute(
+        self,
+        raw_sql: str,
+        replacements: Dict[str, str] = None,
+    ):
+        """given the raw contents of a sql file, break it down into statements
+        and execute all substitutions."""
         if replacements is None:
             replacements = {}
 
         # prepare the full set of replacements
         schema_replacements = {
             f"{k}_schema": v
             for k, v in SchemaManager().get_all_spark_sql_schemas().items()
         }
         replacements = {
             **(Configurator().get_all_details()),
             **schema_replacements,
             **replacements,
         }
 
+        sql_code = raw_sql.format(**replacements)
+
+        if self.statement_spliter is None:
+            code_parts = [sql_code]
+        elif ";" not in self.statement_spliter:
+            code_parts = [sql_code]
+            for sequence in self.statement_spliter:
+                code_parts = itertools.chain.from_iterable(
+                    part.split(sequence) for part in code_parts
+                )
+
+        else:
+            # if ; is included split the file into sql statements
+            # by using parse, we ensure not to split by escaped or commented
+            # occurrences of ;
+
+            for marker in self.statement_spliter:
+                if marker != ";":
+                    sql_code = sql_code.replace(marker, ";")
+
+            code_parts = [
+                "".join(token.value for token in statement)
+                for statement in parse(sql_code)
+            ]
+
+        for full_statement in code_parts:
+            cleaned_statement = (
+                (
+                    "".join(
+                        token.value
+                        for statement in parse(full_statement)
+                        for token in statement
+                        if token.ttype not in sqlparse.tokens.Comment
+                    )
+                )
+                .strip()
+                .strip(";")
+            )
+
+            # skip the statement unless it actually contains code.
+            # spark.sql complains if you only give it comments
+            if cleaned_statement:
+                yield full_statement
+
+    def _get_raw_contents(
+        self,
+        file_pattern: str,
+        exclude_pattern: str = None,
+    ):
+        """Return the raw file contents to be parsed on to replacement parsing,
+        based on the searched module, filepattern and exclude_pattern.
+        Returns a generator of strings."""
+
+        # prepare arguments:
+        file_pattern = self._wildcard_string_to_regexp(file_pattern)
+        if exclude_pattern is not None:
+            exclude_pattern = self._wildcard_string_to_regexp(exclude_pattern)
+
         # loop the module contents and find matching files
         for file_name in ir.contents(self.base_module):
             extension = Path(file_name).suffix
             if extension not in [".sql"]:
                 continue
 
             if not re.match(file_pattern, Path(file_name).stem):
@@ -96,62 +163,18 @@
             if exclude_pattern is not None and re.search(
                 exclude_pattern, Path(file_name).stem
             ):
                 continue
 
             with ir.path(self.base_module, file_name) as file_path:
                 with open(file_path) as file:
-                    conts = file.read()
-                    sql_code = conts.format(**replacements)
-
-                    if self.statement_spliter is None:
-                        code_parts = [sql_code]
-                    elif ";" not in self.statement_spliter:
-                        code_parts = [sql_code]
-                        for sequence in self.statement_spliter:
-                            code_parts = itertools.chain.from_iterable(
-                                part.split(sequence) for part in code_parts
-                            )
-
-                    else:
-                        # if ; is included split the file into sql statements
-                        # by using parse, we ensure not to split by escaped or commented
-                        # occurrences of ;
-
-                        for marker in self.statement_spliter:
-                            if marker != ";":
-                                sql_code = sql_code.replace(marker, ";")
-
-                        code_parts = [
-                            "".join(token.value for token in statement)
-                            for statement in parse(sql_code)
-                        ]
-
-                    for full_statement in code_parts:
-                        cleaned_statement = (
-                            (
-                                "".join(
-                                    token.value
-                                    for statement in parse(full_statement)
-                                    for token in statement
-                                    if token.ttype not in sqlparse.tokens.Comment
-                                )
-                            )
-                            .strip()
-                            .strip(";")
-                        )
-
-                        # skip the statement unless it actually contains code.
-                        # spark.sql complains if you only give it comments
-                        if cleaned_statement:
-                            yield full_statement
+                    yield file.read()
 
     def execute_sql_file(self, file_pattern: str, exclude_pattern: str = None):
         """
         NB: This sql parser can be challenged in parsing sql statements
         which do not use semicolon as a query separator only.
         """
 
         executor = self.server or Spark.get()
-
         for statement in self.get_statements(file_pattern, exclude_pattern):
             executor.sql(statement)
```

### Comparing `spetlr-1.1.89/src/spetlr/sql/SqlServer.py` & `spetlr-1.1.94/src/spetlr/sql/SqlServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/sql/sql_handle.py` & `spetlr-1.1.94/src/spetlr/sql/sql_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/tables/TableHandle.py` & `spetlr-1.1.94/src/spetlr/tables/TableHandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformations.py` & `spetlr-1.1.94/src/spetlr/transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformers/__init__.py` & `spetlr-1.1.94/src/spetlr/transformers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from .country_to_alphacode_transformer_nc import (  # noqa: F401
+    CountryToAlphaCodeTransformerNC,
+)
 from .drop_oldest_duplicate_transformer import (  # noqa: F401
     DropOldestDuplicatesTransformer,
 )
 from .dropColumnsTransformer_nc import DropColumnsTransformerNC  # noqa: F401
 from .join_dataframes_transformer import JoinDataframesTransformerNC  # noqa: F401
 from .select_and_cast_columns_transformer_nc import (  # noqa: F401
     SelectAndCastColumnsTransformerNC,
```

### Comparing `spetlr-1.1.89/src/spetlr/transformers/dropColumnsTransformer_nc.py` & `spetlr-1.1.94/src/spetlr/transformers/dropColumnsTransformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformers/drop_oldest_duplicate_transformer.py` & `spetlr-1.1.94/src/spetlr/transformers/drop_oldest_duplicate_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformers/fuzzy_select.py` & `spetlr-1.1.94/src/spetlr/transformers/fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformers/join_dataframes_transformer.py` & `spetlr-1.1.94/src/spetlr/transformers/join_dataframes_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformers/selectColumnsTransformer_nc.py` & `spetlr-1.1.94/src/spetlr/transformers/selectColumnsTransformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py` & `spetlr-1.1.94/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformers/simple_dataframe_filter_transformer.py` & `spetlr-1.1.94/src/spetlr/transformers/simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py` & `spetlr-1.1.94/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformers/simple_sql_transformer.py` & `spetlr-1.1.94/src/spetlr/transformers/simple_sql_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformers/timezone_transformer_nc.py` & `spetlr-1.1.94/src/spetlr/transformers/timezone_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformers/union_transformer.py` & `spetlr-1.1.94/src/spetlr/transformers/union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformers/union_transformer_nc.py` & `spetlr-1.1.94/src/spetlr/transformers/union_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/transformers/validfromto_transformer.py` & `spetlr-1.1.94/src/spetlr/transformers/validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/utils/CheckDfMerge.py` & `spetlr-1.1.94/src/spetlr/utils/CheckDfMerge.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/utils/CleanupTestDatabases.py` & `spetlr-1.1.94/src/spetlr/utils/CleanupTestDatabases.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/utils/DataframeCreator.py` & `spetlr-1.1.94/src/spetlr/utils/DataframeCreator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/utils/DropOldestDuplicates.py` & `spetlr-1.1.94/src/spetlr/utils/DropOldestDuplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/utils/GetMergeStatement.py` & `spetlr-1.1.94/src/spetlr/utils/GetMergeStatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/utils/MockLoader.py` & `spetlr-1.1.94/src/spetlr/utils/MockLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr/utils/SelectAndCastColumns.py` & `spetlr-1.1.94/src/spetlr/utils/SelectAndCastColumns.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/src/spetlr.egg-info/PKG-INFO` & `spetlr-1.1.94/src/spetlr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: spetlr
-Version: 1.1.89
-Summary: A python SPark ETL libRary (SPETLR) for Databricks.
-Home-page: https://github.com/atc-net/atc-dataplatform
+Version: 1.1.94
+Summary: A python ETL libRary (SPETLR) for Databricks powered by Apache SPark.
+Home-page: https://github.com/spetlr-org/spetlr
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr/issues
 Project-URL: Source Code, https://github.com/spetlr-org/spetlr
 Description: # spetlr
-        A python SPark ETL libRary (SPETLR) for Databricks. 
+        A python ETL libRary (SPETLR) for Databricks powered by Apache SPark. 
         
         Visit SPETLR official webpage: [https://spetlr.com/](https://spetlr.com/)
         
         ## Important Notes
         
         This package can not be run or tested without access to pyspark.
         However, installing pyspark as part of our installer gave issues when
```

### Comparing `spetlr-1.1.89/src/spetlr.egg-info/SOURCES.txt` & `spetlr-1.1.94/src/spetlr.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -34,35 +34,14 @@
 src/spetlr/configurator/sql/exceptions.py
 src/spetlr/configurator/sql/init_sqlparse.py
 src/spetlr/configurator/sql/parse_sql.py
 src/spetlr/configurator/sql/substructures.py
 src/spetlr/configurator/sql/table.py
 src/spetlr/configurator/sql/types.py
 src/spetlr/configurator/sql/utils.py
-src/spetlr/configurator/sql/sqlparse/__init__.py
-src/spetlr/configurator/sql/sqlparse/__main__.py
-src/spetlr/configurator/sql/sqlparse/cli.py
-src/spetlr/configurator/sql/sqlparse/exceptions.py
-src/spetlr/configurator/sql/sqlparse/formatter.py
-src/spetlr/configurator/sql/sqlparse/keywords.py
-src/spetlr/configurator/sql/sqlparse/lexer.py
-src/spetlr/configurator/sql/sqlparse/sql.py
-src/spetlr/configurator/sql/sqlparse/tokens.py
-src/spetlr/configurator/sql/sqlparse/utils.py
-src/spetlr/configurator/sql/sqlparse/engine/__init__.py
-src/spetlr/configurator/sql/sqlparse/engine/filter_stack.py
-src/spetlr/configurator/sql/sqlparse/engine/grouping.py
-src/spetlr/configurator/sql/sqlparse/engine/statement_splitter.py
-src/spetlr/configurator/sql/sqlparse/filters/__init__.py
-src/spetlr/configurator/sql/sqlparse/filters/aligned_indent.py
-src/spetlr/configurator/sql/sqlparse/filters/others.py
-src/spetlr/configurator/sql/sqlparse/filters/output.py
-src/spetlr/configurator/sql/sqlparse/filters/reindent.py
-src/spetlr/configurator/sql/sqlparse/filters/right_margin.py
-src/spetlr/configurator/sql/sqlparse/filters/tokens.py
 src/spetlr/cosmos/__init__.py
 src/spetlr/cosmos/cosmos.py
 src/spetlr/cosmos/cosmos_base_server.py
 src/spetlr/cosmos/cosmos_handle.py
 src/spetlr/delta/__init__.py
 src/spetlr/delta/db_handle.py
 src/spetlr/delta/delta_handle.py
@@ -127,14 +106,15 @@
 src/spetlr/sql/SqlServerBaseOptions.py
 src/spetlr/sql/__init__.py
 src/spetlr/sql/sql_handle.py
 src/spetlr/tables/TableHandle.py
 src/spetlr/tables/ThMaker.py
 src/spetlr/tables/__init__.py
 src/spetlr/transformers/__init__.py
+src/spetlr/transformers/country_to_alphacode_transformer_nc.py
 src/spetlr/transformers/dropColumnsTransformer_nc.py
 src/spetlr/transformers/drop_oldest_duplicate_transformer.py
 src/spetlr/transformers/fuzzy_select.py
 src/spetlr/transformers/join_dataframes_transformer.py
 src/spetlr/transformers/selectColumnsTransformer_nc.py
 src/spetlr/transformers/select_and_cast_columns_transformer_nc.py
 src/spetlr/transformers/simple_dataframe_filter_transformer.py
@@ -154,14 +134,15 @@
 src/spetlr/utils/SelectAndCastColumns.py
 src/spetlr/utils/__init__.py
 tests/cluster/cache/test_cache.py
 tests/cluster/cosmos/test_cosmos.py
 tests/cluster/db/test_db_api.py
 tests/cluster/delta/test_cleanup_databases.py
 tests/cluster/delta/test_delta_class.py
+tests/cluster/delta/test_sparkexecutor.py
 tests/cluster/eh/test_eh_json_orchestrator.py
 tests/cluster/eh/test_eh_json_transformer.py
 tests/cluster/eh/test_eh_saving.py
 tests/cluster/etl/test_delete_data_loader.py
 tests/cluster/etl/test_deltaupsert.py
 tests/cluster/etl/test_extractor.py
 tests/cluster/etl/test_incremental_extractor.py
@@ -194,14 +175,15 @@
 tests/local/entry_points/test_task_entry_point.py
 tests/local/etl/test_orchestrator.py
 tests/local/extractors/test_eventhub_stream_extractor.py
 tests/local/reporting/test_slack_reporting.py
 tests/local/schema_manager/test_schema_manager.py
 tests/local/sql/test_SqlExecutor.py
 tests/local/transformers/test_concat_df.py
+tests/local/transformers/test_country_to_alphacode_transformer.py
 tests/local/transformers/test_drop_columns.py
 tests/local/transformers/test_dropoldestduplicates.py
 tests/local/transformers/test_fuzzy_select.py
 tests/local/transformers/test_join_dataframes_transformer.py
 tests/local/transformers/test_select_and_cast_columns_transformer_nc.py
 tests/local/transformers/test_select_columns.py
 tests/local/transformers/test_simple_dataframe_filter_transformer.py
```

### Comparing `spetlr-1.1.89/tests/cluster/cache/test_cache.py` & `spetlr-1.1.94/tests/cluster/cache/test_cache.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/cosmos/test_cosmos.py` & `spetlr-1.1.94/tests/cluster/cosmos/test_cosmos.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/delta/test_cleanup_databases.py` & `spetlr-1.1.94/tests/cluster/delta/test_cleanup_databases.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/delta/test_delta_class.py` & `spetlr-1.1.94/tests/cluster/delta/test_delta_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 from spetlr.etl.loaders import SimpleLoader
 from spetlr.spark import Spark
 
 
 class DeltaTests(unittest.TestCase):
     @classmethod
     def setUpClass(cls) -> None:
-        Configurator().clear_all_configurations()
+        c = Configurator()
+        c.clear_all_configurations()
+        c.set_debug()
 
     def test_01_configure(self):
         tc = Configurator()
         tc.register(
             "MyDb", {"name": "TestDb{ID}", "path": "/mnt/spetlr/silver/testdb{ID}"}
         )
 
@@ -36,25 +38,28 @@
                 "name": "TestDb{ID}.TestTbl2",
             },
         )
 
         tc.register(
             "MyTbl3",
             {
-                "path": "/mnt/spetlr/silver/testdb/testtbl3",
+                "path": "/mnt/spetlr/silver/testdb{ID}/testtbl3",
             },
         )
 
         # test instantiation without error
         DbHandle.from_tc("MyDb")
         DeltaHandle.from_tc("MyTbl")
         DeltaHandle.from_tc("MyTbl2")
 
     def test_02_write(self):
         dh = DeltaHandle.from_tc("MyTbl")
+        dh2 = DeltaHandle.from_tc("MyTbl2")
+        dh.drop_and_delete()
+        dh2.drop_and_delete()
 
         df = Spark.get().createDataFrame([(1, "a"), (2, "b")], "id int, name string")
 
         dh.overwrite(df, mergeSchema=True)
         dh.append(df, mergeSchema=False)  # schema matches
 
         df = Spark.get().createDataFrame(
@@ -66,21 +71,22 @@
             """,
         )
 
         dh.append(df, mergeSchema=True)
 
     def test_03_create(self):
         db = DbHandle.from_tc("MyDb")
+        db.drop_cascade()
         db.create()
 
         dh = DeltaHandle.from_tc("MyTbl")
         dh.create_hive_table()
 
         # test hive access:
-        df = Spark.get().table("TestDb.TestTbl")
+        df = Spark.get().table(dh._name)
         self.assertTrue(6, df.count())
 
     def test_04_read(self):
         df = DeltaHandle.from_tc("MyTbl").read()
         self.assertEqual(6, df.count())
 
     def test_041_schema(self):
```

### Comparing `spetlr-1.1.89/tests/cluster/eh/test_eh_json_orchestrator.py` & `spetlr-1.1.94/tests/cluster/eh/test_eh_json_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/eh/test_eh_json_transformer.py` & `spetlr-1.1.94/tests/cluster/eh/test_eh_json_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/eh/test_eh_saving.py` & `spetlr-1.1.94/tests/cluster/eh/test_eh_saving.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/etl/test_delete_data_loader.py` & `spetlr-1.1.94/tests/cluster/etl/test_delete_data_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/etl/test_deltaupsert.py` & `spetlr-1.1.94/tests/cluster/etl/test_deltaupsert.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/etl/test_extractor.py` & `spetlr-1.1.94/tests/cluster/etl/test_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/etl/test_incremental_extractor.py` & `spetlr-1.1.94/tests/cluster/etl/test_incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/etl/test_loader.py` & `spetlr-1.1.94/tests/cluster/etl/test_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/etl/test_orchestrator_etl_warning.py` & `spetlr-1.1.94/tests/cluster/etl/test_orchestrator_etl_warning.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/etl/test_transformer.py` & `spetlr-1.1.94/tests/cluster/etl/test_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/etl/test_transformer_nc.py` & `spetlr-1.1.94/tests/cluster/etl/test_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/etl/test_upsertloader.py` & `spetlr-1.1.94/tests/cluster/etl/test_upsertloader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/reporting/test_slack_reporting.py` & `spetlr-1.1.94/tests/cluster/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/schema_manager/test_schema_manager.py` & `spetlr-1.1.94/tests/cluster/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/sql/test_deliveryexecutor.py` & `spetlr-1.1.94/tests/cluster/sql/test_deliveryexecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/sql/test_deliverysql.py` & `spetlr-1.1.94/tests/cluster/sql/test_deliverysql.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/sql/test_simple_sql_etl.py` & `spetlr-1.1.94/tests/cluster/sql/test_simple_sql_etl.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/sql/test_sqlhandle.py` & `spetlr-1.1.94/tests/cluster/sql/test_sqlhandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/transformations/test_merge_df_into_target.py` & `spetlr-1.1.94/tests/cluster/transformations/test_merge_df_into_target.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/cluster/transformations/test_union_transformer.py` & `spetlr-1.1.94/tests/cluster/transformations/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/configurator/test_configurator.py` & `spetlr-1.1.94/tests/local/configurator/test_configurator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/configurator/test_configurator_cli.py` & `spetlr-1.1.94/tests/local/configurator/test_configurator_cli.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/eh/test_EventHubCaptureExtractor.py` & `spetlr-1.1.94/tests/local/eh/test_EventHubCaptureExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/eh/test_ehto_bronze_and_silver.py` & `spetlr-1.1.94/tests/local/eh/test_ehto_bronze_and_silver.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/eh/test_ehtodeltabronze_orchestrator.py` & `spetlr-1.1.94/tests/local/eh/test_ehtodeltabronze_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/eh/test_ehtodeltabronze_transformer.py` & `spetlr-1.1.94/tests/local/eh/test_ehtodeltabronze_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/eh/test_ehtodeltasilver_orchestrator.py` & `spetlr-1.1.94/tests/local/eh/test_ehtodeltasilver_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/extractors/test_eventhub_stream_extractor.py` & `spetlr-1.1.94/tests/local/extractors/test_eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/reporting/test_slack_reporting.py` & `spetlr-1.1.94/tests/local/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/schema_manager/test_schema_manager.py` & `spetlr-1.1.94/tests/local/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/sql/test_SqlExecutor.py` & `spetlr-1.1.94/tests/local/sql/test_SqlExecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/test_functions.py` & `spetlr-1.1.94/tests/local/test_functions.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/test_get_schema.py` & `spetlr-1.1.94/tests/local/test_get_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/test_sqlServer.py` & `spetlr-1.1.94/tests/local/test_sqlServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/test_transformations.py` & `spetlr-1.1.94/tests/local/test_transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/transformers/test_concat_df.py` & `spetlr-1.1.94/tests/local/transformers/test_concat_df.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/transformers/test_drop_columns.py` & `spetlr-1.1.94/tests/local/transformers/test_drop_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/transformers/test_dropoldestduplicates.py` & `spetlr-1.1.94/tests/local/transformers/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/transformers/test_fuzzy_select.py` & `spetlr-1.1.94/tests/local/transformers/test_fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/transformers/test_join_dataframes_transformer.py` & `spetlr-1.1.94/tests/local/transformers/test_join_dataframes_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py` & `spetlr-1.1.94/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/transformers/test_select_columns.py` & `spetlr-1.1.94/tests/local/transformers/test_select_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/transformers/test_simple_dataframe_filter_transformer.py` & `spetlr-1.1.94/tests/local/transformers/test_simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py` & `spetlr-1.1.94/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/transformers/test_timezone_transformer_nc.py` & `spetlr-1.1.94/tests/local/transformers/test_timezone_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/transformers/test_union_transformer.py` & `spetlr-1.1.94/tests/local/transformers/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/transformers/test_union_transformer_nc.py` & `spetlr-1.1.94/tests/local/transformers/test_union_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/transformers/test_validfromto_transformer.py` & `spetlr-1.1.94/tests/local/transformers/test_validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/utils/test_dataframe_creation.py` & `spetlr-1.1.94/tests/local/utils/test_dataframe_creation.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/utils/test_dropoldestduplicates.py` & `spetlr-1.1.94/tests/local/utils/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/utils/test_getmergestatement.py` & `spetlr-1.1.94/tests/local/utils/test_getmergestatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/utils/test_mock_etl.py` & `spetlr-1.1.94/tests/local/utils/test_mock_etl.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.89/tests/local/utils/test_selectandcastcolumns.py` & `spetlr-1.1.94/tests/local/utils/test_selectandcastcolumns.py`

 * *Files identical despite different names*

