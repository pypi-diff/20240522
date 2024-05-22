# Comparing `tmp/cognite_neat-0.77.3.tar.gz` & `tmp/cognite_neat-0.77.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.77.3.tar", max compression
+gzip compressed data, was "cognite_neat-0.77.4.tar", max compression
```

## Comparing `cognite_neat-0.77.3.tar` & `cognite_neat-0.77.4.tar`

### file list

```diff
@@ -1,278 +1,281 @@
--rw-r--r--   0        0        0    11351 2024-05-15 11:15:31.418806 cognite_neat-0.77.3/LICENSE
--rw-r--r--   0        0        0     6775 2024-05-15 11:15:31.418806 cognite_neat-0.77.3/README.md
--rw-r--r--   0        0        0       61 2024-05-15 11:15:31.418806 cognite_neat-0.77.3/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-05-15 11:15:31.418806 cognite_neat-0.77.3/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.418806 cognite_neat-0.77.3/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-05-15 11:15:31.418806 cognite_neat-0.77.3/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4232 2024-05-15 11:15:31.418806 cognite_neat-0.77.3/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-05-15 11:15:31.418806 cognite_neat-0.77.3/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-05-15 11:15:31.418806 cognite_neat-0.77.3/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.418806 cognite_neat-0.77.3/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     1675 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      585 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3523 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4597 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13686 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     8121 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12393 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0    10756 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
--rw-r--r--   0        0        0     8374 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
--rw-r--r--   0        0        0     5333 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
--rw-r--r--   0        0        0      629 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-05-15 11:15:31.422806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1423717 2024-05-15 11:15:31.430806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
--rw-r--r--   0        0        0     2667 2024-05-15 11:15:31.430806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
--rw-r--r--   0        0        0  6282875 2024-05-15 11:15:31.454806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
--rw-r--r--   0        0        0   240334 2024-05-15 11:15:31.454806 cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     6145 2024-05-15 11:15:31.462806 cognite_neat-0.77.3/cognite/neat/config.py
--rw-r--r--   0        0        0     1300 2024-05-15 11:15:31.462806 cognite_neat-0.77.3/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-05-15 11:15:31.462806 cognite_neat-0.77.3/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-05-15 11:15:31.462806 cognite_neat-0.77.3/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-15 11:15:31.466806 cognite_neat-0.77.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14961 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      149 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    13473 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/legacy/__init__.py
--rw-r--r--   0        0        0       73 2024-05-15 11:15:31.470806 cognite_neat-0.77.3/cognite/neat/legacy/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/extractors/__init__.py
--rw-r--r--   0        0        0      363 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/extractors/_base.py
--rw-r--r--   0        0        0    11734 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/extractors/_dexpi.py
--rw-r--r--   0        0        0    17695 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14908 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      701 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/__init__.py
--rw-r--r--   0        0        0    23823 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/_asset_loader.py
--rw-r--r--   0        0        0     2383 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/_base.py
--rw-r--r--   0        0        0     2835 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/_exceptions.py
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/core/__init__.py
--rw-r--r--   0        0        0     2321 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/core/labels.py
--rw-r--r--   0        0        0     5023 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/core/models.py
--rw-r--r--   0        0        0    40464 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22707 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12979 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
--rw-r--r--   0        0        0     3328 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/validator.py
--rw-r--r--   0        0        0      149 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/__init__.py
--rw-r--r--   0        0        0    14289 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/transformations/__init__.py
--rw-r--r--   0        0        0     4765 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/transformations/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
--rw-r--r--   0        0        0    18719 2024-05-15 11:15:31.474806 cognite_neat-0.77.3/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
--rw-r--r--   0        0        0    14737 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/graph/transformations/transformer.py
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/__init__.py
--rw-r--r--   0        0        0     8610 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/__init__.py
--rw-r--r--   0        0        0     2598 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5567 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_base.py
--rw-r--r--   0        0        0      102 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_core/__init__.py
--rw-r--r--   0        0        0      771 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
--rw-r--r--   0        0        0    36813 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     8312 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0     6251 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2graphql.py
--rw-r--r--   0        0        0    18458 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0    28805 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3881 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2rules.py
--rw-r--r--   0        0        0     1085 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2triples.py
--rw-r--r--   0        0        0     5767 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/__init__.py
--rw-r--r--   0        0        0     2273 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_base.py
--rw-r--r--   0        0        0     6476 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_dict2rules.py
--rw-r--r--   0        0        0     7697 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0    12093 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_json2rules.py
--rw-r--r--   0        0        0       63 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9407 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10557 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1502 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0      421 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_xsd2rules.py
--rw-r--r--   0        0        0     1601 2024-05-15 11:15:31.478806 cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      127 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/rules/models/_base.py
--rw-r--r--   0        0        0    12382 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7351 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51091 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/rules/models/tables.py
--rw-r--r--   0        0        0     4402 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/rules/models/value_types.py
--rw-r--r--   0        0        0     1898 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0      170 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0      115 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/analysis/__init__.py
--rw-r--r--   0        0        0      669 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/analysis/_base.py
--rw-r--r--   0        0        0    19584 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/analysis/_information_rules.py
--rw-r--r--   0        0        0      374 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0    65934 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      413 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1511 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1976 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    13688 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0    14172 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    20120 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3026 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4078 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      408 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4274 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0    18546 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12663 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6717 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11897 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7591 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7786 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7437 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     6925 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    11882 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4275 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     6438 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    23617 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     5748 2024-05-15 11:15:31.482806 cognite_neat-0.77.3/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3385 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0    12726 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13936 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0      782 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/__init__.py
--rw-r--r--   0        0        0    10876 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/_base.py
--rw-r--r--   0        0        0    11030 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/_rdfpath.py
--rw-r--r--   0        0        0      305 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/_types/__init__.py
--rw-r--r--   0        0        0      929 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/_types/_base.py
--rw-r--r--   0        0        0     3197 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/_types/_field.py
--rw-r--r--   0        0        0     6078 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/data_types.py
--rw-r--r--   0        0        0      491 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/dms/__init__.py
--rw-r--r--   0        0        0     5863 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/dms/_converter.py
--rw-r--r--   0        0        0    18903 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/dms/_exporter.py
--rw-r--r--   0        0        0    15568 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/dms/_rules.py
--rw-r--r--   0        0        0    13633 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/dms/_rules_input.py
--rw-r--r--   0        0        0    43743 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/dms/_schema.py
--rw-r--r--   0        0        0     6668 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/dms/_serializer.py
--rw-r--r--   0        0        0    14589 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/dms/_validation.py
--rw-r--r--   0        0        0     2993 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/domain.py
--rw-r--r--   0        0        0    16395 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/entities.py
--rw-r--r--   0        0        0      195 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/information/__init__.py
--rw-r--r--   0        0        0     8040 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/information/_converter.py
--rw-r--r--   0        0        0    15546 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/information/_rules.py
--rw-r--r--   0        0        0     7157 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/rules/models/wrapped_entities.py
--rw-r--r--   0        0        0       68 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0     5831 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/cdf_classes.py
--rw-r--r--   0        0        0      483 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11336 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6303 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2714 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12818 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26800 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0    14102 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6570 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     3009 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0        0 2024-05-15 11:15:31.486806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0      225 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/current/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/current/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/current/graph_loader.py
--rw-r--r--   0        0        0     6295 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/current/graph_store.py
--rw-r--r--   0        0        0    22898 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/current/rules_exporter.py
--rw-r--r--   0        0        0    10338 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/current/rules_importer.py
--rw-r--r--   0        0        0     4844 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/current/rules_validator.py
--rw-r--r--   0        0        0       32 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/io/__init__.py
--rw-r--r--   0        0        0    16874 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/io/io_steps.py
--rw-r--r--   0        0        0      274 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/__init__.py
--rw-r--r--   0        0        0     3919 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
--rw-r--r--   0        0        0    29357 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
--rw-r--r--   0        0        0    27265 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
--rw-r--r--   0        0        0    12704 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/graph_store.py
--rw-r--r--   0        0        0     2351 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
--rw-r--r--   0        0        0    20462 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
--rw-r--r--   0        0        0    28065 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
--rw-r--r--   0        0        0     2943 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    11007 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-05-15 11:15:31.490806 cognite_neat-0.77.3/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4589 2024-05-15 11:15:31.878807 cognite_neat-0.77.3/pyproject.toml
--rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.77.3/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/LICENSE
+-rw-r--r--   0        0        0     6775 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/README.md
+-rw-r--r--   0        0        0       61 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4232 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     1675 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      585 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3523 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4597 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13686 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     8121 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12393 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0    10756 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
+-rw-r--r--   0        0        0     8374 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
+-rw-r--r--   0        0        0     5333 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
+-rw-r--r--   0        0        0      629 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-05-22 13:51:29.975081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1423717 2024-05-22 13:51:29.983081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
+-rw-r--r--   0        0        0     2667 2024-05-22 13:51:29.983081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
+-rw-r--r--   0        0        0  6282875 2024-05-22 13:51:30.007081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
+-rw-r--r--   0        0        0   240334 2024-05-22 13:51:30.011081 cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     6145 2024-05-22 13:51:30.015081 cognite_neat-0.77.4/cognite/neat/config.py
+-rw-r--r--   0        0        0     1300 2024-05-22 13:51:30.015081 cognite_neat-0.77.4/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-05-22 13:51:30.015081 cognite_neat-0.77.4/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-05-22 13:51:30.015081 cognite_neat-0.77.4/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-22 13:51:30.019081 cognite_neat-0.77.4/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14961 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      149 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    13473 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/legacy/__init__.py
+-rw-r--r--   0        0        0       73 2024-05-22 13:51:30.023081 cognite_neat-0.77.4/cognite/neat/legacy/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      363 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/extractors/_base.py
+-rw-r--r--   0        0        0    11734 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/extractors/_dexpi.py
+-rw-r--r--   0        0        0    17695 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14908 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      701 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/__init__.py
+-rw-r--r--   0        0        0    23823 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/_asset_loader.py
+-rw-r--r--   0        0        0     2383 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/_base.py
+-rw-r--r--   0        0        0     2835 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2321 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5023 2024-05-22 13:51:30.027082 cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    40464 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22707 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12979 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
+-rw-r--r--   0        0        0     3328 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/validator.py
+-rw-r--r--   0        0        0      149 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14289 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/transformations/__init__.py
+-rw-r--r--   0        0        0     4765 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/transformations/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0    18719 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    14737 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/graph/transformations/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/__init__.py
+-rw-r--r--   0        0        0     8610 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_base.py
+-rw-r--r--   0        0        0      102 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_core/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
+-rw-r--r--   0        0        0    36813 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     8312 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0     6251 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2graphql.py
+-rw-r--r--   0        0        0    18458 2024-05-22 13:51:30.031082 cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0    28805 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3881 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2rules.py
+-rw-r--r--   0        0        0     1085 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2triples.py
+-rw-r--r--   0        0        0     5767 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/__init__.py
+-rw-r--r--   0        0        0     2273 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_base.py
+-rw-r--r--   0        0        0     6476 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_dict2rules.py
+-rw-r--r--   0        0        0     7697 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0    12093 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9407 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10557 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1502 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      421 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_xsd2rules.py
+-rw-r--r--   0        0        0     1601 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      127 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/models/_base.py
+-rw-r--r--   0        0        0    12382 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7351 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51091 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/models/tables.py
+-rw-r--r--   0        0        0     4402 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/rules/models/value_types.py
+-rw-r--r--   0        0        0     1898 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0      170 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0      115 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/analysis/__init__.py
+-rw-r--r--   0        0        0      669 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/analysis/_base.py
+-rw-r--r--   0        0        0    19179 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/analysis/_information_rules.py
+-rw-r--r--   0        0        0      374 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    65934 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      413 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1511 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1976 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    13688 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    14244 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    20120 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3026 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4078 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      408 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4274 2024-05-22 13:51:30.035082 cognite_neat-0.77.4/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    18994 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12663 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6718 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11897 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7591 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7786 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7437 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     6925 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    12438 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4275 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6438 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    23617 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     5748 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3385 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0    12726 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    15825 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0      782 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/__init__.py
+-rw-r--r--   0        0        0    11126 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/_base.py
+-rw-r--r--   0        0        0    11030 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/_rdfpath.py
+-rw-r--r--   0        0        0      305 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/_types/__init__.py
+-rw-r--r--   0        0        0      929 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/_types/_base.py
+-rw-r--r--   0        0        0     3197 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/_types/_field.py
+-rw-r--r--   0        0        0     6078 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/data_types.py
+-rw-r--r--   0        0        0      491 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/dms/__init__.py
+-rw-r--r--   0        0        0     5959 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/dms/_converter.py
+-rw-r--r--   0        0        0    18984 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/dms/_exporter.py
+-rw-r--r--   0        0        0    15690 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/dms/_rules.py
+-rw-r--r--   0        0        0    13467 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/dms/_rules_input.py
+-rw-r--r--   0        0        0    43808 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/dms/_schema.py
+-rw-r--r--   0        0        0     6669 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/dms/_serializer.py
+-rw-r--r--   0        0        0    12963 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/dms/_validation.py
+-rw-r--r--   0        0        0     2993 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/domain.py
+-rw-r--r--   0        0        0    16395 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/entities.py
+-rw-r--r--   0        0        0      291 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/information/__init__.py
+-rw-r--r--   0        0        0     8040 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/information/_converter.py
+-rw-r--r--   0        0        0    13365 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/information/_rules.py
+-rw-r--r--   0        0        0    10147 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/information/_rules_input.py
+-rw-r--r--   0        0        0     3989 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/information/_serializer.py
+-rw-r--r--   0        0        0     7528 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/information/_validation.py
+-rw-r--r--   0        0        0     7157 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/rules/models/wrapped_entities.py
+-rw-r--r--   0        0        0       68 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0     2422 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0     5831 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/cdf_classes.py
+-rw-r--r--   0        0        0      483 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11336 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6303 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2714 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12818 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26800 2024-05-22 13:51:30.039082 cognite_neat-0.77.4/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0    14102 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6570 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     3009 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/current/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/current/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/current/graph_loader.py
+-rw-r--r--   0        0        0     6295 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/current/graph_store.py
+-rw-r--r--   0        0        0    23886 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/current/rules_exporter.py
+-rw-r--r--   0        0        0    11459 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/current/rules_importer.py
+-rw-r--r--   0        0        0     4844 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/current/rules_validator.py
+-rw-r--r--   0        0        0       32 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/io/__init__.py
+-rw-r--r--   0        0        0    16874 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/io/io_steps.py
+-rw-r--r--   0        0        0      274 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/__init__.py
+-rw-r--r--   0        0        0     3919 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
+-rw-r--r--   0        0        0    29357 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
+-rw-r--r--   0        0        0    27265 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
+-rw-r--r--   0        0        0    12704 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/graph_store.py
+-rw-r--r--   0        0        0     2351 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
+-rw-r--r--   0        0        0    20462 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
+-rw-r--r--   0        0        0    28065 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
+-rw-r--r--   0        0        0     2943 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    11007 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-05-22 13:51:30.043082 cognite_neat-0.77.4/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4589 2024-05-22 13:51:30.451087 cognite_neat-0.77.4/pyproject.toml
+-rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.77.4/PKG-INFO
```

### Comparing `cognite_neat-0.77.3/LICENSE` & `cognite_neat-0.77.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/README.md` & `cognite_neat-0.77.4/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/api/configuration.py` & `cognite_neat-0.77.4/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.77.4/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/api/explorer.py` & `cognite_neat-0.77.4/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.77.4/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.77.4/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.77.4/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.77.4/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.77.4/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.77.4/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.77.4/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.77.4/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.77.4/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.77.4/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg` & `cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg` & `cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg` & `cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js` & `cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt` & `cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map` & `cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.77.4/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/config.py` & `cognite_neat-0.77.4/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/constants.py` & `cognite_neat-0.77.4/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/exceptions.py` & `cognite_neat-0.77.4/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.77.4/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.77.4/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.77.4/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/graph/exceptions.py` & `cognite_neat-0.77.4/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.77.4/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.77.4/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.77.4/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.77.4/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.77.4/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.77.4/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.77.4/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.77.4/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/exceptions.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/extractors/_dexpi.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/extractors/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/__init__.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/_asset_loader.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/_base.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/_exceptions.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/core/labels.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/core/models.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/rdf_to_dms.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/loaders/validator.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/__init__.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/_base.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/_graphdb_store.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/_memory_store.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/_oxigraph_store.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/_oxrdflib.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/transformations/entity_matcher.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/transformations/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/transformations/query_generator/sparql.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/transformations/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/graph/transformations/transformer.py` & `cognite_neat-0.77.4/cognite/neat/legacy/graph/transformations/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/analysis.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/__init__.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/power-grid-model.yaml` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/rules-template.xlsx` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/skos-rules.xlsx` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/examples/wind-energy.owl` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/exceptions.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/__init__.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_base.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_core/rules2labels.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2dms.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2excel.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2graphql.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2ontology.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2rules.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_rules2triples.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/exporters/_validation.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/__init__.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_base.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_dict2rules.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_dms2rules.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_graph2rules.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_json2rules.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/importers/_yaml2rules.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/models/_base.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/models/raw_rules.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/models/rdfpath.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/models/rules.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/rules/models/value_types.py` & `cognite_neat-0.77.4/cognite/neat/legacy/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/analysis/_base.py` & `cognite_neat-0.77.4/cognite/neat/rules/analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/analysis/_information_rules.py` & `cognite_neat-0.77.4/cognite/neat/rules/analysis/_information_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,32 +9,22 @@
 
 from cognite.neat.rules.models import SchemaCompleteness
 from cognite.neat.rules.models._rdfpath import TransformationRuleType
 from cognite.neat.rules.models.entities import ClassEntity, EntityTypes, ParentClassEntity, ReferenceEntity
 from cognite.neat.rules.models.information import InformationClass, InformationProperty, InformationRules
 from cognite.neat.utils.utils import get_inheritance_path
 
