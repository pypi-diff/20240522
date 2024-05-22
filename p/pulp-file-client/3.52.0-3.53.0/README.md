# Comparing `tmp/pulp_file-client-3.52.0.tar.gz` & `tmp/pulp_file-client-3.53.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp_file-client-3.52.0.tar", last modified: Tue Apr 23 16:17:54 2024, max compression
+gzip compressed data, was "pulp_file-client-3.53.0.tar", last modified: Tue Apr 30 18:17:29 2024, max compression
```

## Comparing `pulp_file-client-3.52.0.tar` & `pulp_file-client-3.53.0.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:17:54.722746 pulp_file-client-3.52.0/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 16:17:54.722746 pulp_file-client-3.52.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15201 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:17:54.706746 pulp_file-client-3.52.0/pulp_file_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulp_file_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulp_file_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulp_file_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulp_file_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulp_file_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:17:54.706746 pulp_file-client-3.52.0/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:17:54.706746 pulp_file-client-3.52.0/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:17:54.706746 pulp_file-client-3.52.0/pulpcore/client/pulp_file/
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:17:54.710746 pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76061 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/acs_file_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25762 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/content_files_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    85036 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/distributions_file_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    56163 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/publications_file_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    86136 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/remotes_file_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    99509 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/repositories_file_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    33822 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/repositories_file_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26280 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13962 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:17:54.714746 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_alternate_content_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_alternate_content_source_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_content.py
--rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_content_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_publication.py
--rw-r--r--   0 runner    (1001) docker     (127)     9429 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    27059 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_remote_response_hidden_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     9907 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/my_permissions_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/nested_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/nested_role_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/object_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginatedfile_file_alternate_content_source_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginatedfile_file_content_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginatedfile_file_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginatedfile_file_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginatedfile_file_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginatedfile_file_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/patchedfile_file_alternate_content_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/patchedfile_file_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    27368 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/patchedfile_file_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/patchedfile_file_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/set_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/set_label_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/task_group_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/unset_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/unset_label_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/pulpcore/client/pulp_file/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 16:17:54.722746 pulp_file-client-3.52.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:17:54.722746 pulp_file-client-3.52.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/test/test_acs_file_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/test/test_content_files_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/test/test_distributions_file_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_file_file_alternate_content_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_file_file_alternate_content_source_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_file_file_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_file_file_content_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_file_file_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_file_file_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_file_file_publication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_file_file_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_file_file_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_file_file_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_file_file_remote_response_hidden_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_file_file_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_file_file_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_my_permissions_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_nested_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_nested_role_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_object_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_paginatedfile_file_alternate_content_source_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_paginatedfile_file_content_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_paginatedfile_file_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_paginatedfile_file_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_paginatedfile_file_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_paginatedfile_file_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_patchedfile_file_alternate_content_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_patchedfile_file_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_patchedfile_file_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_patchedfile_file_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/test/test_publications_file_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/test/test_remotes_file_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/test/test_repositories_file_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-23 16:17:54.000000 pulp_file-client-3.52.0/test/test_repositories_file_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_set_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_set_label_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_task_group_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_unset_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-23 16:17:53.000000 pulp_file-client-3.52.0/test/test_unset_label_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:29.840822 pulp_file-client-3.53.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-30 18:17:29.840822 pulp_file-client-3.53.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15201 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:29.824822 pulp_file-client-3.53.0/pulp_file_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulp_file_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulp_file_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulp_file_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulp_file_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulp_file_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:29.824822 pulp_file-client-3.53.0/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:29.824822 pulp_file-client-3.53.0/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:29.828822 pulp_file-client-3.53.0/pulpcore/client/pulp_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:29.828822 pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76061 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/acs_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25762 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/content_files_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85036 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/distributions_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56163 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/publications_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86136 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/remotes_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99509 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/repositories_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33822 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/repositories_file_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26280 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13962 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:29.836822 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_alternate_content_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_alternate_content_source_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_publication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9429 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27059 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_remote_response_hidden_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9907 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/my_permissions_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/nested_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/nested_role_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/object_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginatedfile_file_alternate_content_source_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginatedfile_file_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginatedfile_file_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginatedfile_file_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginatedfile_file_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginatedfile_file_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/patchedfile_file_alternate_content_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/patchedfile_file_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27368 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/patchedfile_file_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/patchedfile_file_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/set_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/set_label_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/task_group_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/unset_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/unset_label_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/pulpcore/client/pulp_file/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 18:17:29.840822 pulp_file-client-3.53.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:29.840822 pulp_file-client-3.53.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/test/test_acs_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/test/test_content_files_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/test/test_distributions_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_file_file_alternate_content_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_file_file_alternate_content_source_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_file_file_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_file_file_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_file_file_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_file_file_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_file_file_publication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_file_file_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_file_file_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_file_file_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_file_file_remote_response_hidden_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_file_file_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_file_file_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_my_permissions_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_nested_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_nested_role_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_object_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_paginatedfile_file_alternate_content_source_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_paginatedfile_file_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_paginatedfile_file_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_paginatedfile_file_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_paginatedfile_file_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_paginatedfile_file_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_patchedfile_file_alternate_content_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_patchedfile_file_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_patchedfile_file_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_patchedfile_file_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/test/test_publications_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/test/test_remotes_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/test/test_repositories_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-30 18:17:29.000000 pulp_file-client-3.53.0/test/test_repositories_file_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_set_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_set_label_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_task_group_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_unset_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-30 18:17:28.000000 pulp_file-client-3.53.0/test/test_unset_label_response.py
```

### Comparing `pulp_file-client-3.52.0/README.md` & `pulp_file-client-3.53.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_file-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 3.52.0
+- Package version: 3.53.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulp_file-client-3.52.0/pulp_file_client.egg-info/SOURCES.txt` & `pulp_file-client-3.53.0/pulp_file_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/__init__.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "3.52.0"
+__version__ = "3.53.0"
 
 # import apis into sdk package
 from pulpcore.client.pulp_file.api.acs_file_api import AcsFileApi
 from pulpcore.client.pulp_file.api.content_files_api import ContentFilesApi
 from pulpcore.client.pulp_file.api.distributions_file_api import DistributionsFileApi
 from pulpcore.client.pulp_file.api.publications_file_api import PublicationsFileApi
 from pulpcore.client.pulp_file.api.remotes_file_api import RemotesFileApi
