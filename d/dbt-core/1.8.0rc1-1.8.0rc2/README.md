# Comparing `tmp/dbt_core-1.8.0rc1.tar.gz` & `tmp/dbt_core-1.8.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_core-1.8.0rc1.tar", last modified: Thu May  2 18:57:54 2024, max compression
+gzip compressed data, was "dbt_core-1.8.0rc2.tar", last modified: Wed May  8 00:59:30 2024, max compression
```

## Comparing `dbt_core-1.8.0rc1.tar` & `dbt_core-1.8.0rc2.tar`

### file list

```diff
@@ -1,266 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.532992 dbt_core-1.8.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-02 18:57:54.532992 dbt_core-1.8.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.488993 dbt_core-1.8.0rc1/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.488993 dbt_core-1.8.0rc1/dbt/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.488993 dbt_core-1.8.0rc1/dbt/artifacts/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/exceptions/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.488993 dbt_core-1.8.0rc1/dbt/artifacts/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.492992 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/owner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/saved_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/semantic_layer_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/semantic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/source_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/sql_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/unit_test_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.492992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.492992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/catalog/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/catalog/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/catalog/v1/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/freshness/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/freshness/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/freshness/v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/freshness/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/freshness/v3/freshness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/manifest/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/manifest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/manifest/v12/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/manifest/v12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/manifest/v12/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/run/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/run/v5/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/run/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/run/v5/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/upgrades/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/upgrades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/upgrades/upgrade_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.500992 dbt_core-1.8.0rc1/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20277 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    18831 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    21775 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.500992 dbt_core-1.8.0rc1/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23813 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.500992 dbt_core-1.8.0rc1/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    32085 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.504993 dbt_core-1.8.0rc1/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24310 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    68635 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/query_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.504993 dbt_core-1.8.0rc1/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.508993 dbt_core-1.8.0rc1/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65821 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/node_args.py
--rw-r--r--   0 runner    (1001) docker     (127)    55099 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/semantic_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    22773 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.508993 dbt_core-1.8.0rc1/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.480993 dbt_core-1.8.0rc1/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.508993 dbt_core-1.8.0rc1/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.508993 dbt_core-1.8.0rc1/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (127)   101044 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/events/core_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/events/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    55599 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    49209 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    35223 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.484993 dbt_core-1.8.0rc1/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.516992 dbt_core-1.8.0rc1/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.516992 dbt_core-1.8.0rc1/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.516992 dbt_core-1.8.0rc1/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (127)    16025 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/mp_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.520992 dbt_core-1.8.0rc1/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    19178 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)    80146 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    23806 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    53594 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (127)    17653 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/schema_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    29540 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/schema_yaml_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    43568 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)    15421 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    25079 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/unit_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.520992 dbt_core-1.8.0rc1/dbt/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/plugins/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/plugins/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/plugins/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/selected_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.524992 dbt_core-1.8.0rc1/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17429 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/clone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/deps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.528992 dbt_core-1.8.0rc1/dbt/task/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/docs/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)  1509668 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/docs/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    18669 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26168 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    15067 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.528992 dbt_core-1.8.0rc1/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.528992 dbt_core-1.8.0rc1/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20559 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.532992 dbt_core-1.8.0rc1/dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:57:54.532992 dbt_core-1.8.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.843582 dbt_core-1.8.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-08 00:59:30.839582 dbt_core-1.8.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.803582 dbt_core-1.8.0rc2/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.803582 dbt_core-1.8.0rc2/dbt/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.803582 dbt_core-1.8.0rc2/dbt/artifacts/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/exceptions/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.807582 dbt_core-1.8.0rc2/dbt/artifacts/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.811582 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/owner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/saved_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/semantic_layer_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/semantic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/source_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/sql_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/unit_test_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.811582 dbt_core-1.8.0rc2/dbt/artifacts/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.811582 dbt_core-1.8.0rc2/dbt/artifacts/schemas/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.811582 dbt_core-1.8.0rc2/dbt/artifacts/schemas/catalog/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/catalog/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/catalog/v1/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.811582 dbt_core-1.8.0rc2/dbt/artifacts/schemas/freshness/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/freshness/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.811582 dbt_core-1.8.0rc2/dbt/artifacts/schemas/freshness/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/freshness/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/freshness/v3/freshness.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.811582 dbt_core-1.8.0rc2/dbt/artifacts/schemas/manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/manifest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.811582 dbt_core-1.8.0rc2/dbt/artifacts/schemas/manifest/v12/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/manifest/v12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/manifest/v12/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.811582 dbt_core-1.8.0rc2/dbt/artifacts/schemas/run/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.811582 dbt_core-1.8.0rc2/dbt/artifacts/schemas/run/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/run/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/run/v5/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.811582 dbt_core-1.8.0rc2/dbt/artifacts/schemas/upgrades/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/upgrades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/schemas/upgrades/upgrade_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.811582 dbt_core-1.8.0rc2/dbt/artifacts/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/artifacts/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.815582 dbt_core-1.8.0rc2/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20277 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18831 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21775 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/cli/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.815582 dbt_core-1.8.0rc2/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23813 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.815582 dbt_core-1.8.0rc2/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32085 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.819582 dbt_core-1.8.0rc2/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24310 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68635 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/context/query_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.819582 dbt_core-1.8.0rc2/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.823582 dbt_core-1.8.0rc2/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65763 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/graph/node_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55146 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/graph/semantic_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22867 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.823582 dbt_core-1.8.0rc2/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.799582 dbt_core-1.8.0rc2/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.823582 dbt_core-1.8.0rc2/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.823582 dbt_core-1.8.0rc2/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.823582 dbt_core-1.8.0rc2/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101044 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/events/core_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/events/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55599 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49209 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.827582 dbt_core-1.8.0rc2/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35223 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.827582 dbt_core-1.8.0rc2/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.827582 dbt_core-1.8.0rc2/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.827582 dbt_core-1.8.0rc2/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.827582 dbt_core-1.8.0rc2/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.799582 dbt_core-1.8.0rc2/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.827582 dbt_core-1.8.0rc2/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.827582 dbt_core-1.8.0rc2/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.827582 dbt_core-1.8.0rc2/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.827582 dbt_core-1.8.0rc2/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16025 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/mp_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.831582 dbt_core-1.8.0rc2/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19178 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80184 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23806 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53594 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17653 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/schema_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29540 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/schema_yaml_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43568 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15421 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25079 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/parser/unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.831582 dbt_core-1.8.0rc2/dbt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/plugins/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/plugins/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/plugins/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/selected_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.835582 dbt_core-1.8.0rc2/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17429 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/deps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.839582 dbt_core-1.8.0rc2/dbt/task/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/docs/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1509668 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/docs/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18669 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26168 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15067 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.839582 dbt_core-1.8.0rc2/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.839582 dbt_core-1.8.0rc2/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20559 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:30.839582 dbt_core-1.8.0rc2/dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-08 00:59:30.000000 dbt_core-1.8.0rc2/dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-08 00:59:30.000000 dbt_core-1.8.0rc2/dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:59:30.000000 dbt_core-1.8.0rc2/dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 00:59:30.000000 dbt_core-1.8.0rc2/dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:59:30.000000 dbt_core-1.8.0rc2/dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-08 00:59:30.000000 dbt_core-1.8.0rc2/dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 00:59:30.000000 dbt_core-1.8.0rc2/dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:59:30.843582 dbt_core-1.8.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-08 00:59:17.000000 dbt_core-1.8.0rc2/setup.py
```

### Comparing `dbt_core-1.8.0rc1/PKG-INFO` & `dbt_core-1.8.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.8.0rc1
+Version: 1.8.0rc2
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0rc1 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0rc2 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `dbt_core-1.8.0rc1/README.md` & `dbt_core-1.8.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/exceptions/schemas.py` & `dbt_core-1.8.0rc2/dbt/artifacts/exceptions/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/__init__.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/base.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/base.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/types.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/types.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/components.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/components.py`

 * *Files 4% similar despite different names*