-from ._base import BaseAnalysis, DataModelingScenario
+from ._base import BaseAnalysis
 
 
 class InformationArchitectRulesAnalysis(BaseAnalysis):
     def __init__(self, rules: InformationRules):
         self.rules = rules
 
     @property
-    def data_modeling_scenario(self) -> DataModelingScenario:
-        if not self.rules.reference:
-            return DataModelingScenario.from_scratch
-
-        if self.rules.metadata.namespace == self.rules.reference.metadata.namespace:
-            return DataModelingScenario.extend_reference
-        else:
-            return DataModelingScenario.build_solution
-
-    @property
     def referred_classes(self) -> set[ClassEntity]:
         return self.directly_referred_classes.union(self.inherited_referred_classes)
 
     @property
     def referred_classes_properties(self) -> list[InformationProperty]:
         referred_classes_properties = []
         class_properties_dict = self.classes_with_properties(use_reference=True)
@@ -358,15 +348,15 @@
             This method will attempt to validate the reduced rules with custom validations.
             If it fails, it will return a partial rules with a warning message, validated
             only with base Pydantic validators.
         """
 
         rules = cast(InformationRules, self.rules.reference if use_reference else self.rules)
 
-        if not rules.metadata.schema_ is not SchemaCompleteness.complete:
+        if rules.metadata.schema_ is not SchemaCompleteness.complete:
             raise ValueError("Rules are not complete cannot perform reduction!")
         class_as_dict = self.as_class_dict()
         class_parents_pairs = self.class_parent_pairs()
         defined_classes = self.defined_classes(consider_inheritance=True)
 
         possible_classes = defined_classes.intersection(desired_classes)
         impossible_classes = desired_classes - possible_classes
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.77.4/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/exceptions.py` & `cognite_neat-0.77.4/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.77.4/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.77.4/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.77.4/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.77.4/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,19 +128,19 @@
             if rules.reference:
                 dumped_reference_rules = rules.reference.model_dump(by_alias=True)
 
         self._write_metadata_sheet(workbook, dumped_user_rules["Metadata"])
         self._write_sheets(workbook, dumped_user_rules, rules)
         if dumped_last_rules:
             self._write_sheets(workbook, dumped_last_rules, rules, sheet_prefix="Last")
+            self._write_metadata_sheet(workbook, dumped_last_rules["Metadata"], sheet_prefix="Last")
 
         if dumped_reference_rules:
-            prefix = "Ref"
-            self._write_sheets(workbook, dumped_reference_rules, rules, sheet_prefix=prefix)
-            self._write_metadata_sheet(workbook, dumped_reference_rules["Metadata"], sheet_prefix=prefix)
+            self._write_sheets(workbook, dumped_reference_rules, rules, sheet_prefix="Ref")
+            self._write_metadata_sheet(workbook, dumped_reference_rules["Metadata"], sheet_prefix="Ref")
 
         if self._styling_level > 0:
             self._adjust_column_widths(workbook)
 
         return workbook
 
     def _write_sheets(self, workbook: Workbook, dumped_rules: dict[str, Any], rules: Rules, sheet_prefix: str = ""):
@@ -287,15 +287,15 @@
         created.pop("extension", None)
         return created
 
     def _create_new_info(self, now: datetime) -> InformationMetadata:
         prefix = self.new_model_id[0]
         return InformationMetadata(
             data_model_type=DataModelType.solution,
-            schema_=SchemaCompleteness.extended,
+            schema_=SchemaCompleteness.complete,
             extension=ExtensionCategory.addition,
             prefix=prefix,
             namespace=f"http://purl.org/neat/{prefix}/",  # type: ignore[arg-type]
             description=None,
             version="1",
             created=now,
             updated=now,
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.77.4/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.77.4/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.77.4/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.77.4/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.77.4/cognite/neat/rules/importers/_dms2rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         issue_list = IssueList()
         with _handle_issues(issue_list) as result:
             schema = DMSSchema.from_data_model(client, user_model, ref_model)
 
         if result.result == "failure" or issue_list.has_errors:
             return cls(DMSSchema(), issue_list)
 
-        metadata = cls._create_metadata_from_model(user_model)
+        metadata = cls._create_metadata_from_model(user_model, has_reference=ref_model is not None)
         ref_metadata = cls._create_metadata_from_model(ref_model) if ref_model else None
 
         return cls(schema, issue_list, metadata, ref_metadata)
 
     @classmethod
     def _find_model_in_list(
         cls, data_models: dm.DataModelList[dm.View], model_id: DataModelIdentifier
@@ -127,26 +127,28 @@
             ]
         )
 
     @classmethod
     def _create_metadata_from_model(
         cls,
         model: dm.DataModel[dm.View] | dm.DataModelApply,
+        has_reference: bool = False,
     ) -> DMSMetadata:
         description, creator = DMSMetadata._get_description_and_creator(model.description)
 
         if isinstance(model, dm.DataModel):
             created = ms_to_datetime(model.created_time)
             updated = ms_to_datetime(model.last_updated_time)
         else:
             now = datetime.now().replace(microsecond=0)
             created = now
             updated = now
         return DMSMetadata(
             schema_=SchemaCompleteness.complete,
+            data_model_type=DataModelType.solution if has_reference else DataModelType.enterprise,
             extension=ExtensionCategory.addition,
             space=model.space,
             external_id=model.external_id,
             name=model.name or model.external_id,
             version=model.version or "0.1.0",
             updated=updated,
             created=created,
@@ -198,24 +200,29 @@
             reference: DMSRules | None = None
             if (ref_schema := self.root_schema.reference) and (ref_model := ref_schema.data_model):
                 # Reference should always be an enterprise model.
                 reference = DMSRules(
                     **self._create_rule_components(
                         ref_model,
                         ref_schema,
-                        self.ref_metadata or self._create_default_metadata(list(ref_schema.views.values())),
+                        self.ref_metadata
+                        or self._create_default_metadata(list(ref_schema.views.values()), is_ref=True),
                         DataModelType.enterprise,
                     )
                 )
-                schema_completeness = SchemaCompleteness.extended
                 data_model_type = DataModelType.solution
 
             user_rules = DMSRules(
                 **self._create_rule_components(
-                    model, self.root_schema, self.metadata, data_model_type, schema_completeness
+                    model,
+                    self.root_schema,
+                    self.metadata,
+                    data_model_type,
+                    schema_completeness,
+                    has_reference=reference is not None,
                 ),
                 reference=reference,
             )
 
         if future.result == "failure" or self.issue_list.has_errors:
             return self._return_or_raise(self.issue_list, errors)
 
@@ -224,29 +231,30 @@
     def _create_rule_components(
         self,
         data_model: dm.DataModelApply,
         schema: DMSSchema,
         metadata: DMSMetadata | None = None,
         data_model_type: DataModelType | None = None,
         schema_completeness: SchemaCompleteness | None = None,
+        has_reference: bool = False,
     ) -> dict[str, Any]:
         properties = SheetList[DMSProperty]()
         for view_id, view in schema.views.items():
             view_entity = ViewEntity.from_id(view_id)
             class_entity = view_entity.as_class()
             for prop_id, prop in (view.properties or {}).items():
                 dms_property = self._create_dms_property(prop_id, prop, view_entity, class_entity)
                 if dms_property is not None:
                     properties.append(dms_property)
 
         data_model_view_ids: set[dm.ViewId] = {
             view.as_id() if isinstance(view, dm.View | dm.ViewApply) else view for view in data_model.views or []
         }
 
-        metadata = metadata or DMSMetadata.from_data_model(data_model)
+        metadata = metadata or DMSMetadata.from_data_model(data_model, has_reference)
         if data_model_type is not None:
             metadata.data_model_type = data_model_type
         if schema_completeness is not None:
             metadata.schema_ = schema_completeness
         return dict(
             metadata=metadata,
             properties=properties,
@@ -258,20 +266,21 @@
                     DMSView.from_view(view, in_model=view_id in data_model_view_ids)
                     for view_id, view in schema.views.items()
                 ]
             ),
         )
 
     @classmethod
-    def _create_default_metadata(cls, views: Sequence[dm.View | dm.ViewApply]) -> DMSMetadata:
+    def _create_default_metadata(cls, views: Sequence[dm.View | dm.ViewApply], is_ref: bool = False) -> DMSMetadata:
         now = datetime.now().replace(microsecond=0)
         space = Counter(view.space for view in views).most_common(1)[0][0]
         return DMSMetadata(
             schema_=SchemaCompleteness.complete,
             extension=ExtensionCategory.addition,
+            data_model_type=DataModelType.enterprise if is_ref else DataModelType.solution,
             space=space,
             external_id="Unknown",
             version="0.1.0",
             creator=["Unknown"],
             created=now,
             updated=now,
         )
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.77.4/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.77.4/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.77.4/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
     ) -> tuple[Rules | None, IssueList] | Rules:
         converter = _DTDLConverter(self._read_issues)
 
         converter.convert(self._items)
 
         metadata = self._default_metadata()
         metadata["schema"] = self._schema_completeness.value
+
         if self.title:
             metadata["title"] = to_pascal(self.title)
         try:
             most_common_prefix = converter.get_most_common_prefix()
         except ValueError:
             # No prefixes are defined so we just use the default prefix...
             ...
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.77.4/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.77.4/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.77.4/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.77.4/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.77.4/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.77.4/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     DMSRules,
     DomainRules,
     InformationRules,
     RoleTypes,
     SchemaCompleteness,
 )
 from cognite.neat.rules.models.dms import DMSRulesInput
+from cognite.neat.rules.models.information import InformationRulesInput
 from cognite.neat.utils.auxiliary import local_import
 from cognite.neat.utils.spreadsheet import SpreadsheetRead, read_individual_sheet
 
 from ._base import BaseImporter, Rules, _handle_issues
 
 SOURCE_SHEET__TARGET_FIELD__HEADERS = [
     (
@@ -106,25 +107,35 @@
         metadata: MetadataRaw | None = None,
         sheet_prefix: Literal["", "Last", "Ref"] = "",
     ):
         self.issue_list = issue_list
         self.required = required
         self.metadata = metadata
         self._sheet_prefix = sheet_prefix
+        self._seen_files: set[Path] = set()
+        self._seen_sheets: set[str] = set()
 
     @property
     def metadata_sheet_name(self) -> str:
         return f"{self._sheet_prefix}Metadata"
 
+    @property
+    def seen_sheets(self) -> set[str]:
+        if not self._seen_files:
+            raise ValueError("No files have been read yet.")
+        return self._seen_sheets
+
     def sheet_names(self, role: RoleTypes) -> set[str]:
         names = MANDATORY_SHEETS_BY_ROLE[role]
         return {f"{self._sheet_prefix}{sheet_name}" for sheet_name in names if sheet_name != "Metadata"}
 
     def read(self, filepath: Path) -> None | ReadResult:
         with pd.ExcelFile(filepath) as excel_file:
+            self._seen_files.add(filepath)
+            self._seen_sheets.update(map(str, excel_file.sheet_names))
             metadata: MetadataRaw | None
             if self.metadata is not None:
                 metadata = self.metadata
             else:
                 metadata = self._read_metadata(excel_file, filepath)
                 if metadata is None:
                     # The reading of metadata failed, so we can't continue
@@ -208,28 +219,28 @@
         self, errors: Literal["raise", "continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList] | Rules:
         issue_list = IssueList(title=f"'{self.filepath.name}'")
         if not self.filepath.exists():
             issue_list.append(issues.spreadsheet_file.SpreadsheetNotFoundError(self.filepath))
             return self._return_or_raise(issue_list, errors)
 
-        user_read = SpreadsheetReader(issue_list).read(self.filepath)
+        user_reader = SpreadsheetReader(issue_list)
+        user_read = user_reader.read(self.filepath)
         if user_read is None or issue_list.has_errors:
             return self._return_or_raise(issue_list, errors)
 
         last_read: ReadResult | None = None
+        if any(sheet_name.startswith("Last") for sheet_name in user_reader.seen_sheets):
+            last_read = SpreadsheetReader(issue_list, required=False, sheet_prefix="Last").read(self.filepath)
         reference_read: ReadResult | None = None
-        if user_read.schema == SchemaCompleteness.extended:
-            # Last does not have its own metadata sheet. It is the same as the user's metadata sheet.
-            last_read = SpreadsheetReader(
-                issue_list, required=False, metadata=user_read.metadata, sheet_prefix="Last"
-            ).read(self.filepath)
+        if any(sheet_name.startswith("Ref") for sheet_name in user_reader.seen_sheets):
             reference_read = SpreadsheetReader(issue_list, sheet_prefix="Ref").read(self.filepath)
-            if issue_list.has_errors:
-                return self._return_or_raise(issue_list, errors)
+
+        if issue_list.has_errors:
+            return self._return_or_raise(issue_list, errors)
 
         if reference_read and user_read.role != reference_read.role:
             issue_list.append(issues.spreadsheet_file.RoleMismatchError(self.filepath))
             return self._return_or_raise(issue_list, errors)
 
         sheets = user_read.sheets
         original_role = user_read.role
@@ -249,14 +260,16 @@
             issue_list,
             error_cls=issues.spreadsheet.InvalidSheetError,
             error_args={"read_info_by_sheet": read_info_by_sheet},
         ) as future:
             rules: Rules
             if rules_cls is DMSRules:
                 rules = DMSRulesInput.load(sheets).as_rules()
+            elif rules_cls is InformationRules:
+                rules = InformationRulesInput.load(sheets).as_rules()
             else:
                 rules = rules_cls.model_validate(sheets)  # type: ignore[attr-defined]
 
         if future.result == "failure" or issue_list.has_errors:
             return self._return_or_raise(issue_list, errors)
 
         return self._to_output(
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.77.4/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.77.4/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/issues/base.py` & `cognite_neat-0.77.4/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.77.4/cognite/neat/rules/issues/dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.77.4/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.77.4/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.77.4/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.77.4/cognite/neat/rules/issues/spreadsheet.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from cognite.client.data_classes import data_modeling as dm
 from cognite.client.data_classes.data_modeling import ContainerId, ViewId
 from pydantic_core import ErrorDetails
 
 from cognite.neat.utils.spreadsheet import SpreadsheetRead
 
-from .base import DefaultPydanticError, MultiValueError, NeatValidationError, ValidationWarning
+from .base import DefaultPydanticError, MultiValueError, NeatValidationError
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 __all__ = [
@@ -23,15 +23,15 @@
     "InvalidPropertyError",
     "InvalidClassError",
     "InvalidContainerError",
     "InvalidViewError",
     "InvalidRowUnknownSheetError",
     "NonExistingContainerError",
     "NonExistingViewError",
-    "ClassNoPropertiesNoParentsWarning",
+    "ClassNoPropertiesNoParentError",
     "InconsistentContainerDefinitionError",
     "MultiValueTypeError",
     "MultiValueIsListError",
     "MultiNullableError",
     "MultiDefaultError",
     "MultiIndexError",
     "MultiUniqueConstraintError",
@@ -235,29 +235,84 @@
     def dump(self) -> dict[str, Any]:
         output = super().dump()
         output["view_id"] = self.view_id
         return output
 
 
 @dataclass(frozen=True)
-class ClassNoPropertiesNoParentsWarning(ValidationWarning):
+class PropertiesDefinedForUndefinedClassesError(NeatValidationError):
+    description = "Properties are defined for undefined classes."
+    fix = "Make sure to define class in the Classes sheet."
+
+    classes: list[str]
+
+    def dump(self) -> dict[str, list[str]]:
+        output = super().dump()
+        output["classes"] = self.classes
+        return output
+
+    def message(self) -> str:
+        return (
+            f"Classes {', '.join(self.classes)} have properties assigned to them, but"
+            " they are not defined in the Classes sheet."
+        )
+
+
+@dataclass(frozen=True)
+class ClassNoPropertiesNoParentError(NeatValidationError):
     description = "Class has no properties and no parents."
     fix = "Check if the class should have properties or parents."
 
     classes: list[str]
 
     def dump(self) -> dict[str, list[str]]:
         output = super().dump()
         output["classes"] = self.classes
         return output
 
     def message(self) -> str:
         if len(self.classes) > 1:
-            return f"Classes {', '.join(self.classes)} have no properties and no parents. This may be a mistake."
-        return f"Class {self.classes[0]} has no properties and no parents. This may be a mistake."
+            return f"Classes {', '.join(self.classes)} have no direct or inherited properties. This may be a mistake."
+        return f"Class {self.classes[0]} have no direct or inherited properties. This may be a mistake."
+
+
+@dataclass(frozen=True)
+class ParentClassesNotDefinedError(NeatValidationError):
+    description = "Parent classes are not defined."
+    fix = "Check if the parent classes are defined in Classes sheet."
+
+    classes: list[str]
+
+    def dump(self) -> dict[str, list[str]]:
+        output = super().dump()
+        output["classes"] = self.classes
+        return output
+
+    def message(self) -> str:
+        if len(self.classes) > 1:
+            return f"Parent classes {', '.join(self.classes)} are not defined. This may be a mistake."
+        return f"Parent classes {', '.join(self.classes[0])} are not defined. This may be a mistake."
+
+
+@dataclass(frozen=True)
+class ValueTypeNotDefinedError(NeatValidationError):
+    description = "Value types referred by properties are not defined in Rules."
+    fix = "Make sure that all value types are defined in Rules."
+
+    value_types: list[str]
+
+    def dump(self) -> dict[str, list[str]]:
+        output = super().dump()
+        output["classes"] = self.value_types
+        return output
+
+    def message(self) -> str:
+        if len(self.value_types) > 1:
+            return f"Value types {', '.join(self.value_types)} are not defined. This may be a mistake."
+        return f"Value types {', '.join(self.value_types[0])} are not defined. This may be a mistake."
 
 
 @dataclass(frozen=True)
 class InconsistentContainerDefinitionError(NeatValidationError, ABC):
     description = "This is a base class for all errors related to inconsistent container definitions"
     fix = "Ensure all properties using the same container have the same type, constraints, and indexes."
     container: dm.ContainerId
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.77.4/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/__init__.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/_base.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,20 @@
     from backports.strenum import StrEnum
     from typing_extensions import Self
 
 
 METADATA_VALUE_MAX_LENGTH = 5120
 
 
+def _add_alias(data: dict[str, Any], base_model: type[BaseModel]) -> None:
+    for field_name, field_ in base_model.model_fields.items():
+        if field_name not in data and field_.alias in data:
+            data[field_name] = data[field_.alias]
+
+
 def replace_nan_floats_with_default(values: dict, model_fields: dict[str, FieldInfo]) -> dict:
     output = {}
     for field_name, value in values.items():
         is_nan_float = isinstance(value, float) and math.isnan(value)
         if not is_nan_float:
             output[field_name] = value
             continue
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/_rdfpath.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/_rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/_types/_base.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/_types/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/_types/_field.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/data_types.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/dms/_converter.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/dms/_converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,14 +101,16 @@
     @classmethod
     def _convert_metadata_to_info(cls, metadata: DMSMetadata) -> "InformationMetadata":
         from cognite.neat.rules.models.information._rules import InformationMetadata
 
         prefix = metadata.space
         return InformationMetadata(
             schema_=metadata.schema_,
+            data_model_type=metadata.data_model_type,
+            extension=metadata.extension,
             prefix=prefix,
             namespace=Namespace(f"https://purl.orgl/neat/{prefix}/"),
             version=metadata.version,
             description=metadata.description,
             name=metadata.name or metadata.external_id,
             creator=metadata.creator,
             created=metadata.created,
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/dms/_exporter.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/dms/_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,16 @@
             node_types=node_types,
         )
         if self.include_pipeline:
             return PipelineSchema.from_dms(output, self.instance_space)
 
         if self._ref_schema:
             output.reference = self._ref_schema
-
+        if self.rules.last:
+            output.last = self.rules.last.as_schema()
         return output
 
     def _create_spaces(
         self,
         metadata: DMSMetadata,
         containers: ContainerApplyDict,
         views: ViewApplyDict,
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/dms/_rules.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/dms/_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     from typing_extensions import Self
 
 _DEFAULT_VERSION = "1"
 
 
 class DMSMetadata(BaseMetadata):
     role: ClassVar[RoleTypes] = RoleTypes.dms_architect
-    data_model_type: DataModelType = Field(DataModelType.solution, alias="dataModelType")
+    data_model_type: DataModelType = Field(DataModelType.enterprise, alias="dataModelType")
     schema_: SchemaCompleteness = Field(alias="schema")
     extension: ExtensionCategory = ExtensionCategory.addition
     space: ExternalIdType
     name: str | None = Field(
         None,
         description="Human readable name of the data model",
         min_length=1,
@@ -142,18 +142,19 @@
             description = description_raw
         else:
             creator = ["MISSING"]
             description = None
         return description, creator
 
     @classmethod
-    def from_data_model(cls, data_model: dm.DataModelApply) -> "DMSMetadata":
+    def from_data_model(cls, data_model: dm.DataModelApply, has_reference: bool) -> "DMSMetadata":
         description, creator = cls._get_description_and_creator(data_model.description)
         return cls(
             schema_=SchemaCompleteness.complete,
+            data_model_type=DataModelType.solution if has_reference else DataModelType.enterprise,
             space=data_model.space,
             name=data_model.name or None,
             description=description,
             external_id=data_model.external_id,
             version=data_model.version,
             creator=creator,
             created=datetime.now(),
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/dms/_rules_input.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/dms/_rules_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from collections.abc import Sequence
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Literal, cast, overload
 
-from pydantic import BaseModel
-
-from cognite.neat.rules.models._base import DataModelType, ExtensionCategory, SchemaCompleteness
+from cognite.neat.rules.models._base import DataModelType, ExtensionCategory, SchemaCompleteness, _add_alias
 from cognite.neat.rules.models.data_types import DataType
 from cognite.neat.rules.models.entities import (
     ClassEntity,
     ContainerEntity,
     DMSUnknownEntity,
     Unknown,
     ViewEntity,
@@ -40,16 +38,17 @@
         _add_alias(data, DMSMetadata)
         return cls(
             schema_=data.get("schema_"),  # type: ignore[arg-type]
             space=data.get("space"),  # type: ignore[arg-type]
             external_id=data.get("external_id"),  # type: ignore[arg-type]
             creator=data.get("creator"),  # type: ignore[arg-type]
             version=data.get("version"),  # type: ignore[arg-type]
-            extension=data.get("extension", "addition"),
-            data_model_type=data.get("data_model_type", "solution"),
+            # safeguard from empty cell, i.e. if key provided by value None
+            extension=data.get("extension", "addition") or "addition",
+            data_model_type=data.get("data_model_type", "solution") or "solution",
             name=data.get("name"),
             description=data.get("description"),
             created=data.get("created"),
             updated=data.get("updated"),
         )
 
     def dump(self) -> dict[str, Any]:
@@ -351,13 +350,7 @@
             Metadata=self.metadata.dump(),
             Properties=[prop.dump(default_space, default_version) for prop in self.properties],
             Views=[view.dump(default_space, default_version) for view in self.views],
             Containers=[container.dump(default_space) for container in self.containers or []] or None,
             Last=last,
             Reference=reference,
         )
-
-
-def _add_alias(data: dict[str, Any], base_model: type[BaseModel]) -> None:
-    for field_name, field_ in base_model.model_fields.items():
-        if field_name not in data and field_.alias in data:
-            data[field_name] = data[field_.alias]
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/dms/_schema.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/dms/_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,18 +512,19 @@
             raise ValueError(f"Cannot sort item of type {type(item)}")
 
     def validate(self) -> list[DMSSchemaError]:
         errors: set[DMSSchemaError] = set()
         defined_spaces = self.spaces.copy()
         defined_containers = self.containers.copy()
         defined_views = self.views.copy()
-        if self.reference:
-            defined_spaces |= self.reference.spaces
-            defined_containers |= self.reference.containers
-            defined_views |= self.reference.views
+        for other_schema in [self.reference, self.last]:
+            if other_schema:
+                defined_spaces |= other_schema.spaces
+                defined_containers |= other_schema.containers
+                defined_views |= other_schema.views
 
         for container in self.containers.values():
             if container.space not in defined_spaces:
                 errors.add(MissingSpaceError(space=container.space, referred_by=container.as_id()))
 
         for view in self.views.values():
             view_id = view.as_id()
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/dms/_serializer.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/dms/_serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.container_constraint = "constraint"
 
         if info.by_alias:
             self.properties_fields = [
                 DMSProperty.model_fields[field].alias or field for field in self.properties_fields
             ]
             self.views_fields = [DMSView.model_fields[field].alias or field for field in self.views_fields]
-            self.container_fields = [
+            self.containers_fields = [
                 DMSContainer.model_fields[field].alias or field for field in self.containers_fields
             ]
             self.prop_view = DMSProperty.model_fields[self.prop_view].alias or self.prop_view
             self.prop_view_property = DMSProperty.model_fields[self.prop_view_property].alias or self.prop_view_property
             self.prop_value_type = DMSProperty.model_fields[self.prop_value_type].alias or self.prop_value_type
             self.view_view = DMSView.model_fields[self.view_view].alias or self.view_view
             self.view_implements = DMSView.model_fields[self.view_implements].alias or self.view_implements
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/dms/_validation.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/dms/_validation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from collections import defaultdict
 from typing import Any
 
 from cognite.client import data_modeling as dm
 
 from cognite.neat.rules import issues
 from cognite.neat.rules.issues import IssueList
-from cognite.neat.rules.models._base import ExtensionCategory, SchemaCompleteness
+from cognite.neat.rules.models._base import DataModelType, ExtensionCategory, SchemaCompleteness
 from cognite.neat.rules.models.data_types import DataType
 from cognite.neat.rules.models.entities import ContainerEntity
 from cognite.neat.rules.models.wrapped_entities import RawFilter
 
 from ._rules import DMSProperty, DMSRules
+from ._schema import DMSSchema
 
 
 class DMSPostValidation:
     """This class does all the validation of the DMS rules that have dependencies between
     components."""
 
     def __init__(self, rules: DMSRules):
@@ -22,20 +23,25 @@
         self.metadata = rules.metadata
         self.properties = rules.properties
         self.containers = rules.containers
         self.views = rules.views
         self.issue_list = IssueList()
 
     def validate(self) -> IssueList:
-        self._validate_best_practices()
+        self._validate_raw_filter()
         self._consistent_container_properties()
+
         self._referenced_views_and_containers_are_existing()
-        self._validate_extension()
-        self._validate_schema()
-        self._validate_performance()
+        if self.metadata.schema_ is SchemaCompleteness.extended:
+            self._validate_extension()
+        if self.metadata.schema_ is SchemaCompleteness.partial:
+            return self.issue_list
+        dms_schema = self.rules.as_schema()
+        self.issue_list.extend(dms_schema.validate())
+        self._validate_performance(dms_schema)
         return self.issue_list
 
     def _consistent_container_properties(self) -> None:
         container_properties_by_id: dict[tuple[ContainerEntity, str], list[tuple[int, DMSProperty]]] = defaultdict(list)
         for prop_no, prop in enumerate(self.properties):
             if prop.container and prop.container_property:
                 container_properties_by_id[(prop.container, prop.container_property)].append((prop_no, prop))
@@ -102,16 +108,17 @@
                 prop.nullable = prop.nullable or nullable_definition
                 prop.default = prop.default or default_definition
                 prop.index = prop.index or index_definition
                 prop.constraint = prop.constraint or constraint_definition
         self.issue_list.extend(errors)
 
     def _referenced_views_and_containers_are_existing(self) -> None:
-        # There two checks are done in the same method to raise all the errors at once.
         defined_views = {view.view.as_id() for view in self.views}
+        if self.metadata.schema_ is SchemaCompleteness.extended and self.rules.last:
+            defined_views |= {view.view.as_id() for view in self.rules.last.views}
 
         errors: list[issues.NeatValidationError] = []
         for prop_no, prop in enumerate(self.properties):
             if prop.view and (view_id := prop.view.as_id()) not in defined_views:
                 errors.append(
                     issues.spreadsheet.NonExistingViewError(
                         column="View",
@@ -121,14 +128,19 @@
                         msg="",
                         input=None,
                         url=None,
                     )
                 )
         if self.metadata.schema_ is SchemaCompleteness.complete:
             defined_containers = {container.container.as_id() for container in self.containers or []}
+            if self.metadata.data_model_type == DataModelType.solution and self.rules.reference:
+                defined_containers |= {
+                    container.container.as_id() for container in self.rules.reference.containers or []
+                }
+
             for prop_no, prop in enumerate(self.properties):
                 if prop.container and (container_id := prop.container.as_id()) not in defined_containers:
                     errors.append(
                         issues.spreadsheet.NonExistingContainerError(
                             column="Container",
                             row=prop_no,
                             type="value_error.missing",
@@ -153,27 +165,24 @@
                             )
                         )
         self.issue_list.extend(errors)
 
     def _validate_extension(self) -> None:
         if self.metadata.schema_ is not SchemaCompleteness.extended:
             return None
-        if not self.rules.reference:
-            raise ValueError("The schema is set to 'extended', but no reference rules are provided to validate against")
-        is_solution = self.metadata.space != self.rules.reference.metadata.space
-        if is_solution:
-            return None
+        if not self.rules.last:
+            raise ValueError("The schema is set to 'extended', but no last rules are provided to validate against")
         if self.metadata.extension is ExtensionCategory.rebuild:
             # Everything is allowed
             return None
-        # Is an extension of an existing model.
         user_schema = self.rules.as_schema()
-        ref_schema = self.rules.reference.as_schema()
         new_containers = user_schema.containers.copy()
-        existing_containers = ref_schema.containers.copy()
+
+        last_schema = self.rules.last.as_schema()
+        existing_containers = last_schema.containers.copy()
 
         for container_id, container in new_containers.items():
             existing_container = existing_containers.get(container_id)
             if not existing_container or existing_container == container:
                 # No problem
                 continue
             new_dumped = container.dump()
@@ -185,22 +194,20 @@
                 issues.dms.ChangingContainerError(
                     container_id=container_id,
                     changed_properties=changed_properties or None,
                     changed_attributes=changed_attributes or None,
                 )
             )
 
-        if self.metadata.extension is ExtensionCategory.reshape and self.issue_list:
-            return None
-        elif self.metadata.extension is ExtensionCategory.reshape:
+        if self.metadata.extension is ExtensionCategory.reshape:
             # Reshape allows changes to views
             return None
 
         new_views = user_schema.views.copy()
-        existing_views = ref_schema.views.copy()
+        existing_views = last_schema.views.copy()
         for view_id, view in new_views.items():
             existing_view = existing_views.get(view_id)
             if not existing_view or existing_view == view:
                 # No problem
                 continue
             changed_attributes, changed_properties = self._changed_attributes_and_properties(
                 view.dump(), existing_view.dump()
@@ -209,22 +216,15 @@
                 issues.dms.ChangingViewError(
                     view_id=view_id,
                     changed_properties=changed_properties or None,
                     changed_attributes=changed_attributes or None,
                 )
             )
 
-    def _validate_performance(self) -> None:
-        # we can only validate performance on complete schemas due to the need
-        # to access all the container mappings
-        if self.metadata.schema_ is not SchemaCompleteness.complete:
-            return None
-
-        dms_schema = self.rules.as_schema()
-
+    def _validate_performance(self, dms_schema: DMSSchema) -> None:
         for view_id, view in dms_schema.views.items():
             mapped_containers = dms_schema._get_mapped_container_from_view(view_id)
 
             if mapped_containers and len(mapped_containers) > 10:
                 self.issue_list.append(
                     issues.dms.ViewMapsToTooManyContainersWarning(
                         view_id=view_id,
@@ -239,15 +239,15 @@
                     self.issue_list.append(
                         issues.dms.HasDataFilterAppliedToTooManyContainersWarning(
                             view_id=view_id,
                             container_ids=mapped_containers,
                         )
                     )
 
-    def _validate_best_practices(self) -> None:
+    def _validate_raw_filter(self) -> None:
         for view in self.views:
             if view.filter_ and isinstance(view.filter_, RawFilter):
                 self.issue_list.append(
                     issues.dms.RawFilterAppliedToViewWarning(
                         view_id=view.view.as_id(),
                     )
                 )
@@ -260,40 +260,7 @@
         new_attributes = {key: value for key, value in new_dumped.items() if key != "properties"}
         existing_attributes = {key: value for key, value in existing_dumped.items() if key != "properties"}
         changed_attributes = [key for key in new_attributes if new_attributes[key] != existing_attributes.get(key)]
         new_properties = new_dumped.get("properties", {})
         existing_properties = existing_dumped.get("properties", {})
         changed_properties = [prop for prop in new_properties if new_properties[prop] != existing_properties.get(prop)]
         return changed_attributes, changed_properties
-
-    def _validate_schema(self) -> None:
-        if self.metadata.schema_ is SchemaCompleteness.partial:
-            return None
-        elif self.metadata.schema_ is SchemaCompleteness.complete:
-            rules: DMSRules = self.rules
-        elif self.metadata.schema_ is SchemaCompleteness.extended:
-            if not self.rules.reference:
-                raise ValueError(
-                    "The schema is set to 'extended', but no reference rules are provided to validate against"
-                )
-            # This is an extension of the reference rules, we need to merge the two
-            rules = self.rules.model_copy(deep=True)
-            rules.properties.extend(self.rules.reference.properties.data)
-            existing_views = {view.view.as_id() for view in rules.views}
-            rules.views.extend([view for view in self.rules.reference.views if view.view.as_id() not in existing_views])
-            if rules.containers and self.rules.reference.containers:
-                existing_containers = {container.container.as_id() for container in rules.containers.data}
-                rules.containers.extend(
-                    [
-                        container
-                        for container in self.rules.reference.containers
-                        if container.container.as_id() not in existing_containers
-                    ]
-                )
-            elif not rules.containers and self.rules.reference.containers:
-                rules.containers = self.rules.reference.containers
-        else:
-            raise ValueError("Unknown schema completeness")
-
-        schema = rules.as_schema()
-        errors = schema.validate()
-        self.issue_list.extend(errors)
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/domain.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/domain.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/entities.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/entities.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/information/_converter.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/information/_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/information/_rules.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/information/_rules.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import math
 import sys
-import warnings
+from collections.abc import Callable
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, ClassVar, cast
 
 from pydantic import Field, field_serializer, field_validator, model_serializer, model_validator
 from pydantic_core.core_schema import SerializationInfo
 from rdflib import Namespace
 
-import cognite.neat.rules.issues.spreadsheet
 from cognite.neat.constants import PREFIXES
-from cognite.neat.rules import exceptions
+from cognite.neat.rules import exceptions, issues
+from cognite.neat.rules.issues.base import MultiValueError
 from cognite.neat.rules.models._base import (
     BaseMetadata,
     DataModelType,
     ExtensionCategory,
     ExtensionCategoryType,
     MatchType,
     RoleTypes,
@@ -40,42 +40,40 @@
     StrListType,
     VersionType,
 )
 from cognite.neat.rules.models.data_types import DataType
 from cognite.neat.rules.models.domain import DomainRules
 from cognite.neat.rules.models.entities import (
     ClassEntity,
-    Entity,
     EntityTypes,
     ParentClassEntity,
     ParentEntityList,
     ReferenceEntity,
     Undefined,
-    Unknown,
     UnknownEntity,
     URLEntity,
     _UndefinedType,
-    _UnknownType,
 )
 
 if TYPE_CHECKING:
     from cognite.neat.rules.models.dms._rules import DMSRules
 
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 
 class InformationMetadata(BaseMetadata):
     role: ClassVar[RoleTypes] = RoleTypes.information_architect
-    data_model_type: DataModelType = Field(DataModelType.solution, alias="dataModelType")
-    schema_: SchemaCompleteness = Field(alias="schema")
+    data_model_type: DataModelType = Field(DataModelType.enterprise, alias="dataModelType")
+    schema_: SchemaCompleteness = Field(SchemaCompleteness.partial, alias="schema")
     extension: ExtensionCategoryType | None = ExtensionCategory.addition
+
     prefix: PrefixType
     namespace: NamespaceType
 
     name: str = Field(
         alias="title",
         description="Human readable name of the data model",
         min_length=1,
@@ -93,22 +91,36 @@
     )
     creator: StrListType = Field(
         description=(
             "List of contributors to the data model creation, "
             "typically information architects are considered as contributors."
         ),
     )
+    license: str | None = None
+    rights: str | None = None
 
     @model_validator(mode="after")
     def extension_none_but_schema_extend(self) -> Self:
         if self.extension is None:
             self.extension = ExtensionCategory.addition
             return self
         return self
 
+    @field_validator("schema_", mode="plain")
+    def as_enum_schema(cls, value: str) -> SchemaCompleteness:
+        return SchemaCompleteness(value)
+
+    @field_validator("extension", mode="plain")
+    def as_enum_extension(cls, value: str) -> ExtensionCategory:
+        return ExtensionCategory(value)
+
+    @field_validator("data_model_type", mode="plain")
+    def as_enum_model_type(cls, value: str) -> DataModelType:
+        return DataModelType(value)
+
 
 class InformationClass(SheetEntity):
     """
     Class is a category of things that share a common set of attributes and relationships.
 
     Args:
         class_: The class ID of the class.
