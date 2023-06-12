# Comparing `tmp/cognite_neat-0.12.9.tar.gz` & `tmp/cognite_neat-0.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.12.9.tar", max compression
+gzip compressed data, was "cognite_neat-0.13.0.tar", max compression
```

## Comparing `cognite_neat-0.12.9.tar` & `cognite_neat-0.13.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0    11351 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/LICENSE
--rw-r--r--   0        0        0     8765 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/README.md
--rw-r--r--   0        0        0       23 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/__init__.py
--rw-r--r--   0        0        0      761 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2652 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/app.py
--rw-r--r--   0        0        0     1344 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0      408 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_classes/__init__.py
--rw-r--r--   0        0        0     4775 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_classes/config.py
--rw-r--r--   0        0        0     8132 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_classes/rules.py
--rw-r--r--   0        0        0    30296 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_classes/transformation_rules.py
--rw-r--r--   0        0        0        0 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      646 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     5449 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/extractors/graph_sheet_to_graph.py
--rw-r--r--   0        0        0     2250 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/extractors/labels.py
--rw-r--r--   0        0        0    37477 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/extractors/rdf_to_assets.py
--rw-r--r--   0        0        0    17870 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/extractors/rdf_to_relationships.py
--rw-r--r--   0        0        0     5400 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
--rw-r--r--   0        0        0     6700 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/extractors/rules_to_graphql.py
--rw-r--r--   0        0        0      138 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0      938 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/loader/graph_capturing_sheet.py
--rw-r--r--   0        0        0    10647 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0      913 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/loader/rules.py
--rw-r--r--   0        0        0        0 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    10373 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0    15303 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/modeler.py
--rw-r--r--   0        0        0      110 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/parser/__init__.py
--rw-r--r--   0        0        0     1727 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/parser/transformation_rules.py
--rw-r--r--   0        0        0       73 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9595 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0    11914 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0     6092 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/utils.py
--rw-r--r--   0        0        0     2559 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      311 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    18503 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17764 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0     6200 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     4103 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      781 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     6648 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0      286 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
--rw-r--r--   0        0        0    94607 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
--rw-r--r--   0        0        0    79580 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    77438 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/rules/power-grid-example.xlsx
--rw-r--r--   0        0        0    75865 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/rules/rules-template.xlsx
--rw-r--r--   0        0        0    52178 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    79427 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1461 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15632 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0     3630 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
--rw-r--r--   0        0        0     2573 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
--rw-r--r--   0        0        0    11477 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0    16421 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
--rw-r--r--   0        0        0     8083 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
--rw-r--r--   0        0        0    13784 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6025 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0    11867 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
--rw-r--r--   0        0        0     6837 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
--rw-r--r--   0        0        0        0 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1013 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    21517 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4003 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1359583 2023-06-11 12:15:28.896066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js
--rw-r--r--   0        0        0     2667 2023-06-11 12:15:28.896066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt
--rw-r--r--   0        0        0  5853485 2023-06-11 12:15:28.924066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map
--rw-r--r--   0        0        0     2633 2023-06-11 12:15:28.924066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/main.py
--rw-r--r--   0        0        0        0 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/migration/wf_manifests.py
--rw-r--r--   0        0        0     2471 2023-06-11 12:15:29.380070 cognite_neat-0.12.9/pyproject.toml
--rw-r--r--   0        0        0    10241 1970-01-01 00:00:00.000000 cognite_neat-0.12.9/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/LICENSE
+-rw-r--r--   0        0        0     8765 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/README.md
+-rw-r--r--   0        0        0       23 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2652 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     1344 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0      408 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_classes/__init__.py
+-rw-r--r--   0        0        0     4775 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_classes/config.py
+-rw-r--r--   0        0        0     8132 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_classes/rules.py
+-rw-r--r--   0        0        0    30296 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_classes/transformation_rules.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     1520 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0      646 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0     5449 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/graph_sheet_to_graph.py
+-rw-r--r--   0        0        0     2250 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/labels.py
+-rw-r--r--   0        0        0    39123 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/rdf_to_assets.py
+-rw-r--r--   0        0        0    17870 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/rdf_to_relationships.py
+-rw-r--r--   0        0        0     5400 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
+-rw-r--r--   0        0        0     6700 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/rules_to_graphql.py
+-rw-r--r--   0        0        0      138 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0      938 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/loader/graph_capturing_sheet.py
+-rw-r--r--   0        0        0    10647 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0      913 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/loader/rules.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    10373 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0    15303 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/modeler.py
+-rw-r--r--   0        0        0      110 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/parser/__init__.py
+-rw-r--r--   0        0        0     1727 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/parser/transformation_rules.py
+-rw-r--r--   0        0        0       73 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9595 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0    11914 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0     6092 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/utils.py
+-rw-r--r--   0        0        0     2559 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      311 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    18823 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17764 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0     6200 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     4103 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0      781 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     6648 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0      286 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
+-rw-r--r--   0        0        0    94607 2023-06-12 08:39:19.065880 cognite_neat-0.13.0/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
+-rw-r--r--   0        0        0    79580 2023-06-12 08:39:19.065880 cognite_neat-0.13.0/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    77438 2023-06-12 08:39:19.065880 cognite_neat-0.13.0/cognite/neat/examples/rules/power-grid-example.xlsx
+-rw-r--r--   0        0        0    75865 2023-06-12 08:39:19.065880 cognite_neat-0.13.0/cognite/neat/examples/rules/rules-template.xlsx
+-rw-r--r--   0        0        0    52178 2023-06-12 08:39:19.065880 cognite_neat-0.13.0/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    79427 2023-06-12 08:39:19.065880 cognite_neat-0.13.0/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1461 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15632 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0     3630 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
+-rw-r--r--   0        0        0     2573 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
+-rw-r--r--   0        0        0    11477 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0    16421 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
+-rw-r--r--   0        0        0     8083 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
+-rw-r--r--   0        0        0    14103 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6668 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0    11867 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
+-rw-r--r--   0        0        0     6837 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1013 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    21517 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4003 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1359583 2023-06-12 08:39:19.081880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js
+-rw-r--r--   0        0        0     2667 2023-06-12 08:39:19.081880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt
+-rw-r--r--   0        0        0  5853485 2023-06-12 08:39:19.113881 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map
+-rw-r--r--   0        0        0     2633 2023-06-12 08:39:19.113881 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/main.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/migration/wf_manifests.py
+-rw-r--r--   0        0        0     2577 2023-06-12 08:39:19.565889 cognite_neat-0.13.0/pyproject.toml
+-rw-r--r--   0        0        0    10431 1970-01-01 00:00:00.000000 cognite_neat-0.13.0/PKG-INFO
```

### Comparing `cognite_neat-0.12.9/LICENSE` & `cognite_neat-0.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/README.md` & `cognite_neat-0.13.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/constants.py` & `cognite_neat-0.13.0/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/app.py` & `cognite_neat-0.13.0/cognite/neat/core/app.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/configuration.py` & `cognite_neat-0.13.0/cognite/neat/core/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/data_classes/config.py` & `cognite_neat-0.13.0/cognite/neat/core/data_classes/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/data_classes/rules.py` & `cognite_neat-0.13.0/cognite/neat/core/data_classes/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/data_classes/transformation_rules.py` & `cognite_neat-0.13.0/cognite/neat/core/data_classes/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/data_stores/metrics.py` & `cognite_neat-0.13.0/cognite/neat/core/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.13.0/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/extractors/__init__.py` & `cognite_neat-0.13.0/cognite/neat/core/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/extractors/graph_sheet_to_graph.py` & `cognite_neat-0.13.0/cognite/neat/core/extractors/graph_sheet_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/extractors/labels.py` & `cognite_neat-0.13.0/cognite/neat/core/extractors/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/extractors/rdf_to_assets.py` & `cognite_neat-0.13.0/cognite/neat/core/extractors/rdf_to_assets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import warnings
 from collections.abc import Iterable, Sequence