```diff
@@ -192,14 +192,20 @@
     build_path: Optional[str] = None
     unrendered_config: Dict[str, Any] = field(default_factory=dict)
     created_at: float = field(default_factory=lambda: time.time())
     config_call_dict: Dict[str, Any] = field(default_factory=dict)
     relation_name: Optional[str] = None
     raw_code: str = ""
 
+    def __post_serialize__(self, dct: Dict, context: Optional[Dict] = None):
+        dct = super().__post_serialize__(dct, context)
+        if context and context.get("artifact") and "config_call_dict" in dct:
+            del dct["config_call_dict"]
+        return dct
+
 
 @dataclass
 class CompiledResource(ParsedResource):
     """Contains attributes necessary for SQL files and nodes with refs, sources, etc,
     so all ManifestNodes except SeedNode."""
 
     language: str = "sql"
@@ -211,16 +217,16 @@
     compiled: bool = False
     compiled_code: Optional[str] = None
     extra_ctes_injected: bool = False
     extra_ctes: List[InjectedCTE] = field(default_factory=list)
     _pre_injected_sql: Optional[str] = None
     contract: Contract = field(default_factory=Contract)
 
-    def __post_serialize__(self, dct):
-        dct = super().__post_serialize__(dct)
+    def __post_serialize__(self, dct: Dict, context: Optional[Dict] = None):
+        dct = super().__post_serialize__(dct, context)
         if "_pre_injected_sql" in dct:
             del dct["_pre_injected_sql"]
         # Remove compiled attributes
         if "compiled" in dct and dct["compiled"] is False:
             del dct["compiled"]
             del dct["extra_ctes_injected"]
             del dct["extra_ctes"]
```

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/config.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/config.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/exposure.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/exposure.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/generic_test.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/macro.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/macro.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/metric.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/model.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import Literal, Optional, List
+from typing import Dict, Literal, Optional, List
 from datetime import datetime
 from dbt_common.contracts.config.base import MergeBehavior
 from dbt_common.contracts.constraints import ModelLevelConstraint
 from dbt.artifacts.resources.v1.config import NodeConfig
 from dbt.artifacts.resources.types import AccessType, NodeType
 from dbt.artifacts.resources.v1.components import DeferRelation, NodeVersion, CompiledResource
 