@@ -278,85 +290,32 @@
                         parent.prefix = self.metadata.prefix
             if class_.class_.prefix is Undefined:
                 class_.class_.prefix = self.metadata.prefix
 
         return self
 
     @model_validator(mode="after")
-    def validate_schema_completeness(self) -> Self:
-        # update expected_value_types
-
-        if self.metadata.schema_ == SchemaCompleteness.complete:
-            defined_classes = {str(class_.class_) for class_ in self.classes}
-            referred_classes = {str(property_.class_) for property_ in self.properties} | {
-                str(parent) for class_ in self.classes for parent in class_.parent or []
-            }
-            referred_types = {
-                str(property_.value_type)
-                for property_ in self.properties
-                if isinstance(property_.value_type, Entity)
-                and not isinstance(property_.value_type.suffix, _UnknownType)
-            }
-            if not referred_classes.issubset(defined_classes) or not referred_types.issubset(defined_classes):
-                missing_classes = referred_classes.difference(defined_classes).union(
-                    referred_types.difference(defined_classes)
-                )
-                raise exceptions.IncompleteSchema(missing_classes).to_pydantic_custom_error()
+    def post_validation(self) -> "InformationRules":
+        from ._validation import InformationPostValidation
 
+        issue_list = InformationPostValidation(self).validate()
+        if issue_list.warnings:
+            issue_list.trigger_warnings()
+        if issue_list.has_errors:
+            raise MultiValueError([error for error in issue_list if isinstance(error, issues.NeatValidationError)])
         return self
 