+from dataclasses import dataclass, fields
 from datetime import datetime, timezone
-from typing import Any, Dict, List, Optional, Tuple, Union, overload
+from typing import Any, Dict, List, Optional, Self, Tuple, Union, overload
 from warnings import warn
 
 import numpy as np
 import pandas as pd
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Asset, AssetHierarchy, AssetList
 from deepdiff import DeepDiff
@@ -15,30 +16,39 @@
 
 from cognite.neat.core.data_classes import AssetTemplate, Property
 from cognite.neat.core.data_classes.config import EXCLUDE_PATHS
 from cognite.neat.core.data_classes.transformation_rules import TransformationRules
 from cognite.neat.core.loader.graph_store import NeatGraphStore
 from cognite.neat.core.utils import chunker, datetime_utc_now, remove_namespace, retry_decorator
 
-ORPHANAGE = {
-    "external_id": "orphanage",
-    "name": "Orphanage",
-    "parent_external_id": None,
-    "description": "Used to store all assets which parent does not exist",
-    "metadata": {
-        "type": "Orphanage",
-        "cdfResourceType": "Asset",
-        "identifier": "orphanage",
-        "active": "true",
-        "start_time": "",
-        "update_time": "",
-    },
-    "data_set_id": None,
-    "labels": ["Orphanage", "non-historic"],
-}
+
+@dataclass
+class NeatMetadataKeys:
+    start_time: str = "start_time"
+    end_time: str = "end_time"
+    update_time: str = "update_time"
+    resurrection_time: str = "resurrection_time"
+    identifier: str = "identifier"
+    active: str = "active"
+    type: str = "type"
+
+    @classmethod
+    def load(cls, data: dict) -> Self:
+        cls_field_names = {f.name for f in fields(cls)}
+        valid_keys = {}
+        for key, value in data.items():
+            if key in cls_field_names:
+                valid_keys[key] = value
+            else:
+                logging.warning(f"Invalid key set {key}")
+
+        return cls(**valid_keys)
+
+    def as_aliases(self) -> dict[str, str]:
+        return {field.default: getattr(self, field.name) for field in fields(self)}
 
 
 def _get_class_instance_ids(graph: Graph, class_: str, namespace: Namespace, limit: int = -1) -> List[URIRef]:
     """Get instances ids for a given class
 
     Parameters
     ----------
@@ -189,17 +199,18 @@
 
 
 def _class2asset_instance(
     class_: str,
     class_instance: dict,
     asset_class_mapping: dict,
     data_set_id: int,
+    meta_keys: NeatMetadataKeys,
     orphanage_asset_external_id: str = None,
     external_id_prefix: str = None,
-    fallback_property: str = "identifier",
+    fallback_property: str = NeatMetadataKeys.identifier,
     empty_name_default: str = "Missing Name",
     add_missing_metadata: bool = True,
 ) -> dict:
     """Converts class instance to asset instance dictionary
 
     Parameters
     ----------