@@ -22,7 +22,13 @@
     access: AccessType = AccessType.Protected
     config: ModelConfig = field(default_factory=ModelConfig)
     constraints: List[ModelLevelConstraint] = field(default_factory=list)
     version: Optional[NodeVersion] = None
     latest_version: Optional[NodeVersion] = None
     deprecation_date: Optional[datetime] = None
     defer_relation: Optional[DeferRelation] = None
+
+    def __post_serialize__(self, dct: Dict, context: Optional[Dict] = None):
+        dct = super().__post_serialize__(dct, context)
+        if context and context.get("artifact") and "defer_relation" in dct:
+            del dct["defer_relation"]
+        return dct
```

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/saved_query.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/saved_query.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/seed.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/seed.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import Optional, Literal
+from typing import Dict, Optional, Literal
 from dbt_common.dataclass_schema import ValidationError
 from dbt.artifacts.resources.types import NodeType
 from dbt.artifacts.resources.v1.components import MacroDependsOn, DeferRelation, ParsedResource
 from dbt.artifacts.resources.v1.config import NodeConfig
 
 
 @dataclass
@@ -24,7 +24,13 @@
     resource_type: Literal[NodeType.Seed]
     config: SeedConfig = field(default_factory=SeedConfig)
     # seeds need the root_path because the contents are not loaded initially
     # and we need the root_path to load the seed later
     root_path: Optional[str] = None
     depends_on: MacroDependsOn = field(default_factory=MacroDependsOn)
     defer_relation: Optional[DeferRelation] = None
+
+    def __post_serialize__(self, dct: Dict, context: Optional[Dict] = None):
+        dct = super().__post_serialize__(dct, context)
+        if context and context.get("artifact") and "defer_relation" in dct:
+            del dct["defer_relation"]
+        return dct
```

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/semantic_layer_components.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/semantic_layer_components.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/semantic_model.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/singular_test.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/snapshot.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/snapshot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, List, Optional, Literal
+from typing import Dict, Union, List, Optional, Literal
 from dataclasses import dataclass
 from dbt_common.dataclass_schema import ValidationError
 from dbt.artifacts.resources.types import NodeType
 from dbt.artifacts.resources.v1.components import CompiledResource, DeferRelation
 from dbt.artifacts.resources.v1.config import NodeConfig
 
 
@@ -60,7 +60,13 @@
 
 
 @dataclass
 class Snapshot(CompiledResource):
     resource_type: Literal[NodeType.Snapshot]
     config: SnapshotConfig
     defer_relation: Optional[DeferRelation] = None