-    @model_validator(mode="after")
-    def validate_class_has_properties_or_parent(self) -> Self:
-        defined_classes = {class_.class_ for class_ in self.classes if class_.reference is None}
-        referred_classes = {property_.class_ for property_ in self.properties if property_.class_.suffix is not Unknown}
-        has_parent_classes = {class_.class_ for class_ in self.classes if class_.parent}
-        missing_classes = defined_classes.difference(referred_classes) - has_parent_classes
-        if missing_classes:
-            warnings.warn(
-                cognite.neat.rules.issues.spreadsheet.ClassNoPropertiesNoParentsWarning(
-                    [missing.versioned_id for missing in missing_classes]
-                ),
-                stacklevel=2,
-            )
-        return self
+    @model_serializer(mode="wrap", when_used="always")
+    def information_rules_serializer(self, handler: Callable, info: SerializationInfo) -> dict[str, Any]:
+        from ._serializer import _InformationRulesSerializer
+
+        dumped = cast(dict[str, Any], handler(self, info))
+        prefix = self.metadata.prefix
 
-    @model_serializer(mode="plain", when_used="always")
-    def information_rules_serializer(self, info: SerializationInfo) -> dict[str, Any]:
-        kwargs = vars(info)
-        default_prefix = f"{self.metadata.prefix}:" if self.metadata.prefix else ""
-
-        field_names = ["Class", "Value Type"] if info.by_alias else ["class_", "value_type"]
-        properties = []
-        for prop in self.properties:
-            dumped = prop.model_dump(**kwargs)
-            for field_name in field_names:
-                if value := dumped.get(field_name):
-                    dumped[field_name] = value.removeprefix(default_prefix)
-            properties.append(dumped)
-
-        field_names = ["Class"] if info.by_alias else ["class_"]
-        classes = []
-        parent_name = "Parent Class" if info.by_alias else "parent"
-        for cls in self.classes:
-            dumped = cls.model_dump(**kwargs)
-            for field_name in field_names:
-                if value := dumped.get(field_name):
-                    dumped[field_name] = value.removeprefix(default_prefix)
-            if value := dumped.get(parent_name):
-                dumped[parent_name] = ",".join(
-                    constraint.strip().removeprefix(default_prefix) for constraint in value.split(",")
-                )
-            classes.append(dumped)
-
-        return {
-            "Metadata" if info.by_alias else "metadata": self.metadata.model_dump(**kwargs),
-            "Classes" if info.by_alias else "classes": classes,
-            "Properties" if info.by_alias else "properties": properties,
-            "prefixes": {key: str(value) for key, value in self.prefixes.items()},
-        }
+        return _InformationRulesSerializer(info, prefix).clean(dumped)
 
     def as_domain_rules(self) -> DomainRules:
         from ._converter import _InformationRulesConverter
 
         return _InformationRulesConverter(self).as_domain_rules()
 
     def as_dms_architect_rules(self) -> "DMSRules":
