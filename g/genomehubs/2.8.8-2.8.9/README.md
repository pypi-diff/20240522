# Comparing `tmp/genomehubs-2.8.8.tar.gz` & `tmp/genomehubs-2.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomehubs-2.8.8.tar", last modified: Fri May 17 10:50:10 2024, max compression
+gzip compressed data, was "genomehubs-2.8.9.tar", last modified: Fri May 17 12:24:08 2024, max compression
```

## Comparing `genomehubs-2.8.8.tar` & `genomehubs-2.8.9.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:50:10.782056 genomehubs-2.8.8/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-17 10:49:33.000000 genomehubs-2.8.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-17 10:49:33.000000 genomehubs-2.8.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-17 10:49:33.000000 genomehubs-2.8.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-17 10:49:33.000000 genomehubs-2.8.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 10:49:33.000000 genomehubs-2.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-17 10:49:33.000000 genomehubs-2.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-05-17 10:50:10.782056 genomehubs-2.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-05-17 10:49:33.000000 genomehubs-2.8.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 10:49:33.000000 genomehubs-2.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-17 10:50:10.782056 genomehubs-2.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-17 10:49:33.000000 genomehubs-2.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:50:10.762056 genomehubs-2.8.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:50:10.766056 genomehubs-2.8.8/src/genomehubs/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:50:10.766056 genomehubs-2.8.8/src/genomehubs/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/config/dist.config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/genomehubs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:50:10.770056 genomehubs-2.8.8/src/genomehubs/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/btk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/busco.py
--rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15224 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/es_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    34496 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/fill.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/gbif.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/geo.py
--rw-r--r--   0 runner    (1001) docker     (127)    40630 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    22460 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/init.py
--rw-r--r--   0 runner    (1001) docker     (127)    25539 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    37857 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/taxon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/wikidata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/lib/window.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:50:10.774057 genomehubs-2.8.8/src/genomehubs/templates/
--rw-r--r--   0 runner    (1001) docker     (127)   136093 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/ATTR_ancestral_unit.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8108 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/ATTR_assembly.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/ATTR_btk.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/ATTR_busco.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/ATTR_feature.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/ATTR_sample.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/ATTR_sra.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/ATTR_window_stats.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/TAXON_assembly.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)    16228 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/assembly.json
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/assembly.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/btk.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/busco.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/busco_feature.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/feature.json
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/file.json
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/identifiers.json
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/organelle.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/sample.json
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/sample.types.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:50:10.778056 genomehubs-2.8.8/src/genomehubs/templates/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/analysis_lookup.json
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/analysis_suggest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/assembly_lookup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/assembly_suggest.json
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/attribute_types_by_group.json
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/attribute_values_by_taxon.json
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/attributes_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/attributes_identifiers_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/attributes_names_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/file_lookup.json
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/file_suggest.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/max_nested_value.json
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/max_nested_value_by_key_value.json
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/max_nested_value_by_type.json
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/search_by_taxon.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_attributes_by_taxon_id.json
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_by_any_name.json
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_by_name.json
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_by_specific_name.json
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_lookup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_names.json
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_names_by_root.json
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_suggest.json
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/taxonomy_node_by_taxon_id.json
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/scripts/value_by_type_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/sra.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19022 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/taxon.json
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/taxon.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/taxonomy.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/wikidata.names.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/window_full.types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-17 10:49:33.000000 genomehubs-2.8.8/src/genomehubs/templates/window_stats.types.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:50:10.766056 genomehubs-2.8.8/src/genomehubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-05-17 10:50:10.000000 genomehubs-2.8.8/src/genomehubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-17 10:50:10.000000 genomehubs-2.8.8/src/genomehubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:50:10.000000 genomehubs-2.8.8/src/genomehubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-17 10:50:10.000000 genomehubs-2.8.8/src/genomehubs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-17 10:50:10.000000 genomehubs-2.8.8/src/genomehubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 10:50:10.000000 genomehubs-2.8.8/src/genomehubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:08.980759 genomehubs-2.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-17 12:23:34.000000 genomehubs-2.8.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-17 12:23:34.000000 genomehubs-2.8.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-17 12:23:34.000000 genomehubs-2.8.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-17 12:23:34.000000 genomehubs-2.8.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 12:23:34.000000 genomehubs-2.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-17 12:23:34.000000 genomehubs-2.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-05-17 12:24:08.980759 genomehubs-2.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-05-17 12:23:34.000000 genomehubs-2.8.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 12:23:34.000000 genomehubs-2.8.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-17 12:24:08.980759 genomehubs-2.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-17 12:23:34.000000 genomehubs-2.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:08.960759 genomehubs-2.8.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:08.964758 genomehubs-2.8.9/src/genomehubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:08.964758 genomehubs-2.8.9/src/genomehubs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/config/dist.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/genomehubs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:08.968759 genomehubs-2.8.9/src/genomehubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/btk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/busco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15224 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/es_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34496 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/gbif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40630 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22460 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25539 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37857 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/taxon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/wikidata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/lib/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:08.976759 genomehubs-2.8.9/src/genomehubs/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)   136093 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/ATTR_ancestral_unit.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8108 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/ATTR_assembly.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/ATTR_btk.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/ATTR_busco.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/ATTR_feature.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/ATTR_sample.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/ATTR_sra.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/ATTR_window_stats.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/TAXON_assembly.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16228 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/assembly.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/assembly.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/btk.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/busco.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/busco_feature.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/feature.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/file.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/identifiers.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/organelle.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/sample.types.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:08.980759 genomehubs-2.8.9/src/genomehubs/templates/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/analysis_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/analysis_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/assembly_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/assembly_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/attribute_types_by_group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/attribute_values_by_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/attributes_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/attributes_identifiers_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/attributes_names_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/file_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/file_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/max_nested_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/max_nested_value_by_key_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/max_nested_value_by_type.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/search_by_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_attributes_by_taxon_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_by_any_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_by_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_by_specific_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_names_by_root.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/taxonomy_node_by_taxon_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/scripts/value_by_type_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/sra.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19022 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/taxon.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/taxon.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/taxonomy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/wikidata.names.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/window_full.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-17 12:23:34.000000 genomehubs-2.8.9/src/genomehubs/templates/window_stats.types.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:08.964758 genomehubs-2.8.9/src/genomehubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-05-17 12:24:08.000000 genomehubs-2.8.9/src/genomehubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-17 12:24:08.000000 genomehubs-2.8.9/src/genomehubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:24:08.000000 genomehubs-2.8.9/src/genomehubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-17 12:24:08.000000 genomehubs-2.8.9/src/genomehubs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-17 12:24:08.000000 genomehubs-2.8.9/src/genomehubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 12:24:08.000000 genomehubs-2.8.9/src/genomehubs.egg-info/top_level.txt
```

### Comparing `genomehubs-2.8.8/CONTRIBUTING.rst` & `genomehubs-2.8.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/LICENSE` & `genomehubs-2.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/PKG-INFO` & `genomehubs-2.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomehubs
-Version: 2.8.8
+Version: 2.8.9
 Summary: GenomeHubs
 Home-page: https://github.com/genomehubs/genomehubs
 Author: genomehubs
 Author-email: genomehubs@genomehubs.org
 Project-URL: Bug Reports, https://github.com/genomehubs/genomehubs/issues
 Project-URL: Source, https://github.com/genomehubs/genomehubs
 Keywords: bioinformatics