+
+    def __post_serialize__(self, dct, context: Optional[Dict] = None):
+        dct = super().__post_serialize__(dct, context)
+        if context and context.get("artifact") and "defer_relation" in dct:
+            del dct["defer_relation"]
+        return dct
```

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/source_definition.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/source_definition.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/unit_test_definition.py` & `dbt_core-1.8.0rc2/dbt/artifacts/resources/v1/unit_test_definition.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/schemas/base.py` & `dbt_core-1.8.0rc2/dbt/artifacts/schemas/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def __str__(self) -> str:
         return BASE_SCHEMAS_URL + self.path
 
 
 class Writable:
     def write(self, path: str):
-        write_json(path, self.to_dict(omit_none=False))  # type: ignore
+        write_json(path, self.to_dict(omit_none=False, context={"artifact": True}))  # type: ignore
 
 
 class Readable:
     @classmethod
     def read(cls, path: str):
         try:
             data = read_json(path)
@@ -56,16 +56,16 @@
 class BaseArtifactMetadata(dbtClassMixin):
     dbt_schema_version: str
     dbt_version: str = __version__
     generated_at: datetime = dataclasses.field(default_factory=datetime.utcnow)
     invocation_id: Optional[str] = dataclasses.field(default_factory=get_invocation_id)
     env: Dict[str, str] = dataclasses.field(default_factory=get_metadata_vars)
 
-    def __post_serialize__(self, dct):
-        dct = super().__post_serialize__(dct)
+    def __post_serialize__(self, dct: Dict, context: Optional[Dict] = None):
+        dct = super().__post_serialize__(dct, context)
         if dct["generated_at"] and dct["generated_at"].endswith("+00:00"):
             dct["generated_at"] = dct["generated_at"].replace("+00:00", "") + "Z"
         return dct
 
 
 # This is used as a class decorator to set the schema_version in the
 # 'dbt_schema_version' class attribute. (It's copied into the metadata objects.)
```

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/schemas/catalog/v1/catalog.py` & `dbt_core-1.8.0rc2/dbt/artifacts/schemas/catalog/v1/catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,16 +73,16 @@
 @dataclass
 class CatalogResults(dbtClassMixin):
     nodes: Dict[str, CatalogTable]
     sources: Dict[str, CatalogTable]
     errors: Optional[List[str]] = None
     _compile_results: Optional[Any] = None
 
-    def __post_serialize__(self, dct):
-        dct = super().__post_serialize__(dct)
+    def __post_serialize__(self, dct: Dict, context: Optional[Dict] = None):
+        dct = super().__post_serialize__(dct, context)
         if "_compile_results" in dct:
             del dct["_compile_results"]
         return dct
 
 
 @dataclass
 @schema_version("catalog", 1)