@@ -227,15 +238,15 @@
     """
 
     remapped_class_instance, missing_properties, missing_metadata = _remap_class_properties(
         class_instance, asset_class_mapping
     )
 
     # setting class instance type to class name
-    remapped_class_instance["type"] = class_
+    remapped_class_instance[meta_keys.type] = class_
     # This will be a default case since we want to use original identifier as external_id
     # We are though dropping namespace from the original identifier (avoiding long-tail URIs)
     if "external_id" in missing_properties or asset_class_mapping["external_id"] == []:
         try:
             __extracted_from___class2asset_instance_49(
                 remapped_class_instance,
                 fallback_property,
@@ -337,29 +348,37 @@
 
 
 def rdf2assets(
     graph_store: NeatGraphStore,
     transformation_rules: TransformationRules,
     stop_on_exception: bool = False,
     use_orphanage: bool = True,
+    meta_keys: NeatMetadataKeys | None = None,
 ) -> dict[str, dict[str, Any]]:
     """Creates assets from RDF graph
 
     Parameters
     ----------
-    graph : Graph
+    graph_store : Graph
         Graph containing RDF data
     transformation_rules : TransformationRules
         Instance of TransformationRules class containing transformation rules
+    stop_on_exception : bool
+        Whether to stop upon exception.
+    use_orphanage : bool
+        Whether to use an orphanage for assets without parent_external_id
+    meta_keys : NeatMetadataKeys
+        The names of neat metadat keys to use.
 
     Returns
     -------
