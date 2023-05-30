# Comparing `tmp/cognite_neat-0.12.2.tar.gz` & `tmp/cognite_neat-0.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.12.2.tar", max compression
+gzip compressed data, was "cognite_neat-0.12.3.tar", max compression
```

## Comparing `cognite_neat-0.12.2.tar` & `cognite_neat-0.12.3.tar`

### file list

```diff
@@ -1,82 +1,86 @@
--rw-r--r--   0        0        0    11351 2023-05-30 07:13:02.547906 cognite_neat-0.12.2/LICENSE
--rw-r--r--   0        0        0     8765 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/README.md
--rw-r--r--   0        0        0       23 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/__init__.py
--rw-r--r--   0        0        0      616 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2652 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/app.py
--rw-r--r--   0        0        0     1344 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0      408 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_classes/__init__.py
--rw-r--r--   0        0        0     4775 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_classes/config.py
--rw-r--r--   0        0        0     8132 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_classes/rules.py
--rw-r--r--   0        0        0    28433 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_classes/transformation_rules.py
--rw-r--r--   0        0        0        0 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      470 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     2250 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/extractors/labels.py
--rw-r--r--   0        0        0    35280 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/extractors/rdf_to_assets.py
--rw-r--r--   0        0        0    17870 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/extractors/rdf_to_relationships.py
--rw-r--r--   0        0        0     6700 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/extractors/rules_to_graphql.py
--rw-r--r--   0        0        0      115 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0    10647 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0      913 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/loader/rules.py
--rw-r--r--   0        0        0        0 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    12025 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0    15303 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/modeler.py
--rw-r--r--   0        0        0      110 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/parser/__init__.py
--rw-r--r--   0        0        0     1727 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/parser/transformation_rules.py
--rw-r--r--   0        0        0       73 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9595 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0    10943 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0     4524 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/utils.py
--rw-r--r--   0        0        0     2558 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      311 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    18503 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17764 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0     6200 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     3398 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      781 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     6648 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0    79580 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    52178 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1461 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15632 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0    16382 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/fast_graph/workflow.py
--rw-r--r--   0        0        0     8068 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/fast_graph/workflow.yaml
--rw-r--r--   0        0        0    11477 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0    13115 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6025 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0        0 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1013 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    19784 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4003 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1357930 2023-05-30 07:13:02.563906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js
--rw-r--r--   0        0        0     2667 2023-05-30 07:13:02.563906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.LICENSE.txt
--rw-r--r--   0        0        0  5848771 2023-05-30 07:13:02.591906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.map
--rw-r--r--   0        0        0     2633 2023-05-30 07:13:02.591906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/main.py
--rw-r--r--   0        0        0        0 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/migration/wf_manifests.py
--rw-r--r--   0        0        0     2471 2023-05-30 07:13:02.939909 cognite_neat-0.12.2/pyproject.toml
--rw-r--r--   0        0        0    10241 1970-01-01 00:00:00.000000 cognite_neat-0.12.2/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/LICENSE
+-rw-r--r--   0        0        0     8765 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/README.md
+-rw-r--r--   0        0        0       23 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/__init__.py
+-rw-r--r--   0        0        0      771 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2652 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     1344 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0      408 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/data_classes/__init__.py
+-rw-r--r--   0        0        0     4775 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/data_classes/config.py
+-rw-r--r--   0        0        0     8132 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/data_classes/rules.py
+-rw-r--r--   0        0        0    29278 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/data_classes/transformation_rules.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     1520 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0      642 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0     5028 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/extractors/graph_sheet_to_graph.py
+-rw-r--r--   0        0        0     2250 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/extractors/labels.py
+-rw-r--r--   0        0        0    35280 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/extractors/rdf_to_assets.py
+-rw-r--r--   0        0        0    17870 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/extractors/rdf_to_relationships.py
+-rw-r--r--   0        0        0     5302 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
+-rw-r--r--   0        0        0     6700 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/extractors/rules_to_graphql.py
+-rw-r--r--   0        0        0      138 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0      938 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/loader/graph_capturing_sheet.py
+-rw-r--r--   0        0        0    10647 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0      913 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/loader/rules.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    12025 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0    15303 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/modeler.py
+-rw-r--r--   0        0        0      110 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/parser/__init__.py
+-rw-r--r--   0        0        0     1727 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/parser/transformation_rules.py
+-rw-r--r--   0        0        0       73 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9595 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0    10943 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0     4524 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/utils.py
+-rw-r--r--   0        0        0     2558 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      311 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    18503 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17764 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0     6200 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     3398 2023-05-30 10:48:48.175666 cognite_neat-0.12.3/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0      781 2023-05-30 10:48:48.179666 cognite_neat-0.12.3/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     6648 2023-05-30 10:48:48.179666 cognite_neat-0.12.3/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-05-30 10:48:48.179666 cognite_neat-0.12.3/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0    94607 2023-05-30 10:48:48.179666 cognite_neat-0.12.3/cognite/neat/examples/graph_capturing_sheets/sheet2cdf-graph-capturing.xlsx
+-rw-r--r--   0        0        0    79580 2023-05-30 10:48:48.179666 cognite_neat-0.12.3/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    52178 2023-05-30 10:48:48.179666 cognite_neat-0.12.3/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1461 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15632 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0    16382 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/examples/workflows/fast_graph/workflow.py
+-rw-r--r--   0        0        0     8068 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/examples/workflows/fast_graph/workflow.yaml
+-rw-r--r--   0        0        0    11477 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0    13115 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6025 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-05-30 10:48:48.227666 cognite_neat-0.12.3/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:48:48.227666 cognite_neat-0.12.3/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1013 2023-05-30 10:48:48.227666 cognite_neat-0.12.3/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    19784 2023-05-30 10:48:48.227666 cognite_neat-0.12.3/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:48:48.227666 cognite_neat-0.12.3/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-05-30 10:48:48.227666 cognite_neat-0.12.3/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4003 2023-05-30 10:48:48.227666 cognite_neat-0.12.3/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-05-30 10:48:48.183667 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1357930 2023-05-30 10:48:48.191666 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js
+-rw-r--r--   0        0        0     2667 2023-05-30 10:48:48.195666 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.LICENSE.txt
+-rw-r--r--   0        0        0  5848771 2023-05-30 10:48:48.223666 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.map
+-rw-r--r--   0        0        0     2633 2023-05-30 10:48:48.223666 cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-05-30 10:48:48.227666 cognite_neat-0.12.3/cognite/neat/main.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:48:48.227666 cognite_neat-0.12.3/cognite/neat/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-05-30 10:48:48.227666 cognite_neat-0.12.3/cognite/neat/migration/wf_manifests.py
+-rw-r--r--   0        0        0     2471 2023-05-30 10:48:48.635663 cognite_neat-0.12.3/pyproject.toml
+-rw-r--r--   0        0        0    10241 1970-01-01 00:00:00.000000 cognite_neat-0.12.3/PKG-INFO
```

### Comparing `cognite_neat-0.12.2/LICENSE` & `cognite_neat-0.12.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/README.md` & `cognite_neat-0.12.3/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/constants.py` & `cognite_neat-0.12.3/cognite/neat/constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,12 +3,14 @@
 from cognite import neat
 
 PACKAGE_DIRECTORY = Path(neat.__file__).parent
 EXAMPLES_DIRECTORY = PACKAGE_DIRECTORY / "examples"
 EXAMPLE_RULES = EXAMPLES_DIRECTORY / "rules"
 EXAMPLE_SOURCE_GRAPHS = EXAMPLES_DIRECTORY / "source_graphs"
 EXAMPLE_WORKFLOWS = EXAMPLES_DIRECTORY / "workflows"
