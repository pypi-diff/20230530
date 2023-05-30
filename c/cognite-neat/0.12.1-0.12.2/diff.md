# Comparing `tmp/cognite_neat-0.12.1.tar.gz` & `tmp/cognite_neat-0.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.12.1.tar", max compression
+gzip compressed data, was "cognite_neat-0.12.2.tar", max compression
```

## Comparing `cognite_neat-0.12.1.tar` & `cognite_neat-0.12.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0    11351 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/LICENSE
--rw-r--r--   0        0        0     8765 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/README.md
--rw-r--r--   0        0        0       23 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/__init__.py
--rw-r--r--   0        0        0      616 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2652 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/app.py
--rw-r--r--   0        0        0     1344 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0      408 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_classes/__init__.py
--rw-r--r--   0        0        0     4670 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_classes/config.py
--rw-r--r--   0        0        0     8132 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_classes/rules.py
--rw-r--r--   0        0        0    28433 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_classes/transformation_rules.py
--rw-r--r--   0        0        0        0 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      470 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     2250 2023-05-26 15:36:21.995277 cognite_neat-0.12.1/cognite/neat/core/extractors/labels.py
--rw-r--r--   0        0        0    35280 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/extractors/rdf_to_assets.py
--rw-r--r--   0        0        0    17870 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/extractors/rdf_to_relationships.py
--rw-r--r--   0        0        0     6700 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/extractors/rules_to_graphql.py
--rw-r--r--   0        0        0      115 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0    10647 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0      913 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/loader/rules.py
--rw-r--r--   0        0        0        0 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    12025 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0    15303 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/modeler.py
--rw-r--r--   0        0        0      110 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/parser/__init__.py
--rw-r--r--   0        0        0     1727 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/parser/transformation_rules.py
--rw-r--r--   0        0        0       73 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9595 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0    10943 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0     4524 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/utils.py
--rw-r--r--   0        0        0     2558 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      311 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    18503 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17764 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0     6200 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     3398 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      781 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     6648 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0    79580 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    52178 2023-05-26 15:36:21.999277 cognite_neat-0.12.1/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-05-26 15:36:22.003277 cognite_neat-0.12.1/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1461 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15601 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0    16351 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/fast_graph/workflow.py
--rw-r--r--   0        0        0     8068 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/fast_graph/workflow.yaml
--rw-r--r--   0        0        0    11477 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0    13084 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6025 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0        0 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1013 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    19784 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4003 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-05-26 15:36:22.007277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1357930 2023-05-26 15:36:22.015277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js
--rw-r--r--   0        0        0     2667 2023-05-26 15:36:22.015277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.LICENSE.txt
--rw-r--r--   0        0        0  5848771 2023-05-26 15:36:22.051277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.map
--rw-r--r--   0        0        0     2633 2023-05-26 15:36:22.051277 cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/main.py
--rw-r--r--   0        0        0        0 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-05-26 15:36:22.059277 cognite_neat-0.12.1/cognite/neat/migration/wf_manifests.py
--rw-r--r--   0        0        0     2471 2023-05-26 15:36:22.535279 cognite_neat-0.12.1/pyproject.toml
--rw-r--r--   0        0        0    10241 1970-01-01 00:00:00.000000 cognite_neat-0.12.1/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-05-30 07:13:02.547906 cognite_neat-0.12.2/LICENSE
+-rw-r--r--   0        0        0     8765 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/README.md
+-rw-r--r--   0        0        0       23 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/__init__.py
+-rw-r--r--   0        0        0      616 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2652 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     1344 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0      408 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_classes/__init__.py
+-rw-r--r--   0        0        0     4775 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_classes/config.py
+-rw-r--r--   0        0        0     8132 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_classes/rules.py
+-rw-r--r--   0        0        0    28433 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_classes/transformation_rules.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     1520 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0      470 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0     2250 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/extractors/labels.py
+-rw-r--r--   0        0        0    35280 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/extractors/rdf_to_assets.py
+-rw-r--r--   0        0        0    17870 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/extractors/rdf_to_relationships.py
+-rw-r--r--   0        0        0     6700 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/extractors/rules_to_graphql.py
+-rw-r--r--   0        0        0      115 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0    10647 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0      913 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/loader/rules.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    12025 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0    15303 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/modeler.py
+-rw-r--r--   0        0        0      110 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/parser/__init__.py
+-rw-r--r--   0        0        0     1727 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/parser/transformation_rules.py
+-rw-r--r--   0        0        0       73 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9595 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0    10943 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0     4524 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/utils.py
+-rw-r--r--   0        0        0     2558 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      311 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    18503 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17764 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0     6200 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     3398 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0      781 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     6648 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0    79580 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    52178 2023-05-30 07:13:02.551906 cognite_neat-0.12.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1461 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15632 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0    16382 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/fast_graph/workflow.py
+-rw-r--r--   0        0        0     8068 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/fast_graph/workflow.yaml
+-rw-r--r--   0        0        0    11477 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0    13115 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6025 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1013 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    19784 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4003 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-05-30 07:13:02.555906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1357930 2023-05-30 07:13:02.563906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js
+-rw-r--r--   0        0        0     2667 2023-05-30 07:13:02.563906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.LICENSE.txt
+-rw-r--r--   0        0        0  5848771 2023-05-30 07:13:02.591906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.map
+-rw-r--r--   0        0        0     2633 2023-05-30 07:13:02.591906 cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/main.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-05-30 07:13:02.595906 cognite_neat-0.12.2/cognite/neat/migration/wf_manifests.py
+-rw-r--r--   0        0        0     2471 2023-05-30 07:13:02.939909 cognite_neat-0.12.2/pyproject.toml
+-rw-r--r--   0        0        0    10241 1970-01-01 00:00:00.000000 cognite_neat-0.12.2/PKG-INFO
```

### Comparing `cognite_neat-0.12.1/LICENSE` & `cognite_neat-0.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/README.md` & `cognite_neat-0.12.2/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/constants.py` & `cognite_neat-0.12.2/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/app.py` & `cognite_neat-0.12.2/cognite/neat/core/app.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/configuration.py` & `cognite_neat-0.12.2/cognite/neat/core/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/data_classes/config.py` & `cognite_neat-0.12.2/cognite/neat/core/data_classes/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 import os
 from enum import StrEnum
 from pathlib import Path
 from typing import Literal, Self
 
 import yaml
