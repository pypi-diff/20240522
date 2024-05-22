# Comparing `tmp/boxsdk-3.9.1.tar.gz` & `tmp/boxsdk-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jenkins/workspace/Box_SDKs/Python_Release/box-python-sdk-6/pypi-dist/boxsdk-3.9.1.tar", last modified: Thu Sep 14 11:45:05 2023, max compression
+gzip compressed data, was "/home/jenkins/workspace/Box_SDKs/Python_Release/box-python-sdk-20/pypi-dist/boxsdk-3.9.2.tar", last modified: Wed Oct 18 15:29:36 2023, max compression
```

## Comparing `boxsdk-3.9.1.tar` & `boxsdk-3.9.2.tar`

### file list

```diff
@@ -1,299 +1,440 @@
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/boxsdk/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/boxsdk/auth/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      759 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/auth/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      637 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/auth/ccg_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1039 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/auth/cooperatively_managed_oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1097 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/auth/developer_token_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    12195 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/auth/jwt_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    18876 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/auth/oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      534 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/auth/redis_managed_jwt_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2021 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/auth/redis_managed_oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1135 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/auth/remote_managed_oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8589 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/auth/server_auth.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/boxsdk/client/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      176 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/client/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    66874 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/client/client.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      468 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/client/developer_token_client.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      297 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/client/development_client.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      315 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/client/logging_client.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/boxsdk/network/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/network/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    10506 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/network/default_network.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3515 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/network/network_interface.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/boxsdk/object/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      904 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      578 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/api_json_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5956 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/base_api_json_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1480 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/base_endpoint.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6607 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/base_item.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5749 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/base_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1563 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/cloneable.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2487 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/collaboration.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4365 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/collaboration_allowlist.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      543 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/collaboration_allowlist_entry.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      228 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/collaboration_allowlist_exempt_target.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1346 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1357 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/comment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      143 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/device_pinner.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      140 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/email_alias.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1096 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/enterprise.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      140 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/event.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    12471 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/events.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    36292 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/file.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2731 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/file_request.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      142 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/file_version.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      171 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/file_version_retention.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    30729 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/folder.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      137 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/folder_lock.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3994 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/group.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      207 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/group_membership.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      123 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/invite.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    17229 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/item.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      316 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/legal_hold.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4327 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/legal_hold_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      186 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/legal_hold_policy_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6999 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/metadata.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1539 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/metadata_cascade_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8933 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/metadata_template.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      189 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/recent_item.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3556 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/retention_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1795 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/retention_policy_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    16861 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/search.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1574 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/sign_request.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      385 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/sign_template.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2330 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/storage_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      178 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/storage_policy_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2694 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/task.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      377 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/task_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3961 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/terms_of_service.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      777 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/terms_of_service_user_status.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5375 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/trash.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6451 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/upload_session.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8104 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/user.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      175 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/watermark.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4489 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/web_link.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2483 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/object/webhook.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/boxsdk/pagination/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/pagination/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7071 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/pagination/box_object_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      186 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/pagination/dict_page.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      331 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/pagination/limit_offset_based_dict_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3961 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/pagination/limit_offset_based_object_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      304 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/pagination/marker_based_dict_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4355 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/pagination/marker_based_object_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1864 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/pagination/page.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/boxsdk/session/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/session/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1050 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/session/box_request.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1357 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/session/box_response.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    23264 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/session/session.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/boxsdk/util/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3012 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/api_call_decorator.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7584 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/chunked_uploader.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      795 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/datetime_formatter.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       29 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/default_arg_value.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1172 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/deprecation_decorator.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4299 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/enum.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      494 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/json.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3744 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/log.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1314 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/lru_cache.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      585 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/multipart_stream.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      561 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/shared_link.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      214 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/text_enum.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7743 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/util/translator.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      319 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      899 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/config.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3581 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/exception.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/boxsdk/py.typed
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       22 2023-09-14 11:43:49.000000 boxsdk-3.9.1/boxsdk/version.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/boxsdk.egg-info/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    18375 2023-09-14 11:45:04.000000 boxsdk-3.9.1/boxsdk.egg-info/PKG-INFO
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     9731 2023-09-14 11:45:04.000000 boxsdk-3.9.1/boxsdk.egg-info/SOURCES.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        1 2023-09-14 11:45:04.000000 boxsdk-3.9.1/boxsdk.egg-info/dependency_links.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      335 2023-09-14 11:45:04.000000 boxsdk-3.9.1/boxsdk.egg-info/requires.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        7 2023-09-14 11:45:04.000000 boxsdk-3.9.1/boxsdk.egg-info/top_level.txt
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/functional/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/functional/mock_box/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/functional/mock_box/behavior/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/behavior/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3889 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/behavior/event_behavior.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5755 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/behavior/file_behavior.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5822 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/behavior/folder_behavior.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      617 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/behavior/item_behavior.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6554 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/behavior/oauth2_behavior.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      945 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/behavior/user_behavior.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/functional/mock_box/db_model/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       87 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/db_model/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      945 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/db_model/application_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      767 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/db_model/collaboration_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1260 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/db_model/event_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1666 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/db_model/file_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1862 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/db_model/folder_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      844 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/db_model/group_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      747 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/db_model/lock_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      804 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/db_model/share_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      738 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/db_model/token_model.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1214 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/db_model/user_model.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/functional/mock_box/util/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/util/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2696 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/util/chaos_utils.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1085 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/util/db_utils.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3609 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/util/http_utils.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2112 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/util/json_utils.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/functional/mock_box/views/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/views/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      202 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/views/html_response.tpl
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      256 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/views/oauth2.tpl
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       69 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/views/xml_response.tpl
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11636 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/mock_box/box.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3896 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1241 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/test_delete.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7449 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/test_events.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4287 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/test_file_upload_update_download.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3687 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/test_item_info.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1933 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/test_object_clone.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      383 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/test_rate_limits.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3522 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/test_recovery.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      767 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/functional/test_token_refresh.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/integration/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1403 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1019 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration/mock_network.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3909 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration/test_as_user.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1117 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration/test_retry_and_refresh.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4602 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration/test_with_shared_link.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/integration_new/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/integration_new/context_managers/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      652 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/context_managers/box_metadata_template.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1274 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/context_managers/box_retention_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      828 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/context_managers/box_retention_policy_assigment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      504 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/context_managers/box_sign_request.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      785 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/context_managers/box_test_file.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      665 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/context_managers/box_test_folder.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      498 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/context_managers/box_test_group.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      545 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/context_managers/box_test_user.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      740 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/context_managers/box_test_web_link.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      521 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/context_managers/local_large_file.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/integration_new/object/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1502 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/object/collaboration_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11058 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/object/file_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8169 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/object/folder_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1445 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/object/legal_hold_policy_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1584 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/object/metadata_template_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2288 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/object/retention_policy_assignement_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1573 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/object/retention_policy_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2346 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/object/sign_request_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      254 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/object/sign_template_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2537 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/object/trash_itest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      192 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/object/user_itest.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/integration_new/resources/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1359 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/resources/image.png
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5558 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/resources/small.pdf
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6235 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/resources/small_v2.pdf
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1703 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/README.md
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2092 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1429 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       37 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/integration_tests.cfg
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      921 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/integration_new/util.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/unit/
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/unit/auth/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/auth/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    12588 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/auth/test_ccg_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      564 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/auth/test_cooperatively_managed_oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1072 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/auth/test_developer_token_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    26294 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/auth/test_jwt_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    17298 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/auth/test_oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2377 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/auth/test_redis_managed_oauth2.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      575 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/auth/test_remote_managed_oauth2.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/unit/client/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/client/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    67134 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/client/test_client.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/unit/network/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/network/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1602 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/network/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11382 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/network/test_network.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/unit/object/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    12211 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      477 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_api_json_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2307 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_base_api_json_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6378 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_base_item.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5111 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_base_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    13966 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_chunked_upload.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4274 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_collaboration.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3564 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_collaboration_allowlist.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1143 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_collaboration_allowlist_entry.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1238 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_collaboration_allowlist_exempt_target.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1360 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2262 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_comment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1577 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_device_pin.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1248 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_enterprise.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      430 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_event.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11176 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_events.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    36673 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_file.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3650 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_file_request.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      650 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_file_version_retention.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    27532 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_folder.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     9451 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_group.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    19897 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_item.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      895 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_legal_hold.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2091 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_legal_hold_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5705 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_legal_hold_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4628 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_metadata.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2489 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_metadata_cascade_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5421 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_metadata_template.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4579 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_retention_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3503 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_retention_policy_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    14811 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_search.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5268 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_sign_request.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4122 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_sign_templates.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7028 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_storage_policy.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2332 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_storage_policy_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5585 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_task.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3128 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_task_assignment.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7926 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_terms_of_service.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2885 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_terms_of_service_user_status.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6814 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_trash.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8088 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_upload_session.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     9668 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_user.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4958 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_web_link.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4142 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/object/test_webhook.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/unit/pagination/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/pagination/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4324 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/pagination/box_object_collection_test_base.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5427 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/pagination/test_limit_offset_based_object_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4575 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/pagination/test_marker_based_object_collection.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2966 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/pagination/test_page.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/unit/session/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/session/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    18255 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/session/test_session.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/unit/util/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/util/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3478 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/util/test_api_call_decorator.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2309 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/util/test_datetime_formatter.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4928 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/util/test_enum.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3856 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/util/test_log.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1102 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/util/test_lru_cache.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1098 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/util/test_multipart_stream.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      639 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/util/test_shared_link.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      324 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/util/test_text_enum.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7419 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/util/test_translator.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5085 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1963 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/unit/test_exception.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:45:05.000000 boxsdk-3.9.1/test/util/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/util/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      644 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/util/streamable_mock_open.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8430 2023-09-14 11:40:55.000000 boxsdk-3.9.1/test/conftest.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     9574 2023-09-14 11:40:55.000000 boxsdk-3.9.1/LICENSE
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       52 2023-09-14 11:40:55.000000 boxsdk-3.9.1/MANIFEST.in
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    16885 2023-09-14 11:40:55.000000 boxsdk-3.9.1/README.md
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      136 2023-09-14 11:45:05.000000 boxsdk-3.9.1/setup.cfg
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3827 2023-09-14 11:40:55.000000 boxsdk-3.9.1/setup.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    18375 2023-09-14 11:45:05.000000 boxsdk-3.9.1/PKG-INFO
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk/auth/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      759 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/auth/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      637 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/auth/ccg_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1039 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/auth/cooperatively_managed_oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1097 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/auth/developer_token_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12195 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/auth/jwt_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    18876 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/auth/oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      534 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/auth/redis_managed_jwt_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2021 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/auth/redis_managed_oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1135 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/auth/remote_managed_oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8589 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/auth/server_auth.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk/client/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      176 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/client/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    66874 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/client/client.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      468 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/client/developer_token_client.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      297 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/client/development_client.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      315 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/client/logging_client.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk/network/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/network/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10506 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/network/default_network.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3515 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/network/network_interface.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk/object/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      904 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      578 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/api_json_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5956 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/base_api_json_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1480 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/base_endpoint.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6607 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/base_item.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5749 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/base_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1563 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/cloneable.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2487 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/collaboration.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4365 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/collaboration_allowlist.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      543 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/collaboration_allowlist_entry.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      228 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/collaboration_allowlist_exempt_target.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1346 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1357 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/comment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      143 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/device_pinner.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      140 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/email_alias.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1096 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/enterprise.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      140 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/event.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12471 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/events.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    36292 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/file.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2731 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/file_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      142 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/file_version.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      171 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/file_version_retention.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    30729 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/folder.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      137 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/folder_lock.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3994 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/group.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      207 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/group_membership.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      123 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/invite.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    17229 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/item.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      316 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/legal_hold.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4327 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/legal_hold_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      186 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/legal_hold_policy_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6999 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/metadata.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1539 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/metadata_cascade_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8933 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/metadata_template.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      189 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/recent_item.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3556 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/retention_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1795 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/retention_policy_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    16861 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/search.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1574 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/sign_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      385 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/sign_template.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2330 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/storage_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      178 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/storage_policy_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2694 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/task.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      377 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/task_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3961 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/terms_of_service.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      777 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/terms_of_service_user_status.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5375 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/trash.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6451 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/upload_session.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8104 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/user.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      175 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/watermark.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4489 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/web_link.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2483 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/object/webhook.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk/pagination/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/pagination/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7071 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/pagination/box_object_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      186 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/pagination/dict_page.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      331 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/pagination/limit_offset_based_dict_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3961 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/pagination/limit_offset_based_object_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      304 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/pagination/marker_based_dict_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4355 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/pagination/marker_based_object_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1864 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/pagination/page.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk/session/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/session/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1050 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/session/box_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1357 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/session/box_response.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    23264 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/session/session.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk/util/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3012 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/api_call_decorator.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7584 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/chunked_uploader.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      795 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/datetime_formatter.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       29 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/default_arg_value.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1172 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/deprecation_decorator.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4325 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/enum.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      494 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/json.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3744 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/log.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1314 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/lru_cache.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      585 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/multipart_stream.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      561 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/shared_link.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      214 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/text_enum.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7743 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/util/translator.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      319 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      899 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/config.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3581 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/exception.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/boxsdk/py.typed
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       22 2023-10-18 15:26:45.000000 boxsdk-3.9.2/boxsdk/version.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk.egg-info/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    18375 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk.egg-info/PKG-INFO
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    19146 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        1 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      343 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk.egg-info/requires.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        7 2023-10-18 15:29:36.000000 boxsdk-3.9.2/boxsdk.egg-info/top_level.txt
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      169 2023-10-18 15:27:22.000000 boxsdk-3.9.2/test/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8858 2023-10-18 15:27:22.000000 boxsdk-3.9.2/test/__pycache__/conftest.cpython-37-pytest-7.4.2.pyc
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/functional/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/functional/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      180 2023-10-18 15:27:25.000000 boxsdk-3.9.2/test/functional/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3861 2023-10-18 15:27:25.000000 boxsdk-3.9.2/test/functional/__pycache__/conftest.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2985 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/__pycache__/test_delete.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11948 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/__pycache__/test_events.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8027 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/__pycache__/test_file_upload_update_download.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8193 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/__pycache__/test_item_info.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3954 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/__pycache__/test_object_clone.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1228 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/__pycache__/test_rate_limits.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6644 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/__pycache__/test_recovery.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1452 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/__pycache__/test_token_refresh.cpython-37-pytest-7.4.2.pyc
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/functional/mock_box/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/functional/mock_box/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      189 2023-10-18 15:27:25.000000 boxsdk-3.9.2/test/functional/mock_box/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11140 2023-10-18 15:27:25.000000 boxsdk-3.9.2/test/functional/mock_box/__pycache__/box.cpython-37-pytest-7.4.2.pyc
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      198 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4368 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/__pycache__/event_behavior.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4835 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/__pycache__/file_behavior.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4832 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/__pycache__/folder_behavior.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1184 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/__pycache__/item_behavior.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5675 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/__pycache__/oauth2_behavior.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1450 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/__pycache__/user_behavior.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3889 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/event_behavior.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5755 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/file_behavior.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5822 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/folder_behavior.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      617 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/item_behavior.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6554 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/oauth2_behavior.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      945 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/behavior/user_behavior.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      395 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1223 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/__pycache__/application_model.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1141 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/__pycache__/collaboration_model.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1502 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/__pycache__/event_model.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1797 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/__pycache__/file_model.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1905 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/__pycache__/folder_model.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1239 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/__pycache__/group_model.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1106 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/__pycache__/lock_model.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1451 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/__pycache__/share_model.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1132 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/__pycache__/token_model.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1408 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/__pycache__/user_model.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       87 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      945 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/application_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      767 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/collaboration_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1260 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/event_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1666 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/file_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1862 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/folder_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      844 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/group_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      747 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/lock_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      804 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/share_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      738 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/token_model.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1214 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/db_model/user_model.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/functional/mock_box/util/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/functional/mock_box/util/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      194 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/util/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3742 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/util/__pycache__/chaos_utils.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1612 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/util/__pycache__/db_utils.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4866 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/util/__pycache__/http_utils.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2490 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/util/__pycache__/json_utils.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/util/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2696 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/util/chaos_utils.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1085 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/util/db_utils.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3609 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/util/http_utils.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2112 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/util/json_utils.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/functional/mock_box/views/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/functional/mock_box/views/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      195 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/functional/mock_box/views/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/views/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      202 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/views/html_response.tpl
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      256 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/views/oauth2.tpl
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       69 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/views/xml_response.tpl
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11636 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/mock_box/box.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3896 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1241 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/test_delete.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7449 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/test_events.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4287 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/test_file_upload_update_download.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3687 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/test_item_info.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1933 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/test_object_clone.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      383 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/test_rate_limits.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3522 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/test_recovery.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      767 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/functional/test_token_refresh.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/integration/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/integration/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      181 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/integration/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1679 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/integration/__pycache__/conftest.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1665 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/integration/__pycache__/mock_network.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5005 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/integration/__pycache__/test_as_user.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1574 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/integration/__pycache__/test_retry_and_refresh.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5418 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/integration/__pycache__/test_with_shared_link.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1403 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1019 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration/mock_network.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3909 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration/test_as_user.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1117 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration/test_retry_and_refresh.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4602 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration/test_with_shared_link.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/integration_new/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/integration_new/context_managers/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      652 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/context_managers/box_metadata_template.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1274 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/context_managers/box_retention_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      828 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/context_managers/box_retention_policy_assigment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      504 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/context_managers/box_sign_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      785 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/context_managers/box_test_file.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      665 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/context_managers/box_test_folder.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      498 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/context_managers/box_test_group.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      545 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/context_managers/box_test_user.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      740 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/context_managers/box_test_web_link.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      521 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/context_managers/local_large_file.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/integration_new/object/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1502 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/object/collaboration_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11058 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/object/file_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8169 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/object/folder_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1445 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/object/legal_hold_policy_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1584 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/object/metadata_template_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2288 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/object/retention_policy_assignement_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1573 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/object/retention_policy_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2346 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/object/sign_request_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      254 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/object/sign_template_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2537 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/object/trash_itest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      192 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/object/user_itest.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/integration_new/resources/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1359 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/resources/image.png
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5558 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/resources/small.pdf
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6235 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/resources/small_v2.pdf
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1703 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/README.md
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2092 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1429 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       37 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/integration_tests.cfg
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      921 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/integration_new/util.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      174 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4576 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/__pycache__/conftest.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4712 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/__pycache__/test_exception.cpython-37-pytest-7.4.2.pyc
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/auth/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/auth/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      179 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/auth/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11609 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/auth/__pycache__/test_ccg_auth.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1347 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/auth/__pycache__/test_cooperatively_managed_oauth2.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3369 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/auth/__pycache__/test_developer_token_auth.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    25055 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/auth/__pycache__/test_jwt_auth.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    18571 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/auth/__pycache__/test_oauth2.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3212 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/auth/__pycache__/test_redis_managed_oauth2.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1317 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/auth/__pycache__/test_remote_managed_oauth2.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/auth/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12588 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/auth/test_ccg_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      564 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/auth/test_cooperatively_managed_oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1072 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/auth/test_developer_token_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    26294 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/auth/test_jwt_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    17298 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/auth/test_oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2377 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/auth/test_redis_managed_oauth2.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      575 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/auth/test_remote_managed_oauth2.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/client/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/client/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      181 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/client/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    90425 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/client/__pycache__/test_client.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/client/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    67134 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/client/test_client.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/network/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/network/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      182 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/network/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2400 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/network/__pycache__/conftest.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    15998 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/network/__pycache__/test_network.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/network/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1602 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/network/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11382 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/network/test_network.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/object/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/object/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      181 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/object/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    13001 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/unit/object/__pycache__/conftest.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1757 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_api_json_object.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7240 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_base_api_json_object.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5083 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_base_item.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7570 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_base_object.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11320 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_chunked_upload.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5860 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_collaboration.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6132 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_collaboration_allowlist.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2026 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_collaboration_allowlist_entry.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2057 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_collaboration_allowlist_exempt_target.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2575 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_collection.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3562 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_comment.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2456 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_device_pin.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2429 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_enterprise.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1041 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_event.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12909 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_events.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    40650 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_file.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5913 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_file_request.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1212 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_file_version_retention.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    31622 2023-10-18 15:27:28.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_folder.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11202 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_group.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    21770 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_item.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2200 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_legal_hold.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3224 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_legal_hold_assignment.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7021 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_legal_hold_policy.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5476 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_metadata.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4283 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_metadata_cascade_policy.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7106 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_metadata_template.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7227 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_retention_policy.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4860 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_retention_policy_assignment.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    14032 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_search.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4587 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_sign_request.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3664 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_sign_templates.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8613 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_storage_policy.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2845 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_storage_policy_assignment.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10054 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_task.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5251 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_task_assignment.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11979 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_terms_of_service.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5516 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_terms_of_service_user_status.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10766 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_trash.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10418 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_upload_session.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    13241 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_user.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6090 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_web_link.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6843 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/object/__pycache__/test_webhook.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12211 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      477 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_api_json_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2307 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_base_api_json_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6378 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_base_item.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5111 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_base_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    13966 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_chunked_upload.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4274 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_collaboration.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3564 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_collaboration_allowlist.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1143 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_collaboration_allowlist_entry.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1238 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_collaboration_allowlist_exempt_target.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1360 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2262 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_comment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1577 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_device_pin.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1248 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_enterprise.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      430 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_event.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11176 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_events.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    36673 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_file.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3650 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_file_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      650 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_file_version_retention.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    27532 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_folder.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9451 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_group.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    19897 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_item.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      895 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_legal_hold.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2091 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_legal_hold_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5705 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_legal_hold_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4628 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_metadata.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2489 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_metadata_cascade_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5421 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_metadata_template.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4579 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_retention_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3503 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_retention_policy_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    14811 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_search.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5268 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_sign_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4122 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_sign_templates.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7028 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_storage_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2332 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_storage_policy_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5585 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_task.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3128 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_task_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7926 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_terms_of_service.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2885 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_terms_of_service_user_status.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6814 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_trash.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8088 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_upload_session.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9668 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_user.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4958 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_web_link.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4142 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/object/test_webhook.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/pagination/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/pagination/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      185 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/pagination/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5252 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/pagination/__pycache__/box_object_collection_test_base.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7497 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/pagination/__pycache__/test_limit_offset_based_object_collection.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4884 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/pagination/__pycache__/test_marker_based_object_collection.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5777 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/pagination/__pycache__/test_page.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/pagination/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4324 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/pagination/box_object_collection_test_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5427 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/pagination/test_limit_offset_based_object_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4575 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/pagination/test_marker_based_object_collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2966 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/pagination/test_page.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/session/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/session/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      182 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/session/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    30406 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/session/__pycache__/test_session.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/session/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    18255 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/session/test_session.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/util/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/unit/util/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      179 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/util/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9152 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/util/__pycache__/test_api_call_decorator.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3569 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/util/__pycache__/test_datetime_formatter.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11923 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/util/__pycache__/test_enum.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5599 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/util/__pycache__/test_log.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2773 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/util/__pycache__/test_lru_cache.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2589 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/util/__pycache__/test_multipart_stream.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1618 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/util/__pycache__/test_shared_link.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2090 2023-10-18 15:27:29.000000 boxsdk-3.9.2/test/unit/util/__pycache__/test_text_enum.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    14081 2023-10-18 15:27:30.000000 boxsdk-3.9.2/test/unit/util/__pycache__/test_translator.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/util/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3478 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/util/test_api_call_decorator.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2309 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/util/test_datetime_formatter.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4927 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/util/test_enum.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3856 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/util/test_log.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1102 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/util/test_lru_cache.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1098 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/util/test_multipart_stream.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      639 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/util/test_shared_link.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      324 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/util/test_text_enum.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7419 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/util/test_translator.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5085 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1963 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/unit/test_exception.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/util/
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:29:36.000000 boxsdk-3.9.2/test/util/__pycache__/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      174 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/util/__pycache__/__init__.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1007 2023-10-18 15:27:27.000000 boxsdk-3.9.2/test/util/__pycache__/streamable_mock_open.cpython-37-pytest-7.4.2.pyc
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/util/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      644 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/util/streamable_mock_open.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8430 2023-10-18 15:15:44.000000 boxsdk-3.9.2/test/conftest.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9574 2023-10-18 15:15:44.000000 boxsdk-3.9.2/LICENSE
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       52 2023-10-18 15:15:44.000000 boxsdk-3.9.2/MANIFEST.in
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    16885 2023-10-18 15:15:44.000000 boxsdk-3.9.2/README.md
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      136 2023-10-18 15:29:36.000000 boxsdk-3.9.2/setup.cfg
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3845 2023-10-18 15:15:44.000000 boxsdk-3.9.2/setup.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    18375 2023-10-18 15:29:36.000000 boxsdk-3.9.2/PKG-INFO
```

### Comparing `boxsdk-3.9.1/boxsdk/auth/__init__.py` & `boxsdk-3.9.2/boxsdk/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/auth/ccg_auth.py` & `boxsdk-3.9.2/boxsdk/auth/ccg_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/auth/cooperatively_managed_oauth2.py` & `boxsdk-3.9.2/boxsdk/auth/cooperatively_managed_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/auth/developer_token_auth.py` & `boxsdk-3.9.2/boxsdk/auth/developer_token_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/auth/jwt_auth.py` & `boxsdk-3.9.2/boxsdk/auth/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/auth/oauth2.py` & `boxsdk-3.9.2/boxsdk/auth/oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/auth/redis_managed_jwt_auth.py` & `boxsdk-3.9.2/boxsdk/auth/redis_managed_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/auth/redis_managed_oauth2.py` & `boxsdk-3.9.2/boxsdk/auth/redis_managed_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/auth/remote_managed_oauth2.py` & `boxsdk-3.9.2/boxsdk/auth/remote_managed_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/auth/server_auth.py` & `boxsdk-3.9.2/boxsdk/auth/server_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/client/client.py` & `boxsdk-3.9.2/boxsdk/client/client.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/network/default_network.py` & `boxsdk-3.9.2/boxsdk/network/default_network.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/network/network_interface.py` & `boxsdk-3.9.2/boxsdk/network/network_interface.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/__init__.py` & `boxsdk-3.9.2/boxsdk/object/__init__.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/api_json_object.py` & `boxsdk-3.9.2/boxsdk/object/api_json_object.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/base_api_json_object.py` & `boxsdk-3.9.2/boxsdk/object/base_api_json_object.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/base_endpoint.py` & `boxsdk-3.9.2/boxsdk/object/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/base_item.py` & `boxsdk-3.9.2/boxsdk/object/base_item.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/base_object.py` & `boxsdk-3.9.2/boxsdk/object/base_object.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/cloneable.py` & `boxsdk-3.9.2/boxsdk/object/cloneable.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/collaboration.py` & `boxsdk-3.9.2/boxsdk/object/collaboration.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/collaboration_allowlist.py` & `boxsdk-3.9.2/boxsdk/object/collaboration_allowlist.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/collaboration_allowlist_entry.py` & `boxsdk-3.9.2/boxsdk/object/collaboration_allowlist_entry.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/collection.py` & `boxsdk-3.9.2/boxsdk/object/collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/comment.py` & `boxsdk-3.9.2/boxsdk/object/comment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/enterprise.py` & `boxsdk-3.9.2/boxsdk/object/enterprise.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/events.py` & `boxsdk-3.9.2/boxsdk/object/events.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/file.py` & `boxsdk-3.9.2/boxsdk/object/file.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/file_request.py` & `boxsdk-3.9.2/boxsdk/object/file_request.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/folder.py` & `boxsdk-3.9.2/boxsdk/object/folder.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/group.py` & `boxsdk-3.9.2/boxsdk/object/group.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/item.py` & `boxsdk-3.9.2/boxsdk/object/item.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/legal_hold_policy.py` & `boxsdk-3.9.2/boxsdk/object/legal_hold_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/metadata.py` & `boxsdk-3.9.2/boxsdk/object/metadata.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/metadata_cascade_policy.py` & `boxsdk-3.9.2/boxsdk/object/metadata_cascade_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/metadata_template.py` & `boxsdk-3.9.2/boxsdk/object/metadata_template.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/retention_policy.py` & `boxsdk-3.9.2/boxsdk/object/retention_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/retention_policy_assignment.py` & `boxsdk-3.9.2/boxsdk/object/retention_policy_assignment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/search.py` & `boxsdk-3.9.2/boxsdk/object/search.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/sign_request.py` & `boxsdk-3.9.2/boxsdk/object/sign_request.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/storage_policy.py` & `boxsdk-3.9.2/boxsdk/object/storage_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/task.py` & `boxsdk-3.9.2/boxsdk/object/task.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/terms_of_service.py` & `boxsdk-3.9.2/boxsdk/object/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/terms_of_service_user_status.py` & `boxsdk-3.9.2/boxsdk/object/terms_of_service_user_status.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/trash.py` & `boxsdk-3.9.2/boxsdk/object/trash.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/upload_session.py` & `boxsdk-3.9.2/boxsdk/object/upload_session.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/user.py` & `boxsdk-3.9.2/boxsdk/object/user.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/web_link.py` & `boxsdk-3.9.2/boxsdk/object/web_link.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/object/webhook.py` & `boxsdk-3.9.2/boxsdk/object/webhook.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/pagination/box_object_collection.py` & `boxsdk-3.9.2/boxsdk/pagination/box_object_collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/pagination/limit_offset_based_object_collection.py` & `boxsdk-3.9.2/boxsdk/pagination/limit_offset_based_object_collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/pagination/marker_based_object_collection.py` & `boxsdk-3.9.2/boxsdk/pagination/marker_based_object_collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/pagination/page.py` & `boxsdk-3.9.2/boxsdk/pagination/page.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/session/box_request.py` & `boxsdk-3.9.2/boxsdk/session/box_request.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/session/box_response.py` & `boxsdk-3.9.2/boxsdk/session/box_response.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/session/session.py` & `boxsdk-3.9.2/boxsdk/session/session.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/util/api_call_decorator.py` & `boxsdk-3.9.2/boxsdk/util/api_call_decorator.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/util/chunked_uploader.py` & `boxsdk-3.9.2/boxsdk/util/chunked_uploader.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/util/datetime_formatter.py` & `boxsdk-3.9.2/boxsdk/util/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/util/deprecation_decorator.py` & `boxsdk-3.9.2/boxsdk/util/deprecation_decorator.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/util/enum.py` & `boxsdk-3.9.2/boxsdk/util/enum.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,19 +61,19 @@
         :param value:
             The value to look up. Can be a value, or an enum instance.
         :raises:
             :class:`ValueError` if the value isn't found anywhere.
         """
         try:
             return cls(value)
-        except ValueError as value_error:
+        except (ValueError, TypeError) as value_error:
             for subclass in cls.__subclasses__():
                 try:
                     return subclass.lookup(value)
-                except ValueError:
+                except (ValueError, TypeError):
                     pass
             raise value_error
 
     @property
     def __members__(cls):
         members = OrderedDict(super().__members__)
         for subclass in cls.__subclasses__():
```

### Comparing `boxsdk-3.9.1/boxsdk/util/log.py` & `boxsdk-3.9.2/boxsdk/util/log.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/util/lru_cache.py` & `boxsdk-3.9.2/boxsdk/util/lru_cache.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/util/multipart_stream.py` & `boxsdk-3.9.2/boxsdk/util/multipart_stream.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/util/shared_link.py` & `boxsdk-3.9.2/boxsdk/util/shared_link.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/util/translator.py` & `boxsdk-3.9.2/boxsdk/util/translator.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/config.py` & `boxsdk-3.9.2/boxsdk/config.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk/exception.py` & `boxsdk-3.9.2/boxsdk/exception.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/boxsdk.egg-info/PKG-INFO` & `boxsdk-3.9.2/boxsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxsdk
-Version: 3.9.1
+Version: 3.9.2
 Summary: Official Box Python SDK
 Home-page: https://github.com/box/box-python-sdk
 Author: Box
 Author-email: oss@box.com
 License: Apache Software License, Version 2.0, http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Changelog, https://github.com/box/box-python-sdk/blob/main/CHANGELOG.md
 Keywords: box oauth2 sdk
```

### Comparing `boxsdk-3.9.1/test/functional/mock_box/behavior/event_behavior.py` & `boxsdk-3.9.2/test/functional/mock_box/behavior/event_behavior.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/behavior/file_behavior.py` & `boxsdk-3.9.2/test/functional/mock_box/behavior/file_behavior.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/behavior/folder_behavior.py` & `boxsdk-3.9.2/test/functional/mock_box/behavior/folder_behavior.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/behavior/item_behavior.py` & `boxsdk-3.9.2/test/functional/mock_box/behavior/item_behavior.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/behavior/oauth2_behavior.py` & `boxsdk-3.9.2/test/functional/mock_box/behavior/oauth2_behavior.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/behavior/user_behavior.py` & `boxsdk-3.9.2/test/functional/mock_box/behavior/user_behavior.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/db_model/application_model.py` & `boxsdk-3.9.2/test/functional/mock_box/db_model/application_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/db_model/collaboration_model.py` & `boxsdk-3.9.2/test/functional/mock_box/db_model/collaboration_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/db_model/event_model.py` & `boxsdk-3.9.2/test/functional/mock_box/db_model/event_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/db_model/file_model.py` & `boxsdk-3.9.2/test/functional/mock_box/db_model/file_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/db_model/folder_model.py` & `boxsdk-3.9.2/test/functional/mock_box/db_model/folder_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/db_model/group_model.py` & `boxsdk-3.9.2/test/functional/mock_box/db_model/group_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/db_model/lock_model.py` & `boxsdk-3.9.2/test/functional/mock_box/db_model/lock_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/db_model/share_model.py` & `boxsdk-3.9.2/test/functional/mock_box/db_model/share_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/db_model/token_model.py` & `boxsdk-3.9.2/test/functional/mock_box/db_model/token_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/db_model/user_model.py` & `boxsdk-3.9.2/test/functional/mock_box/db_model/user_model.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/util/chaos_utils.py` & `boxsdk-3.9.2/test/functional/mock_box/util/chaos_utils.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/util/db_utils.py` & `boxsdk-3.9.2/test/functional/mock_box/util/db_utils.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/util/http_utils.py` & `boxsdk-3.9.2/test/functional/mock_box/util/http_utils.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/util/json_utils.py` & `boxsdk-3.9.2/test/functional/mock_box/util/json_utils.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/mock_box/box.py` & `boxsdk-3.9.2/test/functional/mock_box/box.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/conftest.py` & `boxsdk-3.9.2/test/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/test_delete.py` & `boxsdk-3.9.2/test/functional/test_delete.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/test_events.py` & `boxsdk-3.9.2/test/functional/test_events.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/test_file_upload_update_download.py` & `boxsdk-3.9.2/test/functional/test_file_upload_update_download.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/test_item_info.py` & `boxsdk-3.9.2/test/functional/test_item_info.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/test_object_clone.py` & `boxsdk-3.9.2/test/functional/test_object_clone.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/test_recovery.py` & `boxsdk-3.9.2/test/functional/test_recovery.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/functional/test_token_refresh.py` & `boxsdk-3.9.2/test/functional/test_token_refresh.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration/conftest.py` & `boxsdk-3.9.2/test/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration/mock_network.py` & `boxsdk-3.9.2/test/integration/mock_network.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration/test_as_user.py` & `boxsdk-3.9.2/test/integration/test_as_user.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration/test_retry_and_refresh.py` & `boxsdk-3.9.2/test/integration/test_retry_and_refresh.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration/test_with_shared_link.py` & `boxsdk-3.9.2/test/integration/test_with_shared_link.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/context_managers/box_metadata_template.py` & `boxsdk-3.9.2/test/integration_new/context_managers/box_metadata_template.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/context_managers/box_retention_policy.py` & `boxsdk-3.9.2/test/integration_new/context_managers/box_retention_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/context_managers/box_retention_policy_assigment.py` & `boxsdk-3.9.2/test/integration_new/context_managers/box_retention_policy_assigment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/context_managers/box_test_file.py` & `boxsdk-3.9.2/test/integration_new/context_managers/box_test_file.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/context_managers/box_test_folder.py` & `boxsdk-3.9.2/test/integration_new/context_managers/box_test_folder.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/context_managers/box_test_user.py` & `boxsdk-3.9.2/test/integration_new/context_managers/box_test_user.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/context_managers/box_test_web_link.py` & `boxsdk-3.9.2/test/integration_new/context_managers/box_test_web_link.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/context_managers/local_large_file.py` & `boxsdk-3.9.2/test/integration_new/context_managers/local_large_file.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/object/collaboration_itest.py` & `boxsdk-3.9.2/test/integration_new/object/collaboration_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/object/file_itest.py` & `boxsdk-3.9.2/test/integration_new/object/file_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/object/folder_itest.py` & `boxsdk-3.9.2/test/integration_new/object/folder_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/object/legal_hold_policy_itest.py` & `boxsdk-3.9.2/test/integration_new/object/legal_hold_policy_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/object/metadata_template_itest.py` & `boxsdk-3.9.2/test/integration_new/object/metadata_template_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/object/retention_policy_assignement_itest.py` & `boxsdk-3.9.2/test/integration_new/object/retention_policy_assignement_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/object/retention_policy_itest.py` & `boxsdk-3.9.2/test/integration_new/object/retention_policy_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/object/sign_request_itest.py` & `boxsdk-3.9.2/test/integration_new/object/sign_request_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/object/trash_itest.py` & `boxsdk-3.9.2/test/integration_new/object/trash_itest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/resources/image.png` & `boxsdk-3.9.2/test/integration_new/resources/image.png`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/resources/small.pdf` & `boxsdk-3.9.2/test/integration_new/resources/small.pdf`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/resources/small_v2.pdf` & `boxsdk-3.9.2/test/integration_new/resources/small_v2.pdf`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/README.md` & `boxsdk-3.9.2/test/integration_new/README.md`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/__init__.py` & `boxsdk-3.9.2/test/integration_new/__init__.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/conftest.py` & `boxsdk-3.9.2/test/integration_new/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/integration_new/util.py` & `boxsdk-3.9.2/test/integration_new/util.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/auth/test_ccg_auth.py` & `boxsdk-3.9.2/test/unit/auth/test_ccg_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/auth/test_cooperatively_managed_oauth2.py` & `boxsdk-3.9.2/test/unit/auth/test_cooperatively_managed_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/auth/test_developer_token_auth.py` & `boxsdk-3.9.2/test/unit/auth/test_developer_token_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/auth/test_jwt_auth.py` & `boxsdk-3.9.2/test/unit/auth/test_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/auth/test_oauth2.py` & `boxsdk-3.9.2/test/unit/auth/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/auth/test_redis_managed_oauth2.py` & `boxsdk-3.9.2/test/unit/auth/test_redis_managed_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/auth/test_remote_managed_oauth2.py` & `boxsdk-3.9.2/test/unit/auth/test_remote_managed_oauth2.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/client/test_client.py` & `boxsdk-3.9.2/test/unit/client/test_client.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/network/conftest.py` & `boxsdk-3.9.2/test/unit/network/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/network/test_network.py` & `boxsdk-3.9.2/test/unit/network/test_network.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/conftest.py` & `boxsdk-3.9.2/test/unit/object/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_base_api_json_object.py` & `boxsdk-3.9.2/test/unit/object/test_base_api_json_object.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_base_item.py` & `boxsdk-3.9.2/test/unit/object/test_base_item.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_base_object.py` & `boxsdk-3.9.2/test/unit/object/test_base_object.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_chunked_upload.py` & `boxsdk-3.9.2/test/unit/object/test_chunked_upload.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_collaboration.py` & `boxsdk-3.9.2/test/unit/object/test_collaboration.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_collaboration_allowlist.py` & `boxsdk-3.9.2/test/unit/object/test_collaboration_allowlist.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_collaboration_allowlist_entry.py` & `boxsdk-3.9.2/test/unit/object/test_collaboration_allowlist_entry.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_collaboration_allowlist_exempt_target.py` & `boxsdk-3.9.2/test/unit/object/test_collaboration_allowlist_exempt_target.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_collection.py` & `boxsdk-3.9.2/test/unit/object/test_collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_comment.py` & `boxsdk-3.9.2/test/unit/object/test_comment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_device_pin.py` & `boxsdk-3.9.2/test/unit/object/test_device_pin.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_enterprise.py` & `boxsdk-3.9.2/test/unit/object/test_enterprise.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_events.py` & `boxsdk-3.9.2/test/unit/object/test_events.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_file.py` & `boxsdk-3.9.2/test/unit/object/test_file.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_file_request.py` & `boxsdk-3.9.2/test/unit/object/test_file_request.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_file_version_retention.py` & `boxsdk-3.9.2/test/unit/object/test_file_version_retention.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_folder.py` & `boxsdk-3.9.2/test/unit/object/test_folder.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_group.py` & `boxsdk-3.9.2/test/unit/object/test_group.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_item.py` & `boxsdk-3.9.2/test/unit/object/test_item.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_legal_hold.py` & `boxsdk-3.9.2/test/unit/object/test_legal_hold.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_legal_hold_assignment.py` & `boxsdk-3.9.2/test/unit/object/test_legal_hold_assignment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_legal_hold_policy.py` & `boxsdk-3.9.2/test/unit/object/test_legal_hold_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_metadata.py` & `boxsdk-3.9.2/test/unit/object/test_metadata.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_metadata_cascade_policy.py` & `boxsdk-3.9.2/test/unit/object/test_metadata_cascade_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_metadata_template.py` & `boxsdk-3.9.2/test/unit/object/test_metadata_template.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_retention_policy.py` & `boxsdk-3.9.2/test/unit/object/test_retention_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_retention_policy_assignment.py` & `boxsdk-3.9.2/test/unit/object/test_retention_policy_assignment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_search.py` & `boxsdk-3.9.2/test/unit/object/test_search.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_sign_request.py` & `boxsdk-3.9.2/test/unit/object/test_sign_request.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_sign_templates.py` & `boxsdk-3.9.2/test/unit/object/test_sign_templates.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_storage_policy.py` & `boxsdk-3.9.2/test/unit/object/test_storage_policy.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_storage_policy_assignment.py` & `boxsdk-3.9.2/test/unit/object/test_storage_policy_assignment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_task.py` & `boxsdk-3.9.2/test/unit/object/test_task.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_task_assignment.py` & `boxsdk-3.9.2/test/unit/object/test_task_assignment.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_terms_of_service.py` & `boxsdk-3.9.2/test/unit/object/test_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_terms_of_service_user_status.py` & `boxsdk-3.9.2/test/unit/object/test_terms_of_service_user_status.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_trash.py` & `boxsdk-3.9.2/test/unit/object/test_trash.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_upload_session.py` & `boxsdk-3.9.2/test/unit/object/test_upload_session.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_user.py` & `boxsdk-3.9.2/test/unit/object/test_user.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_web_link.py` & `boxsdk-3.9.2/test/unit/object/test_web_link.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/object/test_webhook.py` & `boxsdk-3.9.2/test/unit/object/test_webhook.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/pagination/box_object_collection_test_base.py` & `boxsdk-3.9.2/test/unit/pagination/box_object_collection_test_base.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/pagination/test_limit_offset_based_object_collection.py` & `boxsdk-3.9.2/test/unit/pagination/test_limit_offset_based_object_collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/pagination/test_marker_based_object_collection.py` & `boxsdk-3.9.2/test/unit/pagination/test_marker_based_object_collection.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/pagination/test_page.py` & `boxsdk-3.9.2/test/unit/pagination/test_page.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/session/test_session.py` & `boxsdk-3.9.2/test/unit/session/test_session.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/util/test_api_call_decorator.py` & `boxsdk-3.9.2/test/unit/util/test_api_call_decorator.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/util/test_datetime_formatter.py` & `boxsdk-3.9.2/test/unit/util/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/util/test_enum.py` & `boxsdk-3.9.2/test/unit/util/test_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     assert EnumBase.lookup(enum_instance) == enum_instance
     assert enum_instance.__class__.lookup(enum_instance) == enum_instance
     assert enum_instance.__class__(enum_instance) == enum_instance
     assert enum_instance.__class__(enum_member_value) == enum_instance
 
 
 def test_lookup_raises_value_error_for_non_members(EnumBaseWithSubclassesDefined):
-    with pytest.raises(ValueError):
+    with pytest.raises(Exception):
         EnumBaseWithSubclassesDefined.lookup('foobar')
 
 
 def test_members(EnumBaseWithSubclassesDefined, enum_members):
     assert dict(EnumBaseWithSubclassesDefined.__members__) == enum_members
```

### Comparing `boxsdk-3.9.1/test/unit/util/test_log.py` & `boxsdk-3.9.2/test/unit/util/test_log.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/util/test_lru_cache.py` & `boxsdk-3.9.2/test/unit/util/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/util/test_multipart_stream.py` & `boxsdk-3.9.2/test/unit/util/test_multipart_stream.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/util/test_shared_link.py` & `boxsdk-3.9.2/test/unit/util/test_shared_link.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/util/test_translator.py` & `boxsdk-3.9.2/test/unit/util/test_translator.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/conftest.py` & `boxsdk-3.9.2/test/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/unit/test_exception.py` & `boxsdk-3.9.2/test/unit/test_exception.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/util/streamable_mock_open.py` & `boxsdk-3.9.2/test/util/streamable_mock_open.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/test/conftest.py` & `boxsdk-3.9.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/LICENSE` & `boxsdk-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/README.md` & `boxsdk-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `boxsdk-3.9.1/setup.py` & `boxsdk-3.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         sys.exit(errno)
 
 
 def main():
     base_dir = dirname(__file__)
     install_requires = [
         'attrs>=17.3.0',
-        'urllib3<2',
+        'urllib3',
         'requests>=2.4.3,<3',
         'requests-toolbelt>=0.4.0',
         'python-dateutil',  # To be removed after dropping Python 3.6
     ]
     redis_requires = ['redis>=2.10.3']
     jwt_requires = ['pyjwt>=1.7.0', 'cryptography>=3']
     coveralls_requires = ['coveralls']
@@ -69,14 +69,15 @@
         'jsonpatch>1.14',
         'sqlalchemy<1.4.0',
         'pytest',
         'pytest-timeout',
         'pytest-cov',
         'pytest-lazy-fixture',
         'pytz',
+        'urllib3<2'
     ]
     extra_requires = {
         'jwt': jwt_requires,
         'redis': redis_requires,
         'coveralls': coveralls_requires + dev_requires,
         'dev': dev_requires,
         'gh': gh_requires + dev_requires,
```

### Comparing `boxsdk-3.9.1/PKG-INFO` & `boxsdk-3.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxsdk
-Version: 3.9.1
+Version: 3.9.2
 Summary: Official Box Python SDK
 Home-page: https://github.com/box/box-python-sdk
 Author: Box
 Author-email: oss@box.com
 License: Apache Software License, Version 2.0, http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Changelog, https://github.com/box/box-python-sdk/blob/main/CHANGELOG.md
 Keywords: box oauth2 sdk
```