```

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/schemas/freshness/v3/freshness.py` & `dbt_core-1.8.0rc2/dbt/artifacts/schemas/freshness/v3/freshness.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/schemas/manifest/v12/manifest.py` & `dbt_core-1.8.0rc2/dbt/artifacts/schemas/manifest/v12/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,7 @@
     def upgrade_schema_version(cls, data):
         """This overrides the "upgrade_schema_version" call in VersionedSchema (via
         ArtifactMixin) to modify the dictionary passed in from earlier versions of the manifest."""
         manifest_schema_version = get_artifact_schema_version(data)
         if manifest_schema_version < cls.dbt_schema_version.version:
             data = upgrade_manifest_json(data, manifest_schema_version)
         return cls.from_dict(data)
-
-    def __post_serialize__(self, dct):
-        for unique_id, node in dct["nodes"].items():
-            if "config_call_dict" in node:
-                del node["config_call_dict"]
-            if "defer_relation" in node:
-                del node["defer_relation"]
-        return dct
```

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/schemas/results.py` & `dbt_core-1.8.0rc2/dbt/artifacts/schemas/results.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/schemas/run/v5/run.py` & `dbt_core-1.8.0rc2/dbt/artifacts/schemas/run/v5/run.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/schemas/upgrades/upgrade_manifest.py` & `dbt_core-1.8.0rc2/dbt/artifacts/schemas/upgrades/upgrade_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/artifacts/utils/validation.py` & `dbt_core-1.8.0rc2/dbt/artifacts/utils/validation.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/cli/exceptions.py` & `dbt_core-1.8.0rc2/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/cli/flags.py` & `dbt_core-1.8.0rc2/dbt/cli/flags.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/cli/main.py` & `dbt_core-1.8.0rc2/dbt/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/cli/option_types.py` & `dbt_core-1.8.0rc2/dbt/cli/option_types.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/cli/options.py` & `dbt_core-1.8.0rc2/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/cli/params.py` & `dbt_core-1.8.0rc2/dbt/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/cli/requires.py` & `dbt_core-1.8.0rc2/dbt/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/cli/resolvers.py` & `dbt_core-1.8.0rc2/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/cli/types.py` & `dbt_core-1.8.0rc2/dbt/cli/types.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/clients/git.py` & `dbt_core-1.8.0rc2/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/clients/jinja.py` & `dbt_core-1.8.0rc2/dbt/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/clients/jinja_static.py` & `dbt_core-1.8.0rc2/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/clients/registry.py` & `dbt_core-1.8.0rc2/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/clients/yaml_helper.py` & `dbt_core-1.8.0rc2/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/compilation.py` & `dbt_core-1.8.0rc2/dbt/compilation.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/config/profile.py` & `dbt_core-1.8.0rc2/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/config/project.py` & `dbt_core-1.8.0rc2/dbt/config/project.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/config/renderer.py` & `dbt_core-1.8.0rc2/dbt/config/renderer.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/config/runtime.py` & `dbt_core-1.8.0rc2/dbt/config/runtime.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/config/selectors.py` & `dbt_core-1.8.0rc2/dbt/config/selectors.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/config/utils.py` & `dbt_core-1.8.0rc2/dbt/config/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/constants.py` & `dbt_core-1.8.0rc2/dbt/constants.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/context/base.py` & `dbt_core-1.8.0rc2/dbt/context/base.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/context/configured.py` & `dbt_core-1.8.0rc2/dbt/context/configured.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/context/context_config.py` & `dbt_core-1.8.0rc2/dbt/context/context_config.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/context/docs.py` & `dbt_core-1.8.0rc2/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/context/exceptions_jinja.py` & `dbt_core-1.8.0rc2/dbt/context/exceptions_jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/context/macro_resolver.py` & `dbt_core-1.8.0rc2/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/context/macros.py` & `dbt_core-1.8.0rc2/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/context/manifest.py` & `dbt_core-1.8.0rc2/dbt/context/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/context/providers.py` & `dbt_core-1.8.0rc2/dbt/context/providers.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/context/query_header.py` & `dbt_core-1.8.0rc2/dbt/context/query_header.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/context/secret.py` & `dbt_core-1.8.0rc2/dbt/context/secret.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/context/target.py` & `dbt_core-1.8.0rc2/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/files.py` & `dbt_core-1.8.0rc2/dbt/contracts/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,16 +135,16 @@
             sf = SchemaSourceFile.from_dict(dct)
         elif dct["parse_file_type"] == "fixture":
             sf = FixtureSourceFile.from_dict(dct)
         else:
             sf = SourceFile.from_dict(dct)
         return sf
 
-    def __post_serialize__(self, dct):
-        dct = super().__post_serialize__(dct)
+    def __post_serialize__(self, dct: Dict, context: Optional[Dict] = None):
+        dct = super().__post_serialize__(dct, context)
         # remove empty lists to save space
         dct_keys = list(dct.keys())
         for key in dct_keys:
             if isinstance(dct[key], list) and not dct[key]:
                 del dct[key]
         # remove contents. Schema files will still have 'dict_from_yaml'
         # from the contents
@@ -222,16 +222,16 @@
     def macro_patches(self):
         return self.mcp
 
     @property
     def source_patches(self):
         return self.sop
 
-    def __post_serialize__(self, dct):
-        dct = super().__post_serialize__(dct)
+    def __post_serialize__(self, dct: Dict, context: Optional[Dict] = None):
+        dct = super().__post_serialize__(dct, context)
         # Remove partial parsing specific data
         for key in ("pp_test_index", "pp_dict"):
             if key in dct:
                 del dct[key]
         return dct
 
     def append_patch(self, yaml_key, unique_id):