-    Dict[str, Asset]
-        Dictionary of assets with external_id as key
+    Dict[str, dict]
+        Dictionary representations of assets by external id.
     """
+    meta_keys = NeatMetadataKeys() if meta_keys is None else meta_keys
 
     orphanage_asset_external_id = (
         f"{transformation_rules.metadata.externalIdPrefix or ''}orphanage-{transformation_rules.metadata.data_set_id}"
     )
 
     graph = graph_store.get_graph()
     # Step 1: Create rdf to asset property mapping
@@ -371,14 +390,15 @@
     assets: dict[str, dict[str, Any]] = {}
     class_ids = {
         class_: _get_class_instance_ids(graph, class_, transformation_rules.metadata.namespace)
         for class_ in asset_class_mapping
     }
     # Step 5: Create Assets based on class instances
     logging.info("Create Assets based on class instances")
+    meta_keys_aliases = meta_keys.as_aliases()
     for class_ in asset_class_mapping:
         # TODO: Rename class_id to instance_id
         class_ns = transformation_rules.metadata.namespace[class_]
         logging.debug(f"Processing class <{class_ns}> . Number of instances: {len(class_ids[class_])}")
         progress_counter = 0
         # loading all instances into cache
         try:
@@ -404,22 +424,26 @@
 
                 # class instance is repaired and converted to asset dictionary
                 asset = _class2asset_instance(
                     class_,
                     class_instance,
                     asset_class_mapping[class_],
                     transformation_rules.metadata.data_set_id,
+                    meta_keys,
                     orphanage_asset_external_id if use_orphanage else None,  # we need only base external id
                     transformation_rules.metadata.externalIdPrefix or None,
+                    fallback_property=meta_keys.identifier,
                 )
 
                 # adding labels and timestamps
-                asset["labels"] = [asset["metadata"]["type"], "non-historic"]
-                asset["metadata"]["start_time"] = str(datetime.now(timezone.utc))
-                asset["metadata"]["update_time"] = str(datetime.now(timezone.utc))
+                asset["labels"] = [asset["metadata"][meta_keys.type], "non-historic"]
+                now = str(datetime.now(timezone.utc))
+                asset["metadata"][meta_keys.start_time] = now
+                asset["metadata"][meta_keys.update_time] = now
+                asset["metadata"] = {meta_keys_aliases.get(k, k): v for k, v in asset["metadata"].items()}
 
                 # log every 10000 assets
                 if progress_counter % 10000 == 0:
                     logging.info(" Next 10000 Assets processed")
 
                 assets[asset["external_id"]] = asset
                 progress_counter += 1
@@ -429,15 +453,20 @@
                 )
                 if stop_on_exception:
                     raise ValidationError
 
         logging.debug(f"Class <{class_}> processed")
 
     if orphanage_asset_external_id not in assets:
-        _extracted_from_rdf2asset_dictionary_95(orphanage_asset_external_id, transformation_rules, assets)
+        logging.warning(f"Orphanage with external id {orphanage_asset_external_id} not found in asset hierarchy!")
+        logging.warning(f"Adding default orphanage with external id {orphanage_asset_external_id}")
+        assets[orphanage_asset_external_id] = _create_orphanage(
+            orphanage_asset_external_id, transformation_rules.metadata.data_set_id, meta_keys
+        )
+
     logging.info("Assets dictionary created")
 
     return assets
 
 
 def rdf2asset_dictionary(
     graph_store: NeatGraphStore,
@@ -446,26 +475,32 @@
     use_orphanage: bool = True,
 ) -> Dict[str, Asset]:
     warn("'rdf2asset_dictionary' is deprecated, please use 'rdf2assets' instead!")
     logging.warning("'rdf2asset_dictionary' is deprecated, please use 'rdf2assets' instead!")
     return rdf2assets(graph_store, transformation_rules, stop_on_exception, use_orphanage)
 
 
-# TODO Rename this here and in `rdf2asset_dictionary`
-def _extracted_from_rdf2asset_dictionary_95(orphanage_asset_external_id, transformation_rules, assets):
-    print(f"Orphanage with external id {orphanage_asset_external_id} not found in asset hierarchy!")
-    logging.warning(f"Orphanage with external id {orphanage_asset_external_id} not found in asset hierarchy!")
-    logging.warning(f"Adding default orphanage with external id {orphanage_asset_external_id}")
-
-    # updating default external id for orphanage in case there are additional prefix to be added
-    ORPHANAGE["external_id"] = orphanage_asset_external_id
-    ORPHANAGE["data_set_id"] = transformation_rules.metadata.data_set_id
-    ORPHANAGE["metadata"]["start_time"] = str(datetime_utc_now())
-    ORPHANAGE["metadata"]["update_time"] = str(datetime_utc_now())
-    assets[orphanage_asset_external_id] = ORPHANAGE
+def _create_orphanage(orphanage_external_id: str, dataset_id: int, meta_keys: NeatMetadataKeys) -> dict:
+    now = str(datetime_utc_now())
+    return {
+        "external_id": orphanage_external_id,
+        "name": "Orphanage",
+        "parent_external_id": None,
+        "description": "Used to store all assets which parent does not exist",
+        "metadata": {
+            meta_keys.type: "Orphanage",
+            "cdfResourceType": "Asset",
+            meta_keys.identifier: "orphanage",
+            meta_keys.active: "true",
+            meta_keys.start_time: now,
+            meta_keys.update_time: now,
+        },
+        "data_set_id": dataset_id,
+        "labels": ["Orphanage", "non-historic"],
+    }
 
 
 def _asset2dict(asset: Asset) -> dict:
     """Return asset as dict representation
 
     Parameters
     ----------