```

### Comparing `genomehubs-2.8.8/README.rst` & `genomehubs-2.8.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     :alt: Install with Conda
     :target: https://anaconda.org/tolkit/genomehubs
 
 .. |platforms| image:: https://anaconda.org/tolkit/genomehubs/badges/platforms.svg
     :alt: Conda platforms
     :target: https://anaconda.org/tolkit/genomehubs
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/genomehubs/genomehubs/2.8.8.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/genomehubs/genomehubs/2.8.9.svg
     :alt: Commits since latest release
-    :target: https://github.com/genomehubs/genomehubs/compare/2.8.8...main
+    :target: https://github.com/genomehubs/genomehubs/compare/2.8.9...main
 
 .. |license| image:: https://anaconda.org/tolkit/genomehubs/badges/license.svg
     :alt: MIT License
     :target: https://anaconda.org/tolkit/genomehubs
 
 .. end-badges
```

### Comparing `genomehubs-2.8.8/setup.cfg` & `genomehubs-2.8.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/setup.py` & `genomehubs-2.8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="genomehubs",  # Required
-    version="2.8.8",
+    version="2.8.9",
     description="GenomeHubs",  # Optional
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
```

### Comparing `genomehubs-2.8.8/src/genomehubs/config/dist.config.yaml` & `genomehubs-2.8.9/src/genomehubs/config/dist.config.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/genomehubs.py` & `genomehubs-2.8.9/src/genomehubs/genomehubs.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/attributes.py` & `genomehubs-2.8.9/src/genomehubs/lib/attributes.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/btk.py` & `genomehubs-2.8.9/src/genomehubs/lib/btk.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/busco.py` & `genomehubs-2.8.9/src/genomehubs/lib/busco.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/config.py` & `genomehubs-2.8.9/src/genomehubs/lib/config.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/directory.py` & `genomehubs-2.8.9/src/genomehubs/lib/directory.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/es_functions.py` & `genomehubs-2.8.9/src/genomehubs/lib/es_functions.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/files.py` & `genomehubs-2.8.9/src/genomehubs/lib/files.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/fill.py` & `genomehubs-2.8.9/src/genomehubs/lib/fill.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/gbif.py` & `genomehubs-2.8.9/src/genomehubs/lib/gbif.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/geo.py` & `genomehubs-2.8.9/src/genomehubs/lib/geo.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/hub.py` & `genomehubs-2.8.9/src/genomehubs/lib/hub.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/index.py` & `genomehubs-2.8.9/src/genomehubs/lib/index.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/init.py` & `genomehubs-2.8.9/src/genomehubs/lib/init.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/ncbi.py` & `genomehubs-2.8.9/src/genomehubs/lib/ncbi.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/parse.py` & `genomehubs-2.8.9/src/genomehubs/lib/parse.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/run.py` & `genomehubs-2.8.9/src/genomehubs/lib/run.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/sample.py` & `genomehubs-2.8.9/src/genomehubs/lib/sample.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/search.py` & `genomehubs-2.8.9/src/genomehubs/lib/search.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/taxon.py` & `genomehubs-2.8.9/src/genomehubs/lib/taxon.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/taxonomy.py` & `genomehubs-2.8.9/src/genomehubs/lib/taxonomy.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/test.py` & `genomehubs-2.8.9/src/genomehubs/lib/test.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/utils.py` & `genomehubs-2.8.9/src/genomehubs/lib/utils.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/validate.py` & `genomehubs-2.8.9/src/genomehubs/lib/validate.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/wikidata.py` & `genomehubs-2.8.9/src/genomehubs/lib/wikidata.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/lib/window.py` & `genomehubs-2.8.9/src/genomehubs/lib/window.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/ATTR_ancestral_unit.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/ATTR_ancestral_unit.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/ATTR_assembly.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/ATTR_assembly.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/ATTR_btk.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/ATTR_btk.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/ATTR_busco.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/ATTR_busco.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/ATTR_feature.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/ATTR_feature.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/ATTR_sample.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/ATTR_sample.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/ATTR_sra.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/ATTR_sra.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/ATTR_window_stats.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/ATTR_window_stats.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/TAXON_assembly.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/TAXON_assembly.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/analysis.json` & `genomehubs-2.8.9/src/genomehubs/templates/analysis.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/assembly.json` & `genomehubs-2.8.9/src/genomehubs/templates/assembly.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/assembly.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/assembly.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/attributes.json` & `genomehubs-2.8.9/src/genomehubs/templates/attributes.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/btk.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/btk.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/busco.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/busco.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/busco_feature.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/busco_feature.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/feature.json` & `genomehubs-2.8.9/src/genomehubs/templates/feature.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/file.json` & `genomehubs-2.8.9/src/genomehubs/templates/file.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/identifiers.json` & `genomehubs-2.8.9/src/genomehubs/templates/identifiers.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/organelle.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/organelle.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/sample.json` & `genomehubs-2.8.9/src/genomehubs/templates/sample.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/sample.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/sample.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/assembly_lookup.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/assembly_lookup.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/assembly_suggest.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/assembly_suggest.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/attribute_values_by_taxon.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/attribute_values_by_taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/max_nested_value_by_type.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/max_nested_value_by_type.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_by_any_name.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_by_any_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_by_lineage.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_by_name.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_by_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_by_specific_name.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_by_specific_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_lookup.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_lookup.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/taxon_suggest.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/taxon_suggest.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/scripts/value_by_type_by_lineage.json` & `genomehubs-2.8.9/src/genomehubs/templates/scripts/value_by_type_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/taxon.json` & `genomehubs-2.8.9/src/genomehubs/templates/taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/taxon.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/taxon.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/taxonomy.json` & `genomehubs-2.8.9/src/genomehubs/templates/taxonomy.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/window_full.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/window_full.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs/templates/window_stats.types.yaml` & `genomehubs-2.8.9/src/genomehubs/templates/window_stats.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.8.8/src/genomehubs.egg-info/PKG-INFO` & `genomehubs-2.8.9/src/genomehubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomehubs
-Version: 2.8.8
+Version: 2.8.9
 Summary: GenomeHubs
 Home-page: https://github.com/genomehubs/genomehubs
 Author: genomehubs
 Author-email: genomehubs@genomehubs.org
 Project-URL: Bug Reports, https://github.com/genomehubs/genomehubs/issues
 Project-URL: Source, https://github.com/genomehubs/genomehubs
 Keywords: bioinformatics
```

### Comparing `genomehubs-2.8.8/src/genomehubs.egg-info/SOURCES.txt` & `genomehubs-2.8.9/src/genomehubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

