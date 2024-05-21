# Comparing `tmp/structifyai-0.1.0a8.tar.gz` & `tmp/structifyai-0.1.0a9.tar.gz`

## Comparing `structifyai-0.1.0a8.tar` & `structifyai-0.1.0a9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/__init__.py
--rw-r--r--   0        0        0    64417 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_base_client.py
--rw-r--r--   0        0        0    22539 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_constants.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_qs.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_resource.py
--rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_response.py
--rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_streaming.py
--rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_types.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/lib/.keep
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/__init__.py
--rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/datasets.py
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/documents.py
--rw-r--r--   0        0        0    20198 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/label.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/runs.py
--rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/sources.py
--rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/structure.py
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/usage.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/user.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/admin/__init__.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/admin/admin.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/admin/users.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/server/__init__.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/server/server.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/resources/server/version.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_create_params.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_delete_params.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_descriptor.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_list_response.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_retrieve_params.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_view_params.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/dataset_view_response.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/document_download_response.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/document_list_response.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/document_upload_params.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/is_complete.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/kg_entity.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/label_get_messages_response.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/label_run_params.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/label_submit_params.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/label_submit_response.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/new_token.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/run_list_response.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/source.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/source_list_params.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/structure_is_complete_params.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/structure_job_status_params.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/structure_run_async_params.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/usage_get_job_info_params.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/user_info.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/admin/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/admin/user.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/admin/user_list_response.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/server/__init__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/src/structify/types/server/server_information.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/.gitignore
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/LICENSE
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0    12242 2020-02-02 00:00:00.000000 structifyai-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/__init__.py
+-rw-r--r--   0        0        0    64417 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_base_client.py
+-rw-r--r--   0        0        0    22539 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_constants.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_qs.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_resource.py
+-rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_response.py
+-rw-r--r--   0        0        0    10112 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_streaming.py
+-rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_types.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_utils/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/lib/.keep
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/__init__.py
+-rw-r--r--   0        0        0    17731 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/datasets.py
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/documents.py
+-rw-r--r--   0        0        0    20198 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/label.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/runs.py
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/sources.py
+-rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/structure.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/usage.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/user.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/admin/__init__.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/admin/admin.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/admin/users.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/server/__init__.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/server/server.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/resources/server/version.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/dataset.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/dataset_create_params.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/dataset_delete_params.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/dataset_descriptor.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/dataset_get_params.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/dataset_list_response.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/dataset_view_params.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/dataset_view_response.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/document_download_response.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/document_list_response.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/document_upload_params.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/entity.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/is_complete.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/label_get_messages_response.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/label_run_params.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/label_submit_params.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/label_submit_response.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/new_token.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/run_list_response.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/source.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/source_list_params.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/structure_is_complete_params.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/structure_job_status_params.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/structure_run_async_params.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/usage_get_job_info_params.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/user_info.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/admin/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/admin/user.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/admin/user_list_response.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/server/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/src/structify/types/server/server_information.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/.gitignore
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/LICENSE
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/pyproject.toml
+-rw-r--r--   0        0        0    12242 2020-02-02 00:00:00.000000 structifyai-0.1.0a9/PKG-INFO
```

### Comparing `structifyai-0.1.0a8/src/structify/__init__.py` & `structifyai-0.1.0a9/src/structify/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_base_client.py` & `structifyai-0.1.0a9/src/structify/_base_client.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_client.py` & `structifyai-0.1.0a9/src/structify/_client.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_compat.py` & `structifyai-0.1.0a9/src/structify/_compat.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_exceptions.py` & `structifyai-0.1.0a9/src/structify/_exceptions.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_files.py` & `structifyai-0.1.0a9/src/structify/_files.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_models.py` & `structifyai-0.1.0a9/src/structify/_models.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_qs.py` & `structifyai-0.1.0a9/src/structify/_qs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_resource.py` & `structifyai-0.1.0a9/src/structify/_resource.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_response.py` & `structifyai-0.1.0a9/src/structify/_response.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_streaming.py` & `structifyai-0.1.0a9/src/structify/_streaming.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_types.py` & `structifyai-0.1.0a9/src/structify/_types.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_utils/__init__.py` & `structifyai-0.1.0a9/src/structify/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_utils/_logs.py` & `structifyai-0.1.0a9/src/structify/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_utils/_proxy.py` & `structifyai-0.1.0a9/src/structify/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_utils/_sync.py` & `structifyai-0.1.0a9/src/structify/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_utils/_transform.py` & `structifyai-0.1.0a9/src/structify/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_utils/_typing.py` & `structifyai-0.1.0a9/src/structify/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/_utils/_utils.py` & `structifyai-0.1.0a9/src/structify/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/__init__.py` & `structifyai-0.1.0a9/src/structify/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/datasets.py` & `structifyai-0.1.0a9/src/structify/resources/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,15 @@
 
 from __future__ import annotations
 
 from typing import Iterable, Optional
 
 import httpx
 
