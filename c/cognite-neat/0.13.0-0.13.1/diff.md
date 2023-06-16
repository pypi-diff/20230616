# Comparing `tmp/cognite_neat-0.13.0.tar.gz` & `tmp/cognite_neat-0.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.13.0.tar", max compression
+gzip compressed data, was "cognite_neat-0.13.1.tar", max compression
```

## Comparing `cognite_neat-0.13.0.tar` & `cognite_neat-0.13.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0    11351 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/LICENSE
--rw-r--r--   0        0        0     8765 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/README.md
--rw-r--r--   0        0        0       23 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/__init__.py
--rw-r--r--   0        0        0      761 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2652 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/app.py
--rw-r--r--   0        0        0     1344 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0      408 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_classes/__init__.py
--rw-r--r--   0        0        0     4775 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_classes/config.py
--rw-r--r--   0        0        0     8132 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_classes/rules.py
--rw-r--r--   0        0        0    30296 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_classes/transformation_rules.py
--rw-r--r--   0        0        0        0 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      646 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     5449 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/graph_sheet_to_graph.py
--rw-r--r--   0        0        0     2250 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/labels.py
--rw-r--r--   0        0        0    39123 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/rdf_to_assets.py
--rw-r--r--   0        0        0    17870 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/rdf_to_relationships.py
--rw-r--r--   0        0        0     5400 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
--rw-r--r--   0        0        0     6700 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/extractors/rules_to_graphql.py
--rw-r--r--   0        0        0      138 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0      938 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/loader/graph_capturing_sheet.py
--rw-r--r--   0        0        0    10647 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0      913 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/loader/rules.py
--rw-r--r--   0        0        0        0 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    10373 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0    15303 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/modeler.py
--rw-r--r--   0        0        0      110 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/parser/__init__.py
--rw-r--r--   0        0        0     1727 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/parser/transformation_rules.py
--rw-r--r--   0        0        0       73 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9595 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0    11914 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0     6092 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/utils.py
--rw-r--r--   0        0        0     2559 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      311 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    18823 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17764 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0     6200 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     4103 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      781 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     6648 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0      286 2023-06-12 08:39:19.061880 cognite_neat-0.13.0/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
--rw-r--r--   0        0        0    94607 2023-06-12 08:39:19.065880 cognite_neat-0.13.0/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
--rw-r--r--   0        0        0    79580 2023-06-12 08:39:19.065880 cognite_neat-0.13.0/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    77438 2023-06-12 08:39:19.065880 cognite_neat-0.13.0/cognite/neat/examples/rules/power-grid-example.xlsx
--rw-r--r--   0        0        0    75865 2023-06-12 08:39:19.065880 cognite_neat-0.13.0/cognite/neat/examples/rules/rules-template.xlsx
--rw-r--r--   0        0        0    52178 2023-06-12 08:39:19.065880 cognite_neat-0.13.0/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    79427 2023-06-12 08:39:19.065880 cognite_neat-0.13.0/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1461 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15632 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0     3630 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
--rw-r--r--   0        0        0     2573 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
--rw-r--r--   0        0        0    11477 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0    16421 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
--rw-r--r--   0        0        0     8083 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
--rw-r--r--   0        0        0    14103 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6668 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0    11867 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
--rw-r--r--   0        0        0     6837 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
--rw-r--r--   0        0        0        0 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1013 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    21517 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4003 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-06-12 08:39:19.069880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1359583 2023-06-12 08:39:19.081880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js
--rw-r--r--   0        0        0     2667 2023-06-12 08:39:19.081880 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt
--rw-r--r--   0        0        0  5853485 2023-06-12 08:39:19.113881 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map
--rw-r--r--   0        0        0     2633 2023-06-12 08:39:19.113881 cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/main.py
--rw-r--r--   0        0        0        0 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-06-12 08:39:19.117881 cognite_neat-0.13.0/cognite/neat/migration/wf_manifests.py
--rw-r--r--   0        0        0     2577 2023-06-12 08:39:19.565889 cognite_neat-0.13.0/pyproject.toml
--rw-r--r--   0        0        0    10431 1970-01-01 00:00:00.000000 cognite_neat-0.13.0/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/LICENSE
+-rw-r--r--   0        0        0     8765 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/README.md
+-rw-r--r--   0        0        0       23 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2652 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     1344 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0      408 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/data_classes/__init__.py
+-rw-r--r--   0        0        0     4977 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/data_classes/config.py
+-rw-r--r--   0        0        0     8132 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/data_classes/rules.py
+-rw-r--r--   0        0        0    30296 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/data_classes/transformation_rules.py
+-rw-r--r--   0        0        0        0 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     1520 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0      646 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0     5449 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/extractors/graph_sheet_to_graph.py
+-rw-r--r--   0        0        0     2250 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/extractors/labels.py
+-rw-r--r--   0        0        0    39622 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/extractors/rdf_to_assets.py
+-rw-r--r--   0        0        0    18682 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/extractors/rdf_to_relationships.py
+-rw-r--r--   0        0        0     5400 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
+-rw-r--r--   0        0        0     6700 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/extractors/rules_to_graphql.py
+-rw-r--r--   0        0        0      138 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0      938 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/loader/graph_capturing_sheet.py
+-rw-r--r--   0        0        0    10647 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0      913 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/loader/rules.py
+-rw-r--r--   0        0        0        0 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    10373 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0    15303 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/modeler.py
+-rw-r--r--   0        0        0      110 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/parser/__init__.py
+-rw-r--r--   0        0        0     1727 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/parser/transformation_rules.py
+-rw-r--r--   0        0        0       73 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9595 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0    11914 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0     8385 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/utils.py
+-rw-r--r--   0        0        0     2559 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      311 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    18823 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17764 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0     6200 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     4103 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0      781 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     6648 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0      286 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
+-rw-r--r--   0        0        0    94607 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
+-rw-r--r--   0        0        0    79580 2023-06-16 14:47:25.637715 cognite_neat-0.13.1/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    77438 2023-06-16 14:47:25.641715 cognite_neat-0.13.1/cognite/neat/examples/rules/power-grid-example.xlsx
+-rw-r--r--   0        0        0    75865 2023-06-16 14:47:25.641715 cognite_neat-0.13.1/cognite/neat/examples/rules/rules-template.xlsx
+-rw-r--r--   0        0        0    52178 2023-06-16 14:47:25.641715 cognite_neat-0.13.1/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    79427 2023-06-16 14:47:25.641715 cognite_neat-0.13.1/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1461 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15632 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0     3630 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
+-rw-r--r--   0        0        0     2573 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
+-rw-r--r--   0        0        0    11477 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0    16421 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
+-rw-r--r--   0        0        0     8083 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
+-rw-r--r--   0        0        0    14103 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6668 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0    11867 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
+-rw-r--r--   0        0        0     6837 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-06-16 14:47:25.685715 cognite_neat-0.13.1/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 14:47:25.685715 cognite_neat-0.13.1/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1013 2023-06-16 14:47:25.685715 cognite_neat-0.13.1/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    21517 2023-06-16 14:47:25.685715 cognite_neat-0.13.1/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-06-16 14:47:25.685715 cognite_neat-0.13.1/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-06-16 14:47:25.685715 cognite_neat-0.13.1/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4003 2023-06-16 14:47:25.685715 cognite_neat-0.13.1/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-06-16 14:47:25.645715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1360007 2023-06-16 14:47:25.653715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.4a6a952c.js
+-rw-r--r--   0        0        0     2667 2023-06-16 14:47:25.653715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.4a6a952c.js.LICENSE.txt
+-rw-r--r--   0        0        0  5854465 2023-06-16 14:47:25.681715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.4a6a952c.js.map
+-rw-r--r--   0        0        0     2633 2023-06-16 14:47:25.681715 cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-06-16 14:47:25.685715 cognite_neat-0.13.1/cognite/neat/main.py
+-rw-r--r--   0        0        0        0 2023-06-16 14:47:25.685715 cognite_neat-0.13.1/cognite/neat/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-06-16 14:47:25.685715 cognite_neat-0.13.1/cognite/neat/migration/wf_manifests.py
+-rw-r--r--   0        0        0     2577 2023-06-16 14:47:26.149712 cognite_neat-0.13.1/pyproject.toml
+-rw-r--r--   0        0        0    10431 1970-01-01 00:00:00.000000 cognite_neat-0.13.1/PKG-INFO
```

### Comparing `cognite_neat-0.13.0/LICENSE` & `cognite_neat-0.13.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/README.md` & `cognite_neat-0.13.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/constants.py` & `cognite_neat-0.13.1/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/app.py` & `cognite_neat-0.13.1/cognite/neat/core/app.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/configuration.py` & `cognite_neat-0.13.1/cognite/neat/core/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/data_classes/config.py` & `cognite_neat-0.13.1/cognite/neat/core/data_classes/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 
 class ClientConfig(BaseModel):
     project: str = "dev"
     client_id: str = "neat"
     client_name: str = "neat"
     base_url: str = "https://api.cognitedata.com"
     scopes: list[str] = ["project:read", "project:write"]
+    timeout: int = 60
+    max_workers: int = 3
 
     @validator("scopes", pre=True)
     def string_to_list(cls, value):
         return [value] if isinstance(value, str) else value
 
 
 class InteractiveClient(ClientConfig):
@@ -128,14 +130,16 @@
             project=os.environ.get("NEAT_CDF_PROJECT"),
             client_name=os.environ.get("NEAT_CDF_CLIENT_NAME"),
             client_id=os.environ.get("NEAT_CDF_CLIENT_ID"),
             client_secret=os.environ.get("NEAT_CDF_CLIENT_SECRET"),
             base_url=os.environ.get("NEAT_CDF_BASE_URL"),
             token_url=os.environ.get("NEAT_CDF_TOKEN_URL"),
             scopes=[os.environ.get("NEAT_CDF_SCOPES")],
+            timeout=int(os.environ.get("NEAT_CDF_CLIENT_TIMEOUT", "60")),
+            max_workers=int(os.environ.get("NEAT_CDF_CLIENT_MAX_WORKERS", "3")),
         )
 
         if workflow_downloader_filter := os.environ.get("NEAT_WORKFLOW_DOWNLOADER_FILTER", None):
             workflow_downloader_filter = workflow_downloader_filter.split(",")
 
         return cls(
             cdf_client=cdf_config,
```

### Comparing `cognite_neat-0.13.0/cognite/neat/core/data_classes/rules.py` & `cognite_neat-0.13.1/cognite/neat/core/data_classes/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/data_classes/transformation_rules.py` & `cognite_neat-0.13.1/cognite/neat/core/data_classes/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/data_stores/metrics.py` & `cognite_neat-0.13.1/cognite/neat/core/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.13.1/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/extractors/__init__.py` & `cognite_neat-0.13.1/cognite/neat/core/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/extractors/graph_sheet_to_graph.py` & `cognite_neat-0.13.1/cognite/neat/core/extractors/graph_sheet_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/extractors/labels.py` & `cognite_neat-0.13.1/cognite/neat/core/extractors/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/extractors/rdf_to_assets.py` & `cognite_neat-0.13.1/cognite/neat/core/extractors/rdf_to_assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, Dict, List, Optional, Self, Tuple, Union, overload
 from warnings import warn
 
 import numpy as np
 import pandas as pd
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Asset, AssetHierarchy, AssetList
+from cognite.client.exceptions import CogniteDuplicatedError
 from deepdiff import DeepDiff
 from rdflib import Graph, Namespace
 from rdflib.term import URIRef
 
 from cognite.neat.core.data_classes import AssetTemplate, Property
 from cognite.neat.core.data_classes.config import EXCLUDE_PATHS
 from cognite.neat.core.data_classes.transformation_rules import TransformationRules
@@ -909,15 +910,20 @@
         @retry_decorator(max_retries=max_retries, retry_delay=retry_delay, component_name="microbatch-assets")
         def upsert_assets(batch):
             if push_type == "update":
                 client.assets.update(batch)
             elif push_type == "create":
                 client.assets.create_hierarchy(batch)
 
-        upsert_assets(batch)
+        try:
+            upsert_assets(batch)
+        except CogniteDuplicatedError:
+            # this is handling of very rare case when some assets might be lost . Normally this should not happen.
+            # Last attempt to recover
+            client.assets.create_hierarchy(batch, upsert=True)
 
         delta_time = (datetime_utc_now() - start_time).seconds
 
         msg = f"{message} {counter} of {total} assets, batch processing time: {delta_time:.2f} "
         msg += f"seconds ETC: {delta_time * (total - counter) / (60*batch_size) :.2f} minutes"
         logging.info(msg)
 
@@ -985,15 +991,18 @@
 
     else:
         logging.info("Batch size not set, pushing all assets to CDF in one go!")
 
         @retry_decorator(max_retries=max_retries, retry_delay=retry_delay, component_name="create-assets")
         def create_assets():
             if categorized_assets["create"]:
-                client.assets.create_hierarchy(categorized_assets["create"])
+                try:
+                    client.assets.create_hierarchy(categorized_assets["create"])
+                except CogniteDuplicatedError:
+                    client.assets.create_hierarchy(categorized_assets["create"], upsert=True)
 
             if categorized_assets["update"]:
                 client.assets.create_hierarchy(categorized_assets["update"], upsert=True, upsert_mode="replace")
 
             if categorized_assets["resurrect"]:
                 client.assets.create_hierarchy(categorized_assets["resurrect"], upsert=True, upsert_mode="replace")
```

### Comparing `cognite_neat-0.13.0/cognite/neat/core/extractors/rdf_to_relationships.py` & `cognite_neat-0.13.1/cognite/neat/core/extractors/rdf_to_relationships.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # import traceback
 from typing import Dict, List, Set, Union
 from warnings import warn
 
 import pandas as pd
 from cognite.client import CogniteClient
 from cognite.client.data_classes import LabelFilter, Relationship, RelationshipUpdate
+from cognite.client.exceptions import CogniteDuplicatedError
 
 from cognite.neat.core.data_classes.transformation_rules import TransformationRules
 from cognite.neat.core.extractors.rdf_to_assets import _categorize_cdf_assets
 from cognite.neat.core.loader.graph_store import NeatGraphStore
 from cognite.neat.core.utils import chunker, datetime_utc_now, epoch_now_ms, remove_namespace, retry_decorator
 
 # should be renamed to rdf2relationship_data_frame -> rdf2relationships
@@ -365,15 +366,22 @@
         @retry_decorator(max_retries=max_retries, retry_delay=retry_delay, component_name="microbatch-relationships")
         def update_relationships(batch):
             if push_type == "update":
                 client.relationships.update(batch)
             elif push_type == "create":
                 client.relationships.create(batch)
 
-        update_relationships(batch)
+        try:
+            update_relationships(batch)
+        except CogniteDuplicatedError as e:
+            # This situation should not happen but if it does, we need to handle it
+            exists = {d["externalId"] for d in e.duplicated}
+            missing_relationships = [t for t in batch if t.external_id not in exists]
+            client.relationships.create(missing_relationships)
+
         delta_time = (datetime_utc_now() - start_time).seconds
 
         msg = f"{message} {counter} of {total} relationships, batch processing time: {delta_time:.2f} "
         msg += f"seconds ETC: {delta_time * (total - counter) / (60*batch_size) :.2f} minutes"
         logging.info(msg)
 
 
@@ -438,8 +446,14 @@
 
             if categorized_relationships["resurrect"]:
                 client.relationships.update(categorized_relationships["resurrect"])
 
             if categorized_relationships["decommission"]:
                 client.relationships.update(categorized_relationships["decommission"])
 
-        create_relationships()
+        try:
+            create_relationships()
+        except CogniteDuplicatedError as e:
+            # This situation should not happen but if it does, the code attempts to handle it
+            exists = {d["externalId"] for d in e.duplicated}
+            missing_relationships = [t for t in categorized_relationships["create"] if t.external_id not in exists]
+            client.relationships.create(missing_relationships)
```

### Comparing `cognite_neat-0.13.0/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py` & `cognite_neat-0.13.1/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/extractors/rules_to_graphql.py` & `cognite_neat-0.13.1/cognite/neat/core/extractors/rules_to_graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/loader/config.py` & `cognite_neat-0.13.1/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/loader/graph.py` & `cognite_neat-0.13.1/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/loader/graph_capturing_sheet.py` & `cognite_neat-0.13.1/cognite/neat/core/loader/graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.13.1/cognite/neat/core/loader/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/loader/rules.py` & `cognite_neat-0.13.1/cognite/neat/core/loader/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.13.1/cognite/neat/core/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/modeler.py` & `cognite_neat-0.13.1/cognite/neat/core/modeler.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/parser/transformation_rules.py` & `cognite_neat-0.13.1/cognite/neat/core/parser/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.13.1/cognite/neat/core/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/transformer.py` & `cognite_neat-0.13.1/cognite/neat/core/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/utils.py` & `cognite_neat-0.13.1/cognite/neat/core/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from collections import OrderedDict
 from datetime import datetime, timezone
 from functools import wraps
 
 import pandas as pd
 from cognite.client import ClientConfig, CogniteClient
 from cognite.client.credentials import CredentialProvider, OAuthClientCredentials, OAuthInteractive
+from cognite.client.exceptions import CogniteDuplicatedError, CogniteReadTimeout
 from rdflib.term import URIRef
 
 from cognite.neat.core.data_classes.config import InteractiveClient, ServiceClient
 from cognite.neat.core.loader.graph_store import NeatGraphStore
 
 
 def get_cognite_client_from_config(config: ServiceClient) -> CogniteClient:
@@ -28,22 +29,23 @@
         scopes=config.scopes,
         redirect_port=config.redirect_port,
     )
     return _get_cognite_client(config, credentials)
 
 
 def _get_cognite_client(config: ClientConfig, credentials: CredentialProvider) -> CogniteClient:
+    logging.info(f"Creating CogniteClient with parameters : {config}")
     return CogniteClient(
         ClientConfig(
             client_name=config.client_name,
             base_url=config.base_url,
             project=config.project,
             credentials=credentials,
-            timeout=60,
-            max_workers=3,
+            timeout=config.timeout,
+            max_workers=config.max_workers,
             debug=False,
         )
     )
 
 
 def add_triples(graph_store: NeatGraphStore, triples: list[tuple], batch_size: int = 10000):
     """Adds triples to the graph store in batches.
@@ -152,19 +154,56 @@
     return datetime.now(timezone.utc)
 
 
 def retry_decorator(max_retries=2, retry_delay=3, component_name=""):
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
+            previous_exception = None
             for attempt in range(max_retries + 1):
                 try:
                     logging.debug(f"Attempt {attempt + 1} of {max_retries + 1} for {component_name}")
                     return func(*args, **kwargs)
+                except CogniteReadTimeout as e:
+                    previous_exception = e
+                    if attempt < max_retries:
+                        logging.error(
+                            f"""CogniteReadTimeout retry attempt {attempt + 1} failed for {component_name} .
+                            Retrying in {retry_delay} second(s). Error:"""
+                        )
+                        logging.error(e)
+                        time.sleep(retry_delay)
+                    else:
+                        raise e
+                except CogniteDuplicatedError as e:
+                    if isinstance(previous_exception, CogniteReadTimeout):
+                        # if previous exception was CogniteReadTimeout, we can't be sure if the items were created or not
+                        if len(e.successful) == 0 and len(e.failed) == 0 and len(e.duplicated) >= 0:
+                            logging.warning(
+                                f"Duplicate error for {component_name} . All items already exist in CDF. Suppressing error."
+                            )
+                            return
+                        else:
+                            # can happend because of eventual consistency. Retry with delay to allow for CDF to catch up
+                            if attempt < max_retries:
+                                logging.error(
+                                    f"""CogniteDuplicatedError retry attempt {attempt + 1} failed for {component_name} .
+                                      Retrying in {retry_delay} second(s). Error:"""
+                                )
+                                logging.error(e)
+                                # incerasing delay to allow for CDF to catch up
+                                time.sleep(retry_delay)
+                            else:
+                                raise e
+                    else:
+                        # no point in retrying duplicate error if previous exception was not a timeout
+                        raise e
+
                 except Exception as e:
+                    previous_exception = e
                     if attempt < max_retries:
                         logging.error(
                             f"Retry attempt {attempt + 1} failed for {component_name} . Retrying in {retry_delay} second(s)."
                         )
                         logging.error(e)
                         time.sleep(retry_delay)
                     else:
```

### Comparing `cognite_neat-0.13.0/cognite/neat/core/validator.py` & `cognite_neat-0.13.1/cognite/neat/core/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/workflow/base.py` & `cognite_neat-0.13.1/cognite/neat/core/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.13.1/cognite/neat/core/workflow/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.13.1/cognite/neat/core/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/workflow/model.py` & `cognite_neat-0.13.1/cognite/neat/core/workflow/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.13.1/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.13.1/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx` & `cognite_neat-0.13.1/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.13.1/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/rules/power-grid-example.xlsx` & `cognite_neat-0.13.1/cognite/neat/examples/rules/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/rules/rules-template.xlsx` & `cognite_neat-0.13.1/cognite/neat/examples/rules/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.13.1/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.13.1/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.13.1/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/default/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/sheet2cdf/workflow.py` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/sheet2cdf/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.py` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/sme_graph_capture/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml` & `cognite_neat-0.13.1/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.13.1/cognite/neat/explorer/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/explorer/explorer.py` & `cognite_neat-0.13.1/cognite/neat/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.13.1/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="./favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="NEAT controll panel"/><link rel="apple-touch-icon" href="./logo192.png"/><link rel="manifest" href="./manifest.json"/><title>React App</title><script defer="defer" src="./static/js/main.97e96de0.js"></script><link href="./static/css/main.38a62222.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="./favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="NEAT controll panel"/><link rel="apple-touch-icon" href="./logo192.png"/><link rel="manifest" href="./manifest.json"/><title>React App</title><script defer="defer" src="./static/js/main.4a6a952c.js"></script><link href="./static/css/main.38a62222.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js` & `cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.4a6a952c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.97e96de0.js.LICENSE.txt */ ! function() {
+/*! For license information please see main.4a6a952c.js.LICENSE.txt */ ! function() {
     var e = {
             3361: function(e, t, n) {
                 "use strict";
                 n.d(t, {
                     Z: function() {
                         return oe
                     }
@@ -60883,15 +60883,17 @@
                         cdf_client: {
                             project: "",
                             client_id: "",
                             client_name: "neat",
                             base_url: "https://az-power-no-northeurope.cognitedata.com",
                             scopes: ["https://az-power-no-northeurope.cognitedata.com/.default"],
                             token_url: "",
-                            client_secret: ""
+                            client_secret: "",
+                            timeout: 60,
+                            max_workers: 3
                         },
                         cdf_default_dataset_id: 0,
                         load_examples: !0,
                         download_workflows_from_cdf: !1,
                         workflow_downloader_filter: "",
                         log_level: "DEBUG",
                         log_format: "%(asctime)s.%(msecs)03d %(levelname)-8s %(message)s",
@@ -61013,14 +61015,34 @@
                                         label: "Default CDF dataset id.The dataset is used as workflow and rules storage.",
                                         size: "small",
                                         variant: "outlined",
                                         value: c.cdf_default_dataset_id,
                                         onChange: function(e) {
                                             m("cdf_default_dataset_id", e.target.value)
                                         }
+                                    }), (0, E.jsx)(fg, {
+                                        id: "cdf_timeout",
+                                        type: "number",
+                                        label: "Cdf read timeout in seconds.",
+                                        size: "small",
+                                        variant: "outlined",
+                                        value: c.cdf_client.timeout,
+                                        onChange: function(e) {
+                                            y("timeout", e.target.value)
+                                        }
+                                    }), (0, E.jsx)(fg, {
+                                        id: "cdf_max_workers",
+                                        type: "number",
+                                        label: "Max number of client workers.",
+                                        size: "small",
+                                        variant: "outlined",
+                                        value: c.cdf_client.max_workers,
+                                        onChange: function(e) {
+                                            y("max_workers", e.target.value)
+                                        }
                                     }), (0, E.jsx)("h4", {
                                         children: "Storage and workflows"
                                     }), (0, E.jsx)(fg, {
                                         id: "data_store_path",
                                         label: "Data directory.Is used as local workflow , rules and db storage.",
                                         size: "small",
                                         variant: "outlined",
@@ -61711,8 +61733,8 @@
                 })
             };
             r.createRoot(document.getElementById("root")).render((0, E.jsxs)(e.Fragment, {
                 children: [(0, E.jsx)(aO, {}), (0, E.jsx)(rO, {})]
             }))
         }()
 }();
-//# sourceMappingURL=main.97e96de0.js.map
+//# sourceMappingURL=main.4a6a952c.js.map
```

### Comparing `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt` & `cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.4a6a952c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map` & `cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.4a6a952c.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8569799414795123%*

 * *Differences: {"'file'": "'static/js/main.4a6a952c.js'",*

 * * "'mappings'": "';sFAqDA,IAAIA,EAA0B,WAE5B,SAASA,EAAWC,GAClB,IAAIC,EAAQC,KAEZA,KAAKC,WAAa,SAAUC,GAC1B,IAAIC,EAIAA,EAFsB,IAAtBJ,EAAMK,KAAKC,OACTN,EAAMO,eACCP,EAAMO,eAAeC,YACrBR,EAAMS,QACNT,EAAMU,UAAUC,WAEhBX,EAAMI,OAGRJ,EAAMK,KAAKL,EAAMK,KAAKC,OAAS,GAAGE,YAG7CR,EAAMU,UAAUE,aAAaT,EAAKC,GAElCJ,EAAMK,KAAKQ,KAAKV,EAClB,EAEAF,KAAKa,cAA8BC,IAAnBhB,EAAQiB,QAA+DjB,EAAQiB,OAC/Ff,KAAKI,KAAO,GACZJ,KAAKgB,IAAM,EACXhB,KAAKiB,MAAQnB,EAAQmB,MAErBjB,KAAKkB,IAAMpB,EAAQoB,IACnBlB,KAA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.97e96de0.js",
+    "file": "static/js/main.4a6a952c.js",
     "names": [
         "StyleSheet",
         "options",
         "_this",
         "this",
         "_insertTag",
         "tag",
@@ -10746,14 +10746,15 @@
         "client_id",
         "client_secret",
         "client_name",
         "base_url",
         "scopes",
         "token_url",
         "cdf_default_dataset_id",
+        "max_workers",
         "data_store_path",
         "download_workflows_from_cdf",
         "workflow_downloader_filter",
         "load_examples",
         "log_level",
         "getListItemUtilityClass",
         "getListItemSecondaryActionClassesUtilityClass",
@@ -12611,15 +12612,15 @@
         "import React, { useState, useEffect, useRef, useCallback } from 'react';\nimport loader from '@monaco-editor/loader';\nimport useMount from '../hooks/useMount';\nimport useUpdate from '../hooks/useUpdate';\nimport usePrevious from '../hooks/usePrevious';\nimport { type IDisposable, type editor } from 'monaco-editor';\nimport { noop, getOrCreateModel } from '../utils';\nimport { type EditorProps } from './types';\nimport { type Monaco } from '..';\nimport MonacoContainer from '../MonacoContainer';\n\nconst viewStates = new Map();\n\nfunction Editor({\n  defaultValue,\n  defaultLanguage,\n  defaultPath,\n  value,\n  language,\n  path,\n  /* === */\n  theme = 'light',\n  line,\n  loading = 'Loading...',\n  options = {},\n  overrideServices = {},\n  saveViewState = true,\n  keepCurrentModel = false,\n  /* === */\n  width = '100%',\n  height = '100%',\n  className,\n  wrapperProps = {},\n  /* === */\n  beforeMount = noop,\n  onMount = noop,\n  onChange,\n  onValidate = noop,\n}: EditorProps) {\n  const [isEditorReady, setIsEditorReady] = useState(false);\n  const [isMonacoMounting, setIsMonacoMounting] = useState(true);\n  const monacoRef = useRef<Monaco | null>(null);\n  const editorRef = useRef<editor.IStandaloneCodeEditor | null>(null);\n  const containerRef = useRef<HTMLDivElement>(null);\n  const onMountRef = useRef(onMount);\n  const beforeMountRef = useRef(beforeMount);\n  const subscriptionRef = useRef<IDisposable>();\n  const valueRef = useRef(value);\n  const previousPath = usePrevious(path);\n  const preventCreation = useRef(false);\n  const preventTriggerChangeEvent = useRef<boolean>(false);\n\n  useMount(() => {\n    const cancelable = loader.init();\n\n    cancelable\n      .then((monaco) => (monacoRef.current = monaco) && setIsMonacoMounting(false))\n      .catch(\n        (error) =>\n          error?.type !== 'cancelation' && console.error('Monaco initialization: error:', error),\n      );\n\n    return () => (editorRef.current ? disposeEditor() : cancelable.cancel());\n  });\n\n  useUpdate(\n    () => {\n      const model = getOrCreateModel(\n        monacoRef.current!,\n        defaultValue || value || '',\n        defaultLanguage || language || '',\n        path || defaultPath || '',\n      );\n\n      if (model !== editorRef.current?.getModel()) {\n        if (saveViewState) viewStates.set(previousPath, editorRef.current?.saveViewState());\n        editorRef.current?.setModel(model);\n        if (saveViewState) editorRef.current?.restoreViewState(viewStates.get(path));\n      }\n    },\n    [path],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      editorRef.current?.updateOptions(options);\n    },\n    [options],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      if (!editorRef.current || value === undefined) return;\n      if (editorRef.current.getOption(monacoRef.current!.editor.EditorOption.readOnly)) {\n        editorRef.current.setValue(value);\n      } else if (value !== editorRef.current.getValue()) {\n        preventTriggerChangeEvent.current = true;\n        editorRef.current.executeEdits('', [\n          {\n            range: editorRef.current.getModel()!.getFullModelRange(),\n            text: value,\n            forceMoveMarkers: true,\n          },\n        ]);\n\n        editorRef.current.pushUndoStop();\n        preventTriggerChangeEvent.current = false;\n      }\n    },\n    [value],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      const model = editorRef.current?.getModel();\n      if (model && language) monacoRef.current?.editor.setModelLanguage(model, language);\n    },\n    [language],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      // reason for undefined check: https://github.com/suren-atoyan/monaco-react/pull/188\n      if (line !== undefined) {\n        editorRef.current?.revealLine(line);\n      }\n    },\n    [line],\n    isEditorReady,\n  );\n\n  useUpdate(\n    () => {\n      monacoRef.current?.editor.setTheme(theme);\n    },\n    [theme],\n    isEditorReady,\n  );\n\n  const createEditor = useCallback(() => {\n    if (!containerRef.current || !monacoRef.current) return;\n    if (!preventCreation.current) {\n      beforeMountRef.current(monacoRef.current);\n      const autoCreatedModelPath = path || defaultPath;\n\n      const defaultModel = getOrCreateModel(\n        monacoRef.current,\n        value || defaultValue || '',\n        defaultLanguage || language || '',\n        autoCreatedModelPath || '',\n      );\n\n      editorRef.current = monacoRef.current?.editor.create(\n        containerRef.current,\n        {\n          model: defaultModel,\n          automaticLayout: true,\n          ...options,\n        },\n        overrideServices,\n      );\n\n      saveViewState && editorRef.current.restoreViewState(viewStates.get(autoCreatedModelPath));\n\n      monacoRef.current.editor.setTheme(theme);\n\n      setIsEditorReady(true);\n      preventCreation.current = true;\n    }\n  }, [\n    defaultValue,\n    defaultLanguage,\n    defaultPath,\n    value,\n    language,\n    path,\n    options,\n    overrideServices,\n    saveViewState,\n    theme,\n  ]);\n\n  useEffect(() => {\n    if (isEditorReady) {\n      onMountRef.current(editorRef.current!, monacoRef.current!);\n    }\n  }, [isEditorReady]);\n\n  useEffect(() => {\n    !isMonacoMounting && !isEditorReady && createEditor();\n  }, [isMonacoMounting, isEditorReady, createEditor]);\n\n  // subscription\n  // to avoid unnecessary updates (attach - dispose listener) in subscription\n  valueRef.current = value;\n\n  // onChange\n  useEffect(() => {\n    if (isEditorReady && onChange) {\n      subscriptionRef.current?.dispose();\n      subscriptionRef.current = editorRef.current?.onDidChangeModelContent((event) => {\n        if (!preventTriggerChangeEvent.current) {\n          onChange(editorRef.current!.getValue(), event);\n        }\n      });\n    }\n  }, [isEditorReady, onChange]);\n\n  // onValidate\n  useEffect(() => {\n    if (isEditorReady) {\n      const changeMarkersListener = monacoRef.current!.editor.onDidChangeMarkers((uris) => {\n        const editorUri = editorRef.current!.getModel()?.uri;\n\n        if (editorUri) {\n          const currentEditorHasMarkerChanges = uris.find((uri) => uri.path === editorUri.path);\n          if (currentEditorHasMarkerChanges) {\n            const markers = monacoRef.current!.editor.getModelMarkers({\n              resource: editorUri,\n            });\n            onValidate?.(markers);\n          }\n        }\n      });\n\n      return () => {\n        changeMarkersListener?.dispose();\n      };\n    }\n    return () => {\n      // eslint happy\n    };\n  }, [isEditorReady, onValidate]);\n\n  function disposeEditor() {\n    subscriptionRef.current?.dispose();\n\n    if (keepCurrentModel) {\n      saveViewState && viewStates.set(path, editorRef.current!.saveViewState());\n    } else {\n      editorRef.current!.getModel()?.dispose();\n    }\n\n    editorRef.current!.dispose();\n  }\n\n  return (\n    <MonacoContainer\n      width={width}\n      height={height}\n      isEditorReady={isEditorReady}\n      loading={loading}\n      _ref={containerRef}\n      className={className}\n      wrapperProps={wrapperProps}\n    />\n  );\n}\n\nexport default Editor;\n",
         "import loader from '@monaco-editor/loader';\nexport { loader };\n\nimport DiffEditor from './DiffEditor';\nexport * from './DiffEditor/types';\nexport { DiffEditor };\n\nimport useMonaco from './hooks/useMonaco';\nexport { useMonaco };\n\nimport Editor from './Editor';\nexport * from './Editor/types';\nexport { Editor };\nexport default Editor;\n\n// Monaco\nimport type * as monaco from 'monaco-editor/esm/vs/editor/editor.api';\nexport type Monaco = typeof monaco;\n\n// Default themes\nexport type Theme = 'vs-dark' | 'light';\n",
         "import { memo } from 'react';\n\nimport Editor from './Editor';\n\nexport * from './types';\n\nexport default memo(Editor);\n",
         "import Button from \"@mui/material/Button\"\nimport Dialog from \"@mui/material/Dialog\"\nimport DialogActions from \"@mui/material/DialogActions\"\nimport DialogContent from \"@mui/material/DialogContent\"\nimport DialogTitle from \"@mui/material/DialogTitle\"\nimport FormControl from \"@mui/material/FormControl\"\nimport TextField from \"@mui/material/TextField\"\nimport { useEffect, useState } from \"react\"\nimport { WorkflowSystemComponent } from \"types/WorkflowTypes\"\n\nexport default function OverviewComponentEditorDialog(props: any)\n{\n    const [dialogOpen, setDialogOpen] = useState(false);\n    const [component, setComponent] = useState<WorkflowSystemComponent>(null);\n    const handleDialogSave = () => {\n        setDialogOpen(false);\n        props.onClose(component,\"save\");\n    };\n    const handleDialogCancel = () => {\n        setDialogOpen(false);\n        props.onClose(component,\"cancel\");\n    };\n    const handleDelete = () => {\n        setDialogOpen(false);\n        props.onClose(component,\"delete\");\n    };\n    const handleStepConfigChange = (name: string, value: any) => {\n        console.log('handleComponentConfigChange')\n        console.dir(component);\n        let updComponent = Object.assign({},component);\n        updComponent[name] = value;\n        console.log(\"Updateed component\")\n        console.dir(updComponent);\n        setComponent(updComponent);\n    }\n    useEffect(() => {\n        if (props.open){\n            setDialogOpen(true);\n            setComponent(props.component);\n            console.dir(props.component);\n        }\n      }, [props.open]);\n\n\n\nreturn (\n<Dialog open={dialogOpen} onClose={handleDialogCancel}>\n<DialogTitle>Component editor</DialogTitle>\n<DialogContent>\n  <FormControl sx={{ width: 300 }} >\n    <TextField sx={{ marginTop: 1 }} id=\"step-config-id\" fullWidth label=\"Component id\" size='small' variant=\"outlined\" value={component?.id} onChange={(event) => { handleStepConfigChange(\"id\", event.target.value) }} />\n    <TextField sx={{ marginTop: 1 }} id=\"step-config-label\" fullWidth label=\"Label\" size='small' variant=\"outlined\" value={component?.label} onChange={(event) => { handleStepConfigChange(\"label\", event.target.value) }} />\n    <TextField sx={{ marginTop: 1 }} id=\"step-config-descr\" fullWidth label=\"Description\" size='small' variant=\"outlined\" value={component?.description} onChange={(event) => { handleStepConfigChange(\"description\", event.target.value) }} />\n  </FormControl>\n</DialogContent>\n<DialogActions>\n  <Button variant=\"outlined\" size=\"small\" onClick={handleDialogSave}>Save</Button>\n  <Button variant=\"outlined\" size=\"small\" onClick={handleDialogCancel}>Cancel</Button>\n  <Button variant=\"outlined\" size=\"small\" color=\"error\" onClick={handleDelete}>Delete</Button>\n</DialogActions>\n</Dialog>\n)\n}\n",
         "import Button from \"@mui/material/Button\"\nimport Checkbox from \"@mui/material/Checkbox\"\nimport { red } from \"@mui/material/colors\"\nimport Dialog from \"@mui/material/Dialog\"\nimport DialogActions from \"@mui/material/DialogActions\"\nimport DialogContent from \"@mui/material/DialogContent\"\nimport DialogTitle from \"@mui/material/DialogTitle\"\nimport FormControl from \"@mui/material/FormControl\"\nimport FormControlLabel from \"@mui/material/FormControlLabel\"\nimport MenuItem from \"@mui/material/MenuItem\"\nimport Select from \"@mui/material/Select\"\nimport TextField from \"@mui/material/TextField\"\nimport { useEffect, useState } from \"react\"\nimport { WorkflowStepDefinition, WorkflowSystemComponent } from \"types/WorkflowTypes\"\nimport { getNeatApiRootUrl } from \"./Utils\"\nimport LocalUploader from \"./LocalUploader\"\nimport { Typography } from \"@mui/material\"\n\nexport default function StepEditorDialog(props: any)\n{\n    const [dialogOpen, setDialogOpen] = useState(false);\n    const [selectedStep, setSelectedStep] = useState<WorkflowStepDefinition>();\n    const neatApiRootUrl = getNeatApiRootUrl();\n    const [runPayload,setRunPayload] = useState<string>(JSON.stringify({\"action\":\"approve\"}))\n    const [statusText,setStatusText] = useState<string>(\"\")\n\n    const handleDialogSave = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"save\");\n    };\n    const handleDialogCancel = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"cancel\");\n    };\n    const handleDelete = () => {\n        setDialogOpen(false);\n        props.onClose(selectedStep,\"delete\");\n    };\n\n    const handleRunCommand = () => {\n        setDialogOpen(false);\n        // send POST request to run the step\n        fetch(neatApiRootUrl +'/api/workflow/'+props.workflowName+'/http_trigger/'+selectedStep.id, { method: 'POST', body: runPayload })\n        .then(response => response.json())\n        .then(data => {\n            console.log('Success:', data);\n        }).catch((error) => {\n            console.error('Error:', error);\n        })\n        props.onClose(selectedStep,\"run\");\n    };\n\n    const onUpload = (fileName:string , hash: string) => {\n      console.log(\"onUpload\",fileName,hash)\n      setStatusText(\"File uplloaded \"+fileName)\n    }\n\n    useEffect(() => {\n        if (props.open){\n            setDialogOpen(true);\n            setSelectedStep(props.step);\n            console.dir(props.step);\n        }\n      }, [props.open]);\n\n      const handleStepConfigChange = (name: string, value: any) => {\n        console.log('handleStepConfigChange')\n        console.dir(selectedStep);\n        let updStep= Object.assign({},selectedStep);\n\n        if (selectedStep) {\n          if (!selectedStep.params) {\n            selectedStep.params = {}\n          }\n          if (name == \"stype\") {\n            switch (value) {\n              case \"time_trigger\":\n                updStep.params = { \"interval\": \"every 60 minutes\" }\n                break;\n              case \"start_workflow_task_step\":\n                updStep.params = { \"workflow_name\": \"\", \"sync\": \"false\" }\n                break;\n            }\n            updStep[\"stype\"] = value;\n          } else {\n            switch (name) {\n              case \"time-interval\":\n                updStep.params[\"interval\"] = value;\n                break;\n              case \"workflow_name\":\n                updStep.params[\"workflow_name\"] = value;\n                break;\n              case \"workflow_sync_run_flag\":\n                value = \"false\"\n                if (value) {\n                  value = \"true\"\n                }\n                updStep.params[\"sync\"] = value;\n                break;\n              default:\n                updStep[name] = value;\n            }\n          }\n          console.log(\"rendering view\")\n        }\n        setSelectedStep(updStep);\n      }\n\n\nreturn (\n  <Dialog open={dialogOpen} onClose={handleDialogCancel}>\n        <DialogTitle>Step configurator</DialogTitle>\n        <DialogContent>\n          <FormControl sx={{ width: 500 }} >\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-id\" fullWidth label=\"Step id\" size='small' variant=\"outlined\" value={selectedStep?.id} onChange={(event) => { handleStepConfigChange(\"id\", event.target.value) }} />\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-label\" fullWidth label=\"Label\" size='small' variant=\"outlined\" value={selectedStep?.label} onChange={(event) => { handleStepConfigChange(\"label\", event.target.value) }} />\n            <Select sx={{ marginTop: 1 }}\n              id=\"step-config-stype\"\n              value={selectedStep?.stype}\n              label=\"Step type\"\n              size='small'\n              variant=\"outlined\"\n              onChange={(event) => { handleStepConfigChange(\"stype\", event.target.value) }}\n            >\n              <MenuItem value=\"pystep\">Python function</MenuItem>\n              <MenuItem value=\"http_trigger\">HTTP trigger</MenuItem>\n              <MenuItem value=\"time_trigger\">Time trigger</MenuItem>\n              <MenuItem value=\"wait_for_event\">Wait for event</MenuItem>\n              <MenuItem value=\"start_workflow_task_step\">Start workflow</MenuItem>\n              <MenuItem value=\"file_uploader\">File uploader</MenuItem>\n            </Select>\n\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-descr\" fullWidth label=\"Description\" size='small' variant=\"outlined\" value={selectedStep?.description} onChange={(event) => { handleStepConfigChange(\"description\", event.target.value) }} />\n            {(selectedStep?.stype == \"time_trigger\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-config-time-config\" fullWidth label=\"Time interval\" size='small' variant=\"outlined\" value={selectedStep?.params[\"interval\"]} onChange={(event) => { handleStepConfigChange(\"time-interval\", event.target.value) }} />\n            )}\n             {(selectedStep?.stype == \"pystep\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-pystep-method\" fullWidth label=\"Override function name (optional)\" size='small' variant=\"outlined\" value={selectedStep?.method} onChange={(event) => { handleStepConfigChange(\"method\", event.target.value) }} />\n            )}\n            {(selectedStep?.stype == \"start_workflow_task_step\") && (\n              <TextField sx={{ marginTop: 1 }} id=\"step-start_workflow_task_step\" fullWidth label=\"Name of the workflow\" size='small' variant=\"outlined\" value={selectedStep?.params[\"workflow_name\"]} onChange={(event) => { handleStepConfigChange(\"workflow_name\", event.target.value) }} />\n            )}\n            {(selectedStep?.stype == \"start_workflow_task_step\") && (\n              <FormControlLabel control={<Checkbox checked={selectedStep?.params[\"sync\"] == \"true\"} onChange={(event) => { handleStepConfigChange(\"workflow_sync_run_flag\", event.target.checked) }} />} label=\"Synchronous execution\" />\n            )}\n            {(selectedStep?.stype == \"file_uploader\") && (\n               <LocalUploader fileType=\"staging\" action=\"start_workflow\" onUpload={onUpload} stepId={selectedStep.id} workflowName={props.workflowName} />\n            )}\n\n            <FormControlLabel control={<Checkbox checked={selectedStep?.enabled} onChange={(event) => { handleStepConfigChange(\"enabled\", event.target.checked) }} />} label=\"Is enabled\" />\n            <FormControlLabel control={<Checkbox checked={selectedStep?.trigger} onChange={(event) => { handleStepConfigChange(\"trigger\", event.target.checked) }} />} label=\"Is trigger\" />\n            {(selectedStep?.trigger == false) && (\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-max-retries\" fullWidth label=\"Max retries on failure\" size='small' type=\"number\" variant=\"outlined\" value={selectedStep?.max_retries} onChange={(event) => { handleStepConfigChange(\"max_retries\", event.target.value) }} />\n            )}\n             {(selectedStep?.trigger == false) && (\n            <TextField sx={{ marginTop: 1 }} id=\"step-config-retry-delay\" fullWidth label=\"Retry delay\" size='small' variant=\"outlined\" type=\"number\" value={selectedStep?.retry_delay} onChange={(event) => { handleStepConfigChange(\"retry_delay\", event.target.value) }} />\n             )}\n\n            {(selectedStep?.stype == \"http_trigger\" || selectedStep?.stype == \"wait_for_event\") && (\n              <TextField sx={{ marginTop: 1 }} value={runPayload} label=\"Run payload\" onChange={(event)=>setRunPayload(event.target.value)} id=\"run_payload\"> </TextField>\n            )}\n\n\n          </FormControl>\n          <Typography> {statusText} </Typography>\n\n        </DialogContent>\n        <DialogActions>\n          <Button variant=\"outlined\" size=\"small\" onClick={handleDialogSave}>Save</Button>\n          <Button variant=\"outlined\" size=\"small\" onClick={handleDialogCancel}>Cancel</Button>\n          <Button variant=\"outlined\" size=\"small\" color=\"error\" onClick={handleDelete} >Delete</Button>\n          {(selectedStep?.stype == \"http_trigger\" || selectedStep?.stype == \"wait_for_event\") && (\n              <Button variant=\"outlined\" size=\"small\" color=\"success\" onClick={handleRunCommand}>Run</Button>\n          )}\n\n        </DialogActions>\n      </Dialog>\n)\n}\n",
         "import { useCallback, useRef } from 'react';\nimport ReactFlow, {\n  MiniMap,\n  Controls,\n  Background,\n  useNodesState,\n  useEdgesState,\n  addEdge,\n  Node,\n  updateEdge,\n  Panel,\n  NodeChange,\n  EdgeChange,\n} from 'reactflow';\n// \ud83d\udc47 you need to import the reactflow styles\nimport 'reactflow/dist/style.css';\nimport Button from '@mui/material/Button';\nimport { useState, useEffect } from 'react';\nimport Stack from '@mui/material/Stack';\nimport { styled } from '@mui/material/styles';\nimport Paper from '@mui/material/Paper';\nimport { UIConfig, WorkflowDefinition, WorkflowStepDefinition, WorkflowSystemComponent} from 'types/WorkflowTypes';\nimport FormControl from '@mui/material/FormControl';\nimport InputLabel from '@mui/material/InputLabel';\nimport Select, { SelectChangeEvent } from '@mui/material/Select';\nimport { Box } from '@mui/system';\nimport MenuItem from '@mui/material/MenuItem';\nimport ToggleButtonGroup from '@mui/material/ToggleButtonGroup';\nimport ToggleButton from '@mui/material/ToggleButton';\nimport { getNeatApiRootUrl, getSelectedWorkflowName, setSelectedWorkflowName } from 'components/Utils';\nimport CdfPublisher from 'components/CdfPublisher';\nimport CdfDownloader from 'components/CdfDownloader';\nimport WorkflowExecutionReport from 'components/WorkflowExecutionReport';\nimport ConfigView from './ConfigView';\nimport TransformationTable from './TransformationView';\nimport QDataTable from './ExplorerView';\nimport Editor, { DiffEditor, useMonaco, loader } from '@monaco-editor/react';\nimport OverviewComponentEditorDialog from 'components/OverviewComponentEditorDialog';\nimport StepEditorDialog from 'components/StepEditorDialog';\n\nexport interface ExecutionLog {\n  id: string;\n  state: string;\n  elapsed_time: number;\n  timestamp: string;\n  error: string;\n  output_text: string;\n  data: any;\n}\n\nexport interface WorkflowStats {\n  state: string;\n  elapsed_time: number;\n  last_error: string;\n  execution_log: ExecutionLog[];\n}\n\nconst Item = styled(Paper)(({ theme }) => ({\n  backgroundColor: theme.palette.mode === 'dark' ? '#1A2027' : '#fff',\n  ...theme.typography.body2,\n  padding: theme.spacing(1),\n  textAlign: 'left',\n  color: theme.palette.text.secondary,\n}));\n\n\n\nexport default function WorkflowView() {\n  const neatApiRootUrl = getNeatApiRootUrl();\n  const edgeUpdateSuccessful = useRef(true);\n  const [nodes, setNodes, onNodesChange] = useNodesState([]);\n  const [edges, setEdges, onEdgesChange] = useEdgesState([]);\n  const [workflowStats, setWorkflowStats] = useState<WorkflowStats>();\n  const [timerInterval, setTimerInterval] = useState(null);\n  const [workflowDefinitions, setWorkflowDefinitions] = useState<WorkflowDefinition>();\n  const [selectedWorkflow, setSelectedWorkflow] = useState<string>(getSelectedWorkflowName());\n  const [listOfWorkflows, setListOfWorkflows] = useState<string[]>([]);\n  const [viewType, setViewType] = useState<string>(\"system\");\n  const [dialogOpen, setDialogOpen] = useState(false);\n  const [openOverviewComponentEditorDialog, setOpenOverviewComponentEditorDialog] = useState(false);\n  const [selectedStep, setSelectedStep] = useState<WorkflowStepDefinition>();\n  const [selectedComponent, setSelectedComponent] = useState<WorkflowSystemComponent>();\n  const [fileContent, setFileContent] = useState('');\n\n\n  useEffect(() => {\n    loadListOfWorkflows();\n    loadWorkflowDefinitions(getSelectedWorkflowName());\n    startStatePolling(selectedWorkflow);\n\n  }, []);\n\n  const fetchFileContent = async () => {\n    try {\n      var myHeaders = new Headers();\n      myHeaders.append('pragma', 'no-cache');\n      myHeaders.append('cache-control', 'no-cache');\n      const response = await fetch(neatApiRootUrl + '/data/workflows/' + selectedWorkflow + '/workflow.py', { method: \"get\", headers: myHeaders });\n      const content = await response.text();\n      setFileContent(content);\n    } catch (error) {\n      console.error('Error fetching file:', error);\n    }\n  };\n\n  useEffect(() => {\n    console.log(\"workflow definition changed\")\n    syncWorkflowDefToNodesAndEdges(viewType);\n  }, [workflowDefinitions]);\n\n  const startStatePolling = (workflowName:string) => {\n    if (timerInterval) {\n      clearInterval(timerInterval);\n    }\n    let newTimerInterval = setInterval(() => {\n      loadWorkflowStats(workflowName);\n    }, 2000);\n    setTimerInterval(newTimerInterval);\n  }\n\n  const stopStatePolling = () => {\n    clearInterval(timerInterval);\n  }\n\n  const loadListOfWorkflows = () => {\n    const url = neatApiRootUrl + \"/api/workflow/workflows\";\n    fetch(url).then((response) => response.json()).then((data) => {\n      setListOfWorkflows(data.workflows);\n    }).catch((error) => {\n      console.error('Error:', error);\n    }).finally(() => { });\n  }\n\n  const loadWorkflowDefinitions = (workflowName: string = \"\") => {\n    if (workflowName == \"\")\n      workflowName = selectedWorkflow;\n    const url = neatApiRootUrl + \"/api/workflow/workflow-definition/\" + workflowName;\n    fetch(url).then((response) => response.json()).then((data) => {\n      const workflows = WorkflowDefinition.fromJSON(data.definition);\n      setWorkflowDefinitions(workflows);\n      // loadWorkflowStats(workflowName);\n  }).catch ((error) => {\n    console.error('Error:', error);\n  }).finally(() => { });\n}\n\nconst filterStats = (stats: WorkflowStats) => {\n  console.log(\"loadWorkflowStats\")\n  console.dir(stats)\n  // detelete all log RUNNING entries that have both RUNNING and COMPLETED entries for the same step\n  if (stats.execution_log == null)\n    return stats;\n\n  const filteredLog = stats.execution_log!.filter((log, index) => {\n    if (log.state == \"STARTED\") {\n      const nextLog = stats.execution_log[index + 1];\n      if (nextLog && nextLog.state == \"COMPLETED\" && nextLog.id == log.id)\n        return false;\n    }\n    return true;\n  })\n  stats.execution_log = filteredLog;\n  return stats;\n}\n\nconst loadWorkflowStats = (workflowName: string = \"\") => {\n  if (workflowName == \"\")\n    workflowName = selectedWorkflow;\n  const url = neatApiRootUrl + \"/api/workflow/stats/\" + workflowName;\n  fetch(url).then((response) => response.json()).then((data) => {\n\n    // const filteredStats = filterStats(data);\n    setWorkflowStats(data);\n    if (data.state == \"RUNNING\") {\n      // startStatePolling();\n    } else if (data.state == \"COMPLETED\" || data.state == \"FAILED\") {\n      // stopStatePolling();\n    }\n\n  }).catch((error) => {\n    console.error('Error:', error);\n  })\n}\n\nconst startWorkflow = () => {\n  const url = neatApiRootUrl + \"/api/workflow/start\";\n  const params = { name: selectedWorkflow, config: \"\", start_step: \"\" };\n  fetch(url, {\n    method: \"post\", body: JSON.stringify(params), headers: {\n      'Content-Type': 'application/json;charset=utf-8'\n    }\n  }).then((response) => response.json()).then((data) => {\n    console.dir(data)\n    setWorkflowStats(data);\n    startStatePolling(selectedWorkflow);\n    loadWorkflowStats();\n  }).catch((error) => {\n    console.error('Error:', error);\n  })\n}\n\n\nconst saveWorkflow = () => {\n  console.dir(nodes);\n  syncNodesAndEdgesToWorkflowDef();\n  let wdef = workflowDefinitions;\n  console.dir(wdef);\n  const url = neatApiRootUrl + \"/api/workflow/workflow-definition/\" + selectedWorkflow;\n  fetch(url, {\n    method: \"post\", body: wdef.serializeToJson(), headers: {\n      'Content-Type': 'application/json;charset=utf-8'\n    }\n  }).then((response) => response.json()).then((data) => {\n    console.dir(data)\n  }\n  ).catch((error) => {\n    console.error('Error:', error);\n  })\n};\n\nconst syncNodesAndEdgesToWorkflowDef = () => {\n  if (workflowDefinitions) {\n    workflowDefinitions.updatePositions(nodes);\n    if (viewType == \"system\")\n      workflowDefinitions.updateSystemComponentTransitions(edges);\n    else\n      workflowDefinitions.updateStepTransitions(edges);\n  } else {\n    console.error(\"workflowDefinitions is null\");\n  }\n\n}\n\nconst syncWorkflowDefToNodesAndEdges = (viewType:string) => {\n  if (!workflowDefinitions)\n    return;\n  switch (viewType) {\n    case 'steps':\n      setNodes(workflowDefinitions.convertStepsToNodes());\n      setEdges(workflowDefinitions.convertStepsToEdges());\n      break;\n    case 'system':\n      setNodes(workflowDefinitions.convertSystemComponentsToNodes());\n      setEdges(workflowDefinitions.convertSystemComponentsToEdges());\n  }\n}\n\n\nconst reloadWorkflows = () => {\n  const url = neatApiRootUrl + \"/api/workflow/reload-workflows\";\n  fetch(url, {\n    method: \"post\", body: \"\", headers: {\n      'Content-Type': 'application/json;charset=utf-8'\n    }\n  }).then((response) => response.json()).then((data) => {\n    loadWorkflowDefinitions();\n  }\n  ).catch((error) => {\n    console.error('Error:', error);\n  })\n};\n\nconst handleWorkflowSelectorChange = (event: SelectChangeEvent) => {\n  console.dir(\"Workflow changed to :\" + event.target.value);\n  setSelectedWorkflowName(event.target.value);\n  setSelectedWorkflow(event.target.value);\n  loadWorkflowDefinitions(event.target.value);\n  setViewType(\"system\");\n  syncWorkflowDefToNodesAndEdges(\"system\");\n  startStatePolling(event.target.value);\n};\n\nconst handleViewTypeChange = (\n  event: React.MouseEvent<HTMLElement>,\n  newViewType: string,\n) => {\n\n  setViewType(newViewType);\n  syncWorkflowDefToNodesAndEdges(newViewType);\n  if (newViewType == \"src\") {\n    fetchFileContent();\n  }\n};\n\n\nconst onConnect = useCallback((params) => {\n  console.log('onConnect')\n  setEdges((eds) => addEdge(params, eds))\n  syncNodesAndEdgesToWorkflowDef();\n}, [setEdges]);\n\nconst onEdgeUpdateStart = useCallback(() => {\n  console.log('onEdgeUpdateStart')\n  edgeUpdateSuccessful.current = false;\n}, []);\n\nconst onEdgeUpdate = useCallback((oldEdge, newConnection) => {\n  console.log('onEdgeUpdate')\n  edgeUpdateSuccessful.current = true;\n  setEdges((els) => updateEdge(oldEdge, newConnection, els));\n}, [setEdges]);\n\nconst onEdgeUpdateEnd = useCallback((_, edge) => {\n  console.log('onEdgeUpdateEnd')\n  if (!edgeUpdateSuccessful.current) {\n    setEdges((eds) => eds.filter((e) => e.id !== edge.id));\n    syncNodesAndEdgesToWorkflowDef();\n  }\n\n  edgeUpdateSuccessful.current = true;\n}, [setEdges]);\n\nconst onNodeClick = useCallback((event, node) => {\n  console.log('onNodeClick')\n  console.dir(node);\n  handleDialogClickOpen(node.id, viewType);\n}, [workflowDefinitions, viewType]);\n\nconst onAddStep = (() => {\n  console.log('onAddStep')\n  const ui_config = new UIConfig();\n  ui_config.pos_x = 100;\n  ui_config.pos_y = 100;\n  if (viewType == \"steps\") {\n    const step = new WorkflowStepDefinition();\n    step.id = \"step_\" + Math.floor(Math.random() * 1000000);\n    step.label = \"New step\";\n    step.ui_config = ui_config;\n    workflowDefinitions.steps.push(step);\n  } else {\n    const systemComponent = new WorkflowSystemComponent();\n    systemComponent.id = \"system_comp_\" + Math.floor(Math.random() * 1000000);\n    systemComponent.label = \"New component\";\n    systemComponent.ui_config = ui_config;\n    if (workflowDefinitions.system_components == null)\n      workflowDefinitions.system_components = [];\n    workflowDefinitions.system_components.push(systemComponent);\n  }\n  syncWorkflowDefToNodesAndEdges(viewType);\n});\n\nconst handleDialogClickOpen = (id: string, viewType: string) => {\n  console.log(viewType);\n  if (viewType == \"steps\") {\n    setSelectedStep(workflowDefinitions.getStepById(id));\n    setDialogOpen(true);\n  } else {\n    setSelectedComponent(workflowDefinitions.getSystemComponentById(id));\n    setOpenOverviewComponentEditorDialog(true);\n  }\n};\n\nconst handleDialogClose = (step:WorkflowStepDefinition,action:string) => {\n  setDialogOpen(false);\n  switch (action) {\n    case \"delete\":\n      workflowDefinitions.deleteStep(selectedStep.id);\n      syncWorkflowDefToNodesAndEdges(viewType);\n      break;\n    case \"save\":\n      workflowDefinitions.updateStep(selectedStep.id, step);\n      setSelectedStep(step);\n      syncWorkflowDefToNodesAndEdges(viewType);\n      break;\n  }\n\n};\n\n\nconst onDownloadSuccess = (fileName: string, hash: string) => {\n  console.log(\"onDownloadSuccess\", fileName, hash)\n  reloadWorkflows();\n}\nconst solutionComponentEditorDialogHandler = (component: WorkflowSystemComponent,action: string) => {\n  console.log(\"OverviewComponentEditorDialogHandler\")\n  console.dir(component)\n  switch (action) {\n    case \"save\":\n      workflowDefinitions.updateSystemComponent(selectedComponent.id, component);\n      setSelectedComponent(component);\n      syncWorkflowDefToNodesAndEdges(viewType);\n      break;\n    case \"delete\":\n      workflowDefinitions.deleteSystemComponent(component.id);\n      syncWorkflowDefToNodesAndEdges(viewType);\n      break;\n  }\n  setOpenOverviewComponentEditorDialog(false);\n}\n\nconst onNodesChangeN = useCallback((nodeChanges: NodeChange[]) => {\n  // console.log('onNodesChange')\n  // console.dir(nodeChanges);\n  onNodesChange(nodeChanges);\n  syncNodesAndEdgesToWorkflowDef();\n}, [workflowDefinitions,nodes,edges]);\n\nconst onEdgesChangeN = useCallback((edgeChanges: EdgeChange[]) => {\n  console.log('onEdgesChange')\n  console.dir(edgeChanges);\n  onEdgesChange(edgeChanges);\n  syncNodesAndEdgesToWorkflowDef();\n}, [workflowDefinitions,nodes,edges]);\n\nreturn (\n  <div style={{ height: '85vh', width: '97vw' }}>\n    <Box>\n      <FormControl sx={{ width: 300, marginBottom: 2 }}>\n        <InputLabel id=\"workflowSelectorLabel\">Workflow selector</InputLabel>\n        <Select\n          labelId=\"workflowSelectorLabel\"\n          id=\"workflowSelector\"\n          value={selectedWorkflow}\n          size='small'\n          label=\"Query template\"\n          onChange={handleWorkflowSelectorChange}\n        >\n          {\n            listOfWorkflows && listOfWorkflows.map((item, i) => (\n              <MenuItem value={item} key={item}>{item} </MenuItem>\n            ))\n          }\n        </Select>\n      </FormControl>\n      <ToggleButtonGroup\n        color=\"primary\"\n        value={viewType}\n        exclusive\n        size='small'\n        sx={{ marginLeft: 2 }}\n        onChange={handleViewTypeChange}\n        aria-label=\"View type\"\n      >\n        <ToggleButton value=\"system\">Solution overview</ToggleButton>\n        <ToggleButton value=\"steps\">Workflow steps</ToggleButton>\n        <ToggleButton value=\"configurations\">Configurations</ToggleButton>\n        <ToggleButton value=\"src\">Source code</ToggleButton>\n        <ToggleButton value=\"transformations\">Transformation rules</ToggleButton>\n        <ToggleButton value=\"data_explorer\">Data explorer</ToggleButton>\n\n      </ToggleButtonGroup>\n    </Box>\n    {(viewType == \"system\" || viewType == \"steps\") && (\n      <Stack direction=\"row\" spacing={1} justifyContent=\"left\"\n        alignItems=\"left\">\n        <Item>\n          <OverviewComponentEditorDialog open={openOverviewComponentEditorDialog} component={selectedComponent} onClose={solutionComponentEditorDialogHandler} />\n          <StepEditorDialog open={dialogOpen} step={selectedStep} workflowName={selectedWorkflow} onClose={handleDialogClose} />\n          <div style={{ height: '75vh', width: '70vw' }}>\n            <ReactFlow\n              nodes={nodes}\n              edges={edges}\n              onNodeClick={onNodeClick}\n              onNodesChange={onNodesChangeN}\n              onEdgesChange={onEdgesChangeN}\n              onEdgeUpdate={onEdgeUpdate}\n              onEdgeUpdateStart={onEdgeUpdateStart}\n              onEdgeUpdateEnd={onEdgeUpdateEnd}\n              onConnect={onConnect}\n            >\n              <MiniMap />\n              <Controls />\n              <Background />\n              <Panel position=\"bottom-center\">\n              {viewType == \"system\" && (<Button variant=\"outlined\" onClick={onAddStep}>Add solution component</Button>)}\n              {viewType == \"steps\" && (<Button variant=\"outlined\" onClick={onAddStep}>Add workflow step</Button>)}\n              </Panel>\n            </ReactFlow>\n\n            <Button variant=\"outlined\" onClick={startWorkflow} sx={{ marginTop: 2, marginRight: 1 }}>Start workflow</Button>\n            <Button variant=\"outlined\" onClick={saveWorkflow} sx={{ marginTop: 2, marginRight: 1 }}>Save workflow</Button>\n            <Button variant=\"outlined\" onClick={reloadWorkflows} sx={{ marginTop: 2, marginRight: 1 }} >Reload local workflows</Button>\n            <Box sx={{ marginTop: 1, marginBottom: 1 }}>\n              <CdfPublisher type=\"workflow\" />\n              <CdfDownloader type=\"workflow-package\" onDownloadSuccess={onDownloadSuccess} />\n            </Box>\n          </div>\n\n        </Item>\n        <Item >\n          <WorkflowExecutionReport report={workflowStats} />\n        </Item>\n      </Stack>\n    )}\n    {viewType == \"configurations\" && (\n      <ConfigView></ConfigView>\n    )}\n    {viewType == \"transformations\" && (\n      <TransformationTable />\n    )}\n    {viewType == \"data_explorer\" && (\n      <QDataTable />\n    )}\n    {viewType == \"src\" && (\n      <Editor height=\"90vh\" defaultLanguage=\"python\" value={fileContent} />\n    )}\n\n  </div>\n\n\n);\n}\n",
         "import * as React from 'react';\nimport {useState,useEffect} from 'react';\n\nimport { DataGrid, GridColDef, GridRenderCellParams } from '@mui/x-data-grid';\nimport parsePrometheusTextFormat from 'parse-prometheus-text-format';\nimport Box from '@mui/material/Box';\nimport Collapse from '@mui/material/Collapse';\nimport IconButton from '@mui/material/IconButton';\nimport Table from '@mui/material/Table';\nimport TableBody from '@mui/material/TableBody';\nimport TableCell from '@mui/material/TableCell';\nimport TableContainer from '@mui/material/TableContainer';\nimport TableHead from '@mui/material/TableHead';\nimport TableRow from '@mui/material/TableRow';\nimport Typography from '@mui/material/Typography';\nimport Paper from '@mui/material/Paper';\nimport KeyboardArrowDownIcon from '@mui/icons-material/KeyboardArrowDown';\nimport KeyboardArrowUpIcon from '@mui/icons-material/KeyboardArrowUp';\nimport { convertMillisToStr, getNeatApiRootUrl } from 'components/Utils';\nimport WorkflowExecutionReport from 'components/WorkflowExecutionReport';\n\nfunction Row(props: { row: any }) {\n  const { row } = props;\n  const [open, setOpen] = React.useState(false);\n  const [activeRunId, setActiveRunId] = React.useState(\"\");\n  const [detailedExecutionReport, setDetailedExecutionReport] = React.useState(\"\");\n\n\n  const loadExecutionLog = () => {\n    setOpen(!open)\n    console.log(\"run_id: \"+row.run_id)\n\n  }\n\n  return (\n    <React.Fragment>\n      <TableRow sx={{ '& > *': { borderBottom: 'unset' } }}>\n        <TableCell>\n          <IconButton\n            aria-label=\"expand row\"\n            size=\"small\"\n            onClick={() => loadExecutionLog()}\n          >\n            {open ? <KeyboardArrowUpIcon /> : <KeyboardArrowDownIcon />}\n          </IconButton>\n        </TableCell>\n        <TableCell component=\"th\" scope=\"row\">\n          {row.workflow_name}\n        </TableCell>\n        <TableCell align=\"right\">{row.run_id}</TableCell>\n        <TableCell align=\"right\" style={{color: row.state == \"FAILED\" || row.state == \"EXPIRED\" ? \"red\" : \"green\"}}>{row.state}</TableCell>\n        <TableCell align=\"right\">{convertMillisToStr(row.start_time)}</TableCell>\n        <TableCell align=\"right\">{convertMillisToStr(row.end_time)}</TableCell>\n        <TableCell align=\"right\">{row.elapsed_time} sec</TableCell>\n      </TableRow>\n      <TableRow>\n        <TableCell style={{ paddingBottom: 0, paddingTop: 0 }} colSpan={6}>\n          <Collapse in={open} timeout=\"auto\" unmountOnExit>\n            <Box sx={{ margin: 1 }}>\n              <Typography variant=\"h6\" gutterBottom component=\"div\">\n                Detailed execution log\n              </Typography>\n              {open && (\n                <WorkflowExecutionReport report={row} run_id = {row.run_id}/>\n              )}\n\n            </Box>\n          </Collapse>\n        </TableCell>\n      </TableRow>\n    </React.Fragment>\n  );\n}\n\nexport default function ExecutionsTable() {\n  const neatApiRootUrl = getNeatApiRootUrl();\n  const [data, setData] = useState(Array<any>);\n\n  useEffect(() => {\n    loadDataset();\n  }, []);\n\n  const loadDataset = () => {\n    let url = neatApiRootUrl+\"/api/workflow/executions\"\n    fetch(url)\n    .then((response) => {\n      return response.json();\n    }).then((jdata) => {\n      setData(jdata.executions);\n\n    }\n  )}\n  return (\n    <div>\n    <TableContainer component={Paper}>\n      <Table aria-label=\"collapsible table\">\n        <TableHead>\n          <TableRow>\n            <TableCell />\n            <TableCell>Workflow name</TableCell>\n            <TableCell align=\"right\">Run id</TableCell>\n            <TableCell align=\"right\">State</TableCell>\n            <TableCell align=\"right\">Start time</TableCell>\n            <TableCell align=\"right\">End time</TableCell>\n            <TableCell align=\"right\">Duration</TableCell>\n          </TableRow>\n        </TableHead>\n        <TableBody>\n          {data.map((row:any) => (\n            <Row key={row.name} row={row} />\n          ))}\n        </TableBody>\n      </Table>\n\n    </TableContainer>\n    </div>\n  );\n}\n",
-        "import * as React from 'react';\nimport Box from '@mui/material/Box';\nimport Paper from '@mui/material/Paper';\nimport Stack from '@mui/material/Stack';\nimport { styled } from '@mui/material/styles';\nimport Button from '@mui/material/Button';\nimport TextField from '@mui/material/TextField';\nimport LinearProgress from '@mui/material/LinearProgress';\nimport { useState, useEffect } from 'react';\nimport { getNeatApiRootUrl } from 'components/Utils';\nimport FormControlLabel from '@mui/material/FormControlLabel';\nimport Switch from '@mui/material/Switch';\n\nconst Item = styled(Paper)(({ theme }) => ({\n  backgroundColor: theme.palette.mode === 'dark' ? '#1A2027' : '#fff',\n  ...theme.typography.body2,\n  padding: theme.spacing(1),\n  textAlign: 'left',\n  color: theme.palette.text.secondary,\n}));\n\nexport default function GlobalConfigView() {\n  const [loading, setLoading] = React.useState(false);\n  const [configs, setConfigs] = React.useState({\n    \"data_store_path\": \"\",\n    \"cdf_client\": {\n      \"project\": \"\",\n      \"client_id\": \"\",\n      \"client_name\": \"neat\",\n      \"base_url\": \"https://az-power-no-northeurope.cognitedata.com\",\n      \"scopes\": [\n        \"https://az-power-no-northeurope.cognitedata.com/.default\"\n      ],\n      \"token_url\": \"\",\n      \"client_secret\": \"\"\n    },\n    \"cdf_default_dataset_id\": 0,\n    \"load_examples\": true,\n    \"download_workflows_from_cdf\": false,\n    \"workflow_downloader_filter\": \"\",\n    \"log_level\": \"DEBUG\",\n    \"log_format\": \"%(asctime)s.%(msecs)03d %(levelname)-8s %(message)s\",\n    \"stop_on_error\": false\n  });\n\n  let initCdfResourcesResult:string = \"\";\n\n  const [neatApiRootUrl, setNeatApiRootUrl] = useState(getNeatApiRootUrl());\n\n  useEffect(() => {\n    loadConfigs();\n  }, []);\n\n  const loadConfigs = () => {\n    const url = neatApiRootUrl+\"/api/configs/global\";\n    fetch(url).then((response) => response.json()).then((data) => {\n      console.dir(data)\n      setConfigs(data)\n    }).catch((error) => {\n      console.error('Error:', error);\n    }).finally(() => { setLoading(false); });\n  }\n\n\n  const saveConfigButtonHandler = () => {\n    console.dir(configs);\n    setLoading(true);\n    let url = neatApiRootUrl+\"/api/configs/global\";\n\n    fetch(url, {\n      method: \"post\", body: JSON.stringify(configs), headers: {\n        'Content-Type': 'application/json;charset=utf-8'\n      }\n    }).then((response) => response.json()).then((data) => {\n      console.dir(data)\n    }).catch((error) => {\n      console.error('Error:', error);\n    }).finally(() => { setLoading(false); });\n  }\n\n  const saveNeatApiConfigButtonHandler = () => {\n    localStorage.setItem(\"neatApiRootUrl\", neatApiRootUrl);\n  }\n\n  const handleConfigChange = (name, value) => {\n    if (name == \"neatApiRootUrl\") {\n      setNeatApiRootUrl(value);\n    }else {\n      setConfigs({ ...configs, [name]: value });\n    }\n  };\n  const handleCdfConfigChange = (name, value) => {\n    let new_config  = {...configs};\n    new_config.cdf_client[name] = value;\n    setConfigs(new_config);\n  };\n\n  const initCdfResources = () => {\n    setLoading(true);\n    let url = neatApiRootUrl+\"/api/cdf/init-neat-resources\";\n    // send post request\n    fetch(url, {\n      method: \"post\"})\n      .then((response) => response.json())\n      .then((data) => {\n        console.dir(data)\n        initCdfResourcesResult = data.result;\n      }).catch((error) => {\n        console.error('Error:', error);\n        initCdfResourcesResult = \"Error: \"+error;\n      }).finally(() => { setLoading(false); });\n  }\n\n  return (\n    <Box sx={{ width: \"70%\" }}>\n      <Stack spacing={2}>\n        <Item>\n          <h3>Global configurations</h3>\n          <Box sx={{ minWidth: 200 }}>\n            <Stack spacing={2} direction=\"column\">\n              <h4>CDF configurations</h4>\n              <TextField id=\"project_name\" label=\"Project name\" size='small' variant=\"outlined\" value={configs.cdf_client.project} onChange={(event) => { handleCdfConfigChange(\"project\", event.target.value) }} />\n              <TextField id=\"client_id\" label=\"Client id\" size='small' variant=\"outlined\" value={configs.cdf_client.client_id} onChange={(event) => { handleCdfConfigChange(\"client_id\", event.target.value) }} />\n              <TextField id=\"client_secret\" label=\"Client secret\" type=\"password\" size='small' variant=\"outlined\" value={configs.cdf_client.client_secret} onChange={(event) => { handleCdfConfigChange(\"client_secret\", event.target.value) }} />\n              <TextField id=\"client_name\" label=\"Client name\" size='small' variant=\"outlined\" value={configs.cdf_client.client_name} onChange={(event) => { handleCdfConfigChange(\"client_name\", event.target.value) }} />\n              <TextField id=\"cdf_api_base_url\" label=\"CDF api base url\" size='small' variant=\"outlined\" value={configs.cdf_client.base_url} onChange={(event) => { handleCdfConfigChange(\"base_url\", event.target.value) }} />\n              <TextField id=\"scopes\" label=\"Scopes\" size='small' variant=\"outlined\" value={configs.cdf_client.scopes} onChange={(event) => { handleCdfConfigChange(\"scopes\", event.target.value) }} />\n              <TextField id=\"oidc_token_url\" label=\"OIDC token url\" size='small' variant=\"outlined\" value={configs.cdf_client.token_url} onChange={(event) => { handleCdfConfigChange(\"token_url\", event.target.value) }} />\n              <TextField id=\"cdf_default_dataset_id\" type=\"number\"  label=\"Default CDF dataset id.The dataset is used as workflow and rules storage.\" size='small' variant=\"outlined\" value={configs.cdf_default_dataset_id} onChange={(event) => { handleConfigChange(\"cdf_default_dataset_id\", event.target.value) }} />\n              <h4>Storage and workflows</h4>\n              <TextField id=\"data_store_path\" label=\"Data directory.Is used as local workflow , rules and db storage.\" size='small' variant=\"outlined\" value={configs.data_store_path} onChange={(event) => { handleConfigChange(\"data_store_path\", event.target.value) }} />\n              <FormControlLabel control={<Switch checked={configs.download_workflows_from_cdf} onChange={(event) => { handleConfigChange(\"download_workflows_from_cdf\", event.target.checked) }} />} label=\"Automatically download workflows from CDF on startup\"  />\n              <TextField id=\"workflow_downloader_filter\" label=\"List of workflows or filters that will be used for downloading workflows\" size='small' variant=\"outlined\" value={configs.workflow_downloader_filter} onChange={(event) => { handleConfigChange(\"workflow_downloader_filter\", event.target.value) }} />\n              <FormControlLabel control={<Switch checked={configs.load_examples} onChange={(event) => { handleConfigChange(\"load_examples\", event.target.checked) }} />} label=\"Load default examples\"  />\n              <TextField id=\"log_level\" label=\"Log level\" size='small' variant=\"outlined\" value={configs.log_level} onChange={(event) => { handleConfigChange(\"log_level\", event.target.value) }} />\n              <Button variant=\"contained\" onClick={saveConfigButtonHandler}>Save</Button>\n              {loading && (<LinearProgress />)}\n            </Stack>\n          </Box>\n          <h3>NEAT UI configuration</h3>\n          <Box sx={{ minWidth: 120 }}>\n            <Stack spacing={2} direction=\"column\">\n              <TextField id=\"neat_api_root_url\" label=\"API root url\" size='small' variant=\"outlined\" value={neatApiRootUrl} onChange={(event) => { handleConfigChange(\"neatApiRootUrl\", event.target.value) }} />\n              <Button variant=\"contained\" onClick={saveNeatApiConfigButtonHandler}>Save</Button>\n            </Stack>\n          </Box>\n          <h3>Neat internal CDF resources (used for storing files and execution history)</h3>\n\n          <Button variant=\"contained\" onClick={initCdfResources}>Initialize CDF resources</Button>\n\n        </Item>\n\n\n      </Stack>\n    </Box>\n  );\n}\n",
+        "import * as React from 'react';\nimport Box from '@mui/material/Box';\nimport Paper from '@mui/material/Paper';\nimport Stack from '@mui/material/Stack';\nimport { styled } from '@mui/material/styles';\nimport Button from '@mui/material/Button';\nimport TextField from '@mui/material/TextField';\nimport LinearProgress from '@mui/material/LinearProgress';\nimport { useState, useEffect } from 'react';\nimport { getNeatApiRootUrl } from 'components/Utils';\nimport FormControlLabel from '@mui/material/FormControlLabel';\nimport Switch from '@mui/material/Switch';\n\nconst Item = styled(Paper)(({ theme }) => ({\n  backgroundColor: theme.palette.mode === 'dark' ? '#1A2027' : '#fff',\n  ...theme.typography.body2,\n  padding: theme.spacing(1),\n  textAlign: 'left',\n  color: theme.palette.text.secondary,\n}));\n\nexport default function GlobalConfigView() {\n  const [loading, setLoading] = React.useState(false);\n  const [configs, setConfigs] = React.useState({\n    \"data_store_path\": \"\",\n    \"cdf_client\": {\n      \"project\": \"\",\n      \"client_id\": \"\",\n      \"client_name\": \"neat\",\n      \"base_url\": \"https://az-power-no-northeurope.cognitedata.com\",\n      \"scopes\": [\n        \"https://az-power-no-northeurope.cognitedata.com/.default\"\n      ],\n      \"token_url\": \"\",\n      \"client_secret\": \"\",\n      \"timeout\": 60,\n      \"max_workers\": 3,\n\n    },\n    \"cdf_default_dataset_id\": 0,\n    \"load_examples\": true,\n    \"download_workflows_from_cdf\": false,\n    \"workflow_downloader_filter\": \"\",\n    \"log_level\": \"DEBUG\",\n    \"log_format\": \"%(asctime)s.%(msecs)03d %(levelname)-8s %(message)s\",\n    \"stop_on_error\": false\n  });\n\n  let initCdfResourcesResult:string = \"\";\n\n  const [neatApiRootUrl, setNeatApiRootUrl] = useState(getNeatApiRootUrl());\n\n  useEffect(() => {\n    loadConfigs();\n  }, []);\n\n  const loadConfigs = () => {\n    const url = neatApiRootUrl+\"/api/configs/global\";\n    fetch(url).then((response) => response.json()).then((data) => {\n      console.dir(data)\n      setConfigs(data)\n    }).catch((error) => {\n      console.error('Error:', error);\n    }).finally(() => { setLoading(false); });\n  }\n\n\n  const saveConfigButtonHandler = () => {\n    console.dir(configs);\n    setLoading(true);\n    let url = neatApiRootUrl+\"/api/configs/global\";\n\n    fetch(url, {\n      method: \"post\", body: JSON.stringify(configs), headers: {\n        'Content-Type': 'application/json;charset=utf-8'\n      }\n    }).then((response) => response.json()).then((data) => {\n      console.dir(data)\n    }).catch((error) => {\n      console.error('Error:', error);\n    }).finally(() => { setLoading(false); });\n  }\n\n  const saveNeatApiConfigButtonHandler = () => {\n    localStorage.setItem(\"neatApiRootUrl\", neatApiRootUrl);\n  }\n\n  const handleConfigChange = (name, value) => {\n    if (name == \"neatApiRootUrl\") {\n      setNeatApiRootUrl(value);\n    }else {\n      setConfigs({ ...configs, [name]: value });\n    }\n  };\n  const handleCdfConfigChange = (name, value) => {\n    let new_config  = {...configs};\n    new_config.cdf_client[name] = value;\n    setConfigs(new_config);\n  };\n\n  const initCdfResources = () => {\n    setLoading(true);\n    let url = neatApiRootUrl+\"/api/cdf/init-neat-resources\";\n    // send post request\n    fetch(url, {\n      method: \"post\"})\n      .then((response) => response.json())\n      .then((data) => {\n        console.dir(data)\n        initCdfResourcesResult = data.result;\n      }).catch((error) => {\n        console.error('Error:', error);\n        initCdfResourcesResult = \"Error: \"+error;\n      }).finally(() => { setLoading(false); });\n  }\n\n  return (\n    <Box sx={{ width: \"70%\" }}>\n      <Stack spacing={2}>\n        <Item>\n          <h3>Global configurations</h3>\n          <Box sx={{ minWidth: 200 }}>\n            <Stack spacing={2} direction=\"column\">\n              <h4>CDF configurations</h4>\n              <TextField id=\"project_name\" label=\"Project name\" size='small' variant=\"outlined\" value={configs.cdf_client.project} onChange={(event) => { handleCdfConfigChange(\"project\", event.target.value) }} />\n              <TextField id=\"client_id\" label=\"Client id\" size='small' variant=\"outlined\" value={configs.cdf_client.client_id} onChange={(event) => { handleCdfConfigChange(\"client_id\", event.target.value) }} />\n              <TextField id=\"client_secret\" label=\"Client secret\" type=\"password\" size='small' variant=\"outlined\" value={configs.cdf_client.client_secret} onChange={(event) => { handleCdfConfigChange(\"client_secret\", event.target.value) }} />\n              <TextField id=\"client_name\" label=\"Client name\" size='small' variant=\"outlined\" value={configs.cdf_client.client_name} onChange={(event) => { handleCdfConfigChange(\"client_name\", event.target.value) }} />\n              <TextField id=\"cdf_api_base_url\" label=\"CDF api base url\" size='small' variant=\"outlined\" value={configs.cdf_client.base_url} onChange={(event) => { handleCdfConfigChange(\"base_url\", event.target.value) }} />\n              <TextField id=\"scopes\" label=\"Scopes\" size='small' variant=\"outlined\" value={configs.cdf_client.scopes} onChange={(event) => { handleCdfConfigChange(\"scopes\", event.target.value) }} />\n              <TextField id=\"oidc_token_url\" label=\"OIDC token url\" size='small' variant=\"outlined\" value={configs.cdf_client.token_url} onChange={(event) => { handleCdfConfigChange(\"token_url\", event.target.value) }} />\n              <TextField id=\"cdf_default_dataset_id\" type=\"number\"  label=\"Default CDF dataset id.The dataset is used as workflow and rules storage.\" size='small' variant=\"outlined\" value={configs.cdf_default_dataset_id} onChange={(event) => { handleConfigChange(\"cdf_default_dataset_id\", event.target.value) }} />\n              <TextField id=\"cdf_timeout\" type=\"number\"  label=\"Cdf read timeout in seconds.\" size='small' variant=\"outlined\" value={configs.cdf_client.timeout} onChange={(event) => { handleCdfConfigChange(\"timeout\", event.target.value) }} />\n              <TextField id=\"cdf_max_workers\" type=\"number\"  label=\"Max number of client workers.\" size='small' variant=\"outlined\" value={configs.cdf_client.max_workers} onChange={(event) => { handleCdfConfigChange(\"max_workers\", event.target.value) }} />\n              \n              <h4>Storage and workflows</h4>\n              <TextField id=\"data_store_path\" label=\"Data directory.Is used as local workflow , rules and db storage.\" size='small' variant=\"outlined\" value={configs.data_store_path} onChange={(event) => { handleConfigChange(\"data_store_path\", event.target.value) }} />\n              <FormControlLabel control={<Switch checked={configs.download_workflows_from_cdf} onChange={(event) => { handleConfigChange(\"download_workflows_from_cdf\", event.target.checked) }} />} label=\"Automatically download workflows from CDF on startup\"  />\n              <TextField id=\"workflow_downloader_filter\" label=\"List of workflows or filters that will be used for downloading workflows\" size='small' variant=\"outlined\" value={configs.workflow_downloader_filter} onChange={(event) => { handleConfigChange(\"workflow_downloader_filter\", event.target.value) }} />\n              <FormControlLabel control={<Switch checked={configs.load_examples} onChange={(event) => { handleConfigChange(\"load_examples\", event.target.checked) }} />} label=\"Load default examples\"  />\n              <TextField id=\"log_level\" label=\"Log level\" size='small' variant=\"outlined\" value={configs.log_level} onChange={(event) => { handleConfigChange(\"log_level\", event.target.value) }} />\n              <Button variant=\"contained\" onClick={saveConfigButtonHandler}>Save</Button>\n              {loading && (<LinearProgress />)}\n            </Stack>\n          </Box>\n          <h3>NEAT UI configuration</h3>\n          <Box sx={{ minWidth: 120 }}>\n            <Stack spacing={2} direction=\"column\">\n              <TextField id=\"neat_api_root_url\" label=\"API root url\" size='small' variant=\"outlined\" value={neatApiRootUrl} onChange={(event) => { handleConfigChange(\"neatApiRootUrl\", event.target.value) }} />\n              <Button variant=\"contained\" onClick={saveNeatApiConfigButtonHandler}>Save</Button>\n            </Stack>\n          </Box>\n          <h3>Neat internal CDF resources (used for storing files and execution history)</h3>\n\n          <Button variant=\"contained\" onClick={initCdfResources}>Initialize CDF resources</Button>\n\n        </Item>\n\n\n      </Stack>\n    </Box>\n  );\n}\n",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getListItemUtilityClass(slot) {\n  return generateUtilityClass('MuiListItem', slot);\n}\nconst listItemClasses = generateUtilityClasses('MuiListItem', ['root', 'container', 'focusVisible', 'dense', 'alignItemsFlexStart', 'disabled', 'divider', 'gutters', 'padding', 'button', 'secondaryAction', 'selected']);\nexport default listItemClasses;",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getListItemButtonUtilityClass(slot) {\n  return generateUtilityClass('MuiListItemButton', slot);\n}\nconst listItemButtonClasses = generateUtilityClasses('MuiListItemButton', ['root', 'focusVisible', 'dense', 'alignItemsFlexStart', 'disabled', 'divider', 'gutters', 'selected']);\nexport default listItemButtonClasses;",
         "import { unstable_generateUtilityClasses as generateUtilityClasses } from '@mui/utils';\nimport generateUtilityClass from '../generateUtilityClass';\nexport function getListItemSecondaryActionClassesUtilityClass(slot) {\n  return generateUtilityClass('MuiListItemSecondaryAction', slot);\n}\nconst listItemSecondaryActionClasses = generateUtilityClasses('MuiListItemSecondaryAction', ['root', 'disableGutters']);\nexport default listItemSecondaryActionClasses;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"className\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport styled from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\nimport ListContext from '../List/ListContext';\nimport { getListItemSecondaryActionClassesUtilityClass } from './listItemSecondaryActionClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst useUtilityClasses = ownerState => {\n  const {\n    disableGutters,\n    classes\n  } = ownerState;\n  const slots = {\n    root: ['root', disableGutters && 'disableGutters']\n  };\n  return composeClasses(slots, getListItemSecondaryActionClassesUtilityClass, classes);\n};\nconst ListItemSecondaryActionRoot = styled('div', {\n  name: 'MuiListItemSecondaryAction',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.root, ownerState.disableGutters && styles.disableGutters];\n  }\n})(({\n  ownerState\n}) => _extends({\n  position: 'absolute',\n  right: 16,\n  top: '50%',\n  transform: 'translateY(-50%)'\n}, ownerState.disableGutters && {\n  right: 0\n}));\n\n/**\n * Must be used as the last child of ListItem to function properly.\n */\nconst ListItemSecondaryAction = /*#__PURE__*/React.forwardRef(function ListItemSecondaryAction(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiListItemSecondaryAction'\n  });\n  const {\n      className\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const context = React.useContext(ListContext);\n  const ownerState = _extends({}, props, {\n    disableGutters: context.disableGutters\n  });\n  const classes = useUtilityClasses(ownerState);\n  return /*#__PURE__*/_jsx(ListItemSecondaryActionRoot, _extends({\n    className: clsx(classes.root, className),\n    ownerState: ownerState,\n    ref: ref\n  }, other));\n});\nprocess.env.NODE_ENV !== \"production\" ? ListItemSecondaryAction.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * The content of the component, normally an `IconButton` or selection control.\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nListItemSecondaryAction.muiName = 'ListItemSecondaryAction';\nexport default ListItemSecondaryAction;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"className\"],\n  _excluded2 = [\"alignItems\", \"autoFocus\", \"button\", \"children\", \"className\", \"component\", \"components\", \"componentsProps\", \"ContainerComponent\", \"ContainerProps\", \"dense\", \"disabled\", \"disableGutters\", \"disablePadding\", \"divider\", \"focusVisibleClassName\", \"secondaryAction\", \"selected\", \"slotProps\", \"slots\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { unstable_composeClasses as composeClasses, isHostComponent } from '@mui/base';\nimport { chainPropTypes, elementTypeAcceptingRef } from '@mui/utils';\nimport { alpha } from '@mui/system';\nimport styled from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\nimport ButtonBase from '../ButtonBase';\nimport isMuiElement from '../utils/isMuiElement';\nimport useEnhancedEffect from '../utils/useEnhancedEffect';\nimport useForkRef from '../utils/useForkRef';\nimport ListContext from '../List/ListContext';\nimport listItemClasses, { getListItemUtilityClass } from './listItemClasses';\nimport { listItemButtonClasses } from '../ListItemButton';\nimport ListItemSecondaryAction from '../ListItemSecondaryAction';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\nexport const overridesResolver = (props, styles) => {\n  const {\n    ownerState\n  } = props;\n  return [styles.root, ownerState.dense && styles.dense, ownerState.alignItems === 'flex-start' && styles.alignItemsFlexStart, ownerState.divider && styles.divider, !ownerState.disableGutters && styles.gutters, !ownerState.disablePadding && styles.padding, ownerState.button && styles.button, ownerState.hasSecondaryAction && styles.secondaryAction];\n};\nconst useUtilityClasses = ownerState => {\n  const {\n    alignItems,\n    button,\n    classes,\n    dense,\n    disabled,\n    disableGutters,\n    disablePadding,\n    divider,\n    hasSecondaryAction,\n    selected\n  } = ownerState;\n  const slots = {\n    root: ['root', dense && 'dense', !disableGutters && 'gutters', !disablePadding && 'padding', divider && 'divider', disabled && 'disabled', button && 'button', alignItems === 'flex-start' && 'alignItemsFlexStart', hasSecondaryAction && 'secondaryAction', selected && 'selected'],\n    container: ['container']\n  };\n  return composeClasses(slots, getListItemUtilityClass, classes);\n};\nexport const ListItemRoot = styled('div', {\n  name: 'MuiListItem',\n  slot: 'Root',\n  overridesResolver\n})(({\n  theme,\n  ownerState\n}) => _extends({\n  display: 'flex',\n  justifyContent: 'flex-start',\n  alignItems: 'center',\n  position: 'relative',\n  textDecoration: 'none',\n  width: '100%',\n  boxSizing: 'border-box',\n  textAlign: 'left'\n}, !ownerState.disablePadding && _extends({\n  paddingTop: 8,\n  paddingBottom: 8\n}, ownerState.dense && {\n  paddingTop: 4,\n  paddingBottom: 4\n}, !ownerState.disableGutters && {\n  paddingLeft: 16,\n  paddingRight: 16\n}, !!ownerState.secondaryAction && {\n  // Add some space to avoid collision as `ListItemSecondaryAction`\n  // is absolutely positioned.\n  paddingRight: 48\n}), !!ownerState.secondaryAction && {\n  [`& > .${listItemButtonClasses.root}`]: {\n    paddingRight: 48\n  }\n}, {\n  [`&.${listItemClasses.focusVisible}`]: {\n    backgroundColor: (theme.vars || theme).palette.action.focus\n  },\n  [`&.${listItemClasses.selected}`]: {\n    backgroundColor: theme.vars ? `rgba(${theme.vars.palette.primary.mainChannel} / ${theme.vars.palette.action.selectedOpacity})` : alpha(theme.palette.primary.main, theme.palette.action.selectedOpacity),\n    [`&.${listItemClasses.focusVisible}`]: {\n      backgroundColor: theme.vars ? `rgba(${theme.vars.palette.primary.mainChannel} / calc(${theme.vars.palette.action.selectedOpacity} + ${theme.vars.palette.action.focusOpacity}))` : alpha(theme.palette.primary.main, theme.palette.action.selectedOpacity + theme.palette.action.focusOpacity)\n    }\n  },\n  [`&.${listItemClasses.disabled}`]: {\n    opacity: (theme.vars || theme).palette.action.disabledOpacity\n  }\n}, ownerState.alignItems === 'flex-start' && {\n  alignItems: 'flex-start'\n}, ownerState.divider && {\n  borderBottom: `1px solid ${(theme.vars || theme).palette.divider}`,\n  backgroundClip: 'padding-box'\n}, ownerState.button && {\n  transition: theme.transitions.create('background-color', {\n    duration: theme.transitions.duration.shortest\n  }),\n  '&:hover': {\n    textDecoration: 'none',\n    backgroundColor: (theme.vars || theme).palette.action.hover,\n    // Reset on touch devices, it doesn't add specificity\n    '@media (hover: none)': {\n      backgroundColor: 'transparent'\n    }\n  },\n  [`&.${listItemClasses.selected}:hover`]: {\n    backgroundColor: theme.vars ? `rgba(${theme.vars.palette.primary.mainChannel} / calc(${theme.vars.palette.action.selectedOpacity} + ${theme.vars.palette.action.hoverOpacity}))` : alpha(theme.palette.primary.main, theme.palette.action.selectedOpacity + theme.palette.action.hoverOpacity),\n    // Reset on touch devices, it doesn't add specificity\n    '@media (hover: none)': {\n      backgroundColor: theme.vars ? `rgba(${theme.vars.palette.primary.mainChannel} / ${theme.vars.palette.action.selectedOpacity})` : alpha(theme.palette.primary.main, theme.palette.action.selectedOpacity)\n    }\n  }\n}, ownerState.hasSecondaryAction && {\n  // Add some space to avoid collision as `ListItemSecondaryAction`\n  // is absolutely positioned.\n  paddingRight: 48\n}));\nconst ListItemContainer = styled('li', {\n  name: 'MuiListItem',\n  slot: 'Container',\n  overridesResolver: (props, styles) => styles.container\n})({\n  position: 'relative'\n});\n\n/**\n * Uses an additional container component if `ListItemSecondaryAction` is the last child.\n */\nconst ListItem = /*#__PURE__*/React.forwardRef(function ListItem(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiListItem'\n  });\n  const {\n      alignItems = 'center',\n      autoFocus = false,\n      button = false,\n      children: childrenProp,\n      className,\n      component: componentProp,\n      components = {},\n      componentsProps = {},\n      ContainerComponent = 'li',\n      ContainerProps: {\n        className: ContainerClassName\n      } = {},\n      dense = false,\n      disabled = false,\n      disableGutters = false,\n      disablePadding = false,\n      divider = false,\n      focusVisibleClassName,\n      secondaryAction,\n      selected = false,\n      slotProps = {},\n      slots = {}\n    } = props,\n    ContainerProps = _objectWithoutPropertiesLoose(props.ContainerProps, _excluded),\n    other = _objectWithoutPropertiesLoose(props, _excluded2);\n  const context = React.useContext(ListContext);\n  const childContext = React.useMemo(() => ({\n    dense: dense || context.dense || false,\n    alignItems,\n    disableGutters\n  }), [alignItems, context.dense, dense, disableGutters]);\n  const listItemRef = React.useRef(null);\n  useEnhancedEffect(() => {\n    if (autoFocus) {\n      if (listItemRef.current) {\n        listItemRef.current.focus();\n      } else if (process.env.NODE_ENV !== 'production') {\n        console.error('MUI: Unable to set focus to a ListItem whose component has not been rendered.');\n      }\n    }\n  }, [autoFocus]);\n  const children = React.Children.toArray(childrenProp);\n\n  // v4 implementation, deprecated in v5, will be removed in v6\n  const hasSecondaryAction = children.length && isMuiElement(children[children.length - 1], ['ListItemSecondaryAction']);\n  const ownerState = _extends({}, props, {\n    alignItems,\n    autoFocus,\n    button,\n    dense: childContext.dense,\n    disabled,\n    disableGutters,\n    disablePadding,\n    divider,\n    hasSecondaryAction,\n    selected\n  });\n  const classes = useUtilityClasses(ownerState);\n  const handleRef = useForkRef(listItemRef, ref);\n  const Root = slots.root || components.Root || ListItemRoot;\n  const rootProps = slotProps.root || componentsProps.root || {};\n  const componentProps = _extends({\n    className: clsx(classes.root, rootProps.className, className),\n    disabled\n  }, other);\n  let Component = componentProp || 'li';\n  if (button) {\n    componentProps.component = componentProp || 'div';\n    componentProps.focusVisibleClassName = clsx(listItemClasses.focusVisible, focusVisibleClassName);\n    Component = ButtonBase;\n  }\n\n  // v4 implementation, deprecated in v5, will be removed in v6\n  if (hasSecondaryAction) {\n    // Use div by default.\n    Component = !componentProps.component && !componentProp ? 'div' : Component;\n\n    // Avoid nesting of li > li.\n    if (ContainerComponent === 'li') {\n      if (Component === 'li') {\n        Component = 'div';\n      } else if (componentProps.component === 'li') {\n        componentProps.component = 'div';\n      }\n    }\n    return /*#__PURE__*/_jsx(ListContext.Provider, {\n      value: childContext,\n      children: /*#__PURE__*/_jsxs(ListItemContainer, _extends({\n        as: ContainerComponent,\n        className: clsx(classes.container, ContainerClassName),\n        ref: handleRef,\n        ownerState: ownerState\n      }, ContainerProps, {\n        children: [/*#__PURE__*/_jsx(Root, _extends({}, rootProps, !isHostComponent(Root) && {\n          as: Component,\n          ownerState: _extends({}, ownerState, rootProps.ownerState)\n        }, componentProps, {\n          children: children\n        })), children.pop()]\n      }))\n    });\n  }\n  return /*#__PURE__*/_jsx(ListContext.Provider, {\n    value: childContext,\n    children: /*#__PURE__*/_jsxs(Root, _extends({}, rootProps, {\n      as: Component,\n      ref: handleRef\n    }, !isHostComponent(Root) && {\n      ownerState: _extends({}, ownerState, rootProps.ownerState)\n    }, componentProps, {\n      children: [children, secondaryAction && /*#__PURE__*/_jsx(ListItemSecondaryAction, {\n        children: secondaryAction\n      })]\n    }))\n  });\n});\nprocess.env.NODE_ENV !== \"production\" ? ListItem.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * Defines the `align-items` style property.\n   * @default 'center'\n   */\n  alignItems: PropTypes.oneOf(['center', 'flex-start']),\n  /**\n   * If `true`, the list item is focused during the first mount.\n   * Focus will also be triggered if the value changes from false to true.\n   * @default false\n   * @deprecated checkout [ListItemButton](/material-ui/api/list-item-button/) instead\n   */\n  autoFocus: PropTypes.bool,\n  /**\n   * If `true`, the list item is a button (using `ButtonBase`). Props intended\n   * for `ButtonBase` can then be applied to `ListItem`.\n   * @default false\n   * @deprecated checkout [ListItemButton](/material-ui/api/list-item-button/) instead\n   */\n  button: PropTypes.bool,\n  /**\n   * The content of the component if a `ListItemSecondaryAction` is used it must\n   * be the last child.\n   */\n  children: chainPropTypes(PropTypes.node, props => {\n    const children = React.Children.toArray(props.children);\n\n    // React.Children.toArray(props.children).findLastIndex(isListItemSecondaryAction)\n    let secondaryActionIndex = -1;\n    for (let i = children.length - 1; i >= 0; i -= 1) {\n      const child = children[i];\n      if (isMuiElement(child, ['ListItemSecondaryAction'])) {\n        secondaryActionIndex = i;\n        break;\n      }\n    }\n\n    //  is ListItemSecondaryAction the last child of ListItem\n    if (secondaryActionIndex !== -1 && secondaryActionIndex !== children.length - 1) {\n      return new Error('MUI: You used an element after ListItemSecondaryAction. ' + 'For ListItem to detect that it has a secondary action ' + 'you must pass it as the last child to ListItem.');\n    }\n    return null;\n  }),\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: PropTypes.elementType,\n  /**\n   * The components used for each slot inside.\n   *\n   * This prop is an alias for the `slots` prop.\n   * It's recommended to use the `slots` prop instead.\n   *\n   * @default {}\n   */\n  components: PropTypes.shape({\n    Root: PropTypes.elementType\n  }),\n  /**\n   * The extra props for the slot components.\n   * You can override the existing props or add new ones.\n   *\n   * This prop is an alias for the `slotProps` prop.\n   * It's recommended to use the `slotProps` prop instead, as `componentsProps` will be deprecated in the future.\n   *\n   * @default {}\n   */\n  componentsProps: PropTypes.shape({\n    root: PropTypes.object\n  }),\n  /**\n   * The container component used when a `ListItemSecondaryAction` is the last child.\n   * @default 'li'\n   * @deprecated\n   */\n  ContainerComponent: elementTypeAcceptingRef,\n  /**\n   * Props applied to the container component if used.\n   * @default {}\n   * @deprecated\n   */\n  ContainerProps: PropTypes.object,\n  /**\n   * If `true`, compact vertical padding designed for keyboard and mouse input is used.\n   * The prop defaults to the value inherited from the parent List component.\n   * @default false\n   */\n  dense: PropTypes.bool,\n  /**\n   * If `true`, the component is disabled.\n   * @default false\n   * @deprecated checkout [ListItemButton](/material-ui/api/list-item-button/) instead\n   */\n  disabled: PropTypes.bool,\n  /**\n   * If `true`, the left and right padding is removed.\n   * @default false\n   */\n  disableGutters: PropTypes.bool,\n  /**\n   * If `true`, all padding is removed.\n   * @default false\n   */\n  disablePadding: PropTypes.bool,\n  /**\n   * If `true`, a 1px light border is added to the bottom of the list item.\n   * @default false\n   */\n  divider: PropTypes.bool,\n  /**\n   * @ignore\n   */\n  focusVisibleClassName: PropTypes.string,\n  /**\n   * The element to display at the end of ListItem.\n   */\n  secondaryAction: PropTypes.node,\n  /**\n   * Use to apply selected styling.\n   * @default false\n   * @deprecated checkout [ListItemButton](/material-ui/api/list-item-button/) instead\n   */\n  selected: PropTypes.bool,\n  /**\n   * The extra props for the slot components.\n   * You can override the existing props or add new ones.\n   *\n   * This prop is an alias for the `componentsProps` prop, which will be deprecated in the future.\n   *\n   * @default {}\n   */\n  slotProps: PropTypes.shape({\n    root: PropTypes.object\n  }),\n  /**\n   * The components used for each slot inside.\n   *\n   * This prop is an alias for the `components` prop, which will be deprecated in the future.\n   *\n   * @default {}\n   */\n  slots: PropTypes.shape({\n    root: PropTypes.elementType\n  }),\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nexport default ListItem;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"children\", \"className\", \"disableTypography\", \"inset\", \"primary\", \"primaryTypographyProps\", \"secondary\", \"secondaryTypographyProps\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport Typography from '../Typography';\nimport ListContext from '../List/ListContext';\nimport useThemeProps from '../styles/useThemeProps';\nimport styled from '../styles/styled';\nimport listItemTextClasses, { getListItemTextUtilityClass } from './listItemTextClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\nconst useUtilityClasses = ownerState => {\n  const {\n    classes,\n    inset,\n    primary,\n    secondary,\n    dense\n  } = ownerState;\n  const slots = {\n    root: ['root', inset && 'inset', dense && 'dense', primary && secondary && 'multiline'],\n    primary: ['primary'],\n    secondary: ['secondary']\n  };\n  return composeClasses(slots, getListItemTextUtilityClass, classes);\n};\nconst ListItemTextRoot = styled('div', {\n  name: 'MuiListItemText',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [{\n      [`& .${listItemTextClasses.primary}`]: styles.primary\n    }, {\n      [`& .${listItemTextClasses.secondary}`]: styles.secondary\n    }, styles.root, ownerState.inset && styles.inset, ownerState.primary && ownerState.secondary && styles.multiline, ownerState.dense && styles.dense];\n  }\n})(({\n  ownerState\n}) => _extends({\n  flex: '1 1 auto',\n  minWidth: 0,\n  marginTop: 4,\n  marginBottom: 4\n}, ownerState.primary && ownerState.secondary && {\n  marginTop: 6,\n  marginBottom: 6\n}, ownerState.inset && {\n  paddingLeft: 56\n}));\nconst ListItemText = /*#__PURE__*/React.forwardRef(function ListItemText(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiListItemText'\n  });\n  const {\n      children,\n      className,\n      disableTypography = false,\n      inset = false,\n      primary: primaryProp,\n      primaryTypographyProps,\n      secondary: secondaryProp,\n      secondaryTypographyProps\n    } = props,\n    other = _objectWithoutPropertiesLoose(props, _excluded);\n  const {\n    dense\n  } = React.useContext(ListContext);\n  let primary = primaryProp != null ? primaryProp : children;\n  let secondary = secondaryProp;\n  const ownerState = _extends({}, props, {\n    disableTypography,\n    inset,\n    primary: !!primary,\n    secondary: !!secondary,\n    dense\n  });\n  const classes = useUtilityClasses(ownerState);\n  if (primary != null && primary.type !== Typography && !disableTypography) {\n    primary = /*#__PURE__*/_jsx(Typography, _extends({\n      variant: dense ? 'body2' : 'body1',\n      className: classes.primary,\n      component: primaryTypographyProps != null && primaryTypographyProps.variant ? undefined : 'span',\n      display: \"block\"\n    }, primaryTypographyProps, {\n      children: primary\n    }));\n  }\n  if (secondary != null && secondary.type !== Typography && !disableTypography) {\n    secondary = /*#__PURE__*/_jsx(Typography, _extends({\n      variant: \"body2\",\n      className: classes.secondary,\n      color: \"text.secondary\",\n      display: \"block\"\n    }, secondaryTypographyProps, {\n      children: secondary\n    }));\n  }\n  return /*#__PURE__*/_jsxs(ListItemTextRoot, _extends({\n    className: clsx(classes.root, className),\n    ownerState: ownerState,\n    ref: ref\n  }, other, {\n    children: [primary, secondary]\n  }));\n});\nprocess.env.NODE_ENV !== \"production\" ? ListItemText.propTypes /* remove-proptypes */ = {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n  /**\n   * Alias for the `primary` prop.\n   */\n  children: PropTypes.node,\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n  /**\n   * If `true`, the children won't be wrapped by a Typography component.\n   * This can be useful to render an alternative Typography variant by wrapping\n   * the `children` (or `primary`) text, and optional `secondary` text\n   * with the Typography component.\n   * @default false\n   */\n  disableTypography: PropTypes.bool,\n  /**\n   * If `true`, the children are indented.\n   * This should be used if there is no left avatar or left icon.\n   * @default false\n   */\n  inset: PropTypes.bool,\n  /**\n   * The main content element.\n   */\n  primary: PropTypes.node,\n  /**\n   * These props will be forwarded to the primary typography component\n   * (as long as disableTypography is not `true`).\n   */\n  primaryTypographyProps: PropTypes.object,\n  /**\n   * The secondary content element.\n   */\n  secondary: PropTypes.node,\n  /**\n   * These props will be forwarded to the secondary typography component\n   * (as long as disableTypography is not `true`).\n   */\n  secondaryTypographyProps: PropTypes.object,\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nexport default ListItemText;",
         "import React, { useState, useEffect } from 'react';\nimport { Typography, List, ListItem, ListItemText } from '@mui/material';\nimport { getNeatApiRootUrl } from 'components/Utils';\n\n\nconst AboutView = () => {\n  const [structure, setStructure] = useState(null);\n  const [neatApiRootUrl, setNeatApiRootUrl] = useState(getNeatApiRootUrl());\n  useEffect(() => {\n    const fetchData = async () => {\n      try {\n        const response = await fetch(neatApiRootUrl+'/api/about');\n        const data = await response.json();\n        setStructure(data);\n      } catch (error) {\n        console.error('Error fetching data:', error);\n      }\n    };\n\n    fetchData();\n  }, []);\n\n  if (!structure) {\n    return <div>Loading...</div>;\n  }\n\n  return (\n    <div >\n      <Typography variant=\"h5\" >\n        NEAT Version: {structure.version}\n      </Typography>\n      <Typography variant=\"h6\" >\n        Docs URL: <a href='https://thisisneat.io'>https://thisisneat.io</a>\n      </Typography>\n      <Typography variant=\"h6\" >\n        Docs URL: <a href='https://cognite-neat.readthedocs-hosted.com/en/latest/'>https://cognite-neat.readthedocs-hosted.com/en/latest/</a>\n      </Typography>\n      <Typography variant=\"h6\" >\n        Github: <a href='https://github.com/cognitedata/neat'>https://github.com/cognitedata/neat</a>\n      </Typography>\n      <Typography variant=\"h6\" >\n        Issues tracker (Github): <a href='https://github.com/cognitedata/neat/issues'> https://github.com/cognitedata/neat/issues </a>\n      </Typography>\n      <Typography variant=\"h6\" >\n        License (Apache 2.0): <a href='https://github.com/cognitedata/neat/blob/main/LICENSE'> https://github.com/cognitedata/neat/blob/main/LICENSE </a>\n      </Typography>\n      <Typography variant=\"h5\">\n        3rd party packages :\n      </Typography>\n      <List dense={true}>\n        {structure.packages.map((spackage, index) => (\n          <ListItem key={index}>\n            <ListItemText primary={spackage} />\n          </ListItem>\n        ))}\n      </List>\n    </div>\n  );\n};\n\nexport default AboutView;\n",
```

### Comparing `cognite_neat-0.13.0/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.13.1/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/cognite/neat/migration/wf_manifests.py` & `cognite_neat-0.13.1/cognite/neat/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.13.0/pyproject.toml` & `cognite_neat-0.13.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.13.0"
+version = "0.13.1"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 documentation = "https://cognite-neat.readthedocs-hosted.com/"
```

### Comparing `cognite_neat-0.13.0/PKG-INFO` & `cognite_neat-0.13.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.13.0
+Version: 0.13.1
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```