```

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/graph/manifest.py` & `dbt_core-1.8.0rc2/dbt/contracts/graph/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import enum
 from collections import defaultdict
 from dataclasses import dataclass, field, replace
 from itertools import chain
-from mashumaro.mixins.msgpack import DataClassMessagePackMixin
 from multiprocessing.synchronize import Lock
 from typing import (
     DefaultDict,
     Dict,
     List,
     Optional,
     Union,
@@ -799,15 +798,15 @@
 
 
 NodeClassT = TypeVar("NodeClassT", bound="BaseNode")
 ResourceClassT = TypeVar("ResourceClassT", bound="BaseResource")
 
 
 @dataclass
-class Manifest(MacroMethods, DataClassMessagePackMixin, dbtClassMixin):
+class Manifest(MacroMethods, dbtClassMixin):
     """The manifest for the full graph, after parsing and during compilation."""
 
     # These attributes are both positional and by keyword. If an attribute
     # is added it must all be added in the __reduce_ex__ method in the
     # args tuple in the right position.
     nodes: MutableMapping[str, ManifestNode] = field(default_factory=dict)
     sources: MutableMapping[str, SourceDefinition] = field(default_factory=dict)
@@ -866,15 +865,15 @@
         metadata={"serialize": lambda x: None, "deserialize": lambda x: None},
     )
     _macros_by_package: Optional[Dict[str, Dict[str, Macro]]] = field(
         default=None,
         metadata={"serialize": lambda x: None, "deserialize": lambda x: None},
     )
 
-    def __pre_serialize__(self):
+    def __pre_serialize__(self, context: Optional[Dict] = None):
         # serialization won't work with anything except an empty source_patches because
         # tuple keys are not supported, so ensure it's empty
         self.source_patches = {}
         return self
 
     @classmethod
     def __post_deserialize__(cls, obj):
```

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/graph/metrics.py` & `dbt_core-1.8.0rc2/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/graph/model_config.py` & `dbt_core-1.8.0rc2/dbt/contracts/graph/model_config.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/graph/node_args.py` & `dbt_core-1.8.0rc2/dbt/contracts/graph/node_args.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/graph/nodes.py` & `dbt_core-1.8.0rc2/dbt/contracts/graph/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,16 +258,16 @@
         else:
             full_path = os.path.join(project_root, compiled_path)
         write_file(full_path, compiled_code)
 
     def _serialize(self):
         return self.to_dict()
 
-    def __post_serialize__(self, dct):
-        dct = super().__post_serialize__(dct)
+    def __post_serialize__(self, dct: Dict, context: Optional[Dict] = None):
+        dct = super().__post_serialize__(dct, context)
         if "_event_status" in dct:
             del dct["_event_status"]
         return dct
 
     @classmethod
     def _deserialize(cls, dct: Dict[str, int]):
         # The serialized ParsedNodes do not differ from each other