@@ -111,16 +112,19 @@
         return self.data_store_path / "source_graphs"
 
     @classmethod
     def from_yaml(cls, filepath: Path) -> Self:
         return cls(**safe_load(filepath.read_text()))
 
     def to_yaml(self, filepath: Path):
+        # Parse as json to avoid Path and Enum objects
+        dump = json.loads(self.json())
+
         with filepath.open("w") as f:
-            yaml.dump(self.dict(), f)
+            yaml.safe_dump(dump, f)
 
     @classmethod
     def from_env(cls) -> Self:
         cdf_config = ServiceClient(
             project=os.environ.get("NEAT_CDF_PROJECT"),
             client_name=os.environ.get("NEAT_CDF_CLIENT_NAME"),
             client_id=os.environ.get("NEAT_CDF_CLIENT_ID"),
```

### Comparing `cognite_neat-0.12.1/cognite/neat/core/data_classes/rules.py` & `cognite_neat-0.12.2/cognite/neat/core/data_classes/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/data_classes/transformation_rules.py` & `cognite_neat-0.12.2/cognite/neat/core/data_classes/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/data_stores/metrics.py` & `cognite_neat-0.12.2/cognite/neat/core/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.12.2/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/extractors/labels.py` & `cognite_neat-0.12.2/cognite/neat/core/extractors/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/extractors/rdf_to_assets.py` & `cognite_neat-0.12.2/cognite/neat/core/extractors/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/extractors/rdf_to_relationships.py` & `cognite_neat-0.12.2/cognite/neat/core/extractors/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/extractors/rules_to_graphql.py` & `cognite_neat-0.12.2/cognite/neat/core/extractors/rules_to_graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/loader/config.py` & `cognite_neat-0.12.2/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/loader/graph.py` & `cognite_neat-0.12.2/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.12.2/cognite/neat/core/loader/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/loader/rules.py` & `cognite_neat-0.12.2/cognite/neat/core/loader/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.12.2/cognite/neat/core/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/modeler.py` & `cognite_neat-0.12.2/cognite/neat/core/modeler.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/parser/transformation_rules.py` & `cognite_neat-0.12.2/cognite/neat/core/parser/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.12.2/cognite/neat/core/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/transformer.py` & `cognite_neat-0.12.2/cognite/neat/core/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/utils.py` & `cognite_neat-0.12.2/cognite/neat/core/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/validator.py` & `cognite_neat-0.12.2/cognite/neat/core/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/workflow/base.py` & `cognite_neat-0.12.2/cognite/neat/core/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.12.2/cognite/neat/core/workflow/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.12.2/cognite/neat/core/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/workflow/model.py` & `cognite_neat-0.12.2/cognite/neat/core/workflow/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.12.2/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.12.2/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.12.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.12.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.12.2/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.12.2/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.12.2/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.12.2/cognite/neat/examples/workflows/default/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 cdf_store.load_rules_file_from_cdf(rules_file, version)
         else:
             cdf_store.load_rules_file_from_cdf(self.cdf_client, version)
 
         tables = loader.rules.excel_file_to_table_by_name(rules_file_path)
         self.transformation_rules = parser.parse_transformation_rules(tables)
         self.dataset_id = self.transformation_rules.metadata.data_set_id
-        logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules")
+        logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules from {rules_file_path.name!r}.")
         output_text = f"Loaded {len(self.transformation_rules.properties)} rules"
         logging.info(output_text)
         return FlowMessage(output_text=output_text)
 
     def step_configuring_stores(self, flow_msg: FlowMessage = None, clean_start: bool = True):
         # Initialize source and solution graph stores . clean_start=True will delete all artifacts(files , locks , etc) from previous runs
         logging.info("Initializing source graph")
```

### Comparing `cognite_neat-0.12.1/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.12.2/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/examples/workflows/fast_graph/workflow.py` & `cognite_neat-0.12.2/cognite/neat/examples/workflows/fast_graph/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 cdf_store.load_rules_file_from_cdf(rules_file, version)
         else:
             cdf_store.load_rules_file_from_cdf(self.cdf_client, version)
 
         tables = loader.rules.excel_file_to_table_by_name(rules_file_path)
         self.transformation_rules = parser.parse_transformation_rules(tables)
         self.dataset_id = self.transformation_rules.metadata.data_set_id
-        logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules")
+        logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules from {rules_file_path.name!r}.")
         output_text = f"Loaded {len(self.transformation_rules.properties)} rules"
         logging.info(output_text)
         return FlowMessage(output_text=output_text)
 
     def step_configuring_stores(self, flow_msg: FlowMessage = None, clean_start: bool = True):
         # Initialize source and solution graph stores . clean_start=True will delete all artifacts(files , locks , etc) from previous runs
         logging.info("Initializing source graph")
```

### Comparing `cognite_neat-0.12.1/cognite/neat/examples/workflows/fast_graph/workflow.yaml` & `cognite_neat-0.12.2/cognite/neat/examples/workflows/fast_graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.12.2/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.12.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/examples/workflows/sheet2cdf/workflow.py` & `cognite_neat-0.12.2/cognite/neat/examples/workflows/sheet2cdf/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                 cdf_store.load_rules_file_from_cdf(rules_file, version)
         else:
             cdf_store.load_rules_file_from_cdf(self.cdf_client, rules_file, version)
 
         self.raw_tables = loader.rules.excel_file_to_table_by_name(rules_file_path)
         self.transformation_rules = parser.parse_transformation_rules(self.raw_tables)
 
-        output_text = f"Loaded {len(self.transformation_rules.properties)} rules"
+        output_text = f"Loaded {len(self.transformation_rules.properties)} rules from {rules_file_path.name!r}."
         logging.info(output_text)
         logging.info(f"Loaded prefixes {str(self.transformation_rules.prefixes)} rules")
 
         self.dataset_id = self.transformation_rules.metadata.data_set_id
         return FlowMessage(output_text=output_text)
 
     def step_configuring_stores(self, flow_msg: FlowMessage = None):
```

### Comparing `cognite_neat-0.12.1/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.12.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.12.2/cognite/neat/explorer/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/explorer/explorer.py` & `cognite_neat-0.12.2/cognite/neat/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.12.2/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js` & `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.LICENSE.txt` & `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.map` & `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.e4f085cf.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.12.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/cognite/neat/migration/wf_manifests.py` & `cognite_neat-0.12.2/cognite/neat/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.1/pyproject.toml` & `cognite_neat-0.12.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.12.1"
+version = "0.12.2"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 packages = [
```

### Comparing `cognite_neat-0.12.1/PKG-INFO` & `cognite_neat-0.12.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.12.1
+Version: 0.12.2
 Summary: Knowledge graph transformation
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