@@ -612,27 +647,30 @@
     return []
 
 
 def _assets_to_update(
     rdf_assets: dict,
     cdf_assets: pd.DataFrame,
     asset_ids: set,
+    meta_keys: NeatMetadataKeys,
     exclude_paths: list = EXCLUDE_PATHS,
     stop_on_exception: bool = False,
 ) -> tuple[list[Asset], dict[str, dict]]:
     """Return list of assets to be updated
 
     Parameters
     ----------
     rdf_assets : dict
         Dictionary containing assets derived from knowledge graph (RDF)
     cdf_assets : pd.DataFrame
         Dataframe containing assets from CDF
     asset_ids : set
         Candidate assets to be updated
+    meta_keys : NeatMetadataKeys
+        The neat meta data keys.
     exclude_paths : list, optional
         Paths not to be checked when diffing rdf and cdf assets, by default EXCLUDE_PATHS
     stop_on_exception: bool, optional
         Whether to stop on exception or not, by default False
 
     Returns
     -------
@@ -665,30 +703,32 @@
                 logging.warning(msg)
                 warnings.warn(
                     msg,
                     stacklevel=2,
                 )
                 continue
 
-        if diffing_result and "root['metadata']['active']" not in diffing_result.affected_paths:
+        if diffing_result and f"root['metadata']['{meta_keys.active}']" not in diffing_result.affected_paths:
             asset = Asset(**rdf_assets[external_id])
             try:
-                asset.metadata["start_time"] = cdf_asset[external_id]["metadata"]["start_time"]
+                asset.metadata[meta_keys.start_time] = cdf_asset[external_id]["metadata"][meta_keys.start_time]
             except KeyError:
-                asset.metadata["start_time"] = str(datetime.now(timezone.utc))
-            asset.metadata["update_time"] = str(datetime.now(timezone.utc))
+                asset.metadata[meta_keys.start_time] = str(datetime.now(timezone.utc))
+            asset.metadata[meta_keys.update_time] = str(datetime.now(timezone.utc))
             assets.append(asset)
 
             report[external_id] = dict(diffing_result)
 
     logging.info(f"Wrangling of {len(assets)} completed in {(datetime_utc_now() - start_time).seconds} seconds")
     return assets, report
 
 
-def _assets_to_resurrect(rdf_assets: dict, cdf_assets: pd.DataFrame, asset_ids: set) -> list[Asset]:
+def _assets_to_resurrect(
+    rdf_assets: dict, cdf_assets: pd.DataFrame, asset_ids: set, meta_keys: NeatMetadataKeys
+) -> list[Asset]:
     """Returns list of assets to be resurrected
 
     Parameters
     ----------
     rdf_assets : dict
         Dictionary containing assets derived from knowledge graph (RDF)
     cdf_assets : pd.DataFrame
@@ -710,46 +750,47 @@
         row["external_id"]: row
         for row in cdf_assets[cdf_assets["external_id"].isin(asset_ids)].to_dict(orient="records")
     }
     for external_id in asset_ids:
         cdf_asset = cdf_asset_subset[external_id]
 
         asset = Asset(**rdf_assets[external_id])
-
+        now = str(datetime.now(timezone.utc))
         try:
-            asset.metadata["start_time"] = cdf_asset[external_id]["metadata"]["start_time"]
+            asset.metadata[meta_keys.start_time] = cdf_asset[external_id]["metadata"][meta_keys.start_time]
         except KeyError:
-            asset.metadata["start_time"] = str(datetime.now(timezone.utc))
-        asset.metadata["update_time"] = str(datetime.now(timezone.utc))
-        asset.metadata["resurrection_time"] = str(datetime.now(timezone.utc))
+            asset.metadata[meta_keys.start_time] = now
+        asset.metadata[meta_keys.update_time] = now
+        asset.metadata[meta_keys.resurrection_time] = now
         assets.append(asset)
 
     logging.info(f"Wrangling of {len(assets)} completed in {(datetime_utc_now() - start_time).seconds} seconds")
     return assets
 
 