```

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/graph/semantic_manifest.py` & `dbt_core-1.8.0rc2/dbt/contracts/graph/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/graph/unparsed.py` & `dbt_core-1.8.0rc2/dbt/contracts/graph/unparsed.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,16 +272,16 @@
     loaded_at_field_present: Optional[bool] = None
     identifier: Optional[str] = None
     quoting: Quoting = field(default_factory=Quoting)
     freshness: Optional[FreshnessThreshold] = field(default_factory=FreshnessThreshold)
     external: Optional[ExternalTable] = None
     tags: List[str] = field(default_factory=list)
 
-    def __post_serialize__(self, dct):
-        dct = super().__post_serialize__(dct)
+    def __post_serialize__(self, dct: Dict, context: Optional[Dict] = None):
+        dct = super().__post_serialize__(dct, context)
         if "freshness" not in dct and self.freshness is None:
             dct["freshness"] = None
         return dct
 
 
 @dataclass
 class UnparsedSourceDefinition(dbtClassMixin):
@@ -310,16 +310,16 @@
                 if table.get("loaded_at_field", None) == "":
                     raise ValidationError("loaded_at_field cannot be an empty string.")
 
     @property
     def yaml_key(self) -> "str":
         return "sources"
 
-    def __post_serialize__(self, dct):
-        dct = super().__post_serialize__(dct)
+    def __post_serialize__(self, dct: Dict, context: Optional[Dict] = None):
+        dct = super().__post_serialize__(dct, context)
         if "freshness" not in dct and self.freshness is None:
             dct["freshness"] = None
         return dct
 
 
 @dataclass
 class SourceTablePatch(dbtClassMixin):
```

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/project.py` & `dbt_core-1.8.0rc2/dbt/contracts/project.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/results.py` & `dbt_core-1.8.0rc2/dbt/contracts/results.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/selection.py` & `dbt_core-1.8.0rc2/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/sql.py` & `dbt_core-1.8.0rc2/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/state.py` & `dbt_core-1.8.0rc2/dbt/contracts/state.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/contracts/util.py` & `dbt_core-1.8.0rc2/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/deprecations.py` & `dbt_core-1.8.0rc2/dbt/deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/deps/base.py` & `dbt_core-1.8.0rc2/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/deps/git.py` & `dbt_core-1.8.0rc2/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/deps/local.py` & `dbt_core-1.8.0rc2/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/deps/registry.py` & `dbt_core-1.8.0rc2/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/deps/resolver.py` & `dbt_core-1.8.0rc2/dbt/deps/resolver.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/deps/tarball.py` & `dbt_core-1.8.0rc2/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/docs/source/_ext/dbt_click.py` & `dbt_core-1.8.0rc2/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/docs/source/conf.py` & `dbt_core-1.8.0rc2/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/events/base_types.py` & `dbt_core-1.8.0rc2/dbt/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/events/core_types_pb2.py` & `dbt_core-1.8.0rc2/dbt/events/core_types_pb2.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/events/logging.py` & `dbt_core-1.8.0rc2/dbt/events/logging.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/events/types.py` & `dbt_core-1.8.0rc2/dbt/events/types.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/exceptions.py` & `dbt_core-1.8.0rc2/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/flags.py` & `dbt_core-1.8.0rc2/dbt/flags.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/graph/cli.py` & `dbt_core-1.8.0rc2/dbt/graph/cli.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/graph/graph.py` & `dbt_core-1.8.0rc2/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/graph/queue.py` & `dbt_core-1.8.0rc2/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/graph/selector.py` & `dbt_core-1.8.0rc2/dbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/graph/selector_methods.py` & `dbt_core-1.8.0rc2/dbt/graph/selector_methods.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/graph/selector_spec.py` & `dbt_core-1.8.0rc2/dbt/graph/selector_spec.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/include/README.md` & `dbt_core-1.8.0rc2/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/include/starter_project/README.md` & `dbt_core-1.8.0rc2/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/include/starter_project/dbt_project.yml` & `dbt_core-1.8.0rc2/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/internal_deprecations.py` & `dbt_core-1.8.0rc2/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/logger.py` & `dbt_core-1.8.0rc2/dbt/logger.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/node_types.py` & `dbt_core-1.8.0rc2/dbt/node_types.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/__init__.py` & `dbt_core-1.8.0rc2/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/analysis.py` & `dbt_core-1.8.0rc2/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/base.py` & `dbt_core-1.8.0rc2/dbt/parser/base.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/common.py` & `dbt_core-1.8.0rc2/dbt/parser/common.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/docs.py` & `dbt_core-1.8.0rc2/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/fixtures.py` & `dbt_core-1.8.0rc2/dbt/parser/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/generic_test.py` & `dbt_core-1.8.0rc2/dbt/parser/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/generic_test_builders.py` & `dbt_core-1.8.0rc2/dbt/parser/generic_test_builders.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/hooks.py` & `dbt_core-1.8.0rc2/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/macros.py` & `dbt_core-1.8.0rc2/dbt/parser/macros.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/manifest.py` & `dbt_core-1.8.0rc2/dbt/parser/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     parse_project_elapsed: Optional[float] = None
     patch_sources_elapsed: Optional[float] = None
     process_manifest_elapsed: Optional[float] = None
     load_all_elapsed: Optional[float] = None
     projects: List[ProjectLoaderInfo] = field(default_factory=list)
     _project_index: Dict[str, ProjectLoaderInfo] = field(default_factory=dict)
 
-    def __post_serialize__(self, dct):
+    def __post_serialize__(self, dct: Dict, context: Optional[Dict] = None):
         del dct["_project_index"]
         return dct
 
 
 # The ManifestLoader loads the manifest. The standard way to use the
 # ManifestLoader is using the 'get_full_manifest' class method, but
 # many tests use abbreviated processes.