-from ..types import (
-    dataset_view_params,
-    dataset_create_params,
-    dataset_delete_params,
-    dataset_retrieve_params,
-)
+from ..types import dataset_get_params, dataset_view_params, dataset_create_params, dataset_delete_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NoneType, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
@@ -82,106 +77,106 @@
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=NoneType,
         )
 
-    def retrieve(
+    def list(
+        self,
+        *,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> DatasetListResponse:
+        """Gets all datasets owned by the current user"""
+        return self._get(
+            "/dataset/list",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=DatasetListResponse,
+        )
+
+    def delete(
         self,
         *,
         name: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Optional[DatasetDescriptor]:
+    ) -> None:
         """
-        Grab a dataset by its name.
+        Permanently delete a dataset and all its contents
 
         Args:
-          name: Information about the dataset
+          name: The name of the dataset
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        return self._get(
-            "/dataset/info",
+        extra_headers = {"Accept": "*/*", **(extra_headers or {})}
+        return self._delete(
+            "/dataset/delete",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
-                query=maybe_transform({"name": name}, dataset_retrieve_params.DatasetRetrieveParams),
-            ),
-            cast_to=DatasetDescriptor,
-        )
-
-    def list(
-        self,
-        *,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> DatasetListResponse:
-        """Gets all datasets owned by the current user"""
-        return self._get(
-            "/dataset/list",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+                query=maybe_transform({"name": name}, dataset_delete_params.DatasetDeleteParams),
             ),
-            cast_to=DatasetListResponse,
+            cast_to=NoneType,
         )
 
-    def delete(
+    def get(
         self,
         *,
         name: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> None:
+    ) -> Optional[DatasetDescriptor]:
         """
-        Permanently delete a dataset and all its contents
+        Grab a dataset by its name.
 
         Args:
-          name: The name of the dataset
+          name: Information about the dataset
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        extra_headers = {"Accept": "*/*", **(extra_headers or {})}
-        return self._delete(
-            "/dataset/delete",
+        return self._get(
+            "/dataset/info",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
-                query=maybe_transform({"name": name}, dataset_delete_params.DatasetDeleteParams),
+                query=maybe_transform({"name": name}, dataset_get_params.DatasetGetParams),
             ),
-            cast_to=NoneType,
+            cast_to=DatasetDescriptor,
         )
 
     def view(
         self,
         *,
         dataset_name: str,
         table_name: str,
@@ -274,106 +269,106 @@
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=NoneType,
         )
 
-    async def retrieve(
+    async def list(
+        self,
+        *,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+    ) -> DatasetListResponse:
+        """Gets all datasets owned by the current user"""
+        return await self._get(
+            "/dataset/list",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=DatasetListResponse,
+        )
+
+    async def delete(
         self,
         *,
         name: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Optional[DatasetDescriptor]:
+    ) -> None:
         """
-        Grab a dataset by its name.
+        Permanently delete a dataset and all its contents
 
         Args:
-          name: Information about the dataset
+          name: The name of the dataset
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        return await self._get(
-            "/dataset/info",
+        extra_headers = {"Accept": "*/*", **(extra_headers or {})}
+        return await self._delete(
+            "/dataset/delete",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
-                query=await async_maybe_transform({"name": name}, dataset_retrieve_params.DatasetRetrieveParams),
-            ),
-            cast_to=DatasetDescriptor,
-        )
-
-    async def list(
-        self,
-        *,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> DatasetListResponse:
-        """Gets all datasets owned by the current user"""
-        return await self._get(
-            "/dataset/list",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+                query=await async_maybe_transform({"name": name}, dataset_delete_params.DatasetDeleteParams),
             ),
-            cast_to=DatasetListResponse,
+            cast_to=NoneType,
         )
 
-    async def delete(
+    async def get(
         self,
         *,
         name: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> None:
+    ) -> Optional[DatasetDescriptor]:
         """
-        Permanently delete a dataset and all its contents
+        Grab a dataset by its name.
 
         Args:
-          name: The name of the dataset
+          name: Information about the dataset
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
-        extra_headers = {"Accept": "*/*", **(extra_headers or {})}
-        return await self._delete(
-            "/dataset/delete",
+        return await self._get(
+            "/dataset/info",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
-                query=await async_maybe_transform({"name": name}, dataset_delete_params.DatasetDeleteParams),
+                query=await async_maybe_transform({"name": name}, dataset_get_params.DatasetGetParams),
             ),
-            cast_to=NoneType,
+            cast_to=DatasetDescriptor,
         )
 
     async def view(
         self,
         *,
         dataset_name: str,
         table_name: str,
@@ -422,82 +417,82 @@
 class DatasetsResourceWithRawResponse:
     def __init__(self, datasets: DatasetsResource) -> None:
         self._datasets = datasets
 
         self.create = to_raw_response_wrapper(
             datasets.create,
         )
-        self.retrieve = to_raw_response_wrapper(
-            datasets.retrieve,
-        )
         self.list = to_raw_response_wrapper(
             datasets.list,
         )
         self.delete = to_raw_response_wrapper(
             datasets.delete,
         )
+        self.get = to_raw_response_wrapper(
+            datasets.get,
+        )
         self.view = to_raw_response_wrapper(
             datasets.view,
         )
 
 
 class AsyncDatasetsResourceWithRawResponse:
     def __init__(self, datasets: AsyncDatasetsResource) -> None:
         self._datasets = datasets
 
         self.create = async_to_raw_response_wrapper(
             datasets.create,
         )
-        self.retrieve = async_to_raw_response_wrapper(
-            datasets.retrieve,
-        )
         self.list = async_to_raw_response_wrapper(
             datasets.list,
         )
         self.delete = async_to_raw_response_wrapper(
             datasets.delete,
         )
+        self.get = async_to_raw_response_wrapper(
+            datasets.get,
+        )
         self.view = async_to_raw_response_wrapper(
             datasets.view,
         )
 
 
 class DatasetsResourceWithStreamingResponse:
     def __init__(self, datasets: DatasetsResource) -> None:
         self._datasets = datasets
 
         self.create = to_streamed_response_wrapper(
             datasets.create,
         )
-        self.retrieve = to_streamed_response_wrapper(
-            datasets.retrieve,
-        )
         self.list = to_streamed_response_wrapper(
             datasets.list,
         )
         self.delete = to_streamed_response_wrapper(
             datasets.delete,
         )
+        self.get = to_streamed_response_wrapper(
+            datasets.get,
+        )
         self.view = to_streamed_response_wrapper(
             datasets.view,
         )
 
 
 class AsyncDatasetsResourceWithStreamingResponse:
     def __init__(self, datasets: AsyncDatasetsResource) -> None:
         self._datasets = datasets
 
         self.create = async_to_streamed_response_wrapper(
             datasets.create,
         )
-        self.retrieve = async_to_streamed_response_wrapper(
-            datasets.retrieve,
-        )
         self.list = async_to_streamed_response_wrapper(
             datasets.list,
         )
         self.delete = async_to_streamed_response_wrapper(
             datasets.delete,
         )
+        self.get = async_to_streamed_response_wrapper(
+            datasets.get,
+        )
         self.view = async_to_streamed_response_wrapper(
             datasets.view,
         )
```

### Comparing `structifyai-0.1.0a8/src/structify/resources/documents.py` & `structifyai-0.1.0a9/src/structify/resources/documents.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/label.py` & `structifyai-0.1.0a9/src/structify/resources/label.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/runs.py` & `structifyai-0.1.0a9/src/structify/resources/runs.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/sources.py` & `structifyai-0.1.0a9/src/structify/resources/sources.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/structure.py` & `structifyai-0.1.0a9/src/structify/resources/structure.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/usage.py` & `structifyai-0.1.0a9/src/structify/resources/usage.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/user.py` & `structifyai-0.1.0a9/src/structify/resources/user.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/admin/__init__.py` & `structifyai-0.1.0a9/src/structify/resources/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/admin/admin.py` & `structifyai-0.1.0a9/src/structify/resources/admin/admin.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/admin/users.py` & `structifyai-0.1.0a9/src/structify/resources/admin/users.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/server/__init__.py` & `structifyai-0.1.0a9/src/structify/resources/server/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/server/server.py` & `structifyai-0.1.0a9/src/structify/resources/server/server.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/resources/server/version.py` & `structifyai-0.1.0a9/src/structify/resources/server/version.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/types/__init__.py` & `structifyai-0.1.0a9/src/structify/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
+from .entity import Entity as Entity
 from .source import Source as Source
 from .dataset import Dataset as Dataset
-from .kg_entity import KgEntity as KgEntity
 from .new_token import NewToken as NewToken
 from .user_info import UserInfo as UserInfo
 from .is_complete import IsComplete as IsComplete
 from .label_run_params import LabelRunParams as LabelRunParams
 from .run_list_response import RunListResponse as RunListResponse
 from .dataset_descriptor import DatasetDescriptor as DatasetDescriptor
+from .dataset_get_params import DatasetGetParams as DatasetGetParams
 from .source_list_params import SourceListParams as SourceListParams
 from .dataset_view_params import DatasetViewParams as DatasetViewParams
 from .label_submit_params import LabelSubmitParams as LabelSubmitParams
 from .dataset_create_params import DatasetCreateParams as DatasetCreateParams
 from .dataset_delete_params import DatasetDeleteParams as DatasetDeleteParams
 from .dataset_list_response import DatasetListResponse as DatasetListResponse
 from .dataset_view_response import DatasetViewResponse as DatasetViewResponse
 from .label_submit_response import LabelSubmitResponse as LabelSubmitResponse
 from .document_list_response import DocumentListResponse as DocumentListResponse
 from .document_upload_params import DocumentUploadParams as DocumentUploadParams
-from .dataset_retrieve_params import DatasetRetrieveParams as DatasetRetrieveParams
 from .usage_get_job_info_params import UsageGetJobInfoParams as UsageGetJobInfoParams
 from .document_download_response import DocumentDownloadResponse as DocumentDownloadResponse
 from .structure_run_async_params import StructureRunAsyncParams as StructureRunAsyncParams
 from .label_get_messages_response import LabelGetMessagesResponse as LabelGetMessagesResponse
 from .structure_job_status_params import StructureJobStatusParams as StructureJobStatusParams
 from .structure_is_complete_params import StructureIsCompleteParams as StructureIsCompleteParams
```

### Comparing `structifyai-0.1.0a8/src/structify/types/dataset_create_params.py` & `structifyai-0.1.0a9/src/structify/types/dataset_create_params.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/types/dataset_descriptor.py` & `structifyai-0.1.0a9/src/structify/types/dataset_descriptor.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/types/label_run_params.py` & `structifyai-0.1.0a9/src/structify/types/label_run_params.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/types/source.py` & `structifyai-0.1.0a9/src/structify/types/source.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/src/structify/types/structure_run_async_params.py` & `structifyai-0.1.0a9/src/structify/types/structure_run_async_params.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/LICENSE` & `structifyai-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `structifyai-0.1.0a8/pyproject.toml` & `structifyai-0.1.0a9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "structifyai"
-version = "0.1.0-alpha.8"
+version = "0.1.0-alpha.9"
 description = "The official Python library for the structify API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Structify", email = "team@structify.ai" },
 ]
 dependencies = [
```

### Comparing `structifyai-0.1.0a8/PKG-INFO` & `structifyai-0.1.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: structifyai
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: The official Python library for the structify API
 Project-URL: Homepage, https://github.com/StructifyAI/structify-python
 Project-URL: Repository, https://github.com/StructifyAI/structify-python
 Author-email: Structify <team@structify.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