```

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/__init__.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/acs_file_api.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/acs_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/content_files_api.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/content_files_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/distributions_file_api.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/distributions_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/publications_file_api.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/publications_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/remotes_file_api.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/remotes_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/repositories_file_api.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/repositories_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/api/repositories_file_versions_api.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/api/repositories_file_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/api_client.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/3.52.0/python'
+        self.user_agent = 'OpenAPI-Generator/3.53.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/configuration.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 3.52.0".\
+               "SDK Package Version: 3.53.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/exceptions.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/__init__.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/async_operation_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/content_summary_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_alternate_content_source.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_alternate_content_source.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_alternate_content_source_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_alternate_content_source_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_content.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_content.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_content_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_content_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_distribution.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_distribution_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_publication.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_publication_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_remote.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_remote_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_remote_response_hidden_fields.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_remote_response_hidden_fields.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_repository.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/file_file_repository_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/file_file_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/my_permissions_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/my_permissions_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/nested_role.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/nested_role.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/nested_role_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/nested_role_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/object_roles_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/object_roles_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginated_repository_version_response_list.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginatedfile_file_alternate_content_source_response_list.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginatedfile_file_alternate_content_source_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginatedfile_file_content_response_list.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginatedfile_file_content_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginatedfile_file_distribution_response_list.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginatedfile_file_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginatedfile_file_publication_response_list.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginatedfile_file_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginatedfile_file_remote_response_list.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginatedfile_file_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/paginatedfile_file_repository_response_list.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/paginatedfile_file_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/patchedfile_file_alternate_content_source.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/patchedfile_file_alternate_content_source.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/patchedfile_file_distribution.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/patchedfile_file_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/patchedfile_file_remote.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/patchedfile_file_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/patchedfile_file_repository.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/patchedfile_file_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/policy_enum.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/repair.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/repair.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/repository_add_remove_content.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/repository_sync_url.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/repository_version_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/set_label.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/set_label.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/set_label_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/set_label_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/task_group_operation_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/task_group_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/unset_label.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/unset_label.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/models/unset_label_response.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/models/unset_label_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/pulpcore/client/pulp_file/rest.py` & `pulp_file-client-3.53.0/pulpcore/client/pulp_file/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/setup.py` & `pulp_file-client-3.53.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_file-client"
-VERSION = "3.52.0"
+VERSION = "3.53.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_file-client-3.52.0/test/test_acs_file_api.py` & `pulp_file-client-3.53.0/test/test_acs_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_async_operation_response.py` & `pulp_file-client-3.53.0/test/test_async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_content_files_api.py` & `pulp_file-client-3.53.0/test/test_content_files_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_content_summary_response.py` & `pulp_file-client-3.53.0/test/test_content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_distributions_file_api.py` & `pulp_file-client-3.53.0/test/test_distributions_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_file_file_alternate_content_source.py` & `pulp_file-client-3.53.0/test/test_file_file_alternate_content_source.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_file_file_alternate_content_source_response.py` & `pulp_file-client-3.53.0/test/test_file_file_alternate_content_source_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_file_file_content.py` & `pulp_file-client-3.53.0/test/test_file_file_content.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_file_file_content_response.py` & `pulp_file-client-3.53.0/test/test_file_file_content_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_file_file_distribution.py` & `pulp_file-client-3.53.0/test/test_file_file_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_file_file_distribution_response.py` & `pulp_file-client-3.53.0/test/test_file_file_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_file_file_publication.py` & `pulp_file-client-3.53.0/test/test_file_file_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_file_file_publication_response.py` & `pulp_file-client-3.53.0/test/test_file_file_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_file_file_remote.py` & `pulp_file-client-3.53.0/test/test_file_file_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_file_file_remote_response.py` & `pulp_file-client-3.53.0/test/test_file_file_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_file_file_remote_response_hidden_fields.py` & `pulp_file-client-3.53.0/test/test_file_file_remote_response_hidden_fields.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_file_file_repository.py` & `pulp_file-client-3.53.0/test/test_file_file_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_file_file_repository_response.py` & `pulp_file-client-3.53.0/test/test_file_file_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_my_permissions_response.py` & `pulp_file-client-3.53.0/test/test_my_permissions_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_nested_role.py` & `pulp_file-client-3.53.0/test/test_nested_role.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_nested_role_response.py` & `pulp_file-client-3.53.0/test/test_nested_role_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_object_roles_response.py` & `pulp_file-client-3.53.0/test/test_object_roles_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_paginated_repository_version_response_list.py` & `pulp_file-client-3.53.0/test/test_paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_paginatedfile_file_alternate_content_source_response_list.py` & `pulp_file-client-3.53.0/test/test_paginatedfile_file_alternate_content_source_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_paginatedfile_file_content_response_list.py` & `pulp_file-client-3.53.0/test/test_paginatedfile_file_content_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_paginatedfile_file_distribution_response_list.py` & `pulp_file-client-3.53.0/test/test_paginatedfile_file_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_paginatedfile_file_publication_response_list.py` & `pulp_file-client-3.53.0/test/test_paginatedfile_file_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_paginatedfile_file_remote_response_list.py` & `pulp_file-client-3.53.0/test/test_paginatedfile_file_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_paginatedfile_file_repository_response_list.py` & `pulp_file-client-3.53.0/test/test_paginatedfile_file_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_patchedfile_file_alternate_content_source.py` & `pulp_file-client-3.53.0/test/test_patchedfile_file_alternate_content_source.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_patchedfile_file_distribution.py` & `pulp_file-client-3.53.0/test/test_patchedfile_file_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_patchedfile_file_remote.py` & `pulp_file-client-3.53.0/test/test_patchedfile_file_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_patchedfile_file_repository.py` & `pulp_file-client-3.53.0/test/test_patchedfile_file_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_policy_enum.py` & `pulp_file-client-3.53.0/test/test_policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_publications_file_api.py` & `pulp_file-client-3.53.0/test/test_publications_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_remotes_file_api.py` & `pulp_file-client-3.53.0/test/test_remotes_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_repair.py` & `pulp_file-client-3.53.0/test/test_repair.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_repositories_file_api.py` & `pulp_file-client-3.53.0/test/test_repositories_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_repositories_file_versions_api.py` & `pulp_file-client-3.53.0/test/test_repositories_file_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_repository_add_remove_content.py` & `pulp_file-client-3.53.0/test/test_repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_repository_sync_url.py` & `pulp_file-client-3.53.0/test/test_repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_repository_version_response.py` & `pulp_file-client-3.53.0/test/test_repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_set_label.py` & `pulp_file-client-3.53.0/test/test_set_label.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_set_label_response.py` & `pulp_file-client-3.53.0/test/test_set_label_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_task_group_operation_response.py` & `pulp_file-client-3.53.0/test/test_task_group_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_unset_label.py` & `pulp_file-client-3.53.0/test/test_unset_label.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-3.52.0/test/test_unset_label_response.py` & `pulp_file-client-3.53.0/test/test_unset_label_response.py`

 * *Files identical despite different names*

