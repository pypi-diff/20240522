# Comparing `tmp/conviso-flowcli-2.0.0rc8.tar.gz` & `tmp/conviso-flowcli-2.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conviso-flowcli-2.0.0rc8.tar", last modified: Wed Jan 17 20:54:59 2024, max compression
+gzip compressed data, was "conviso-flowcli-2.0.0rc9.tar", last modified: Wed Jan 17 21:40:26 2024, max compression
```

## Comparing `conviso-flowcli-2.0.0rc8.tar` & `conviso-flowcli-2.0.0rc9.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.370624 conviso-flowcli-2.0.0rc8/
--rw-r--r--   0 root         (0) root         (0)      497 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      234 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.358624 conviso-flowcli-2.0.0rc8/conviso_flowcli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      497 2024-01-17 20:54:59.000000 conviso-flowcli-2.0.0rc8/conviso_flowcli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5567 2024-01-17 20:54:59.000000 conviso-flowcli-2.0.0rc8/conviso_flowcli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-17 20:54:59.000000 conviso-flowcli-2.0.0rc8/conviso_flowcli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-01-17 20:54:59.000000 conviso-flowcli-2.0.0rc8/conviso_flowcli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      232 2024-01-17 20:54:59.000000 conviso-flowcli-2.0.0rc8/conviso_flowcli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-01-17 20:54:59.000000 conviso-flowcli-2.0.0rc8/conviso_flowcli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.358624 conviso-flowcli-2.0.0rc8/convisoappsec/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.358624 conviso-flowcli-2.0.0rc8/convisoappsec/common/
--rw-r--r--   0 root         (0) root         (0)      105 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7970 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/common/box.py
--rw-r--r--   0 root         (0) root         (0)    12525 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/common/docker.py
--rw-r--r--   0 root         (0) root         (0)      230 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/common/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2067 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/common/git_data_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.358624 conviso-flowcli-2.0.0rc8/convisoappsec/common/graphql/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/common/graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2055 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/common/graphql/error_handlers.py
--rw-r--r--   0 root         (0) root         (0)      247 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/common/graphql/errors.py
--rw-r--r--   0 root         (0) root         (0)     1294 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/common/graphql/low_client.py
--rw-r--r--   0 root         (0) root         (0)      185 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/common/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.358624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/
--rw-r--r--   0 root         (0) root         (0)       81 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11584 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.358624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/__init__.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/models/issues/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/models/issues/__init__.py
--rw-r--r--   0 root         (0) root         (0)      311 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/models/issues/iac.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/models/issues/normalize.py
--rw-r--r--   0 root         (0) root         (0)     1488 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/models/issues/sast.py
--rw-r--r--   0 root         (0) root         (0)     1349 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/models/issues/sca.py
--rw-r--r--   0 root         (0) root         (0)     2113 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/resources_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/schemas/mutations/
--rw-r--r--   0 root         (0) root         (0)      327 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/schemas/resolvers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/schemas/resolvers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      790 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      345 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/models/asset.py
--rw-r--r--   0 root         (0) root         (0)      863 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/models/project.py
--rw-r--r--   0 root         (0) root         (0)     5835 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/resources_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/schemas/mutations/
--rw-r--r--   0 root         (0) root         (0)      970 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/schemas/resolvers/
--rw-r--r--   0 root         (0) root         (0)     1522 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/source_code_scanner/
--rw-r--r--   0 root         (0) root         (0)      227 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/source_code_scanner/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/source_code_scanner/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1655 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/source_code_scanner/scc.py
--rw-r--r--   0 root         (0) root         (0)     4726 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/source_code_scanner/source_code_scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/util/
--rw-r--r--   0 root         (0) root         (0)      160 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2093 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/util/ci_provider.py
--rw-r--r--   0 root         (0) root         (0)      480 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/util/metrics.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/util/source_code_compressor.py
--rw-r--r--   0 root         (0) root         (0)    12087 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/version_control_system_adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/version_searchers/
--rw-r--r--   0 root         (0) root         (0)      294 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/version_searchers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py
--rw-r--r--   0 root         (0) root         (0)     1266 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/version_searchers/timebased_version_seacher.py
--rw-r--r--   0 root         (0) root         (0)      943 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/version_searchers/version_searcher_result.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flow/versioning_style/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/versioning_style/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1041 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flow/versioning_style/semantic_versioning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/
--rw-r--r--   0 root         (0) root         (0)       64 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/__init__.py
--rw-r--r--   0 root         (0) root         (0)       99 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/assets/
--rw-r--r--   0 root         (0) root         (0)       54 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2278 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/assets/create.py
--rw-r--r--   0 root         (0) root         (0)      310 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/assets/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     1484 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/assets/ls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/ast/
--rw-r--r--   0 root         (0) root         (0)       47 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/ast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6207 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/ast/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     5350 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.362624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/companies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/companies/__init__.py
--rw-r--r--   0 root         (0) root         (0)      892 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/companies/ls.py
--rw-r--r--   0 root         (0) root         (0)     1309 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/
--rw-r--r--   0 root         (0) root         (0)       54 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/
--rw-r--r--   0 root         (0) root         (0)       54 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      190 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/context.py
--rw-r--r--   0 root         (0) root         (0)      677 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/
--rw-r--r--   0 root         (0) root         (0)       51 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/__init__.py
--rw-r--r--   0 root         (0) root         (0)      346 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/
--rw-r--r--   0 root         (0) root         (0)       64 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      194 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/context.py
--rw-r--r--   0 root         (0) root         (0)      675 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/
--rw-r--r--   0 root         (0) root         (0)       56 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/__init__.py
--rw-r--r--   0 root         (0) root         (0)      382 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2815 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py
--rw-r--r--   0 root         (0) root         (0)     3500 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py
--rw-r--r--   0 root         (0) root         (0)     4580 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/values.py
--rw-r--r--   0 root         (0) root         (0)      353 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      763 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/ls.py
--rw-r--r--   0 root         (0) root         (0)      970 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/show.py
--rw-r--r--   0 root         (0) root         (0)     2878 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/
--rw-r--r--   0 root         (0) root         (0)       58 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/create/
--rw-r--r--   0 root         (0) root         (0)       54 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      269 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/create/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/create/with_/
--rw-r--r--   0 root         (0) root         (0)       51 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/create/with_/__init__.py
--rw-r--r--   0 root         (0) root         (0)      309 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/create/with_/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/create/with_/version_tracker.py
--rw-r--r--   0 root         (0) root         (0)      344 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/import_sarif/
--rw-r--r--   0 root         (0) root         (0)       66 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/import_sarif/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7209 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/import_sarif/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      331 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/help_option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/iac/
--rw-r--r--   0 root         (0) root         (0)       47 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/iac/__init__.py
--rw-r--r--   0 root         (0) root         (0)      241 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/iac/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    11081 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/iac/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/projects/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/projects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/projects/ls.py
--rw-r--r--   0 root         (0) root         (0)     8055 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/requirements_verifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/sast/
--rw-r--r--   0 root         (0) root         (0)       49 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/sast/__init__.py
--rw-r--r--   0 root         (0) root         (0)      245 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/sast/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    15835 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/sast/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/sca/
--rw-r--r--   0 root         (0) root         (0)       47 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/sca/__init__.py
--rw-r--r--   0 root         (0) root         (0)      241 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/sca/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    10508 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/sca/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/vulnerability/
--rw-r--r--   0 root         (0) root         (0)       67 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/vulnerability/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4298 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/vulnerability/assert_security_rules.py
--rw-r--r--   0 root         (0) root         (0)      335 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/vulnerability/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      231 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/convisoappsec/sast/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/sast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/sast/decision.py
--rw-r--r--   0 root         (0) root         (0)     6217 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/sast/sastbox.py
--rw-r--r--   0 root         (0) root         (0)       27 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/convisoappsec/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.358624 conviso-flowcli-2.0.0rc8/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 20:54:59.366624 conviso-flowcli-2.0.0rc8/scripts/shell_completer/
--rw-r--r--   0 root         (0) root         (0)      624 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/scripts/shell_completer/flow_bash_completer.sh
--rw-r--r--   0 root         (0) root         (0)      147 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/scripts/shell_completer/flow_fish_completer.fish
--rw-r--r--   0 root         (0) root         (0)      844 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/scripts/shell_completer/flow_zsh_completer.sh
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-17 20:54:59.370624 conviso-flowcli-2.0.0rc8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1744 2024-01-17 20:54:56.000000 conviso-flowcli-2.0.0rc8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/
+-rw-r--r--   0 root         (0) root         (0)      497 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      234 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.153240 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      497 2024-01-17 21:40:26.000000 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5567 2024-01-17 21:40:26.000000 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-17 21:40:26.000000 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-01-17 21:40:26.000000 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      232 2024-01-17 21:40:26.000000 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-01-17 21:40:26.000000 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.153240 conviso-flowcli-2.0.0rc9/convisoappsec/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.153240 conviso-flowcli-2.0.0rc9/convisoappsec/common/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7970 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/box.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/docker.py
+-rw-r--r--   0 root         (0) root         (0)      230 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/git_data_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.153240 conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/error_handlers.py
+-rw-r--r--   0 root         (0) root         (0)      247 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/low_client.py
+-rw-r--r--   0 root         (0) root         (0)      185 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/
+-rw-r--r--   0 root         (0) root         (0)       81 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11584 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      311 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/iac.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/normalize.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/sast.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/sca.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/resources_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/schemas/mutations/
+-rw-r--r--   0 root         (0) root         (0)      327 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/schemas/resolvers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/schemas/resolvers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      345 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/models/asset.py
+-rw-r--r--   0 root         (0) root         (0)      863 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/models/project.py
+-rw-r--r--   0 root         (0) root         (0)     5835 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/resources_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/mutations/
+-rw-r--r--   0 root         (0) root         (0)      970 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/resolvers/
+-rw-r--r--   0 root         (0) root         (0)     1522 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/
+-rw-r--r--   0 root         (0) root         (0)      227 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/scc.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/source_code_scanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/util/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/util/ci_provider.py
+-rw-r--r--   0 root         (0) root         (0)      480 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/util/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      508 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/util/source_code_compressor.py
+-rw-r--r--   0 root         (0) root         (0)    12087 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_control_system_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/
+-rw-r--r--   0 root         (0) root         (0)      294 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/timebased_version_seacher.py
+-rw-r--r--   0 root         (0) root         (0)      943 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/version_searcher_result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/versioning_style/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/versioning_style/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/versioning_style/semantic_versioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       99 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/create.py
+-rw-r--r--   0 root         (0) root         (0)      310 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/ls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/ast/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/ast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6207 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/ast/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     5350 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/companies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/companies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      892 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/companies/ls.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      190 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/context.py
+-rw-r--r--   0 root         (0) root         (0)      677 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      346 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      194 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/context.py
+-rw-r--r--   0 root         (0) root         (0)      675 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/
+-rw-r--r--   0 root         (0) root         (0)       56 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      382 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py
+-rw-r--r--   0 root         (0) root         (0)     4580 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/values.py
+-rw-r--r--   0 root         (0) root         (0)      353 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      763 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/ls.py
+-rw-r--r--   0 root         (0) root         (0)      970 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/show.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      269 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/with_/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/with_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      309 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/with_/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/with_/version_tracker.py
+-rw-r--r--   0 root         (0) root         (0)      344 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/import_sarif/
+-rw-r--r--   0 root         (0) root         (0)       66 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/import_sarif/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/import_sarif/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      331 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/help_option.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/iac/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/iac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      241 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/iac/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    11081 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/iac/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/projects/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/projects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/projects/ls.py
+-rw-r--r--   0 root         (0) root         (0)     8055 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/requirements_verifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sast/
+-rw-r--r--   0 root         (0) root         (0)       49 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      245 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sast/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    15835 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sast/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sca/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sca/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      241 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sca/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    10508 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sca/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/vulnerability/
+-rw-r--r--   0 root         (0) root         (0)       67 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/vulnerability/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4298 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/vulnerability/assert_security_rules.py
+-rw-r--r--   0 root         (0) root         (0)      335 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/vulnerability/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      231 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/convisoappsec/sast/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/sast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/sast/decision.py
+-rw-r--r--   0 root         (0) root         (0)     6218 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/sast/sastbox.py
+-rw-r--r--   0 root         (0) root         (0)       27 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.153240 conviso-flowcli-2.0.0rc9/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/scripts/shell_completer/
+-rw-r--r--   0 root         (0) root         (0)      624 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/scripts/shell_completer/flow_bash_completer.sh
+-rw-r--r--   0 root         (0) root         (0)      147 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/scripts/shell_completer/flow_fish_completer.fish
+-rw-r--r--   0 root         (0) root         (0)      844 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/scripts/shell_completer/flow_zsh_completer.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/setup.py
```

### Comparing `conviso-flowcli-2.0.0rc8/conviso_flowcli.egg-info/SOURCES.txt` & `conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/common/box.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/common/box.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/common/docker.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/common/docker.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/common/git_data_parser.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/common/git_data_parser.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/common/graphql/error_handlers.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/error_handlers.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/common/graphql/low_client.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/low_client.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/api.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/api.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/models/issues/sast.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/sast.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/models/issues/sca.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/sca.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/beta/resources_api.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/resources_api.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/client.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/client.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/models/project.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/models/project.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/resources_api.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/resources_api.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/source_code_scanner/scc.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/scc.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/source_code_scanner/source_code_scanner.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/source_code_scanner.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/util/ci_provider.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/util/ci_provider.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/version_control_system_adapter.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_control_system_adapter.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/version_searchers/timebased_version_seacher.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/timebased_version_seacher.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/version_searchers/version_searcher_result.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/version_searcher_result.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flow/versioning_style/semantic_versioning.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flow/versioning_style/semantic_versioning.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/assets/create.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/create.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/assets/ls.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/ast/entrypoint.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/ast/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/common.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/common.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/companies/ls.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/companies/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/context.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/context.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/entrypoint.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/create/with_/values.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/values.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/ls.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/deploy/show.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/show.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/entrypoint.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/create/with_/version_tracker.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/with_/version_tracker.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/findings/import_sarif/entrypoint.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/import_sarif/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/iac/run.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/iac/run.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/projects/ls.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/projects/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/requirements_verifier.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/requirements_verifier.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/sast/run.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sast/run.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/sca/run.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sca/run.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/flowcli/vulnerability/assert_security_rules.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/vulnerability/assert_security_rules.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/sast/decision.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/sast/decision.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/convisoappsec/sast/sastbox.py` & `conviso-flowcli-2.0.0rc9/convisoappsec/sast/sastbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class SASTBox(object):
     REGISTRY = 'docker.convisoappsec.com'
     REPOSITORY_NAME = 'sastbox_v2'
     DEFAULT_TAG = 'unstable'
     CONTAINER_REPORTS_DIR = '/tmp'
-    CONTAINER_CODE_DIR = bitbucket or '/tmp'
+    CONTAINER_CODE_DIR = bitbucket or '/code'
     WORKSPACE_REPORT_PATH = ["tmp"]
     JSON_REPORT_PATTERN = 'output.sarif'
     SUCCESS_EXIT_CODE = 1
     USER_ENV_VAR = "USER"
 
     def __init__(self, registry=None, repository_name=None, tag=None):
         self.docker = docker.from_env(
```

### Comparing `conviso-flowcli-2.0.0rc8/scripts/shell_completer/flow_bash_completer.sh` & `conviso-flowcli-2.0.0rc9/scripts/shell_completer/flow_bash_completer.sh`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/scripts/shell_completer/flow_zsh_completer.sh` & `conviso-flowcli-2.0.0rc9/scripts/shell_completer/flow_zsh_completer.sh`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc8/setup.py` & `conviso-flowcli-2.0.0rc9/setup.py`

 * *Files identical despite different names*