-def _assets_to_decommission(cdf_assets, asset_ids) -> list[Asset]:
+def _assets_to_decommission(cdf_assets, asset_ids, meta_keys: NeatMetadataKeys) -> list[Asset]:
     start_time = datetime_utc_now()
 
     assets = []
     if not asset_ids:
         return []
     logging.info("Wrangling assets to be decommissioned into their final form")
     cdf_asset_subset = {
         row["external_id"]: row
         for row in cdf_assets[cdf_assets["external_id"].isin(asset_ids)].to_dict(orient="records")
     }
 
     for external_id in asset_ids:
         cdf_asset = cdf_asset_subset[external_id]
 
-        cdf_asset["metadata"]["update_time"] = str(datetime.now(timezone.utc))
-        cdf_asset["metadata"].pop("resurrection_time", None)
-        cdf_asset["metadata"]["end_time"] = str(datetime.now(timezone.utc))
-        cdf_asset["metadata"]["active"] = "false"
+        now = str(datetime.now(timezone.utc))
+        cdf_asset["metadata"][meta_keys.update_time] = now
+        cdf_asset["metadata"].pop(meta_keys.resurrection_time, None)
+        cdf_asset["metadata"][meta_keys.end_time] = now
+        cdf_asset["metadata"][meta_keys.active] = "false"
         try:
             cdf_asset["labels"].remove("non-historic")
         except KeyError:
             logging.info(f"Asset {external_id} missed label 'non-historic'")
         cdf_asset["labels"].add("historic")
 
         assets.append(Asset(**cdf_asset))
@@ -761,14 +802,15 @@
 def categorize_assets(
     client: CogniteClient,
     rdf_assets: dict,
     data_set_id: int,
     partitions: int = 2,
     stop_on_exception: bool = False,
     return_report: bool = False,
+    meta_keys: NeatMetadataKeys | None = None,
 ) -> Union[tuple[dict, dict], dict]:
     """Categorize assets on those that are to be created, updated and decommissioned
 
     Parameters
     ----------
     client : CogniteClient
         Instance of CogniteClient
@@ -778,22 +820,25 @@
         Dataset id to which assets are to be/are stored
     partitions : int, optional
         Number of partitions to use when fetching assets from CDF, by default 2
     stop_on_exception : bool, optional
         Whether to stop on exception or not, by default False
     return_report : bool, optional
         Whether to report on the diffing results or not, by default False
+    meta_keys : NeatMetadataKeys, optional
+        The metadata keys used by neat.
 
     Returns
     -------
     Dict[str, list]
         dictionary containing asset category - list of asset pairs
     """
-    # TODO: Cache categorized assets somewhere instead of creating them
+    meta_keys = NeatMetadataKeys() if meta_keys is None else meta_keys
 