```

### Comparing `dbt_core-1.8.0rc1/dbt/parser/models.py` & `dbt_core-1.8.0rc2/dbt/parser/models.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/partial.py` & `dbt_core-1.8.0rc2/dbt/parser/partial.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/read_files.py` & `dbt_core-1.8.0rc2/dbt/parser/read_files.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/schema_generic_tests.py` & `dbt_core-1.8.0rc2/dbt/parser/schema_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/schema_renderer.py` & `dbt_core-1.8.0rc2/dbt/parser/schema_renderer.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/schema_yaml_readers.py` & `dbt_core-1.8.0rc2/dbt/parser/schema_yaml_readers.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/schemas.py` & `dbt_core-1.8.0rc2/dbt/parser/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/search.py` & `dbt_core-1.8.0rc2/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/seeds.py` & `dbt_core-1.8.0rc2/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/singular_test.py` & `dbt_core-1.8.0rc2/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/snapshots.py` & `dbt_core-1.8.0rc2/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/sources.py` & `dbt_core-1.8.0rc2/dbt/parser/sources.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/sql.py` & `dbt_core-1.8.0rc2/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/parser/unit_tests.py` & `dbt_core-1.8.0rc2/dbt/parser/unit_tests.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/plugins/__init__.py` & `dbt_core-1.8.0rc2/dbt/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/plugins/manager.py` & `dbt_core-1.8.0rc2/dbt/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/plugins/manifest.py` & `dbt_core-1.8.0rc2/dbt/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/base.py` & `dbt_core-1.8.0rc2/dbt/task/base.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/build.py` & `dbt_core-1.8.0rc2/dbt/task/build.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/clean.py` & `dbt_core-1.8.0rc2/dbt/task/clean.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/clone.py` & `dbt_core-1.8.0rc2/dbt/task/clone.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/compile.py` & `dbt_core-1.8.0rc2/dbt/task/compile.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/debug.py` & `dbt_core-1.8.0rc2/dbt/task/debug.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/deps.py` & `dbt_core-1.8.0rc2/dbt/task/deps.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/docs/generate.py` & `dbt_core-1.8.0rc2/dbt/task/docs/generate.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/docs/index.html` & `dbt_core-1.8.0rc2/dbt/task/docs/index.html`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/docs/serve.py` & `dbt_core-1.8.0rc2/dbt/task/docs/serve.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/freshness.py` & `dbt_core-1.8.0rc2/dbt/task/freshness.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/init.py` & `dbt_core-1.8.0rc2/dbt/task/init.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/list.py` & `dbt_core-1.8.0rc2/dbt/task/list.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/printer.py` & `dbt_core-1.8.0rc2/dbt/task/printer.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/retry.py` & `dbt_core-1.8.0rc2/dbt/task/retry.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/run.py` & `dbt_core-1.8.0rc2/dbt/task/run.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/run_operation.py` & `dbt_core-1.8.0rc2/dbt/task/run_operation.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/runnable.py` & `dbt_core-1.8.0rc2/dbt/task/runnable.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/seed.py` & `dbt_core-1.8.0rc2/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/show.py` & `dbt_core-1.8.0rc2/dbt/task/show.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/snapshot.py` & `dbt_core-1.8.0rc2/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/sql.py` & `dbt_core-1.8.0rc2/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/task/test.py` & `dbt_core-1.8.0rc2/dbt/task/test.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/tests/fixtures/project.py` & `dbt_core-1.8.0rc2/dbt/tests/fixtures/project.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/tests/util.py` & `dbt_core-1.8.0rc2/dbt/tests/util.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/tracking.py` & `dbt_core-1.8.0rc2/dbt/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/utils.py` & `dbt_core-1.8.0rc2/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/dbt/version.py` & `dbt_core-1.8.0rc2/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,9 +225,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.8.0rc1"
+__version__ = "1.8.0rc2"
 installed = get_installed_version()
```

### Comparing `dbt_core-1.8.0rc1/dbt_core.egg-info/PKG-INFO` & `dbt_core-1.8.0rc2/dbt_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.8.0rc1
+Version: 1.8.0rc2
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0rc1 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0rc2 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `dbt_core-1.8.0rc1/dbt_core.egg-info/SOURCES.txt` & `dbt_core-1.8.0rc2/dbt_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0rc1/setup.py` & `dbt_core-1.8.0rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "dbt-core"
-package_version = "1.8.0rc1"
+package_version = "1.8.0rc2"
 description = """With dbt, data analysts and engineers can build analytics \
 the way engineers build applications."""
 
 
 setup(
     name=package_name,
     version=package_version,
```