@@ -364,25 +323,25 @@
 
         return _InformationRulesConverter(self).as_dms_architect_rules()
 
     def reference_self(self) -> "InformationRules":
         new_self = self.model_copy(deep=True)
         for prop in new_self.properties:
             prop.reference = ReferenceEntity(
-                prefix=prop.class_.prefix
-                if not isinstance(prop.class_.prefix, _UndefinedType)
-                else self.metadata.prefix,
+                prefix=(
+                    prop.class_.prefix if not isinstance(prop.class_.prefix, _UndefinedType) else self.metadata.prefix
+                ),
                 suffix=prop.class_.suffix,
                 version=prop.class_.version,
                 property=prop.property_,
             )
 
         for cls_ in new_self.classes:
             cls_.reference = ReferenceEntity(
-                prefix=cls_.class_.prefix
-                if not isinstance(cls_.class_.prefix, _UndefinedType)
-                else self.metadata.prefix,
+                prefix=(
+                    cls_.class_.prefix if not isinstance(cls_.class_.prefix, _UndefinedType) else self.metadata.prefix
+                ),
                 suffix=cls_.class_.suffix,
                 version=cls_.class_.version,
             )
 
         return new_self
```

### Comparing `cognite_neat-0.77.3/cognite/neat/rules/models/wrapped_entities.py` & `cognite_neat-0.77.4/cognite/neat/rules/models/wrapped_entities.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/utils/cdf_classes.py` & `cognite_neat-0.77.4/cognite/neat/utils/cdf_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.77.4/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.77.4/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.77.4/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.77.4/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/utils/exceptions.py` & `cognite_neat-0.77.4/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.77.4/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/utils/text.py` & `cognite_neat-0.77.4/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/utils/utils.py` & `cognite_neat-0.77.4/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/utils/xml.py` & `cognite_neat-0.77.4/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.77.4/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/base.py` & `cognite_neat-0.77.4/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.77.4/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.77.4/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/manager.py` & `cognite_neat-0.77.4/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.77.4/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.77.4/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/model.py` & `cognite_neat-0.77.4/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/current/graph_extractor.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/current/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/current/graph_loader.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/current/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/current/graph_store.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/current/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/current/rules_exporter.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/current/rules_exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -265,39 +265,62 @@
             value="input",
             label="The role to use for the exported spreadsheet. If provided, the rules will be converted to "
             "this role format before being written to excel. If not provided, the role from the input "
             "rules will be used.",
             options=["input", *RoleTypes.__members__.keys()],
         ),
         Configurable(
-            name="Is Reference",
-            value="False",
-            label="Export rules as reference rules. If provided, the rules will be exported as reference rules. ",
-            options=["True", "False"],
+            name="Dump Format",
+            value="user",
+            label="How to dump the rules to the Excel file.\n"
+            "'user' - just as is.\n'reference' - enterprise model used as basis for a solution model\n"
+            "'last' - used when updating a data model.",
+            options=list(exporters.ExcelExporter.dump_options),
+        ),
+        Configurable(
+            name="New Data Model ID",
+            value="",
+            label="If you chose Dump Format 'reference', the provided ID will be use in the new medata sheet. "
+            "Expected format 'sp_space:my_external_id'.",
+            options=list(exporters.ExcelExporter.dump_options),
         ),
         Configurable(
             name="File path",
             value="",
             label="File path to the generated Excel file.For example: 'staging/exported-rules.xlsx'",
         ),
     ]
 
     def run(self, rules: MultiRuleData) -> FlowMessage:  # type: ignore[override, syntax]
         if self.configs is None or self.data_store_path is None:
             raise StepNotInitialized(type(self).__name__)
 
