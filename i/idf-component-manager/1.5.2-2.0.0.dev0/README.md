# Comparing `tmp/idf_component_manager-1.5.2.tar.gz` & `tmp/idf_component_manager-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf_component_manager-1.5.2.tar", last modified: Fri Feb 23 14:11:44 2024, max compression
+gzip compressed data, was "idf_component_manager-2.0.0.dev0.tar", max compression
```

## Comparing `idf_component_manager-1.5.2.tar` & `idf_component_manager-2.0.0.dev0.tar`

### file list

```diff
@@ -1,126 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.084652 idf_component_manager-1.5.2/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11078 2024-02-23 14:11:44.084652 idf_component_manager-1.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9802 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.076652 idf_component_manager-1.5.2/idf_component_manager/
--rw-rw-rw-   0 root         (0) root         (0)      285 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4843 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.076652 idf_component_manager-1.5.2/idf_component_manager/cli/
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6432 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/cli/autocompletion.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/cli/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5998 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/cli/component.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/cli/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2024-02-22 15:09:26.000000 idf_component_manager-1.5.2/idf_component_manager/cli/core.py
--rw-rw-rw-   0 root         (0) root         (0)     2873 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/cli/manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     1546 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/cli/project.py
--rw-rw-rw-   0 root         (0) root         (0)     6157 2024-02-22 15:09:26.000000 idf_component_manager-1.5.2/idf_component_manager/cli/registry.py
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/cli/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6744 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/cmake_component_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)    39267 2024-02-22 15:09:26.000000 idf_component_manager-1.5.2/idf_component_manager/core.py
--rw-rw-rw-   0 root         (0) root         (0)     7499 2024-02-22 15:09:26.000000 idf_component_manager-1.5.2/idf_component_manager/core_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14329 2024-02-23 08:28:00.000000 idf_component_manager-1.5.2/idf_component_manager/dependencies.py
--rwxrwxrwx   0 root         (0) root         (0)     9113 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/idf_extensions.py
--rw-rw-rw-   0 root         (0) root         (0)      902 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/local_component_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.076652 idf_component_manager-1.5.2/idf_component_manager/prepare_components/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 14:11:27.000000 idf_component_manager-1.5.2/idf_component_manager/prepare_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/prepare_components/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4108 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/prepare_components/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     6564 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/service_details.py
--rw-rw-rw-   0 root         (0) root         (0)    12113 2024-02-22 15:09:26.000000 idf_component_manager-1.5.2/idf_component_manager/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.076652 idf_component_manager-1.5.2/idf_component_manager/templates/
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/templates/idf_component_template.yml
--rw-rw-rw-   0 root         (0) root         (0)     3752 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.076652 idf_component_manager-1.5.2/idf_component_manager/version_solver/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 14:11:27.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6487 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.080652 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 14:11:27.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1789 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/assignment.py
--rw-rw-rw-   0 root         (0) root         (0)     3910 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     9705 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/failure.py
--rw-rw-rw-   0 root         (0) root         (0)    15132 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/incompatibility.py
--rw-rw-rw-   0 root         (0) root         (0)     1602 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/incompatibility_cause.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/package.py
--rw-rw-rw-   0 root         (0) root         (0)     4236 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/package_source.py
--rw-rw-rw-   0 root         (0) root         (0)     7528 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/partial_solution.py
--rw-rw-rw-   0 root         (0) root         (0)    12835 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/range.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/result.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/set_relation.py
--rw-rw-rw-   0 root         (0) root         (0)     6580 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/term.py
--rw-rw-rw-   0 root         (0) root         (0)     7032 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/union.py
--rw-rw-rw-   0 root         (0) root         (0)    15723 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/version_solver.py
--rw-rw-rw-   0 root         (0) root         (0)    10044 2024-02-23 09:55:45.000000 idf_component_manager-1.5.2/idf_component_manager/version_solver/version_solver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.076652 idf_component_manager-1.5.2/idf_component_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11078 2024-02-23 14:11:44.000000 idf_component_manager-1.5.2/idf_component_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4609 2024-02-23 14:11:44.000000 idf_component_manager-1.5.2/idf_component_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-23 14:11:44.000000 idf_component_manager-1.5.2/idf_component_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-02-23 14:11:44.000000 idf_component_manager-1.5.2/idf_component_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      658 2024-02-23 14:11:44.000000 idf_component_manager-1.5.2/idf_component_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-02-23 14:11:44.000000 idf_component_manager-1.5.2/idf_component_manager.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.080652 idf_component_manager-1.5.2/idf_component_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 14:11:27.000000 idf_component_manager-1.5.2/idf_component_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-02-23 13:39:41.000000 idf_component_manager-1.5.2/idf_component_tools/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     3012 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/archive_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     3160 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/build_system_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     7373 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1481 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/environment.py
--rw-rw-rw-   0 root         (0) root         (0)     2442 2024-02-22 15:09:26.000000 idf_component_manager-1.5.2/idf_component_tools/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     6241 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/file_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5348 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/file_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    10393 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/git_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.080652 idf_component_manager-1.5.2/idf_component_tools/hash_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 14:11:27.000000 idf_component_manager-1.5.2/idf_component_tools/hash_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1826 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/hash_tools/calculate.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/hash_tools/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/hash_tools/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     1876 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/hash_tools/validate_managed_component.py
--rw-rw-rw-   0 root         (0) root         (0)      714 2024-02-22 15:09:26.000000 idf_component_manager-1.5.2/idf_component_tools/hash_tools/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.080652 idf_component_manager-1.5.2/idf_component_tools/lock/
--rw-rw-rw-   0 root         (0) root         (0)      208 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/lock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4310 2024-02-23 08:28:00.000000 idf_component_manager-1.5.2/idf_component_tools/lock/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.080652 idf_component_manager-1.5.2/idf_component_tools/manifest/
--rw-rw-rw-   0 root         (0) root         (0)     1199 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/manifest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1799 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/manifest/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2683 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/manifest/env_expander.py
--rw-rw-rw-   0 root         (0) root         (0)     8143 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/manifest/if_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     7148 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/manifest/manager.py
--rw-rw-rw-   0 root         (0) root         (0)    16807 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/manifest/manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     4495 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/manifest/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11881 2024-02-23 10:24:41.000000 idf_component_manager-1.5.2/idf_component_tools/manifest/schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     2917 2024-02-23 08:28:00.000000 idf_component_manager-1.5.2/idf_component_tools/manifest/solved_component.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-02-23 08:28:00.000000 idf_component_manager-1.5.2/idf_component_tools/manifest/solved_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     9389 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/manifest/validator.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/messages.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/network_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.080652 idf_component_manager-1.5.2/idf_component_tools/registry/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 14:11:27.000000 idf_component_manager-1.5.2/idf_component_tools/registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7066 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/registry/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/registry/api_client_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     2145 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/registry/api_schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     7308 2024-02-22 15:09:26.000000 idf_component_manager-1.5.2/idf_component_tools/registry/base_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1183 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/registry/component_details.py
--rw-rw-rw-   0 root         (0) root         (0)     2803 2024-02-22 15:09:26.000000 idf_component_manager-1.5.2/idf_component_tools/registry/multi_storage_client.py
--rw-rw-rw-   0 root         (0) root         (0)     5419 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/registry/request_processor.py
--rw-rw-rw-   0 root         (0) root         (0)     6151 2024-02-22 15:09:26.000000 idf_component_manager-1.5.2/idf_component_tools/registry/storage_client.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/registry/token_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.080652 idf_component_manager-1.5.2/idf_component_tools/semver/
--rw-rw-rw-   0 root         (0) root         (0)      452 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/semver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    33813 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/semver/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2941 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/serialization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 14:11:44.084652 idf_component_manager-1.5.2/idf_component_tools/sources/
--rw-rw-rw-   0 root         (0) root         (0)      589 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6837 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/sources/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2679 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/sources/fetcher.py
--rw-rw-rw-   0 root         (0) root         (0)     7989 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/sources/git.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/sources/idf.py
--rw-rw-rw-   0 root         (0) root         (0)     6014 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/sources/local.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/sources/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    12565 2024-02-22 15:09:26.000000 idf_component_manager-1.5.2/idf_component_tools/sources/web_service.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/sources/web_service_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/idf_component_tools/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4317 2024-02-23 13:39:41.000000 idf_component_manager-1.5.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-23 14:11:44.084652 idf_component_manager-1.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3399 2024-02-22 14:19:58.000000 idf_component_manager-1.5.2/setup.py
+-rw-r--r--   0        0        0    11358 2024-05-22 09:19:17.358948 idf_component_manager-2.0.0.dev0/LICENSE
+-rw-r--r--   0        0        0     9802 2024-05-22 09:19:17.358948 idf_component_manager-2.0.0.dev0/README.md
+-rw-r--r--   0        0        0      285 2024-05-22 09:19:17.362948 idf_component_manager-2.0.0.dev0/idf_component_manager/__init__.py
+-rw-r--r--   0        0        0     4839 2024-05-22 13:25:42.494657 idf_component_manager-2.0.0.dev0/idf_component_manager/__main__.py
+-rw-r--r--   0        0        0      161 2024-05-22 09:19:17.362948 idf_component_manager-2.0.0.dev0/idf_component_manager/cli/__init__.py
+-rw-r--r--   0        0        0     6300 2024-05-22 13:25:42.494657 idf_component_manager-2.0.0.dev0/idf_component_manager/cli/autocompletion.py
+-rw-r--r--   0        0        0     1191 2024-05-22 13:25:42.494657 idf_component_manager-2.0.0.dev0/idf_component_manager/cli/cache.py
+-rw-r--r--   0        0        0     5984 2024-05-22 13:25:42.494657 idf_component_manager-2.0.0.dev0/idf_component_manager/cli/component.py
+-rw-r--r--   0        0        0     1713 2024-05-22 09:19:17.362948 idf_component_manager-2.0.0.dev0/idf_component_manager/cli/constants.py
+-rw-r--r--   0        0        0     1910 2024-05-22 13:25:42.494657 idf_component_manager-2.0.0.dev0/idf_component_manager/cli/core.py
+-rw-r--r--   0        0        0     2883 2024-05-22 13:25:42.494657 idf_component_manager-2.0.0.dev0/idf_component_manager/cli/manifest.py
+-rw-r--r--   0        0        0     1546 2024-05-22 09:19:17.362948 idf_component_manager-2.0.0.dev0/idf_component_manager/cli/project.py
+-rw-r--r--   0        0        0     6444 2024-05-22 13:25:42.494657 idf_component_manager-2.0.0.dev0/idf_component_manager/cli/registry.py
+-rw-r--r--   0        0        0      573 2024-05-22 13:25:42.494657 idf_component_manager-2.0.0.dev0/idf_component_manager/cli/utils.py
+-rw-r--r--   0        0        0     6654 2024-05-22 13:25:42.494657 idf_component_manager-2.0.0.dev0/idf_component_manager/cmake_component_requirements.py
+-rw-r--r--   0        0        0    38819 2024-05-22 13:25:42.494657 idf_component_manager-2.0.0.dev0/idf_component_manager/core.py
+-rw-r--r--   0        0        0     7123 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/core_utils.py
+-rw-r--r--   0        0        0    14325 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/dependencies.py
+-rwxr-xr-x   0        0        0     9048 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/idf_extensions.py
+-rw-r--r--   0        0        0      832 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/local_component_list.py
+-rw-r--r--   0        0        0       85 2024-05-22 09:19:17.362948 idf_component_manager-2.0.0.dev0/idf_component_manager/prepare_components/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 14:04:24.673927 idf_component_manager-2.0.0.dev0/idf_component_manager/prepare_components/__init__.py
+-rw-r--r--   0        0        0      140 2024-05-22 09:19:17.362948 idf_component_manager-2.0.0.dev0/idf_component_manager/prepare_components/__main__.py
+-rwxr-xr-x   0        0        0     4110 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/prepare_components/prepare.py
+-rw-r--r--   0        0        0    11709 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/sync.py
+-rw-r--r--   0        0        0      559 2024-05-22 09:19:17.362948 idf_component_manager-2.0.0.dev0/idf_component_manager/templates/idf_component_template.yml
+-rw-r--r--   0        0        0     3616 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/utils.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:04:24.677927 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/__init__.py
+-rw-r--r--   0        0        0     6283 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/helper.py
+-rw-r--r--   0        0        0     1130 2024-05-22 09:19:17.362948 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-22 14:04:24.677927 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/__init__.py
+-rw-r--r--   0        0        0     1743 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/assignment.py
+-rw-r--r--   0        0        0     3669 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/constraint.py
+-rw-r--r--   0        0        0     9480 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/failure.py
+-rw-r--r--   0        0        0    14713 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/incompatibility.py
+-rw-r--r--   0        0        0     1578 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/incompatibility_cause.py
+-rw-r--r--   0        0        0     1294 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/package.py
+-rw-r--r--   0        0        0     4039 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/package_source.py
+-rw-r--r--   0        0        0     7263 2024-05-22 13:25:42.498657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/partial_solution.py
+-rw-r--r--   0        0        0    12420 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/range.py
+-rw-r--r--   0        0        0      765 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/result.py
+-rw-r--r--   0        0        0      328 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/set_relation.py
+-rw-r--r--   0        0        0     6340 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/term.py
+-rw-r--r--   0        0        0     6872 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/union.py
+-rw-r--r--   0        0        0    15396 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/version_solver.py
+-rw-r--r--   0        0        0     9321 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/version_solver.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:04:24.677927 idf_component_manager-2.0.0.dev0/idf_component_tools/__init__.py
+-rw-r--r--   0        0        0      172 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_tools/__version__.py
+-rw-r--r--   0        0        0     2945 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_tools/archive_tools.py
+-rw-r--r--   0        0        0     3219 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_tools/build_system_tools.py
+-rw-r--r--   0        0        0     3372 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_tools/config.py
+-rw-r--r--   0        0        0     1032 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_tools/constants.py
+-rw-r--r--   0        0        0     1948 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_tools/environment.py
+-rw-r--r--   0        0        0     2519 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_tools/errors.py
+-rw-r--r--   0        0        0     6179 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_tools/file_cache.py
+-rw-r--r--   0        0        0     5292 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_tools/file_tools.py
+-rw-r--r--   0        0        0    10137 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_tools/git_client.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:04:24.677927 idf_component_manager-2.0.0.dev0/idf_component_tools/hash_tools/__init__.py
+-rw-r--r--   0        0        0     2193 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_tools/hash_tools/calculate.py
+-rw-r--r--   0        0        0      191 2024-05-22 09:19:17.366948 idf_component_manager-2.0.0.dev0/idf_component_tools/hash_tools/constants.py
+-rw-r--r--   0        0        0      328 2024-05-22 09:19:17.366948 idf_component_manager-2.0.0.dev0/idf_component_tools/hash_tools/errors.py
+-rw-r--r--   0        0        0     1835 2024-05-22 13:25:42.502657 idf_component_manager-2.0.0.dev0/idf_component_tools/hash_tools/validate_managed_component.py
+-rw-r--r--   0        0        0      632 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/hash_tools/validator.py
+-rw-r--r--   0        0        0      234 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/lock/__init__.py
+-rw-r--r--   0        0        0     3486 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/lock/manager.py
+-rw-r--r--   0        0        0     4414 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/manager.py
+-rw-r--r--   0        0        0      903 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/manifest/__init__.py
+-rw-r--r--   0        0        0     1591 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/manifest/constants.py
+-rw-r--r--   0        0        0     2598 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/manifest/env_expander.py
+-rw-r--r--   0        0        0     8042 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/manifest/if_parser.py
+-rw-r--r--   0        0        0     2739 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/manifest/metadata.py
+-rw-r--r--   0        0        0    22100 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/manifest/models.py
+-rw-r--r--   0        0        0     5091 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/manifest/schemas.py
+-rw-r--r--   0        0        0      788 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/messages.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:04:24.677927 idf_component_manager-2.0.0.dev0/idf_component_tools/registry/__init__.py
+-rw-r--r--   0        0        0     6368 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/registry/api_client.py
+-rw-r--r--   0        0        0     1864 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/registry/api_models.py
+-rw-r--r--   0        0        0     7646 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/registry/base_client.py
+-rw-r--r--   0        0        0     1437 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/registry/client_errors.py
+-rw-r--r--   0        0        0     4401 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/registry/multi_storage_client.py
+-rw-r--r--   0        0        0     5391 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/registry/request_processor.py
+-rw-r--r--   0        0        0     5584 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/registry/service_details.py
+-rw-r--r--   0        0        0     4726 2024-05-22 13:25:42.506657 idf_component_manager-2.0.0.dev0/idf_component_tools/registry/storage_client.py
+-rw-r--r--   0        0        0     1382 2024-05-22 09:19:17.366948 idf_component_manager-2.0.0.dev0/idf_component_tools/semver/LICENSE
+-rw-r--r--   0        0        0      428 2024-05-22 13:25:42.510657 idf_component_manager-2.0.0.dev0/idf_component_tools/semver/__init__.py
+-rw-r--r--   0        0        0    33652 2024-05-22 13:25:42.510657 idf_component_manager-2.0.0.dev0/idf_component_tools/semver/base.py
+-rw-r--r--   0        0        0     2025 2024-05-22 13:25:42.510657 idf_component_manager-2.0.0.dev0/idf_component_tools/sources/__init__.py
+-rw-r--r--   0        0        0     4098 2024-05-22 13:25:42.514657 idf_component_manager-2.0.0.dev0/idf_component_tools/sources/base.py
+-rw-r--r--   0        0        0     2606 2024-05-22 13:25:42.514657 idf_component_manager-2.0.0.dev0/idf_component_tools/sources/fetcher.py
+-rw-r--r--   0        0        0     6561 2024-05-22 13:25:42.514657 idf_component_manager-2.0.0.dev0/idf_component_tools/sources/git.py
+-rw-r--r--   0        0        0      983 2024-05-22 13:25:42.514657 idf_component_manager-2.0.0.dev0/idf_component_tools/sources/idf.py
+-rw-r--r--   0        0        0     5554 2024-05-22 13:25:42.514657 idf_component_manager-2.0.0.dev0/idf_component_tools/sources/local.py
+-rw-r--r--   0        0        0     9176 2024-05-22 13:25:42.514657 idf_component_manager-2.0.0.dev0/idf_component_tools/sources/web_service.py
+-rw-r--r--   0        0        0    13275 2024-05-22 13:25:42.514657 idf_component_manager-2.0.0.dev0/idf_component_tools/utils.py
+-rw-r--r--   0        0        0     4404 2024-05-22 13:25:42.514657 idf_component_manager-2.0.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0    11352 1970-01-01 00:00:00.000000 idf_component_manager-2.0.0.dev0/PKG-INFO
```

### Comparing `idf_component_manager-1.5.2/LICENSE` & `idf_component_manager-2.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.5.2/PKG-INFO` & `idf_component_manager-2.0.0.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 Metadata-Version: 2.1
-Name: idf_component_manager
-Version: 1.5.2
-Summary: The component manager for ESP-IDF
-Home-page: https://github.com/espressif/idf-component-manager
+Name: idf-component-manager
+Version: 2.0.0.dev0
+Summary: Espressif IDF Component Manager
+Home-page: https://github.com/espressif/idf-component-manager.git
+License: Apache-2.0
 Author: Sergei Silnov
 Author-email: sergei.silnov@espressif.com
-Maintainer: Sergei Silnov
-License: Apache License 2.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
+Requires-Dist: cachecontrol[filecache]
+Requires-Dist: click
+Requires-Dist: colorama
+Requires-Dist: jsonref (>=1.1.0,<2.0.0)
+Requires-Dist: packaging
+Requires-Dist: pydantic (>=2.5,<3.0)
+Requires-Dist: pydantic-core (>=2.14,<3.0)
+Requires-Dist: pyparsing
+Requires-Dist: pyyaml
+Requires-Dist: requests
+Requires-Dist: requests-file
+Requires-Dist: requests-toolbelt
+Requires-Dist: tqdm
+Requires-Dist: typing-extensions (>=4.7,<5.0)
+Requires-Dist: urllib3 (<2)
+Project-URL: Documentation, https://docs.espressif.com/projects/idf-component-manager/en/latest/
+Project-URL: Repository, https://github.com/espressif/idf-component-manager.git
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # IDF Component Manager
 
 The IDF Component manager is a tool that downloads dependencies for any [ESP-IDF](https://www.espressif.com/en/products/sdks/esp-idf) CMake project. It makes sure that the right versions of all components required for a successful build of your project are in place. The download happens automatically during a run of CMake. It can source components either from [the component registry](https://components.espressif.com/) or from a git repository.
 
 **A list of components can be found at https://components.espressif.com/**
 
@@ -194,7 +203,8 @@
 ```
 
 ## Resources
 
 - The Component manager [Documentation](https://docs.espressif.com/projects/idf-component-manager/en/latest/)
 - The Python Package Index project page https://pypi.org/project/idf-component-manager/
 - The Component Manager section in the [ESP-IDF Programming Guide](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-guides/tools/idf-component-manager.html)
+
```

### Comparing `idf_component_manager-1.5.2/README.md` & `idf_component_manager-2.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.5.2/idf_component_manager/__main__.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 #
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import argparse
 import os
 import sys
+import typing as t
 import warnings
 
 from idf_component_manager.utils import print_error, showwarning
 from idf_component_tools.errors import FatalError
 
 from . import version
 from .core import ComponentManager
@@ -27,16 +28,16 @@
     required_field = required_field or []
 
     for _f in required_field:
         if getattr(args, _f) is None:
             raise ValueError('--{} is required'.format(_f.replace('_', '-')))
 
 
-def main(command_args=None):  # type: (list[str] | None) -> None
-    parser = argparse.ArgumentParser(description='IDF component manager v{}'.format(version))
+def main(command_args: t.Optional[t.List[str]] = None) -> None:
+    parser = argparse.ArgumentParser(description=f'IDF component manager v{version}')
     parser.add_argument('command', choices=KNOWN_ACTIONS, help='Command to execute')
     parser.add_argument(
         '--path',
         help='Working directory (default: current directory).',
         default=os.getcwd(),
     )
     parser.add_argument(
@@ -107,15 +108,15 @@
             manager.upload_component_status(job_id=args.job, service_profile=args.service_profile)
         elif args.command == 'create-project-from-example':
             warnings.warn(
                 'Deprecated! New CLI command: "compote project create-from-example"',
                 DeprecationWarning,
             )
             check_required_args(args, ['namespace', 'name', 'example', 'version'])
-            example = '{}/{}={}:{}'.format(args.namespace, args.name, args.version, args.example)
+            example = f'{args.namespace}/{args.name}={args.version}:{args.example}'
             manager.create_project_from_example(example=example)
         elif args.command == 'delete-version':
             warnings.warn(
                 'Deprecated! New CLI command: "compote component delete"',
                 DeprecationWarning,
             )
             check_required_args(args, ['name', 'version'])
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/cli/autocompletion.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/cli/autocompletion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 import os
-import subprocess  # nosec
-from io import open
+import subprocess  # noqa: S404
+import typing as t
 
 import click
 
 from idf_component_manager.utils import print_info
 from idf_component_tools.errors import FatalError
 from idf_component_tools.semver import Version
 
 CLI_NAME = 'compote'
 CLICK_VERSION = Version.coerce(click.__version__)
 
 
-def _get_shell_completion(shell):  # type: (str) -> str
+def _get_shell_completion(shell: str) -> str:
     if CLICK_VERSION.major == 7:
         return 'source_' + shell
     elif CLICK_VERSION.major > 7:
         return shell + '_source'
     else:
         raise NotImplementedError
 
 
 def _append_text_line(
-    strings,  # type: str | list[str]
-    filepath,  # type: str
-    write_string=None,  # type: str | None
-    dry_run=False,  # type: bool
-):  # type: (...) -> None
+    strings: t.Union[str, t.List[str]],
+    filepath: str,
+    write_string: t.Optional[str] = None,
+    dry_run: bool = False,
+) -> None:
     if isinstance(strings, str):
         strings = [strings]
 
     if not os.path.isfile(filepath):
         lines = []
     else:
         with open(filepath, encoding='utf8') as fr:
@@ -45,35 +45,35 @@
             break
 
     if not found:
         if write_string is None:
             write_string = strings[-1]
 
         if dry_run:
-            print_info('"{}" would be appended to {}'.format(write_string, filepath))
+            print_info(f'"{write_string}" would be appended to {filepath}')
         else:
             with open(filepath, 'ab+') as fw:
-                fw.write('\n{}\n'.format(write_string).encode('utf8'))
+                fw.write(f'\n{write_string}\n'.encode())
 
 
 _COMPLETE_FILE_PATH = {
-    'bash': '~/.{}-complete.bash'.format(CLI_NAME),
-    'zsh': '~/.{}-complete.zsh'.format(CLI_NAME),
-    'fish': '~/.config/fish/completions/{}.fish'.format(CLI_NAME),
+    'bash': f'~/.{CLI_NAME}-complete.bash',
+    'zsh': f'~/.{CLI_NAME}-complete.zsh',
+    'fish': f'~/.config/fish/completions/{CLI_NAME}.fish',
 }
 
 _RC_FILE_PATH = {
     'bash': '~/.bashrc',
     'zsh': '~/.zshrc',
     'fish': None,  # not needed
 }
 
 _SOURCING_STR = {
-    'bash': '. {}'.format(_COMPLETE_FILE_PATH['bash']),
-    'zsh': '. {}'.format(_COMPLETE_FILE_PATH['zsh']),
+    'bash': f". {_COMPLETE_FILE_PATH['bash']}",
+    'zsh': f". {_COMPLETE_FILE_PATH['zsh']}",
     'fish': None,  # not needed
 }
 
 _DOC_STRSTRING = """
     Generate tab-completion scripts for the specified shell.
 
     \b
@@ -153,35 +153,33 @@
                     'library `click` version 7.1 and higher. An older version '
                     'is installed on your machine due to an outdated version of python. '
                     'We recommend using python 3.7 and higher with compote CLI.'
                 )
 
         # the return code could be 1 even succeeded
         # use || true to swallow the return code
-        autocomplete_script_str = subprocess.check_output(  # nosec
+        autocomplete_script_str = subprocess.check_output(
             '_{}_COMPLETE={} {} || true'.format(
                 CLI_NAME.upper(), _get_shell_completion(shell), CLI_NAME
             ),
-            shell=True,
-        ).decode(
-            'utf8'
-        )  # nosec
+            shell=True,  # noqa: S602
+        ).decode('utf8')
 
         if not install:  # print the autocomplete script only
             print(autocomplete_script_str)
             return
 
         # write autocomplete script
         completion_filepath = os.path.realpath(os.path.expanduser(_COMPLETE_FILE_PATH[shell]))
         if not os.path.isdir(os.path.dirname(completion_filepath)):
             if not dry_run:
                 os.makedirs(os.path.dirname(completion_filepath))
 
         if dry_run:
-            print_info('Completion file would be created at: {}'.format(completion_filepath))
+            print_info(f'Completion file would be created at: {completion_filepath}')
         else:
             with open(completion_filepath, 'w') as fw:
                 fw.write(autocomplete_script_str)
 
         # write sourcing autocomplete script statements
         if _RC_FILE_PATH[shell] and _SOURCING_STR[shell]:
             rc_filepath = os.path.realpath(os.path.expanduser(_RC_FILE_PATH[shell]))
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/cli/cache.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/cli/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     @cache.command()
     def clear():
         """
         Clear the cache of components and API client cache.
         """
         FileCache().clear()
-        print_info('Successfully cleared cache at\n\t{}'.format(FileCache().path()))
+        print_info(f'Successfully cleared cache at\n\t{FileCache().path()}')
 
     @cache.command()
     def path():
         """
         Print the cache path.
         """
         print_info(FileCache().path())
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/cli/component.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/cli/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,17 +56,15 @@
     @add_options(
         PROJECT_DIR_OPTION
         + NAMESPACE_NAME_OPTIONS
         + COMPONENT_VERSION_OPTION
         + DEST_DIR_OPTION
         + COMMIT_SHA_REPO_OPTION
     )
-    def pack(
-        manager, namespace, name, version, dest_dir, repository, commit_sha, repository_path
-    ):  # noqa: namespace is not used
+    def pack(manager, namespace, name, version, dest_dir, repository, commit_sha, repository_path):  # noqa: namespace is not used
         """
         Create component archive and store it in the dist directory.
         """
         manager.pack_component(
             name=name,
             version=version,
             dest_dir=dest_dir,
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/cli/constants.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/cli/constants.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.5.2/idf_component_manager/cli/core.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/cli/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 import sys
+import typing as t
 import warnings
 
 import click
 
 from idf_component_manager import version as idf_component_manager_version
 from idf_component_manager.utils import (
     CLICK_SUPPORTS_SHOW_DEFAULT,
@@ -17,22 +18,17 @@
 from .autocompletion import init_autocomplete
 from .cache import init_cache
 from .component import init_component
 from .manifest import init_manifest
 from .project import init_project
 from .registry import init_registry
 
-try:
-    from typing import Any
-except ImportError:
-    pass
-
-DEFAULT_SETTINGS = {
+DEFAULT_SETTINGS: t.Dict[str, t.Any] = {
     'help_option_names': ['-h', '--help'],
-}  # type: dict[str, Any]
+}
 
 if CLICK_SUPPORTS_SHOW_DEFAULT:
     DEFAULT_SETTINGS['show_default'] = True
 
 
 def initialize_cli():
     """
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/cli/manifest.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/cli/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 import json
 
 import click
 
 from idf_component_manager.utils import print_info
-from idf_component_tools.manifest.schemas import JSON_SCHEMA
+from idf_component_tools.manifest import MANIFEST_JSON_SCHEMA
 
 from .constants import get_project_dir_option, get_service_profile_option
 from .utils import add_options
 
 
 def init_manifest():
     PROJECT_DIR_OPTION = get_project_dir_option()
@@ -23,15 +23,15 @@
         pass
 
     @manifest.command()
     def schema():
         """
         Print json schema of the manifest file idf_component.yml
         """
-        print_info(json.dumps(JSON_SCHEMA, indent=2))
+        print_info(json.dumps(MANIFEST_JSON_SCHEMA, indent=2))
 
     MANIFEST_OPTION = [
         click.option('--component', default='main', help='Component name in the project.'),
         click.option(
             '-p',
             '--path',
             default=None,
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/cli/project.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/cli/project.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.5.2/idf_component_manager/cli/registry.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/cli/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 import os
+import typing as t
 import webbrowser
 
 import click
 import requests
-from six.moves import input
 
-from idf_component_manager.service_details import get_api_client
+from idf_component_manager.core import ComponentManager
 from idf_component_manager.utils import print_error, print_info
-from idf_component_tools.config import ConfigManager
+from idf_component_tools.config import ConfigManager, ServiceProfileItem
 from idf_component_tools.errors import FatalError
-from idf_component_tools.registry.api_client_errors import APIClientError
+from idf_component_tools.registry.client_errors import APIClientError
+from idf_component_tools.registry.service_details import NoSuchProfile, get_api_client
 
-from ..core import ComponentManager
 from .constants import get_project_dir_option, get_service_profile_option
 from .utils import add_options, deprecated_option
 
 
 def init_registry():
     @click.group()
     def registry():
@@ -67,31 +67,34 @@
         """
 
         if registry_url:
             os.environ['IDF_COMPONENT_REGISTRY_URL'] = registry_url
 
         # Load config for dump later
         config = ConfigManager().load()
-        profile = config.profiles.setdefault(service_profile, {})
+        if service_profile not in config.profiles:
+            profile = ServiceProfileItem()
+            config.profiles[service_profile] = profile
+        else:
+            profile = config.profiles[service_profile]
 
         # Check if token is already in the profile
-        if 'api_token' in profile:
+        if profile.api_token:
             raise FatalError(
                 'You are already logged in with profile "{}", '
                 'please either logout or use different profile'.format(service_profile)
             )
 
-        api_client, _ = get_api_client(
-            service_profile=service_profile,
+        api_client = get_api_client(
             namespace=default_namespace,
-            token_required=False,
-            raise_on_missing_profile=False,
+            service_profile=service_profile,
+            profile=profile,
         )
 
-        auth_url = '{}/tokens/'.format(api_client.frontend_url)
+        auth_url = f'{api_client.registry_url}/tokens/'
 
         auth_params = {
             'scope': 'user write:components',
             'description': description,
         }
         auth_request = requests.Request('GET', auth_url, params=auth_params).prepare()
 
@@ -112,47 +115,50 @@
         # Wait for token
         print_info('Please create a token in the browser window and paste here')
         token_valid = False
         while not token_valid:
             token = input('Token:')
 
             try:
-                api_client.auth_token = token
+                api_client.api_token = token
                 api_client.token_information()
                 token_valid = True
             except APIClientError as e:
                 # Handle 401 and 403 explicitly
-                print_error(
-                    'Provided token does not seem to be working: {}\nPlease try again.'.format(e)
-                )
+                print_error(f'Provided token does not seem to be working: {e}\nPlease try again.')
                 continue
 
         # Update config with token and default namespace, registry URL if they are provided
         if default_namespace:
-            profile['namespace'] = default_namespace
+            profile.default_namespace = default_namespace
         if registry_url:
-            profile['registry_url'] = registry_url
-        profile['api_token'] = token
+            profile.registry_url = registry_url
+        profile.api_token = token
 
         ConfigManager().dump(config)
 
         print_info('Successfully logged in')
 
     @registry.command()
     @add_options(get_service_profile_option())
     def logout(service_profile):
         # Load config to get
         config = ConfigManager().load()
 
         # Check if token is already in the profile
-        profile = config.profiles.setdefault(service_profile, {})
-        if 'api_token' not in profile:
+        profile = config.profiles.get(service_profile)
+        if profile is None:
+            raise NoSuchProfile(
+                f'Profile "{service_profile}" not found in the idf_component_manager.yml config file'
+            )
+
+        if profile.api_token is None:
             raise FatalError('You are not logged in')
 
-        del profile['api_token']
+        profile.api_token = None
         ConfigManager().dump(config)
 
         print_info('Successfully logged out')
 
     @registry.command()
     @add_options(get_service_profile_option() + get_project_dir_option())
     @click.option(
@@ -174,16 +180,21 @@
         default=[],
         help='Specify the components you want to upload to the mirror. '
         'Use multiple --component options for multiple components. '
         'Format: namespace/name<version_spec>. Example: example/cmp==1.0.0',
     )
     @click.argument('path', required=True)
     def sync(
-        manager, service_profile, interval, component, recursive, path
-    ):  # type: (ComponentManager, str, int, list[str], bool, str) -> None
+        manager: ComponentManager,
+        service_profile: str,
+        interval: int,
+        component: t.List[str],
+        recursive: bool,
+        path: str,
+    ) -> None:
         manager.sync_registry(
             service_profile,
             path,
             interval=interval,
             components=component,
             recursive=recursive,
         )
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/cli/utils.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/cli/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,8 +14,8 @@
         return func
 
     return wrapper
 
 
 def deprecated_option(ctx, param, value):
     if any(True for arg in sys.argv if arg.startswith(param.opts[0])):
-        warnings.warn('The option {} is deprecated.'.format(param.name), UserDeprecationWarning)
+        warnings.warn(f'The option {param.name} is deprecated.', UserDeprecationWarning)
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/cmake_component_requirements.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/cmake_component_requirements.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,103 +1,102 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import re
+import typing as t
 from collections import OrderedDict, namedtuple
-from io import open
 
 from idf_component_tools.errors import FatalError
 
-try:
-    from typing import Mapping
-except ImportError:
-    pass
-
 ComponentProperty = namedtuple('ComponentProperty', ['component', 'prop', 'value'])
 ITERABLE_PROPS = ['REQUIRES', 'PRIV_REQUIRES', 'MANAGED_REQUIRES', 'MANAGED_PRIV_REQUIRES']
 REQ_RE = re.compile(
     r'^__component_set_property\(___(?P<prefix>[a-zA-Z\d\-]+)_(?P<name>[a-zA-Z\d_\-\.\+]+)'
     r'\s+(?P<prop>\w+)\s+(?P<value>.*)\)'
 )
 
 
-def name_without_namespace(name):  # type: (str) -> str
+def name_without_namespace(name: str) -> str:
     name_parts = name.rsplit('__', 1)
 
     try:
         return name_parts[1]
     except IndexError:
         return name_parts[0]
 
 
-class ComponentName(object):
-    def __init__(self, prefix, name):  # type: (str, str) -> None
+class ComponentName:
+    def __init__(self, prefix: str, name: str) -> None:
         self.prefix = prefix
         self.name = name
 
-        self._name_without_namespace = None  # type: str | None
+        self._name_without_namespace: t.Optional[str] = None
 
-    def __eq__(self, another):  # type: (object) -> bool
+    def __eq__(self, another: object) -> bool:
         if not isinstance(another, ComponentName):
             return False
 
         return (self.prefix, self.name) == (another.prefix, another.name)
 
-    def __hash__(self):  # type: () -> int
+    def __hash__(self) -> int:
         return hash((self.prefix, self.name))
 
-    def __repr__(self):  # type: () -> str
-        return 'ComponentName({}, {})'.format(self.prefix, self.name)
+    def __repr__(self) -> str:
+        return f'ComponentName({self.prefix}, {self.name})'
 
     @property
-    def name_without_namespace(self):  # type: ()  -> str
+    def name_without_namespace(self) -> str:
         if self._name_without_namespace is None:
             self._name_without_namespace = name_without_namespace(self.name)
 
         return self._name_without_namespace
 
 
 class RequirementsProcessingError(FatalError):
     pass
 
 
-def parse_requirements_line(line):  # type: (str) -> ComponentProperty
+def parse_requirements_line(line: str) -> ComponentProperty:
     match = REQ_RE.match(line)
 
     if not match:
-        raise RequirementsProcessingError('Cannot parse CMake requirements line: %s' % line)
+        raise RequirementsProcessingError(f'Cannot parse CMake requirements line: {line}')
 
     return ComponentProperty(
         ComponentName(match.group('prefix'), match.group('name')),
         match.group('prop'),
         match.group('value'),
     )
 
 
-class CMakeRequirementsManager(object):
+class CMakeRequirementsManager:
     def __init__(self, path):
         self.path = path
 
-    def dump(self, requirements):  # type: (Mapping[ComponentName, dict[str, list | str]]) -> None
+    def dump(
+        self, requirements: t.Mapping[ComponentName, t.Dict[str, t.Union[t.List, str]]]
+    ) -> None:
         with open(self.path, mode='w', encoding='utf-8') as f:
             for name, requirement in requirements.items():
                 for prop, value in requirement.items():
                     if prop in ITERABLE_PROPS:
                         value = '"{}"'.format(';'.join(value))
 
                     f.write(
-                        u'__component_set_property(___{prefix}_{name} {prop} {value})\n'.format(
+                        '__component_set_property(___{prefix}_{name} {prop} {value})\n'.format(
                             prefix=name.prefix, name=name.name, prop=prop, value=value
                         )
                     )
 
-    def load(self):  # type: () -> OrderedDict[ComponentName, dict[str, list[str] | str]]
-        requirements = OrderedDict()  # type: OrderedDict[ComponentName, dict[str, list[str] | str]]
+    def load(self) -> t.OrderedDict[ComponentName, t.Dict[str, t.Union[t.List[str], str]]]:
+        requirements: t.OrderedDict[ComponentName, t.Dict[str, t.Union[t.List[str], str]]] = (
+            OrderedDict()
+        )
 
-        with open(self.path, mode='r', encoding='utf-8') as f:
+        with open(self.path, encoding='utf-8') as f:
             for line in f:
                 if line.strip():
                     prop = parse_requirements_line(line)
                     requirement = requirements.setdefault(prop.component, OrderedDict())
 
                     value = prop.value
                     if prop.prop in ITERABLE_PROPS:
@@ -109,26 +108,26 @@
 
                     requirement[prop.prop] = value
 
         return requirements
 
 
 def check_requirements_name_collisions(
-    requirements,
-):  # type: (dict[ComponentName, dict[str, list[str] | str]]) -> None
+    requirements: t.Dict[ComponentName, t.Dict[str, t.Union[t.List[str], str]]],
+) -> None:
     """
     DEPRECATE: This function is deprecated since interface_version 3,
         Remove it after ESP-IDF 5.1 EOL
     """
     # Pay attention only to components without namespaces
-    name_variants = {
+    name_variants: t.Dict[str, t.Set[str]] = {
         cmp.name: {cmp.name}
         for cmp in requirements.keys()
         if cmp.name == cmp.name_without_namespace
-    }  # type: dict[str, set[str]]
+    }
 
     for cmp in requirements.keys():
         if cmp.name_without_namespace not in name_variants:
             continue
 
         name_variants[cmp.name_without_namespace].add(cmp.name)
 
@@ -143,54 +142,54 @@
             'Cannot process component requirements. '
             'Multiple candidates to satisfy project requirements:\n{}'.format(
                 '\n'.join(descriptions)
             )
         )
 
 
-def _choose_component(component, known_components):  # type: (str, list[str]) -> str
+def _choose_component(component: str, known_components: t.List[str]) -> str:
     if component in known_components:
         return component
 
     # Name without namespace is required, but one with namespace is known
     # Or the the opposite: namespaced is known but required one without namespace
-    namespaced_name = '__{}'.format(component)
+    namespaced_name = f'__{component}'
     for known_component in known_components:
         if (
             known_component.endswith(namespaced_name)
             or name_without_namespace(component) == known_component
         ):
             return known_component
 
     # In this case CMake will fail due to unknown target
     return component
 
 
-def _handle_component_reqs(
-    components, known_components
-):  # type: (list[str], list[str]) -> list[str]
+def _handle_component_reqs(components: t.List[str], known_components: t.List[str]) -> t.List[str]:
     updated_items = []
     for component in components:
         name_to_add = _choose_component(component, known_components)
         if name_to_add not in updated_items:
             updated_items.append(name_to_add)
 
     return updated_items
 
 
 def handle_project_requirements(
-    requirements,
-):  # type: (OrderedDict[ComponentName, dict[str, list[str] | str]]) -> None
+    requirements: t.OrderedDict[ComponentName, t.Dict[str, t.Union[t.List[str], str]]],
+) -> None:
     """
     Use local components with higher priority.
     For example if in some manifest has a dependency `namespace/component`,
-    but there is a local component named `namespace__component` or `component` it will be used instead.
+    but there is a local component named `namespace__component` or `component`
+    it will be used instead.
     """
     known_components = [component_name.name for component_name in requirements.keys()]
     for component, requirement in requirements.items():
         for prop in ITERABLE_PROPS:
             if prop not in requirement:
                 continue
 
             requirements[component][prop] = _handle_component_reqs(
-                requirement[prop], known_components  # type: ignore # these props are always lists
+                requirement[prop],  # type: ignore # these props are always lists
+                known_components,  # type: ignore # these props are always lists
             )
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/core.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 """Core module of component manager"""
-from __future__ import print_function
 
 import functools
 import os
 import re
 import shutil
 import tarfile
 import tempfile
 import time
+import typing as t
 from collections import OrderedDict
 from datetime import datetime, timedelta
-from io import open
+from functools import lru_cache
 from pathlib import Path
 
 import requests
 from requests_toolbelt import MultipartEncoderMonitor
 
 from idf_component_manager.utils import ComponentSource, print_info, print_warn
 from idf_component_tools.archive_tools import pack_archive, unpack_archive
 from idf_component_tools.build_system_tools import build_name, is_component
 from idf_component_tools.config import root_managed_components_dir
+from idf_component_tools.constants import MANIFEST_FILENAME
 from idf_component_tools.environment import getenv_int
 from idf_component_tools.errors import (
     FatalError,
     InternalError,
     ManifestError,
     NothingToDoError,
     VersionAlreadyExistsError,
@@ -41,30 +42,31 @@
     HashDoesNotExistError,
     HashNotEqualError,
     HashNotSHA256Error,
 )
 from idf_component_tools.hash_tools.validate_managed_component import (
     validate_managed_component_hash,
 )
+from idf_component_tools.manager import (
+    ManifestManager,
+)
 from idf_component_tools.manifest import (
-    MANIFEST_FILENAME,
     WEB_DEPENDENCY_REGEX,
     Manifest,
-    ManifestManager,
-    ProjectRequirements,
 )
-from idf_component_tools.registry.api_client_errors import (
+from idf_component_tools.registry.client_errors import (
     APIClientError,
     ComponentNotFound,
     NetworkConnectionError,
     VersionNotFound,
 )
+from idf_component_tools.registry.service_details import get_api_client, get_storage_client
 from idf_component_tools.semver import SimpleSpec, Version
 from idf_component_tools.sources import WebServiceSource
-from idf_component_tools.utils import lru_cache
+from idf_component_tools.utils import ProjectRequirements
 
 from .cmake_component_requirements import (
     CMakeRequirementsManager,
     ComponentName,
     RequirementsProcessingError,
     check_requirements_name_collisions,
     handle_project_requirements,
@@ -75,22 +77,16 @@
     copy_examples_folders,
     dist_name,
     parse_example,
     raise_component_modified_error,
 )
 from .dependencies import download_project_dependencies
 from .local_component_list import parse_component_list
-from .service_details import get_api_client, get_storage_client
 from .sync import sync_components
 
-try:
-    from typing import Optional, Tuple
-except ImportError:
-    pass
-
 
 # PROCESSING_TIMEOUT
 def get_processing_timeout():
     try:
         return getenv_int('COMPONENT_MANAGER_JOB_TIMEOUT', 300)
     except ValueError:
         print_warn(
@@ -122,43 +118,46 @@
 
         except APIClientError as e:
             raise FatalError('\n'.join([str(e)] + e.request_info()))
 
     return wrapper
 
 
-def _create_manifest_if_missing(manifest_dir):  # type: (str) -> bool
+def _create_manifest_if_missing(manifest_dir: str) -> bool:
     manifest_filepath = os.path.join(manifest_dir, MANIFEST_FILENAME)
     if os.path.exists(manifest_filepath):
         return False
     example_path = os.path.join(
         os.path.dirname(os.path.realpath(__file__)), 'templates', 'idf_component_template.yml'
     )
     create_directory(manifest_dir)
     shutil.copyfile(example_path, manifest_filepath)
-    print_info('Created "{}"'.format(manifest_filepath))
+    print_info(f'Created "{manifest_filepath}"')
     return True
 
 
-class ComponentManager(object):
-    def __init__(self, path, lock_path=None, manifest_path=None, interface_version=0):
-        # type: (str, Optional[str], Optional[str], int) -> None
-
+class ComponentManager:
+    def __init__(
+        self,
+        path: str,
+        lock_path: t.Optional[str] = None,
+        manifest_path: t.Optional[str] = None,
+        interface_version: int = 0,
+    ) -> None:
         # Working directory
         path = os.path.abspath(path)
         self.path = path
 
         # Set path of the project's main component
-        self.main_component_path = os.path.join(path, 'main')
+        self.main_component_path = os.path.normpath(os.path.join(path, 'main'))
 
         # Set path of the manifest file for the project's main component
         self.main_manifest_path = manifest_path or (
             os.path.join(path, 'main', MANIFEST_FILENAME) if os.path.isdir(path) else path
         )
-        self.main_component_path = os.path.normpath(self.main_component_path)
 
         # Lock path
         if not lock_path:
             if os.path.isfile(path):
                 self.lock_path = path
             else:
                 self.lock_path = os.path.join(path, 'dependencies.lock')
@@ -174,15 +173,15 @@
         self.managed_components_path = os.path.join(self.path, 'managed_components')
 
         # Dist directory
         self.dist_path = os.path.join(self.path, 'dist')
 
         self.interface_version = interface_version
 
-    def _get_manifest_dir(self, component='main', path=None):  # type: (str, Optional[str]) -> str
+    def _get_manifest_dir(self, component: str = 'main', path: t.Optional[str] = None) -> str:
         if component != 'main' and path is not None:
             raise FatalError(
                 'Cannot determine manifest directory. Please specify either component or path.'
             )
 
         # If path is specified
         if path is not None:
@@ -208,105 +207,112 @@
                 'Please specify a valid component under {}'.format(manifest_dir, self.path)
             )
 
         return manifest_dir
 
     @property
     @lru_cache(1)
-    def root_managed_components_dir(self):  # type: () -> str
+    def root_managed_components_dir(self) -> str:
         return root_managed_components_dir()  # type: ignore
 
     @property
     @lru_cache(1)
-    def root_managed_components_lock_path(self):  # type: () -> str
+    def root_managed_components_lock_path(self) -> str:
         return os.path.join(self.root_managed_components_dir, 'dependencies.lock')  # type: ignore
 
     def _get_manifest(
-        self, component='main', path=None
-    ):  # type: (str, Optional[str]) -> Tuple[str, bool]
+        self, component: str = 'main', path: t.Optional[str] = None
+    ) -> t.Tuple[str, bool]:
         manifest_dir = self._get_manifest_dir(component=component, path=path)
         manifest_filepath = os.path.join(manifest_dir, MANIFEST_FILENAME)
         # Create manifest file if it doesn't exist in work directory
         manifest_created = _create_manifest_if_missing(manifest_dir)
         return manifest_filepath, manifest_created
 
     @general_error_handler
-    def create_manifest(self, component='main', path=None):  # type: (str, Optional[str]) -> None
+    def create_manifest(self, component: str = 'main', path: t.Optional[str] = None) -> None:
         manifest_filepath, created = self._get_manifest(component=component, path=path)
         if not created:
-            print_info('"{}" already exists, skipping...'.format(manifest_filepath))
+            print_info(f'"{manifest_filepath}" already exists, skipping...')
 
     @general_error_handler
-    def create_project_from_example(self, example, path=None, service_profile=None):
-        # type: (str, str | None, str | None) -> None
-        client, namespace = get_storage_client(None, service_profile)
-        component_name, version_spec, example_name = parse_example(example, namespace)
+    def create_project_from_example(
+        self, example: str, path: t.Optional[str] = None, service_profile: t.Optional[str] = None
+    ) -> None:
+        client = get_storage_client(None, service_profile)
+        component_name, version_spec, example_name = parse_example(
+            example, client.default_namespace
+        )
         project_path = path or os.path.join(self.path, os.path.basename(example_name))
 
         if os.path.isfile(project_path):
             raise FatalError(
                 'Your target path is not a directory. '
                 'Please remove the {} or use different target path.'.format(
                     os.path.abspath(project_path)
                 ),
                 exit_code=4,
             )
 
         if os.path.isdir(project_path) and os.listdir(project_path):
             raise FatalError(
-                'The directory {} is not empty. '
+                f'The directory {project_path} is not empty. '
                 'To create an example you must empty the directory or '
-                'choose a different path.'.format(project_path),
+                'choose a different path.',
                 exit_code=3,
             )
 
         component_details = client.component(component_name=component_name, version=version_spec)
 
         try:
             example_url = [
-                example for example in component_details.examples if example_name == example['name']
+                example
+                for example in component_details['examples']
+                if example_name == example['name']
             ][-1]
         except IndexError:
             raise FatalError(
-                'Cannot find example "{}" for "{}" version "{}"'.format(
-                    example_name, component_name, version_spec
-                ),
+                f'Cannot find example "{example_name}" for "{component_name}" '
+                f'version "{version_spec}"',
                 exit_code=2,
             )
 
-        response = requests.get(example_url['url'], stream=True)
+        response = requests.get(example_url['url'], stream=True)  # noqa: S113
         with tarfile.open(fileobj=response.raw, mode='r|gz') as tar:
-            tar.extractall(project_path)
+            tar.extractall(project_path)  # noqa: S202
         print_info(
             'Example "{}" successfully downloaded to {}'.format(
                 example_name, os.path.abspath(project_path)
             )
         )
 
     @general_error_handler
     def add_dependency(
-        self, dependency, component='main', path=None, service_profile=None
-    ):  # type: (str, str, Optional[str], str | None) -> None
+        self,
+        dependency: str,
+        component: str = 'main',
+        path: t.Optional[str] = None,
+        service_profile: t.Optional[str] = None,
+    ) -> None:
         manifest_filepath, _ = self._get_manifest(component=component, path=path)
-        client, _ = get_storage_client(None, service_profile)
 
         if path is not None:
             component_path = os.path.abspath(path)
             component = os.path.basename(component_path)
         # If the path refers to a component context
         # we need to use the components name as the component
         elif is_component(Path(os.getcwd())):
             component = os.path.basename(os.path.normpath(self.path))
 
         match = re.match(WEB_DEPENDENCY_REGEX, dependency)
         if match:
             name, spec = match.groups()
         else:
             raise FatalError(
-                'Invalid dependency: "{}". Please use format "namespace/name".'.format(dependency)
+                f'Invalid dependency: "{dependency}". Please use format "namespace/name".'
             )
 
         if not spec:
             spec = '*'
 
         try:
             SimpleSpec(spec)
@@ -315,41 +321,46 @@
                 'Invalid dependency version requirement: {}. '
                 'Please use format like ">=1" or "*".'.format(spec)
             )
 
         name = WebServiceSource().normalized_name(name)
 
         # Check if dependency exists in the registry
+        # make sure it exists in the registry's storage url
+        client = get_storage_client(service_profile=service_profile).registry_storage_client
+        if not client:
+            raise InternalError()
+
         client.component(component_name=name, version=spec)
 
         manifest_manager = ManifestManager(manifest_filepath, component)
         manifest = manifest_manager.load()
 
-        for dep in manifest.raw_dependencies:
+        for dep in manifest.raw_requirements:
             if dep.name == name:
                 raise FatalError(
                     'Dependency "{}" already exists for in manifest "{}"'.format(
                         name, manifest_filepath
                     )
                 )
 
-        with open(manifest_filepath, 'r', encoding='utf-8') as file:
+        with open(manifest_filepath, encoding='utf-8') as file:
             file_lines = file.readlines()
 
         index = 0
         if 'dependencies' in manifest_manager.manifest_tree.keys():
             for i, line in enumerate(file_lines):
                 if line.startswith('dependencies:'):
                     index = i + 1
                     break
         else:
             file_lines.append('\ndependencies:\n')
             index = len(file_lines) + 1
 
-        file_lines.insert(index, '  {}: "{}"\n'.format(name, spec))
+        file_lines.insert(index, f'  {name}: "{spec}"\n')
 
         # Check result for correctness
         with tempfile.NamedTemporaryFile(delete=False) as temp_manifest_file:
             temp_manifest_file.writelines(line.encode('utf-8') for line in file_lines)
 
         try:
             ManifestManager(temp_manifest_file.name, name).load()
@@ -366,16 +377,22 @@
             'Successfully added dependency "{}{}" to component "{}"'.format(
                 name, spec, manifest_manager.name
             )
         )
 
     @general_error_handler
     def pack_component(
-        self, name, version, dest_dir=None, repository=None, commit_sha=None, repository_path=None
-    ):  # type: (str, str, str | None, str | None, str | None, str | None) -> tuple[str, Manifest]
+        self,
+        name: str,
+        version: t.Optional[str] = None,
+        dest_dir: t.Optional[str] = None,
+        repository: t.Optional[str] = None,
+        commit_sha: t.Optional[str] = None,
+        repository_path: t.Optional[str] = None,
+    ) -> t.Tuple[str, Manifest]:
         dest_path = os.path.join(self.path, dest_dir) if dest_dir else self.dist_path
 
         if version == 'git':
             version = str(GitClient().get_tag_version(cwd=self.path))
         elif version:
             try:
                 # In CI the version can come from a git tag, handle it with the same logic
@@ -388,88 +405,95 @@
                     'Documentation: https://docs.espressif.com/projects/idf-component-manager/en/'
                     'latest/reference/versioning.html#versioning-scheme'.format(version)
                 )
 
         manifest_manager = ManifestManager(
             self.path,
             name,
-            check_required_fields=True,
             version=version,
             repository=repository,
             commit_sha=commit_sha,
             repository_path=repository_path,
         )
         manifest = manifest_manager.load()
-        dest_temp_dir = Path(dest_path, dist_name(manifest))
-        include = set(manifest.files['include'])
-        exclude = set(manifest.files['exclude'])
-        copy_filtered_directory(self.path, str(dest_temp_dir), include=include, exclude=exclude)
+        dest_temp_dir = Path(dest_path, dist_name(name, manifest.version))
+        copy_filtered_directory(
+            self.path,
+            str(dest_temp_dir),
+            include=manifest.include_set,
+            exclude=manifest.exclude_set,
+        )
 
         if manifest.examples:
             copy_examples_folders(
-                manifest.examples, Path(self.path), dest_temp_dir, include=include, exclude=exclude
+                manifest.examples,
+                Path(self.path),
+                dest_temp_dir,
+                include=manifest.include_set,
+                exclude=manifest.exclude_set,
             )
 
         manifest_manager.dump(str(dest_temp_dir))
 
         check_unexpected_component_files(str(dest_temp_dir))
 
-        archive_filepath = os.path.join(dest_path, archive_filename(manifest))
-        print_info('Saving archive to "{}"'.format(archive_filepath))
+        archive_filepath = os.path.join(dest_path, archive_filename(name, manifest.version))
+        print_info(f'Saving archive to "{archive_filepath}"')
         pack_archive(str(dest_temp_dir), archive_filepath)
         return archive_filepath, manifest
 
     @general_error_handler
     def delete_version(
         self,
-        name,  # type: str
-        version,  # type: str
-        service_profile=None,  # type: str | None
-        namespace=None,  # type: str | None
-    ):  # type: (...) -> None
-        client, namespace = get_api_client(namespace, service_profile)
+        name: str,
+        version: str,
+        service_profile: t.Optional[str] = None,
+        namespace: t.Optional[str] = None,
+    ) -> None:
         if not version:
             raise FatalError('Argument "version" is required')
 
-        component_name = '/'.join([namespace, name])
+        api_client = get_api_client(namespace, service_profile)
+        component_name = '/'.join([api_client.default_namespace, name])
+
         # Checking if current version already uploaded
-        versions = client.versions(component_name=component_name).versions
+        versions = api_client.versions(component_name=component_name).versions
 
         if version not in versions:
             raise VersionNotFoundError(
                 'Version {} of the component "{}" is not on the registry'.format(
                     version, component_name
                 )
             )
 
-        client.delete_version(component_name=component_name, component_version=version)
-        print_info('Deleted version {} of the component {}'.format(version, component_name))
+        api_client.delete_version(component_name=component_name, component_version=version)
+        print_info(f'Deleted version {version} of the component {component_name}')
 
     @general_error_handler
     def yank_version(
         self,
-        name,  # type: str
-        version,  # type: str
-        message,  # type: str
-        service_profile=None,  # type: str | None
-        namespace=None,  # type: str | None
+        name: str,
+        version: str,
+        message: str,
+        service_profile: t.Optional[str] = None,
+        namespace: t.Optional[str] = None,
     ):
-        client, namespace = get_api_client(namespace, service_profile)
-        component_name = '/'.join([namespace, name])
+        api_client = get_api_client(namespace, service_profile)
+        component_name = '/'.join([api_client.default_namespace, name])
 
-        versions = client.versions(component_name=component_name).versions
+        versions = api_client.versions(component_name=component_name).versions
 
         if version not in versions:
             raise VersionNotFoundError(
                 'Version {} of the component "{}" is not on the registry'.format(
                     version, component_name
                 )
             )
 
-        client.yank_version(
+        api_client.yank_version(
             component_name=component_name, component_version=version, yank_message=message
         )
         print_info(
             'Version {} of the component {} was yanked due to reason "{}"'.format(
                 component_name, version, message
             )
         )
@@ -501,74 +525,65 @@
 
         elif any(managed_components_dir.iterdir()) == 0:
             shutil.rmtree(str(managed_components_dir))
 
     @general_error_handler
     def upload_component(
         self,
-        name,  # type: str
-        version=None,  # type: str | None
-        service_profile=None,  # type: str | None
-        namespace=None,  # type: str | None
-        archive=None,  # type: str | None
-        skip_pre_release=False,  # type: bool
-        check_only=False,  # type: bool
-        allow_existing=False,  # type: bool
-        dry_run=False,  # type: bool
-        dest_dir=None,  # type: str | None
-        repository=None,  # type: str | None
-        commit_sha=None,  # type: str | None
-        repository_path=None,  # type: str | None
-    ):  # type: (...) -> None
+        name: str,
+        version: t.Optional[str] = None,
+        service_profile: t.Optional[str] = None,
+        namespace: t.Optional[str] = None,
+        archive: t.Optional[str] = None,
+        skip_pre_release: bool = False,
+        check_only: bool = False,
+        allow_existing: bool = False,
+        dry_run: bool = False,
+        dest_dir: t.Optional[str] = None,
+        repository: t.Optional[str] = None,
+        commit_sha: t.Optional[str] = None,
+        repository_path: t.Optional[str] = None,
+    ) -> None:
         """
         Uploads a component version to the registry.
         """
-        token_required = not (check_only or dry_run)
-        client, namespace = get_api_client(
-            namespace, service_profile, token_required=token_required
-        )
+        api_client = get_api_client(namespace, service_profile)
 
         if archive:
             if not os.path.isfile(archive):
-                raise FatalError('Cannot find archive to upload: {}'.format(archive))
+                raise FatalError(f'Cannot find archive to upload: {archive}')
 
             if version:
                 raise FatalError(
                     'Parameters "version" and "archive" are not supported at the same time'
                 )
 
             tempdir = tempfile.mkdtemp()
             try:
                 unpack_archive(archive, tempdir)
-                manifest = ManifestManager(tempdir, name, check_required_fields=True).load()
+                manifest = ManifestManager(tempdir, name, upload_mode=True).load()
             finally:
                 shutil.rmtree(tempdir)
         else:
             archive, manifest = self.pack_component(
                 name=name,
                 version=version,
                 dest_dir=dest_dir,
                 repository=repository,
                 commit_sha=commit_sha,
                 repository_path=repository_path,
             )
 
-        if not manifest.version:
-            raise FatalError('"version" field is required when uploading the component')
-
-        if not manifest.version.is_semver:
-            raise FatalError('Only components with semantic versions are allowed on the service')
-
         if manifest.version.semver.prerelease and skip_pre_release:
-            raise NothingToDoError('Skipping pre-release version {}'.format(manifest.version))
+            raise NothingToDoError(f'Skipping pre-release version {manifest.version}')
 
-        component_name = '/'.join([namespace, manifest.name])
+        component_name = '/'.join([api_client.default_namespace, name])
         # Checking if current version already uploaded
         try:
-            versions = client.versions(component_name=component_name, spec='*').versions
+            versions = api_client.versions(component_name=component_name, spec='*').versions
 
             if manifest.version in versions:
                 if allow_existing:
                     return
 
                 raise VersionAlreadyExistsError(
                     'Version {} of the component "{}" is already on the registry'.format(
@@ -581,40 +596,40 @@
 
         # Exit if check flag was set
         if check_only:
             return
 
         # Uploading/validating the component
         info_message = 'Uploading' if not dry_run else 'Validating'
-        print_info('{} archive {}'.format(info_message, archive))
+        print_info(f'{info_message} archive {archive}')
 
         file_stat = os.stat(archive)  # type: ignore
         with ProgressBar(
             total=file_stat.st_size, unit='B', unit_scale=True, leave=False
         ) as progress_bar:
             memo = {'progress': 0}
 
-            def callback(monitor):  # type: (MultipartEncoderMonitor) -> None
+            def callback(monitor: MultipartEncoderMonitor) -> None:
                 progress_bar.update(monitor.bytes_read - memo['progress'])
                 memo['progress'] = monitor.bytes_read
 
             if dry_run:
-                job_id = client.validate_version(file_path=archive, callback=callback)
+                job_id = api_client.validate_version(file_path=archive, callback=callback)
             else:
-                job_id = client.upload_version(
+                job_id = api_client.upload_version(
                     component_name=component_name, file_path=archive, callback=callback
                 )
 
             progress_bar.close()
 
         # Wait for processing
         profile_text = (
             ''
             if service_profile is None or service_profile == 'default'
-            else ' --service-profile={}'.format(service_profile)
+            else f' --service-profile={service_profile}'
         )
         print_info(
             'Wait for processing, it is safe to press CTRL+C and exit\n'
             'You can check the state of processing by running CLI command '
             '"compote component upload-status --job={} {}"'.format(job_id, profile_text)
         )
 
@@ -622,15 +637,15 @@
 
         try:
             warnings = set()
             with ProgressBar(total=MAX_PROGRESS, unit='%', leave=False) as progress_bar:
                 while True:
                     if datetime.now() > timeout_at:
                         raise TimeoutError()
-                    status = client.task_status(job_id=job_id)
+                    status = api_client.task_status(job_id=job_id)
 
                     for warning in status.warnings:
                         if warning not in warnings:
                             warnings.add(warning)
 
                     if status.status == 'failure' or status.status == 'success':
                         progress_bar.close()
@@ -654,29 +669,26 @@
 
                     progress_bar.set_description(status.message)
                     progress_bar.update_to(status.progress)
 
                     time.sleep(CHECK_INTERVAL)
         except TimeoutError:
             raise FatalError(
-                "Component wasn't processed in {} seconds. Check processing status later.".format(
-                    get_processing_timeout()
-                )
+                f"Component wasn't processed in {get_processing_timeout()} seconds. "
+                'Check processing status later.'
             )
 
     @general_error_handler
-    def upload_component_status(
-        self, job_id, service_profile=None
-    ):  # type: (str, str | None) -> None
-        client, _ = get_api_client(None, service_profile)
-        status = client.task_status(job_id=job_id)
+    def upload_component_status(self, job_id: str, service_profile: t.Optional[str] = None) -> None:
+        api_client = get_api_client(None, service_profile)
+        status = api_client.task_status(job_id=job_id)
         if status.status == 'failure':
-            raise FatalError("Uploaded version wasn't processed successfully.\n%s" % status.message)
+            raise FatalError(f"Uploaded version wasn't processed successfully.\n{status.message}")
         else:
-            print_info('Status: %s. %s' % (status.status, status.message))
+            print_info(f'Status: {status.status}. {status.message}')
 
     def update_dependencies(self, **kwargs):
         if os.path.isfile(self.lock_path):
             os.remove(self.lock_path)
 
     # Function executed from CMake
 
@@ -685,24 +697,20 @@
         self, managed_components_list_file, component_list_file, local_components_list_file=None
     ):
         """Process all manifests and download all dependencies"""
         # root core components
         root_manifest_filepath = os.path.join(root_managed_components_dir(), MANIFEST_FILENAME)
         if os.path.isfile(root_manifest_filepath):
             root_managed_components = download_project_dependencies(
-                ProjectRequirements(
-                    [
-                        ManifestManager(
-                            self.root_managed_components_dir,
-                            'root',
-                            expand_environment=True,
-                            process_opt_deps=True,
-                        ).load()
-                    ]
-                ),
+                ProjectRequirements([
+                    ManifestManager(
+                        self.root_managed_components_dir,
+                        'root',
+                    ).load()
+                ]),
                 self.root_managed_components_lock_path,
                 self.root_managed_components_dir,
                 is_idf_root_dependencies=True,
             )
         else:
             root_managed_components = []
 
@@ -733,16 +741,14 @@
             manifests = []
 
             for component in local_components:
                 manifests.append(
                     ManifestManager(
                         component['path'],
                         component['name'],
-                        expand_environment=True,
-                        process_opt_deps=True,
                     ).load()
                 )
 
             project_requirements = ProjectRequirements(manifests)
             downloaded_components = download_project_dependencies(
                 project_requirements, self.lock_path, self.managed_components_path
             )
@@ -751,109 +757,109 @@
         downloaded_components = {
             comp
             for comp in downloaded_components
             if comp.downloaded_path not in [local_comp['path'] for local_comp in local_components]
         }
 
         # Include managed components in project directory
-        all_managed_components = set(
-            sorted(downloaded_components) + sorted(root_managed_components)
-        )
+        # order is important, since kconfig items are processed in order
+        downloaded_components = sorted(downloaded_components)
+        root_managed_components = sorted(root_managed_components)
+        all_managed_components = sorted(set(downloaded_components + root_managed_components))
+
         with open(managed_components_list_file, mode='w', encoding='utf-8') as file:
             for is_root, group in enumerate([downloaded_components, root_managed_components]):
                 for downloaded_component in group:
                     file.write(
-                        u'idf_build_component("{}" "{}")\n'.format(
+                        'idf_build_component("{}" "{}")\n'.format(
                             downloaded_component.abs_posix_path,
                             'idf_components' if is_root == 1 else 'project_managed_components',
                         )
                     )
                     file.write(
-                        u'idf_component_set_property({} {} "{}")\n'.format(
+                        'idf_component_set_property({} {} "{}")\n'.format(
                             downloaded_component.name,
                             'COMPONENT_VERSION',
                             downloaded_component.version,
                         )
                     )
 
                     if downloaded_component.targets:
                         file.write(
-                            u'idf_component_set_property({} {} "{}")\n'.format(
+                            'idf_component_set_property({} {} "{}")\n'.format(
                                 downloaded_component.name,
                                 'REQUIRED_IDF_TARGETS',
                                 ' '.join(downloaded_component.targets),
                             )
                         )
 
             file.write(
-                u'set(managed_components "%s")\n'
+                'set(managed_components "%s")\n'
                 % ';'.join(component.name for component in all_managed_components)
             )
 
         # Saving list of all components with manifests for use on requirements injection step
         all_components = sorted(
-            set(component.abs_path for component in all_managed_components).union(
+            {component.abs_path for component in all_managed_components}.union(
                 component['path'] for component in local_components
             )
         )
         with open(component_list_file, mode='w', encoding='utf-8') as file:
-            file.write(u'\n'.join(all_components))
+            file.write('\n'.join(all_components))
 
     @general_error_handler
     def inject_requirements(
         self,
-        component_requires_file,  # type: Path | str
-        component_list_file,  # type: Path | str
+        component_requires_file: t.Union[Path, str],
+        component_list_file: t.Union[Path, str],
     ):
-        '''Set build dependencies for components with manifests'''
+        """Set build dependencies for components with manifests"""
         requirements_manager = CMakeRequirementsManager(component_requires_file)
         requirements = requirements_manager.load()
 
         try:
-            with open(component_list_file, mode='r', encoding='utf-8') as f:
+            with open(component_list_file, encoding='utf-8') as f:
                 components_with_manifests = f.readlines()
             os.remove(component_list_file)
         except FileNotFoundError:
             raise FatalError(
                 'Cannot find component list file. '
                 'Please make sure this script is executed from CMake'
             )
 
         add_all_components_to_main = False
         for component in components_with_manifests:
             component = component.strip()
             name = os.path.basename(component)
-            manifest = ManifestManager(
-                component, name, expand_environment=True, process_opt_deps=True
-            ).load()
+            manifest = ManifestManager(component, name).load()
             name_key = ComponentName('idf', name)
 
-            for dependency in manifest.dependencies:
+            for dep in manifest.requirements:
                 # Meta dependencies, like 'idf' are not used directly
-                if dependency.meta:
+                if dep.meta:
                     continue
 
                 # No required dependencies shouldn't be added to the build system
-                if not dependency.require:
+                if not dep.is_required:
                     continue
 
-                dependency_name = build_name(dependency.name)
-                requirement_key = 'REQUIRES' if dependency.public else 'PRIV_REQUIRES'
+                dependency_name = build_name(dep.name)
+                requirement_key = 'REQUIRES' if dep.is_public else 'PRIV_REQUIRES'
 
-                def add_req(key):  # type: (str) -> None
+                def add_req(key: str) -> None:
                     if key not in requirements[name_key]:
                         requirements[name_key][key] = []
 
                     req = requirements[name_key][key]
                     if isinstance(req, list) and dependency_name not in req:
                         req.append(dependency_name)
 
                 add_req(requirement_key)
 
-                managed_requirement_key = 'MANAGED_{}'.format(requirement_key)
+                managed_requirement_key = f'MANAGED_{requirement_key}'
                 add_req(managed_requirement_key)
 
                 # In interface v0, component_requires_file contains also common requirements
                 if self.interface_version == 0 and name_key == ComponentName('idf', 'main'):
                     add_all_components_to_main = True
 
         # If there are dependencies added to the `main` component,
@@ -882,16 +888,16 @@
             check_requirements_name_collisions(new_requirements)
 
         handle_project_requirements(new_requirements)
         requirements_manager.dump(new_requirements)
 
     @staticmethod
     def _override_requirements_by_component_sources(
-        requirements,  # type: OrderedDict[ComponentName, dict[str, list[str] | str]]
-    ):  # type: (...) -> OrderedDict[ComponentName, dict[str, list[str] | str]]
+        requirements: t.OrderedDict[ComponentName, t.Dict[str, t.Union[t.List[str], str]]],
+    ) -> t.OrderedDict[ComponentName, t.Dict[str, t.Union[t.List[str], str]]]:
         """
         group the requirements, the overriding sequence here is: (the latter, the higher priority)
         - idf_components (IDF_PATH/components)
         - idf_managed_components (IDF_TOOLS_DIR/root_managed_components/idf5.3/managed_components)
         - project_managed_components (project_managed_components)
         - project_extra_components (project_extra_components)
         - project_components (PROJECT_DIR/components)
@@ -909,15 +915,15 @@
             elif props['__COMPONENT_SOURCE'] == ComponentSource.PROJECT_MANAGED_COMPONENTS:
                 project_managed_components[comp_name] = props
             elif props['__COMPONENT_SOURCE'] == ComponentSource.PROJECT_EXTRA_COMPONENTS:
                 project_extra_components[comp_name] = props
             elif props['__COMPONENT_SOURCE'] == ComponentSource.PROJECT_COMPONENTS:
                 project_components[comp_name] = props
             else:
-                raise InternalError
+                raise InternalError()
 
         # overriding the sequence
         new_requirements = project_components
         for component_group in [
             project_extra_components,
             project_managed_components,
             idf_components,
@@ -967,17 +973,22 @@
                             props['__COMPONENT_SOURCE'],
                         )
                     )
 
         return new_requirements
 
     def sync_registry(
-        self, service_profile, save_path, interval=0, components=None, recursive=True
-    ):  # type: (str, str | Path, int, list[str] | None, bool) -> None
-        client, namespace = get_storage_client(None, service_profile)
+        self,
+        service_profile: str,
+        save_path: t.Union[str, Path],
+        interval: int = 0,
+        components: t.Optional[t.List[str]] = None,
+        recursive: bool = True,
+    ) -> None:
+        client = get_storage_client(None, service_profile)
         save_path = Path(save_path)
         if interval:
             while True:
-                sync_components(client, self.path, namespace, save_path, components, recursive)
+                sync_components(client, self.path, save_path, components, recursive)
                 time.sleep(interval)
         else:
-            sync_components(client, self.path, namespace, save_path, components, recursive)
+            sync_components(client, self.path, save_path, components, recursive)
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/core_utils.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/core_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 import os
 import re
+import typing as t
 from collections import namedtuple
 from pathlib import Path
 
 from tqdm import tqdm
 
 from idf_component_tools.constants import DEFAULT_NAMESPACE
 from idf_component_tools.errors import ComponentModifiedError, FatalError
 from idf_component_tools.file_tools import copy_directories, filtered_paths
 from idf_component_tools.hash_tools.constants import HASH_FILENAME
-from idf_component_tools.manifest import Manifest
 from idf_component_tools.manifest.constants import SLUG_BODY_REGEX
 from idf_component_tools.semver import SimpleSpec
 
 CREATE_PROJECT_FROM_EXAMPLE_NAME_REGEX = (
     r'^((?P<namespace>{slug})\/)?'
     r'(?P<component>{slug})'
     r'(?P<version>[<=>!^~\*].+)?:'
@@ -27,32 +27,27 @@
     r'^((?P<namespace>{slug})\/)?' r'(?P<component>{slug})' r'(?P<version>[<=>!^~\*].+)?'
 ).format(slug=SLUG_BODY_REGEX)
 
 
 class ProgressBar(tqdm):
     """Wrapper for tqdm for updating progress bar status"""
 
-    def update_to(self, count):  # type: (int) -> bool | None
+    def update_to(self, count: t.Union[int, float]) -> t.Optional[bool]:
         return self.update(count - self.n)
 
 
-def dist_name(manifest):  # type: (Manifest) -> str
-    if manifest.version is None:
-        raise ValueError('Version is required in this manifest')
+def dist_name(name: str, version: str) -> str:
+    return f'{name}_{version}'
 
-    return '{}_{}'.format(manifest.name, manifest.version)
 
+def archive_filename(name: str, version: str) -> str:
+    return f'{dist_name(name, version)}.tgz'
 
-def archive_filename(manifest):  # type: (Manifest) -> str
-    return '{}.tgz'.format(dist_name(manifest))
 
-
-def raise_component_modified_error(
-    managed_components_dir, components
-):  # type: (str, list[str]) -> None
+def raise_component_modified_error(managed_components_dir: str, components: t.List[str]) -> None:
     project_path = Path(managed_components_dir).parent
     component_example_name = components[0].replace('/', '__')
     managed_component_dir = Path(managed_components_dir, component_example_name)
     component_dir = project_path / 'components' / component_example_name
     hash_path = managed_component_dir / HASH_FILENAME
     error = (
         'Some components ({component_names}) in the "managed_components" directory were modified '
@@ -60,29 +55,29 @@
         'Content of this directory is managed automatically.\n'
         'If you want to keep the changes, '
         'you can move the directory with the component to the "components"'
         'directory of your project.\n'
         'I.E. for "{component_example}" run:\n'
         'mv {managed_component_dir} {component_dir}\n'
         'Or, if you want to discard the changes remove the "{hash_filename}" file '
-        'from the component\'s directory.\n'
+        "from the component's directory.\n"
         'I.E. for "{component_example}" run:\n'
         'rm {hash_path}'
     ).format(
         component_names=', '.join(components),
         component_example=component_example_name,
         managed_component_dir=managed_component_dir,
         component_dir=component_dir,
         hash_path=hash_path,
         hash_filename=HASH_FILENAME,
     )
     raise ComponentModifiedError(error)
 
 
-def parse_example(example, namespace):  # type: (str, str) -> tuple[str, str, str]
+def parse_example(example: str, namespace: str) -> t.Tuple[str, str, str]:
     match = re.match(CREATE_PROJECT_FROM_EXAMPLE_NAME_REGEX, example)
     if not match:
         raise FatalError(
             'Cannot parse EXAMPLE argument. '
             'Please use format like: namespace/component=1.0.0:example_name'
         )
 
@@ -91,76 +86,72 @@
     version_spec = match.group('version') or '*'
     example_name = match.group('example')
 
     try:
         SimpleSpec(version_spec)
     except ValueError:
         raise FatalError(
-            'Invalid version specification: "{}". Please use format like ">=1" or "*".'.format(
-                version_spec
-            )
+            f'Invalid version specification: "{version_spec}". Please use format like ">=1" or "*".'
         )
 
-    return '{}/{}'.format(namespace, component), version_spec, example_name
+    return f'{namespace}/{component}', version_spec, example_name
 
 
 ComponentInfo = namedtuple('ComponentInfo', ['component_name', 'version_spec'])
 
 
-def parse_component(component_name, namespace):  # type: (str, str) -> ComponentInfo
+def parse_component(component_name: str, namespace: str) -> ComponentInfo:
     match = re.match(SYNC_REGISTRY_COMPONENT_NAME_REGEX, component_name)
     if not match:
         raise FatalError(
             'Cannot parse COMPONENT argument. ' 'Please use format like: namespace/component=1.0.0'
         )
 
     namespace = match.group('namespace') or namespace or DEFAULT_NAMESPACE
     component = match.group('component')
     version_spec = match.group('version') or '*'
 
     try:
         SimpleSpec(version_spec)
     except ValueError:
         raise FatalError(
-            'Invalid version specification: "{}". Please use format like ">=1" or "*".'.format(
-                version_spec
-            )
+            f'Invalid version specification: "{version_spec}". Please use format like ">=1" or "*".'
         )
 
-    return ComponentInfo('{}/{}'.format(namespace, component), version_spec)
+    return ComponentInfo(f'{namespace}/{component}', version_spec)
 
 
-def collect_directories(dir_path):  # type: (Path) -> list[str]
-    directories = []  # type: list[str]
+def collect_directories(dir_path: Path) -> t.List[str]:
+    directories: t.List[str] = []
     if not dir_path.is_dir():
         return directories
 
     for directory in os.listdir(str(dir_path)):
         if directory.startswith('.') or not (dir_path / directory).is_dir():
             continue
 
         directories.append(directory)
 
     return directories
 
 
-def detect_duplicate_examples(example_folders, example_path, example_name):  # type ()
+def detect_duplicate_examples(example_folders, example_path, example_name):
     for key, value in example_folders.items():
         if example_name in value:
             return key, example_path, example_name
     return
 
 
 def copy_examples_folders(
-    examples_manifest,  # type: list[dict[str,str]]
-    working_path,  # type: Path
-    dist_dir,  # type: Path
-    include=None,  # type: set[str] | None
-    exclude=None,  # type: set[str] | None
-):  # type: (...) -> None
+    examples_manifest: t.List[t.Dict[str, str]],
+    working_path: Path,
+    dist_dir: Path,
+    include: t.Optional[t.Set[str]] = None,
+    exclude: t.Optional[t.Set[str]] = None,
+) -> None:
     examples_path = working_path / 'examples'
     example_folders = {'examples': collect_directories(examples_path)}
     error_paths = []
     duplicate_paths = []
     for example_info in examples_manifest:
         example_path = example_info['path']
         example_name = Path(example_path).name
@@ -193,14 +184,13 @@
             'in `idf_component.yml` file'.format(', '.join(error_paths))
         )
 
     if duplicate_paths:
         error_messages = []
         for first_path, second_path, example_name in duplicate_paths:
             error_messages.append(
-                'Examples from "{}" and "{}" have the same name: {}.'.format(
-                    first_path, second_path, example_name
-                )
+                f'Examples from "{first_path}" and "{second_path}" '
+                f'have the same name: {example_name}.'
             )
         error_messages.append('Please rename one of them, or delete if there are the same')
 
         raise FatalError('\n'.join(error_messages))
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/dependencies.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/dependencies.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,196 +1,198 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 import shutil
+import typing as t
 from functools import total_ordering
 from pathlib import Path
 
 from idf_component_manager.core_utils import raise_component_modified_error
-from idf_component_manager.utils import print_info, print_warn
+from idf_component_manager.utils import print_info, print_notice
 from idf_component_manager.version_solver.helper import parse_root_dep_conflict_constraints
 from idf_component_manager.version_solver.mixology.failure import SolverFailure
 from idf_component_manager.version_solver.mixology.package import Package
 from idf_component_manager.version_solver.version_solver import VersionSolver
 from idf_component_tools.build_system_tools import build_name
 from idf_component_tools.environment import getenv_bool
 from idf_component_tools.errors import (
     ComponentModifiedError,
     FetchingError,
     InvalidComponentHashError,
+    LockVersionMismatchError,
     SolverError,
 )
 from idf_component_tools.hash_tools.errors import ValidatingHashError
 from idf_component_tools.hash_tools.validate_managed_component import (
     validate_managed_component_hash,
 )
 from idf_component_tools.lock import LockManager
-from idf_component_tools.manifest import ProjectRequirements
-from idf_component_tools.manifest.solved_component import SolvedComponent
-from idf_component_tools.manifest.solved_manifest import SolvedManifest
+from idf_component_tools.manifest import SolvedComponent, SolvedManifest
 from idf_component_tools.messages import hint, warn
-from idf_component_tools.registry.api_client_errors import NetworkConnectionError
+from idf_component_tools.registry.client_errors import NetworkConnectionError
 from idf_component_tools.sources.fetcher import ComponentFetcher
+from idf_component_tools.utils import ProjectRequirements
 
 
-def check_manifests_targets(project_requirements):  # type: (ProjectRequirements) -> None
+def check_manifests_targets(project_requirements: ProjectRequirements) -> None:
     for manifest in project_requirements.manifests:
         if not manifest.targets:
             continue
 
         if project_requirements.target not in manifest.targets:
             raise FetchingError(
-                'Component "{}" does not support target {}'.format(
-                    manifest.name, project_requirements.target
-                )
+                f'Component "{manifest.real_name}" '
+                f'defined in manifest file "{manifest.path}" '
+                f'is not compatible with target "{project_requirements.target}"'
             )
 
 
 def get_unused_components(
-    unused_files_with_components, managed_components_path
-):  # type: (set[str], str) -> set[str]
+    unused_files_with_components: t.Set[str], managed_components_path: str
+) -> t.Set[str]:
     unused_components = set()
 
     for component in unused_files_with_components:
         try:
             validate_managed_component_hash(os.path.join(managed_components_path, component))
             unused_components.add(component)
         except ValidatingHashError:
             pass
 
     return unused_components
 
 
 def detect_unused_components(
-    requirement_dependencies, managed_components_path
-):  # type: (list[SolvedComponent], str) -> None
+    requirement_dependencies: t.List[SolvedComponent], managed_components_path: str
+) -> None:
     downloaded_components = os.listdir(managed_components_path)
     unused_files_with_components = set(downloaded_components) - {
         build_name(component.name) for component in requirement_dependencies
     }
     unused_components = get_unused_components(unused_files_with_components, managed_components_path)
     unused_files = unused_files_with_components - unused_components
     if unused_components:
-        print_info('Deleting {} unused components'.format(len(unused_components)))
+        print_info(f'Deleting {len(unused_components)} unused components')
         for unused_component_name in unused_components:
-            print_info(' {}'.format(unused_component_name))
+            print_info(f' {unused_component_name}')
             shutil.rmtree(os.path.join(managed_components_path, unused_component_name))
     if unused_files and not getenv_bool('IGNORE_UNKNOWN_FILES_FOR_MANAGED_COMPONENTS'):
         warning = (
             '{} unexpected files and directories were found in the "managed_components" directory:'
         )
         warning = warning.format(len(unused_files))
 
         for unexpected_name in unused_files:
-            warning += ' {}'.format(unexpected_name)
+            warning += f' {unexpected_name}'
 
         warning += (
             '\nContent of the managed components directory is managed automatically '
-            'and it\'s not recommended to place any files there manually. '
+            "and it's not recommended to place any files there manually. "
             'To suppress this warning set the environment variable: '
             'IGNORE_UNKNOWN_FILES_FOR_MANAGED_COMPONENTS=1'
         )
         warn(warning)
 
 
-def is_solve_required(project_requirements, solution):
-    # type: (ProjectRequirements, SolvedManifest) -> bool
-
+def is_solve_required(project_requirements: ProjectRequirements, solution: SolvedManifest) -> bool:
     if not solution.manifest_hash:
-        print_info('Dependencies lock doesn\'t exist, solving dependencies.')
+        print_info("Dependencies lock doesn't exist, solving dependencies.")
         return True
 
     if project_requirements.manifest_hash != solution.manifest_hash:
         print_info('Manifest files have changed, solving dependencies.')
         return True
 
     if solution.target and project_requirements.target != solution.target:
         print_info(
             'Target changed from {} to {}, solving dependencies.'.format(
                 solution.target, project_requirements.target
             )
         )
         return True
 
+    # check the dependencies are the same
+    if set(project_requirements.direct_dep_names) != set(solution.direct_dependencies or []):
+        print_info('Direct dependencies have changed, solving dependencies.')
+        return True
+
     for component in solution.dependencies:
         try:
             # For downloadable volatile dependencies, like ones from git,
             # if manifest didn't change, no need to solve
             if component.source.downloadable and component.source.volatile:
                 continue
 
             # For local components without version specified, nothing to do
             if not component.version.is_semver and component.source.volatile:
                 continue
 
             # get the same version one
             try:
                 component_versions = component.source.versions(
-                    component.name, spec='=={}'.format(component.version.semver)
+                    component.name, spec=f'=={component.version.semver}'
                 )
             except FetchingError:
-                print_warn(
-                    'Version {} of dependency {} not found, probably it was deleted, solving dependencies.'.format(
-                        component.version, component.name
-                    )
+                warn(
+                    f'Version {component.version} of dependency {component.name} not found, '
+                    'probably it was deleted, solving dependencies.'
                 )
                 return True
             except NetworkConnectionError:
                 hint(
-                    'Cannot establish a connection to the component registry. Skipping checks of dependency changes.'
+                    'Cannot establish a connection to the component registry. '
+                    'Skipping checks of dependency changes.'
                 )
                 return False
 
             component_version = component_versions.versions[0]
 
             # Handle meta components, like ESP-IDF, and volatile components, like local
             if component.source.meta or component.source.volatile:
-                if component_version != component.version:
+                if component_version.version != component.version:
                     print_info(
                         'Dependency "{}" version has changed from {} to {}, '
                         'solving dependencies.'.format(
                             component, component.version, component_version
                         )
                     )
                     return True
 
             # Should check for all types of source, but after version checking
             if component_version.component_hash != component.component_hash:
                 if component.source.volatile:
-                    print_info(
-                        'Dependency "{}" has changed, solving dependencies.'.format(component)
-                    )
+                    print_info(f'Dependency "{component}" has changed, solving dependencies.')
                     return True
                 else:
                     raise InvalidComponentHashError(
                         'The hash sum of the component "{}" does not match '
                         'the one recorded in your dependencies.lock file. '
                         'This could be due to a potential spoofing of the download server, '
                         'or your lock file may have become corrupted. '
-                        'Please review the lock file and verify the download server\'s '
-                        'authenticity to ensure the component\'s security and integrity.'.format(
+                        "Please review the lock file and verify the download server's "
+                        "authenticity to ensure the component's security and integrity.".format(
                             component
                         )
                     )
 
         except IndexError:
-            print_info('Dependency "{}" version changed, solving dependencies.'.format(component))
+            print_info(f'Dependency "{component}" version changed, solving dependencies.')
             return True
 
     return False
 
 
 def print_dot():
     print_info('.', nl=False)
 
 
 @total_ordering
 class DownloadedComponent:
-    def __init__(self, downloaded_path, targets, version):  # type: (str, list[str], str) -> None
+    def __init__(self, downloaded_path: str, targets: t.List[str], version: str) -> None:
         self.downloaded_path = downloaded_path
         self.targets = targets
         self.version = version
 
     def __hash__(self):
         return hash(self.abs_path)
 
@@ -203,23 +205,23 @@
     def __lt__(self, other):
         if not isinstance(other, DownloadedComponent):
             return NotImplemented
 
         return self.abs_path < other.abs_path
 
     @property
-    def name(self):  # type: () -> str
+    def name(self) -> str:
         return os.path.basename(self.abs_path)
 
     @property
     def abs_path(self):
         return os.path.abspath(self.downloaded_path)
 
     @property
-    def abs_posix_path(self):  # type: () -> str
+    def abs_posix_path(self) -> str:
         return Path(self.abs_path).as_posix()
 
 
 def check_for_new_component_versions(project_requirements, old_solution):
     if getenv_bool('IDF_COMPONENT_CHECK_NEW_VERSION', False):
         # Check for newer versions of components
         solver = VersionSolver(project_requirements, old_solution)
@@ -242,72 +244,79 @@
                             old_dep.name, old_dep.version, new_dep.version
                         )
                     )
 
             if updateable_components_messages:
                 hint(
                     '\nFollowing dependencies have new versions available:\n{}'
-                    '\nConsider running "idf.py update-dependencies" to update your lock file.\n'.format(
-                        '\n'.join(updateable_components_messages)
-                    )
+                    '\nConsider running "idf.py update-dependencies" to update '
+                    'your lock file.\n'.format('\n'.join(updateable_components_messages))
                 )
 
         except (SolverFailure, NetworkConnectionError):
             pass
 
 
 def download_project_dependencies(
-    project_requirements, lock_path, managed_components_path, is_idf_root_dependencies=False
-):
-    # type: (ProjectRequirements, str, str, bool) -> set[DownloadedComponent]
+    project_requirements: ProjectRequirements,
+    lock_path: str,
+    managed_components_path: str,
+    is_idf_root_dependencies: bool = False,
+) -> t.Set[DownloadedComponent]:
     """Solves dependencies and download components"""
     lock_manager = LockManager(lock_path)
-    solution = lock_manager.load()
+
+    try:
+        solution = lock_manager.load()
+    except LockVersionMismatchError as e:
+        print_notice(str(e))
+        os.remove(lock_path)
+        solution = SolvedManifest()
+
     check_manifests_targets(project_requirements)
 
     if is_solve_required(project_requirements, solution):
         solver = VersionSolver(project_requirements, solution, component_solved_callback=print_dot)
 
         try:
             solution = solver.solve()
         except SolverFailure as e:
             conflict_constraints = parse_root_dep_conflict_constraints(e)
             components_introduce_conflict = []
             for conflict_constraint in conflict_constraints:
                 for manifest in project_requirements.manifests:
-                    for dep in manifest.dependencies:
-                        for source in dep.sources:
-                            if Package(
-                                dep.name, source
-                            ) == conflict_constraint.package and dep.version_spec == str(
-                                conflict_constraint.constraint
-                            ):
-                                components_introduce_conflict.append(manifest.name)
-                                break
+                    for dep in manifest.requirements:
+                        if Package(
+                            dep.name, dep.source
+                        ) == conflict_constraint.package and dep.version_spec == str(
+                            conflict_constraint.constraint
+                        ):
+                            components_introduce_conflict.append(manifest.real_name)
+                            break
 
             if components_introduce_conflict:
                 hint(
                     'Please check manifest file of the following component(s): {}'.format(
                         ', '.join(components_introduce_conflict)
                     )
                 )
             raise SolverError(str(e))
-        print_info('Updating lock file at %s' % lock_path)
+        print_info(f'Updating lock file at {lock_path}')
         lock_manager.dump(solution)
 
     else:
         check_for_new_component_versions(
             project_requirements=project_requirements, old_solution=solution
         )
     # Download components
     downloaded_components = set()
 
     requirement_dependencies = []
     project_requirements_dependencies = [
-        manifest.name for manifest in project_requirements.manifests
+        manifest.real_name for manifest in project_requirements.manifests
     ]
 
     for component in solution.dependencies:
         component_name_with_namespace = build_name(component.name)
         component_name = component_name_with_namespace.split('__')[-1]
         if (
             component_name_with_namespace not in project_requirements_dependencies
@@ -317,22 +326,18 @@
 
     if os.path.exists(managed_components_path) and is_idf_root_dependencies is False:
         detect_unused_components(requirement_dependencies, managed_components_path)
 
     if requirement_dependencies:
         number_of_components = len(requirement_dependencies)
         changed_components = []
-        print_info('Processing {} dependencies:'.format(number_of_components))
+        print_info(f'Processing {number_of_components} dependencies:')
 
         for index, component in enumerate(requirement_dependencies):
-            print_info(
-                '[{index}/{num_components}] {component}'.format(
-                    index=index + 1, num_components=number_of_components, component=str(component)
-                )
-            )
+            print_info(f'[{index + 1}/{number_of_components}] {str(component)}')
             fetcher = ComponentFetcher(component, managed_components_path)
             try:
                 download_path = fetcher.download()
                 if download_path:
                     fetcher.create_hash(download_path, component.component_hash)
                     downloaded_components.add(
                         DownloadedComponent(
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/idf_extensions.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/idf_extensions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,72 +1,68 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import sys
+import typing as t
 import warnings
 
 from idf_component_manager.utils import CLICK_SUPPORTS_SHOW_DEFAULT, print_error, showwarning
 from idf_component_tools.errors import FatalError
 
 from .core import ComponentManager
 
-try:
-    from typing import Any, Dict, List
-except ImportError:
-    pass
-
-SERVICE_PROFILE = [
+SERVICE_PROFILE: t.List[t.Dict[str, t.Any]] = [
     {
         'names': ['--service-profile'],
         'help': 'Profile for the component registry to use. '
         'By default profile named "default" will be used.',
         'envvar': 'IDF_COMPONENT_SERVICE_PROFILE',
     },
-]  # type: List[Dict[str, Any]]
+]
 
-NAMESPACE = [
+NAMESPACE: t.List[t.Dict[str, t.Any]] = [
     {
         'names': ['--namespace'],
         'help': 'Namespace for the component. Can be set in the config file.',
         'envvar': 'IDF_COMPONENT_NAMESPACE',
     },
-]  # type: List[Dict[str, Any]]
+]
 
-NAME = [
+NAME: t.List[t.Dict[str, t.Any]] = [
     {
         'names': ['--name'],
         'help': 'Component name.',
         'required': True,
     },
-]  # type: List[Dict[str, Any]]
+]
 
 SERVICE_OPTIONS = SERVICE_PROFILE + NAMESPACE + NAME
 
-LOCAL_MANIFEST_OPTIONS = [
+LOCAL_MANIFEST_OPTIONS: t.List[t.Dict[str, t.Any]] = [
     {
         'names': ['--component'],
         'default': 'main',
         'help': 'Name of the component in the project.',
     },
     {
         'names': ['-p', '--path'],
         'help': 'Path to the component. The component name is ignored when path the is specified.',
         'default': None,
     },
-]  # type: list[dict[str, Any]]
+]
 
 if CLICK_SUPPORTS_SHOW_DEFAULT:
     LOCAL_MANIFEST_OPTIONS[0]['show_default'] = True
 
 VERSION_PARAMETER = [
     {
         'names': ['--version'],
         'help': 'Set version, if not defined in the manifest. '
         'Use "git" to get version from git tag. '
-        "The command won\'t try uploading, if running not from a git tag.",
+        "The command won't try uploading, if running not from a git tag.",
         'required': False,
     }
 ]
 
 CREATE_PROJECT_FROM_EXAMPLE_DESCR = """
 Create a project from an example.
 
@@ -146,15 +142,15 @@
             'remove_managed_components': {'callback': callback, 'hidden': True},
             'upload-component': {
                 'callback': callback,
                 'deprecated': True,
                 'help': (
                     'New CLI command: "compote component upload". '
                     'Upload component to the component registry. '
-                    'If the component doesn\'t exist in the registry '
+                    "If the component doesn't exist in the registry "
                     'it will be created automatically.'
                 ),
                 'options': SERVICE_OPTIONS
                 + VERSION_PARAMETER
                 + [
                     {
                         'names': ['--archive'],
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/prepare_components/prepare.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/prepare_components/prepare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 #!/usr/bin/env python
-# coding=utf-8
 #
 # SPDX-FileCopyrightText: 2019-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 #
 # 'prepare.py' is a tool to be used by CMake build system to prepare components
 # from package manager
 
 import argparse
 import os
 import sys
 import warnings
 
+from idf_component_manager.core import ComponentManager
 from idf_component_manager.utils import print_error, showwarning
 from idf_component_tools.errors import FatalError
 
-from ..core import ComponentManager
-
 
 def _component_list_file(build_dir):
     return os.path.join(build_dir, 'components_with_manifests_list.temp')
 
 
 def prepare_dep_dirs(args):
     build_dir = args.build_dir or os.path.dirname(args.managed_components_list_file)
@@ -106,15 +104,15 @@
             'name': 'inject_requrements',
             'extra_help': ' (alias)',
         },
     ]
 
     for step in inject_step_data:
         inject_step = subparsers.add_parser(
-            step['name'], help='Inject requirements to CMake%s' % step.get('extra_help', '')
+            step['name'], help=f"Inject requirements to CMake{step.get('extra_help', '')}"
         )
         inject_step.set_defaults(func=inject_requirements)
         inject_step.add_argument(
             '--component_requires_file',
             help='Path to temporary file with component requirements',
             required=True,
         )
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/sync.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/sync.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 # SPDX-FileCopyrightText: 2023-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 import errno
 import json
+import typing as t
 from collections import namedtuple
 from pathlib import Path
 
 from tqdm import tqdm
 
 from idf_component_manager.core_utils import parse_component
 from idf_component_manager.utils import print_info
 from idf_component_tools.build_system_tools import is_component
+from idf_component_tools.constants import MANIFEST_FILENAME
 from idf_component_tools.errors import SyncError
-from idf_component_tools.manifest import MANIFEST_FILENAME, ComponentRequirement, ManifestManager
+from idf_component_tools.manager import ManifestManager
+from idf_component_tools.manifest import ComponentRequirement
 from idf_component_tools.messages import warn
-from idf_component_tools.registry.api_client_errors import ComponentNotFound, VersionNotFound
+from idf_component_tools.registry.client_errors import ComponentNotFound, VersionNotFound
 from idf_component_tools.registry.multi_storage_client import MultiStorageClient
 from idf_component_tools.registry.request_processor import join_url
-from idf_component_tools.sources.web_service import WebServiceSource, download_archive
+from idf_component_tools.sources.web_service import download_archive
+
+ComponentVersion = namedtuple('ComponentVersion', ['version', 'file_path', 'storage_url'])
 
 
 class ComponentStaticVersions:  # Should be mutable for updating metadata
-    metadata = {}  # type: dict[str, str]
-    versions = []  # type: list[ComponentVersion]
+    metadata: t.Dict[str, str] = {}
+    versions: t.List[ComponentVersion] = []
 
     def __init__(self, metadata, versions):
         self.metadata = metadata
         self.versions = versions
 
 
-ComponentVersion = namedtuple('ComponentVersion', ['version', 'file_path', 'storage_url'])
-
-
-def dump_metadata(metadata, save_path):  # type: (dict[str, ComponentStaticVersions], Path) -> None
+def dump_metadata(metadata: t.Dict[str, ComponentStaticVersions], save_path: Path) -> None:
     for component_name, component_info in metadata.items():
         namespace, name = component_name.split('/')
         path = save_path / 'components' / namespace
         try:
             path.mkdir(parents=True)
         except OSError as e:
             if e.errno != errno.EEXIST:
                 raise e
 
-        with open(str(path / '{}.json'.format(name)), 'w') as f:
+        with open(str(path / f'{name}.json'), 'w') as f:
             json.dump(component_info.metadata, f)
 
 
-def download_dependency(version, path):  # type: (ComponentVersion, Path) -> bool
+def download_dependency(version: ComponentVersion, path: Path) -> bool:
     if version.storage_url is None:  # Local component
         return False
     filename = Path(version.file_path)
     url = join_url(version.storage_url, str(filename))
 
     try:
         path.mkdir(parents=True)
@@ -60,48 +62,46 @@
     if not (path / filename).is_file():
         download_archive(url, str(path), save_original_filename=True)
         return True
     return False
 
 
 def download_components_archives(
-    metadata, save_path
-):  # type: (dict[str, ComponentStaticVersions], Path) -> dict[str, int]
+    metadata: t.Dict[str, ComponentStaticVersions], save_path: Path
+) -> t.Dict[str, int]:
     progress_bar = tqdm(total=sum([len(x.versions) for x in metadata.values()]))
-    loading_data = {}  # type: dict[str, int]
+    loading_data: t.Dict[str, int] = {}
     for component_name, component_info in metadata.items():
         for version in component_info.versions:
-            progress_bar.set_description(
-                'Downloading {}({})'.format(component_name, version.version)
-            )
+            progress_bar.set_description(f'Downloading {component_name}({version.version})')
             status = download_dependency(version, Path(save_path))
             progress_bar.update(1)
             if status:
                 loading_data[component_name] = loading_data.get(component_name, 0) + 1
     progress_bar.close()
 
     return loading_data
 
 
-def update_component_metadata(component_metadata, api_metadata):  # type: (dict, dict) -> dict
+def update_component_metadata(component_metadata: t.Dict, api_metadata: t.Dict) -> t.Dict:
     for api_version in api_metadata['versions']:
         for i, component_version in enumerate(component_metadata['versions']):
             if component_version['version'] == api_version['version']:
                 component_metadata['versions'][i] = api_version  # Update old metadata
                 break
         else:
             component_metadata['versions'].append(api_version)
 
     api_metadata['versions'] = component_metadata['versions']  # Update header
     return api_metadata
 
 
 def update_static_versions(
-    old, new
-):  # type: (dict[str, ComponentStaticVersions], dict[str, ComponentStaticVersions]) -> dict
+    old: t.Dict[str, ComponentStaticVersions], new: t.Dict[str, ComponentStaticVersions]
+) -> t.Dict:
     result = old.copy()
     for component_name, component_info in new.items():
         if component_name not in result:
             result[component_name] = component_info
         elif result[component_name].metadata != component_info.metadata:
             result[component_name].metadata = update_component_metadata(
                 result[component_name].metadata, component_info.metadata
@@ -114,21 +114,21 @@
                 else:
                     result[component_name].versions.append(version)
 
     return result
 
 
 def get_component_metadata(
-    client,  # type: MultiStorageClient
-    requirement,  # type: ComponentRequirement
-    version_spec,  # type: str | None
-    metadata,  # type: dict
-    warnings,  # type: list[str]
-    progress_bar=None,  # type: tqdm | None
-):  # type: (...) -> tuple[dict, list[str]]
+    client: MultiStorageClient,
+    requirement: ComponentRequirement,
+    version_spec: t.Optional[str],
+    metadata: t.Dict,
+    warnings: t.List[str],
+    progress_bar: t.Optional[tqdm] = None,
+) -> t.Tuple[t.Dict, t.List[str]]:
     try:
         component_info = client.get_component_info(
             component_name=requirement.name, spec=version_spec
         )
         if not component_info.data['versions']:
             raise VersionNotFound()
     except (VersionNotFound, ComponentNotFound):
@@ -160,27 +160,27 @@
 
     metadata[requirement.name].versions = loaded_versions
 
     return metadata, warnings
 
 
 def prepare_metadata(
-    client,  # type: MultiStorageClient
-    dependencies,  # type: list[ComponentRequirement]
-    progress_bar=None,  # type: tqdm | None
-    metadata=None,  # type: dict | None
-    warnings=None,  # type: list | None
-):  # type: (...) -> tuple[dict, list[str]]
+    client: MultiStorageClient,
+    dependencies: t.List[ComponentRequirement],
+    progress_bar: t.Optional[tqdm] = None,
+    metadata: t.Optional[t.Dict] = None,
+    warnings: t.Optional[t.List] = None,
+) -> t.Tuple[t.Dict, t.List[str]]:
     if metadata is None:
         metadata = {}
     if warnings is None:
         warnings = []
 
     for requirement in dependencies:
-        if requirement.source.name == 'service':
+        if requirement.source.type == 'service':
             version_specs = []
             if requirement.optional_requirement and requirement.optional_requirement.matches:
                 version_specs = [elem.version for elem in requirement.optional_requirement.matches]
 
             if not version_specs:
                 version_specs = [requirement.version_spec]
 
@@ -188,108 +188,104 @@
                 metadata, warnings = get_component_metadata(
                     client, requirement, version_spec, metadata, warnings, progress_bar
                 )
 
     return metadata, warnings
 
 
-def load_saved_metadata(path):  # type: (Path) -> dict[str, ComponentStaticVersions]
+def load_saved_metadata(path: Path) -> t.Dict[str, ComponentStaticVersions]:
     components_json_path = path / 'components'
     metadata = {}
     for json_filename in components_json_path.rglob('*.json'):
-        component_name = '{}/{}'.format(json_filename.parent.name, json_filename.stem)
+        component_name = f'{json_filename.parent.name}/{json_filename.stem}'
         versions = []
         try:
             with open(str(json_filename)) as f:
                 loaded_component_metadata = json.load(f)
             for version in loaded_component_metadata['versions']:
                 versions.append(ComponentVersion(version['version'], version['url'], None))
         except (ValueError, KeyError):
             raise SyncError('Metadata file is not valid')
 
         metadata[component_name] = ComponentStaticVersions(loaded_component_metadata, versions)
     return metadata
 
 
 def collect_metadata(
-    client,  # type: MultiStorageClient
-    path,  # type: str | Path
-    namespace,  # type: str
-    save_path,  # type: str | Path
-    components=None,  # type: list[str] | None
-    recursive=False,  # type: bool
-):  # type: (...) -> dict[str, ComponentStaticVersions]
-    metadata = {}  # type: dict[str, ComponentStaticVersions]
+    client: MultiStorageClient,
+    path: t.Union[str, Path],
+    components: t.Optional[t.List[str]] = None,
+    recursive: bool = False,
+) -> t.Dict[str, ComponentStaticVersions]:
+    metadata: t.Dict[str, ComponentStaticVersions] = {}
     path = Path(path)
-    warnings = []  # type: list[str]
+    warnings: t.List[str] = []
     progress_bar = tqdm(
         total=10000,
         desc='Metadata downloaded from the registry',
         bar_format='{desc}: {n_fmt}',
     )  # We don't show total, so we can set total as any big number
     if components:
         dependencies = []
         for component_info in components:
-            component_name, spec = parse_component(component_info, namespace)
+            component_name, spec = parse_component(component_info, client.default_namespace)
             dependencies.append(
                 ComponentRequirement(
-                    component_name, version_spec=spec, sources=[WebServiceSource({})]
+                    name=component_name,
+                    version=spec,
                 )
             )
         metadata, warnings = prepare_metadata(
             client, dependencies, progress_bar, metadata, warnings
         )
     else:
         paths = [path]
         if recursive:
             paths = list(path.glob('**'))
         for path in paths:
             if path.is_dir() and is_component(path) and (path / MANIFEST_FILENAME).exists():
-                manifest = ManifestManager(
-                    str(path), '', expand_environment=True, process_opt_deps=True
-                ).load()
+                manifest = ManifestManager(str(path), '').load()
                 metadata, warnings = prepare_metadata(
-                    client, manifest.dependencies, progress_bar, metadata, warnings
+                    client, manifest.requirements, progress_bar, metadata, warnings
                 )
     progress_bar.close()
 
     for warning in warnings:
         warn(warning)
 
     return metadata
 
 
-def metadata_has_changes(old, new):  # type: (dict, dict) -> bool
+def metadata_has_changes(old: t.Dict, new: t.Dict) -> bool:
     if not all(
         x in old['versions'] for x in new['versions']
     ):  # In old metadata may be more versions than in new
         return True
 
     old_without_version = {k: v for k, v in old.items() if k != 'versions'}
     new_without_version = {k: v for k, v in new.items() if k != 'versions'}
     if old_without_version != new_without_version:
         return True
     return False
 
 
 def sync_components(
-    client,  # type: MultiStorageClient
-    path,  # type: str | Path
-    namespace,  # type: str
-    save_path,  # type: Path
-    components=None,  # type: list[str] | None
-    recursive=False,  # type: bool
-):  # type: (...) -> None
+    client: MultiStorageClient,
+    path: t.Union[str, Path],
+    save_path: Path,
+    components: t.Optional[t.List[str]] = None,
+    recursive: bool = False,
+) -> None:
     save_path = Path(save_path)
-    print_info('Collecting metadata files into the folder "{}"'.format(save_path.absolute()))
+    print_info(f'Collecting metadata files into the folder "{save_path.absolute()}"')
 
     metadata = load_saved_metadata(Path(save_path))
-    print_info('{} metadata loaded from "{}" folder'.format(len(metadata), save_path))
+    print_info(f'{len(metadata)} metadata loaded from "{save_path}" folder')
 
-    new_metadata = collect_metadata(client, path, namespace, save_path, components, recursive)
+    new_metadata = collect_metadata(client, path, components, recursive)
     if not len(new_metadata):
         raise SyncError('No components found for those requirements')
 
     if metadata.keys() == new_metadata.keys():
         for component_name in metadata.keys():
             if metadata_has_changes(
                 metadata[component_name].metadata, new_metadata[component_name].metadata
@@ -297,15 +293,15 @@
                 break
         else:
             print_info('The new metadata is identical to the loaded one. Nothing to update')
             return
 
     print_info('Updating metadata')
     metadata = update_static_versions(metadata, new_metadata)
-    print_info('Collected {} components. Downloading archives'.format(len(metadata)))
+    print_info(f'Collected {len(metadata)} components. Downloading archives')
 
     loading_data = download_components_archives(metadata, save_path)
 
     dump_metadata(metadata, save_path)
 
     total_versions = sum(list(loading_data.values()))
     if total_versions:
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/templates/idf_component_template.yml` & `idf_component_manager-2.0.0.dev0/idf_component_manager/templates/idf_component_template.yml`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.5.2/idf_component_manager/utils.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/sources/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,125 +1,140 @@
 # SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
-import enum
-import re
+import os
+import typing as t
+from abc import abstractmethod
 
-import click
-from packaging import version
+from idf_component_tools.errors import FetchingError
+from idf_component_tools.file_cache import FileCache
+from idf_component_tools.semver import SimpleSpec
+from idf_component_tools.utils import BaseModel, ComponentWithVersions, Literal
 
-from idf_component_tools.messages import UserHint, UserNotice
+if t.TYPE_CHECKING:
+    from idf_component_tools.manifest import SolvedComponent
 
-CLICK_SUPPORTS_SHOW_DEFAULT = version.parse(click.__version__) >= version.parse('7.1.0')
 
+class BaseSource(BaseModel):
+    type: Literal['base'] = 'base'  # type: ignore
 
-def print_prefixed(
-    prefix, color, message, stderr
-):  # type: (str, str, Exception | str, bool) -> None
-    styled_prefix = click.style('{}: '.format(prefix), fg=color)
-    click.echo(styled_prefix + str(message), err=stderr)
+    _hash_key = None
 
+    def __init__(
+        self,
+        system_cache_path: t.Optional[str] = None,
+        **kwargs,
+    ) -> None:
+        super().__init__(**kwargs)
 
-def print_stderr_prefixed(prefix, color, message):  # type: (str, str, Exception | str) -> None
-    print_prefixed(prefix, color, message, stderr=True)
+        self._hash_key = None
 
+        self._system_cache_path = (
+            FileCache().path() if system_cache_path is None else system_cache_path
+        )
 
-def print_error(message):  # type: (Exception | str) -> None
-    print_stderr_prefixed('ERROR', 'red', message)
+    @property
+    def system_cache_path(self):
+        return self._system_cache_path
 
+    def cache_path(self):  # type: () -> str
+        path = os.path.join(self._system_cache_path, '{}_{}'.format(self.type, self.hash_key[:8]))
+        return path
 
-def print_warn(message):  # type: (Exception | str) -> None
-    print_stderr_prefixed('WARNING', 'yellow', message)
+    def _hash_values(self):
+        return self.type, self.hash_key
 
-
-def print_hint(message):  # type: (Exception | str) -> None
-    print_prefixed('HINT', 'yellow', message, stderr=False)
-
-
-def print_notice(message):  # type: (Exception | str) -> None
-    print_prefixed('NOTICE', 'green', message, stderr=False)
-
-
-def showwarning(message, category, filename, lineno, file=None, line=None):
-    if category is UserHint:
-        print_hint(message)
-    elif category is UserNotice:
-        print_notice(message)
-    else:
-        print_warn(message)
-
-
-def print_info(
-    message,  # type: str
-    fg=None,  # type: str | None
-    bg=None,  # type: str | None
-    bold=None,  # type: str | None
-    underline=None,  # type: str | None
-    blink=None,  # type: str | None
-    **kwargs
-):  # type: (...) -> None
-    click.secho(message, fg=fg, bg=bg, bold=bold, underline=underline, blink=blink, **kwargs)
-
-
-RE_PATTERN = type(re.compile(''))  # this is a workaround for `re.Pattern` for python<3.7
-
-
-# total_ordering will raise an error in python 2.7 with enum34
-#   ValueError: must define at least one ordering operation: < > <= >=
-# The reason is that the `dir()` behavior is different,
-# ___eq__, __lt__, __hash__ are not in the dir() result.
-# define all six operators here
-class ComponentSource(str, enum.Enum):
-    # These double-quotes are coming from the build system
-    IDF_COMPONENTS = '"idf_components"'
-    PROJECT_MANAGED_COMPONENTS = '"project_managed_components"'
-    PROJECT_EXTRA_COMPONENTS = '"project_extra_components"'
-    PROJECT_COMPONENTS = '"project_components"'
-
-    # the lower value is, the lower priority it is
-    @classmethod
-    def order(cls):
-        return {
-            cls.IDF_COMPONENTS: 0,
-            cls.PROJECT_MANAGED_COMPONENTS: 1,
-            cls.PROJECT_EXTRA_COMPONENTS: 2,
-            cls.PROJECT_COMPONENTS: 3,
-        }
-
-    def __hash__(self):
-        return hash(self.value)
-
-    def __eq__(self, other):
-        if not isinstance(other, ComponentSource):
-            return NotImplemented
-
-        return self.value == other.value
-
-    def __ne__(self, other):
-        if not isinstance(other, ComponentSource):
-            return NotImplemented
-
-        return self.value != other.value
-
-    def __lt__(self, other):
-        if not isinstance(other, ComponentSource):
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, BaseSource):
             return NotImplemented
 
-        return self.order()[self] < self.order()[other]
+        return self._hash_values() == other._hash_values() and self.name == other.name
 
-    def __le__(self, other):
-        if not isinstance(other, ComponentSource):
-            return NotImplemented
-
-        return self < other or self == other
-
-    def __gt__(self, other):
-        if not isinstance(other, ComponentSource):
-            return NotImplemented
-
-        return not self <= other
+    def __hash__(self):
+        return hash(self._hash_values())
 
-    def __ge__(self, other):
-        if not isinstance(other, ComponentSource):
-            return NotImplemented
+    def __repr__(self) -> str:
+        return f'{type(self).__name__}({self.hash_key})'
 
-        return not self < other
+    @property
+    def is_overrider(self):
+        return False
+
+    @property
+    def name(self):
+        return self.type
+
+    @property
+    def hash_key(self) -> str:
+        """Hash key is used for comparison sources initialised with different settings"""
+        return self.type
+
+    @property
+    def component_hash_required(self) -> bool:
+        """Returns True if component's hash have to present and be validated"""
+        return False
+
+    @property
+    def downloadable(self) -> bool:
+        """Returns True if components have to be fetched"""
+        return False
+
+    @property
+    def meta(self) -> bool:
+        """
+        Returns True for meta components.
+        Meta components are not included in the build directly
+        """
+        return False
+
+    @property
+    def volatile(self) -> bool:
+        """
+        Returns True for volatile components.
+        Volatile components may change their content, even if their version stays the same.
+        """
+        return False
+
+    def normalized_name(self, name: str) -> str:
+        return name
+
+    def up_to_date(self, component: 'SolvedComponent', path: str) -> bool:
+        from idf_component_tools.hash_tools.validate_managed_component import (  # avoid circular import
+            validate_managed_component_by_manifest,
+        )
+
+        if self.component_hash_required and not component.component_hash:
+            raise FetchingError('Cannot install component with unknown hash')
+
+        if self.downloadable:
+            if not os.path.isdir(path):
+                return False
+
+            if component.component_hash:
+                return validate_managed_component_by_manifest(path, component.component_hash)
+
+        return True
+
+    def validate_version_spec(self, spec: str) -> bool:
+        if not spec or spec == '*':
+            return True
+
+        try:
+            return bool(SimpleSpec(spec))
+        except ValueError:
+            return False
+
+    def normalize_spec(self, spec: str) -> str:
+        return spec or '*'
+
+    @abstractmethod
+    def versions(
+        self, name: str, spec: str = '*', target: t.Optional[str] = None
+    ) -> ComponentWithVersions:
+        """List of versions for given spec"""
+
+    @abstractmethod
+    def download(self, component: 'SolvedComponent', download_path: str) -> t.Optional[str]:
+        """
+        Fetch required component version from the source
+        Returns list of absolute paths to directories with component on local filesystem
+        """
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/helper.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,25 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
-from idf_component_tools.manifest import HashedComponentVersion
-
-from .mixology.failure import SolverFailure
-
-try:
-    from typing import Any, Dict, List, Optional
-    from typing import Union as _Union
-except ImportError:
-    pass
+import typing as t
 
 from idf_component_tools.semver import Range as SemverRange
 from idf_component_tools.semver import SimpleSpec
+from idf_component_tools.utils import HashedComponentVersion
 
 from .mixology.constraint import Constraint
+from .mixology.failure import SolverFailure
 from .mixology.package import Package
 from .mixology.package_source import PackageSource as BasePackageSource
 from .mixology.range import Range
 from .mixology.union import Union
 
 
-def parse_constraint(spec):  # type: (str) -> _Union[Union, Range]
+def parse_constraint(spec: str) -> t.Union[Union, Range]:
     try:
         clause = SimpleSpec(spec).clause
     except ValueError:  # if not semspec, expect an exact version
         constraint = parse_single_constraint(HashedComponentVersion(spec))
     else:
         if isinstance(clause, SemverRange):  # single range
             constraint = parse_single_constraint(clause)
@@ -35,16 +29,16 @@
             for r in ranges[1:]:
                 constraint = constraint.intersect(r)
 
     return constraint
 
 
 def parse_single_constraint(
-    _range,
-):  # type: (_Union[SemverRange, HashedComponentVersion]) -> _Union[Union, Range]
+    _range: t.Union[SemverRange, HashedComponentVersion],
+) -> t.Union[Union, Range]:
     if isinstance(_range, HashedComponentVersion):  # not semver
         return Range(_range, _range, True, True, _range.text)
 
     version = HashedComponentVersion(str(_range.target))
     if _range.operator == _range.OP_LT:
         return Range(max=version, string=str(_range))
     elif _range.operator == _range.OP_LTE:
@@ -55,47 +49,50 @@
         return Range(min=version, include_min=True, string=str(_range))
     elif _range.operator == _range.OP_NEQ:
         return Union(Range(min=version, string=str(_range)), Range(max=version, string=str(_range)))
     else:
         return Range(version, version, True, True, str(_range))
 
 
-def parse_root_dep_conflict_constraints(failure):  # type: (SolverFailure) -> list[Constraint]
+def parse_root_dep_conflict_constraints(failure: SolverFailure) -> t.List[Constraint]:
     terms = failure._incompatibility.terms
     res = []
     if len(terms) == 1 and terms[0].package == Package.root():  # root dep
         conflict_terms = failure._incompatibility.cause.conflict.terms
         for conflict_term in conflict_terms:
             res.append(conflict_term.constraint)
 
     return res
 
 
 class Dependency:
-    def __init__(self, package, spec):  # type: (Package, str) -> None
+    def __init__(self, package: Package, spec: str) -> None:
         self.package = package
         self.constraint = parse_constraint(spec)
         self.text = spec
 
 
 class PackageSource(BasePackageSource):
-    def __init__(self):  # type: () -> None
+    def __init__(self) -> None:
         self._root_version = HashedComponentVersion('0.0.0')
-        self._root_dependencies = []  # type: List[Dependency]
-        self._packages = {}  # type: Dict[Package, Dict[HashedComponentVersion, List[Dependency]]]
+        self._root_dependencies: t.List[Dependency] = []
+        self._packages: t.Dict[Package, t.Dict[HashedComponentVersion, t.List[Dependency]]] = {}
 
-        super(PackageSource, self).__init__()
+        super().__init__()
 
     @property
     def root_version(self):
         return self._root_version
 
     def add(
-        self, package, version, deps=None
-    ):  # type:(Package, _Union[str, HashedComponentVersion],  Optional[Dict[Package, str]]) -> None
+        self,
+        package: Package,
+        version: t.Union[str, HashedComponentVersion],
+        deps: t.Optional[t.Dict[Package, str]] = None,
+    ):
         if deps is None:
             deps = {}
 
         if not isinstance(version, HashedComponentVersion):
             version = HashedComponentVersion(version)
 
         if package not in self._packages:
@@ -109,53 +106,53 @@
             if dep_package.source:
                 spec = dep_package.source.normalize_spec(spec)
 
             dependencies.append(Dependency(dep_package, spec))
 
         self._packages[package][version] = dependencies
 
-    def override_dependencies(self, overriders):  # type: (set[str]) -> None
+    def override_dependencies(self, overriders: t.Set[str]) -> None:
         for package in list(self._packages.keys()):
             if not package.source.is_overrider and package.name in overriders:
                 del self._packages[package]
 
         for package in self._packages.keys():
             for version in self._packages[package].keys():
                 self._packages[package][version] = [
                     elem
                     for elem in self._packages[package][version]
                     if elem.package.source.is_overrider or elem.package.name not in overriders
                 ]
 
-    def root_dep(self, package, spec):  # type: (Package, str) -> None
+    def root_dep(self, package: Package, spec: str) -> None:
         if package.source:
             spec = package.source.normalize_spec(spec)
 
         self._root_dependencies.append(Dependency(package, spec))
 
     def _versions_for(
-        self, package, constraint=None
-    ):  # type: (Package, Any) -> List[HashedComponentVersion]
+        self, package: Package, constraint: t.Any = None
+    ) -> t.List[HashedComponentVersion]:
         if package not in self._packages:
             return []
 
         versions = []
         for version in self._packages[package].keys():
             if not constraint or constraint.allows_any(Range(version, version, True, True)):
                 versions.append(version)
 
         return sorted(versions, reverse=True)
 
-    def dependencies_for(self, package, version):  # type: (Package, Any) -> List[Any]
+    def dependencies_for(self, package: Package, version: t.Any) -> t.List[t.Any]:
         if package == self.root:
             return self._root_dependencies
 
         return self._packages[package][version]
 
-    def convert_dependency(self, dependency):  # type: (Dependency) -> Constraint
+    def convert_dependency(self, dependency: Dependency) -> Constraint:
         if isinstance(dependency.constraint, Range):
             constraint = Range(
                 dependency.constraint.min,
                 dependency.constraint.max,
                 dependency.constraint.include_min,
                 dependency.constraint.include_max,
                 dependency.text,
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/assignment.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/assignment.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,70 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2018 Sébastien Eustace
 # SPDX-License-Identifier: MIT License
-# SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileContributor: 2022-2024 Espressif Systems (Shanghai) CO LTD
 
-try:
-    from typing import Any, Optional
-except ImportError:
-    pass
+from __future__ import annotations
+
+import typing as t
 
 from .constraint import Constraint
 from .incompatibility import Incompatibility
 from .package import Package
 from .range import Range
 from .term import Term
 
 
 class Assignment(Term):
     """
     A term in a PartialSolution that tracks some additional metadata.
     """
 
     def __init__(
-        self, constraint, is_positive, decision_level, index, cause=None
-    ):  # type: (Constraint, bool, int, int, Optional[Incompatibility]) -> None
-        super(Assignment, self).__init__(constraint, is_positive)
+        self,
+        constraint: Constraint,
+        is_positive: bool,
+        decision_level: int,
+        index: int,
+        cause: t.Optional[Incompatibility] = None,
+    ) -> None:
+        super().__init__(constraint, is_positive)
 
         self._decision_level = decision_level
         self._index = index
         self._cause = cause
 
     @property
-    def decision_level(self):  # type: () -> int
+    def decision_level(self) -> int:
         return self._decision_level
 
     @property
-    def index(self):  # type: () -> int
+    def index(self) -> int:
         return self._index
 
     @property
-    def cause(self):  # type: () -> Incompatibility
+    def cause(self) -> Incompatibility:
         return self._cause
 
     @classmethod
     def decision(
-        cls, package, version, decision_level, index
-    ):  # type: (Package, Any, int, int) -> Assignment
+        cls, package: Package, version: t.Any, decision_level: int, index: int
+    ) -> Assignment:
         return cls(
             Constraint(package, Range(version, version, True, True)),
             True,
             decision_level,
             index,
         )
 
     @classmethod
     def derivation(
-        cls, constraint, is_positive, cause, decision_level, index
-    ):  # type: (Constraint, bool, Incompatibility, int, int) -> Assignment
+        cls,
+        constraint: Constraint,
+        is_positive: bool,
+        cause: Incompatibility,
+        decision_level: int,
+        index: int,
+    ) -> Assignment:
         return cls(constraint, is_positive, decision_level, index, cause)
 
-    def is_decision(self):  # type: () -> bool
+    def is_decision(self) -> bool:
         return self._cause is None
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/constraint.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/constraint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,111 +1,108 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2018 Sébastien Eustace
 # SPDX-License-Identifier: MIT License
-# SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileContributor: 2022-2024 Espressif Systems (Shanghai) CO LTD
+from __future__ import annotations
 
-try:
-    from typing import Union as _Union
-except ImportError:
-    pass
+import typing as t
 
 from .package import Package
 from .range import Range
 from .set_relation import SetRelation
 from .union import Union
 
 
-class Constraint(object):
+class Constraint:
     """
     A term constraint.
     """
 
-    def __init__(self, package, constraint):  # type: (Package, _Union[Range, Union]) -> None
+    def __init__(self, package: Package, constraint: t.Union[Range, Union]) -> None:
         self._package = package
         self._constraint = constraint
 
     @property
-    def package(self):  # type: () -> Package
+    def package(self) -> Package:
         return self._package
 
     @property
-    def constraint(self):  # type: () -> _Union[Range, Union]
+    def constraint(self) -> t.Union[Range, Union]:
         return self._constraint
 
     @property
-    def inverse(self):  # type: () -> Constraint
+    def inverse(self) -> Constraint:
         new_constraint = self.constraint.inverse
 
         return self.__class__(self.package, new_constraint)
 
-    def allows_all(self, other):  # type: (Constraint) -> bool
+    def allows_all(self, other: Constraint) -> bool:
         return self.constraint.allows_all(other.constraint)
 
-    def allows_any(self, other):  # type: (Constraint) -> bool
+    def allows_any(self, other: Constraint) -> bool:
         return self.constraint.allows_any(other.constraint)
 
-    def difference(self, other):  # type: (Constraint) -> Constraint
+    def difference(self, other: Constraint) -> bool:
         if not isinstance(self.package.source, type(other.package.source)):
             raise ValueError('Cannot tell difference of two different source types')
 
         return self.__class__(self.package, self.constraint.difference(other.constraint))
 
-    def intersect(self, other):  # type: (Constraint) -> Constraint
+    def intersect(self, other: Constraint) -> Constraint:
         if other.package != self.package:
             raise ValueError('Cannot intersect two constraints for different packages')
 
         if not isinstance(self.package.source, type(other.package.source)):
             raise ValueError('Cannot intersect two different source types')
 
         return self.__class__(self.package, self.constraint.intersect(other.constraint))
 
-    def union(self, other):  # type: (Constraint) -> Constraint
+    def union(self, other: Constraint) -> Constraint:
         if other.package != self.package:
             raise ValueError('Cannot build an union of two constraints for different packages')
 
         if not isinstance(self.package.source, type(other.package.source)):
             raise ValueError('Cannot build an union of two different source types')
 
         return self.__class__(self.package, self.constraint.union(other.constraint))
 
-    def is_subset_of(self, other):  # type: (Constraint) -> bool
+    def is_subset_of(self, other: Constraint) -> bool:
         return other.allows_all(self)
 
-    def overlaps(self, other):  # type: (Constraint) -> bool
+    def overlaps(self, other: Constraint) -> bool:
         return other.allows_any(self)
 
-    def is_disjoint_from(self, other):  # type: (Constraint) -> bool
+    def is_disjoint_from(self, other: Constraint) -> bool:
         return not self.overlaps(other)
 
-    def relation(self, other):  # type: (Constraint) -> SetRelation
+    def relation(self, other: Constraint) -> SetRelation:
         if self.is_subset_of(other):
             return SetRelation.SUBSET
         elif self.overlaps(other):
             return SetRelation.OVERLAPPING
         else:
             return SetRelation.DISJOINT
 
-    def is_any(self):  # type: () -> bool
+    def is_any(self) -> bool:
         return self._constraint.is_any()
 
-    def is_empty(self):  # type: () -> bool
+    def is_empty(self) -> bool:
         return self._constraint.is_empty()
 
-    def __eq__(self, other):  # type: (Constraint) -> bool
+    def __eq__(self, other: Constraint) -> bool:
         if not isinstance(other, Constraint):
             return NotImplemented
 
         return other.package == self.package and other.constraint == self.constraint
 
     def __hash__(self):
         return hash(self.package) ^ hash(self.constraint)
 
-    def to_string(self, allow_every=False):  # type: (bool) -> str
+    def to_string(self, allow_every: bool = False) -> str:
         if self.package == Package.root():
             return 'project'
         elif allow_every and self.is_any():
-            return 'every version of {}'.format(self.package)
+            return f'every version of {self.package}'
 
         return '{} ({})'.format(self.package, '*' if self.is_any() else str(self.constraint))
 
     def __str__(self):
         return self.to_string()
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/failure.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/failure.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,51 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2018 Sébastien Eustace
 # SPDX-License-Identifier: MIT License
-# SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileContributor: 2022-2024 Espressif Systems (Shanghai) CO LTD
 
-try:
-    from typing import Dict, List, Tuple
-except ImportError:
-    pass
+import typing as t
 
 from .incompatibility import Incompatibility
 from .incompatibility_cause import ConflictCause
 
 
 class SolverFailure(Exception):
-    def __init__(self, incompatibility):  # type: (Incompatibility) -> None
+    def __init__(self, incompatibility: Incompatibility) -> None:
         self._incompatibility = incompatibility
 
     @property
     def message(self):
         return str(self)
 
     def __str__(self):
         return _Writer(self._incompatibility).write()
 
 
 class _Writer:
-    def __init__(self, root):  # type: (Incompatibility) -> None
+    def __init__(self, root: Incompatibility) -> None:
         self._root = root
-        self._derivations = {}  # type: Dict[Incompatibility, int]
-        self._lines = []  # type: List[Tuple[str, int]]
-        self._line_numbers = {}  # type: Dict[Incompatibility, int]
+        self._derivations: t.Dict[Incompatibility, int] = {}
+        self._lines: t.List[t.Tuple[str, int]] = []
+        self._line_numbers: t.Dict[Incompatibility, int] = {}
 
         self._count_derivations(self._root)
 
     def write(self):
         buffer = []
 
         required_python_version = None
 
         if required_python_version is not None:
-            buffer.append(
-                'The current supported Python versions are {}'.format(required_python_version)
-            )
+            buffer.append(f'The current supported Python versions are {required_python_version}')
             buffer.append('')
 
         if isinstance(self._root.cause, ConflictCause):
             self._visit(self._root, {})
         else:
-            self._write(self._root, 'Because {}, version solving failed.'.format(self._root))
+            self._write(self._root, f'Because {self._root}, version solving failed.')
 
         padding = (
             0
             if not self._line_numbers
             else len('({}) '.format(list(self._line_numbers.values())[-1]))
         )
 
@@ -74,31 +68,34 @@
                 message = ' ' * padding + message
 
             buffer.append(message)
 
         return '\n'.join(buffer)
 
     def _write(
-        self, incompatibility, message, numbered=False
-    ):  # type: (Incompatibility, str, bool) -> None
+        self, incompatibility: Incompatibility, message: str, numbered: bool = False
+    ) -> None:
         if numbered:
             number = len(self._line_numbers) + 1
             self._line_numbers[incompatibility] = number
             self._lines.append((message, number))
         else:
             self._lines.append((message, None))
 
     def _visit(
-        self, incompatibility, details_for_incompatibility, conclusion=False
-    ):  # type: (Incompatibility, Dict, bool) -> None
+        self,
+        incompatibility: Incompatibility,
+        details_for_incompatibility: t.Dict,
+        conclusion: bool = False,
+    ) -> None:
         numbered = conclusion or self._derivations[incompatibility] > 1
         conjunction = 'So,' if conclusion or incompatibility == self._root else 'And'
         incompatibility_string = str(incompatibility)
 
-        cause = incompatibility.cause  # type: ConflictCause
+        cause: ConflictCause = incompatibility.cause
         details_for_cause = {}
         if isinstance(cause.conflict.cause, ConflictCause) and isinstance(
             cause.other.cause, ConflictCause
         ):
             conflict_line = self._line_numbers.get(cause.conflict)
             other_line = self._line_numbers.get(cause.other)
 
@@ -138,15 +135,15 @@
                 if single_line_other or single_line_conflict:
                     first = cause.conflict if single_line_other else cause.other
                     second = cause.other if single_line_other else cause.conflict
                     self._visit(first, details_for_cause)
                     self._visit(second, details_for_cause)
                     self._write(
                         incompatibility,
-                        'Thus, {}.'.format(incompatibility_string),
+                        f'Thus, {incompatibility_string}.',
                         numbered=numbered,
                     )
                 else:
                     self._visit(cause.conflict, {}, conclusion=True)
                     self._lines.append(('', None))
 
                     self._visit(cause.other, details_for_cause)
@@ -176,15 +173,15 @@
                     'Because {}, {}.'.format(
                         ext.and_to_string(derived, details_for_cause, None, derived_line),
                         incompatibility_string,
                     ),
                     numbered=numbered,
                 )
             elif self._is_collapsible(derived):
-                derived_cause = derived.cause  # type: ConflictCause
+                derived_cause: ConflictCause = derived.cause
                 if isinstance(derived_cause.conflict.cause, ConflictCause):
                     collapsed_derived = derived_cause.conflict
                 else:
                     collapsed_derived = derived_cause.other
 
                 if isinstance(derived_cause.conflict.cause, ConflictCause):
                     collapsed_ext = derived_cause.other
@@ -203,52 +200,52 @@
                     ),
                     numbered=numbered,
                 )
             else:
                 self._visit(derived, details_for_cause)
                 self._write(
                     incompatibility,
-                    '{} because {}, {}.'.format(conjunction, str(ext), incompatibility_string),
+                    f'{conjunction} because {str(ext)}, {incompatibility_string}.',
                     numbered=numbered,
                 )
         else:
             self._write(
                 incompatibility,
                 'Because {}, {}.'.format(
                     cause.conflict.and_to_string(cause.other, details_for_cause, None, None),
                     incompatibility_string,
                 ),
                 numbered=numbered,
             )
 
-    def _is_collapsible(self, incompatibility):  # type: (Incompatibility) -> bool
+    def _is_collapsible(self, incompatibility: Incompatibility) -> bool:
         if self._derivations[incompatibility] > 1:
             return False
 
-        cause = incompatibility.cause  # type: ConflictCause
+        cause: ConflictCause = incompatibility.cause
         if isinstance(cause.conflict.cause, ConflictCause) and isinstance(
             cause.other.cause, ConflictCause
         ):
             return False
 
         if not isinstance(cause.conflict.cause, ConflictCause) and not isinstance(
             cause.other.cause, ConflictCause
         ):
             return False
 
         complex = cause.conflict if isinstance(cause.conflict.cause, ConflictCause) else cause.other
 
         return complex not in self._line_numbers
 
-    def _is_single_line(self, cause):  # type: (ConflictCause) -> bool
+    def _is_single_line(self, cause: ConflictCause) -> bool:
         return not isinstance(cause.conflict.cause, ConflictCause) and not isinstance(
             cause.other.cause, ConflictCause
         )
 
-    def _count_derivations(self, incompatibility):  # type: (Incompatibility) -> None
+    def _count_derivations(self, incompatibility: Incompatibility) -> None:
         if incompatibility in self._derivations:
             self._derivations[incompatibility] += 1
         else:
             self._derivations[incompatibility] = 1
             cause = incompatibility.cause
             if isinstance(cause, ConflictCause):
                 self._count_derivations(cause.conflict)
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/incompatibility.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/incompatibility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2018 Sébastien Eustace
 # SPDX-License-Identifier: MIT License
-# SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileContributor: 2022-2024 Espressif Systems (Shanghai) CO LTD
+from __future__ import annotations
 
-try:
-    from typing import Dict, Generator, Hashable, List, Optional
-except ImportError:
-    pass
+import typing as t
 
 from .incompatibility_cause import (
     ConflictCause,
     DependencyCause,
     IncompatibilityCause,
     NoVersionsCause,
     PackageNotFoundCause,
@@ -18,15 +15,15 @@
     SelfDependentCause,
 )
 from .package import Package
 from .term import Term
 
 
 class Incompatibility:
-    def __init__(self, terms, cause):  # type: (List[Term], IncompatibilityCause) -> None
+    def __init__(self, terms: t.List[Term], cause: IncompatibilityCause) -> None:
         # Remove the root package from generated incompatibilities, since it will
         # always be satisfied. This makes error reporting clearer, and may also
         # make solving more efficient.
         if (
             len(terms) != 1
             and isinstance(cause, ConflictCause)
             and any([term.is_positive() and term.package != Package.root() for term in terms])
@@ -44,15 +41,15 @@
         ):
             pass
         elif isinstance(cause, SelfDependentCause):
             # If one package depends on itself, don't coalesce these two terms.
             terms = terms
         else:
             # Coalesce multiple terms about the same package if possible.
-            by_name = {}  # type: Dict[Hashable, Dict[Hashable, Term]]
+            by_name: t.Dict[t.Hashable, t.Dict[t.Hashable, Term]] = {}
             for term in terms:
                 if term.package not in by_name:
                     by_name[term.package] = {}
 
                 by_ref = by_name[term.package]
                 ref = term.package
 
@@ -79,45 +76,43 @@
 
                 terms = new_terms
 
         self._terms = terms
         self._cause = cause
 
     @property
-    def terms(self):  # type: () -> List[Term]
+    def terms(self) -> t.List[Term]:
         return self._terms
 
     @property
-    def cause(self):  # type: () -> ConflictCause
+    def cause(self) -> ConflictCause:
         return self._cause
 
     @property
-    def external_incompatibilities(self):  # type: () -> Generator[Incompatibility]
+    def external_incompatibilities(self) -> t.Generator[Incompatibility]:
         """
         Returns all external incompatibilities in this incompatibility's
         derivation graph.
         """
         if isinstance(self._cause, ConflictCause):
-            cause = self._cause  # type: ConflictCause
-            for incompatibility in cause.conflict.external_incompatibilities:
-                yield incompatibility
+            cause: ConflictCause = self._cause
+            yield from cause.conflict.external_incompatibilities
 
-            for incompatibility in cause.other.external_incompatibilities:
-                yield incompatibility
+            yield from cause.other.external_incompatibilities
         else:
             yield self
 
-    def is_failure(self):  # type: () -> bool
+    def is_failure(self) -> bool:
         return len(self._terms) == 0 or (
             len(self._terms) == 1
             and self._terms[0].package == Package.root()
             and self._terms[0].is_positive()
         )
 
-    def handle_cause(self):  # type: () -> Optional[str]
+    def handle_cause(self) -> t.Optional[str]:
         if isinstance(self._cause, (DependencyCause, SelfDependentCause)):
             assert len(self._terms) == 2
 
             depender = self._terms[0]
             dependee = self._terms[1]
             assert depender.is_positive()
             assert not dependee.is_positive()
@@ -137,21 +132,21 @@
             return 'no versions of {} match {}'.format(
                 self._terms[0].package, self._terms[0].constraint.constraint
             )
         elif isinstance(self._cause, PackageNotFoundCause):
             assert len(self._terms) == 1
             assert self._terms[0].is_positive()
 
-            return "{} doesn't exist".format(self._terms[0].package)
+            return f"{self._terms[0].package} doesn't exist"
         elif isinstance(self._cause, RootCause):
             assert len(self._terms) == 1
             assert not self._terms[0].is_positive()
             assert self._terms[0].package == Package.root()
 
-            return '{} is {}'.format(self._terms[0].package, self._terms[0].constraint)
+            return f'{self._terms[0].package} is {self._terms[0].constraint}'
 
     def __str__(self):
         cause_string = self.handle_cause()
         if cause_string is not None:
             return cause_string
         elif self.is_failure():
             return 'version solving failed'
@@ -174,17 +169,17 @@
             term2 = self._terms[1]
 
             if term1.is_positive() == term2.is_positive():
                 if term1.is_positive():
                     package1 = term1.package if term1.constraint.is_any() else self._terse(term1)
                     package2 = term2.package if term2.constraint.is_any() else self._terse(term2)
 
-                    return '{} is incompatible with {}'.format(package1, package2)
+                    return f'{package1} is incompatible with {package2}'
                 else:
-                    return 'either {} or {}'.format(self._terse(term1), self._terse(term2))
+                    return f'either {self._terse(term1)} or {self._terse(term2)}'
 
         positive = []
         negative = []
 
         for term in self._terms:
             if term.is_positive():
                 positive.append(term.to_string(allow_every=True))
@@ -202,16 +197,16 @@
                 return 'if {} then {}'.format(' and '.join(positive), ' or '.join(negative))
         elif positive:
             return 'one of {} must be false'.format(' or '.join(positive))
         else:
             return 'one of {} must be true'.format(' or '.join(negative))
 
     def and_to_string(
-        self, other, details, this_line, other_line
-    ):  # type: (Incompatibility, dict, int, int) -> str
+        self, other: Incompatibility, details: t.Dict, this_line: int, other_line: int
+    ) -> str:
         requires_both = self._try_requires_both(other, details, this_line, other_line)
         if requires_both is not None:
             return requires_both
 
         requires_through = self._try_requires_through(other, details, this_line, other_line)
         if requires_through is not None:
             return requires_through
@@ -220,70 +215,70 @@
         if requires_forbidden is not None:
             return requires_forbidden
 
         buffer = [str(self)]
         if this_line is not None:
             buffer.append(' ' + this_line)
 
-        buffer.append(' and {}'.format(str(other)))
+        buffer.append(f' and {str(other)}')
 
         if other_line is not None:
             buffer.append(' ' + other_line)
 
         return '\n'.join(buffer)
 
     def _try_requires_both(
-        self, other, details, this_line, other_line
-    ):  # type: (Incompatibility, dict, int, int) -> Optional[str]
+        self, other: Incompatibility, details: t.Dict, this_line: int, other_line: int
+    ) -> t.Optional[str]:
         if len(self._terms) == 1 or len(other.terms) == 1:
             return
 
         this_positive = self._single_term_where(lambda term: term.is_positive())
         if this_positive is None:
             return
 
         other_positive = other._single_term_where(lambda term: term.is_positive())
         if other_positive is None:
             return
 
         if this_positive.package != other_positive.package:
             return
 
-        this_negatives = ' or '.join(
-            [term.inverse.to_string() for term in self._terms if not term.is_positive()]
-        )
-
-        other_negatives = ' or '.join(
-            [term.inverse.to_string() for term in other.terms if not term.is_positive()]
-        )
+        this_negatives = ' or '.join([
+            term.inverse.to_string() for term in self._terms if not term.is_positive()
+        ])
+
+        other_negatives = ' or '.join([
+            term.inverse.to_string() for term in other.terms if not term.is_positive()
+        ])
 
         buffer = [self._terse(this_positive, allow_every=True) + ' ']
         is_dependency = isinstance(self.cause, DependencyCause) and isinstance(
             other.cause, DependencyCause
         )
 
         if is_dependency:
             buffer.append('depends on')
         else:
             buffer.append('requires')
 
-        buffer.append(' both {}'.format(this_negatives))
+        buffer.append(f' both {this_negatives}')
         if this_line is not None:
-            buffer.append(' ({})'.format(this_line))
+            buffer.append(f' ({this_line})')
 
-        buffer.append(' and {}'.format(other_negatives))
+        buffer.append(f' and {other_negatives}')
 
         if other_line is not None:
-            buffer.append(' ({})'.format(other_line))
+            buffer.append(f' ({other_line})')
 
         return ''.join(buffer)
 
     def _try_requires_through(
-        self, other, details, this_line, other_line
-    ):  # type: (Incompatibility, dict, int, int) -> Optional[str]
+        self, other: Incompatibility, details: t.Dict, this_line: int, other_line: int
+    ) -> t.Optional[str]:
         if len(self._terms) == 1 or len(other.terms) == 1:
             return
 
         this_negative = self._single_term_where(lambda term: not term.is_positive())
         other_negative = other._single_term_where(lambda term: not term.is_positive())
 
         if this_negative is None and other_negative is None:
@@ -318,48 +313,48 @@
             return
 
         prior_positives = [term for term in prior.terms if term.is_positive()]
 
         buffer = []
         if len(prior_positives) > 1:
             prior_string = ' or '.join([self._terse(term) for term in prior_positives])
-            buffer.append('if {} then '.format(prior_string))
+            buffer.append(f'if {prior_string} then ')
         else:
             if isinstance(prior.cause, DependencyCause):
                 verb = 'depends on'
             else:
                 verb = 'requires'
 
             buffer.append('{} {} '.format(prior_positives[0].to_string(allow_every=True), verb))
 
         buffer.append(prior_negative.inverse.to_string())
         if prior_line is not None:
-            buffer.append(' ({})'.format(prior_line))
+            buffer.append(f' ({prior_line})')
 
         buffer.append(' which ')
 
         if isinstance(latter.cause, DependencyCause):
             buffer.append('depends on ')
         else:
             buffer.append('requires ')
 
         buffer.append(
-            ' or '.join(
-                [term.inverse.to_string() for term in latter.terms if not term.is_positive()]
-            )
+            ' or '.join([
+                term.inverse.to_string() for term in latter.terms if not term.is_positive()
+            ])
         )
 
         if latter_line is not None:
-            buffer.append(' ({})'.format(latter_line))
+            buffer.append(f' ({latter_line})')
 
         return ''.join(buffer)
 
     def _try_requires_forbidden(
-        self, other, details, this_line, other_line
-    ):  # type: (Incompatibility, dict, int, int) -> Optional[str]
+        self, other: Incompatibility, details: t.Dict, this_line: int, other_line: int
+    ) -> t.Optional[str]:
         if len(self._terms) != 1 and len(other.terms) != 1:
             return None
 
         if len(self.terms) == 1:
             prior = other
             latter = self
             prior_line = other_line
@@ -378,49 +373,49 @@
             return
 
         positives = [t for t in prior.terms if t.is_positive()]
 
         buffer = []
         if len(positives) > 1:
             prior_string = ' or '.join([self._terse(term) for term in positives])
-            buffer.append('if {} then '.format(prior_string))
+            buffer.append(f'if {prior_string} then ')
         else:
             buffer.append(self._terse(positives[0], allow_every=True))
             if isinstance(prior.cause, DependencyCause):
                 buffer.append(' depends on ')
             else:
                 buffer.append(' requires ')
 
         buffer.append(latter.terms[0].to_string(allow_every=True) + ' ')
         if prior_line is not None:
-            buffer.append('({}) '.format(prior_line))
+            buffer.append(f'({prior_line}) ')
 
         if isinstance(latter.cause, NoVersionsCause):
             buffer.append("which doesn't match any versions")
         elif isinstance(latter.cause, PackageNotFoundCause):
             buffer.append("which doesn't exist")
         else:
             buffer.append('which is forbidden')
 
         if latter_line is not None:
-            buffer.append(' ({})'.format(latter_line))
+            buffer.append(f' ({latter_line})')
 
         return ''.join(buffer)
 
-    def _terse(self, term, allow_every=False):  # type: (Term, bool) -> str
+    def _terse(self, term: Term, allow_every: bool = False) -> str:
         return term.to_string(allow_every=allow_every)
 
-    def _single_term_where(self, callable):  # type: (callable) -> Optional[Term]
+    def _single_term_where(self, callable: callable) -> t.Optional[Term]:
         found = None
         for term in self._terms:
             if not callable(term):
                 continue
 
             if found is not None:
                 return
 
             found = term
 
         return found
 
     def __repr__(self):
-        return '<{} {}>'.format(self.__class__.__name__, str(self))
+        return f'<{self.__class__.__name__} {str(self)}>'
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/incompatibility_cause.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/incompatibility_cause.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2018 Sébastien Eustace
 # SPDX-License-Identifier: MIT License
 # SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
 
 
 class IncompatibilityCause(Exception):
     """
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/package.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/package.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,53 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2018 Sébastien Eustace
 # SPDX-License-Identifier: MIT License
-# SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileContributor: 2022-2024 Espressif Systems (Shanghai) CO LTD
+from __future__ import annotations
 
-try:
-    from typing import Optional
-except ImportError:
-    pass
+import typing as t
 
 from idf_component_tools.sources import BaseSource
 
 
-class Package(object):
+class Package:
     """
     A project's package.
     """
 
     ROOT_PACKAGE_NAME = '_root_'
 
-    def __init__(self, name, source=None):  # type: (str, Optional[BaseSource]) -> None
+    def __init__(self, name: str, source: t.Optional[BaseSource] = None) -> None:
         self._name = name
         self._source = source
 
     @classmethod
-    def root(cls):  # type: () -> Package
+    def root(cls) -> Package:
         return Package(cls.ROOT_PACKAGE_NAME)
 
     @property
-    def name(self):  # type: () -> str
+    def name(self) -> str:
         return self._name
 
     @property
-    def source(self):  # type: () -> BaseSource
+    def source(self) -> BaseSource:
         return self._source
 
-    def __eq__(self, other):  # type: (Package) -> bool
+    def __eq__(self, other: Package) -> bool:
         if not isinstance(other, Package):
             return NotImplemented
 
         return self.name == other.name and self.source == other.source
 
-    def __ne__(self, other):  # type: (Package) -> bool
+    def __ne__(self, other: Package) -> bool:
         if not isinstance(other, Package):
             return NotImplemented
 
         return not (self == other)
 
-    def __str__(self):  # type: () -> str
+    def __str__(self) -> str:
         return self._name
 
-    def __repr__(self):  # type: () -> str
-        return 'Package("{}" {})'.format(self.name, self.source)
+    def __repr__(self) -> str:
+        return f'Package("{self.name}" {self.source})'
 
     def __hash__(self):
         return hash(self.name)
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/package_source.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/package_source.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2018 Sébastien Eustace
 # SPDX-License-Identifier: MIT License
-# SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileContributor: 2022-2024 Espressif Systems (Shanghai) CO LTD
 
-from idf_component_tools.manifest import HashedComponentVersion
+import typing as t
 
-try:
-    from typing import Any, List
-    from typing import Union as _Union
-except ImportError:
-    pass
+from idf_component_tools.utils import HashedComponentVersion
 
 from .constraint import Constraint
 from .incompatibility import Incompatibility
 from .incompatibility_cause import DependencyCause, SelfDependentCause
 from .package import Package
 from .range import Range
 from .term import Term
 from .union import Union
 
 
-class PackageSource(object):
+class PackageSource:
     """
     Provides information about specifications and dependencies to the resolver,
     allowing the VersionResolver class to remain generic while still providing power
     and flexibility.
 
     This contract contains the methods that users of Mixology must implement
     using knowledge of their own model classes.
@@ -60,54 +55,52 @@
 
     It is returned by dependencies_for(package, version) and will be passed to
     convert_dependency(dependency) to convert it to a format Mixology understands.
 
     __eq__() should be defined.
     """
 
-    def __init__(self):  # type: () -> None
+    def __init__(self) -> None:
         self._root_package = Package.root()
 
     @property
-    def root(self):  # type: () -> Package
+    def root(self) -> Package:
         return Package.root()
 
     @property
-    def root_version(self):  # type: () -> HashedComponentVersion
+    def root_version(self) -> HashedComponentVersion:
         raise NotImplementedError()
 
     def versions_for(
-        self, package, constraint=None
-    ):  # type: (Package, Any) -> List[HashedComponentVersion]
+        self, package: Package, constraint: t.Any = None
+    ) -> t.List[HashedComponentVersion]:
         """
         Search for the specifications that match the given constraint.
         """
         if package == self._root_package:
             return [self.root_version]
 
         return self._versions_for(package, constraint)
 
     def _versions_for(
-        self, package, constraint=None
-    ):  # type: (Package, Any) -> List[HashedComponentVersion]
+        self, package: Package, constraint: t.Any = None
+    ) -> t.List[HashedComponentVersion]:
         raise NotImplementedError()
 
-    def dependencies_for(self, package, version):  # type: (Package, Any) -> List[Any]
+    def dependencies_for(self, package: Package, version: t.Any) -> t.List[t.Any]:
         raise NotImplementedError()
 
-    def convert_dependency(self, dependency):  # type: (Any) -> _Union[Constraint, Range, Union]
+    def convert_dependency(self, dependency: t.Any) -> t.Union[Constraint, Range, Union]:
         """
         Converts a user-defined dependency (returned by dependencies_for())
         into a format Mixology understands.
         """
         raise NotImplementedError()
 
-    def incompatibilities_for(
-        self, package, version
-    ):  # type: (Package, Any) -> List[Incompatibility]
+    def incompatibilities_for(self, package: Package, version: t.Any) -> t.List[Incompatibility]:
         """
         Returns the incompatibilities of a given package and version
         """
         dependencies = self.dependencies_for(package, version)
         package_constraint = Constraint(package, Range(version, version, True, True))
 
         incompatibilities = []
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/partial_solution.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/partial_solution.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2018 Sébastien Eustace
 # SPDX-License-Identifier: MIT License
-# SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
-
-try:
-    from typing import Dict, List
-except ImportError:
-    pass
+# SPDX-FileContributor: 2022-2024 Espressif Systems (Shanghai) CO LTD
 
+import typing as t
 from collections import OrderedDict
 
-from idf_component_tools.manifest import HashedComponentVersion
+from idf_component_tools.utils import HashedComponentVersion
 
 from .assignment import Assignment
 from .constraint import Constraint
 from .incompatibility import Incompatibility
 from .package import Package
 from .set_relation import SetRelation
 from .term import Term
@@ -25,59 +20,59 @@
     # A list of Assignments that represent the solver's current best guess about
     # what's true for the eventual set of package versions that will comprise the
     # total solution.
     #
     # See https://github.com/dart-lang/mixology/tree/master/doc/solver.md#partial-solution.
     """
 
-    def __init__(self):  # type: () -> None
+    def __init__(self) -> None:
         # The assignments that have been made so far, in the order they were
         # assigned.
-        self._assignments = []  # type: List[Assignment]
+        self._assignments: t.List[Assignment] = []
 
         # The decisions made for each package.
-        self._decisions = OrderedDict()  # type: Dict[Package, HashedComponentVersion]
+        self._decisions: t.Dict[Package, HashedComponentVersion] = OrderedDict()
 
         # The intersection of all positive Assignments for each package, minus any
         # negative Assignments that refer to that package.
         #
         # This is derived from self._assignments.
-        self._positive = OrderedDict()  # type: Dict[Package, Term]
+        self._positive: t.Dict[Package, Term] = OrderedDict()
 
         # The union of all negative Assignments for each package.
         #
         # If a package has any positive Assignments, it doesn't appear in this
         # map.
         #
         # This is derived from self._assignments.
-        self._negative = OrderedDict()  # type: Dict[Package, Dict[Package, Term]]
+        self._negative: t.Dict[Package, t.Dict[Package, Term]] = OrderedDict()
 
         # The number of distinct solutions that have been attempted so far.
         self._attempted_solutions = 1
 
         # Whether the solver is currently backtracking.
         self._backtracking = False
 
     @property
-    def decisions(self):  # type: () -> Dict[Package, HashedComponentVersion]
+    def decisions(self) -> t.Dict[Package, HashedComponentVersion]:
         return self._decisions
 
     @property
-    def decision_level(self):  # type: () -> int
+    def decision_level(self) -> int:
         return len(self._decisions)
 
     @property
-    def attempted_solutions(self):  # type: () -> int
+    def attempted_solutions(self) -> int:
         return self._attempted_solutions
 
     @property
-    def unsatisfied(self):  # type: () -> List[Term]
+    def unsatisfied(self) -> t.List[Term]:
         return [term for term in self._positive.values() if term.package not in self._decisions]
 
-    def decide(self, package, version):  # type: (Package, HashedComponentVersion) -> None
+    def decide(self, package: Package, version: HashedComponentVersion) -> None:
         """
         Adds an assignment of package as a decision
         and increments the decision level.
         """
         # When we make a new decision after backtracking, count an additional
         # attempted solution. If we backtrack multiple times in a row, though, we
         # only want to count one, since we haven't actually started attempting a
@@ -88,38 +83,36 @@
         self._backtracking = False
         self._decisions[package] = version
 
         self._assign(
             Assignment.decision(package, version, self.decision_level, len(self._assignments))
         )
 
-    def derive(
-        self, constraint, is_positive, cause
-    ):  # type: (Constraint, bool, Incompatibility) -> None
+    def derive(self, constraint: Constraint, is_positive: bool, cause: Incompatibility) -> None:
         """
         Adds an assignment of package as a derivation.
         """
         self._assign(
             Assignment.derivation(
                 constraint,
                 is_positive,
                 cause,
                 self.decision_level,
                 len(self._assignments),
             )
         )
 
-    def _assign(self, assignment):  # type: (Assignment) -> None
+    def _assign(self, assignment: Assignment) -> None:
         """
         Adds an Assignment to _assignments and _positive or _negative.
         """
         self._assignments.append(assignment)
         self._register(assignment)
 
-    def backtrack(self, decision_level):  # type: (int) -> None
+    def backtrack(self, decision_level: int) -> None:
         """
         Resets the current decision level to decision_level, and removes all
         assignments made after that level.
         """
         self._backtracking = True
 
         packages = set()
@@ -137,15 +130,15 @@
             if package in self._negative:
                 del self._negative[package]
 
         for assignment in self._assignments:
             if assignment.package in packages:
                 self._register(assignment)
 
-    def _register(self, assignment):  # type: (Assignment) -> None
+    def _register(self, assignment: Assignment) -> None:
         """
         Registers an Assignment in _positive or _negative.
         """
         package = assignment.package
         old_positive = self._positive.get(package)
         if old_positive is not None:
             self._positive[package] = old_positive.intersect(assignment)
@@ -167,20 +160,20 @@
             self._positive[package] = term
         else:
             if package not in self._negative:
                 self._negative[package] = {}
 
             self._negative[package][package] = term
 
-    def satisfier(self, term):  # type: (Term) -> Assignment
+    def satisfier(self, term: Term) -> Assignment:
         """
         Returns the first Assignment in this solution such that the sublist of
         assignments up to and including that entry collectively satisfies term.
         """
-        assigned_term = None  # type: Term
+        assigned_term: Term = None
 
         for assignment in self._assignments:
             if assignment.package != term.package:
                 continue
 
             if assignment.package != Package.root() and not assignment.package == term.package:
                 if not assignment.is_positive():
@@ -195,20 +188,20 @@
             else:
                 assigned_term = assigned_term.intersect(assignment)
 
             # As soon as we have enough assignments to satisfy term, return them.
             if assigned_term.satisfies(term):
                 return assignment
 
-        raise RuntimeError('[BUG] {} is not satisfied.'.format(term))
+        raise RuntimeError(f'[BUG] {term} is not satisfied.')
 
-    def satisfies(self, term):  # type: (Term) -> bool
+    def satisfies(self, term: Term) -> bool:
         return self.relation(term) == SetRelation.SUBSET
 
-    def relation(self, term):  # type: (Term) -> SetRelation
+    def relation(self, term: Term) -> SetRelation:
         positive = self._positive.get(term.package)
         if positive is not None:
             return positive.relation(term)
 
         by_ref = self._negative.get(term.package)
         if by_ref is None:
             return SetRelation.OVERLAPPING
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/range.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/range.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2018 Sébastien Eustace
 # SPDX-License-Identifier: MIT License
-# SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileContributor: 2022-2024 Espressif Systems (Shanghai) CO LTD
 
-try:
-    from typing import TYPE_CHECKING, Any, NoReturn, Optional
-    from typing import Union as _Union
+from __future__ import annotations
 
-    if TYPE_CHECKING:
-        from .union import Union
-except ImportError:
-    pass
+import typing as t
 
+if t.TYPE_CHECKING:
+    from .union import Union
 
-class Range(object):
+
+class Range:
     """
     A range of versions represented by a minimum version,
     a maximum version and whether they are included in the range.
 
     Both the minimum and maximum versions can be left out
     to represent unbounded ranges.
 
     A single version is represented by Range(version, version, True, True).
     """
 
     def __init__(
         self,
-        min=None,
-        max=None,
-        include_min=False,
-        include_max=False,
-        string=None,
-    ):  # type: (Any, Any, bool, bool, Optional[str]) -> None
+        min: t.Any = None,
+        max: t.Any = None,
+        include_min: bool = False,
+        include_max: bool = False,
+        string: t.Optional[str] = None,
+    ) -> None:
         self._min = min
         self._max = max
         self._include_min = include_min
         self._include_max = include_max
         self._hash = None
         self._string = string
 
@@ -52,15 +49,15 @@
         return self._include_min
 
     @property
     def include_max(self):
         return self._include_max
 
     @property
-    def inverse(self):  # type: () -> _Union[Range, Union]
+    def inverse(self) -> t.Union[Range, Union]:
         if self.is_any():
             return EmptyRange()
 
         low = Range(max=self.min, include_max=not self.include_min)
         high = Range(min=self.max, include_min=not self.include_max)
 
         if self.min is None:
@@ -73,37 +70,37 @@
 
     def is_empty(self):
         return False
 
     def is_any(self):
         return self._min is None and self._max is None
 
-    def allows_all(self, other):  # type: (Range) -> bool
+    def allows_all(self, other: Range) -> bool:
         from .union import Union  # fool the interpreter
 
         if other.is_empty():
             return True
 
         if isinstance(other, Union):
             return all([self.allows_all(constraint) for constraint in other.ranges])
 
         return not other.allows_lower(self) and not other.allows_higher(self)
 
-    def allows_any(self, other):  # type: (Range) -> bool
+    def allows_any(self, other: Range) -> bool:
         from .union import Union  # fool the interpreter
 
         if other.is_empty():
             return False
 
         if isinstance(other, Union):
             return any([self.allows_any(constraint) for constraint in other.ranges])
 
         return not other.is_strictly_lower(self) and not other.is_strictly_higher(self)
 
-    def intersect(self, other):  # type: (_Union[Range, Union]) -> _Union[Range, Union]
+    def intersect(self, other: t.Union[Range, Union]) -> t.Union[Range, Union]:
         from .union import Union  # fool the interpreter
 
         if other.is_empty():
             return other
 
         if isinstance(other, Union):
             return other.intersect(self)
@@ -144,15 +141,15 @@
             assert intersect_include_min and intersect_include_max
 
             return Range(intersect_min, intersect_max, True, True)
 
         # If we got here, there is an actual range.
         return Range(intersect_min, intersect_max, intersect_include_min, intersect_include_max)
 
-    def union(self, other):  # type: (Range) -> _Union[Range, Union]
+    def union(self, other: Range) -> t.Union[Range, Union]:
         from .union import Union  # fool the interpreter
 
         if isinstance(other, Union):
             return other.union(self)
 
         if not self.is_contiguous_to(other):
             return Union.of(self, other)
@@ -174,25 +171,25 @@
         return Range(
             union_min,
             union_max,
             include_min=union_include_min,
             include_max=union_include_max,
         )
 
-    def is_contiguous_to(self, other):  # type: (Range) -> bool
+    def is_contiguous_to(self, other: Range) -> bool:
         if other.is_empty():
             return False
 
         return (
             self.allows_any(other)
             or (self.max == other.min and (self.include_max or other.include_min))
             or (self.min == other.max and (self.include_min or other.include_max))
         )
 
-    def difference(self, other):  # type: (_Union[Range, Union]) -> _Union[Range, Union]
+    def difference(self, other: t.Union[Range, Union]) -> t.Union[Range, Union]:
         from .union import Union  # fool the interpreter
 
         if other.is_empty():
             return self
 
         if isinstance(other, Union):
             ranges = []
@@ -248,68 +245,68 @@
             return after
 
         if after is None:
             return before
 
         return Union.of(before, after)
 
-    def allows_lower(self, other):  # type: (Range) -> bool
+    def allows_lower(self, other: Range) -> bool:
         if self.min is None:
             return other.min is not None
 
         if other.min is None:
             return False
 
         if self.min < other.min:
             return True
 
         if self.min > other.min:
             return False
 
         return self.include_min and not other.include_min
 
-    def allows_higher(self, other):  # type: (Range) -> bool
+    def allows_higher(self, other: Range) -> bool:
         if self.max is None:
             return other.max is not None
 
         if other.max is None:
             return False
 
         if self.max < other.max:
             return False
 
         if self.max > other.max:
             return True
 
         return self.include_max and not other.include_max
 
-    def is_strictly_lower(self, other):  # type: (Range) -> bool
+    def is_strictly_lower(self, other: Range) -> bool:
         if self.max is None or other.min is None:
             return False
 
         if self.max < other.min:
             return True
 
         if self.max > other.min:
             return False
 
         return not self.include_max or not other.include_min
 
-    def is_strictly_higher(self, other):  # type: (Range) -> bool
+    def is_strictly_higher(self, other: Range) -> bool:
         return other.is_strictly_lower(self)
 
-    def is_adjacent_to(self, other):  # type: (Range) -> bool
+    def is_adjacent_to(self, other: Range) -> bool:
         if self.max != other.min:
             return False
 
         return (
             self.include_max and not other.include_min or not self.include_max and other.include_min
         )
 
-    def is_single_version(self):  # type: () -> bool
+    def is_single_version(self) -> bool:
         return (
             self.min is not None and self.min == self.max and self.include_min and self.include_max
         )
 
     def __eq__(self, other):
         if not isinstance(other, Range):
             return False
@@ -329,15 +326,15 @@
 
     def __gt__(self, other):
         return self._cmp(other) > 0
 
     def __ge__(self, other):
         return self._cmp(other) >= 0
 
-    def _cmp(self, other):  # type: (Range) -> int
+    def _cmp(self, other: Range) -> int:
         if self.min is None:
             if other.min is None:
                 return self._compare_max(other)
 
             return -1
         elif other.min is None:
             return 1
@@ -346,15 +343,15 @@
             return -1 if self.min < other.min else 1
 
         if self.include_min != other.include_min:
             return -1 if self.include_min else 1
 
         return self._compare_max(other)
 
-    def _compare_max(self, other):  # type: (Range) -> int
+    def _compare_max(self, other: Range) -> int:
         if self.max is None:
             if other.max is None:
                 return 0
 
             return 1
         elif other.max is None:
             return -1
@@ -371,15 +368,15 @@
         if self._string is not None:
             return self._string
 
         text = ''
 
         if self.min is not None:
             if self.min == self.max and self.include_min and self.include_max:
-                return '{}'.format(self.min)
+                return f'{self.min}'
 
             text += '>=' if self.include_min else '>'
             text += self.min.text
 
         if self.max is not None:
             if self.min is not None:
                 text += ','
@@ -388,62 +385,62 @@
 
         if self.min is None and self.max is None:
             return '*'
 
         return text
 
     def __repr__(self):
-        return '<Range ({})>'.format(str(self))
+        return f'<Range ({str(self)})>'
 
     def __hash__(self):
         if self._hash is None:
             self._hash = (
                 hash(self.min) ^ hash(self.max) ^ hash(self.include_min) ^ hash(self.include_max)
             )
 
         return self._hash
 
 
 class EmptyRange(Range):
     @property
-    def min(self):  # type: () -> NoReturn
+    def min(self) -> t.NoReturn:
         raise NotImplementedError()
 
     @property
-    def max(self):  # type: () -> NoReturn
+    def max(self) -> t.NoReturn:
         raise NotImplementedError()
 
     @property
-    def include_min(self):  # type: () -> NoReturn
+    def include_min(self) -> t.NoReturn:
         raise NotImplementedError()
 
     @property
-    def include_max(self):  # type: () -> NoReturn
+    def include_max(self) -> t.NoReturn:
         raise NotImplementedError()
 
-    def is_empty(self):  # type: () -> bool
+    def is_empty(self) -> bool:
         return True
 
-    def is_any(self):  # type: () -> bool
+    def is_any(self) -> bool:
         return False
 
-    def __eq__(self, other):  # type: (Range) -> bool
+    def __eq__(self, other: Range) -> bool:
         return other.is_empty()
 
-    def intersect(self, other):  # type: (Range) -> Range
+    def intersect(self, other: Range) -> Range:
         return self
 
-    def allows_all(self, other):  # type: (Range) -> bool
+    def allows_all(self, other: Range) -> bool:
         return other.is_empty()
 
-    def allows_any(self, other):  # type: (Range) -> bool
+    def allows_any(self, other: Range) -> bool:
         return other.is_empty()
 
-    def is_single_version(self):  # type: () -> bool
+    def is_single_version(self) -> bool:
         return False
 
     @property
-    def inverse(self):  # type: () -> _Union[Range, Union]
+    def inverse(self) -> t.Union[Range, Union]:
         return Range()
 
-    def __str__(self):  # type: () -> str
+    def __str__(self) -> str:
         return '(no versions)'
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/result.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/result.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2018 Sébastien Eustace
 # SPDX-License-Identifier: MIT License
-# SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileContributor: 2022-2024 Espressif Systems (Shanghai) CO LTD
 
-try:
-    from typing import Dict
-except ImportError:
-    pass
+import typing as t
 
 from idf_component_manager.version_solver.mixology.package import Package
-from idf_component_tools.manifest import HashedComponentVersion
+from idf_component_tools.utils import HashedComponentVersion
 
 
 class SolverResult:
     def __init__(
-        self, decisions, attempted_solutions
-    ):  # type: (Dict[Package, HashedComponentVersion], int) -> None
+        self, decisions: t.Dict[Package, HashedComponentVersion], attempted_solutions: int
+    ) -> None:
         self._decisions = decisions
         self._attempted_solutions = attempted_solutions
 
     @property
-    def decisions(self):  # type: () -> Dict[Package, HashedComponentVersion]
+    def decisions(self) -> t.Dict[Package, HashedComponentVersion]:
         return self._decisions
 
     @property
-    def attempted_solutions(self):  # type: () -> int
+    def attempted_solutions(self) -> int:
         return self._attempted_solutions
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/term.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/term.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,69 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2018 Sébastien Eustace
 # SPDX-License-Identifier: MIT License
-# SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileContributor: 2022-2024 Espressif Systems (Shanghai) CO LTD
+from __future__ import annotations
 
-try:
-    from typing import Optional
-except ImportError:
-    pass
+import typing as t
 
 from .constraint import Constraint
 from .package import Package
 from .set_relation import SetRelation
 
 
-class Term(object):
+class Term:
     """
     A statement about a package which is true or false for a given selection of
     package versions.
     """
 
-    def __init__(self, constraint, is_positive):  # type: (Constraint, bool) -> None
+    def __init__(self, constraint: Constraint, is_positive: bool) -> None:
         self._constraint = constraint
         self._package = constraint.package
         self._positive = is_positive
         self._normalized_constraint = None
         self._empty = None
 
     @property
-    def inverse(self):  # type: () -> Term
+    def inverse(self) -> Term:
         return Term(self.constraint, not self.is_positive())
 
     @property
-    def package(self):  # type: () -> Package
+    def package(self) -> Package:
         return self._package
 
     @property
-    def constraint(self):  # type: () -> Constraint
+    def constraint(self) -> Constraint:
         return self._constraint
 
     @property
-    def normalized_constraint(self):  # type: () -> Constraint
+    def normalized_constraint(self) -> Constraint:
         if self._normalized_constraint is None:
             self._normalized_constraint = (
                 self.constraint if self.is_positive() else self.constraint.inverse
             )
 
         return self._normalized_constraint
 
-    def is_positive(self):  # type: () -> bool
+    def is_positive(self) -> bool:
         return self._positive
 
-    def satisfies(self, other):  # type: (Term) -> bool
+    def satisfies(self, other: Term) -> bool:
         """
         Returns whether this term satisfies another.
         """
         return self._package == other.package and self.relation(other) == SetRelation.SUBSET
 
-    def relation(self, other):  # type: (Term) -> SetRelation
+    def relation(self, other: Term) -> SetRelation:
         """
         Returns the relationship between the package versions
         allowed by this term and another.
         """
         if self.package != other.package:
-            raise ValueError('{} should refer to {}'.format(other, self.package))
+            raise ValueError(f'{other} should refer to {self.package}')
 
         if other.is_positive():
             if self.is_positive():
                 if not self.is_compatible_with(other):
                     return SetRelation.DISJOINT
 
                 # foo ^1.5.0 is a subset of foo ^1.0.0
@@ -112,21 +109,21 @@
                 if self.constraint.allows_all(other.constraint):
                     return SetRelation.SUBSET
 
                 # not foo ^2.0.0 overlaps not foo ^1.0.0
                 # not foo ^1.5.0 is a superset of not foo ^1.0.0
                 return SetRelation.OVERLAPPING
 
-    def intersect(self, other):  # type: (Term) -> Optional[Term]
+    def intersect(self, other: Term) -> t.Optional[Term]:
         """
         Returns a Term that represents the packages
         allowed by both this term and another
         """
         if self.package != other.package:
-            raise ValueError('{} should refer to {}'.format(other, self.package))
+            raise ValueError(f'{other} should refer to {self.package}')
 
         if self.is_compatible_with(other):
             if self.is_positive() != other.is_positive():
                 # foo ^1.0.0 ∩ not foo ^1.5.0 → foo >=1.0.0 <1.5.0
                 positive = self if self.is_positive() else other
                 negative = other if self.is_positive() else self
 
@@ -140,46 +137,44 @@
                 # not foo ^1.0.0 ∩ not foo >=1.5.0 <3.0.0 → not foo >=1.0.0 <3.0.0
                 return self._non_empty_term(self.constraint.union(other.constraint), False)
         elif self.is_positive() != other.is_positive():
             return self if self.is_positive() else other
         else:
             return
 
-    def difference(self, other):  # type: (Term) -> Term
+    def difference(self, other: Term) -> Term:
         """
         Returns a Term that represents packages
         allowed by this term and not by the other
         """
         return self.intersect(other.inverse)
 
-    def is_compatible_with(self, other):  # type: (Term) -> bool
+    def is_compatible_with(self, other: Term) -> bool:
         return (
             self.package == Package.root()
             or other.package == Package.root()
             or self.package == other.package
         )
 
-    def is_empty(self):  # type: () -> bool
+    def is_empty(self) -> bool:
         if self._empty is None:
             self._empty = self.normalized_constraint.is_empty()
 
         return self._empty
 
-    def _non_empty_term(
-        self, constraint, is_positive
-    ):  # type: (Constraint, bool) -> Optional[Term]
+    def _non_empty_term(self, constraint: Constraint, is_positive: bool) -> t.Optional[Term]:
         if constraint.is_empty():
             return
 
         return Term(constraint, is_positive)
 
-    def to_string(self, allow_every=False):  # type: (bool) -> str
+    def to_string(self, allow_every: bool = False) -> str:
         if self.is_positive():
             return self.constraint.to_string(allow_every=allow_every)
 
-        return 'not {}'.format(self.constraint)
+        return f'not {self.constraint}'
 
     def __str__(self):
         return self.to_string()
 
     def __repr__(self):
-        return '<Term {}>'.format(str(self))
+        return f'<Term {str(self)}>'
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/union.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/union.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2018 Sébastien Eustace
 # SPDX-License-Identifier: MIT License
-# SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileContributor: 2022-2024 Espressif Systems (Shanghai) CO LTD
 
-try:
-    from typing import List
-    from typing import Union as _Union
-except ImportError:
-    pass
+from __future__ import annotations
+
+import typing as t
 
 from .range import EmptyRange, Range
 
 
-class Union(object):
+class Union:
     """
     An union of Ranges.
     """
 
     def __init__(self, *ranges):
         self._ranges = list(ranges)
 
@@ -62,30 +59,30 @@
 
     def is_empty(self):
         return False
 
     def is_any(self):
         return False
 
-    def allows_all(self, other):  # type: (_Union[Range, Union]) -> bool
+    def allows_all(self, other: t.Union[Range, Union]) -> bool:
         our_ranges = iter(self._ranges)
         their_ranges = iter(self._ranges_for(other))
 
         our_current_range = next(our_ranges, None)
         their_current_range = next(their_ranges, None)
 
         while our_current_range and their_current_range:
             if our_current_range.allows_all(their_current_range):
                 their_current_range = next(their_ranges, None)
             else:
                 our_current_range = next(our_ranges, None)
 
         return their_current_range is None
 
-    def allows_any(self, other):  # type: (_Union[Range, Union]) -> bool
+    def allows_any(self, other: t.Union[Range, Union]) -> bool:
         our_ranges = iter(self._ranges)
         their_ranges = iter(self._ranges_for(other))
 
         our_current_range = next(our_ranges, None)
         their_current_range = next(their_ranges, None)
 
         while our_current_range and their_current_range:
@@ -95,15 +92,15 @@
             if their_current_range.allows_higher(our_current_range):
                 our_current_range = next(our_ranges, None)
             else:
                 their_current_range = next(their_ranges, None)
 
         return False
 
-    def intersect(self, other):  # type: (_Union[Range, Union]) -> _Union[Range, Union]
+    def intersect(self, other: t.Union[Range, Union]) -> t.Union[Range, Union]:
         our_ranges = iter(self._ranges)
         their_ranges = iter(self._ranges_for(other))
         new_ranges = []
 
         our_current_range = next(our_ranges, None)
         their_current_range = next(their_ranges, None)
 
@@ -116,18 +113,18 @@
             if their_current_range.allows_higher(our_current_range):
                 our_current_range = next(our_ranges, None)
             else:
                 their_current_range = next(their_ranges, None)
 
         return Union.of(*new_ranges)
 
-    def union(self, other):  # type: (_Union[Range, Union]) -> _Union[Range, Union]
+    def union(self, other: t.Union[Range, Union]) -> t.Union[Range, Union]:
         return Union.of(self, other)
 
-    def difference(self, other):  # type: (_Union[Range, Union]) -> _Union[Range, Union]
+    def difference(self, other: t.Union[Range, Union]) -> t.Union[Range, Union]:
         our_ranges = iter(self._ranges)
         their_ranges = iter(self._ranges_for(other))
         new_ranges = []
 
         state = {
             'current': next(our_ranges, None),
             'their_range': next(their_ranges, None),
@@ -199,20 +196,20 @@
             return EmptyRange()
 
         if len(new_ranges) == 1:
             return new_ranges[0]
 
         return Union.of(*new_ranges)
 
-    def excludes_single_version(self):  # type: () -> bool
+    def excludes_single_version(self) -> bool:
         difference = self.difference(Range())
 
         return isinstance(difference, Range) and difference.is_single_version()
 
-    def _ranges_for(self, constraint):  # type: (_Union[Union, Range]) -> List[Range]
+    def _ranges_for(self, constraint: t.Union[Union, Range]) -> t.List[Range]:
         if constraint.is_empty():
             return []
 
         if isinstance(constraint, Union):
             return constraint.ranges
 
         return [constraint]
@@ -221,13 +218,13 @@
         if not isinstance(other, Union):
             return False
 
         return self._ranges == other.ranges
 
     def __str__(self):
         if self.excludes_single_version():
-            return '!={}'.format(Range().difference(self))
+            return f'!={Range().difference(self)}'
 
         return ' || '.join([str(r) for r in self._ranges])
 
     def __repr__(self):
-        return '<Union {}>'.format(str(self))
+        return f'<Union {self}>'
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/mixology/version_solver.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/mixology/version_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2018 Sébastien Eustace
 # SPDX-License-Identifier: MIT License
-# SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileContributor: 2022-2024 Espressif Systems (Shanghai) CO LTD
 
 import logging
 import time
-
-try:
-    from typing import Dict, List, Optional, Set, Union
-except ImportError:
-    pass
+import typing as t
 
 from .constraint import Constraint
 from .failure import SolverFailure
 from .incompatibility import Incompatibility
 from .incompatibility_cause import ConflictCause, NoVersionsCause, RootCause
 from .package import Package
 from .package_source import PackageSource
@@ -35,29 +30,29 @@
 
     See https://github.com/dart-lang/pub/tree/master/doc/solver.md for details
     on how this solver works.
     """
 
     def __init__(
         self,
-        source,  # type: PackageSource
+        source: PackageSource,
     ):
         self._source = source
 
-        self._incompatibilities = {}  # type: Dict[Package, List[Incompatibility]]
+        self._incompatibilities: t.Dict[Package, t.List[Incompatibility]] = {}
         self._solution = PartialSolution()
 
     @property
-    def solution(self):  # type: () -> PartialSolution
+    def solution(self) -> PartialSolution:
         return self._solution
 
-    def is_solved(self):  # type: () -> bool
+    def is_solved(self) -> bool:
         return not self._solution.unsatisfied
 
-    def solve(self):  # type: () -> SolverResult
+    def solve(self) -> SolverResult:
         """
         Finds a set of dependencies that match the root package's constraints,
         or raises an error if no such set is available.
         """
         start = time.time()
 
         self._add_incompatibility(
@@ -66,36 +61,36 @@
         self._propagate(self._source.root)
 
         while not self.is_solved():
             if not self._run():
                 break
 
         logger.info('Version solving took {:.3f} seconds.\n'.format(time.time() - start))
-        logger.info('Tried {} solutions.'.format(self._solution.attempted_solutions))
+        logger.info(f'Tried {self._solution.attempted_solutions} solutions.')
 
         return SolverResult(self._solution.decisions, self._solution.attempted_solutions)
 
-    def _run(self):  # type: () -> bool
+    def _run(self) -> bool:
         if self.is_solved():
             return False
 
         next_package = self._choose_package_version()
         self._propagate(next_package)
 
         if self.is_solved():
             return False
 
         return True
 
-    def _propagate(self, package):  # type: (Package) -> None
+    def _propagate(self, package: Package) -> None:
         """
         Performs unit propagation on incompatibilities transitively
         related to package to derive new assignments for _solution.
         """
-        changed = set()  # type: Set[Package]
+        changed: t.Set[Package] = set()
         changed.add(package)
 
         while changed:
             package = changed.pop()
             # Iterate in reverse because conflict resolution tends to produce more
             # general incompatibilities as time goes on. If we look at those first,
             # we can derive stronger assignments sooner and more eagerly find
@@ -119,16 +114,16 @@
                     changed.clear()
                     changed.add(self._propagate_incompatibility(root_cause))
                     break
                 elif result is not None:
                     changed.add(result)
 
     def _propagate_incompatibility(
-        self, incompatibility
-    ):  # type: (Incompatibility) -> Union[Package, _conflict, None]
+        self, incompatibility: Incompatibility
+    ) -> t.Union[Package, object, None]:
         """
         If incompatibility is almost satisfied by _solution, adds the
         negation of the unsatisfied term to _solution.
 
         If incompatibility is satisfied by _solution, returns _conflict. If
         incompatibility is almost satisfied by _solution, returns the
         unsatisfied term's package.
@@ -160,35 +155,35 @@
                 unsatisfied = term
 
         # If *all* terms in incompatibility are satisfied by _solution, then
         # incompatibility is satisfied and we have a conflict.
         if unsatisfied is None:
             return _conflict
 
-        logger.info('derived: {}'.format(unsatisfied.inverse))
+        logger.info(f'derived: {unsatisfied.inverse}')
 
         self._solution.derive(
             unsatisfied.constraint, not unsatisfied.is_positive(), incompatibility
         )
 
         return unsatisfied.package
 
-    def _resolve_conflict(self, incompatibility):  # type: (Incompatibility) -> Incompatibility
+    def _resolve_conflict(self, incompatibility: Incompatibility) -> Incompatibility:
         """
         Given an incompatibility that's satisfied by _solution,
         The `conflict resolution`_ constructs a new incompatibility that encapsulates the root
         cause of the conflict and backtracks _solution until the new
         incompatibility will allow _propagate() to deduce new assignments.
 
         Adds the new incompatibility to _incompatibilities and returns it.
 
         .. _conflict resolution:
         https://github.com/dart-lang/pub/tree/master/doc/solver.md#conflict-resolution
         """
-        logger.info('conflict: {}'.format(incompatibility))
+        logger.info(f'conflict: {incompatibility}')
 
         new_incompatibility = False
         while not incompatibility.is_failure():
             # The term in incompatibility.terms that was most recently satisfied by
             # _solution.
             most_recent_term = None
 
@@ -296,20 +291,20 @@
             partially = '' if difference is None else ' partially'
             bang = '!'
             logger.info(
                 '{} {} is{} satisfied by {}'.format(
                     bang, most_recent_term, partially, most_recent_satisfier
                 )
             )
-            logger.info('{} which is caused by "{}"'.format(bang, most_recent_satisfier.cause))
-            logger.info('{} thus: {}'.format(bang, incompatibility))
+            logger.info(f'{bang} which is caused by "{most_recent_satisfier.cause}"')
+            logger.info(f'{bang} thus: {incompatibility}')
 
         raise SolverFailure(incompatibility)
 
-    def _next_term_to_try(self):  # type: () -> Optional[Term]
+    def _next_term_to_try(self) -> t.Optional[Term]:
         unsatisfied = self._solution.unsatisfied
         if not unsatisfied:
             return
 
         # Prefer packages with as few remaining versions as possible,
         # so that if a conflict is necessary it's forced quickly.
         def _get_min(_term):
@@ -318,15 +313,15 @@
         if len(unsatisfied) == 1:
             term = unsatisfied[0]
         else:
             term = min(*unsatisfied, key=_get_min)
 
         return term
 
-    def _choose_package_version(self):  # type: () -> Optional[Package]
+    def _choose_package_version(self) -> t.Optional[Package]:
         """
         Tries to select a version of a required package.
 
         Returns the name of the package whose incompatibilities should be
         propagated by _propagate(), or None indicating that version solving is
         complete and a solution has been found.
         """
@@ -348,29 +343,27 @@
             self._add_incompatibility(incompatibility)
 
             # If an incompatibility is already satisfied, then selecting version
             # would cause a conflict.
             #
             # We'll continue adding its dependencies, then go back to
             # unit propagation which will guide us to choose a better version.
-            conflict = conflict or all(
-                [
-                    iterm.package == term.package or self._solution.satisfies(iterm)
-                    for iterm in incompatibility.terms
-                ]
-            )
+            conflict = conflict or all([
+                iterm.package == term.package or self._solution.satisfies(iterm)
+                for iterm in incompatibility.terms
+            ])
 
         if not conflict:
             self._solution.decide(term.package, version)
-            logger.info('selecting {} ({})'.format(term.package, str(version)))
+            logger.info(f'selecting {term.package} ({str(version)})')
 
         return term.package
 
-    def _add_incompatibility(self, incompatibility):  # type: (Incompatibility) -> None
-        logger.info('fact: {}'.format(incompatibility))
+    def _add_incompatibility(self, incompatibility: Incompatibility) -> None:
+        logger.info(f'fact: {incompatibility}')
 
         for term in incompatibility.terms:
             if term.package not in self._incompatibilities:
                 self._incompatibilities[term.package] = []
 
             if incompatibility in self._incompatibilities[term.package]:
                 continue
```

### Comparing `idf_component_manager-1.5.2/idf_component_manager/version_solver/version_solver.py` & `idf_component_manager-2.0.0.dev0/idf_component_manager/version_solver/version_solver.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,60 @@
 # SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import os
+import typing as t
 
-from idf_component_tools.errors import DependencySolveError, FetchingError, SolverError
+from idf_component_manager.utils import print_info
+from idf_component_tools.errors import DependencySolveError, SolverError
 from idf_component_tools.manifest import (
     ComponentRequirement,
-    ComponentWithVersions,
     Manifest,
-    ProjectRequirements,
+    SolvedComponent,
+    SolvedManifest,
 )
-from idf_component_tools.manifest.solved_component import SolvedComponent
-from idf_component_tools.manifest.solved_manifest import SolvedManifest
-from idf_component_tools.registry.api_client_errors import ComponentNotFound
-from idf_component_tools.sources import BaseSource, LocalSource
+from idf_component_tools.sources import LocalSource, WebServiceSource
+from idf_component_tools.utils import ProjectRequirements
 
-from ..utils import print_info, print_warn
 from .helper import PackageSource
 from .mixology.package import Package
 from .mixology.version_solver import VersionSolver as Solver
 
-try:
-    from typing import Callable
-except ImportError:
-    pass
 
-
-class VersionSolver(object):
+class VersionSolver:
     """
     The version solver that finds a set of package versions
     satisfies the root package's dependencies.
     """
 
-    def __init__(self, requirements, old_solution=None, component_solved_callback=None):
-        # type:(ProjectRequirements, SolvedManifest | None, Callable[[], None] | None) -> None
+    def __init__(
+        self,
+        requirements: ProjectRequirements,
+        old_solution: t.Optional[SolvedManifest] = None,
+        component_solved_callback: t.Optional[t.Callable[[], None]] = None,
+    ) -> None:
         self.requirements = requirements
         self.old_solution = old_solution
         self.component_solved_callback = component_solved_callback
 
         self._source = PackageSource()
         self._solver = Solver(self._source)
         self._target = None
-        self._overriders = set()  # type: set[str]
-        self._local_root_requirements = dict()  # type: dict[str, ComponentRequirement]
-        self._solved_requirements = set()  # type: set[ComponentRequirement]
+        self._overriders: t.Set[str] = set()
+        self._local_root_requirements: t.Dict[str, ComponentRequirement] = dict()
+        self._solved_requirements: t.Set[ComponentRequirement] = set()
 
-    def solve(self):  # type: () -> SolvedManifest
+    def solve(self) -> SolvedManifest:
         # scan all root local requirements
         # root local requirements defined in the file system manifest files
         # would have higher priorities
 
         # scan all root local requirements
         for manifest in self.requirements.manifests:
-            for requirement in manifest.dependencies:  # type: ComponentRequirement
+            for requirement in manifest.requirements:
                 if isinstance(requirement.source, LocalSource):
                     _recorded_requirement = self._local_root_requirements.get(
                         requirement.build_name
                     )
                     if _recorded_requirement:
                         # can't specify two different root local source dependencies
                         if _recorded_requirement.source.hash_key != requirement.source.hash_key:
@@ -67,119 +65,114 @@
                             )
                     else:
                         self._local_root_requirements[requirement.build_name] = requirement
 
         # scan all root local components
         for manifest in self.requirements.manifests[1:]:
             # add itself as highest priority component
-            if manifest.name and manifest.version and manifest._manifest_manager:
-                _source = LocalSource({'path': os.path.dirname(manifest._manifest_manager.path)})
+            if manifest.real_name and manifest.version and manifest._manifest_manager:
+                _source = LocalSource(
+                    path=os.path.dirname(manifest.path),
+                    manifest_manager=manifest._manifest_manager,
+                )
                 self._source.add(
-                    Package(manifest.name, _source),
+                    Package(manifest.real_name, _source),
                     str(manifest.version),
                     deps=self._component_dependencies_with_local_precedence(
-                        manifest.dependencies, manifest.name
+                        manifest.requirements, manifest.real_name
                     ),
                 )
 
-                self._local_root_requirements[manifest.name] = ComponentRequirement(
-                    name=manifest.name,
-                    sources=[_source],
-                    version_spec=str(manifest.version),
+                self._local_root_requirements[manifest.real_name] = ComponentRequirement(
+                    name=manifest.real_name,
+                    path=os.path.dirname(manifest.path),
+                    version=str(manifest.version),
+                    manifest_manager=manifest._manifest_manager,
                 )
 
         for manifest in self.requirements.manifests:
             self.solve_manifest(manifest)
 
         self._source.override_dependencies(self._overriders)
 
         result = self._solver.solve()
 
         solved_components = []
         for package, version in result.decisions.items():
             if package == Package.root():
                 continue
-            kwargs = {'name': package.name, 'source': package.source, 'version': version}
+
+            kwargs = {
+                'name': package.name,
+                'source': package.source,
+                'version': version.version,
+                'dependencies': version.dependencies,
+            }
             if package.source.component_hash_required:
                 kwargs['component_hash'] = version.component_hash
+
             if version.targets:
                 kwargs['targets'] = version.targets
-            solved_components.append(SolvedComponent(**kwargs))  # type: ignore
-        return SolvedManifest(
-            solved_components, self.requirements.manifest_hash, self.requirements.target
-        )
 
-    def get_versions_from_sources(
-        self, requirement
-    ):  # type: (ComponentRequirement) -> tuple[ComponentWithVersions | None, BaseSource | None]
-        latest_source = None
-        cmp_with_versions = None
-        for source in requirement.sources:
-            try:
-                cmp_with_versions = source.versions(
-                    name=requirement.name,
-                    spec=requirement.version_spec,
-                    target=self.requirements.target,
-                )
-                latest_source = source
-                if cmp_with_versions.versions:
-                    break
-            # ComponentNotFound will be raised by API client
-            # FetchingError will be raised by sources
-            except (ComponentNotFound, FetchingError):
-                pass
-        return cmp_with_versions, latest_source
+            if isinstance(package.source, WebServiceSource):
+                kwargs['download_url'] = version.download_url
+
+            solved_components.append(SolvedComponent.fromdict(kwargs))
+
+        return SolvedManifest.fromdict({
+            'direct_dependencies': self.requirements.direct_dep_names or None,
+            'dependencies': solved_components,
+            'manifest_hash': self.requirements.manifest_hash,
+            'target': self.requirements.target,
+        })
 
-    def solve_manifest(self, manifest):  # type: (Manifest) -> None
+    def solve_manifest(self, manifest: Manifest) -> None:
         for dep in self._dependencies_with_local_precedence(
-            manifest.dependencies, manifest_path=manifest.path
+            manifest.requirements, manifest_path=manifest.path
         ):
-            if len(dep.sources) == 1:
-                source = dep.source
-            else:
-                _, source = self.get_versions_from_sources(dep)
-
-            self._source.root_dep(Package(dep.name, source), dep.version_spec)
+            self._source.root_dep(Package(dep.name, dep.source), dep.version_spec)
             try:
                 self.solve_component(dep, manifest_path=manifest.path)
             except DependencySolveError as e:
                 raise SolverError(
                     'Solver failed processing dependency "{dependency}" '
                     'from the manifest file "{path}".\n{original_error}'.format(
                         path=manifest.path, dependency=e.dependency, original_error=str(e)
                     )
                 )
             except SolverError as e:
                 raise SolverError(
-                    'Solver failed processing manifest file "{path}".'
-                    '\n{original_error}'.format(path=manifest.path, original_error=str(e))
+                    'Solver failed processing manifest file "{path}".' '\n{original_error}'.format(
+                        path=manifest.path, original_error=str(e)
+                    )
                 )
 
     def solve_component(
-        self, requirement, manifest_path=None
-    ):  # type: (ComponentRequirement, str | None) -> None
+        self, requirement: ComponentRequirement, manifest_path: t.Optional[str] = None
+    ) -> None:
         if requirement in self._solved_requirements:
             return
 
-        cmp_with_versions, source = self.get_versions_from_sources(requirement)
+        cmp_with_versions = requirement.source.versions(
+            name=requirement.name, spec=requirement.version_spec, target=self.requirements.target
+        )
 
-        if not cmp_with_versions or not cmp_with_versions.versions or not source:
-            print_warn('Component "{}" not found'.format(requirement.name))
+        if not cmp_with_versions or not cmp_with_versions.versions:
             return
 
         for version in cmp_with_versions.versions:
-            if source.is_overrider:
+            if requirement.source.is_overrider:
                 self._overriders.add(requirement.build_name)
 
             deps = self._component_dependencies_with_local_precedence(
                 version.dependencies, component_name=requirement.name, manifest_path=manifest_path
             )
 
             self._source.add(
-                Package(requirement.name, source),
+                Package(requirement.name, requirement.source),
                 version,
                 deps=deps,
             )
 
             if version.dependencies:
                 for dep in version.dependencies:
                     self.solve_component(dep)
@@ -187,35 +180,33 @@
         self._solved_requirements.add(requirement)
 
         if self.component_solved_callback:
             self.component_solved_callback()
 
     def _dependencies_with_local_precedence(
         self,
-        dependencies,  # type: list[ComponentRequirement]
-        component_name=None,  # type: str | None
-        manifest_path=None,  # type: str | None
-    ):  # type: (...) -> list[ComponentRequirement]
-        deps = []  # type: list[ComponentRequirement]
+        dependencies: t.List[ComponentRequirement],
+        component_name: t.Optional[str] = None,
+        manifest_path: t.Optional[str] = None,
+    ) -> t.List[ComponentRequirement]:
+        deps: t.List[ComponentRequirement] = []
         for dep in dependencies:
             # replace version dependencies to local one if exists
             # use build_name in both recording and replacing
             matching_dep_name = None
             if dep.build_name in self._local_root_requirements:
                 matching_dep_name = dep.build_name
             elif dep.short_name in self._local_root_requirements:
                 matching_dep_name = dep.short_name
 
             if not matching_dep_name:
                 deps.append(dep)
                 continue
 
-            component_path = self._local_root_requirements[
-                matching_dep_name
-            ].source._path  # type: ignore
+            component_path = self._local_root_requirements[matching_dep_name].source._path  # type: ignore
 
             print_info(
                 'Using component placed at {path} '
                 'for dependency {dep}{introduced_by}{specified_in}'.format(
                     # must be a local source here
                     path=component_path,
                     dep=dep,
@@ -227,19 +218,19 @@
             )
             deps.append(self._local_root_requirements[matching_dep_name])
 
         return deps
 
     def _component_dependencies_with_local_precedence(
         self,
-        dependencies,  # type: list[ComponentRequirement]
-        component_name=None,  # type: str | None
-        manifest_path=None,  # type: str | None
-    ):  # type: (...) -> dict[Package, str]
-        deps = {}  # type: dict[Package, str]
+        dependencies: t.List[ComponentRequirement],
+        component_name: t.Optional[str] = None,
+        manifest_path: t.Optional[str] = None,
+    ) -> t.Dict[Package, str]:
+        deps: t.Dict[Package, str] = {}
         for dep in self._dependencies_with_local_precedence(
             dependencies,
             component_name,
             manifest_path,
         ):
             deps[Package(dep.name, dep.source)] = dep.version_spec
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/archive_tools.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/archive_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 """Set of tools to work with archives"""
 
 import re
 import tarfile
+import typing as t
 from pathlib import Path
 from shutil import get_archive_formats
 
 from .errors import FatalError
 from .file_tools import prepare_empty_directory
 
-try:
-    from typing import Text, Union
-except ImportError:
-    pass
-
 
 class ArchiveError(FatalError):
     pass
 
 
 KNOWN_MIME_TYPES = [
     'application/x-tar',
@@ -51,15 +47,15 @@
     elif re.search(r'(\.tar\.bz2$)|(\.tbz2$)', path):
         return ('bztar', 'tbz2', unpack_tar)
     elif re.search(r'(\.tar\.xz$)|(\.txz$)', path):
         return ('xztar', 'txz', unpack_tar)
     elif path.endswith('.tar'):
         return ('tar', 'tar', unpack_tar)
     else:
-        raise ArchiveError('Unknown archive extension for path: %s' % path)
+        raise ArchiveError(f'Unknown archive extension for path: {path}')
 
 
 def is_known_format(fmt):
     for known_format in get_archive_formats():
         if fmt == known_format[0]:
             return True
 
@@ -68,44 +64,44 @@
 
 def unpack_tar(file, destination_directory):
     """Unpack .(tar.|t)(xz|gz|bz2) file"""
     try:
         tar = tarfile.open(file)
         prepare_empty_directory(destination_directory)
     except tarfile.TarError:
-        raise ArchiveError('%s is not a valid tar archive' % file)
+        raise ArchiveError(f'{file} is not a valid tar archive')
 
     try:
-        tar.extractall(destination_directory)
+        tar.extractall(destination_directory)  # noqa: S202
     finally:
         tar.close()
 
 
 def unpack_zip(file, destination_directory):
     """Unpack zip file"""
     import zipfile
 
     if not zipfile.is_zipfile(file):
-        raise ArchiveError('%s is not a zip file' % file)
+        raise ArchiveError(f'{file} is not a zip file')
 
     prepare_empty_directory(destination_directory)
 
     with zipfile.ZipFile(file) as archive:
         for item in archive.infolist():
             archive.extract(item, destination_directory)
 
 
-def unpack_archive(file, destination_directory):  # type: (Union[Text, Path], Text) -> None
+def unpack_archive(file: t.Union[str, Path], destination_directory: str) -> None:
     prepare_empty_directory(destination_directory)
     archive_format, ext, handler = get_format_from_path(file)
     if not is_known_format(archive_format):
-        raise ArchiveError('.%s files are not supported on your system' % ext)
+        raise ArchiveError(f'.{ext} files are not supported on your system')
     handler(file, destination_directory)
 
 
-def pack_archive(source_dir, archive_filepath):  # type: (Union[Text, Path], Text) -> None
+def pack_archive(source_dir: t.Union[str, Path], archive_filepath: str) -> None:
     """Create tar+gzip archive"""
     try:
         with tarfile.open(archive_filepath, 'w:gz') as archive:
             archive.add(source_dir, arcname='')
     except tarfile.TarError:
-        raise ArchiveError('%s is not a valid tar archive' % archive_filepath)
+        raise ArchiveError(f'{archive_filepath} is not a valid tar archive')
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/build_system_tools.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/build_system_tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,107 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
-'''Tools for interaction with IDF build system'''
+"""Tools for interaction with IDF build system"""
+
 import os
 import re
-import subprocess  # nosec
+import subprocess  # noqa: S404
 import sys
 from pathlib import Path
 
-from idf_component_tools.errors import FetchingError, ProcessingError
+from idf_component_tools.errors import RunningEnvironmentError
 
 from .semver import Version
 
 IDF_VERSION_REGEX = re.compile(r'v(\d\.\d(?:\.\d)?)')
 
 CMAKE_PROJECT_LINE = r'include($ENV{IDF_PATH}/tools/cmake/project.cmake)'
 
 
 def build_name(name):
     name_parts = name.split('/')
     return '__'.join(name_parts)
 
 
-def get_env_idf_target():  # type: () -> str
+def get_env_idf_target() -> str:
     """
     `IDF_TARGET` should be set automatically while compiling with cmake
     """
     env_idf_target = os.getenv('IDF_TARGET')
     if not env_idf_target:
-        raise ProcessingError(
+        raise RunningEnvironmentError(
             'IDF_TARGET is not set, should be set by CMake, please check your configuration'
         )
     return env_idf_target
 
 
 def get_idf_version():
     idf_version = os.getenv('IDF_VERSION')
     if idf_version:
         return idf_version
 
     idf_py_path = os.path.join(get_idf_path(), 'tools', 'idf.py')
     try:
-        idf_version = subprocess.check_output([sys.executable, idf_py_path, '--version'])  # nosec
+        idf_version = subprocess.check_output([sys.executable, idf_py_path, '--version'])  # noqa: S603
     except subprocess.CalledProcessError:
-        raise FetchingError(
-            'Could not get IDF version from calling "idf.py --version".\n'
-            'idf.py path: {}'.format(idf_py_path)
+        raise RunningEnvironmentError(
+            'Could not get IDF version from calling "idf.py --version".\n' 'idf.py path: {}'.format(
+                idf_py_path
+            )
         )
     else:
         try:
             string_type = basestring  # type: ignore
         except NameError:
             string_type = str
 
         if not isinstance(idf_version, string_type):
             idf_version = idf_version.decode('utf-8')
 
     res = IDF_VERSION_REGEX.findall(idf_version)
     if len(res) == 1:
         return str(Version.coerce(res[0]))
     else:
-        raise FetchingError(
-            'Could not parse IDF version from calling "idf.py --version".\n'
-            'Output: {}'.format(idf_version)
+        raise RunningEnvironmentError(
+            'Could not parse IDF version from calling "idf.py --version".\n' 'Output: {}'.format(
+                idf_version
+            )
         )
 
 
-def get_idf_path():  # type: () -> str
+def get_idf_path() -> str:
     try:
         return os.environ['IDF_PATH']
     except KeyError:
-        raise FetchingError('Please set IDF_PATH environment variable with a valid path to ESP-IDF')
+        raise RunningEnvironmentError(
+            'Please set IDF_PATH environment variable with a valid path to ESP-IDF'
+        )
 
 
-def is_component(path):  # type: (Path) -> bool
-    '''
+def is_component(path: Path) -> bool:
+    """
     This function is used in the manifest processing to determine,
     if the given path is a component or not.
     If the directory on the path:
         - Does not contain CMakeLists.txt, it is not considered as a component
         (nor a project).
         - Contains idf_component.yml, it is considered as a component, as projects
         do not contain it.
         - Contains CMakeLists.txt and this file contains CMAKE_PROJECT_LINE,
         it is considered as a project, otherwise it is considered as a component.
     Note that this function may be adequate only for the manifest processing.
-    '''
+    """
 
     cmakelists_path = path / 'CMakeLists.txt'
 
     if not cmakelists_path.exists():
         return False
 
     if (path / 'idf_component.yml').exists():
         return True
 
-    with open((str(cmakelists_path)), 'r') as f:
+    with open(str(cmakelists_path)) as f:
         for line in f:
             if CMAKE_PROJECT_LINE in line:
                 return False
 
     return True
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/constants.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,27 @@
-# SPDX-FileCopyrightText: 2018-2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2018-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 #
 # Contains elements taken from "is-git-url" github repository
 # https://github.com/jonschlinkert/is-git-url
 # Copyright (c) 2017, Jon Schlinkert.
 # Originally released under the MIT License.
 
 import re
 import sys
 
-URL_RE = (
-    r'^https?://'  # http:// or https://
-    r'(?:(?:[A-Za-z0-9](?:[A-Za-z0-9-]{0,61}[A-Za-z0-9])?\.)+'
-    r'(?:[A-Za-z]{2,6}\.?|[A-Za-z0-9-]{2,}\.?)|'  # domain
-    r'localhost|'  # or localhost
-    r'\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})'  # or ip
-    r'(?::\d+)?'  # optional port
-    r'(?:/?|[/?]\S+)$'
-)
-COMPILED_URL_RE = re.compile(URL_RE, re.IGNORECASE)
-
 GIT_URL_RE = r'^(?:git|ssh|https?|git@[-\w.]+):(\/\/)?(.*)(\.git)?(/?|#[-\d\w._]+?)$'
 COMPILED_GIT_URL_RE = re.compile(GIT_URL_RE, re.IGNORECASE)
-
-FILE_RE = (
-    r'^file://'  # file URI
-    r'([A-Za-z]:\\\\(?:[^\\/:*?\"<>|\r\n]+\\)*$|'  # Windows path
-    r'\/.*$)$'  # Unix path
-)
-COMPILED_FILE_RE = re.compile(FILE_RE, re.IGNORECASE)
+COMMIT_ID_RE = r'[0-9a-f]{40}'
+COMPILED_COMMIT_ID_RE = re.compile(COMMIT_ID_RE)
 
 # Registry related constants
 DEFAULT_NAMESPACE = 'espressif'
 IDF_COMPONENT_REGISTRY_URL = 'https://components.espressif.com/'
 IDF_COMPONENT_STORAGE_URL = 'https://components-file.espressif.com/'
 
 UPDATE_SUGGESTION = """
 SUGGESTION: This component may be using a newer version of the component manager.
 You can try to update the component manager by running:
     {} -m pip install --upgrade idf-component-manager
-""".format(
-    sys.executable
-)
+""".format(sys.executable)
+MANIFEST_FILENAME = 'idf_component.yml'
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/environment.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/environment.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: 2023-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
-'''
+"""
 This module contains utility functions for working with environment variables.
-'''
+"""
 
 import os
+import typing as t
 
 KNOWN_CI_ENVIRONMENTS = {
     'GITHUB_ACTIONS': 'github-actions',
     'GITLAB_CI': 'gitlab-ci',
     'CIRCLECI': 'circle-ci',
     'TRAVIS': 'travis',
     'JENKINS_URL': 'jenkins',
@@ -17,49 +18,49 @@
     'BITBUCKET_COMMIT': 'bitbucket-pipelines',
     'SEMAPHORE': 'semaphore',
     'TEAMCITY_VERSION': 'teamcity',
     'CI': 'unknown',
 }
 
 
-def getenv_int(name, default):  # type: (str, int) -> int
-    '''
+def getenv_int(name: str, default: int) -> int:
+    """
     Returns environment variable as an integer, or default if not set.
     Raises ValueError if not an integer.
-    '''
+    """
 
     try:
         return int(os.environ.get(name, default))
     except ValueError:
-        raise ValueError('Environment variable "{}" must contain a numeric value'.format(name))
+        raise ValueError(f'Environment variable "{name}" must contain a numeric value')
 
 
-def getenv_bool(name, default=False):  # type: (str, bool) -> bool
-    '''Returns True if environment variable is set to 1, t, y, yes, true, or False otherwise'''
+def getenv_bool(name: str, default: bool = False) -> bool:
+    """Returns True if environment variable is set to 1, t, y, yes, true, or False otherwise"""
 
     return os.getenv(name, str(default)).lower() in {'1', 't', 'true', 'y', 'yes'}
 
 
-def getenv_bool_or_string(name, default=False):  # type: (str, bool | str) -> bool | str
-    '''Returns
+def getenv_bool_or_string(name: str, default: t.Union[bool, str] = False) -> t.Union[bool, str]:
+    """Returns
     - True if environment variable is set to 1, t, y, yes, true,
     - False if environment variable is set to 0, f, n, no, false
     - or the string value otherwise
-    '''
+    """
 
     value = os.getenv(name, str(default))
     if value.lower() in {'1', 't', 'true', 'y', 'yes'}:
         return True
     elif value.lower() in {'0', 'f', 'false', 'n', 'no'}:
         return False
     else:
         return value
 
 
-def detect_ci():  # type: () ->  str | None
-    '''Returns the name of CI environment if running in a CI environment'''
+def detect_ci() -> t.Optional[str]:
+    """Returns the name of CI environment if running in a CI environment"""
 
     for env_var, name in KNOWN_CI_ENVIRONMENTS.items():
         if os.environ.get(env_var):
             return name
 
     return None
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/errors.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 
-try:
-    from typing import Any
-except ImportError:
-    pass
+import typing as t
 
 
 class FatalError(RuntimeError):
     """Generic unrecoverable runtime error"""
 
     exit_code = 2
 
-    def __init__(self, *args, **kwargs):  # type: (Any, Any) -> None
-        super(FatalError, self).__init__(*args)
+    def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
+        super().__init__(*args)
         exit_code = kwargs.pop('exit_code', None)
         if exit_code:
             self.exit_code = exit_code
 
 
 class InternalError(RuntimeError):
     """Internal Error, should report to us"""
 
-    def __init__(self):
-        super(InternalError, self).__init__(
+    def __init__(self, extra_msg: t.Optional[str] = None):
+        err = (
             'This is an internal error. Please report on '
             '`https://github.com/espressif/idf-component-manager/issues '
             'with your operating system, idf-component-manager version, '
             'and the traceback log. Thanks for reporting! '
         )
 
+        if extra_msg:
+            err = extra_msg + '\n' + err
+
+        super().__init__(err)
+
 
 class NothingToDoError(FatalError):
-    '''Generic Runtime error for states when operation is prematurely
-    aborted due to nothing to do'''
+    """Generic Runtime error for states when operation is prematurely
+    aborted due to nothing to do"""
 
     exit_code = 144  # NOP
 
 
 class SolverError(FatalError):
     pass
 
@@ -71,25 +73,29 @@
 
 class MetadataError(ProcessingError):
     pass
 
 
 class MetadataKeyError(ProcessingError):
     def __init__(self, field_name, field_type):
-        super(MetadataKeyError, self).__init__(
+        super().__init__(
             'Unknown {} field "{}" in the manifest file that may affect build result'.format(
                 field_type, field_name
             )
         )
 
 
 class LockError(ProcessingError):
     pass
 
 
+class LockVersionMismatchError(LockError):
+    pass
+
+
 class GitError(ProcessingError):
     pass
 
 
 class ComponentModifiedError(ProcessingError):
     pass
 
@@ -102,13 +108,13 @@
     pass
 
 
 class VersionAlreadyExistsError(FatalError):
     pass
 
 
-class ProfileNotValid(FatalError):
+class SyncError(FatalError):
     pass
 
 
-class SyncError(FatalError):
+class RunningEnvironmentError(FatalError):
     pass
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/file_cache.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/file_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-# SPDX-FileCopyrightText: 2019-2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2019-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 #
 # Contains elements taken from "appdirs" python package
 # https://github.com/ActiveState/appdirs/tree/1.4.3
 # Copyright (c) 2005-2010 ActiveState Software Inc.
 # Copyright (c) 2013 Eddy Petrisor
 # Originally released under MIT license
 """Classes to work with file cache"""
 
 import errno
 import os
 import shutil
 import sys
+import typing as t
 
 from idf_component_tools.errors import FatalError
 from idf_component_tools.file_tools import directory_size
 
 
-def system_cache_path():  # type: () -> str
+def system_cache_path() -> str:
     """Path of system cache directory"""
     system_cache_path = SystemCachePath()
 
     if sys.platform.startswith('win'):
         cache_directory = system_cache_path.cache_path_win()
         return os.path.join(cache_directory, 'Espressif', 'ComponentManager', 'Cache')
     else:
@@ -29,46 +30,46 @@
             cache_directory = system_cache_path.cache_path_macos()
         else:
             cache_directory = system_cache_path.cache_path_unix()
 
         return os.path.join(cache_directory, 'Espressif', 'ComponentManager')
 
 
-class FileCache(object):
+class FileCache:
     """Common functions to work with components cache"""
 
-    def __init__(self, path=None):  # type: (str | None) -> None
-        self._path = path  # type: str | None
+    def __init__(self, path: t.Optional[str] = None) -> None:
+        self._path: t.Optional[str] = path
 
-    def path(self):  # type: () -> str
+    def path(self) -> str:
         """Path of cache directory. Make directory if it doesn't exist"""
         if not self._path:
             self._path = os.getenv('IDF_COMPONENT_CACHE_PATH')
 
         if not self._path:
             self._path = system_cache_path()
 
         try:
             os.makedirs(self._path)
         except OSError as e:
             if e.errno != errno.EEXIST:
-                raise FatalError('Failed to create cache directory: {}'.format(self._path))
+                raise FatalError(f'Failed to create cache directory: {self._path}')
 
         return self._path
 
-    def clear(self):  # type: () -> None
-        '''Clear cache directory'''
+    def clear(self) -> None:
+        """Clear cache directory"""
         shutil.rmtree(self.path())
 
-    def size(self):  # type: () -> int
+    def size(self) -> int:
         """Disk usage of cache directory"""
         return directory_size(self.path())
 
 
-class SystemCachePath(object):
+class SystemCachePath:
     """Methods to fetch user specific cache path for every platform"""
 
     PY3 = sys.version_info[0] == 3
 
     def _get_win_folder_from_registry(self):
         """This is a fallback technique at best. I'm not sure if using the
         registry for this guarantees us the correct answer for all CSIDL_*
@@ -81,15 +82,15 @@
 
         shell_folder_name = 'Local AppData'
 
         key = _winreg.OpenKey(
             _winreg.HKEY_CURRENT_USER,
             r'Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders',
         )
-        dir, type = _winreg.QueryValueEx(key, shell_folder_name)
+        dir, _ = _winreg.QueryValueEx(key, shell_folder_name)
         return dir
 
     def _get_win_folder_with_pywin32(self):
         from win32com.shell import shell, shellcon
 
         dir = shell.SHGetFolderPath(0, getattr(shellcon, 'CSIDL_LOCAL_APPDATA'), 0, 0)
         # Try to make this a unicode path because SHGetFolderPath does
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/file_tools.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/file_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
-"""Set of tools and constants to work with files and directories """
+"""Set of tools and constants to work with files and directories"""
+
 import os
 import shutil
+import typing as t
 from pathlib import Path
 from shutil import copytree, rmtree
 
 from idf_component_tools.messages import warn
 
-try:
-    from typing import Iterable
-except ImportError:
-    pass
-
 DEFAULT_EXCLUDE = [
     # Python files
     '**/__pycache__',
     '**/*.pyc',
     '**/*.pyd',
     '**/*.pyo',
     # macOS files
     '**/.DS_Store',
     # Git
     '**/.git/**/*',
     # SVN
     '**/.svn/**/*',
-    # dist and build artefacts
+    # dist and build artifacts
     '**/dist/**/*',
     '**/build/**/*',
+    # idf-build-apps artifacts
+    '**/build_*/**/*',
     # artifacts from example projects
     '**/managed_components/**/*',
     '**/dependencies.lock',
     # CI files
     '**/.github/**/*',
     '**/.gitlab-ci.yml',
     # IDE files
@@ -47,30 +46,29 @@
 
 UNEXPECTED_FILES = {
     'CMakeCache.txt',
 }
 
 
 def filtered_paths(
-    path,  # type: str | Path
-    include=None,  # type: Iterable[str] | None
-    exclude=None,  # type: Iterable[str] | None
-    exclude_default=True,  # type: bool
-):
-    # type: (...) -> set[Path]
+    path: t.Union[str, Path],
+    include: t.Optional[t.Iterable[str]] = None,
+    exclude: t.Optional[t.Iterable[str]] = None,
+    exclude_default: bool = True,
+) -> t.Set[Path]:
     """Returns set of paths that should be included in component archive"""
 
     if include is None:
         include = set()
 
     if exclude is None:
         exclude = set()
 
     base_path = Path(path)
-    paths = set()  # type: set[Path]
+    paths: t.Set[Path] = set()
 
     def include_paths(pattern):
         paths.update(base_path.glob(pattern))
 
     def exclude_paths(pattern):
         paths.difference_update(base_path.glob(pattern))
 
@@ -91,42 +89,42 @@
     # Include everything that was explicitly added
     for pattern in include:
         include_paths(pattern)
 
     return paths
 
 
-def create_directory(directory):  # type: (str) -> None
+def create_directory(directory: str) -> None:
     """Create directory, if doesn't exist yet"""
     if not os.path.exists(directory):
         os.makedirs(directory)
 
 
-def prepare_empty_directory(directory):  # type: (str) -> None
+def prepare_empty_directory(directory: str) -> None:
     """Prepare directory empty"""
     dir_exist = os.path.exists(directory)
 
     # Delete path if it's not empty
     if dir_exist and os.listdir(directory):
         rmtree(directory)
         dir_exist = False
 
     if not dir_exist:
         os.makedirs(directory)
 
 
-def copy_directory(source_directory, destination_directory):  # type: (str, str) -> None
+def copy_directory(source_directory: str, destination_directory: str) -> None:
     if os.path.exists(destination_directory):
         rmtree(destination_directory)
     copytree(source_directory, destination_directory)
 
 
 def copy_directories(
-    source_directory, destination_directory, paths
-):  # type: (str, str, Iterable[Path]) -> None
+    source_directory: str, destination_directory: str, paths: t.Iterable[Path]
+) -> None:
     for path in sorted(paths):
         path = str(path)  # type: ignore # Path backward compatibility
         rel_path = os.path.relpath(path, source_directory)
         dest_path = os.path.join(destination_directory, rel_path)
 
         if os.path.isfile(path):
             dest_dir = os.path.dirname(dest_path)
@@ -135,48 +133,52 @@
                 os.makedirs(dest_dir)
 
             shutil.copy2(path, dest_path)
         else:
             os.makedirs(dest_path)
 
 
-def copy_filtered_directory(source_directory, destination_directory, include=None, exclude=None):
-    # type: (str, str, Iterable[str] | None, Iterable[str] | None) -> None
+def copy_filtered_directory(
+    source_directory: str,
+    destination_directory: str,
+    include: t.Optional[t.Iterable[str]] = None,
+    exclude: t.Optional[t.Iterable[str]] = None,
+) -> None:
     paths = filtered_paths(source_directory, include=include, exclude=exclude)
     prepare_empty_directory(destination_directory)
     copy_directories(source_directory, destination_directory, paths)
 
 
-def check_unexpected_component_files(path):  # type: (str | Path) -> None
-    '''Create a warning if a directory contains files not expected inside component'''
+def check_unexpected_component_files(path: t.Union[str, Path]) -> None:
+    """Create a warning if a directory contains files not expected inside component"""
     for root, _dirs, files in os.walk(str(path)):
         unexpected_files = UNEXPECTED_FILES.intersection(files)
         if unexpected_files:
             warn(
                 'Unexpected files "{files}" found in the component directory "{path}". '
                 'Please check if these files should be ignored'.format(
                     files=', '.join(unexpected_files), path=os.path.relpath(root, start=str(path))
                 )
             )
 
 
-def directory_size(dir_path):  # type: (str) -> int
-    '''Return the total size of all files in the directory tree'''
+def directory_size(dir_path: str) -> int:
+    """Return the total size of all files in the directory tree"""
     total_size = 0
     directory = Path(dir_path)
     for file in directory.glob('**/*'):
         try:
             total_size += os.stat(str(file)).st_size
         except OSError:
             pass
     return total_size
 
 
-def human_readable_size(size):  # type: (int) -> str
-    '''Return a human readable string representation of a data size'''
+def human_readable_size(size: int) -> str:
+    """Return a human readable string representation of a data size"""
     if size < 0:
         raise ValueError('size must be non-negative')
 
     if size < 1024:
         return '{} bytes'.format(size)
 
     if size < 1024**2:
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/git_client.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/git_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 # SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
 import os
 import re
-import subprocess  # nosec
+import subprocess  # noqa: S404
 import time
+import typing as t
 from datetime import datetime
 from functools import wraps
 
 from .errors import GitError
 from .messages import warn
 from .semver import Version
 
-try:
-    from typing import Any, Callable, Union
-except ImportError:
-    pass
-
 
 class GitCommandError(Exception):
     """
     Exception class for git errors.
 
     Git error that is supposed to be handled in the code in the code of this class,
     not in the user code.
     """
 
-    def __init__(self, *args, **kwargs):  # type: (Any, Any) -> None
+    def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
         self.exit_code = kwargs.get('exit_code')
-        super(GitCommandError, self).__init__(*args)
+        super().__init__(*args)
 
 
-def clean_tag_version(tag):  # type: (str) -> str
+def clean_tag_version(tag: str) -> str:
     """Clean version from tag before processing it"""
     tag = tag.strip()
 
     # Remove leading 'v' from tag
     if tag.startswith('v'):
         tag = tag[1:]
 
     # Replace revision 1.2.3.4 with 1.2.3~4
     tag = re.sub(r'^(\d+\.\d+\.\d+)\.(\d+)', r'\1~\2', tag)
 
     return tag
 
 
-class GitClient(object):
+class GitClient:
     """Set of tools for working with git repos"""
 
     def __init__(
-        self, git_command='git', min_supported='2.0.0'
-    ):  # type: (str, Union[str, Version]) -> None
+        self, git_command: str = 'git', min_supported: t.Union[str, Version] = '2.0.0'
+    ) -> None:
         self.git_command = git_command or 'git'
         self.git_min_supported = (
             min_supported if isinstance(min_supported, Version) else Version(min_supported)
         )
 
         self._git_checked = False
         self._repo_updated = False
 
-    def _git_cmd(func):  # type: (Union[GitClient, Callable[..., Any]]) -> Callable
+    def _git_cmd(func: t.Union[GitClient, t.Callable[..., t.Any]]) -> t.Callable:
         @wraps(func)  # type: ignore
         def wrapper(self, *args, **kwargs):
             if not self._git_checked:
                 self.check_version()
                 self._git_checked = True
 
             try:
@@ -89,55 +86,55 @@
         fetch_file = os.path.join(bare_path, 'FETCH_HEAD')
         current_time = time.mktime(datetime.now().timetuple())
 
         # Don't fetch too often, at most once a minute
         if not os.path.isfile(fetch_file) or current_time - os.stat(fetch_file).st_mtime > 60:
             self.run(['fetch', 'origin'], cwd=bare_path)
 
-    def _bare_repo(func):  # type: (Union[GitClient, Callable[..., Any]]) -> Callable
+    def _bare_repo(func: t.Union[GitClient, t.Callable[..., t.Any]]) -> t.Callable:
         @wraps(func)  # type: ignore
         def wrapper(self, *args, **kwargs):
             if not self._repo_updated:
                 self._update_bare_repo(*args, **kwargs)
                 self._repo_updated = True
 
             return func(self, *args, **kwargs)
 
         return wrapper
 
     @_git_cmd
-    def commit_id(self, path):  # type: (str) -> str
+    def commit_id(self, path: str) -> str:
         return self.run(['show', '--format="%H"', '--no-patch'], cwd=path)
 
     @_git_cmd
-    def is_dirty(self, path):  # type: (str) -> bool
+    def is_dirty(self, path: str) -> bool:
         try:
             self.run(['diff', '--quiet'], cwd=path)
             return False
         except GitCommandError:
             return True
 
     @_git_cmd
-    def is_git_dir(self, path):  # type: (str) -> bool
+    def is_git_dir(self, path: str) -> bool:
         try:
             return self.run(['rev-parse', '--is-inside-work-tree'], cwd=path).strip() == 'true'
         except GitCommandError:
             return False
 
     @_git_cmd
     @_bare_repo
     def prepare_ref(
         self,
-        repo,  # type: str
-        bare_path,  # type: str
-        checkout_path,  # type: str
-        ref=None,  # type: str | None
-        with_submodules=True,  # type: bool
-        selected_paths=None,  # type: list[str] | None
-    ):  # type: (...) -> str
+        repo: str,
+        bare_path: str,
+        checkout_path: str,
+        ref: t.Optional[str] = None,
+        with_submodules: bool = True,
+        selected_paths: t.Optional[t.List[str]] = None,
+    ) -> str:
         """
         Checkout required branch to desired path. Create a bare repo, if necessary
 
         Parameters
         ----------
         repo: str
             URL of the repository
@@ -145,15 +142,15 @@
             Path to the bare repository
         checkout_path: str
             Path to checkout working repository
         ref: str
             Branch name, commit id or '*'
         with_submodules: bool
              If True, submodules will be downloaded
-        selected_paths: List[str]
+        selected_paths: t.List[str]
             List of folders and files that need to download
         Returns
         -------
             Commit id of the current checkout
         """
         commit_id = self.get_commit_id_by_ref(repo, bare_path, ref)
 
@@ -176,59 +173,57 @@
             checkout_command += ['--'] + selected_paths
         self.run(checkout_command)
 
         # And remove all untracked files
         self.run(['--work-tree', checkout_path, '--git-dir', bare_path, 'clean', '--force'])
         # Submodules
         if with_submodules:
-            self.run(
-                [
-                    '--work-tree=.',
-                    '-C',
-                    checkout_path,
-                    '--git-dir',
-                    bare_path,
-                    'submodule',
-                    'update',
-                    '--init',
-                    '--recursive',
-                ]
-            )
+            self.run([
+                '--work-tree=.',
+                '-C',
+                checkout_path,
+                '--git-dir',
+                bare_path,
+                'submodule',
+                'update',
+                '--init',
+                '--recursive',
+            ])
 
         return commit_id
 
     @_git_cmd
     @_bare_repo
-    def get_commit_id_by_ref(self, repo, bare_path, ref):  # type: (str, str, str) -> str
+    def get_commit_id_by_ref(self, repo: str, bare_path: str, ref: str) -> str:
         if ref:
             # If branch is provided check that exists
             try:
                 self.run(['branch', '--contains', ref], cwd=bare_path)
             except GitCommandError:
-                raise GitError('Branch "%s" doesn\'t exist in repo "%s"' % (ref, repo))
+                raise GitError(f'Branch "{ref}" doesn\'t exist in repo "{repo}"')
 
         else:
             # Set to latest commit from remote's HEAD
             ref = self.run(['ls-remote', '--exit-code', 'origin', 'HEAD'], cwd=bare_path)[:40]
 
         return self.run(['rev-parse', '--verify', ref], cwd=bare_path).strip()
 
     @_git_cmd
     @_bare_repo
-    def has_gitmodules_by_ref(self, repo, bare_path, ref):  # type: (str, str, str) -> bool
+    def has_gitmodules_by_ref(self, repo: str, bare_path: str, ref: str) -> bool:
         return (
             '.gitmodules' in self.run(['ls-tree', '--name-only', ref], cwd=bare_path).splitlines()
         )
 
     def run(self, args, cwd=None, env=None):
         """
         Executes a Git command with the given arguments.
 
         Args:
-            args (List[str]): The list of command-line arguments for the Git command.
+            args (t.List[str]): The list of command-line arguments for the Git command.
             cwd (str | None):
                 The current working directory for the Git command.
                 If None, the current working directory is used.
             env (dict | None):
                 The environment variables for the Git command.
                 If None, the current environment variables are used.
 
@@ -240,16 +235,16 @@
         """
         if cwd is None:
             cwd = os.getcwd()
         env_copy = dict(os.environ)
         if env:
             env_copy.update(env)
 
-        p = subprocess.Popen(  # nosec
-            [self.git_command] + list(args),
+        p = subprocess.Popen(
+            [self.git_command] + list(args),  # noqa: S603
             cwd=cwd,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             env=env_copy,
         )
         stdout, stderr = p.communicate()
 
@@ -262,30 +257,31 @@
                     ' '.join(args), p.returncode, stderr.decode('utf-8'), stdout.decode('utf-8')
                 ),
                 exit_code=p.returncode,
             )
 
         return stdout.decode('utf-8')
 
-    def check_version(self):  # type: () -> None
+    def check_version(self) -> None:
         version = self.version()
 
         if version < self.git_min_supported:
             raise GitError(
                 'Your git version %s is older than minimally required %s.'
                 % (
                     version,
                     self.git_min_supported,
                 )
             )
 
-    def version(self):  # type: () -> Version
+    def version(self) -> Version:
         try:
-            git_version_str = subprocess.check_output(  # nosec
-                [self.git_command, '--version'], stderr=subprocess.STDOUT
+            git_version_str = subprocess.check_output(
+                [self.git_command, '--version'],  # noqa: S603
+                stderr=subprocess.STDOUT,
             ).decode('utf-8')
         except OSError:
             raise GitError('"git" command was not found')
 
         ver_match = re.match(r'^git version (\d+\.\d+\.\d+)', git_version_str)
 
         try:
@@ -293,26 +289,26 @@
                 return Version(ver_match.group(1))
             else:
                 raise GitCommandError()
         except (IndexError, ValueError, GitCommandError):
             raise GitError('Cannot recognize git version')
 
     @_git_cmd
-    def get_tag_version(self, cwd=None):  # type: (str | None) -> Version
+    def get_tag_version(self, cwd: t.Optional[str] = None) -> Version:
         """
         Return a valid component version of the current commit if it is tagged,
         otherwise a `GitError` is raised.
         """
 
         try:
             tag_str = self.run(['describe', '--tags', '--exact-match'], cwd=cwd)
         except GitCommandError as e:
             if e.exit_code == 128:
                 raise GitError('Not a tagged commit, cannot get version')
             else:
-                raise GitError('Cannot get tag version due to git error\n{}'.format(e))
+                raise GitError(f'Cannot get tag version due to git error\n{e}')
 
         try:
             semantic_version = Version(clean_tag_version(tag_str))
             return semantic_version
         except ValueError:
-            raise GitError('Git tag does not contain a valid component version: {}'.format(tag_str))
+            raise GitError(f'Git tag does not contain a valid component version: {tag_str}')
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/hash_tools/calculate.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/hash_tools/calculate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,62 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 """Tools for hashing and hash validation for whole packages"""
+
 import json
+import typing as t
 from hashlib import sha256
-from io import open
 from pathlib import Path
+from urllib.parse import urlparse
 
+from idf_component_tools.errors import ProcessingError
 from idf_component_tools.file_tools import filtered_paths
-from idf_component_tools.hash_tools.constants import BLOCK_SIZE
 
-try:
-    from typing import Any, Iterable, Text
-except ImportError:
-    pass
+from .constants import BLOCK_SIZE
 
 
-def hash_object(obj):  # type: (Any) -> str
+def hash_object(obj: t.Any) -> str:
     """Calculate sha256 of passed json-serialisable object"""
     sha = sha256()
     json_string = json.dumps(obj, sort_keys=True, separators=(',', ':'))
     sha.update(json_string.encode())
     return sha.hexdigest()
 
 
-def hash_file(file_path):  # type: (Text | Path) -> str
+def hash_file(file_path: t.Union[str, Path]) -> str:
     """Calculate sha256 of file"""
     sha = sha256()
 
-    with open(Path(file_path).as_posix(), 'rb') as f:
-        while True:
-            block = f.read(BLOCK_SIZE)
-            if not block:
-                break
-            sha.update(block)
+    try:
+        with open(Path(file_path).as_posix(), 'rb') as f:
+            while True:
+                block = f.read(BLOCK_SIZE)
+                if not block:
+                    break
+                sha.update(block)
+    except FileNotFoundError:
+        raise ProcessingError(f'Path {file_path} does not exist or is a broken symbolic link')
 
     return sha.hexdigest()
 
 
+def hash_url(url_string: str) -> str:
+    url = urlparse(url_string)
+    netloc = url.netloc
+    path = '/'.join(filter(None, url.path.split('/')))
+    normalized_path = '/'.join([netloc, path])
+    return sha256(normalized_path.encode('utf-8')).hexdigest()
+
+
 def hash_dir(
-    root,  # type: Text | Path
-    include=None,  # type: Iterable[Text] | None
-    exclude=None,  # type: Iterable[Text] | None
-    exclude_default=True,  # type: bool
-):  # type: (...) -> str
+    root: t.Union[str, Path],
+    include: t.Optional[t.Iterable[str]] = None,
+    exclude: t.Optional[t.Iterable[str]] = None,
+    exclude_default: bool = True,
+) -> str:
     """Calculate sha256 of sha256 of all files and file names."""
     sha = sha256()
 
     paths = sorted(
         filtered_paths(root, include=include, exclude=exclude, exclude_default=exclude_default),
         key=lambda path: path.relative_to(root).as_posix(),
     )
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/hash_tools/validate_managed_component.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/hash_tools/validate_managed_component.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,58 @@
-# SPDX-FileCopyrightText: 2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2023-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 import os
 import re
-from io import open
+import typing as t
 from pathlib import Path
 
+from idf_component_tools.constants import MANIFEST_FILENAME
 from idf_component_tools.environment import getenv_bool
-from idf_component_tools.hash_tools.validator import validate_dir
-from idf_component_tools.manifest import MANIFEST_FILENAME, ManifestManager
+from idf_component_tools.manager import ManifestManager
 
 from .constants import HASH_FILENAME, SHA256_RE
 from .errors import HashDoesNotExistError, HashNotEqualError, HashNotSHA256Error
-
-try:
-    from typing import Any, Iterable, Text
-except ImportError:
-    pass
+from .validator import validate_dir
 
 
 def validate_managed_component_by_manifest(
-    root,  # type: Text | Path
-    component_hash,  # type: str
-):  # type: (...) -> bool
+    root: t.Union[str, Path],
+    component_hash: str,
+) -> bool:
+    # TODO Te dependency is weird
+    #   move to source?
+
     """Validate component in managed directory"""
     manifest_file_path = os.path.join(root, MANIFEST_FILENAME)
 
     manifest_manager = ManifestManager(manifest_file_path, 'cmp')
     manifest = manifest_manager.load()
-    include = set(manifest.files['include'])
-    exclude = set(manifest.files['exclude'])
-    exclude.add('**/.component_hash')
+    exclude_set = set(manifest.exclude_set)
+    exclude_set.add('**/.component_hash')
 
     return validate_dir(
-        root, component_hash, include=include, exclude=exclude, exclude_default=False
+        root,
+        component_hash,
+        include=manifest.include_set,
+        exclude=exclude_set,
+        exclude_default=False,
     )
 
 
-def validate_managed_component_hash(root):  # type: (str) -> None
-    '''Validate managed components directory, raise exception if validation fails'''
+def validate_managed_component_hash(root: str) -> None:
+    """Validate managed components directory, raise exception if validation fails"""
     if getenv_bool('IDF_COMPONENT_OVERWRITE_MANAGED_COMPONENTS'):
         return
 
     hash_file_path = os.path.join(root, HASH_FILENAME)
 
     if not os.path.isdir(root) or not os.path.exists(hash_file_path):
         raise HashDoesNotExistError()
 
-    with open(hash_file_path, mode='r', encoding='utf-8') as f:
+    with open(hash_file_path, encoding='utf-8') as f:
         hash_from_file = f.read().strip()
 
     if not re.match(SHA256_RE, hash_from_file):
         raise HashNotSHA256Error()
 
     if not validate_managed_component_by_manifest(root, hash_from_file):
         raise HashNotEqualError()
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/lock/manager.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/lock/manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,102 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import os
+import typing as t
 from collections import OrderedDict
-from io import open
 
-from schema import And, Optional, Or, Schema, SchemaError, Use
-from six import string_types
-from yaml import Node, SafeDumper, YAMLError
+from pydantic import ValidationError
+from yaml import Node, SafeDumper, YAMLError, safe_load
 from yaml import dump as dump_yaml
-from yaml import safe_load
 
-import idf_component_tools as tools
+from idf_component_tools.build_system_tools import get_env_idf_target, get_idf_version
+from idf_component_tools.errors import LockError, LockVersionMismatchError
+from idf_component_tools.manifest import SolvedComponent, SolvedManifest
+from idf_component_tools.sources import IDFSource
+from idf_component_tools.utils import ComponentVersion
 
-from ..build_system_tools import get_env_idf_target, get_idf_version
-from ..errors import LockError
-from ..manifest import ComponentVersion, known_targets
-from ..manifest.solved_component import SolvedComponent
-from ..manifest.solved_manifest import SolvedManifest
-from ..sources import IDFSource
-
-FORMAT_VERSION = '1.0.0'
-
-EMPTY_LOCK = {
-    'manifest_hash': None,
-    'version': FORMAT_VERSION,
-}
-
-HASH_SCHEMA = Or(And(Or(*string_types), lambda h: len(h) == 64), None)
-
-LOCK_SCHEMA = Schema(
-    {
-        Optional('dependencies'): {
-            Optional(Or(*string_types)): {
-                'source': Or(*[source.schema() for source in tools.sources.KNOWN_SOURCES]),
-                'version': Or(*string_types),
-                Optional('component_hash'): HASH_SCHEMA,
-            }
-        },
-        'manifest_hash': HASH_SCHEMA,
-        'version': And(Or(*string_types), len),
-        Optional('target'): And(Use(str.lower), lambda s: s in known_targets()),
-    }
-)
+FORMAT_VERSION = '2.0.0'
 
 
-def _ordered_dict_representer(dumper, data):  # type: (SafeDumper, OrderedDict) -> Node
-    return dumper.represent_data(dict(data))
+class LockFile(SolvedManifest):
+    version: str = FORMAT_VERSION
+
 
+EMPTY_LOCK: t.Dict[str, t.Any] = {}
 
-def _unicode_representer(dumper, data):  # type: (SafeDumper, str) -> Node
-    return dumper.represent_str(data.encode('utf-8'))  # type: ignore
+
+def _ordered_dict_representer(dumper: SafeDumper, data: t.OrderedDict) -> Node:
+    return dumper.represent_data(dict(data))
 
 
 SafeDumper.add_representer(OrderedDict, _ordered_dict_representer)
-SafeDumper.add_representer(string_types, _unicode_representer)  # type: ignore
 
 
 class LockManager:
     def __init__(self, path):
         self._path = path
 
     def exists(self):
         return os.path.isfile(self._path)
 
-    def dump(self, solution):  # type: (SolvedManifest) -> None
+    def dump(self, solution: SolvedManifest) -> None:
         """Writes updated lockfile to disk"""
         # add idf version if not in solution.dependencies
         if 'idf' not in solution.solved_components:
             solution.dependencies.append(
                 SolvedComponent(
-                    'idf',
-                    ComponentVersion(get_idf_version()),
-                    IDFSource(),
+                    name='idf',
+                    version=ComponentVersion(get_idf_version()),
+                    source=IDFSource(),
                 )
             )
 
         try:
             with open(self._path, mode='w', encoding='utf-8') as f:
-                # inject format version
-                solution_dict = solution.serialize()
-                solution_dict['version'] = FORMAT_VERSION
-                solution_dict['target'] = get_env_idf_target()
-                lock = LOCK_SCHEMA.validate(solution_dict)
+                # inject lock file version and current target
+                lock = LockFile(**solution.model_dump())
+                lock.target = get_env_idf_target()
+
                 dump_yaml(
-                    data=lock, stream=f, encoding='utf-8', allow_unicode=True, Dumper=SafeDumper
+                    data=lock.model_dump(),
+                    stream=f,
+                    encoding='utf-8',
+                    allow_unicode=True,
+                    Dumper=SafeDumper,
                 )
-        except SchemaError as e:
-            raise LockError('Lock format is not valid:\n%s' % str(e))
+        except ValidationError as e:
+            raise LockError(f'Lock format is not valid:\n{e}')
 
-    def load(self):  # type: () -> SolvedManifest
+    def load(self) -> SolvedManifest:
         if not self.exists():
             return SolvedManifest.fromdict(EMPTY_LOCK)
 
-        with open(self._path, mode='r', encoding='utf-8') as f:
-            try:
-                content = f.read()
-
-                if not content:
-                    return SolvedManifest.fromdict(EMPTY_LOCK)
-
-                lock = LOCK_SCHEMA.validate(safe_load(content))
-
-                version = lock.pop('version')
-                if version != FORMAT_VERSION:
-                    raise LockError(
-                        'Cannot parse components lock file.'
-                        'Lock file format version is %s, while only %s is supported'
-                        % (version, FORMAT_VERSION)
-                    )
-
-                return SolvedManifest.fromdict(lock)
-            except (YAMLError, SchemaError):
-                raise LockError(
-                    (
-                        'Cannot parse components lock file. '
-                        'Please check that\n\t%s\nis a valid lock YAML file.\n'
-                        'You can delete corrupted lock file and it will be recreated on next run. '
-                        'Some components may be updated in this case.'
-                    )
-                    % self._path
+        try:
+            with open(self._path, encoding='utf-8') as f:
+                yaml_dict = safe_load(f)
+
+            if not yaml_dict:
+                lock = LockFile.fromdict(EMPTY_LOCK)
+            else:
+                lock = LockFile.fromdict(yaml_dict)
+
+            lock_dict = lock.model_dump()
+            version = lock_dict.pop('version')
+            if version != FORMAT_VERSION:
+                raise LockVersionMismatchError(
+                    f'Current idf-component-manager default lock file version is {FORMAT_VERSION}, '
+                    f'but found {version} in {self._path}. '
+                    f'Recreating lock file with the current version.'
                 )
+
+            return SolvedManifest.fromdict(lock_dict)
+        except (YAMLError, ValidationError):
+            raise LockError(
+                (
+                    'Cannot parse components lock file. '
+                    'Please check that\n\t%s\nis a valid lock YAML file.\n'
+                    'You can delete corrupted lock file and it will be recreated on next run. '
+                    'Some components may be updated in this case.'
+                )
+                % self._path
+            )
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/manifest/__init__.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/manifest/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,42 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 from .constants import (
     FULL_SLUG_REGEX,
-    MANIFEST_FILENAME,
     SLUG_REGEX,
     WEB_DEPENDENCY_REGEX,
     known_targets,
 )
-from .manager import ManifestManager
-from .manifest import (
+from .metadata import Metadata
+from .models import (
     ComponentRequirement,
-    ComponentVersion,
-    ComponentWithVersions,
-    HashedComponentVersion,
     Manifest,
     OptionalDependency,
     OptionalRequirement,
-    ProjectRequirements,
-    filter_optional_dependencies,
+    SolvedComponent,
+    SolvedManifest,
+)
+from .schemas import (
+    BUILD_METADATA_KEYS,
+    INFO_METADATA_KEYS,
+    MANIFEST_JSON_SCHEMA,
+    METADATA_JSON_SCHEMA,
 )
-from .schemas import BUILD_METADATA_KEYS, INFO_METADATA_KEYS, JSON_SCHEMA
-from .validator import ExpandedManifestValidator, ManifestValidator
 
 __all__ = [
     'BUILD_METADATA_KEYS',
     'ComponentRequirement',
-    'ComponentVersion',
-    'ComponentWithVersions',
-    'filter_optional_dependencies',
     'FULL_SLUG_REGEX',
-    'HashedComponentVersion',
     'INFO_METADATA_KEYS',
-    'JSON_SCHEMA',
     'known_targets',
-    'MANIFEST_FILENAME',
     'Manifest',
-    'ManifestManager',
-    'ManifestValidator',
-    'ExpandedManifestValidator',
+    'MANIFEST_JSON_SCHEMA',
     'OptionalDependency',
     'OptionalRequirement',
-    'ProjectRequirements',
     'SLUG_REGEX',
     'WEB_DEPENDENCY_REGEX',
+    'SolvedComponent',
+    'SolvedManifest',
+    'Metadata',
+    'METADATA_JSON_SCHEMA',
 ]
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/manifest/constants.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/manifest/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import os
+import re
 import sys
+import typing as t
 
-MANIFEST_FILENAME = 'idf_component.yml'
-SLUG_BODY_REGEX = r'[a-zA-Z\d]+(?:(?:[_-](?![_-]+))|(?:[a-zA-Z\d]))*[a-zA-Z\d]+'
+SLUG_BODY_REGEX = r'[a-zA-Z\d]+(?:[_-][a-zA-Z\d]*)*[a-zA-Z\d]+'
 SLUG_REGEX = r'^{}$'.format(SLUG_BODY_REGEX)
 FULL_SLUG_REGEX = r'^((?:{slug}/{slug})|(?:{slug}))$'.format(slug=SLUG_BODY_REGEX)
-TAGS_REGEX = r'^[A-Za-z0-9\_\-]{3,32}$'
+COMPILED_FULL_SLUG_REGEX = re.compile(FULL_SLUG_REGEX)
 WEB_DEPENDENCY_REGEX = r'^((?:{slug}/{slug})|(?:{slug}))(.*)$'.format(slug=SLUG_BODY_REGEX)
-COMMIT_ID_RE = r'[0-9a-f]{40}'
-IF_IDF_VERSION_REGEX = r'^(?P<keyword>idf_version) *(?P<comparison>[\^=~<>!]+)(?P<spec>.+)$'
-IF_TARGET_REGEX = r'^(?P<keyword>target) *(?P<comparison>!=|==|not in|in)(?P<targets>.+)$'
 
-LINKS = ['repository', 'documentation', 'issues', 'discussion', 'url']
+LINKS = ['repository', 'commit_sha', 'documentation', 'issues', 'discussion', 'url']
 KNOWN_INFO_METADATA_FIELDS = [
     'maintainers',
     'description',
     'tags',
     'examples',
     'license',
     'repository_info',
@@ -29,21 +27,22 @@
     'esp32',
     'esp32s2',
     'esp32c3',
     'esp32s3',
     'esp32c2',
     'esp32c5',
     'esp32c6',
+    'esp32c61',
     'esp32h2',
     'esp32p4',
     'linux',
 ]
 
 
-def known_targets():  # type: () -> list[str]
+def known_targets() -> t.List[str]:
     try:
         targets = os.environ['IDF_COMPONENT_MANAGER_KNOWN_TARGETS'].split(',')
         if any(targets):
             return targets
     except KeyError:
         pass
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/messages.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/messages.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# SPDX-FileCopyrightText: 2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2023-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
+import typing as t
 import warnings
 
 
 class UserHint(Warning):
     pass
 
 
@@ -11,40 +12,29 @@
     pass
 
 
 class MetadataWarning(UserHint):
     pass
 
 
-class MetadataKeyWarning(MetadataWarning):
-    def __init__(self, field_name, field_type):
-        super(MetadataKeyWarning, self).__init__(
-            'Unknown {} field "{}" in the manifest file'.format(field_type, field_name)
-        )
-
-
 class UserDeprecationWarning(UserWarning):
     pass
 
 
 def warn(
-    message,
-):  # type: (Exception | str) -> None
+    message: t.Union[Exception, str],
+) -> None:
     warnings.warn(str(message))
 
 
-def hint(
-    message,
-):  # type: (Warning | Exception | str) -> None
+def hint(message: t.Union[Warning, Exception, str]) -> None:
     if isinstance(message, Warning):
         warnings.warn(message)
     else:
         warnings.warn(str(message), UserHint)
 
 
-def notice(
-    message,
-):  # type: (Warning | Exception | str) -> None
+def notice(message: t.Union[Warning, Exception, str]) -> None:
     if isinstance(message, Warning):
         warnings.warn(message)
     else:
         warnings.warn(str(message), UserNotice)
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/registry/api_client_errors.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/registry/client_errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
-try:
-    import http.client as http_client
-except ImportError:
-    # Python 2
-    import httplib as http_client  # type: ignore
-
-try:
-    from typing import Any
-except ImportError:
-    pass
+import http.client as http_client
+import typing as t
 
 
 class APIClientError(Exception):
-    def __init__(self, message='API Request Error', endpoint=None, status_code=None):
-        # type: (Any, str | None, int | None) -> None
-        super(APIClientError, self).__init__(message)
+    def __init__(
+        self,
+        message: t.Any = 'API Request Error',
+        endpoint: t.Optional[str] = None,
+        status_code: t.Optional[int] = None,
+    ) -> None:
+        super().__init__(message)
         self.endpoint = endpoint
         self.status_code = status_code
 
-    def request_info(self):  # type: () -> list[str]
+    def request_info(self) -> t.List[str]:
         messages = []
         if self.endpoint is not None:
-            messages.append('URL: {}'.format(self.endpoint))
+            messages.append(f'URL: {self.endpoint}')
 
         if self.status_code is not None:
             messages.append(
                 'Status code: {} {}'.format(
                     self.status_code, http_client.responses.get(self.status_code, '')
                 )
             )
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/registry/base_client.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/registry/base_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 # SPDX-FileCopyrightText: 2023-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 import os
 import platform
+import typing as t
 
 import requests
 from cachecontrol import CacheControlAdapter
 from cachecontrol.caches import FileCache
 from cachecontrol.heuristics import ExpiresAfter
 from requests.adapters import HTTPAdapter
+from requests.auth import AuthBase
 from requests_file import FileAdapter
 
-import idf_component_tools as tools
 from idf_component_tools.__version__ import __version__
+from idf_component_tools.constants import DEFAULT_NAMESPACE, IDF_COMPONENT_REGISTRY_URL
 from idf_component_tools.environment import detect_ci, getenv_int
 from idf_component_tools.file_cache import FileCache as ComponentFileCache
+from idf_component_tools.manifest import BUILD_METADATA_KEYS, ComponentRequirement
 from idf_component_tools.messages import warn
 from idf_component_tools.semver import SimpleSpec, Version
+from idf_component_tools.utils import (
+    ComponentWithVersions,
+    HashedComponentVersion,
+)
 
-from ..manifest import BUILD_METADATA_KEYS, ComponentWithVersions
-from .api_schemas import COMPONENT_SCHEMA
-from .token_auth import TokenAuth
-
-try:
-    from typing import Callable
-except ImportError:
-    pass
+from .api_models import ComponentResponse
 
 DEFAULT_API_CACHE_EXPIRATION_MINUTES = 0
 MAX_RETRIES = 3
 
 
-def env_cache_time():  # type: () -> int
+def env_cache_time() -> int:
     try:
         return getenv_int(
             'IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES',
             DEFAULT_API_CACHE_EXPIRATION_MINUTES,
         )
     except ValueError:
         warn(
             'IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES is set to a non-numeric value. '
             'Please set the variable to the number of minutes. Disabling caching.'
         )
         return DEFAULT_API_CACHE_EXPIRATION_MINUTES
 
 
 def create_session(
-    cache=False,  # type: bool
-    cache_path=None,  # type: str | None
-    cache_time=None,  # type: int | None
-    token=None,  # type: str | None
-):  # type: (...) -> requests.Session
+    cache: bool = False,
+    cache_path: t.Optional[str] = None,
+    cache_time: t.Optional[int] = None,
+    token: t.Optional[str] = None,
+) -> requests.Session:
     if cache_path is None:
         cache_path = ComponentFileCache().path()
 
     cache_time = cache_time or env_cache_time()
     if cache and cache_time:
         api_adapter = CacheControlAdapter(
             max_retries=MAX_RETRIES,
@@ -70,75 +70,75 @@
     session.mount('http://', api_adapter)
     session.mount('https://', api_adapter)
     session.mount('file://', FileAdapter())
 
     return session
 
 
-def user_agent():  # type: () -> str
+def user_agent() -> str:
     """
     Returns user agent string.
     """
 
     environment_info = [
-        '{os}/{release} {arch}'.format(
-            os=platform.system(), release=platform.release(), arch=platform.machine()
-        ),
-        'python/{version}'.format(version=platform.python_version()),
+        f'{platform.system()}/{platform.release()} {platform.machine()}',
+        f'python/{platform.python_version()}',
     ]
 
     ci_name = detect_ci()
     if ci_name:
-        environment_info.append('ci/{}'.format(ci_name))
+        environment_info.append(f'ci/{ci_name}')
 
     user_agent = 'idf-component-manager/{version} ({env})'.format(
         version=__version__,
         env='; '.join(environment_info),
     )
 
     return user_agent
 
 
-class BaseClient(object):
-    def __init__(self, sources=None):
-        self.sources = sources
+class BaseClient:
+    def __init__(self, default_namespace: t.Optional[str]) -> None:
+        self.default_namespace = default_namespace or DEFAULT_NAMESPACE
 
-    def version_dependencies(self, version):
-        dependencies = []
+    def version_dependencies(self, version: t.Dict[str, t.Any]) -> t.List[ComponentRequirement]:
+        deps: t.List[ComponentRequirement] = []
         for dependency in version.get('dependencies', []):
-            # Support only idf and service sources
-            if dependency['source'] == 'idf':
-                sources = [tools.sources.IDFSource({})]
-            else:
-                sources = self.sources or [tools.sources.WebServiceSource({})]
+            # make it compatible with the old format
+            dependency['name'] = f'{dependency.pop("namespace")}/{dependency.pop("name")}'
 
-            is_public = dependency.get('is_public', False)
-            require = dependency.get('require', True)
-            require_string = 'public' if is_public else ('private' if require else 'no')
-
-            dependencies.append(
-                tools.manifest.ComponentRequirement(
-                    name='{}/{}'.format(dependency['namespace'], dependency['name']),
-                    version_spec=dependency['spec'],
-                    sources=sources,
-                    public=is_public,
-                    require=require_string,
-                    optional_requirement=tools.manifest.OptionalRequirement.fromdict(dependency),
-                )
-            )
+            is_public = dependency.pop('is_public', False)
+            require = dependency.pop('require', True)
+            dependency['require'] = 'public' if is_public else ('private' if require else 'no')
+
+            dependency['version'] = dependency.pop('spec')
+
+            source_str = dependency.pop('source')
+            if source_str == 'idf':
+                dependency['name'] = 'idf'
+            elif source_str == 'service':
+                dependency['service_url'] = IDF_COMPONENT_REGISTRY_URL
+            else:
+                raise ValueError('Unknown source type, Internal error')
 
-        return tools.manifest.filter_optional_dependencies(dependencies)
+            dep = ComponentRequirement.fromdict(dependency)
+            deps.append(dep)
+        return [dep for dep in deps if dep.meet_optional_dependencies]
 
     def versions(
-        self, request, component_name, spec='*'
-    ):  # type: (Callable, str, str) -> ComponentWithVersions
+        self,
+        request: t.Callable,
+        component_name: str,
+        spec: str = '*',
+        **kwargs,
+    ) -> ComponentWithVersions:
         """List of versions for given component with required spec"""
         component_name = component_name.lower()
         semantic_spec = SimpleSpec(spec or '*')
-        body = request('get', ['components', component_name.lower()], schema=COMPONENT_SCHEMA)
+        body = request('get', ['components', component_name.lower()], schema=ComponentResponse)
 
         versions = []
         filtered_versions = filter_versions(body['versions'], spec, component_name)
 
         for version in filtered_versions:
             if not semantic_spec.match(Version(version['version'])):
                 continue
@@ -152,29 +152,30 @@
 
             if all_build_keys_known:
                 versions.append((version, all_build_keys_known))
 
         return ComponentWithVersions(
             name=component_name,
             versions=[
-                tools.manifest.HashedComponentVersion(
+                HashedComponentVersion(
                     version_string=version['version'],
                     component_hash=version['component_hash'],
                     dependencies=self.version_dependencies(version),
                     targets=version['targets'],
                     all_build_keys_known=all_build_keys_known,
+                    **kwargs,
                 )
                 for version, all_build_keys_known in versions
             ],
         )
 
 
 def filter_versions(
-    versions, spec, component_name
-):  # type: (list[dict], str | None, str) -> list[dict]
+    versions: t.List[t.Dict], spec: t.Optional[str], component_name: str
+) -> t.List[t.Dict]:
     if spec and spec != '*':
         requested_version = SimpleSpec(str(spec))
         filtered_versions = [v for v in versions if requested_version.match(Version(v['version']))]
 
         if not filtered_versions or not any([bool(v.get('yanked_at')) for v in filtered_versions]):
             return filtered_versions
 
@@ -198,7 +199,17 @@
             )
         else:
             filtered_versions = [v for v in filtered_versions if not v.get('yanked_at')]
     else:
         filtered_versions = [v for v in versions if not v.get('yanked_at')]
 
     return filtered_versions
+
+
+class TokenAuth(AuthBase):
+    def __init__(self, token: t.Optional[str]) -> None:
+        self.token = token
+
+    def __call__(self, request):
+        if self.token:
+            request.headers['Authorization'] = f'Bearer {self.token}'
+        return request
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/registry/request_processor.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/registry/request_processor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 # SPDX-FileCopyrightText: 2023-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 import os
+import typing as t
+import warnings
+from copy import deepcopy
 
 import requests
+from pydantic import ValidationError
 from requests import Response
-from schema import Schema, SchemaError
 
 from idf_component_tools.environment import getenv_bool_or_string
-from idf_component_tools.registry.api_schemas import ERROR_SCHEMA
 
-from .api_client_errors import (
+from .api_models import ApiBaseModel, ErrorResponse
+from .client_errors import (
     KNOWN_API_ERRORS,
     APIClientError,
     ContentTooLargeError,
     NetworkConnectionError,
     StorageFileNotFound,
 )
 
 DEFAULT_TIMEOUT = (6.05, 30.1)  # Connect timeout  # Read timeout
 
 
-def join_url(*args):  # type: (*str) -> str
+def join_url(*args) -> str:
     """
     Joins given arguments into an url and add trailing slash
     """
     parts = [part[:-1] if part and part[-1] == '/' else part for part in args]
     return '/'.join(parts)
 
 
-def get_timeout():  # type: () -> float | tuple[float, float]
+def get_timeout() -> t.Union[float, t.Tuple[float, float]]:
     try:
         return float(os.environ['IDF_COMPONENT_SERVICE_TIMEOUT'])
     except ValueError:
         raise APIClientError(
             'Cannot parse IDF_COMPONENT_SERVICE_TIMEOUT. It should be a number in seconds.'
         )
     except KeyError:
         return DEFAULT_TIMEOUT
 
 
-def verify_ssl():  # type: () -> bool | str
+def verify_ssl() -> t.Union[bool, str]:
     """Returns either True, False or a path to a CA bundle file"""
 
     return getenv_bool_or_string('IDF_COMPONENT_VERIFY_SSL', True)
 
 
 def make_request(
-    method,  # type: str
-    session,  # type: requests.Session
-    endpoint,  # type: str
-    data,  # type: dict | None
-    json,  # type: dict | None
-    headers,  # type: dict | None
-    timeout,  # type: float | tuple[float, float]
-):  # type: (...) -> Response
+    method: str,
+    session: requests.Session,
+    endpoint: str,
+    data: t.Optional[t.Dict],
+    json: t.Optional[t.Dict],
+    headers: t.Optional[t.Dict],
+    timeout: t.Union[float, t.Tuple[float, float]],
+) -> Response:
     try:
         response = session.request(
             method,
             endpoint,
             data=data,
             json=json,
             headers=headers,
@@ -70,18 +73,18 @@
     except requests.exceptions.RequestException:
         raise APIClientError('HTTP request error', endpoint=endpoint)
 
     return response
 
 
 def handle_response_errors(
-    response,  # type:  requests.Response
-    endpoint,  # type:  str
-    use_storage,  # type:  bool
-):  # type: (...) -> dict
+    response: requests.Response,
+    endpoint: str,
+    use_storage: bool,
+) -> t.Dict:
     if response.status_code == 204:  # NO CONTENT
         return {}
     elif 400 <= response.status_code < 500:
         if use_storage:
             if response.status_code == 404:
                 raise StorageFileNotFound()
             raise APIClientError(
@@ -94,30 +97,30 @@
             endpoint=endpoint,
             status_code=response.status_code,
         )
 
     return response.json()
 
 
-def handle_4xx_error(response):  # type: (requests.Response) -> None
+def handle_4xx_error(response: requests.Response) -> None:
     if response.status_code == 413:
         raise ContentTooLargeError(
             'Error during request. The provided content is too large '
             'to process. Please reduce the size and try again.',
             endpoint=response.url,
             status_code=response.status_code,
         )
 
     try:
-        json = ERROR_SCHEMA.validate(response.json())
-        name = json['error']
-        messages = json['messages']
-    except SchemaError as e:
+        error = ErrorResponse.model_validate(response.json())
+        name = error.error
+        messages = error.messages
+    except ValidationError as e:
         raise APIClientError(
-            'API Endpoint returned unexpected error description:\n{}'.format(str(e)),
+            f'API Endpoint returned unexpected error description:\n{e}',
             endpoint=response.url,
             status_code=response.status_code,
         )
     except ValueError:
         raise APIClientError(
             'Server returned an error in unexpected format',
             endpoint=response.url,
@@ -131,42 +134,41 @@
         raise exception(
             'Error during request:\n{}\nStatus code: {} Error code: {}'.format(
                 str(messages), response.status_code, name
             )
         )
 
 
-def validate_response(
-    response_json,  # type: dict
-    schema,  # type:  Schema | None
-    endpoint,  # type: str
-):  # type: (...) -> dict
+def base_request(
+    url: str,
+    session: requests.Session,
+    method: str,
+    path: t.List[str],
+    data: t.Optional[t.Dict] = None,
+    json: t.Optional[t.Dict] = None,
+    headers: t.Optional[t.Dict] = None,
+    schema: t.Optional[ApiBaseModel] = None,
+    use_storage: bool = False,
+) -> t.Dict:
+    endpoint = join_url(url, *path)
+    timeout = get_timeout()
+    response = make_request(method, session, endpoint, data, json, headers, timeout)
+    response_json = handle_response_errors(response, endpoint, use_storage)
+
+    if schema is None:
+        return response_json
+
     try:
-        if schema is not None:
-            schema.validate(response_json)
-    except SchemaError as e:
+        # model validation will modify the response_json, so we need to deepcopy it
+        # besides, the unknown fields will be ignored, suppressing the warnings
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore', UserWarning)
+            schema.model_validate(deepcopy(response_json))
+    except ValidationError as e:
         raise APIClientError(
-            'API Endpoint returned unexpected JSON:\n{}'.format(str(e)),
+            f'API Endpoint returned unexpected JSON:\n{e}',
             endpoint=endpoint,
         )
     except (ValueError, KeyError, IndexError):
         raise APIClientError('Unexpected component server response', endpoint=endpoint)
 
     return response_json
-
-
-def base_request(
-    url,  # type: str
-    session,  # type: requests.Session
-    method,  # type: str
-    path,  # type: list[str]
-    data=None,  # type: dict | None
-    json=None,  # type: dict | None
-    headers=None,  # type: dict | None
-    schema=None,  # type: Schema
-    use_storage=False,  # type: bool
-):  # type: (...) -> dict
-    endpoint = join_url(url, *path)
-    timeout = get_timeout()
-    response = make_request(method, session, endpoint, data, json, headers, timeout)
-    response_json = handle_response_errors(response, endpoint, use_storage)
-    return validate_response(response_json, schema, endpoint)
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/registry/storage_client.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/registry/storage_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,46 @@
 # SPDX-FileCopyrightText: 2023-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
+import typing as t
 from functools import wraps
 
-from schema import Schema
-
-import idf_component_tools as tools
-from idf_component_tools.manifest import ComponentWithVersions, HashedComponentVersion
-from idf_component_tools.registry.api_client_errors import (
-    ComponentNotFound,
-    StorageFileNotFound,
-    VersionNotFound,
-)
-from idf_component_tools.registry.api_schemas import COMPONENT_SCHEMA
-from idf_component_tools.registry.base_client import BaseClient, create_session, filter_versions
-from idf_component_tools.registry.component_details import ComponentDetailsWithStorageURL
-from idf_component_tools.registry.request_processor import base_request, join_url
 from idf_component_tools.semver import SimpleSpec, Version
+from idf_component_tools.utils import (
+    ComponentWithVersions,
+)
 
-try:
-    from typing import Any, Callable
-except ImportError:
-    pass
-
-
-class ComponentWithVersionsAndStorageURL(ComponentWithVersions):
-    def __init__(
-        self, name, versions, storage_url
-    ):  # type: (str, list[HashedComponentVersion], str | None) -> None
-        super(ComponentWithVersionsAndStorageURL, self).__init__(name, versions)
-        self.storage_url = storage_url
-
-    @classmethod
-    def from_component_with_versions(cls, cmp_with_versions, storage_url):
-        return cls(cmp_with_versions.name, cmp_with_versions.versions, storage_url)
+from .api_models import ApiBaseModel, ComponentResponse
+from .base_client import BaseClient, create_session, filter_versions
+from .client_errors import ComponentNotFound, StorageFileNotFound, VersionNotFound
+from .request_processor import base_request, join_url
 
 
 class StorageClient(BaseClient):
-    def __init__(self, storage_url=None, sources=None):
-        super(StorageClient, self).__init__(sources)
+    def __init__(self, storage_url: str, default_namespace: t.Optional[str] = None) -> None:
+        super().__init__(default_namespace=default_namespace)
+
         self.storage_url = storage_url
 
-    def _request(cache=False):  # type: (BaseClient | bool) -> Callable
-        def decorator(f):  # type: (Callable[..., Any]) -> Callable
+    def _request(cache: bool = False) -> t.Callable:  # type: ignore
+        def decorator(f: t.Callable[..., t.Any]) -> t.Callable:
             @wraps(f)  # type: ignore
             def wrapper(self, *args, **kwargs):
-                url = self.storage_url
                 session = create_session(cache=cache)
 
                 def request(
-                    method,  # type: str
-                    path,  # type: list[str]
-                    data=None,  # type: dict | None
-                    json=None,  # type: dict | None
-                    headers=None,  # type: dict | None
-                    schema=None,  # type: Schema | None
+                    method: str,
+                    path: t.List[str],
+                    data: t.Optional[t.Dict] = None,
+                    json: t.Optional[t.Dict] = None,
+                    headers: t.Optional[t.Dict] = None,
+                    schema: t.Optional[ApiBaseModel] = None,
                 ):
                     path[-1] += '.json'
                     return base_request(
-                        url,
+                        self.storage_url,
                         session,
                         method,
                         path,
                         data=data,
                         json=json,
                         headers=headers,
                         schema=schema,
@@ -72,89 +51,77 @@
 
             return wrapper
 
         return decorator
 
     @_request(cache=True)
     def versions(
-        self, request, component_name, spec='*'
-    ):  # type: (Callable, str, str) -> ComponentWithVersionsAndStorageURL
+        self, request: t.Callable, component_name: str, spec: str = '*', **kwargs
+    ) -> ComponentWithVersions:
         """List of versions for given component with required spec"""
         try:
-            cmp_with_versions = super(StorageClient, self).versions(
-                request=request, component_name=component_name, spec=spec
+            cmp_with_versions = super().versions(
+                request=request,
+                component_name=component_name,
+                spec=spec,
+                download_url=self.storage_url,
+                **kwargs,
             )
         except StorageFileNotFound:
-            raise ComponentNotFound('Component "{}" not found'.format(component_name))
+            raise ComponentNotFound(f'Component "{component_name}" not found')
+
+        return cmp_with_versions
 
-        return ComponentWithVersionsAndStorageURL.from_component_with_versions(
-            cmp_with_versions, self.storage_url
-        )
-
-    def component(
-        self, component_name, version=None
-    ):  # type: (str, str | None) -> ComponentDetailsWithStorageURL
+    def component(self, component_name: str, version: t.Optional[str] = None) -> t.Dict[str, t.Any]:
         """
         Manifest for given version of component, if version is None highest version is returned
         """
-
         component_name = component_name.lower()
         info = self.get_component_info(component_name=component_name)
 
         versions = info['versions']
         filtered_versions = filter_versions(versions, version, component_name)
 
         if not filtered_versions:
             raise VersionNotFound(
                 'Version of the component "{}" satisfying the spec "{}" was not found.'.format(
                     component_name, str(version)
                 )
             )
 
         best_version = max(filtered_versions, key=lambda v: Version(v['version']))
-        download_url = join_url(self.storage_url, best_version['url'])
+
+        best_version['name'] = component_name
+
+        best_version['download_url'] = join_url(self.storage_url, best_version['url'])
 
         documents = best_version['docs']
         for document, url in documents.items():
             documents[document] = join_url(self.storage_url, url)
 
         license_info = best_version['license']
-        license_name = None
-        license_url = None
         if license_info:
-            license_name = license_info['name']
-            license_url = join_url(self.storage_url, license_info['url'])
+            license_info['url'] = join_url(self.storage_url, license_info['url'])
 
         examples = best_version['examples']
         for example in examples:
             example.update({'url': join_url(self.storage_url, example['url'])})
 
-        return ComponentDetailsWithStorageURL(
-            name=('%s/%s' % (info['namespace'], info['name'])),
-            version=tools.manifest.ComponentVersion(best_version['version']),
-            dependencies=self.version_dependencies(best_version),
-            maintainers=None,
-            download_url=download_url,
-            documents=documents,
-            license_name=license_name,
-            license_url=license_url,
-            examples=examples,
-            storage_url=self.storage_url,
-        )
+        return best_version
 
     @_request(cache=True)
     def get_component_info(
-        self, request, component_name, spec='*'
-    ):  # type: (Callable, str, str) -> dict
+        self, request: t.Callable, component_name: str, spec: str = '*'
+    ) -> t.Dict:
         try:
             response = request(
-                'get', ['components', component_name.lower()], schema=COMPONENT_SCHEMA
+                'get', ['components', component_name.lower()], schema=ComponentResponse
             )
         except StorageFileNotFound:
-            raise ComponentNotFound('Component "{}" not found'.format(component_name))
+            raise ComponentNotFound(f'Component "{component_name}" not found')
 
         if spec != '*':
             versions = []
             for version in response['versions']:
                 if not SimpleSpec(spec).match(Version(version['version'])):
                     continue
                 versions.append(version)
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/semver/base.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/semver/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-# -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2016 Python-SemanticVersion project
 # SPDX-License-Identifier: BSD 2-Clause License
-# SPDX-FileContributor: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileContributor: 2022-2024 Espressif Systems (Shanghai) CO LTD
+from __future__ import annotations
 
 import functools
 import re
+import typing as t
 
 
 def _has_leading_zero(value):
     return value and value[0] == '0' and value.isdigit() and value != '0'
 
 
-class MaxIdentifier(object):
-    __slots__ = []  # type: list[str]
+class MaxIdentifier:
+    __slots__: t.List[str] = []
 
     def __repr__(self):
         return 'MaxIdentifier()'
 
     def __eq__(self, other):
         return isinstance(other, self.__class__)
 
 
 @functools.total_ordering
-class NumericIdentifier(object):
+class NumericIdentifier:
     __slots__ = ['value']
 
     def __init__(self, value):
         self.value = int(value)
 
     def __repr__(self):
-        return 'NumericIdentifier(%r)' % self.value
+        return f'NumericIdentifier({self.value!r})'
 
     def __eq__(self, other):
         if isinstance(other, NumericIdentifier):
             return self.value == other.value
         return NotImplemented
 
     def __lt__(self, other):
@@ -44,22 +45,22 @@
         elif isinstance(other, NumericIdentifier):
             return self.value < other.value
         else:
             return NotImplemented
 
 
 @functools.total_ordering
-class AlphaIdentifier(object):
+class AlphaIdentifier:
     __slots__ = ['value']
 
     def __init__(self, value):
         self.value = value.encode('ascii')
 
     def __repr__(self):
-        return 'AlphaIdentifier(%r)' % self.value
+        return f'AlphaIdentifier({self.value!r})'
 
     def __eq__(self, other):
         if isinstance(other, AlphaIdentifier):
             return self.value == other.value
         return NotImplemented
 
     def __lt__(self, other):
@@ -69,15 +70,15 @@
             return False
         elif isinstance(other, AlphaIdentifier):
             return self.value < other.value
         else:
             return NotImplemented
 
 
-class Version(object):
+class Version:
     version_re = re.compile(
         r'^(\d+)\.(\d+)\.(\d+)(?:~(\d+))?(?:-([0-9a-zA-Z.-]+))?(?:\+([0-9a-zA-Z.-]+))?$'
     )
 
     def __init__(
         self,
         version_string=None,
@@ -163,15 +164,15 @@
         elif level == 'major':
             return Version(
                 major=self.major,
                 minor=0,
                 patch=0,
             )
         else:
-            raise ValueError('Invalid truncation level `%s`.' % level)
+            raise ValueError(f'Invalid truncation level `{level}`.')
 
     @classmethod
     def coerce(cls, version_string):
         """Coerce an arbitrary version string into a semver-compatible one.
 
         The rule is:
         - If not enough components, fill minor/patch with zeroes
@@ -191,15 +192,15 @@
             >>> Version.coerce('0.1~2')
             Version(0, 1, 0, 2)
         """
         base_re = re.compile(r'^\d+(?:\.\d+(?:\.\d+)?)?(?:~\d+)?')
 
         match = base_re.match(version_string)
         if not match:
-            raise ValueError('Version string lacks a numerical component: %r' % version_string)
+            raise ValueError(f'Version string lacks a numerical component: {version_string!r}')
 
         version = version_string[: match.end()]
         if '~' in version:
             version, revision = version.split('~')
         else:
             version, revision = version, '0'
         revision = int(revision)
@@ -214,15 +215,15 @@
             part.lstrip('0') or '0'
             for part in version.split('.')
         )
 
         if match.end() == len(version_string):
             return Version(version, revision=revision)
 
-        rest = version_string[match.end() :]  # noqa
+        rest = version_string[match.end() :]
 
         # Cleanup the 'rest'
         rest = re.sub(r'[^a-zA-Z0-9+.-]', '-', rest)
 
         if rest[0] == '+':
             # A 'build' component
             prerelease = ''
@@ -241,53 +242,53 @@
             prerelease, build = rest.split('+', 1)
         else:
             prerelease, build = rest, ''
 
         build = build.replace('+', '.')
 
         if prerelease:
-            version = '%s-%s' % (version, prerelease)
+            version = f'{version}-{prerelease}'
         if build:
-            version = '%s+%s' % (version, build)
+            version = f'{version}+{build}'
 
         return cls(version, revision=revision)
 
     @classmethod
     def parse(cls, version_string):
         """Parse a version string into a tuple of components:
            (major, minor, patch, revision, prerelease, build).
 
         Args:
             version_string (str), the version string to parse
         """
         if not version_string:
-            raise ValueError('Invalid empty version string: %r' % version_string)
+            raise ValueError(f'Invalid empty version string: "{version_string}"')
 
         version_re = cls.version_re
 
         match = version_re.match(version_string)
         if not match:
-            raise ValueError('Invalid version string: %r' % version_string)
+            raise ValueError(f'Invalid version string: "{version_string}"')
 
         major, minor, patch, revision, prerelease, build = match.groups()
 
         if _has_leading_zero(major):
-            raise ValueError('Invalid leading zero in major: %r' % version_string)
+            raise ValueError(f'Invalid leading zero in major: "{version_string}"')
         if _has_leading_zero(minor):
-            raise ValueError('Invalid leading zero in minor: %r' % version_string)
+            raise ValueError(f'Invalid leading zero in minor: "{version_string}"')
         if _has_leading_zero(patch):
-            raise ValueError('Invalid leading zero in patch: %r' % version_string)
+            raise ValueError(f'Invalid leading zero in patch: "{version_string}"')
 
         major = int(major)
         minor = cls._coerce(minor)
         patch = cls._coerce(patch)
         revision = int(revision) if revision else 0
         if revision < 0:
             raise ValueError(
-                'Invalid revision number, must be an integer greater than or equal to 0'
+                f'Invalid revision number in "{version_string}", must be an integer greater than or equal to 0'
             )
 
         if not prerelease:
             prerelease = ()
         else:
             prerelease = tuple(prerelease.split('.'))
             cls._validate_identifiers(prerelease, allow_leading_zeroes=False)
@@ -301,19 +302,19 @@
         return major, minor, patch, revision, prerelease, build
 
     @classmethod
     def _validate_identifiers(cls, identifiers, allow_leading_zeroes=False):
         for item in identifiers:
             if not item:
                 raise ValueError(
-                    'Invalid empty identifier %r in %r' % (item, '.'.join(identifiers))
+                    'Invalid empty identifier {!r} in {!r}'.format(item, '.'.join(identifiers))
                 )
 
             if item[0] == '0' and item.isdigit() and item != '0' and not allow_leading_zeroes:
-                raise ValueError('Invalid leading zero in identifier %r' % item)
+                raise ValueError(f'Invalid leading zero in identifier {item!r}')
 
     @classmethod
     def _validate_kwargs(cls, major, minor, patch, revision, prerelease, build):
         if (
             major != int(major)
             or minor != cls._coerce(minor)
             or patch != cls._coerce(patch)
@@ -325,43 +326,53 @@
             )
         if prerelease is not None:
             cls._validate_identifiers(prerelease, allow_leading_zeroes=False)
         if build is not None:
             cls._validate_identifiers(build, allow_leading_zeroes=True)
 
     def __iter__(self):
-        return iter(
-            (self.major, self.minor, self.patch, self.revision, self.prerelease, self.build)
-        )
+        return iter((
+            self.major,
+            self.minor,
+            self.patch,
+            self.revision,
+            self.prerelease,
+            self.build,
+        ))
 
     def __str__(self):
         version = '%d' % self.major
         if self.minor is not None:
             version = '%s.%d' % (version, self.minor)
         if self.patch is not None:
             version = '%s.%d' % (version, self.patch)
         if self.revision:
             version = '%s~%d' % (version, self.revision)
         if self.prerelease:
-            version = '%s-%s' % (version, '.'.join(self.prerelease))
+            version = '{}-{}'.format(version, '.'.join(self.prerelease))
         if self.build:
-            version = '%s+%s' % (version, '.'.join(self.build))
+            version = '{}+{}'.format(version, '.'.join(self.build))
         return version
 
     def __repr__(self):
         return '%s(%r, revision=%d)' % (
             self.__class__.__name__,
             str(self),
             self.revision,
         )
 
     def __hash__(self):
-        return hash(
-            (self.major, self.minor, self.patch, self.revision, self.prerelease, self.build)
-        )
+        return hash((
+            self.major,
+            self.minor,
+            self.patch,
+            self.revision,
+            self.prerelease,
+            self.build,
+        ))
 
     @property
     def precedence_key(self):
         if self.prerelease:
             prerelease_key = tuple(
                 NumericIdentifier(part) if re.match(r'^[0-9]+$', part) else AlphaIdentifier(part)
                 for part in self.prerelease
@@ -440,18 +451,15 @@
     try:
         Version.parse(version_string)
         return True
     except ValueError:
         return False
 
 
-DEFAULT_SYNTAX = 'simple'
-
-
-class BaseSpec(object):
+class BaseSpec:
     """A specification of compatible versions.
 
     Usage:
     >>> Spec('>=1.0.0', syntax='npm')
 
     A version matches a specification if it matches any
     of the clauses of that specification.
@@ -459,15 +467,15 @@
     Internally, a Spec is AnyOf(
         AllOf(Matcher, Matcher, Matcher),
         AllOf(...),
     )
     """
 
     def __init__(self, expression):
-        super(BaseSpec, self).__init__()
+        super().__init__()
         self.expression = expression
         self.clause = self._parse_to_clause(expression)
 
     @classmethod
     def parse(cls, expression):
         """Convert a syntax-specific expression into a BaseSpec instance."""
         return cls(expression)
@@ -509,32 +517,32 @@
     def __hash__(self):
         return hash(self.clause)
 
     def __str__(self):
         return self.expression
 
     def __repr__(self):
-        return '<%s: %r>' % (self.__class__.__name__, self.expression)
+        return f'<{self.__class__.__name__}: {self.expression!r}>'
 
     @classmethod
-    def _contains_prerelease(cls, clause):  # type: (Clause) -> bool
+    def _contains_prerelease(cls, clause: Clause) -> bool:
         if hasattr(clause, 'clauses'):
             return any(cls._contains_prerelease(c) for c in clause.clauses)
         elif isinstance(clause, Range):
             return bool(clause.target.prerelease)
         else:
             return False
 
     @property
-    def contains_prerelease(self):  # type: () -> bool
+    def contains_prerelease(self) -> bool:
         return self._contains_prerelease(self.clause)
 
 
-class Clause(object):
-    __slots__ = []  # type: list[str]
+class Clause:
+    __slots__: t.List[str] = []
 
     def match(self, version):
         raise NotImplementedError()
 
     def __and__(self, other):
         raise NotImplementedError()
 
@@ -563,15 +571,15 @@
         return self
 
 
 class AnyOf(Clause):
     __slots__ = ['clauses']
 
     def __init__(self, *clauses):
-        super(AnyOf, self).__init__()
+        super().__init__()
         self.clauses = frozenset(clauses)
 
     def match(self, version):
         return any(c.match(version) for c in self.clauses)
 
     def simplify(self):
         subclauses = set()
@@ -604,15 +612,15 @@
         else:
             return NotImplemented
 
     def __or__(self, other):
         if isinstance(other, AnyOf):
             clauses = list(self.clauses | other.clauses)
         elif isinstance(other, Matcher) or isinstance(other, AllOf):
-            clauses = list(self.clauses | set([other]))
+            clauses = list(self.clauses | {other})
         else:
             return NotImplemented
         return AnyOf(*clauses)
 
     def __repr__(self):
         return 'AnyOf(%s)' % ', '.join(sorted(repr(c) for c in self.clauses))
 
@@ -626,15 +634,15 @@
         yield ')'
 
 
 class AllOf(Clause):
     __slots__ = ['clauses']
 
     def __init__(self, *clauses):
-        super(AllOf, self).__init__()
+        super().__init__()
         self.clauses = frozenset(clauses)
 
     def match(self, version):
         return all(clause.match(version) for clause in self.clauses)
 
     def simplify(self):
         subclauses = set()
@@ -657,15 +665,15 @@
         return iter(self.clauses)
 
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.clauses == other.clauses
 
     def __and__(self, other):
         if isinstance(other, Matcher) or isinstance(other, AnyOf):
-            clauses = list(self.clauses | set([other]))
+            clauses = list(self.clauses | {other})
         elif isinstance(other, AllOf):
             clauses = list(self.clauses | other.clauses)
         else:
             return NotImplemented
         return AllOf(*clauses)
 
     def __or__(self, other):
@@ -688,15 +696,15 @@
             for line in lines[:-1]:
                 yield '\t' + line
             yield '\t' + lines[-1] + ','
         yield ')'
 
 
 class Matcher(Clause):
-    __slots__ = []  # type: list[str]
+    __slots__: t.List[str] = []
 
     def __and__(self, other):
         if isinstance(other, AllOf):
             return other & self
         elif isinstance(other, Matcher) or isinstance(other, AnyOf):
             return AllOf(self, other)
         else:
@@ -708,15 +716,15 @@
         elif isinstance(other, Matcher) or isinstance(other, AllOf):
             return AnyOf(self, other)
         else:
             return NotImplemented
 
 
 class Never(Matcher):
-    __slots__ = []  # type: list[str]
+    __slots__: t.List[str] = []
 
     def match(self, version):
         return False
 
     def __hash__(self):
         return hash((Never,))
 
@@ -730,15 +738,15 @@
         return other
 
     def __repr__(self):
         return 'Never()'
 
 
 class Always(Matcher):
-    __slots__ = []  # type: list[str]
+    __slots__: t.List[str] = []
 
     def match(self, version):
         return True
 
     def __hash__(self):
         return hash((Always,))
 
@@ -776,21 +784,19 @@
     BUILD_STRICT = 'strict'
 
     __slots__ = ['operator', 'target', 'prerelease_policy', 'build_policy']
 
     def __init__(
         self, operator, target, prerelease_policy=PRERELEASE_NATURAL, build_policy=BUILD_IMPLICIT
     ):
-        super(Range, self).__init__()
+        super().__init__()
         if target.build and operator not in (self.OP_EQ, self.OP_NEQ):
-            raise ValueError(
-                'Invalid range %s%s: build numbers have no ordering.' % (operator, target)
-            )
+            raise ValueError(f'Invalid range {operator}{target}: build numbers have no ordering.')
         self.operator = operator
-        self.target = target  # type: Version
+        self.target: Version = target
         self.prerelease_policy = prerelease_policy
         self.build_policy = self.BUILD_STRICT if target.build else build_policy
 
     def match(self, version):
         if self.build_policy != self.BUILD_STRICT:
             version = version.truncate('prerelease')
 
@@ -847,31 +853,27 @@
             isinstance(other, self.__class__)
             and self.operator == other.operator
             and self.target == other.target
             and self.prerelease_policy == other.prerelease_policy
         )
 
     def __str__(self):
-        return '%s%s' % (self.operator, self.target)
+        return f'{self.operator}{self.target}'
 
     def __repr__(self):
         policy_part = (
             ''
             if self.prerelease_policy == self.PRERELEASE_NATURAL
-            else ', prerelease_policy=%r' % self.prerelease_policy
+            else f', prerelease_policy={self.prerelease_policy!r}'
         ) + (
             ''
             if self.build_policy == self.BUILD_IMPLICIT
-            else ', build_policy=%r' % self.build_policy
-        )
-        return 'Range(%r, %r%s)' % (
-            self.operator,
-            self.target,
-            policy_part,
+            else f', build_policy={self.build_policy!r}'
         )
+        return f'Range({self.operator!r}, {self.target!r}{policy_part})'
 
 
 class SimpleSpec(BaseSpec):
     @classmethod
     def _parse_to_clause(cls, expression):
         return cls.Parser.parse(expression)
 
@@ -881,39 +883,37 @@
         # remove the \n and the extra spaces
         naive_spec_string = ''.join([line.strip() for line in naive_spec_string.split()])
         # remove the name group
         naive_spec_string = re.sub(r'\(\?P<\w+>', '(?:', naive_spec_string)
         # remove the first ^ and the last $ and make it as a group
         naive_spec_group = '(' + naive_spec_string[1:-1] + ')'
         # ^group(,group)*$ means it could be a comma separated lists
-        return '^{}(,{})*$'.format(naive_spec_group, naive_spec_group)
+        return f'^{naive_spec_group}(,{naive_spec_group})*$'
 
     class Parser:
         NUMBER = r'\*|0|[1-9][0-9]*'
         NAIVE_SPEC = re.compile(
             r"""^
             (?P<op><|<=||=|==|>=|>|!=|\^|~|~=)
             (?P<major>{nb})(?:\.(?P<minor>{nb})(?:\.(?P<patch>{nb}))?)?
             (?:~(?P<revision>\d+))?
             (?:-(?P<prerel>[a-z0-9A-Z.-]*))?
             (?:\+(?P<build>[a-z0-9A-Z.-]*))?
             $
-            """.format(
-                nb=NUMBER
-            ),
+            """.format(nb=NUMBER),
             re.VERBOSE,
         )
 
         @classmethod
         def parse(cls, expression):
             blocks = expression.split(',')
             clause = Always()
             for block in blocks:
                 if not cls.NAIVE_SPEC.match(block):
-                    raise ValueError('Invalid simple block %r' % block)
+                    raise ValueError(f'Invalid simple block {block!r}')
                 clause &= cls.parse_block(block)
 
             return clause
 
         PREFIX_CARET = '^'
         PREFIX_TILDE = '~'
         PREFIX_COMPATIBLE = '~='
@@ -930,35 +930,35 @@
         }
 
         EMPTY_VALUES = ['*', 'x', 'X', None]
 
         @classmethod
         def parse_block(cls, expr):
             if not cls.NAIVE_SPEC.match(expr):
-                raise ValueError('Invalid simple spec component: %r' % expr)
+                raise ValueError(f'Invalid simple spec component: {expr!r}')
             prefix, major_t, minor_t, patch_t, revision, prerel, build = cls.NAIVE_SPEC.match(
                 expr
             ).groups()
             prefix = cls.PREFIX_ALIASES.get(prefix, prefix)
 
             major = None if major_t in cls.EMPTY_VALUES else int(major_t)
             minor = None if minor_t in cls.EMPTY_VALUES else int(minor_t)
             patch = None if patch_t in cls.EMPTY_VALUES else int(patch_t)
             revision = None if revision in cls.EMPTY_VALUES else int(revision)
 
             if (major is None or minor is None or patch is None) and (revision or prerel or build):
-                raise ValueError('Invalid simple spec: %r' % expr)
+                raise ValueError(f'Invalid simple spec: {expr!r}')
 
             if build is not None and prefix not in (cls.PREFIX_EQ, cls.PREFIX_NEQ):
-                raise ValueError('Invalid simple spec: %r' % expr)
+                raise ValueError(f'Invalid simple spec: {expr!r}')
 
             if major is None:  # '*'
                 target = Version(major=0, minor=0, patch=0)
                 if prefix not in (cls.PREFIX_EQ, cls.PREFIX_GTE):
-                    raise ValueError('Invalid simple spec: %r' % expr)
+                    raise ValueError(f'Invalid simple spec: {expr!r}')
             elif minor is None:
                 target = Version(major=major, minor=0, patch=0)
             elif patch is None:
                 target = Version(major=major, minor=minor, patch=0)
             else:
                 target = Version(
                     major=major,
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/sources/base.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/sources/git.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,226 +1,189 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import os
-from abc import ABCMeta, abstractmethod
+import re
+import shutil
+import tempfile
+import typing as t
+
+from idf_component_tools.constants import MANIFEST_FILENAME
+from idf_component_tools.errors import FetchingError
+from idf_component_tools.file_tools import copy_filtered_directory
+from idf_component_tools.git_client import GitClient
+from idf_component_tools.hash_tools.calculate import hash_dir, hash_url
+from idf_component_tools.manager import ManifestManager
+from idf_component_tools.utils import (
+    ComponentVersion,
+    ComponentWithVersions,
+    HashedComponentVersion,
+    Literal,
+)
 
-from schema import Optional, Or
-from six import string_types
+from .base import BaseSource
 
-import idf_component_tools as tools
-from idf_component_tools.hash_tools.validate_managed_component import (
-    validate_managed_component_by_manifest,
-)
+if t.TYPE_CHECKING:
+    from idf_component_tools.manifest import SolvedComponent
 
-from ..errors import FetchingError, SourceError
-from ..file_cache import FileCache
-from ..semver import SimpleSpec
-
-try:
-    from typing import TYPE_CHECKING, Callable
-
-    if TYPE_CHECKING:
-        from ..manifest import ComponentWithVersions, ManifestManager
-        from ..manifest.solved_component import SolvedComponent
-except ImportError:
-    pass
-
-VALUE_TYPES = {
-    'str': Or(*string_types),
-    'bool': bool,
-}
-
-
-class BaseSource(object):
-    __metaclass__ = ABCMeta
-    NAME = 'base'
+BRANCH_TAG_RE = re.compile(
+    r'^(?!.*/\.)(?!.*\.\.)(?!/)(?!.*//)(?!.*@\{)(?!.*\\)[^\177\s~^:?*\[]+[^.]$'
+)
 
-    def __init__(
-        self,
-        source_details=None,  # type: dict | None
-        system_cache_path=None,  # type: str | None
-        manifest_manager=None,  # type: ManifestManager | None
-    ):  # type: (...) -> None
-        self._source_details = source_details or {}
-        self._hash_key = None
-
-        if system_cache_path is None:
-            system_cache_path = FileCache().path()
-        self.system_cache_path = system_cache_path
-
-        self.is_overrider = False
-
-        unknown_keys = [key for key in self._source_details.keys() if key not in self.known_keys()]
-        if unknown_keys:
-            raise SourceError('Unknown keys in dependency details: %s' % ', '.join(unknown_keys))
 
-        self._manifest_manager = manifest_manager
+class GitSource(BaseSource):
+    type: Literal['git'] = 'git'  # type: ignore
+    git: str
+    path: str = '.'
 
-    def _hash_values(self):
-        return self.name, self.hash_key
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
 
-    def cache_path(self):  # type: () -> str
-        path = os.path.join(self.system_cache_path, '{}_{}'.format(self.NAME, self.hash_key[:8]))
-        return path
+        self._client = GitClient()
 
-    def __eq__(self, other):  # type: (object) -> bool
-        if not isinstance(other, BaseSource):
-            return NotImplemented
-
-        return self._hash_values() == other._hash_values() and self.name == other.name
-
-    def __hash__(self):
-        return hash(self._hash_values())
-
-    def __repr__(self):  # type: () -> str
-        return '{}({})'.format(type(self).__name__, self.hash_key)
-
-    @staticmethod
-    def fromdict(
-        name,  # type: str
-        details,  # type: dict
-        manifest_manager=None,  # type: ManifestManager | None
-    ):  # type: (...) -> list[BaseSource]
-        """Build component source by dict"""
-        for source_class in tools.sources.KNOWN_SOURCES:
-            # MARKER
-            sources = source_class.build_if_valid(name, details, manifest_manager)
-
-            if sources:
-                return sources
-            else:
-                continue
-
-        raise SourceError('Unknown source for component: %s' % name)
-
-    @staticmethod
-    def create_sources_if_valid(
-        name, details, manifest_manager=None
-    ):  # type: (str, dict, ManifestManager | None) -> list[BaseSource] | None
-        return None
-
-    @classmethod
-    def required_keys(cls):
-        return {}
-
-    @classmethod
-    def optional_keys(cls):
-        return {}
-
-    @classmethod
-    def known_keys(cls):  # type: () -> list[str]
-        """List of known details key"""
-        return (
-            ['version', 'public', 'matches', 'rules', 'require']
-            + list(cls.required_keys().keys())
-            + list(cls.optional_keys().keys())
+    def _checkout_git_source(
+        self,
+        version: t.Union[str, ComponentVersion, None],
+        path: str,
+        selected_paths: t.Optional[t.List[str]] = None,
+    ) -> str:
+        if version is not None:
+            version = None if version == '*' else str(version)
+        return self._client.prepare_ref(
+            repo=self.git,
+            bare_path=self.cache_path(),
+            checkout_path=path,
+            ref=version,
+            with_submodules=True,
+            selected_paths=selected_paths,
         )
 
-    @classmethod
-    def schema(cls):  # type: () -> dict
-        """Schema for lock file"""
-        source_schema = {'type': cls.NAME}  # type: dict[str, str | Callable]
-
-        for key, type_field in cls.required_keys().items():
-            source_schema[key] = VALUE_TYPES[type_field]
-
-        for key, type_field in cls.optional_keys().items():
-            source_schema[Optional(key)] = VALUE_TYPES[type_field]
-
-        return source_schema
-
-    @classmethod
-    def build_if_valid(cls, name, details, manifest_manager=None):
-        """Returns source if details are matched, otherwise returns None"""
-        return cls.create_sources_if_valid(name, details, manifest_manager)
-
     @property
-    def source_details(self):
-        return self._source_details
+    def component_hash_required(self) -> bool:
+        return True
 
     @property
-    def name(self):
-        return self.NAME
+    def downloadable(self) -> bool:
+        return True
 
     @property
     def hash_key(self):
-        """Hash key is used for comparison sources initialised with different settings"""
-        return 'Base'
+        if self._hash_key is None:
+            self._hash_key = hash_url(self.git)
+        return self._hash_key
 
     @property
-    def component_hash_required(self):  # type: () -> bool
-        """Returns True if component's hash have to present and be validated"""
-        return False
+    def volatile(self) -> bool:
+        return True
 
-    @property
-    def downloadable(self):  # type: () -> bool
-        """Returns True if components have to be fetched"""
-        return False
+    def cache_path(self):
+        # Using `b_` prefix for bare git repos in cache
+        path = os.path.join(self.system_cache_path, 'b_{}_{}'.format(self.type, self.hash_key[:8]))
+        return path
 
-    @property
-    def meta(self):  # type: () -> bool
-        """
-        Returns True for meta components.
-        Meta components are not included in the build directly
-        """
-        return False
+    def download(self, component: 'SolvedComponent', download_path: str) -> t.Optional[str]:
+        # Check for required components
+        if not component.component_hash:
+            raise FetchingError('Component hash is required for components from git repositories')
 
-    @property
-    def volatile(self):  # type: () -> bool
-        """
-        Returns True for volatile components.
-        Volatile components may change their content, even if their version stays the same.
-        """
-        return False
-
-    def normalized_name(self, name):  # type: (str) -> str
-        return name
-
-    def up_to_date(self, component, path):  # type: (SolvedComponent, str) -> bool
-        if self.component_hash_required and not component.component_hash:
-            raise FetchingError('Cannot install component with unknown hash')
-
-        if self.downloadable:
-            if not os.path.isdir(path):
-                return False
+        if not component.version:
+            raise FetchingError(f'Version should provided for {component.name}')
 
-            if component.component_hash:
-                return validate_managed_component_by_manifest(path, component.component_hash)
+        if self.up_to_date(component, download_path):
+            return download_path
 
-        return True
+        temp_dir = tempfile.mkdtemp()
+        try:
+            self._checkout_git_source(component.version, temp_dir, selected_paths=[self.path])
+            source_path = os.path.join(str(temp_dir), self.path)
+            if not os.path.isdir(source_path):
+                raise FetchingError(
+                    'Directory {} wasn\'t found for the commit id "{}" of the '
+                    'git repository "{}"'.format(self.path, component.version, self.git)
+                )
+
+            if os.path.isdir(download_path):
+                shutil.rmtree(download_path)
+
+            possible_manifest_filepath = os.path.join(source_path, MANIFEST_FILENAME)
+            include, exclude = set(), set()
+            if os.path.isfile(possible_manifest_filepath):
+                manifest = ManifestManager(possible_manifest_filepath, component.name).load()
+                include.update(manifest.include_set)
+                exclude.update(manifest.exclude_set)
+
+            copy_filtered_directory(source_path, download_path, include=include, exclude=exclude)
+        finally:
+            shutil.rmtree(temp_dir)
+
+        return download_path
+
+    def versions(self, name, spec='*', target=None):
+        """For git returns hash of locked commit, ignoring manifest"""
+        version = None if spec == '*' else spec
+        temp_dir = tempfile.mkdtemp()
+        try:
+            commit_id = self._checkout_git_source(version, temp_dir, selected_paths=[self.path])
+            source_path = os.path.join(str(temp_dir), self.path)
 
-    def validate_version_spec(self, spec):  # type: (str) -> bool
+            if not os.path.isdir(source_path):
+                dependency_description = f'commit id "{commit_id}"'
+                if version:
+                    dependency_description = 'version "{}" ({})'.format(
+                        version, dependency_description
+                    )
+                raise FetchingError(
+                    'Directory {} wasn\'t found for the {} of the git repository "{}"'.format(
+                        self.path, dependency_description, self.git
+                    )
+                )
+
+            manifest_path = os.path.join(source_path, MANIFEST_FILENAME)
+            targets = []
+            dependencies = []
+            include = set()
+            exclude = set()
+
+            if os.path.isfile(manifest_path):
+                manifest = ManifestManager(manifest_path, name=name).load()
+                dependencies = manifest.raw_requirements
+
+                if manifest.targets:  # only check when exists
+                    if target and target not in manifest.targets:
+                        raise FetchingError(
+                            'Version "{}" (commit id "{}") of the component "{}" '
+                            'does not support target "{}"'.format(version, commit_id, name, target)
+                        )
+
+                    targets = manifest.targets
+
+                    include = manifest.include_set
+                    exclude = manifest.exclude_set
+
+            component_hash = hash_dir(source_path, include=include, exclude=exclude)
+        finally:
+            shutil.rmtree(temp_dir)
+
+        return ComponentWithVersions(
+            name=name,
+            versions=[
+                HashedComponentVersion(
+                    commit_id,
+                    targets=targets,
+                    component_hash=component_hash,
+                    dependencies=dependencies,
+                )
+            ],
+        )
+
+    def validate_version_spec(self, spec: str) -> bool:
         if not spec or spec == '*':
             return True
 
-        try:
-            return bool(SimpleSpec(spec))
-        except ValueError:
-            return False
+        return bool(BRANCH_TAG_RE.match(spec))
 
-    def normalize_spec(self, spec):  # type: (str) -> str
-        return spec or '*'
-
-    @abstractmethod
-    def versions(
-        self,
-        name,  # type: str
-        details=None,  # type: dict | None
-        spec='*',  # type: str
-        target=None,  # type: str | None
-    ):
-        # type: (...) -> ComponentWithVersions
-        """List of versions for given spec"""
-
-    @abstractmethod
-    def download(self, component, download_path):  # type: (SolvedComponent, str) -> str | None
-        """
-        Fetch required component version from the source
-        Returns list of absolute paths to directories with component on local filesystem
-        """
-
-    @abstractmethod
-    def serialize(self):  # type: () -> dict
-        """
-        Return fields to describe source to be saved in lock file
-        """
+    def normalize_spec(self, spec: str) -> str:
+        if not spec:
+            return '*'
+        ref = None if spec == '*' else spec
+        commit_id = self._client.get_commit_id_by_ref(self.git, self.cache_path(), ref)
+        return commit_id
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/sources/fetcher.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/sources/fetcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,44 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 """Small class that manages getting components to right path using system-wide cache"""
 
 import os
-from io import open
+import typing as t
 
+from idf_component_tools.build_system_tools import build_name
+from idf_component_tools.errors import ComponentModifiedError, InvalidComponentHashError
 from idf_component_tools.hash_tools.constants import HASH_FILENAME
 from idf_component_tools.hash_tools.errors import (
     HashDoesNotExistError,
     HashNotEqualError,
     HashNotSHA256Error,
 )
 from idf_component_tools.hash_tools.validate_managed_component import (
     validate_managed_component_hash,
 )
+from idf_component_tools.manifest import SolvedComponent
 
-from ..build_system_tools import build_name
-from ..errors import ComponentModifiedError, InvalidComponentHashError
-from ..manifest.solved_component import SolvedComponent
+if t.TYPE_CHECKING:
+    from . import BaseSource
 
-try:
-    from typing import TYPE_CHECKING
 
-    if TYPE_CHECKING:
-        from . import BaseSource
-except ImportError:
-    pass
-
-
-class ComponentFetcher(object):
+class ComponentFetcher:
     def __init__(
         self,
-        solved_component,
-        components_path,
-        source=None,
-    ):  # type: (SolvedComponent, str, BaseSource | None) -> None
+        solved_component: SolvedComponent,
+        components_path: str,
+        source: t.Optional['BaseSource'] = None,
+    ) -> None:
         self.source = source if source else solved_component.source
         self.component = solved_component
         self.components_path = components_path
         self.managed_path = os.path.join(self.components_path, build_name(self.component.name))
 
-    def download(self):  # type: () -> str | None
+    def download(self) -> t.Optional[str]:
         """If necessary, it downloads component and returns local path to component directory"""
         try:
             validate_managed_component_hash(self.managed_path)
         except HashNotEqualError:
             raise ComponentModifiedError(
                 'Component directory was modified on the disk since the last run of ' 'the CMake'
             )
@@ -57,14 +51,14 @@
                 'maintainer to remove it.'.format(self.component.name)
             )
         except HashDoesNotExistError:
             pass
 
         return self.source.download(self.component, self.managed_path)
 
-    def create_hash(self, path, component_hash):  # type: (str, None | str) -> None
+    def create_hash(self, path: str, component_hash: t.Optional[str]) -> None:
         if self.component.source.downloadable:
             hash_file = os.path.join(path, HASH_FILENAME)
 
             if not os.path.isfile(hash_file):
                 with open(hash_file, mode='w+', encoding='utf-8') as f:
-                    f.write(u'{}'.format(component_hash))
+                    f.write(f'{component_hash}')
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/sources/git.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/sources/web_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,235 +1,253 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
+"""Component source that downloads components from web service"""
 
 import os
 import re
 import shutil
 import tempfile
-from hashlib import sha256
+import typing as t
 
-from idf_component_tools.hash_tools.calculate import hash_dir
+import requests
+from pydantic import field_validator
 
-from ..errors import FetchingError
-from ..file_tools import copy_filtered_directory
-from ..git_client import GitClient
-from ..manifest import (
-    MANIFEST_FILENAME,
-    ComponentVersion,
-    ComponentWithVersions,
-    HashedComponentVersion,
-    ManifestManager,
+from idf_component_tools.archive_tools import ArchiveError, get_format_from_path, unpack_archive
+from idf_component_tools.constants import (
+    DEFAULT_NAMESPACE,
+    IDF_COMPONENT_REGISTRY_URL,
+    UPDATE_SUGGESTION,
 )
+from idf_component_tools.errors import FetchingError
+from idf_component_tools.file_tools import copy_directory
+from idf_component_tools.hash_tools.calculate import hash_url
+from idf_component_tools.messages import hint
+from idf_component_tools.semver import SimpleSpec
+
 from .base import BaseSource
 
-try:
-    from urllib.parse import urlparse  # type: ignore
-except ImportError:
-    from urlparse import urlparse  # type: ignore
-
-try:
-    from typing import TYPE_CHECKING, Dict
-
-    if TYPE_CHECKING:
-        from ..manifest.solved_component import SolvedComponent
-except ImportError:
-    pass
+if t.TYPE_CHECKING:
+    from idf_component_tools.manifest import SolvedComponent
 
-BRANCH_TAG_RE = re.compile(
-    r'^(?!.*/\.)(?!.*\.\.)(?!/)(?!.*//)(?!.*@\{)(?!.*\\)[^\177\s~^:?*\[]+[^.]$'
-)
+from idf_component_tools.utils import Literal
 
+CANONICAL_IDF_COMPONENT_REGISTRY_API_URL = 'https://api.components.espressif.com/'
 
-class GitSource(BaseSource):
-    NAME = 'git'
 
-    def __init__(self, source_details=None, **kwargs):
-        super(GitSource, self).__init__(source_details=source_details, **kwargs)
-        self.git_repo = self.source_details['git']
-        self.component_path = self.source_details.get('path') or '.'
-
-        self._client = GitClient()
-
-    def _checkout_git_source(
-        self,
-        version,  # type: str | ComponentVersion | None
-        path,  # type: str
-        selected_paths=None,  # type: list[str] | None
-    ):  # type: (...) -> str
-        if version is not None:
-            version = None if version == '*' else str(version)
-        return self._client.prepare_ref(
-            repo=self.git_repo,
-            bare_path=self.cache_path(),
-            checkout_path=path,
-            ref=version,
-            with_submodules=True,
-            selected_paths=selected_paths,
-        )
+def download_archive(url: str, download_dir: str, save_original_filename: bool = False) -> str:
+    from idf_component_tools.registry.base_client import create_session  # avoid circular import
 
-    @staticmethod
-    def create_sources_if_valid(
-        name, details, manifest_manager=None
-    ):  # type: (str, dict, ManifestManager | None) -> list[BaseSource] | None
-        if details.get('git', None):
-            return [GitSource(details, manifest_manager=manifest_manager)]
-        return None
+    session = create_session(cache=False)
 
-    @classmethod
-    def required_keys(cls):
-        return {'git': 'str'}
+    try:
+        with session.get(url, stream=True, allow_redirects=True) as r:  # type: requests.Response
+            # Trying to get extension from url
+            original_filename = url.split('/')[-1]
 
-    @classmethod
-    def optional_keys(cls):
-        return {'path': 'str'}
+            try:
+                extension = get_format_from_path(original_filename)[1]
+            except ArchiveError:
+                extension = None
 
-    @property
-    def component_hash_required(self):  # type: () -> bool
-        return True
+            if r.status_code != 200:
+                raise FetchingError(f'Server returned HTTP code {r.status_code}')
+
+            # If didn't find anything useful, trying content disposition
+            content_disposition = r.headers.get('content-disposition')
+            if not extension and content_disposition:
+                filenames = re.findall('filename=(.+)', content_disposition)
+                try:
+                    extension = get_format_from_path(filenames[0])[1]
+                except IndexError:
+                    raise FetchingError('Web Service returned invalid download url')
+
+            filename = original_filename
+            if not save_original_filename:
+                filename = f'component.{extension}'
+
+            tmp_file_path = os.path.join(download_dir, f'{filename}.tmp')
+
+            with open(tmp_file_path, 'wb') as f:
+                for chunk in r.iter_content(chunk_size=65536):
+                    if chunk:
+                        f.write(chunk)
+
+            file_path = os.path.join(download_dir, filename)
+            if os.path.exists(file_path):
+                os.remove(file_path)
+            shutil.move(tmp_file_path, file_path)
+
+            return file_path
+    except requests.exceptions.RequestException as e:
+        raise FetchingError(str(e))
+
+
+class WebServiceSource(BaseSource):
+    service_url: str = None  # type: ignore
+    type: Literal['service'] = 'service'  # type: ignore
+    pre_release: bool = None  # type: ignore
+
+    @field_validator('service_url')
+    @classmethod
+    def validate_service_url(cls, v):
+        # Use canonical API url for lock file
+        if not v or v == IDF_COMPONENT_REGISTRY_URL:
+            return CANONICAL_IDF_COMPONENT_REGISTRY_API_URL
+
+        return v
+
+    def model_post_init(self, __context: t.Any) -> None:
+        if not self.base_url:
+            FetchingError('Cannot fetch a dependency with when registry is not defined')
 
     @property
-    def downloadable(self):  # type: () -> bool
-        return True
+    def base_url(self) -> str:
+        # Use the default URL, even if the lock file was made with the canonical one
+        return (
+            IDF_COMPONENT_REGISTRY_URL
+            if self.service_url == CANONICAL_IDF_COMPONENT_REGISTRY_API_URL
+            else self.service_url
+        ) or IDF_COMPONENT_REGISTRY_URL
 
     @property
     def hash_key(self):
         if self._hash_key is None:
-            url = urlparse(self.git_repo)
-            netloc = url.netloc
-            path = '/'.join(filter(None, url.path.split('/')))
-            normalized_path = '/'.join([netloc, path])
-            self._hash_key = sha256(normalized_path.encode('utf-8')).hexdigest()
+            self._hash_key = hash_url(self.base_url)
         return self._hash_key
 
-    @property
-    def volatile(self):  # type: () -> bool
-        return True
-
-    def cache_path(self):
-        # Using `b_` prefix for bare git repos in cache
-        path = os.path.join(self.system_cache_path, 'b_{}_{}'.format(self.NAME, self.hash_key[:8]))
+    def component_cache_path(self, component: 'SolvedComponent') -> str:
+        component_dir_name = '_'.join([
+            self.normalized_name(component.name).replace('/', '__'),
+            str(component.version),
+            str(component.component_hash)[:8],
+        ])
+        path = os.path.join(self.cache_path(), component_dir_name)
         return path
 
-    def download(self, component, download_path):  # type: (SolvedComponent, str) -> str | None
-        # Check for required components
-        if not component.component_hash:
-            raise FetchingError('Component hash is required for components from git repositories')
-
-        if not component.version:
-            raise FetchingError('Version should provided for %s' % component.name)
-
-        if self.up_to_date(component, download_path):
-            return download_path
+    def versions(self, name, spec='*', target=None):
+        from idf_component_tools.registry.service_details import (
+            get_storage_client,  # avoid circular import
+        )
 
-        temp_dir = tempfile.mkdtemp()
-        try:
-            self._checkout_git_source(
-                component.version, temp_dir, selected_paths=[self.component_path]
-            )
-            source_path = os.path.join(str(temp_dir), self.component_path)
-            if not os.path.isdir(source_path):
-                raise FetchingError(
-                    'Directory {} wasn\'t found for the commit id "{}" of the '
-                    'git repository "{}"'.format(
-                        self.component_path, component.version, self.git_repo
+        client = get_storage_client(self.base_url)
+        if self.base_url != client.registry_url:
+            client.registry_url = self.base_url
+
+        cmp_with_versions = client.versions(component_name=self.normalized_name(name), spec=spec)
+
+        versions = []
+        other_targets_versions = []
+        pre_release_versions = []
+        newer_component_manager_versions = []
+
+        for version in cmp_with_versions.versions:
+            if target and version.targets and target not in version.targets:
+                other_targets_versions.append(version)
+                continue
+
+            if (
+                not self.pre_release
+                and version.semver.prerelease
+                and not SimpleSpec(spec).contains_prerelease
+            ):
+                pre_release_versions.append(str(version))
+                continue
+
+            if not version.all_build_keys_known:
+                newer_component_manager_versions.append(str(version))
+                continue
+
+            versions.append(version)
+
+        cmp_with_versions.versions = versions
+        if not versions:
+            current_target = f'"{target}"' if target else ''
+
+            if pre_release_versions:
+                hint(
+                    'Component "{}" has some pre-release versions: "{}" '
+                    'satisfies your requirements. '
+                    'To allow pre-release versions add "pre_release: true" '
+                    'to the dependency in the manifest.'.format(
+                        name, '", "'.join(pre_release_versions)
                     )
                 )
 
-            if os.path.isdir(download_path):
-                shutil.rmtree(download_path)
+            if other_targets_versions:
+                targets = {t for v in other_targets_versions for t in v.targets}
+                hint(
+                    'Component "{}" has suitable versions for other targets: "{}". '
+                    'Is your current target {} set correctly?'.format(
+                        name, '", "'.join(targets), current_target
+                    )
+                )
 
-            possible_manifest_filepath = os.path.join(source_path, MANIFEST_FILENAME)
-            include, exclude = set(), set()
-            if os.path.isfile(possible_manifest_filepath):
-                manifest = ManifestManager(possible_manifest_filepath, component.name).load()
-                include.update(manifest.files['include'])
-                exclude.update(manifest.files['exclude'])
+            if newer_component_manager_versions:
+                hint(
+                    'Component "{}" has versions "{}" '
+                    'that support only newer version of idf-component-manager '
+                    'that satisfy your requirements.\n'
+                    '{}'.format(
+                        name, '", "'.join(newer_component_manager_versions), UPDATE_SUGGESTION
+                    )
+                )
 
-            copy_filtered_directory(source_path, download_path, include=include, exclude=exclude)
-        finally:
-            shutil.rmtree(temp_dir)
+        return cmp_with_versions
 
-        return download_path
+    @property
+    def component_hash_required(self) -> bool:
+        return True
 
-    def versions(self, name, details=None, spec='*', target=None):
-        """For git returns hash of locked commit, ignoring manifest"""
-        version = None if spec == '*' else spec
-        temp_dir = tempfile.mkdtemp()
-        try:
-            commit_id = self._checkout_git_source(
-                version, temp_dir, selected_paths=[self.component_path]
-            )
-            source_path = os.path.join(str(temp_dir), self.component_path)
+    @property
+    def downloadable(self) -> bool:
+        return True
 
-            if not os.path.isdir(source_path):
-                dependency_description = 'commit id "{}"'.format(commit_id)
-                if version:
-                    dependency_description = 'version "{}" ({})'.format(
-                        version, dependency_description
-                    )
-                raise FetchingError(
-                    'Directory {} wasn\'t found for the {} of the git repository "{}"'.format(
-                        self.component_path, dependency_description, self.git_repo
-                    )
-                )
+    def normalized_name(self, name):
+        if '/' not in name:
+            name = '/'.join([DEFAULT_NAMESPACE, name])
+
+        return name
+
+    def download(self, component: 'SolvedComponent', download_path: str) -> str:
+        from idf_component_tools.hash_tools.validate_managed_component import (
+            validate_managed_component_by_manifest,  # avoid circular import
+        )
+        from idf_component_tools.registry.storage_client import (
+            StorageClient,  # avoid circular import
+        )
 
-            manifest_path = os.path.join(source_path, MANIFEST_FILENAME)
-            targets = []
-            dependencies = []
-            include = set()
-            exclude = set()
-
-            if os.path.isfile(manifest_path):
-                manifest = ManifestManager(manifest_path, name=name).load()
-                dependencies = manifest.dependencies
-
-                if manifest.targets:  # only check when exists
-                    if target and target not in manifest.targets:
-                        raise FetchingError(
-                            'Version "{}" (commit id "{}") of the component "{}" '
-                            'does not support target "{}"'.format(version, commit_id, name, target)
-                        )
+        # Check for required components
+        if not component.component_hash:
+            raise FetchingError('Component hash is required for components from web service')
 
-                    targets = manifest.targets
+        if not component.version:
+            raise FetchingError(f'Version should be provided for {component.name}')
 
-                    include = set(manifest.files['include'])
-                    exclude = set(manifest.files['exclude'])
+        if self.up_to_date(component, download_path):
+            return download_path
 
-            component_hash = hash_dir(source_path, include=include, exclude=exclude)
-        finally:
-            shutil.rmtree(temp_dir)
+        # Check if component is in the cache
+        if validate_managed_component_by_manifest(
+            self.component_cache_path(component), component.component_hash
+        ):
+            copy_directory(self.component_cache_path(component), download_path)
+            return download_path
 
-        return ComponentWithVersions(
-            name=name,
-            versions=[
-                HashedComponentVersion(
-                    commit_id,
-                    targets=targets,
-                    component_hash=component_hash,
-                    dependencies=dependencies,
+        tempdir = tempfile.mkdtemp()
+        try:
+            url = StorageClient(component.download_url).component(
+                component.name, component.version
+            )['download_url']
+
+            file_path = download_archive(url, tempdir)
+            unpack_archive(file_path, self.component_cache_path(component))
+            copy_directory(self.component_cache_path(component), download_path)
+        except (KeyError, FetchingError) as e:
+            raise FetchingError(
+                'Cannot download component {}@{}. {}'.format(
+                    component.name, component.version, str(e)
                 )
-            ],
-        )
+            )
+        finally:
+            shutil.rmtree(tempdir)
 
-    def serialize(self):  # type: () -> Dict
-        source = {
-            'git': self.git_repo,
-            'type': self.name,
-        }
-
-        if self.component_path:
-            source['path'] = self.component_path
-
-        return source
-
-    def validate_version_spec(self, spec):  # type: (str) -> bool
-        if not spec or spec == '*':
-            return True
-
-        return bool(BRANCH_TAG_RE.match(spec))
-
-    def normalize_spec(self, spec):  # type: (str) -> str
-        if not spec:
-            return '*'
-        ref = None if spec == '*' else spec
-        commit_id = self._client.get_commit_id_by_ref(self.git_repo, self.cache_path(), ref)
-        return commit_id
+        return download_path
```

### Comparing `idf_component_manager-1.5.2/idf_component_tools/sources/local.py` & `idf_component_manager-2.0.0.dev0/idf_component_tools/sources/local.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,173 +1,149 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import os
+import typing as t
 from pathlib import Path
 
-from ..errors import SourceError
-from ..manifest import (
-    MANIFEST_FILENAME,
-    ComponentWithVersions,
-    HashedComponentVersion,
-    ManifestManager,
-)
-from ..messages import warn
-from .base import BaseSource
-from .web_service_keys import WEB_SERVICE_OPTIONAL_KEYS
+from pydantic import model_serializer
+from pydantic_core.core_schema import SerializerFunctionWrapHandler
 
-try:
-    from typing import Dict
-except ImportError:
-    pass
+from idf_component_tools.constants import MANIFEST_FILENAME
+from idf_component_tools.errors import InternalError, SourceError
+from idf_component_tools.manager import ManifestManager
+from idf_component_tools.messages import warn
+from idf_component_tools.utils import ComponentWithVersions, HashedComponentVersion, Literal
+
+from .base import BaseSource
 
 
 class ManifestContextError(SourceError):
     pass
 
 
 class SourcePathError(SourceError):
     pass
 
 
 class LocalSource(BaseSource):
-    NAME = 'local'
+    type: Literal['local'] = 'local'  # type: ignore
+    path: t.Optional[str] = None
+    override_path: t.Optional[str] = None
+
+    def model_post_init(self, __context: t.Any) -> None:
+        if not self.path and not self.override_path:
+            raise SourceError('Either "path" or "override_path" must be specified for local source')
+
+    @model_serializer(mode='wrap')
+    def serialize_model(self, handler: SerializerFunctionWrapHandler) -> t.Dict[str, t.Any]:
+        # serialize from flat dict to {'name': {...}}
+        d = handler(self)
+
+        # only use path in the lock file
+        # turn override path into path
+        d['path'] = str(self._path)
+        d.pop('override_path', None)
 
-    def __init__(self, source_details, **kwargs):
-        super(LocalSource, self).__init__(source_details=source_details, **kwargs)
-
-        self.is_overrider = 'override_path' in self.source_details
-        self._raw_path = Path(
-            self.source_details.get('override_path' if self.is_overrider else 'path')
-        )
+        return d
 
     @property
-    def _path(self):  # type: () -> Path
-        try:
-            if self._manifest_manager:
-                path = (Path(self._manifest_manager.path).parent / self._raw_path).resolve()
-            elif not self._manifest_manager and self._raw_path.is_absolute():
-                path = self._raw_path.resolve()
-            else:
-                raise ManifestContextError(
-                    "Can't reliably evaluate relative path without context: {}".format(
-                        str(self._raw_path)
-                    )
-                )
+    def is_overrider(self) -> bool:
+        return bool(self.override_path)
 
-            if not path.is_dir():  # for Python > 3.6, where .resolve(strict=False)
-                raise OSError()
+    @property
+    def _path(self) -> Path:
+        if self.override_path:
+            if self.path:
+                warn('Both "path" and "override_path" are set. "override_path" will be used.')
+            _raw_path = Path(self.override_path)
+            field_name = 'override_path'
+        elif self.path:
+            _raw_path = Path(self.path)
+            field_name = 'path'
+        else:
+            raise InternalError()
+
+        if _raw_path.is_absolute():
+            path = _raw_path.resolve()
+        elif self._manifest_manager:
+            path = (Path(self._manifest_manager.path).parent / _raw_path).resolve()
+        else:
+            raise ManifestContextError(
+                "Can't reliably evaluate relative path without context: {}".format(str(_raw_path))
+            )
 
-        except OSError:
+        if not path.is_dir():  # for Python > 3.6, where .resolve(strict=False)
             raise SourcePathError(
-                "The 'override_path' field in the manifest file '{}' "
-                'does not point to a directory. You can safely '
-                'remove this field from the manifest if this project '
-                'is an example copied from a component '
-                'repository. The dependency will be downloaded from '
-                'the ESP component registry. Documentation: '
+                f'The "{field_name}" field in the manifest file "{path / MANIFEST_FILENAME}" '
+                'does not point to a directory. '
+                'You can safely remove this field from the manifest '
+                'if this project is an example copied from a component repository. '
+                'The dependency will be downloaded from the ESP component registry. '
+                'Documentation: '
                 'https://docs.espressif.com/projects/idf-component-manager/en/latest/reference/'
-                'manifest_file.html'
-                '#override-path'.format(str(self._raw_path / 'idf_component.yml'))
+                'manifest_file.html#override-path'
             )
 
         if self.is_overrider and path / 'CMakeLists.txt' not in path.iterdir():
             raise SourcePathError(
-                'The override_path you\'re using is pointing'
+                "The override_path you're using is pointing"
                 ' to directory "%s" that is not a component.' % str(path)
             )
 
         return path
 
     @property
-    def component_hash_required(self):  # type: () -> bool
-        return False
-
-    @classmethod
-    def required_keys(cls):
-        return {'path': 'str'}
-
-    @classmethod
-    def optional_keys(cls):
-        # support `web_service` fields for override_path source changing
-        local_keys = {'override_path': 'str'}
-        local_keys.update(WEB_SERVICE_OPTIONAL_KEYS)
-        return local_keys
-
-    @staticmethod
-    def create_sources_if_valid(name, details, manifest_manager=None):
-        if details.get('path', None) or 'override_path' in details:
-            return [LocalSource(details, manifest_manager=manifest_manager)]
-        return None
-
-    @property
-    def hash_key(self):
-        return self.source_details.get('path')
+    def hash_key(self) -> str:
+        return self.path or self.override_path  # type: ignore
 
     @property
-    def volatile(self):  # type: () -> bool
+    def volatile(self) -> bool:
         return True
 
     def download(self, component, download_path):
         directory_name = os.path.basename(str(self._path))
         component_with_namespace = component.name.replace('/', '__')
         namespace_and_component = component.name.split('/')
         component_without_namespace = namespace_and_component[-1]
         if (
             component_without_namespace != directory_name
             and component_with_namespace != directory_name
         ):
             alternative_name = (
-                ' or "{}"'.format(component_with_namespace)
-                if len(namespace_and_component) == 2
-                else ''
+                f' or "{component_with_namespace}"' if len(namespace_and_component) == 2 else ''
             )
             warn(
                 'Component name "{component_name}" doesn\'t match the '
                 'directory name "{directory_name}".\n'.format(
                     component_name=component.name,
                     directory_name=directory_name,
                 )
                 + 'ESP-IDF CMake build system uses directory names as names '
                 + 'of components, so different names may break '
                 + 'requirements resolution. To avoid the problem rename the component directory to '
-                + '"{component_without_namespace}"{alternative_name}'.format(
-                    component_without_namespace=component_without_namespace,
-                    alternative_name=alternative_name,
-                )
+                + f'"{component_without_namespace}"{alternative_name}'
             )
         return str(self._path)
 
-    def versions(self, name, details=None, spec='*', target=None):
+    def versions(self, name, spec='*', target=None):
         """For local return version from manifest, or * if manifest not found"""
-        manifest_path = self._path / MANIFEST_FILENAME
         name = self._path.name
 
         version_str = '*'
-        targets = []
-        dependencies = []
+        manifest = ManifestManager(str(self._path), name).load()
+        if manifest.version:
+            version_str = str(manifest.version)
+
+        if manifest.targets:  # only check when exists
+            if target and target not in manifest.targets:
+                return ComponentWithVersions(name=name, versions=[])
 
-        if manifest_path.is_file():
-            manifest = ManifestManager(str(manifest_path), name=name).load()
-            if manifest.version:
-                version_str = str(manifest.version)
-
-            if manifest.targets:  # only check when exists
-                if target and target not in manifest.targets:
-                    return ComponentWithVersions(name=name, versions=[])
-
-                targets = manifest.targets
-
-            dependencies = manifest.dependencies
+        targets = manifest.targets
+        dependencies = manifest.raw_requirements
 
         return ComponentWithVersions(
             name=name,
             versions=[
                 HashedComponentVersion(version_str, targets=targets, dependencies=dependencies)
             ],
         )
-
-    def serialize(self):  # type: () -> Dict
-        return {
-            'path': str(self._path),
-            'type': self.name,
-        }
```