+    # TODO: Cache categorized assets somewhere instead of creating them
     cdf_assets, categorized_asset_ids = _categorize_cdf_assets(client, data_set_id, partitions)
 
     rdf_asset_ids = set(rdf_assets.keys())
 
     # ids to create
     create_ids = rdf_asset_ids.difference(
         categorized_asset_ids["historic"].union(categorized_asset_ids["non-historic"])
@@ -813,20 +858,20 @@
     logging.info(f"Number of assets to decommission: { len(decommission_ids)}")
     logging.info(f"Number of assets to resurrect: { len(resurrect_ids)}")
 
     report = {"create": create_ids, "resurrect": resurrect_ids, "decommission": decommission_ids, "update": None}
     categorized_assets = {
         "create": _assets_to_create(rdf_assets, create_ids),
         "update": None,
-        "resurrect": _assets_to_resurrect(rdf_assets, cdf_assets, resurrect_ids),
-        "decommission": _assets_to_decommission(cdf_assets, decommission_ids),
+        "resurrect": _assets_to_resurrect(rdf_assets, cdf_assets, resurrect_ids, meta_keys),
+        "decommission": _assets_to_decommission(cdf_assets, decommission_ids, meta_keys),
     }
 
     categorized_assets["update"], report["update"] = _assets_to_update(
-        rdf_assets, cdf_assets, update_ids, stop_on_exception=stop_on_exception
+        rdf_assets, cdf_assets, update_ids, meta_keys=meta_keys, stop_on_exception=stop_on_exception
     )
 
     return (categorized_assets, report) if return_report else categorized_assets
 
 
 def _micro_batch_push(
     client: CogniteClient,
```

### Comparing `cognite_neat-0.12.9/cognite/neat/core/extractors/rdf_to_relationships.py` & `cognite_neat-0.13.0/cognite/neat/core/extractors/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py` & `cognite_neat-0.13.0/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/extractors/rules_to_graphql.py` & `cognite_neat-0.13.0/cognite/neat/core/extractors/rules_to_graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/loader/config.py` & `cognite_neat-0.13.0/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/loader/graph.py` & `cognite_neat-0.13.0/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/loader/graph_capturing_sheet.py` & `cognite_neat-0.13.0/cognite/neat/core/loader/graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.13.0/cognite/neat/core/loader/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/loader/rules.py` & `cognite_neat-0.13.0/cognite/neat/core/loader/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.13.0/cognite/neat/core/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/modeler.py` & `cognite_neat-0.13.0/cognite/neat/core/modeler.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/parser/transformation_rules.py` & `cognite_neat-0.13.0/cognite/neat/core/parser/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.13.0/cognite/neat/core/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/transformer.py` & `cognite_neat-0.13.0/cognite/neat/core/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/utils.py` & `cognite_neat-0.13.0/cognite/neat/core/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/validator.py` & `cognite_neat-0.13.0/cognite/neat/core/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/workflow/base.py` & `cognite_neat-0.13.0/cognite/neat/core/workflow/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,14 +402,21 @@
 
     def set_task_builder(self, task_builder: WorkflowTaskBuilder):
         self.task_builder = task_builder
 
     def get_config_item(self, config_name: str) -> WorkflowConfigItem:
         return next((item for item in self.configs if item.name == config_name), None)
 
+    def get_config_group_values_by_name(self, group_name: str, remove_group_prefix: bool = True) -> dict[str, str]:
+        return {
+            (item.name.removeprefix(item.group) if remove_group_prefix else item.name): item.value
+            for item in self.configs
+            if item.group == group_name
+        }
+
     def get_config_item_value(self, config_name: str, default_value=None) -> str | None:
         return config.value if (config := self.get_config_item(config_name)) else default_value
 
     def set_default_dataset_id(self, default_dataset_id: int):
         self.default_dataset_id = default_dataset_id
         self.cdf_store = (
             cdf_store.CdfStore(self.cdf_client, data_set_id=self.default_dataset_id)
```

### Comparing `cognite_neat-0.12.9/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.13.0/cognite/neat/core/workflow/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.13.0/cognite/neat/core/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/workflow/model.py` & `cognite_neat-0.13.0/cognite/neat/core/workflow/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.13.0/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.13.0/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx` & `cognite_neat-0.13.0/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.13.0/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/rules/power-grid-example.xlsx` & `cognite_neat-0.13.0/cognite/neat/examples/rules/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/rules/rules-template.xlsx` & `cognite_neat-0.13.0/cognite/neat/examples/rules/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.13.0/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.13.0/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.13.0/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/default/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/sheet2cdf/workflow.py` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/sheet2cdf/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from cognite.client.data_classes import AssetFilter
 from prometheus_client import Gauge
 
 from cognite.neat.core import loader, parser
 from cognite.neat.core.data_classes.transformation_rules import TransformationRules
 from cognite.neat.core.extractors.labels import upload_labels
 from cognite.neat.core.extractors.rdf_to_assets import (
+    NeatMetadataKeys,
     categorize_assets,
     rdf2assets,
     remove_non_existing_labels,
     unique_asset_labels,
     upload_assets,
 )
 from cognite.neat.core.extractors.rdf_to_relationships import (
@@ -47,14 +48,15 @@
         self.solution_graph: NeatGraphStore = None
         self.raw_tables = None
         self.transformation_rules: TransformationRules = None
         self.stop_on_error = False
         self.triples = []
         self.instance_ids = set()
         self.count_create_assets = 0
+        self.meta_keys: NeatMetadataKeys | None = None
 
     def step_load_transformation_rules(self, flow_msg: FlowMessage = None):
         # Load rules from file or remote location
         cdf_store = CdfStore(self.cdf_client, self.dataset_id, rules_storage_path=self.rules_storage_path)
 
         rules_file = self.get_config_item("rules.file").value
         rules_file_path = Path(self.rules_storage_path, rules_file)
@@ -124,19 +126,23 @@
     def step_create_cdf_labels(self, flow_msg: FlowMessage = None):
         logging.info("Creating CDF labels")
         upload_labels(self.cdf_client, self.transformation_rules, extra_labels=["non-historic", "historic"])
 
     def step_prepare_cdf_assets(self, flow_msg: FlowMessage):
         # export graph into CDF
         # TODO : decide on error handling and retry logic\
+        self.meta_keys = NeatMetadataKeys.load(
+            self.get_config_group_values_by_name("cdf.asset.metadata.", remove_group_prefix=True)
+        )
 
         rdf_assets = rdf2assets(
             self.solution_graph,
             self.transformation_rules,
             stop_on_exception=self.stop_on_error,
+            meta_keys=self.meta_keys,
         )
 
         if not self.cdf_client:
             logging.info("Dry run, no CDF client available")
             return
 
         # Label Validation
@@ -199,15 +205,17 @@
         elif orphan_assets:
             msg = f"Not able to fix orphans: {', '.join(orphan_assets)}"
             logging.error(msg)
             raise Exception(msg)
         else:
             logging.info("No circular dependency among assets found, your assets hierarchy look healthy!")
 
-        self.categorized_assets = categorize_assets(self.cdf_client, rdf_assets, self.dataset_id)
+        self.categorized_assets = categorize_assets(
+            self.cdf_client, rdf_assets, self.dataset_id, meta_keys=self.meta_keys
+        )
 
         count_create_assets = len(self.categorized_assets["create"])
         count_update_assets = len(self.categorized_assets["update"])
         count_decommission_assets = len(self.categorized_assets["decommission"])
         count_resurrect_assets = len(self.categorized_assets["resurrect"])
 
         prom_cdf_resource_stats.labels(resource_type="asset", state="create").set(count_create_assets)
```

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,35 @@
 -   group: rules
     label: null
     name: rules.version
     options: null
     required: false
     type: null
     value: ''
+-   group: cdf.asset.metadata.
+    name: cdf.asset.metadata.type
+    value: type
+-   group: cdf.asset.metadata.
+    name: cdf.asset.metadata.active
+    value: active
+-   group: cdf.asset.metadata.
+    name: cdf.asset.metadata.identifier
+    value: identifier
+-   group: cdf.asset.metadata.
+    name: cdf.asset.metadata.start_time
+    value: start_time
+-   group: cdf.asset.metadata.
+    name: cdf.asset.metadata.end_time
+    value: end_time
+-   group: cdf.asset.metadata.
+    name: cdf.asset.metadata.update_time
+    value: update_time
+-   group: cdf.asset.metadata.
+    name: cdf.asset.metadata.resurrection_time
+    value: resurrection_time
 description: null
 system_components:
 -   description: null
     id: source_excel_sheet
     label: Transformation Rules
     transition_to:
     - excel2rdf_parser
```

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/sme_graph_capture/workflow.py` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml` & `cognite_neat-0.13.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.13.0/cognite/neat/explorer/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/explorer/explorer.py` & `cognite_neat-0.13.0/cognite/neat/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.13.0/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js` & `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt` & `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map` & `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/cognite/neat/migration/wf_manifests.py` & `cognite_neat-0.13.0/cognite/neat/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.9/pyproject.toml` & `cognite_neat-0.13.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.12.9"
+version = "0.13.0"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
+documentation = "https://cognite-neat.readthedocs-hosted.com/"
+homepage = "https://cognite-neat.readthedocs-hosted.com/"
+repository = "https://github.com/cognitedata/neat"
 packages = [
     { include="cognite", from="." },
 ]
 exclude = [
     "cognite/neat/explorer-ui/neat-app/public/**",
     "cognite/neat/explorer-ui/neat-app/src/**",
     "cognite/neat/explorer-ui/neat-app/node_modules/**",
     "cognite/neat/explorer-ui/neat-app/*.json",
 ]
-[tool.poetry.group.dev.dependencies]
-mkdocs-glightbox = "^0.3.4"
-
 
 
 [tool.black]
 line-length = 120
 target_version = ['py311']
 include = '\.py$'
```

### Comparing `cognite_neat-0.12.9/PKG-INFO` & `cognite_neat-0.13.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.12.9
+Version: 0.13.0
 Summary: Knowledge graph transformation
+Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -32,14 +33,16 @@
 Requires-Dist: pydantic
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: rdflib
 Requires-Dist: requests
 Requires-Dist: schedule (>=1,<2)
 Requires-Dist: urllib3 (>=1.26,<2.0)
 Requires-Dist: uvicorn[standard] (>=0.21.0,<0.22.0)
+Project-URL: Documentation, https://cognite-neat.readthedocs-hosted.com/
+Project-URL: Repository, https://github.com/cognitedata/neat
 Description-Content-Type: text/markdown
 
 # kNowlEdge grAph Transformer (NEAT)
 
 This is python package handles transformation of domain knowledge graphs (more detailed, overarching) to app specific knowledge graphs.
 
 ## Quickstart
```