-        is_reference = self.configs.get("Is Reference") == "True"
+        dump_format = self.configs.get("Dump Format", "user")
         styling = cast(exporters.ExcelExporter.Style, self.configs.get("Styling", "default"))
         role = self.configs.get("Output role format")
         output_role = None
         if role != "input" and role is not None:
             output_role = RoleTypes[role]
 
-        dump_as = "reference" if is_reference else "user"
-        excel_exporter = exporters.ExcelExporter(styling=styling, output_role=output_role, dump_as=dump_as)  # type: ignore[arg-type]
+        new_model_str = self.configs.get("New Data Model ID")
+        new_model_id: tuple[str, str] | None = None
+        if new_model_str and ":" in new_model_str:
+            new_model_id = tuple(new_model_str.split(":", 1))  # type: ignore[assignment]
+        elif new_model_str:
+            return FlowMessage(
+                error_text="New Data Model ID must be in the format 'sp_space:my_external_id'!",
+                step_execution_status=StepExecutionStatus.ABORT_AND_FAIL,
+            )
+
+        excel_exporter = exporters.ExcelExporter(
+            styling=styling,
+            output_role=output_role,
+            dump_as=dump_format,  # type: ignore[arg-type]
+            new_model_id=new_model_id,
+        )
 
         rule_instance: Rules
         if rules.domain:
             rule_instance = rules.domain
         elif rules.information:
             rule_instance = rules.information
         elif rules.dms:
```

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/current/rules_importer.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/current/rules_importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
 from pathlib import Path
 from typing import ClassVar
 
 from cognite.client import CogniteClient
+from cognite.client.data_classes.data_modeling import DataModelId
 
 from cognite.neat.rules import importers
 from cognite.neat.rules.issues.formatters import FORMATTER_BY_NAME
 from cognite.neat.rules.models import RoleTypes
 from cognite.neat.rules.models.entities import DataModelEntity, DMSUnknownEntity
 from cognite.neat.workflows._exceptions import StepNotInitialized
 from cognite.neat.workflows.model import FlowMessage, StepExecutionStatus
@@ -181,14 +182,21 @@
             name="Data model id",
             value="",
             label="The ID of the Data Model to import. Written at 'my_space:my_data_model(version=1)'",
             type="string",
             required=True,
         ),
         Configurable(
+            name="Reference data model id",
+            value=None,
+            label="The ID of the Reference Data Model to import. Written at 'my_space:my_data_model(version=1)'. "
+            "This is typically an enterprise data model when you want to import a solution model",
+            type="string",
+        ),
+        Configurable(
             name="Report formatter",
             value=next(iter(FORMATTER_BY_NAME.keys())),
             label="The format of the report for the validation of the rules",
             options=list(FORMATTER_BY_NAME),
         ),
         Configurable(
             name="Role",
@@ -210,16 +218,27 @@
         datamodel_entity = DataModelEntity.load(datamodel_id_str)
         if isinstance(datamodel_entity, DMSUnknownEntity):
             error_text = (
                 f"Data model id should be in the format 'my_space:my_data_model(version=1)' "
                 f"or 'my_space:my_data_model', failed to parse space from {datamodel_id_str}"
             )
             return FlowMessage(error_text=error_text, step_execution_status=StepExecutionStatus.ABORT_AND_FAIL)
+        ref_datamodel_str = self.configs.get("Reference data model id")
+        ref_model_id: DataModelId | None = None
+        if ref_datamodel_str is not None:
+            ref_model = DataModelEntity.load(ref_datamodel_str)
+            if isinstance(ref_model, DMSUnknownEntity):
+                error_text = (
+                    f"Reference data model id should be in the format 'my_space:my_data_model(version=1)' "
+                    f"or 'my_space:my_data_model', failed to parse space from {ref_datamodel_str}"
+                )
+                return FlowMessage(error_text=error_text, step_execution_status=StepExecutionStatus.ABORT_AND_FAIL)
+            ref_model_id = ref_model.as_id()
 
-        dms_importer = importers.DMSImporter.from_data_model_id(cdf_client, datamodel_entity.as_id())
+        dms_importer = importers.DMSImporter.from_data_model_id(cdf_client, datamodel_entity.as_id(), ref_model_id)
 
         # if role is None, it will be inferred from the rules file
         role = self.configs.get("Role")
         role_enum = None
         if role != "infer" and role is not None:
             role_enum = RoleTypes[role]
```

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/current/rules_validator.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/current/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/io/io_steps.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/io/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/graph_loader.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/graph_store.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/lib/legacy/rules_importer.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/lib/legacy/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.77.4/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/tasks.py` & `cognite_neat-0.77.4/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/cognite/neat/workflows/triggers.py` & `cognite_neat-0.77.4/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.77.3/pyproject.toml` & `cognite_neat-0.77.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.77.3"
+version = "0.77.4"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.77.3/PKG-INFO` & `cognite_neat-0.77.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.77.3
+Version: 0.77.4
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