+EXAMPLE_GRAPH_CAPTURING = EXAMPLES_DIRECTORY / "graph_capturing_sheets"
 
 TNT_TRANSFORMATION_RULES = EXAMPLE_RULES / "Rules-Nordic44-to-TNT.xlsx"
 SIMPLE_TRANSFORMATION_RULES = EXAMPLE_RULES / "sheet2cdf-transformation-rules.xlsx"
 NORDIC44_KNOWLEDGE_GRAPH = EXAMPLE_SOURCE_GRAPHS / "Knowledge-Graph-Nordic44.xml"
+GRAPH_CAPTURING_SHEET = EXAMPLE_GRAPH_CAPTURING / "sheet2cdf-graph-capturing.xlsx"
 UI_PATH = PACKAGE_DIRECTORY / "explorer-ui" / "neat-app" / "build"
```

### Comparing `cognite_neat-0.12.2/cognite/neat/core/app.py` & `cognite_neat-0.12.3/cognite/neat/core/app.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/configuration.py` & `cognite_neat-0.12.3/cognite/neat/core/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/data_classes/config.py` & `cognite_neat-0.12.3/cognite/neat/core/data_classes/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/data_classes/rules.py` & `cognite_neat-0.12.3/cognite/neat/core/data_classes/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/data_classes/transformation_rules.py` & `cognite_neat-0.12.3/cognite/neat/core/data_classes/transformation_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,28 +406,46 @@
 
         return class_labels.union(relationship_labels).union(property_labels)
 
     def get_defined_classes(self) -> set[str]:
         """Returns classes that have been defined in the data model."""
         return {property.class_name for property in self.properties.values()}
 
-    def get_classes_with_properties(self) -> dict[str, Property]:
+    def get_classes_with_properties(self) -> dict[str, list[Property]]:
         """Returns classes that have been defined in the data model."""
         # TODO: Do not particularly like method name, find something more suitable
         class_property_pairs = {}
 
         for property_ in self.properties.values():
             class_ = property_.class_name
             if class_ in class_property_pairs:
                 class_property_pairs[class_] += [property_]
             else:
                 class_property_pairs[class_] = [property_]
 
         return class_property_pairs
 
+    def get_class_property_pairs(self) -> dict[str, dict[str, Property]]:
+        """This method will actually consider only the first definition of given property!"""
+        class_property_pairs = {}
+
+        for class_, properties in self.get_classes_with_properties().items():
+            processed_properties = {}
+            for property_ in properties:
+                if property_.property_name in processed_properties:
+                    warnings.warn(
+                        "Property has been defined more than once! Only first definition will be considered.",
+                        stacklevel=2,
+                    )
+                    continue
+                processed_properties[property_.property_name] = property_
+            class_property_pairs[class_] = processed_properties
+
+        return class_property_pairs
+
     def check_data_model_definitions(self):
         """Check if data model definitions are valid."""
         issues = set()
         for class_, properties in self.get_classes_with_properties().items():
             analyzed_properties = []
             for property in properties:
                 if property.property_name not in analyzed_properties:
```

### Comparing `cognite_neat-0.12.2/cognite/neat/core/data_stores/metrics.py` & `cognite_neat-0.12.3/cognite/neat/core/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.12.3/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/extractors/labels.py` & `cognite_neat-0.12.3/cognite/neat/core/extractors/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/extractors/rdf_to_assets.py` & `cognite_neat-0.12.3/cognite/neat/core/extractors/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/extractors/rdf_to_relationships.py` & `cognite_neat-0.12.3/cognite/neat/core/extractors/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/extractors/rules_to_graphql.py` & `cognite_neat-0.12.3/cognite/neat/core/extractors/rules_to_graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/loader/config.py` & `cognite_neat-0.12.3/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/loader/graph.py` & `cognite_neat-0.12.3/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.12.3/cognite/neat/core/loader/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/loader/rules.py` & `cognite_neat-0.12.3/cognite/neat/core/loader/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.12.3/cognite/neat/core/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/modeler.py` & `cognite_neat-0.12.3/cognite/neat/core/modeler.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/parser/transformation_rules.py` & `cognite_neat-0.12.3/cognite/neat/core/parser/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.12.3/cognite/neat/core/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/transformer.py` & `cognite_neat-0.12.3/cognite/neat/core/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/utils.py` & `cognite_neat-0.12.3/cognite/neat/core/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/validator.py` & `cognite_neat-0.12.3/cognite/neat/core/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/workflow/base.py` & `cognite_neat-0.12.3/cognite/neat/core/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.12.3/cognite/neat/core/workflow/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.12.3/cognite/neat/core/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/workflow/model.py` & `cognite_neat-0.12.3/cognite/neat/core/workflow/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.12.3/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.12.3/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.12.3/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.12.3/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.12.3/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.12.3/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.12.3/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.12.3/cognite/neat/examples/workflows/default/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.12.3/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/examples/workflows/fast_graph/workflow.py` & `cognite_neat-0.12.3/cognite/neat/examples/workflows/fast_graph/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/examples/workflows/fast_graph/workflow.yaml` & `cognite_neat-0.12.3/cognite/neat/examples/workflows/fast_graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.12.3/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.12.3/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/examples/workflows/sheet2cdf/workflow.py` & `cognite_neat-0.12.3/cognite/neat/examples/workflows/sheet2cdf/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.12.3/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.12.3/cognite/neat/explorer/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/explorer/explorer.py` & `cognite_neat-0.12.3/cognite/neat/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.12.3/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js` & `cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.LICENSE.txt` & `cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.map` & `cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.12.3/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/cognite/neat/migration/wf_manifests.py` & `cognite_neat-0.12.3/cognite/neat/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.2/pyproject.toml` & `cognite_neat-0.12.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.12.2"
+version = "0.12.3"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 packages = [
```

### Comparing `cognite_neat-0.12.2/PKG-INFO` & `cognite_neat-0.12.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.12.2
+Version: 0.12.3
 Summary: Knowledge graph transformation
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

