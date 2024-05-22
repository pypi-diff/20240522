# Comparing `tmp/Files.com-1.4.81.tar.gz` & `tmp/Files.com-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Files.com-1.4.81.tar", last modified: Wed May 22 17:34:32 2024, max compression
+gzip compressed data, was "Files.com-1.4.9.tar", last modified: Fri Jan 12 16:43:33 2024, max compression
```

## Comparing `Files.com-1.4.81.tar` & `Files.com-1.4.9.tar`

### file list

```diff
@@ -1,114 +1,104 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-05-22 17:34:32.493854 Files.com-1.4.81/
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-05-22 17:34:32.481854 Files.com-1.4.81/Files.com.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)      233 2024-05-22 17:34:32.000000 Files.com-1.4.81/Files.com.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3480 2024-05-22 17:34:32.000000 Files.com-1.4.81/Files.com.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)        1 2024-05-22 17:34:32.000000 Files.com-1.4.81/Files.com.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)       43 2024-05-22 17:34:32.000000 Files.com-1.4.81/Files.com.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)       10 2024-05-22 17:34:32.000000 Files.com-1.4.81/Files.com.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)      233 2024-05-22 17:34:32.493854 Files.com-1.4.81/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5785 2024-05-22 17:34:22.000000 Files.com-1.4.81/README.md
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-05-22 17:34:32.485854 Files.com-1.4.81/files_sdk/
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    11135 2024-05-22 17:34:31.000000 Files.com-1.4.81/files_sdk/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1606 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/api.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10789 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/api_client.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    60155 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/error.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1157 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/list_obj.py
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-05-22 17:34:32.493854 Files.com-1.4.81/files_sdk/models/
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5141 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1913 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/account_line_item.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1915 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/action.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6432 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/action_notification_export.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4071 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/action_notification_export_result.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2357 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/action_webhook_failure.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    16013 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/api_key.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    62800 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/api_request_log.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4655 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/app.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7265 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/as2_incoming_message.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6808 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/as2_outgoing_message.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    12559 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/as2_partner.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10676 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/as2_station.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)      995 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/auto.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    36787 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/automation.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    15298 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/automation_log.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4684 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/automation_run.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4755 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/bandwidth_snapshot.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    18152 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/behavior.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    31917 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/bundle.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5104 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/bundle_action.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4865 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/bundle_download.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8563 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/bundle_notification.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1249 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/bundle_path.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5647 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/bundle_recipient.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3384 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/bundle_registration.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    11290 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/clickwrap.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2370 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/dns_record.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5313 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/email_incoming_message.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3715 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/email_log.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1101 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/errors.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5863 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/exavault_api_request_log.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7628 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/external_event.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    32443 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/file.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1230 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/file_action.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7152 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/file_comment.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4350 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/file_comment_reaction.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2552 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/file_migration.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8369 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/file_migration_log.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2583 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/file_upload_part.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9010 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/folder.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1501 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/form_field.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9304 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/form_field_set.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    59363 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/ftp_action_log.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10440 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/gpg_key.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    14023 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/group.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9760 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/group_user.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    14183 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/history.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    14402 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/history_export.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6239 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/history_export_result.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1052 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/image.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5603 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/inbox_recipient.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3341 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/inbox_registration.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4714 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/inbox_upload.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3737 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/invoice.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1578 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/invoice_line_item.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5775 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/ip_address.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6673 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/lock.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10184 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/message.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8265 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/message_comment.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6517 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/message_comment_reaction.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6288 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/message_reaction.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    18662 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/notification.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3737 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/payment.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1284 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/payment_line_item.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7575 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/permission.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1347 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/preview.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2679 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/priority.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7510 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/project.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1259 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/public_ip_address.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8414 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/public_key.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4509 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/remote_bandwidth_snapshot.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    74125 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/remote_server.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3276 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/remote_server_configuration_file.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8681 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/request.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3790 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/session.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3317 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/settings_change.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    59657 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/sftp_action_log.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7918 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/sftp_host_key.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9058 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/share_group.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1248 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/share_group_member.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    47110 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/site.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9840 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/snapshot.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8680 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/sso_strategy.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1355 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/status.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5200 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/style.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8511 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/sync_log.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5518 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/usage_daily_snapshot.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3999 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/usage_snapshot.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    48670 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/user.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2954 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/user_cipher_use.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6187 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/user_request.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4601 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/models/webhook_test.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1694 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/path_util.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)      962 2024-05-22 17:34:22.000000 Files.com-1.4.81/files_sdk/util.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)      313 2024-05-22 17:34:22.000000 Files.com-1.4.81/pyproject.toml
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)       38 2024-05-22 17:34:32.493854 Files.com-1.4.81/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)      585 2024-05-22 17:34:22.000000 Files.com-1.4.81/setup.py
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-01-12 16:43:33.662317 Files.com-1.4.9/
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-01-12 16:43:33.654317 Files.com-1.4.9/Files.com.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)      232 2024-01-12 16:43:33.000000 Files.com-1.4.9/Files.com.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3129 2024-01-12 16:43:33.000000 Files.com-1.4.9/Files.com.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)        1 2024-01-12 16:43:33.000000 Files.com-1.4.9/Files.com.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)       43 2024-01-12 16:43:33.000000 Files.com-1.4.9/Files.com.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)       10 2024-01-12 16:43:33.000000 Files.com-1.4.9/Files.com.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)      232 2024-01-12 16:43:33.662317 Files.com-1.4.9/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5764 2024-01-12 16:43:22.000000 Files.com-1.4.9/README.md
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-01-12 16:43:33.654317 Files.com-1.4.9/files_sdk/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9986 2024-01-12 16:43:32.000000 Files.com-1.4.9/files_sdk/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1606 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/api.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10789 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/api_client.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    57103 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/error.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1157 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/list_obj.py
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-01-12 16:43:33.662317 Files.com-1.4.9/files_sdk/models/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4565 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1977 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/account_line_item.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1915 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/action.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6432 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/action_notification_export.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4071 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/action_notification_export_result.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2357 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/action_webhook_failure.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    16013 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/api_key.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4655 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/app.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7265 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/as2_incoming_message.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6808 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/as2_outgoing_message.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    11107 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/as2_partner.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10676 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/as2_station.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)      995 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/auto.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    29066 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/automation.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4467 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/automation_run.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4755 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/bandwidth_snapshot.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    17233 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/behavior.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    30540 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/bundle.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4865 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/bundle_download.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8563 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/bundle_notification.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5647 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/bundle_recipient.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3384 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/bundle_registration.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    11290 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/clickwrap.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2370 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/dns_record.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5313 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/email_incoming_message.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1101 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/errors.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7403 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/external_event.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    29891 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/file.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1230 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/file_action.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7152 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/file_comment.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4350 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/file_comment_reaction.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2552 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/file_migration.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2583 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/file_upload_part.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7285 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/folder.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1501 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/form_field.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9304 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/form_field_set.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10440 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/gpg_key.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    13089 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/group.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9760 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/group_user.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    14183 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/history.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    14156 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/history_export.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6188 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/history_export_result.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1052 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/image.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5603 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/inbox_recipient.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3341 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/inbox_registration.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4714 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/inbox_upload.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3801 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/invoice.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1657 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/invoice_line_item.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4660 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/ip_address.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6673 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/lock.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10184 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/message.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8265 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/message_comment.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6517 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/message_comment_reaction.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6288 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/message_reaction.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    18626 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/notification.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3801 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/payment.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1284 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/payment_line_item.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7575 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/permission.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1347 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/preview.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2679 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/priority.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7510 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/project.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1259 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/public_ip_address.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8414 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/public_key.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4509 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/remote_bandwidth_snapshot.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    74969 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/remote_server.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1721 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/remote_server_configuration_file.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8681 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/request.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3790 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/session.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3317 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/settings_change.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7918 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/sftp_host_key.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9058 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/share_group.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1248 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/share_group_member.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    43258 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/site.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8577 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/snapshot.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8580 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/sso_strategy.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1355 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/status.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5200 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/style.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5518 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/usage_daily_snapshot.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3999 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/usage_snapshot.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    47558 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/user.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2954 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/user_cipher_use.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5929 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/user_request.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4601 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/webhook_test.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1694 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/path_util.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)      962 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/util.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)      313 2024-01-12 16:43:22.000000 Files.com-1.4.9/pyproject.toml
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)       38 2024-01-12 16:43:33.662317 Files.com-1.4.9/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)      585 2024-01-12 16:43:22.000000 Files.com-1.4.9/setup.py
```

### Comparing `Files.com-1.4.81/Files.com.egg-info/SOURCES.txt` & `Files.com-1.4.9/Files.com.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,51 +16,43 @@
 files_sdk/models/__init__.py
 files_sdk/models/account_line_item.py
 files_sdk/models/action.py
 files_sdk/models/action_notification_export.py
 files_sdk/models/action_notification_export_result.py
 files_sdk/models/action_webhook_failure.py
 files_sdk/models/api_key.py
-files_sdk/models/api_request_log.py
 files_sdk/models/app.py
 files_sdk/models/as2_incoming_message.py
 files_sdk/models/as2_outgoing_message.py
 files_sdk/models/as2_partner.py
 files_sdk/models/as2_station.py
 files_sdk/models/auto.py
 files_sdk/models/automation.py
-files_sdk/models/automation_log.py
 files_sdk/models/automation_run.py
 files_sdk/models/bandwidth_snapshot.py
 files_sdk/models/behavior.py
 files_sdk/models/bundle.py
-files_sdk/models/bundle_action.py
 files_sdk/models/bundle_download.py
 files_sdk/models/bundle_notification.py
-files_sdk/models/bundle_path.py
 files_sdk/models/bundle_recipient.py
 files_sdk/models/bundle_registration.py
 files_sdk/models/clickwrap.py
 files_sdk/models/dns_record.py
 files_sdk/models/email_incoming_message.py
-files_sdk/models/email_log.py
 files_sdk/models/errors.py
-files_sdk/models/exavault_api_request_log.py
 files_sdk/models/external_event.py
 files_sdk/models/file.py
 files_sdk/models/file_action.py
 files_sdk/models/file_comment.py
 files_sdk/models/file_comment_reaction.py
 files_sdk/models/file_migration.py
-files_sdk/models/file_migration_log.py
 files_sdk/models/file_upload_part.py
 files_sdk/models/folder.py
 files_sdk/models/form_field.py
 files_sdk/models/form_field_set.py
-files_sdk/models/ftp_action_log.py
 files_sdk/models/gpg_key.py
 files_sdk/models/group.py
 files_sdk/models/group_user.py
 files_sdk/models/history.py
 files_sdk/models/history_export.py
 files_sdk/models/history_export_result.py
 files_sdk/models/image.py
@@ -86,23 +78,21 @@
 files_sdk/models/public_key.py
 files_sdk/models/remote_bandwidth_snapshot.py
 files_sdk/models/remote_server.py
 files_sdk/models/remote_server_configuration_file.py
 files_sdk/models/request.py
 files_sdk/models/session.py
 files_sdk/models/settings_change.py
-files_sdk/models/sftp_action_log.py
 files_sdk/models/sftp_host_key.py
 files_sdk/models/share_group.py
 files_sdk/models/share_group_member.py
 files_sdk/models/site.py
 files_sdk/models/snapshot.py
 files_sdk/models/sso_strategy.py
 files_sdk/models/status.py
 files_sdk/models/style.py
-files_sdk/models/sync_log.py
 files_sdk/models/usage_daily_snapshot.py
 files_sdk/models/usage_snapshot.py
 files_sdk/models/user.py
 files_sdk/models/user_cipher_use.py
 files_sdk/models/user_request.py
 files_sdk/models/webhook_test.py
```

### Comparing `Files.com-1.4.81/README.md` & `Files.com-1.4.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Files.com Python Client
 
 The Files.com Python client library provides convenient access to the Files.com API from applications written in the Python language.
 
-
 ## Installation
 
 To install the package:
 
     pip3 install Files.com
 
 
@@ -81,45 +80,39 @@
 and you can set the module specific log level and other logging settings by getting the logger
 object in the standard manner as shown below:
 
     import logging
 
     logging.getLogger("files_sdk")
 
-
 ### Error Handling
 
 Unexpected errors when attempting to connect to the API inherit from the base level `Error` class. They all contain a `__str__()`
 implementation to describe what went wrong.
 
-
 #### Unable to connect to the API
-
 ```python
 try:
     for f in files_sdk.folder.list_for("/").auto_paging_iter():
         print(f.type, f.path)
 except files_sdk.error.APIConnectionError as e:
     print("Unable to list root folder: " + str(e))
 ```
 
 Errors from the API inherit from `ApiError`. They all contain more properties to describe the error such as `code`, `headers`, etc.
 
-
 #### Path does not exist
-
 ```python
 try:
     for f in files_sdk.folder.list_for("/missing").auto_paging_iter():
         print(f.type, f.path)
 except files_sdk.error.FolderNotFoundError as e:
     print(f"Unable to list folder: {e.code}")
 ```
 
-
 ### File Operations
 
 This SDK allows both file based transfer and data based transfer. Please see the examples below.
 
 
 #### File Download
 
@@ -135,15 +128,14 @@
     files_sdk.file.upload_file("local.txt", "/remote.txt")
 
 If the parent directories do not already exist, they can be automatically created by passing
 `mkdir_parents` in the `params`.
 
     files_sdk.file.upload_file("local.txt", "/uploads/remote.txt", params={"mkdir_parents": True})
 
-
 #### List root folder
 
     for f in files_sdk.folder.list_for("/").auto_paging_iter():
         print(f.type, f.path)
 
 
 #### Writing a file example (string)
@@ -194,33 +186,31 @@
         print(f.type, f.path)
 
     while list_obj.has_next_page:
         list_obj.load_next_page()
         for f in list_obj:
             print(f.type, f.path)
 
-
 ### Comparing Case insensitive files and paths
 
-For related documentation see [Case Sensitivity Documentation](https://www.files.com/docs/files-and-folders/file-system-semantics/case-sensitivity).
+For related documentation see [Case Sensitivity Documentation](https://www.files.com/docs/topics/file-system-semantics#case-sensitivity).
 
     if files_sdk.path_util.is_same("Fïłèńämê.Txt", "filename.txt"):
         print("Paths are the same")
 
-
 ### Additional Object Documentation
 
 Additional docs are available at https://developers.files.com/ and also
 in the `docs/` subdirectory of this directory.
 
-
 ### Pydoc Generated Documentation coming in the future
 
 We hope to add Pydoc documentation to a future release.
 
 
 ## Getting Support
 
 The Files.com team is happy to help with any SDK Integration challenges you
 may face.
 
 Just email support@files.com and we'll get the process started.
+
```

### Comparing `Files.com-1.4.81/files_sdk/__init__.py` & `Files.com-1.4.9/files_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,43 @@
 from pathlib import Path
 import files_sdk.models.account_line_item as account_line_item
 import files_sdk.models.action as action
 import files_sdk.models.action_notification_export as action_notification_export
 import files_sdk.models.action_notification_export_result as action_notification_export_result
 import files_sdk.models.action_webhook_failure as action_webhook_failure
 import files_sdk.models.api_key as api_key
-import files_sdk.models.api_request_log as api_request_log
 import files_sdk.models.app as app
 import files_sdk.models.as2_incoming_message as as2_incoming_message
 import files_sdk.models.as2_outgoing_message as as2_outgoing_message
 import files_sdk.models.as2_partner as as2_partner
 import files_sdk.models.as2_station as as2_station
 import files_sdk.models.auto as auto
 import files_sdk.models.automation as automation
-import files_sdk.models.automation_log as automation_log
 import files_sdk.models.automation_run as automation_run
 import files_sdk.models.bandwidth_snapshot as bandwidth_snapshot
 import files_sdk.models.behavior as behavior
 import files_sdk.models.bundle as bundle
-import files_sdk.models.bundle_action as bundle_action
 import files_sdk.models.bundle_download as bundle_download
 import files_sdk.models.bundle_notification as bundle_notification
-import files_sdk.models.bundle_path as bundle_path
 import files_sdk.models.bundle_recipient as bundle_recipient
 import files_sdk.models.bundle_registration as bundle_registration
 import files_sdk.models.clickwrap as clickwrap
 import files_sdk.models.dns_record as dns_record
 import files_sdk.models.email_incoming_message as email_incoming_message
-import files_sdk.models.email_log as email_log
 import files_sdk.models.errors as errors
-import files_sdk.models.exavault_api_request_log as exavault_api_request_log
 import files_sdk.models.external_event as external_event
 import files_sdk.models.file as file
 import files_sdk.models.file_action as file_action
 import files_sdk.models.file_comment as file_comment
 import files_sdk.models.file_comment_reaction as file_comment_reaction
 import files_sdk.models.file_migration as file_migration
-import files_sdk.models.file_migration_log as file_migration_log
 import files_sdk.models.file_upload_part as file_upload_part
 import files_sdk.models.folder as folder
 import files_sdk.models.form_field as form_field
 import files_sdk.models.form_field_set as form_field_set
-import files_sdk.models.ftp_action_log as ftp_action_log
 import files_sdk.models.gpg_key as gpg_key
 import files_sdk.models.group as group
 import files_sdk.models.group_user as group_user
 import files_sdk.models.history as history
 import files_sdk.models.history_export as history_export
 import files_sdk.models.history_export_result as history_export_result
 import files_sdk.models.image as image
@@ -71,24 +63,22 @@
 import files_sdk.models.public_key as public_key
 import files_sdk.models.remote_bandwidth_snapshot as remote_bandwidth_snapshot
 import files_sdk.models.remote_server as remote_server
 import files_sdk.models.remote_server_configuration_file as remote_server_configuration_file
 import files_sdk.models.request as request
 import files_sdk.models.session as session
 import files_sdk.models.settings_change as settings_change
-import files_sdk.models.sftp_action_log as sftp_action_log
 import files_sdk.models.sftp_host_key as sftp_host_key
 import files_sdk.models.share_group as share_group
 import files_sdk.models.share_group_member as share_group_member
 import files_sdk.models.site as site
 import files_sdk.models.snapshot as snapshot
 import files_sdk.models.sso_strategy as sso_strategy
 import files_sdk.models.status as status
 import files_sdk.models.style as style
-import files_sdk.models.sync_log as sync_log
 import files_sdk.models.usage_daily_snapshot as usage_daily_snapshot
 import files_sdk.models.usage_snapshot as usage_snapshot
 import files_sdk.models.user as user
 import files_sdk.models.user_cipher_use as user_cipher_use
 import files_sdk.models.user_request as user_request
 import files_sdk.models.webhook_test as webhook_test
 
@@ -98,51 +88,43 @@
     ActionNotificationExport,
 )
 from files_sdk.models.action_notification_export_result import (
     ActionNotificationExportResult,
 )
 from files_sdk.models.action_webhook_failure import ActionWebhookFailure
 from files_sdk.models.api_key import ApiKey
-from files_sdk.models.api_request_log import ApiRequestLog
 from files_sdk.models.app import App
 from files_sdk.models.as2_incoming_message import As2IncomingMessage
 from files_sdk.models.as2_outgoing_message import As2OutgoingMessage
 from files_sdk.models.as2_partner import As2Partner
 from files_sdk.models.as2_station import As2Station
 from files_sdk.models.auto import Auto
 from files_sdk.models.automation import Automation
-from files_sdk.models.automation_log import AutomationLog
 from files_sdk.models.automation_run import AutomationRun
 from files_sdk.models.bandwidth_snapshot import BandwidthSnapshot
 from files_sdk.models.behavior import Behavior
 from files_sdk.models.bundle import Bundle
-from files_sdk.models.bundle_action import BundleAction
 from files_sdk.models.bundle_download import BundleDownload
 from files_sdk.models.bundle_notification import BundleNotification
-from files_sdk.models.bundle_path import BundlePath
 from files_sdk.models.bundle_recipient import BundleRecipient
 from files_sdk.models.bundle_registration import BundleRegistration
 from files_sdk.models.clickwrap import Clickwrap
 from files_sdk.models.dns_record import DnsRecord
 from files_sdk.models.email_incoming_message import EmailIncomingMessage
-from files_sdk.models.email_log import EmailLog
 from files_sdk.models.errors import Errors
-from files_sdk.models.exavault_api_request_log import ExavaultApiRequestLog
 from files_sdk.models.external_event import ExternalEvent
 from files_sdk.models.file import File
 from files_sdk.models.file_action import FileAction
 from files_sdk.models.file_comment import FileComment
 from files_sdk.models.file_comment_reaction import FileCommentReaction
 from files_sdk.models.file_migration import FileMigration
-from files_sdk.models.file_migration_log import FileMigrationLog
 from files_sdk.models.file_upload_part import FileUploadPart
 from files_sdk.models.folder import Folder
 from files_sdk.models.form_field import FormField
 from files_sdk.models.form_field_set import FormFieldSet
-from files_sdk.models.ftp_action_log import FtpActionLog
 from files_sdk.models.gpg_key import GpgKey
 from files_sdk.models.group import Group
 from files_sdk.models.group_user import GroupUser
 from files_sdk.models.history import History
 from files_sdk.models.history_export import HistoryExport
 from files_sdk.models.history_export_result import HistoryExportResult
 from files_sdk.models.image import Image
@@ -170,38 +152,36 @@
 from files_sdk.models.remote_server import RemoteServer
 from files_sdk.models.remote_server_configuration_file import (
     RemoteServerConfigurationFile,
 )
 from files_sdk.models.request import Request
 from files_sdk.models.session import Session
 from files_sdk.models.settings_change import SettingsChange
-from files_sdk.models.sftp_action_log import SftpActionLog
 from files_sdk.models.sftp_host_key import SftpHostKey
 from files_sdk.models.share_group import ShareGroup
 from files_sdk.models.share_group_member import ShareGroupMember
 from files_sdk.models.site import Site
 from files_sdk.models.snapshot import Snapshot
 from files_sdk.models.sso_strategy import SsoStrategy
 from files_sdk.models.status import Status
 from files_sdk.models.style import Style
-from files_sdk.models.sync_log import SyncLog
 from files_sdk.models.usage_daily_snapshot import UsageDailySnapshot
 from files_sdk.models.usage_snapshot import UsageSnapshot
 from files_sdk.models.user import User
 from files_sdk.models.user_cipher_use import UserCipherUse
 from files_sdk.models.user_request import UserRequest
 from files_sdk.models.webhook_test import WebhookTest
 
 import files_sdk.path_util
 
 the_api_key = ""
 session_id = None
 base_url = "https://app.files.com"
 base_path = "api/rest/v1"
-version = "1.4.81"
+version = "1.4.9"
 
 __version__ = version
 
 initial_network_retry_delay = 0.5
 max_network_retry_delay = 2
 open_timeout = 30
 read_timeout = 80
```

### Comparing `Files.com-1.4.81/files_sdk/api.py` & `Files.com-1.4.9/files_sdk/api.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/api_client.py` & `Files.com-1.4.9/files_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/error.py` & `Files.com-1.4.9/files_sdk/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -498,30 +498,30 @@
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class PartNumberTooLargeError(BadRequestError):
+class OperationOnNonScimResourceError(BadRequestError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class PathCannotHaveTrailingWhitespaceError(BadRequestError):
+class PartNumberTooLargeError(BadRequestError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
@@ -543,180 +543,180 @@
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class RequestParamsContainInvalidCharacterError(BadRequestError):
+class RequestParamPathCannotHaveTrailingWhitespaceError(BadRequestError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class RequestParamsInvalidError(BadRequestError):
+class RequestParamsContainInvalidCharacterError(BadRequestError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class RequestParamsRequiredError(BadRequestError):
+class RequestParamsInvalidError(BadRequestError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class SearchAllOnChildPathError(BadRequestError):
+class RequestParamsRequiredError(BadRequestError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class UnsupportedCurrencyError(BadRequestError):
+class SearchAllOnChildPathError(BadRequestError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class UnsupportedHttpResponseFormatError(BadRequestError):
+class UnsupportedCurrencyError(BadRequestError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class UnsupportedMediaTypeError(BadRequestError):
+class UnsupportedHttpResponseFormatError(BadRequestError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class UserIdInvalidError(BadRequestError):
+class UnsupportedMediaTypeError(BadRequestError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class UserIdOnUserEndpointError(BadRequestError):
+class UserIdInvalidError(BadRequestError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class UserRequiredError(BadRequestError):
+class UserIdOnUserEndpointError(BadRequestError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class NotAuthenticatedError(APIError):
+class UserRequiredError(BadRequestError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class AdditionalAuthenticationRequiredError(NotAuthenticatedError):
+class NotAuthenticatedError(APIError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
@@ -1338,29 +1338,14 @@
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class RecaptchaFailedError(NotAuthorizedError):
-    def __init__(
-        self,
-        message=None,
-        http_body=None,
-        http_status=None,
-        json_body=None,
-        headers=None,
-        code=None,
-    ):
-        super().__init__(
-            message, http_body, http_status, json_body, headers, code
-        )
-
-
 class SelfManagedRequiredError(NotAuthorizedError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
@@ -1698,29 +1683,14 @@
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class AlreadyCompletedError(ProcessingFailureError):
-    def __init__(
-        self,
-        message=None,
-        http_body=None,
-        http_status=None,
-        json_body=None,
-        headers=None,
-        code=None,
-    ):
-        super().__init__(
-            message, http_body, http_status, json_body, headers, code
-        )
-
-
 class AutomationCannotBeRunManuallyError(ProcessingFailureError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
@@ -1728,29 +1698,14 @@
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class BehaviorNotAllowedOnRemoteServerError(ProcessingFailureError):
-    def __init__(
-        self,
-        message=None,
-        http_body=None,
-        http_status=None,
-        json_body=None,
-        headers=None,
-        code=None,
-    ):
-        super().__init__(
-            message, http_body, http_status, json_body, headers, code
-        )
-
-
 class BundleOnlyAllowsPreviewsError(ProcessingFailureError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
@@ -1968,29 +1923,14 @@
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class FileProcessingErrorError(ProcessingFailureError):
-    def __init__(
-        self,
-        message=None,
-        http_body=None,
-        http_status=None,
-        json_body=None,
-        headers=None,
-        code=None,
-    ):
-        super().__init__(
-            message, http_body, http_status, json_body, headers, code
-        )
-
-
 class FileTooBigToDecryptError(ProcessingFailureError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
@@ -2028,29 +1968,14 @@
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class FilenameTooLongError(ProcessingFailureError):
-    def __init__(
-        self,
-        message=None,
-        http_body=None,
-        http_status=None,
-        json_body=None,
-        headers=None,
-        code=None,
-    ):
-        super().__init__(
-            message, http_body, http_status, json_body, headers, code
-        )
-
-
 class FolderLockedError(ProcessingFailureError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
@@ -2133,29 +2058,14 @@
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class InvalidPriorityColorError(ProcessingFailureError):
-    def __init__(
-        self,
-        message=None,
-        http_body=None,
-        http_status=None,
-        json_body=None,
-        headers=None,
-        code=None,
-    ):
-        super().__init__(
-            message, http_body, http_status, json_body, headers, code
-        )
-
-
 class InvalidRangeError(ProcessingFailureError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
@@ -2390,29 +2300,14 @@
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
 
 
-class TooManyConcurrentLoginsError(RateLimitedError):
-    def __init__(
-        self,
-        message=None,
-        http_body=None,
-        http_status=None,
-        json_body=None,
-        headers=None,
-        code=None,
-    ):
-        super().__init__(
-            message, http_body, http_status, json_body, headers, code
-        )
-
-
 class TooManyConcurrentRequestsError(RateLimitedError):
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
@@ -2503,44 +2398,14 @@
     def __init__(
         self,
         message=None,
         http_body=None,
         http_status=None,
         json_body=None,
         headers=None,
-        code=None,
-    ):
-        super().__init__(
-            message, http_body, http_status, json_body, headers, code
-        )
-
-
-class MigrationInProgressError(ServiceUnavailableError):
-    def __init__(
-        self,
-        message=None,
-        http_body=None,
-        http_status=None,
-        json_body=None,
-        headers=None,
-        code=None,
-    ):
-        super().__init__(
-            message, http_body, http_status, json_body, headers, code
-        )
-
-
-class SiteDisabledError(ServiceUnavailableError):
-    def __init__(
-        self,
-        message=None,
-        http_body=None,
-        http_status=None,
-        json_body=None,
-        headers=None,
         code=None,
     ):
         super().__init__(
             message, http_body, http_status, json_body, headers, code
         )
```

### Comparing `Files.com-1.4.81/files_sdk/list_obj.py` & `Files.com-1.4.9/files_sdk/list_obj.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/__init__.py` & `Files.com-1.4.9/files_sdk/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,51 +4,43 @@
     ActionNotificationExport,
 )
 from files_sdk.models.action_notification_export_result import (
     ActionNotificationExportResult,
 )
 from files_sdk.models.action_webhook_failure import ActionWebhookFailure
 from files_sdk.models.api_key import ApiKey
-from files_sdk.models.api_request_log import ApiRequestLog
 from files_sdk.models.app import App
 from files_sdk.models.as2_incoming_message import As2IncomingMessage
 from files_sdk.models.as2_outgoing_message import As2OutgoingMessage
 from files_sdk.models.as2_partner import As2Partner
 from files_sdk.models.as2_station import As2Station
 from files_sdk.models.auto import Auto
 from files_sdk.models.automation import Automation
-from files_sdk.models.automation_log import AutomationLog
 from files_sdk.models.automation_run import AutomationRun
 from files_sdk.models.bandwidth_snapshot import BandwidthSnapshot
 from files_sdk.models.behavior import Behavior
 from files_sdk.models.bundle import Bundle
-from files_sdk.models.bundle_action import BundleAction
 from files_sdk.models.bundle_download import BundleDownload
 from files_sdk.models.bundle_notification import BundleNotification
-from files_sdk.models.bundle_path import BundlePath
 from files_sdk.models.bundle_recipient import BundleRecipient
 from files_sdk.models.bundle_registration import BundleRegistration
 from files_sdk.models.clickwrap import Clickwrap
 from files_sdk.models.dns_record import DnsRecord
 from files_sdk.models.email_incoming_message import EmailIncomingMessage
-from files_sdk.models.email_log import EmailLog
 from files_sdk.models.errors import Errors
-from files_sdk.models.exavault_api_request_log import ExavaultApiRequestLog
 from files_sdk.models.external_event import ExternalEvent
 from files_sdk.models.file import File
 from files_sdk.models.file_action import FileAction
 from files_sdk.models.file_comment import FileComment
 from files_sdk.models.file_comment_reaction import FileCommentReaction
 from files_sdk.models.file_migration import FileMigration
-from files_sdk.models.file_migration_log import FileMigrationLog
 from files_sdk.models.file_upload_part import FileUploadPart
 from files_sdk.models.folder import Folder
 from files_sdk.models.form_field import FormField
 from files_sdk.models.form_field_set import FormFieldSet
-from files_sdk.models.ftp_action_log import FtpActionLog
 from files_sdk.models.gpg_key import GpgKey
 from files_sdk.models.group import Group
 from files_sdk.models.group_user import GroupUser
 from files_sdk.models.history import History
 from files_sdk.models.history_export import HistoryExport
 from files_sdk.models.history_export_result import HistoryExportResult
 from files_sdk.models.image import Image
@@ -76,23 +68,21 @@
 from files_sdk.models.remote_server import RemoteServer
 from files_sdk.models.remote_server_configuration_file import (
     RemoteServerConfigurationFile,
 )
 from files_sdk.models.request import Request
 from files_sdk.models.session import Session
 from files_sdk.models.settings_change import SettingsChange
-from files_sdk.models.sftp_action_log import SftpActionLog
 from files_sdk.models.sftp_host_key import SftpHostKey
 from files_sdk.models.share_group import ShareGroup
 from files_sdk.models.share_group_member import ShareGroupMember
 from files_sdk.models.site import Site
 from files_sdk.models.snapshot import Snapshot
 from files_sdk.models.sso_strategy import SsoStrategy
 from files_sdk.models.status import Status
 from files_sdk.models.style import Style
-from files_sdk.models.sync_log import SyncLog
 from files_sdk.models.usage_daily_snapshot import UsageDailySnapshot
 from files_sdk.models.usage_snapshot import UsageSnapshot
 from files_sdk.models.user import User
 from files_sdk.models.user_cipher_use import UserCipherUse
 from files_sdk.models.user_request import UserRequest
 from files_sdk.models.webhook_test import WebhookTest
```

### Comparing `Files.com-1.4.81/files_sdk/models/account_line_item.py` & `Files.com-1.4.9/files_sdk/models/account_line_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         "invoice_line_items": None,  # array - Associated invoice line items
         "method": None,  # string - Line item payment method
         "payment_line_items": None,  # array - Associated payment line items
         "payment_reversed_at": None,  # date-time - Date/time payment was reversed if applicable
         "payment_type": None,  # string - Type of payment if applicable
         "site_name": None,  # string - Site name this line item is for
         "type": None,  # string - Type of line item, either payment or invoice
+        "updated_at": None,  # date-time - Line item updated at
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
             options = {}
```

### Comparing `Files.com-1.4.81/files_sdk/models/action.py` & `Files.com-1.4.9/files_sdk/models/action.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/action_notification_export.py` & `Files.com-1.4.9/files_sdk/models/action_notification_export.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/action_notification_export_result.py` & `Files.com-1.4.9/files_sdk/models/action_notification_export_result.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/action_webhook_failure.py` & `Files.com-1.4.9/files_sdk/models/action_webhook_failure.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/api_key.py` & `Files.com-1.4.9/files_sdk/models/api_key.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/app.py` & `Files.com-1.4.9/files_sdk/models/app.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/as2_incoming_message.py` & `Files.com-1.4.9/files_sdk/models/as2_incoming_message.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/as2_outgoing_message.py` & `Files.com-1.4.9/files_sdk/models/as2_outgoing_message.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/as2_partner.py` & `Files.com-1.4.9/files_sdk/models/as2_partner.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 class As2Partner:
     default_attributes = {
         "id": None,  # int64 - Id of the AS2 Partner.
         "as2_station_id": None,  # int64 - Id of the AS2 Station associated with this partner.
         "name": None,  # string - The partner's formal AS2 name.
         "uri": None,  # string - Public URI for sending AS2 message to.
         "server_certificate": None,  # string - Remote server certificate security setting
-        "mdn_validation_level": None,  # string - MDN Validation Level controls how to evaluate message transfer success based on a partner's MDN response. NOTE: This setting does not affect MDN storage; all MDNs received from a partner are always stored. `none`: MDN is stored for informational purposes only, a successful HTTPS transfer is a successful AS2 transfer. `weak`: Inspect the MDN for MIC and Disposition only. `normal`: `weak` plus validate MDN signature matches body, `strict`: `normal` but do not allow signatures from self-signed or incorrectly purposed certificates.
         "enable_dedicated_ips": None,  # boolean - `true` if remote server only accepts connections from dedicated IPs
         "hex_public_certificate_serial": None,  # string - Serial of public certificate used for message security in hex format.
         "public_certificate_md5": None,  # string - MD5 hash of public certificate used for message security.
         "public_certificate_subject": None,  # string - Subject of public certificate used for message security.
         "public_certificate_issuer": None,  # string - Issuer of public certificate used for message security.
         "public_certificate_serial": None,  # string - Serial of public certificate used for message security.
         "public_certificate_not_before": None,  # string - Not before value of public certificate used for message security.
@@ -46,15 +45,14 @@
             if getattr(self, k, None) is not None
         }
 
     # Parameters:
     #   name - string - AS2 Name
     #   uri - string - URL base for AS2 responses
     #   server_certificate - string - Remote server certificate security setting
-    #   mdn_validation_level - string - MDN Validation Level
     #   public_certificate - string
     #   enable_dedicated_ips - boolean
     def update(self, params=None):
         if not isinstance(params, dict):
             params = {}
 
         if hasattr(self, "id") and self.id:
@@ -71,20 +69,14 @@
             raise InvalidParameterError("Bad parameter: uri must be an str")
         if "server_certificate" in params and not isinstance(
             params["server_certificate"], str
         ):
             raise InvalidParameterError(
                 "Bad parameter: server_certificate must be an str"
             )
-        if "mdn_validation_level" in params and not isinstance(
-            params["mdn_validation_level"], str
-        ):
-            raise InvalidParameterError(
-                "Bad parameter: mdn_validation_level must be an str"
-            )
         if "public_certificate" in params and not isinstance(
             params["public_certificate"], str
         ):
             raise InvalidParameterError(
                 "Bad parameter: public_certificate must be an str"
             )
         response, _options = Api.send_request(
@@ -171,15 +163,14 @@
 
 # Parameters:
 #   name (required) - string - AS2 Name
 #   uri (required) - string - URL base for AS2 responses
 #   public_certificate (required) - string
 #   as2_station_id (required) - int64 - Id of As2Station for this partner
 #   server_certificate - string - Remote server certificate security setting
-#   mdn_validation_level - string - MDN Validation Level
 #   enable_dedicated_ips - boolean
 def create(params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     if "name" in params and not isinstance(params["name"], str):
@@ -200,20 +191,14 @@
         )
     if "server_certificate" in params and not isinstance(
         params["server_certificate"], str
     ):
         raise InvalidParameterError(
             "Bad parameter: server_certificate must be an str"
         )
-    if "mdn_validation_level" in params and not isinstance(
-        params["mdn_validation_level"], str
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: mdn_validation_level must be an str"
-        )
     if "name" not in params:
         raise MissingParameterError("Parameter missing: name")
     if "uri" not in params:
         raise MissingParameterError("Parameter missing: uri")
     if "public_certificate" not in params:
         raise MissingParameterError("Parameter missing: public_certificate")
     if "as2_station_id" not in params:
@@ -224,15 +209,14 @@
     return As2Partner(response.data, options)
 
 
 # Parameters:
 #   name - string - AS2 Name
 #   uri - string - URL base for AS2 responses
 #   server_certificate - string - Remote server certificate security setting
-#   mdn_validation_level - string - MDN Validation Level
 #   public_certificate - string
 #   enable_dedicated_ips - boolean
 def update(id, params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
@@ -245,20 +229,14 @@
         raise InvalidParameterError("Bad parameter: uri must be an str")
     if "server_certificate" in params and not isinstance(
         params["server_certificate"], str
     ):
         raise InvalidParameterError(
             "Bad parameter: server_certificate must be an str"
         )
-    if "mdn_validation_level" in params and not isinstance(
-        params["mdn_validation_level"], str
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: mdn_validation_level must be an str"
-        )
     if "public_certificate" in params and not isinstance(
         params["public_certificate"], str
     ):
         raise InvalidParameterError(
             "Bad parameter: public_certificate must be an str"
         )
     if "id" not in params:
```

### Comparing `Files.com-1.4.81/files_sdk/models/as2_station.py` & `Files.com-1.4.9/files_sdk/models/as2_station.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/auto.py` & `Files.com-1.4.9/files_sdk/models/auto.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/automation.py` & `Files.com-1.4.9/files_sdk/models/automation.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,29 +15,21 @@
         "automation": None,  # string - Automation type
         "deleted": None,  # boolean - Indicates if the automation has been deleted.
         "description": None,  # string - Description for the this Automation.
         "destination_replace_from": None,  # string - If set, this string in the destination path will be replaced with the value in `destination_replace_to`.
         "destination_replace_to": None,  # string - If set, this string will replace the value `destination_replace_from` in the destination filename. You can use special patterns here.
         "destinations": None,  # array - Destination Paths
         "disabled": None,  # boolean - If true, this automation will not run.
-        "flatten_destination_structure": None,  # boolean - Normally copy and move automations that use globs will implicitly preserve the source folder structure in the destination.  If this flag is `true`, the source folder structure will be flattened in the destination.  This is useful for copying or moving files from multiple folders into a single destination folder.
         "group_ids": None,  # array - IDs of Groups for the Automation (i.e. who to Request File from)
-        "ignore_locked_folders": None,  # boolean - If true, the Lock Folders behavior will be disregarded for automated actions.
         "interval": None,  # string - If trigger is `daily`, this specifies how often to run this automation.  One of: `day`, `week`, `week_end`, `month`, `month_end`, `quarter`, `quarter_end`, `year`, `year_end`
         "last_modified_at": None,  # date-time - Time when automation was last modified. Does not change for name or description updates.
         "name": None,  # string - Name for this automation.
-        "overwrite_files": None,  # boolean - If true, existing files will be overwritten with new files on Move/Copy automations.  Note: by default files will not be overwritten if they appear to be the same file size as the newly incoming file.  Use the `:always_overwrite_size_matching_files` option to override this.
         "path": None,  # string - Path on which this Automation runs.  Supports globs, except on remote mounts. This must be slash-delimited, but it must neither start nor end with a slash. Maximum of 5000 characters.
-        "path_time_zone": None,  # string - Timezone to use when rendering timestamps in paths.
         "recurring_day": None,  # int64 - If trigger type is `daily`, this specifies a day number to run in one of the supported intervals: `week`, `month`, `quarter`, `year`.
-        "schedule": None,  # object - If trigger is `custom_schedule`, Custom schedule description for when the automation should be run in json format.
-        "human_readable_schedule": None,  # string - If trigger is `custom_schedule`, Human readable Custom schedule description for when the automation should be run.
-        "schedule_days_of_week": None,  # array - If trigger is `custom_schedule`, Custom schedule description for when the automation should be run. 0-based days of the week. 0 is Sunday, 1 is Monday, etc.
-        "schedule_times_of_day": None,  # array - If trigger is `custom_schedule`, Custom schedule description for when the automation should be run. Times of day in HH:MM format.
-        "schedule_time_zone": None,  # string - If trigger is `custom_schedule`, Custom schedule Time Zone for when the automation should be run.
+        "schedule": None,  # object - If trigger is `custom_schedule`, Custom schedule description for when the automation should be run.
         "source": None,  # string - Source Path
         "sync_ids": None,  # array - IDs of remote sync folder behaviors to run by this Automation
         "trigger_actions": None,  # array - If trigger is `action`, this is the list of action types on which to trigger the automation. Valid actions are create, read, update, destroy, move, copy
         "trigger": None,  # string - How this automation is triggered to run.
         "user_id": None,  # int64 - User ID of the Automation's creator.
         "user_ids": None,  # array - IDs of Users for the Automation (i.e. who to Request File from)
         "value": None,  # object - A Hash of attributes specific to the automation type.
@@ -91,25 +83,19 @@
     #   destination_replace_from - string - If set, this string in the destination path will be replaced with the value in `destination_replace_to`.
     #   destination_replace_to - string - If set, this string will replace the value `destination_replace_from` in the destination filename. You can use special patterns here.
     #   interval - string - How often to run this automation? One of: `day`, `week`, `week_end`, `month`, `month_end`, `quarter`, `quarter_end`, `year`, `year_end`
     #   path - string - Path on which this Automation runs.  Supports globs.
     #   sync_ids - string - A list of sync IDs the automation is associated with. If sent as a string, it should be comma-delimited.
     #   user_ids - string - A list of user IDs the automation is associated with. If sent as a string, it should be comma-delimited.
     #   group_ids - string - A list of group IDs the automation is associated with. If sent as a string, it should be comma-delimited.
-    #   schedule_days_of_week - array(int64) - If trigger is `custom_schedule`. A list of days of the week to run this automation. 0 is Sunday, 1 is Monday, etc.
-    #   schedule_times_of_day - array(string) - If trigger is `custom_schedule`. A list of times of day to run this automation. 24-hour time format.
-    #   schedule_time_zone - string - If trigger is `custom_schedule`. Time zone for the schedule.
+    #   schedule - object - Custom schedule for running this automation.
     #   always_overwrite_size_matching_files - boolean - Ordinarily, files with identical size in the source and destination will be skipped from copy operations to prevent wasted transfer.  If this flag is `true` we will overwrite the destination file always.  Note that this may cause large amounts of wasted transfer usage.
     #   description - string - Description for the this Automation.
     #   disabled - boolean - If true, this automation will not run.
-    #   flatten_destination_structure - boolean - Normally copy and move automations that use globs will implicitly preserve the source folder structure in the destination.  If this flag is `true`, the source folder structure will be flattened in the destination.  This is useful for copying or moving files from multiple folders into a single destination folder.
-    #   ignore_locked_folders - boolean - If true, the Lock Folders behavior will be disregarded for automated actions.
     #   name - string - Name for this automation.
-    #   overwrite_files - boolean - If true, existing files will be overwritten with new files on Move/Copy automations.  Note: by default files will not be overwritten if they appear to be the same file size as the newly incoming file.  Use the `:always_overwrite_size_matching_files` option to override this.
-    #   path_time_zone - string - Timezone to use when rendering timestamps in paths.
     #   trigger - string - How this automation is triggered to run.
     #   trigger_actions - array(string) - If trigger is `action`, this is the list of action types on which to trigger the automation. Valid actions are create, read, update, destroy, move, copy
     #   value - object - A Hash of attributes specific to the automation type.
     #   recurring_day - int64 - If trigger type is `daily`, this specifies a day number to run in one of the supported intervals: `week`, `month`, `quarter`, `year`.
     #   automation - string - Automation type
     def update(self, params=None):
         if not isinstance(params, dict):
@@ -163,46 +149,22 @@
             raise InvalidParameterError(
                 "Bad parameter: user_ids must be an str"
             )
         if "group_ids" in params and not isinstance(params["group_ids"], str):
             raise InvalidParameterError(
                 "Bad parameter: group_ids must be an str"
             )
-        if "schedule_days_of_week" in params and not isinstance(
-            params["schedule_days_of_week"], builtins.list
-        ):
-            raise InvalidParameterError(
-                "Bad parameter: schedule_days_of_week must be an list"
-            )
-        if "schedule_times_of_day" in params and not isinstance(
-            params["schedule_times_of_day"], builtins.list
-        ):
-            raise InvalidParameterError(
-                "Bad parameter: schedule_times_of_day must be an list"
-            )
-        if "schedule_time_zone" in params and not isinstance(
-            params["schedule_time_zone"], str
-        ):
-            raise InvalidParameterError(
-                "Bad parameter: schedule_time_zone must be an str"
-            )
         if "description" in params and not isinstance(
             params["description"], str
         ):
             raise InvalidParameterError(
                 "Bad parameter: description must be an str"
             )
         if "name" in params and not isinstance(params["name"], str):
             raise InvalidParameterError("Bad parameter: name must be an str")
-        if "path_time_zone" in params and not isinstance(
-            params["path_time_zone"], str
-        ):
-            raise InvalidParameterError(
-                "Bad parameter: path_time_zone must be an str"
-            )
         if "trigger" in params and not isinstance(params["trigger"], str):
             raise InvalidParameterError(
                 "Bad parameter: trigger must be an str"
             )
         if "trigger_actions" in params and not isinstance(
             params["trigger_actions"], builtins.list
         ):
@@ -333,25 +295,19 @@
 #   destination_replace_from - string - If set, this string in the destination path will be replaced with the value in `destination_replace_to`.
 #   destination_replace_to - string - If set, this string will replace the value `destination_replace_from` in the destination filename. You can use special patterns here.
 #   interval - string - How often to run this automation? One of: `day`, `week`, `week_end`, `month`, `month_end`, `quarter`, `quarter_end`, `year`, `year_end`
 #   path - string - Path on which this Automation runs.  Supports globs.
 #   sync_ids - string - A list of sync IDs the automation is associated with. If sent as a string, it should be comma-delimited.
 #   user_ids - string - A list of user IDs the automation is associated with. If sent as a string, it should be comma-delimited.
 #   group_ids - string - A list of group IDs the automation is associated with. If sent as a string, it should be comma-delimited.
-#   schedule_days_of_week - array(int64) - If trigger is `custom_schedule`. A list of days of the week to run this automation. 0 is Sunday, 1 is Monday, etc.
-#   schedule_times_of_day - array(string) - If trigger is `custom_schedule`. A list of times of day to run this automation. 24-hour time format.
-#   schedule_time_zone - string - If trigger is `custom_schedule`. Time zone for the schedule.
+#   schedule - object - Custom schedule for running this automation.
 #   always_overwrite_size_matching_files - boolean - Ordinarily, files with identical size in the source and destination will be skipped from copy operations to prevent wasted transfer.  If this flag is `true` we will overwrite the destination file always.  Note that this may cause large amounts of wasted transfer usage.
 #   description - string - Description for the this Automation.
 #   disabled - boolean - If true, this automation will not run.
-#   flatten_destination_structure - boolean - Normally copy and move automations that use globs will implicitly preserve the source folder structure in the destination.  If this flag is `true`, the source folder structure will be flattened in the destination.  This is useful for copying or moving files from multiple folders into a single destination folder.
-#   ignore_locked_folders - boolean - If true, the Lock Folders behavior will be disregarded for automated actions.
 #   name - string - Name for this automation.
-#   overwrite_files - boolean - If true, existing files will be overwritten with new files on Move/Copy automations.  Note: by default files will not be overwritten if they appear to be the same file size as the newly incoming file.  Use the `:always_overwrite_size_matching_files` option to override this.
-#   path_time_zone - string - Timezone to use when rendering timestamps in paths.
 #   trigger - string - How this automation is triggered to run.
 #   trigger_actions - array(string) - If trigger is `action`, this is the list of action types on which to trigger the automation. Valid actions are create, read, update, destroy, move, copy
 #   value - object - A Hash of attributes specific to the automation type.
 #   recurring_day - int64 - If trigger type is `daily`, this specifies a day number to run in one of the supported intervals: `week`, `month`, `quarter`, `year`.
 #   automation (required) - string - Automation type
 def create(params=None, options=None):
     if not isinstance(params, dict):
@@ -388,44 +344,22 @@
         raise InvalidParameterError("Bad parameter: path must be an str")
     if "sync_ids" in params and not isinstance(params["sync_ids"], str):
         raise InvalidParameterError("Bad parameter: sync_ids must be an str")
     if "user_ids" in params and not isinstance(params["user_ids"], str):
         raise InvalidParameterError("Bad parameter: user_ids must be an str")
     if "group_ids" in params and not isinstance(params["group_ids"], str):
         raise InvalidParameterError("Bad parameter: group_ids must be an str")
-    if "schedule_days_of_week" in params and not isinstance(
-        params["schedule_days_of_week"], builtins.list
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: schedule_days_of_week must be an list"
-        )
-    if "schedule_times_of_day" in params and not isinstance(
-        params["schedule_times_of_day"], builtins.list
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: schedule_times_of_day must be an list"
-        )
-    if "schedule_time_zone" in params and not isinstance(
-        params["schedule_time_zone"], str
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: schedule_time_zone must be an str"
-        )
+    if "schedule" in params and not isinstance(params["schedule"], dict):
+        raise InvalidParameterError("Bad parameter: schedule must be an dict")
     if "description" in params and not isinstance(params["description"], str):
         raise InvalidParameterError(
             "Bad parameter: description must be an str"
         )
     if "name" in params and not isinstance(params["name"], str):
         raise InvalidParameterError("Bad parameter: name must be an str")
-    if "path_time_zone" in params and not isinstance(
-        params["path_time_zone"], str
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: path_time_zone must be an str"
-        )
     if "trigger" in params and not isinstance(params["trigger"], str):
         raise InvalidParameterError("Bad parameter: trigger must be an str")
     if "trigger_actions" in params and not isinstance(
         params["trigger_actions"], builtins.list
     ):
         raise InvalidParameterError(
             "Bad parameter: trigger_actions must be an list"
@@ -474,25 +408,19 @@
 #   destination_replace_from - string - If set, this string in the destination path will be replaced with the value in `destination_replace_to`.
 #   destination_replace_to - string - If set, this string will replace the value `destination_replace_from` in the destination filename. You can use special patterns here.
 #   interval - string - How often to run this automation? One of: `day`, `week`, `week_end`, `month`, `month_end`, `quarter`, `quarter_end`, `year`, `year_end`
 #   path - string - Path on which this Automation runs.  Supports globs.
 #   sync_ids - string - A list of sync IDs the automation is associated with. If sent as a string, it should be comma-delimited.
 #   user_ids - string - A list of user IDs the automation is associated with. If sent as a string, it should be comma-delimited.
 #   group_ids - string - A list of group IDs the automation is associated with. If sent as a string, it should be comma-delimited.
-#   schedule_days_of_week - array(int64) - If trigger is `custom_schedule`. A list of days of the week to run this automation. 0 is Sunday, 1 is Monday, etc.
-#   schedule_times_of_day - array(string) - If trigger is `custom_schedule`. A list of times of day to run this automation. 24-hour time format.
-#   schedule_time_zone - string - If trigger is `custom_schedule`. Time zone for the schedule.
+#   schedule - object - Custom schedule for running this automation.
 #   always_overwrite_size_matching_files - boolean - Ordinarily, files with identical size in the source and destination will be skipped from copy operations to prevent wasted transfer.  If this flag is `true` we will overwrite the destination file always.  Note that this may cause large amounts of wasted transfer usage.
 #   description - string - Description for the this Automation.
 #   disabled - boolean - If true, this automation will not run.
-#   flatten_destination_structure - boolean - Normally copy and move automations that use globs will implicitly preserve the source folder structure in the destination.  If this flag is `true`, the source folder structure will be flattened in the destination.  This is useful for copying or moving files from multiple folders into a single destination folder.
-#   ignore_locked_folders - boolean - If true, the Lock Folders behavior will be disregarded for automated actions.
 #   name - string - Name for this automation.
-#   overwrite_files - boolean - If true, existing files will be overwritten with new files on Move/Copy automations.  Note: by default files will not be overwritten if they appear to be the same file size as the newly incoming file.  Use the `:always_overwrite_size_matching_files` option to override this.
-#   path_time_zone - string - Timezone to use when rendering timestamps in paths.
 #   trigger - string - How this automation is triggered to run.
 #   trigger_actions - array(string) - If trigger is `action`, this is the list of action types on which to trigger the automation. Valid actions are create, read, update, destroy, move, copy
 #   value - object - A Hash of attributes specific to the automation type.
 #   recurring_day - int64 - If trigger type is `daily`, this specifies a day number to run in one of the supported intervals: `week`, `month`, `quarter`, `year`.
 #   automation - string - Automation type
 def update(id, params=None, options=None):
     if not isinstance(params, dict):
@@ -532,44 +460,22 @@
         raise InvalidParameterError("Bad parameter: path must be an str")
     if "sync_ids" in params and not isinstance(params["sync_ids"], str):
         raise InvalidParameterError("Bad parameter: sync_ids must be an str")
     if "user_ids" in params and not isinstance(params["user_ids"], str):
         raise InvalidParameterError("Bad parameter: user_ids must be an str")
     if "group_ids" in params and not isinstance(params["group_ids"], str):
         raise InvalidParameterError("Bad parameter: group_ids must be an str")
-    if "schedule_days_of_week" in params and not isinstance(
-        params["schedule_days_of_week"], builtins.list
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: schedule_days_of_week must be an list"
-        )
-    if "schedule_times_of_day" in params and not isinstance(
-        params["schedule_times_of_day"], builtins.list
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: schedule_times_of_day must be an list"
-        )
-    if "schedule_time_zone" in params and not isinstance(
-        params["schedule_time_zone"], str
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: schedule_time_zone must be an str"
-        )
+    if "schedule" in params and not isinstance(params["schedule"], dict):
+        raise InvalidParameterError("Bad parameter: schedule must be an dict")
     if "description" in params and not isinstance(params["description"], str):
         raise InvalidParameterError(
             "Bad parameter: description must be an str"
         )
     if "name" in params and not isinstance(params["name"], str):
         raise InvalidParameterError("Bad parameter: name must be an str")
-    if "path_time_zone" in params and not isinstance(
-        params["path_time_zone"], str
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: path_time_zone must be an str"
-        )
     if "trigger" in params and not isinstance(params["trigger"], str):
         raise InvalidParameterError("Bad parameter: trigger must be an str")
     if "trigger_actions" in params and not isinstance(
         params["trigger_actions"], builtins.list
     ):
         raise InvalidParameterError(
             "Bad parameter: trigger_actions must be an list"
```

### Comparing `Files.com-1.4.81/files_sdk/models/automation_run.py` & `Files.com-1.4.9/files_sdk/models/automation_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,15 @@
 
 class AutomationRun:
     default_attributes = {
         "id": None,  # int64 - ID.
         "automation_id": None,  # int64 - ID of the associated Automation.
         "completed_at": None,  # date-time - Automation run completion/failure date/time.
         "created_at": None,  # date-time - Automation run start date/time.
-        "runtime": None,  # double - Automation run runtime.
         "status": None,  # string - The success status of the AutomationRun. One of `running`, `success`, `partial_failure`, or `failure`.
-        "successful_operations": None,  # int64 - Count of successful operations.
-        "failed_operations": None,  # int64 - Count of failed operations.
         "status_messages_url": None,  # string - Link to status messages log file.
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
```

### Comparing `Files.com-1.4.81/files_sdk/models/bandwidth_snapshot.py` & `Files.com-1.4.9/files_sdk/models/bandwidth_snapshot.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/behavior.py` & `Files.com-1.4.9/files_sdk/models/behavior.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,16 +13,14 @@
         "id": None,  # int64 - Folder behavior ID
         "path": None,  # string - Folder path.  Note that Behavior paths cannot be updated once initially set.  You will need to remove and re-create the behavior on the new path. This must be slash-delimited, but it must neither start nor end with a slash. Maximum of 5000 characters.
         "attachment_url": None,  # string - URL for attached file
         "behavior": None,  # string - Behavior type.
         "name": None,  # string - Name for this behavior.
         "description": None,  # string - Description for this behavior.
         "value": None,  # object - Settings for this behavior.  See the section above for an example value to provide here.  Formatting is different for each Behavior type.  May be sent as nested JSON or a single JSON-encoded string.  If using XML encoding for the API call, this data must be sent as a JSON-encoded string.
-        "disable_parent_folder_behavior": None,  # boolean - If true, the parent folder's behavior will be disabled for this folder and its children.
-        "recursive": None,  # boolean - Is behavior recursive?
         "attachment_file": None,  # file - Certain behaviors may require a file, for instance, the "watermark" behavior requires a watermark image
         "attachment_delete": None,  # boolean - If true, will delete the file stored in attachment
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
@@ -39,18 +37,16 @@
         return {
             k: getattr(self, k, None)
             for k in Behavior.default_attributes
             if getattr(self, k, None) is not None
         }
 
     # Parameters:
-    #   value - string - The value of the folder behavior.  Can be an integer, array, or hash depending on the type of folder behavior. See The Behavior Types section for example values for each type of behavior.
+    #   value - string - The value of the folder behavior.  Can be a integer, array, or hash depending on the type of folder behavior. See The Behavior Types section for example values for each type of behavior.
     #   attachment_file - file - Certain behaviors may require a file, for instance, the "watermark" behavior requires a watermark image
-    #   disable_parent_folder_behavior - boolean - If true, the parent folder's behavior will be disabled for this folder and its children.
-    #   recursive - boolean - Is behavior recursive?
     #   name - string - Name for this behavior.
     #   description - string - Description for this behavior.
     #   behavior - string - Behavior type.
     #   path - string - Folder behaviors path.
     #   attachment_delete - boolean - If true, will delete the file stored in attachment
     def update(self, params=None):
         if not isinstance(params, dict):
@@ -120,16 +116,16 @@
             self.set_attributes(new_obj.get_attributes())
             return True
 
 
 # Parameters:
 #   cursor - string - Used for pagination.  When a list request has more records available, cursors are provided in the response headers `X-Files-Cursor-Next` and `X-Files-Cursor-Prev`.  Send one of those cursor value here to resume an existing list from the next available record.  Note: many of our SDKs have iterator methods that will automatically handle cursor-based pagination.
 #   per_page - int64 - Number of records to show per page.  (Max: 10,000, 1,000 or less is recommended).
-#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[behavior]=desc`). Valid fields are `behavior` and `impacts_ui`.
-#   filter - object - If set, return records where the specified field is equal to the supplied value. Valid fields are `impacts_ui` and `behavior`.
+#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[behavior]=desc`). Valid fields are `behavior`.
+#   filter - object - If set, return records where the specified field is equal to the supplied value. Valid fields are `behavior`.
 #   filter_prefix - object - If set, return records where the specified field is prefixed by the supplied value. Valid fields are `behavior`.
 def list(params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     if "cursor" in params and not isinstance(params["cursor"], str):
@@ -174,19 +170,19 @@
 def get(id, params=None, options=None):
     find(id, params, options)
 
 
 # Parameters:
 #   cursor - string - Used for pagination.  When a list request has more records available, cursors are provided in the response headers `X-Files-Cursor-Next` and `X-Files-Cursor-Prev`.  Send one of those cursor value here to resume an existing list from the next available record.  Note: many of our SDKs have iterator methods that will automatically handle cursor-based pagination.
 #   per_page - int64 - Number of records to show per page.  (Max: 10,000, 1,000 or less is recommended).
-#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[behavior]=desc`). Valid fields are `behavior` and `impacts_ui`.
-#   filter - object - If set, return records where the specified field is equal to the supplied value. Valid fields are `impacts_ui` and `behavior`.
+#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[behavior]=desc`). Valid fields are `behavior`.
+#   filter - object - If set, return records where the specified field is equal to the supplied value. Valid fields are `behavior`.
 #   filter_prefix - object - If set, return records where the specified field is prefixed by the supplied value. Valid fields are `behavior`.
 #   path (required) - string - Path to operate on.
-#   ancestor_behaviors - string - Show behaviors above this path?
+#   recursive - string - Show behaviors above this path?
 #   behavior - string - DEPRECATED: If set only shows folder behaviors matching this behavior type. Use `filter[behavior]` instead.
 def list_for(path, params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     params["path"] = path
@@ -202,38 +198,32 @@
         params["filter_prefix"], dict
     ):
         raise InvalidParameterError(
             "Bad parameter: filter_prefix must be an dict"
         )
     if "path" in params and not isinstance(params["path"], str):
         raise InvalidParameterError("Bad parameter: path must be an str")
-    if "ancestor_behaviors" in params and not isinstance(
-        params["ancestor_behaviors"], str
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: ancestor_behaviors must be an str"
-        )
+    if "recursive" in params and not isinstance(params["recursive"], str):
+        raise InvalidParameterError("Bad parameter: recursive must be an str")
     if "behavior" in params and not isinstance(params["behavior"], str):
         raise InvalidParameterError("Bad parameter: behavior must be an str")
     if "path" not in params:
         raise MissingParameterError("Parameter missing: path")
     return ListObj(
         Behavior,
         "GET",
         "/behaviors/folders/{path}".format(path=params["path"]),
         params,
         options,
     )
 
 
 # Parameters:
-#   value - string - The value of the folder behavior.  Can be an integer, array, or hash depending on the type of folder behavior. See The Behavior Types section for example values for each type of behavior.
+#   value - string - The value of the folder behavior.  Can be a integer, array, or hash depending on the type of folder behavior. See The Behavior Types section for example values for each type of behavior.
 #   attachment_file - file - Certain behaviors may require a file, for instance, the "watermark" behavior requires a watermark image
-#   disable_parent_folder_behavior - boolean - If true, the parent folder's behavior will be disabled for this folder and its children.
-#   recursive - boolean - Is behavior recursive?
 #   name - string - Name for this behavior.
 #   description - string - Description for this behavior.
 #   path (required) - string - Folder behaviors path.
 #   behavior (required) - string - Behavior type.
 def create(params=None, options=None):
     if not isinstance(params, dict):
         params = {}
@@ -285,18 +275,16 @@
         raise InvalidParameterError("Bad parameter: action must be an str")
     if "url" not in params:
         raise MissingParameterError("Parameter missing: url")
     Api.send_request("POST", "/behaviors/webhook/test", params, options)
 
 
 # Parameters:
-#   value - string - The value of the folder behavior.  Can be an integer, array, or hash depending on the type of folder behavior. See The Behavior Types section for example values for each type of behavior.
+#   value - string - The value of the folder behavior.  Can be a integer, array, or hash depending on the type of folder behavior. See The Behavior Types section for example values for each type of behavior.
 #   attachment_file - file - Certain behaviors may require a file, for instance, the "watermark" behavior requires a watermark image
-#   disable_parent_folder_behavior - boolean - If true, the parent folder's behavior will be disabled for this folder and its children.
-#   recursive - boolean - Is behavior recursive?
 #   name - string - Name for this behavior.
 #   description - string - Description for this behavior.
 #   behavior - string - Behavior type.
 #   path - string - Folder behaviors path.
 #   attachment_delete - boolean - If true, will delete the file stored in attachment
 def update(id, params=None, options=None):
     if not isinstance(params, dict):
```

### Comparing `Files.com-1.4.81/files_sdk/models/bundle.py` & `Files.com-1.4.9/files_sdk/models/bundle.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,27 +32,25 @@
         "start_access_on_date": None,  # date-time - Date when share will start to be accessible. If `nil` access granted right after create.
         "skip_company": None,  # boolean - BundleRegistrations can be saved without providing company?
         "id": None,  # int64 - Bundle ID
         "created_at": None,  # date-time - Bundle created at date/time
         "dont_separate_submissions_by_folder": None,  # boolean - Do not create subfolders for files uploaded to this share. Note: there are subtle security pitfalls with allowing anonymous uploads from multiple users to live in the same folder. We strongly discourage use of this option unless absolutely required.
         "max_uses": None,  # int64 - Maximum number of times bundle can be accessed
         "note": None,  # string - Bundle internal note
-        "path_template": None,  # string - Template for creating submission subfolders. Can use the uploader's name, email address, ip, company, `strftime` directives, and any custom form data.
-        "path_template_time_zone": None,  # string - Timezone to use when rendering timestamps in path templates.
+        "path_template": None,  # string - Template for creating submission subfolders. Can use the uploader's name, email address, ip, company, and any custom form data.
         "send_email_receipt_to_uploader": None,  # boolean - Send delivery receipt to the uploader. Note: For writable share only
         "snapshot_id": None,  # int64 - ID of the snapshot containing this bundle's contents.
         "user_id": None,  # int64 - Bundle creator user ID
         "username": None,  # string - Bundle creator username
         "clickwrap_id": None,  # int64 - ID of the clickwrap to use with this bundle.
         "inbox_id": None,  # int64 - ID of the associated inbox, if available.
         "watermark_attachment": None,  # Image - Preview watermark image applied to all bundle items.
         "watermark_value": None,  # object - Preview watermark settings applied to all bundle items. Uses the same keys as Behavior.value
         "has_inbox": None,  # boolean - Does this bundle have an associated inbox?
         "paths": None,  # array - A list of paths in this bundle.  For performance reasons, this is not provided when listing bundles.
-        "bundlepaths": None,  # array - A list of bundlepaths in this bundle.  For performance reasons, this is not provided when listing bundles.
         "password": None,  # string - Password for this bundle.
         "form_field_set_id": None,  # int64 - Id of Form Field Set to use with this bundle
         "create_snapshot": None,  # boolean - If true, create a snapshot of this bundle's contents.
         "finalize_snapshot": None,  # boolean - If true, finalize the snapshot of this bundle's contents. Note that `create_snapshot` must also be true.
         "watermark_attachment_file": None,  # file - Preview watermark image applied to all bundle items.
         "watermark_attachment_delete": None,  # boolean - If true, will delete the file stored in watermark_attachment
     }
@@ -121,16 +119,15 @@
     #   description - string - Public description
     #   dont_separate_submissions_by_folder - boolean - Do not create subfolders for files uploaded to this share. Note: there are subtle security pitfalls with allowing anonymous uploads from multiple users to live in the same folder. We strongly discourage use of this option unless absolutely required.
     #   expires_at - string - Bundle expiration date/time
     #   finalize_snapshot - boolean - If true, finalize the snapshot of this bundle's contents. Note that `create_snapshot` must also be true.
     #   inbox_id - int64 - ID of the associated inbox, if available.
     #   max_uses - int64 - Maximum number of times bundle can be accessed
     #   note - string - Bundle internal note
-    #   path_template - string - Template for creating submission subfolders. Can use the uploader's name, email address, ip, company, `strftime` directives, and any custom form data.
-    #   path_template_time_zone - string - Timezone to use when rendering timestamps in path templates.
+    #   path_template - string - Template for creating submission subfolders. Can use the uploader's name, email address, ip, company, and any custom form data.
     #   permissions - string - Permissions that apply to Folders in this Share Link.
     #   preview_only - boolean - DEPRECATED: Restrict users to previewing files only. Use `permissions` instead.
     #   require_registration - boolean - Show a registration page that captures the downloader's name and email address?
     #   require_share_recipient - boolean - Only allow access to recipients who have explicitly received the share via an email sent through the Files.com UI?
     #   send_email_receipt_to_uploader - boolean - Send delivery receipt to the uploader. Note: For writable share only
     #   skip_company - boolean - BundleRegistrations can be saved without providing company?
     #   start_access_on_date - string - Date when share will start to be accessible. If `nil` access granted right after create.
@@ -196,20 +193,14 @@
             raise InvalidParameterError("Bad parameter: note must be an str")
         if "path_template" in params and not isinstance(
             params["path_template"], str
         ):
             raise InvalidParameterError(
                 "Bad parameter: path_template must be an str"
             )
-        if "path_template_time_zone" in params and not isinstance(
-            params["path_template_time_zone"], str
-        ):
-            raise InvalidParameterError(
-                "Bad parameter: path_template_time_zone must be an str"
-            )
         if "permissions" in params and not isinstance(
             params["permissions"], str
         ):
             raise InvalidParameterError(
                 "Bad parameter: permissions must be an str"
             )
         if "start_access_on_date" in params and not isinstance(
@@ -334,16 +325,15 @@
 #   dont_separate_submissions_by_folder - boolean - Do not create subfolders for files uploaded to this share. Note: there are subtle security pitfalls with allowing anonymous uploads from multiple users to live in the same folder. We strongly discourage use of this option unless absolutely required.
 #   expires_at - string - Bundle expiration date/time
 #   finalize_snapshot - boolean - If true, finalize the snapshot of this bundle's contents. Note that `create_snapshot` must also be true.
 #   max_uses - int64 - Maximum number of times bundle can be accessed
 #   description - string - Public description
 #   note - string - Bundle internal note
 #   code - string - Bundle code.  This code forms the end part of the Public URL.
-#   path_template - string - Template for creating submission subfolders. Can use the uploader's name, email address, ip, company, `strftime` directives, and any custom form data.
-#   path_template_time_zone - string - Timezone to use when rendering timestamps in path templates.
+#   path_template - string - Template for creating submission subfolders. Can use the uploader's name, email address, ip, company, and any custom form data.
 #   permissions - string - Permissions that apply to Folders in this Share Link.
 #   preview_only - boolean - DEPRECATED: Restrict users to previewing files only. Use `permissions` instead.
 #   require_registration - boolean - Show a registration page that captures the downloader's name and email address?
 #   clickwrap_id - int64 - ID of the clickwrap to use with this bundle.
 #   inbox_id - int64 - ID of the associated inbox, if available.
 #   require_share_recipient - boolean - Only allow access to recipients who have explicitly received the share via an email sent through the Files.com UI?
 #   send_email_receipt_to_uploader - boolean - Send delivery receipt to the uploader. Note: For writable share only
@@ -384,20 +374,14 @@
         raise InvalidParameterError("Bad parameter: code must be an str")
     if "path_template" in params and not isinstance(
         params["path_template"], str
     ):
         raise InvalidParameterError(
             "Bad parameter: path_template must be an str"
         )
-    if "path_template_time_zone" in params and not isinstance(
-        params["path_template_time_zone"], str
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: path_template_time_zone must be an str"
-        )
     if "permissions" in params and not isinstance(params["permissions"], str):
         raise InvalidParameterError(
             "Bad parameter: permissions must be an str"
         )
     if "clickwrap_id" in params and not isinstance(
         params["clickwrap_id"], int
     ):
@@ -463,16 +447,15 @@
 #   description - string - Public description
 #   dont_separate_submissions_by_folder - boolean - Do not create subfolders for files uploaded to this share. Note: there are subtle security pitfalls with allowing anonymous uploads from multiple users to live in the same folder. We strongly discourage use of this option unless absolutely required.
 #   expires_at - string - Bundle expiration date/time
 #   finalize_snapshot - boolean - If true, finalize the snapshot of this bundle's contents. Note that `create_snapshot` must also be true.
 #   inbox_id - int64 - ID of the associated inbox, if available.
 #   max_uses - int64 - Maximum number of times bundle can be accessed
 #   note - string - Bundle internal note
-#   path_template - string - Template for creating submission subfolders. Can use the uploader's name, email address, ip, company, `strftime` directives, and any custom form data.
-#   path_template_time_zone - string - Timezone to use when rendering timestamps in path templates.
+#   path_template - string - Template for creating submission subfolders. Can use the uploader's name, email address, ip, company, and any custom form data.
 #   permissions - string - Permissions that apply to Folders in this Share Link.
 #   preview_only - boolean - DEPRECATED: Restrict users to previewing files only. Use `permissions` instead.
 #   require_registration - boolean - Show a registration page that captures the downloader's name and email address?
 #   require_share_recipient - boolean - Only allow access to recipients who have explicitly received the share via an email sent through the Files.com UI?
 #   send_email_receipt_to_uploader - boolean - Send delivery receipt to the uploader. Note: For writable share only
 #   skip_company - boolean - BundleRegistrations can be saved without providing company?
 #   start_access_on_date - string - Date when share will start to be accessible. If `nil` access granted right after create.
@@ -520,20 +503,14 @@
         raise InvalidParameterError("Bad parameter: note must be an str")
     if "path_template" in params and not isinstance(
         params["path_template"], str
     ):
         raise InvalidParameterError(
             "Bad parameter: path_template must be an str"
         )
-    if "path_template_time_zone" in params and not isinstance(
-        params["path_template_time_zone"], str
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: path_template_time_zone must be an str"
-        )
     if "permissions" in params and not isinstance(params["permissions"], str):
         raise InvalidParameterError(
             "Bad parameter: permissions must be an str"
         )
     if "start_access_on_date" in params and not isinstance(
         params["start_access_on_date"], str
     ):
```

### Comparing `Files.com-1.4.81/files_sdk/models/bundle_action.py` & `Files.com-1.4.9/files_sdk/models/bundle_download.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,51 +4,49 @@
 from files_sdk.error import (  # noqa: F401
     InvalidParameterError,
     MissingParameterError,
     NotImplementedError,
 )
 
 
-class BundleAction:
+class BundleDownload:
     default_attributes = {
-        "action": None,  # string - Type of action
-        "bundle_registration": None,  # BundleRegistration - Object that contains bundle registration information
-        "when": None,  # date-time - Action occurrence date/time
-        "destination": None,  # string - The destination path for this bundle action, if applicable
-        "path": None,  # string - Path This must be slash-delimited, but it must neither start nor end with a slash. Maximum of 5000 characters.
-        "source": None,  # string - The source path for this bundle action, if applicable
+        "bundle_registration": None,  # BundleRegistration
+        "download_method": None,  # string - Download method (file or full_zip)
+        "path": None,  # string - Download path This must be slash-delimited, but it must neither start nor end with a slash. Maximum of 5000 characters.
+        "created_at": None,  # date-time - Download date/time
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
             options = {}
         self.set_attributes(attributes)
         self.options = options
 
     def set_attributes(self, attributes):
         for (
             attribute,
             default_value,
-        ) in BundleAction.default_attributes.items():
+        ) in BundleDownload.default_attributes.items():
             setattr(self, attribute, attributes.get(attribute, default_value))
 
     def get_attributes(self):
         return {
             k: getattr(self, k, None)
-            for k in BundleAction.default_attributes
+            for k in BundleDownload.default_attributes
             if getattr(self, k, None) is not None
         }
 
 
 # Parameters:
 #   cursor - string - Used for pagination.  When a list request has more records available, cursors are provided in the response headers `X-Files-Cursor-Next` and `X-Files-Cursor-Prev`.  Send one of those cursor value here to resume an existing list from the next available record.  Note: many of our SDKs have iterator methods that will automatically handle cursor-based pagination.
 #   per_page - int64 - Number of records to show per page.  (Max: 10,000, 1,000 or less is recommended).
-#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[bundle_registration_id]=desc`). Valid fields are `bundle_registration_id` and `created_at`.
+#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[created_at]=desc`). Valid fields are `created_at`.
 #   filter - object - If set, return records where the specified field is equal to the supplied value. Valid fields are `created_at`.
 #   filter_gt - object - If set, return records where the specified field is greater than the supplied value. Valid fields are `created_at`.
 #   filter_gteq - object - If set, return records where the specified field is greater than or equal the supplied value. Valid fields are `created_at`.
 #   filter_lt - object - If set, return records where the specified field is less than the supplied value. Valid fields are `created_at`.
 #   filter_lteq - object - If set, return records where the specified field is less than or equal the supplied value. Valid fields are `created_at`.
 #   bundle_id - int64 - Bundle ID
 #   bundle_registration_id - int64 - BundleRegistration ID
@@ -81,16 +79,16 @@
         raise InvalidParameterError("Bad parameter: bundle_id must be an int")
     if "bundle_registration_id" in params and not isinstance(
         params["bundle_registration_id"], int
     ):
         raise InvalidParameterError(
             "Bad parameter: bundle_registration_id must be an int"
         )
-    return ListObj(BundleAction, "GET", "/bundle_actions", params, options)
+    return ListObj(BundleDownload, "GET", "/bundle_downloads", params, options)
 
 
 def all(params=None, options=None):
     list(params, options)
 
 
 def new(*args, **kwargs):
-    return BundleAction(*args, **kwargs)
+    return BundleDownload(*args, **kwargs)
```

### Comparing `Files.com-1.4.81/files_sdk/models/bundle_download.py` & `Files.com-1.4.9/files_sdk/models/email_incoming_message.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,56 +4,60 @@
 from files_sdk.error import (  # noqa: F401
     InvalidParameterError,
     MissingParameterError,
     NotImplementedError,
 )
 
 
-class BundleDownload:
+class EmailIncomingMessage:
     default_attributes = {
-        "bundle_registration": None,  # BundleRegistration
-        "download_method": None,  # string - Download method (file or full_zip)
-        "path": None,  # string - Download path This must be slash-delimited, but it must neither start nor end with a slash. Maximum of 5000 characters.
-        "created_at": None,  # date-time - Download date/time
+        "id": None,  # int64 - Id of the Email Incoming Message
+        "inbox_id": None,  # int64 - Id of the Inbox associated with this message
+        "sender": None,  # string - Sender of the email
+        "sender_name": None,  # string - Sender name
+        "status": None,  # string - Status of the message
+        "body": None,  # string - Body of the email
+        "message": None,  # string - Message describing the failure
+        "created_at": None,  # date-time - Message creation date/time
+        "inbox_title": None,  # string - Title of the Inbox associated with this message
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
             options = {}
         self.set_attributes(attributes)
         self.options = options
 
     def set_attributes(self, attributes):
         for (
             attribute,
             default_value,
-        ) in BundleDownload.default_attributes.items():
+        ) in EmailIncomingMessage.default_attributes.items():
             setattr(self, attribute, attributes.get(attribute, default_value))
 
     def get_attributes(self):
         return {
             k: getattr(self, k, None)
-            for k in BundleDownload.default_attributes
+            for k in EmailIncomingMessage.default_attributes
             if getattr(self, k, None) is not None
         }
 
 
 # Parameters:
 #   cursor - string - Used for pagination.  When a list request has more records available, cursors are provided in the response headers `X-Files-Cursor-Next` and `X-Files-Cursor-Prev`.  Send one of those cursor value here to resume an existing list from the next available record.  Note: many of our SDKs have iterator methods that will automatically handle cursor-based pagination.
 #   per_page - int64 - Number of records to show per page.  (Max: 10,000, 1,000 or less is recommended).
-#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[created_at]=desc`). Valid fields are `created_at`.
-#   filter - object - If set, return records where the specified field is equal to the supplied value. Valid fields are `created_at`.
+#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[created_at]=desc`). Valid fields are `created_at`, `sender`, `status` or `inbox_id`.
+#   filter - object - If set, return records where the specified field is equal to the supplied value. Valid fields are `created_at`, `inbox_id`, `sender` or `status`. Valid field combinations are `[ sender, created_at ]`, `[ status, created_at ]`, `[ inbox_id, created_at ]`, `[ inbox_id, status, created_at ]` or `[ inbox_id, status, sender, created_at ]`.
 #   filter_gt - object - If set, return records where the specified field is greater than the supplied value. Valid fields are `created_at`.
 #   filter_gteq - object - If set, return records where the specified field is greater than or equal the supplied value. Valid fields are `created_at`.
+#   filter_prefix - object - If set, return records where the specified field is prefixed by the supplied value. Valid fields are `sender`.
 #   filter_lt - object - If set, return records where the specified field is less than the supplied value. Valid fields are `created_at`.
 #   filter_lteq - object - If set, return records where the specified field is less than or equal the supplied value. Valid fields are `created_at`.
-#   bundle_id - int64 - Bundle ID
-#   bundle_registration_id - int64 - BundleRegistration ID
 def list(params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     if "cursor" in params and not isinstance(params["cursor"], str):
         raise InvalidParameterError("Bad parameter: cursor must be an str")
@@ -65,30 +69,34 @@
         raise InvalidParameterError("Bad parameter: filter must be an dict")
     if "filter_gt" in params and not isinstance(params["filter_gt"], dict):
         raise InvalidParameterError("Bad parameter: filter_gt must be an dict")
     if "filter_gteq" in params and not isinstance(params["filter_gteq"], dict):
         raise InvalidParameterError(
             "Bad parameter: filter_gteq must be an dict"
         )
+    if "filter_prefix" in params and not isinstance(
+        params["filter_prefix"], dict
+    ):
+        raise InvalidParameterError(
+            "Bad parameter: filter_prefix must be an dict"
+        )
     if "filter_lt" in params and not isinstance(params["filter_lt"], dict):
         raise InvalidParameterError("Bad parameter: filter_lt must be an dict")
     if "filter_lteq" in params and not isinstance(params["filter_lteq"], dict):
         raise InvalidParameterError(
             "Bad parameter: filter_lteq must be an dict"
         )
-    if "bundle_id" in params and not isinstance(params["bundle_id"], int):
-        raise InvalidParameterError("Bad parameter: bundle_id must be an int")
-    if "bundle_registration_id" in params and not isinstance(
-        params["bundle_registration_id"], int
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: bundle_registration_id must be an int"
-        )
-    return ListObj(BundleDownload, "GET", "/bundle_downloads", params, options)
+    return ListObj(
+        EmailIncomingMessage,
+        "GET",
+        "/email_incoming_messages",
+        params,
+        options,
+    )
 
 
 def all(params=None, options=None):
     list(params, options)
 
 
 def new(*args, **kwargs):
-    return BundleDownload(*args, **kwargs)
+    return EmailIncomingMessage(*args, **kwargs)
```

### Comparing `Files.com-1.4.81/files_sdk/models/bundle_notification.py` & `Files.com-1.4.9/files_sdk/models/bundle_notification.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -144,18 +144,18 @@
 
 
 def get(id, params=None, options=None):
     find(id, params, options)
 
 
 # Parameters:
-#   bundle_id (required) - int64 - Bundle ID to notify on
-#   user_id - int64 - The id of the user to notify.
 #   notify_on_registration - boolean - Triggers bundle notification when a registration action occurs for it.
 #   notify_on_upload - boolean - Triggers bundle notification when a upload action occurs for it.
+#   bundle_id (required) - int64 - Bundle ID to notify on
+#   user_id - int64 - The id of the user to notify.
 def create(params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     if "bundle_id" in params and not isinstance(params["bundle_id"], int):
         raise InvalidParameterError("Bad parameter: bundle_id must be an int")
```

### Comparing `Files.com-1.4.81/files_sdk/models/bundle_path.py` & `Files.com-1.4.9/files_sdk/models/form_field.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,35 +3,41 @@
 from files_sdk.error import (  # noqa: F401
     InvalidParameterError,
     MissingParameterError,
     NotImplementedError,
 )
 
 
-class BundlePath:
+class FormField:
     default_attributes = {
-        "recursive": None,  # boolean - Allow access to subfolders content?
-        "path": None,  # string - The path to the resource relative to filesystem. This must be slash-delimited, but it must neither start nor end with a slash. Maximum of 5000 characters.
+        "id": None,  # int64 - Form field id
+        "label": None,  # string - Label to be displayed
+        "required": None,  # boolean - Is this a required field?
+        "help_text": None,  # string - Help text to be displayed
+        "field_type": None,  # string - Type of Field
+        "options_for_select": None,  # array - Options to display for radio and dropdown
+        "default_option": None,  # string - Default option for radio and dropdown
+        "form_field_set_id": None,  # int64 - Form field set id
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
             options = {}
         self.set_attributes(attributes)
         self.options = options
 
     def set_attributes(self, attributes):
-        for attribute, default_value in BundlePath.default_attributes.items():
+        for attribute, default_value in FormField.default_attributes.items():
             setattr(self, attribute, attributes.get(attribute, default_value))
 
     def get_attributes(self):
         return {
             k: getattr(self, k, None)
-            for k in BundlePath.default_attributes
+            for k in FormField.default_attributes
             if getattr(self, k, None) is not None
         }
 
 
 def new(*args, **kwargs):
-    return BundlePath(*args, **kwargs)
+    return FormField(*args, **kwargs)
```

### Comparing `Files.com-1.4.81/files_sdk/models/bundle_recipient.py` & `Files.com-1.4.9/files_sdk/models/bundle_recipient.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/bundle_registration.py` & `Files.com-1.4.9/files_sdk/models/bundle_registration.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/clickwrap.py` & `Files.com-1.4.9/files_sdk/models/clickwrap.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/dns_record.py` & `Files.com-1.4.9/files_sdk/models/dns_record.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/email_incoming_message.py` & `Files.com-1.4.9/files_sdk/models/inbox_upload.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,60 +4,52 @@
 from files_sdk.error import (  # noqa: F401
     InvalidParameterError,
     MissingParameterError,
     NotImplementedError,
 )
 
 
-class EmailIncomingMessage:
+class InboxUpload:
     default_attributes = {
-        "id": None,  # int64 - Id of the Email Incoming Message
-        "inbox_id": None,  # int64 - Id of the Inbox associated with this message
-        "sender": None,  # string - Sender of the email
-        "sender_name": None,  # string - Sender name
-        "status": None,  # string - Status of the message
-        "body": None,  # string - Body of the email
-        "message": None,  # string - Message describing the failure
-        "created_at": None,  # date-time - Message creation date/time
-        "inbox_title": None,  # string - Title of the Inbox associated with this message
+        "inbox_registration": None,  # InboxRegistration
+        "path": None,  # string - Upload path This must be slash-delimited, but it must neither start nor end with a slash. Maximum of 5000 characters.
+        "created_at": None,  # date-time - Upload date/time
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
             options = {}
         self.set_attributes(attributes)
         self.options = options
 
     def set_attributes(self, attributes):
-        for (
-            attribute,
-            default_value,
-        ) in EmailIncomingMessage.default_attributes.items():
+        for attribute, default_value in InboxUpload.default_attributes.items():
             setattr(self, attribute, attributes.get(attribute, default_value))
 
     def get_attributes(self):
         return {
             k: getattr(self, k, None)
-            for k in EmailIncomingMessage.default_attributes
+            for k in InboxUpload.default_attributes
             if getattr(self, k, None) is not None
         }
 
 
 # Parameters:
 #   cursor - string - Used for pagination.  When a list request has more records available, cursors are provided in the response headers `X-Files-Cursor-Next` and `X-Files-Cursor-Prev`.  Send one of those cursor value here to resume an existing list from the next available record.  Note: many of our SDKs have iterator methods that will automatically handle cursor-based pagination.
 #   per_page - int64 - Number of records to show per page.  (Max: 10,000, 1,000 or less is recommended).
-#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[created_at]=desc`). Valid fields are `created_at`, `sender`, `status` or `inbox_id`.
-#   filter - object - If set, return records where the specified field is equal to the supplied value. Valid fields are `created_at`, `inbox_id`, `sender` or `status`. Valid field combinations are `[ sender, created_at ]`, `[ status, created_at ]`, `[ inbox_id, created_at ]`, `[ inbox_id, status, created_at ]` or `[ inbox_id, status, sender, created_at ]`.
+#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[created_at]=desc`). Valid fields are `created_at`.
+#   filter - object - If set, return records where the specified field is equal to the supplied value. Valid fields are `created_at`.
 #   filter_gt - object - If set, return records where the specified field is greater than the supplied value. Valid fields are `created_at`.
 #   filter_gteq - object - If set, return records where the specified field is greater than or equal the supplied value. Valid fields are `created_at`.
-#   filter_prefix - object - If set, return records where the specified field is prefixed by the supplied value. Valid fields are `sender`.
 #   filter_lt - object - If set, return records where the specified field is less than the supplied value. Valid fields are `created_at`.
 #   filter_lteq - object - If set, return records where the specified field is less than or equal the supplied value. Valid fields are `created_at`.
+#   inbox_registration_id - int64 - InboxRegistration ID
+#   inbox_id - int64 - Inbox ID
 def list(params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     if "cursor" in params and not isinstance(params["cursor"], str):
         raise InvalidParameterError("Bad parameter: cursor must be an str")
@@ -69,34 +61,30 @@
         raise InvalidParameterError("Bad parameter: filter must be an dict")
     if "filter_gt" in params and not isinstance(params["filter_gt"], dict):
         raise InvalidParameterError("Bad parameter: filter_gt must be an dict")
     if "filter_gteq" in params and not isinstance(params["filter_gteq"], dict):
         raise InvalidParameterError(
             "Bad parameter: filter_gteq must be an dict"
         )
-    if "filter_prefix" in params and not isinstance(
-        params["filter_prefix"], dict
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: filter_prefix must be an dict"
-        )
     if "filter_lt" in params and not isinstance(params["filter_lt"], dict):
         raise InvalidParameterError("Bad parameter: filter_lt must be an dict")
     if "filter_lteq" in params and not isinstance(params["filter_lteq"], dict):
         raise InvalidParameterError(
             "Bad parameter: filter_lteq must be an dict"
         )
-    return ListObj(
-        EmailIncomingMessage,
-        "GET",
-        "/email_incoming_messages",
-        params,
-        options,
-    )
+    if "inbox_registration_id" in params and not isinstance(
+        params["inbox_registration_id"], int
+    ):
+        raise InvalidParameterError(
+            "Bad parameter: inbox_registration_id must be an int"
+        )
+    if "inbox_id" in params and not isinstance(params["inbox_id"], int):
+        raise InvalidParameterError("Bad parameter: inbox_id must be an int")
+    return ListObj(InboxUpload, "GET", "/inbox_uploads", params, options)
 
 
 def all(params=None, options=None):
     list(params, options)
 
 
 def new(*args, **kwargs):
-    return EmailIncomingMessage(*args, **kwargs)
+    return InboxUpload(*args, **kwargs)
```

### Comparing `Files.com-1.4.81/files_sdk/models/errors.py` & `Files.com-1.4.9/files_sdk/models/errors.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/external_event.py` & `Files.com-1.4.9/files_sdk/models/external_event.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,14 @@
         "body": None,  # string - Event body
         "created_at": None,  # date-time - External event create date/time
         "body_url": None,  # string - Link to log file.
         "folder_behavior_id": None,  # int64 - Folder Behavior ID
         "successful_files": None,  # int64 - For sync events, the number of files handled successfully.
         "errored_files": None,  # int64 - For sync events, the number of files that encountered errors.
         "bytes_synced": None,  # int64 - For sync events, the total number of bytes synced.
-        "compared_files": None,  # int64 - For sync events, the number of files considered for the sync.
-        "compared_folders": None,  # int64 - For sync events, the number of folders listed and considered for the sync.
         "remote_server_type": None,  # string - Associated Remote Server type, if any
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
```

### Comparing `Files.com-1.4.81/files_sdk/models/file.py` & `Files.com-1.4.9/files_sdk/models/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,33 +12,18 @@
     NotImplementedError,
 )
 
 
 class File:
     default_attributes = {
         "path": None,  # string - File/Folder path This must be slash-delimited, but it must neither start nor end with a slash. Maximum of 5000 characters.
-        "created_by_id": None,  # int64 - User ID of the User who created the file/folder
-        "created_by_api_key_id": None,  # int64 - ID of the API key that created the file/folder
-        "created_by_as2_incoming_message_id": None,  # int64 - ID of the AS2 Incoming Message that created the file/folder
-        "created_by_automation_id": None,  # int64 - ID of the Automation that created the file/folder
-        "created_by_bundle_registration_id": None,  # int64 - ID of the Bundle Registration that created the file/folder
-        "created_by_inbox_id": None,  # int64 - ID of the Inbox that created the file/folder
-        "created_by_remote_server_id": None,  # int64 - ID of the Remote Server that created the file/folder
-        "created_by_remote_server_sync_id": None,  # int64 - ID of the Remote Server Sync that created the file/folder
-        "custom_metadata": None,  # object - Custom metadata map of keys and values. Limited to 32 keys, 256 characters per key and 1024 characters per value.
         "display_name": None,  # string - File/Folder display name
         "type": None,  # string - Type: `directory` or `file`.
         "size": None,  # int64 - File/Folder size
         "created_at": None,  # date-time - File created date/time
-        "last_modified_by_id": None,  # int64 - User ID of the User who last modified the file/folder
-        "last_modified_by_api_key_id": None,  # int64 - ID of the API key that last modified the file/folder
-        "last_modified_by_automation_id": None,  # int64 - ID of the Automation that last modified the file/folder
-        "last_modified_by_bundle_registration_id": None,  # int64 - ID of the Bundle Registration that last modified the file/folder
-        "last_modified_by_remote_server_id": None,  # int64 - ID of the Remote Server that last modified the file/folder
-        "last_modified_by_remote_server_sync_id": None,  # int64 - ID of the Remote Server Sync that last modified the file/folder
         "mtime": None,  # date-time - File last modified date/time, according to the server.  This is the timestamp of the last Files.com operation of the file, regardless of what modified timestamp was sent.
         "provided_mtime": None,  # date-time - File last modified date/time, according to the client who set it.  Files.com allows desktop, FTP, SFTP, and WebDAV clients to set modified at times.  This allows Desktop<->Cloud syncing to preserve modified at times.
         "crc32": None,  # string - File CRC32 checksum. This is sometimes delayed, so if you get a blank response, wait and try again.
         "md5": None,  # string - File MD5 checksum. This is sometimes delayed, so if you get a blank response, wait and try again.
         "mime_type": None,  # string - MIME Type.  This is determined by the filename extension and is not stored separately internally.
         "region": None,  # string - Region location
         "permissions": None,  # string - A short string representing the current user's permissions.  Can be `r` (Read),`w` (Write),`d` (Delete), `l` (List) or any combination
@@ -239,15 +224,14 @@
             "/files/{path}".format(path=params["path"]),
             params,
             self.options,
         )
         return response.data
 
     # Parameters:
-    #   custom_metadata - object - Custom metadata map of keys and values. Limited to 32 keys, 256 characters per key and 1024 characters per value.
     #   provided_mtime - string - Modified time of file.
     #   priority_color - string - Priority/Bookmark color of file.
     def update(self, params=None):
         if not isinstance(params, dict):
             params = {}
 
         if hasattr(self, "path") and self.path:
@@ -303,15 +287,14 @@
         self.delete(params)
 
     # Copy file/folder
     #
     # Parameters:
     #   destination (required) - string - Copy destination path.
     #   structure - boolean - Copy structure only?
-    #   overwrite - boolean - Overwrite existing file(s) in the destination?
     def copy(self, params=None):
         if not isinstance(params, dict):
             params = {}
 
         if hasattr(self, "path") and self.path:
             params["path"] = self.path
         else:
@@ -336,15 +319,14 @@
         )
         return response.data
 
     # Move file/folder
     #
     # Parameters:
     #   destination (required) - string - Move destination path.
-    #   overwrite - boolean - Overwrite existing file(s) in the destination?
     def move(self, params=None):
         if not isinstance(params, dict):
             params = {}
 
         if hasattr(self, "path") and self.path:
             params["path"] = self.path
         else:
@@ -498,31 +480,24 @@
     response, options = Api.send_request(
         "POST", "/files/{path}".format(path=params["path"]), params, options
     )
     return File(response.data, options)
 
 
 # Parameters:
-#   custom_metadata - object - Custom metadata map of keys and values. Limited to 32 keys, 256 characters per key and 1024 characters per value.
 #   provided_mtime - string - Modified time of file.
 #   priority_color - string - Priority/Bookmark color of file.
 def update(path, params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     params["path"] = path
     if "path" in params and not isinstance(params["path"], str):
         raise InvalidParameterError("Bad parameter: path must be an str")
-    if "custom_metadata" in params and not isinstance(
-        params["custom_metadata"], dict
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: custom_metadata must be an dict"
-        )
     if "provided_mtime" in params and not isinstance(
         params["provided_mtime"], str
     ):
         raise InvalidParameterError(
             "Bad parameter: provided_mtime must be an str"
         )
     if "priority_color" in params and not isinstance(
@@ -595,15 +570,14 @@
 
 
 # Copy file/folder
 #
 # Parameters:
 #   destination (required) - string - Copy destination path.
 #   structure - boolean - Copy structure only?
-#   overwrite - boolean - Overwrite existing file(s) in the destination?
 def copy(path, params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     params["path"] = path
     if "path" in params and not isinstance(params["path"], str):
@@ -625,15 +599,14 @@
     return FileAction(response.data, options)
 
 
 # Move file/folder
 #
 # Parameters:
 #   destination (required) - string - Move destination path.
-#   overwrite - boolean - Overwrite existing file(s) in the destination?
 def move(path, params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     params["path"] = path
     if "path" in params and not isinstance(params["path"], str):
@@ -727,14 +700,18 @@
             {"part": 1}
             if not upload
             else {"ref": upload.ref, "part": upload.part_number + 1}
         )
         params.update(chunk_params)
         upload = begin_upload(path, params, options)[0]
         buf = io.read(upload.partsize)
+        if (
+            buf == b"" or buf == ""
+        ):  # Empty bytearray means EOF for BytesIO, Empty String means EOF for StringIO
+            return (upload, etags, bytes_written)
         if buf is not None:  # None means no data but io still open
             bytes_written += len(buf)
             response = Api.api_client().send_remote_request(
                 upload.http_method,
                 upload.upload_uri,
                 {"Content-Length": str(len(buf))},
                 buf,
@@ -742,18 +719,14 @@
             if "ETag" in response.headers:
                 etags.append(
                     {
                         "etag": response.headers["ETag"].strip('"'),
                         "part": upload.part_number,
                     }
                 )
-        if buf in [b"", ""] or (
-            len(buf) < upload.partsize
-        ):  # Empty bytearray means EOF for BytesIO, Empty String means EOF for StringIO
-            return (upload, etags, bytes_written)
 
 
 def upload_file(path, destination=None, options=None, params=None):
     if not isinstance(options, dict):
         options = {}
     pth = Path(path)
     stat = pth.stat()
```

### Comparing `Files.com-1.4.81/files_sdk/models/file_action.py` & `Files.com-1.4.9/files_sdk/models/file_action.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/file_comment.py` & `Files.com-1.4.9/files_sdk/models/file_comment.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/file_comment_reaction.py` & `Files.com-1.4.9/files_sdk/models/file_comment_reaction.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/file_migration.py` & `Files.com-1.4.9/files_sdk/models/file_migration.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/file_upload_part.py` & `Files.com-1.4.9/files_sdk/models/file_upload_part.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/folder.py` & `Files.com-1.4.9/files_sdk/models/sso_strategy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,148 +1,161 @@
 import builtins  # noqa: F401
-from files_sdk.models.file import File
 from files_sdk.api import Api  # noqa: F401
 from files_sdk.list_obj import ListObj
 from files_sdk.error import (  # noqa: F401
     InvalidParameterError,
     MissingParameterError,
     NotImplementedError,
 )
 
 
-class Folder:
+class SsoStrategy:
     default_attributes = {
-        "path": None,  # string - File/Folder path This must be slash-delimited, but it must neither start nor end with a slash. Maximum of 5000 characters.
-        "created_by_id": None,  # int64 - User ID of the User who created the file/folder
-        "created_by_api_key_id": None,  # int64 - ID of the API key that created the file/folder
-        "created_by_as2_incoming_message_id": None,  # int64 - ID of the AS2 Incoming Message that created the file/folder
-        "created_by_automation_id": None,  # int64 - ID of the Automation that created the file/folder
-        "created_by_bundle_registration_id": None,  # int64 - ID of the Bundle Registration that created the file/folder
-        "created_by_inbox_id": None,  # int64 - ID of the Inbox that created the file/folder
-        "created_by_remote_server_id": None,  # int64 - ID of the Remote Server that created the file/folder
-        "created_by_remote_server_sync_id": None,  # int64 - ID of the Remote Server Sync that created the file/folder
-        "custom_metadata": None,  # object - Custom metadata map of keys and values. Limited to 32 keys, 256 characters per key and 1024 characters per value.
-        "display_name": None,  # string - File/Folder display name
-        "type": None,  # string - Type: `directory` or `file`.
-        "size": None,  # int64 - File/Folder size
-        "created_at": None,  # date-time - File created date/time
-        "last_modified_by_id": None,  # int64 - User ID of the User who last modified the file/folder
-        "last_modified_by_api_key_id": None,  # int64 - ID of the API key that last modified the file/folder
-        "last_modified_by_automation_id": None,  # int64 - ID of the Automation that last modified the file/folder
-        "last_modified_by_bundle_registration_id": None,  # int64 - ID of the Bundle Registration that last modified the file/folder
-        "last_modified_by_remote_server_id": None,  # int64 - ID of the Remote Server that last modified the file/folder
-        "last_modified_by_remote_server_sync_id": None,  # int64 - ID of the Remote Server Sync that last modified the file/folder
-        "mtime": None,  # date-time - File last modified date/time, according to the server.  This is the timestamp of the last Files.com operation of the file, regardless of what modified timestamp was sent.
-        "provided_mtime": None,  # date-time - File last modified date/time, according to the client who set it.  Files.com allows desktop, FTP, SFTP, and WebDAV clients to set modified at times.  This allows Desktop<->Cloud syncing to preserve modified at times.
-        "crc32": None,  # string - File CRC32 checksum. This is sometimes delayed, so if you get a blank response, wait and try again.
-        "md5": None,  # string - File MD5 checksum. This is sometimes delayed, so if you get a blank response, wait and try again.
-        "mime_type": None,  # string - MIME Type.  This is determined by the filename extension and is not stored separately internally.
-        "region": None,  # string - Region location
-        "permissions": None,  # string - A short string representing the current user's permissions.  Can be `r` (Read),`w` (Write),`d` (Delete), `l` (List) or any combination
-        "subfolders_locked?": None,  # boolean - Are subfolders locked and unable to be modified?
-        "is_locked": None,  # boolean - Is this folder locked and unable to be modified?
-        "download_uri": None,  # string - Link to download file. Provided only in response to a download request.
-        "priority_color": None,  # string - Bookmark/priority color of file/folder
-        "preview_id": None,  # int64 - File preview ID
-        "preview": None,  # Preview - File preview
-        "mkdir_parents": None,  # boolean - Create parent directories if they do not exist?
+        "protocol": None,  # string - SSO Protocol
+        "provider": None,  # string - Provider name
+        "label": None,  # string - Custom label for the SSO provider on the login page.
+        "logo_url": None,  # string - URL holding a custom logo for the SSO provider on the login page.
+        "id": None,  # int64 - ID
+        "user_count": None,  # int64 - Count of users with this SSO Strategy
+        "saml_provider_cert_fingerprint": None,  # string - Identity provider sha256 cert fingerprint if saml_provider_metadata_url is not available.
+        "saml_provider_issuer_url": None,  # string - Identity provider issuer url
+        "saml_provider_metadata_content": None,  # string - Custom identity provider metadata
+        "saml_provider_metadata_url": None,  # string - Metadata URL for the SAML identity provider
+        "saml_provider_slo_target_url": None,  # string - Identity provider SLO endpoint
+        "saml_provider_sso_target_url": None,  # string - Identity provider SSO endpoint if saml_provider_metadata_url is not available.
+        "scim_authentication_method": None,  # string - SCIM authentication type.
+        "scim_username": None,  # string - SCIM username.
+        "scim_oauth_access_token": None,  # string - SCIM OAuth Access Token.
+        "scim_oauth_access_token_expires_at": None,  # string - SCIM OAuth Access Token Expiration Time.
+        "subdomain": None,  # string - Subdomain
+        "provision_users": None,  # boolean - Auto-provision users?
+        "provision_groups": None,  # boolean - Auto-provision group membership based on group memberships on the SSO side?
+        "deprovision_users": None,  # boolean - Auto-deprovision users?
+        "deprovision_groups": None,  # boolean - Auto-deprovision group membership based on group memberships on the SSO side?
+        "deprovision_behavior": None,  # string - Method used for deprovisioning users.
+        "provision_group_default": None,  # string - Comma-separated list of group names for groups to automatically add all auto-provisioned users to.
+        "provision_group_exclusion": None,  # string - Comma-separated list of group names for groups (with optional wildcards) that will be excluded from auto-provisioning.
+        "provision_group_inclusion": None,  # string - Comma-separated list of group names for groups (with optional wildcards) that will be auto-provisioned.
+        "provision_group_required": None,  # string - Comma or newline separated list of group names (with optional wildcards) to require membership for user provisioning.
+        "provision_email_signup_groups": None,  # string - Comma-separated list of group names whose members will be created with email_signup authentication.
+        "provision_site_admin_groups": None,  # string - Comma-separated list of group names whose members will be created as Site Admins.
+        "provision_group_admin_groups": None,  # string - Comma-separated list of group names whose members will be provisioned as Group Admins.
+        "provision_attachments_permission": None,  # boolean - DEPRECATED: Auto-provisioned users get Sharing permission. Use a Group with the Bundle permission instead.
+        "provision_dav_permission": None,  # boolean - Auto-provisioned users get WebDAV permission?
+        "provision_ftp_permission": None,  # boolean - Auto-provisioned users get FTP permission?
+        "provision_sftp_permission": None,  # boolean - Auto-provisioned users get SFTP permission?
+        "provision_time_zone": None,  # string - Default time zone for auto provisioned users.
+        "provision_company": None,  # string - Default company for auto provisioned users.
+        "ldap_base_dn": None,  # string - Base DN for looking up users in LDAP server
+        "ldap_domain": None,  # string - Domain name that will be appended to LDAP usernames
+        "enabled": None,  # boolean - Is strategy enabled?  This may become automatically set to `false` after a high number and duration of failures.
+        "ldap_host": None,  # string - LDAP host
+        "ldap_host_2": None,  # string - LDAP backup host
+        "ldap_host_3": None,  # string - LDAP backup host
+        "ldap_port": None,  # int64 - LDAP port
+        "ldap_secure": None,  # boolean - Use secure LDAP?
+        "ldap_username": None,  # string - Username for signing in to LDAP server.
+        "ldap_username_field": None,  # string - LDAP username field
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
             options = {}
         self.set_attributes(attributes)
         self.options = options
 
     def set_attributes(self, attributes):
-        for attribute, default_value in Folder.default_attributes.items():
+        for attribute, default_value in SsoStrategy.default_attributes.items():
             setattr(self, attribute, attributes.get(attribute, default_value))
 
     def get_attributes(self):
         return {
             k: getattr(self, k, None)
-            for k in Folder.default_attributes
+            for k in SsoStrategy.default_attributes
             if getattr(self, k, None) is not None
         }
 
-    def save(self):
-        new_obj = create(self.path, self.get_attributes(), self.options)
-        self.set_attributes(new_obj.get_attributes())
-        return True
+    # Synchronize provisioning data with the SSO remote server
+    def sync(self, params=None):
+        if not isinstance(params, dict):
+            params = {}
+
+        if hasattr(self, "id") and self.id:
+            params["id"] = self.id
+        else:
+            raise MissingParameterError("Current object doesn't have a id")
+        if "id" not in params:
+            raise MissingParameterError("Parameter missing: id")
+        if "id" in params and not isinstance(params["id"], int):
+            raise InvalidParameterError("Bad parameter: id must be an int")
+        Api.send_request(
+            "POST",
+            "/sso_strategies/{id}/sync".format(id=params["id"]),
+            params,
+            self.options,
+        )
 
 
 # Parameters:
-#   cursor - string - Send cursor to resume an existing list from the point at which you left off.  Get a cursor from an existing list via the X-Files-Cursor-Next header or the X-Files-Cursor-Prev header.
+#   cursor - string - Used for pagination.  When a list request has more records available, cursors are provided in the response headers `X-Files-Cursor-Next` and `X-Files-Cursor-Prev`.  Send one of those cursor value here to resume an existing list from the next available record.  Note: many of our SDKs have iterator methods that will automatically handle cursor-based pagination.
 #   per_page - int64 - Number of records to show per page.  (Max: 10,000, 1,000 or less is recommended).
-#   path (required) - string - Path to operate on.
-#   filter - string - If specified, will filter folders/files list by name. Ignores text before last `/`. Wildcards of `*` and `?` are acceptable here.
-#   preview_size - string - Request a preview size.  Can be `small` (default), `large`, `xlarge`, or `pdf`.
-#   sort_by - object - Search by field and direction. Valid fields are `path`, `size`, `modified_at_datetime`, `provided_modified_at`.  Valid directions are `asc` and `desc`.  Defaults to `{"path":"asc"}`.
-#   search - string - If `search_all` is `true`, provide the search string here.  Otherwise, this parameter acts like an alias of `filter`.
-#   search_all - boolean - Search entire site?  If set, we will ignore the folder path provided and search the entire site.  This is the same API used by the search bar in the UI.  Search results are a best effort, not real time, and not guaranteed to match every file.  This field should only be used for ad-hoc (human) searching, and not as part of an automated process.
-#   with_previews - boolean - Include file previews?
-#   with_priority_color - boolean - Include file priority color information?
-def list_for(path, params=None, options=None):
+def list(params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
-    params["path"] = path
     if "cursor" in params and not isinstance(params["cursor"], str):
         raise InvalidParameterError("Bad parameter: cursor must be an str")
     if "per_page" in params and not isinstance(params["per_page"], int):
         raise InvalidParameterError("Bad parameter: per_page must be an int")
-    if "path" in params and not isinstance(params["path"], str):
-        raise InvalidParameterError("Bad parameter: path must be an str")
-    if "filter" in params and not isinstance(params["filter"], str):
-        raise InvalidParameterError("Bad parameter: filter must be an str")
-    if "preview_size" in params and not isinstance(
-        params["preview_size"], str
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: preview_size must be an str"
-        )
-    if "sort_by" in params and not isinstance(params["sort_by"], dict):
-        raise InvalidParameterError("Bad parameter: sort_by must be an dict")
-    if "search" in params and not isinstance(params["search"], str):
-        raise InvalidParameterError("Bad parameter: search must be an str")
-    if "path" not in params:
-        raise MissingParameterError("Parameter missing: path")
-    return ListObj(
-        File,
-        "GET",
-        "/folders/{path}".format(path=params["path"]),
-        params,
-        options,
-    )
+    return ListObj(SsoStrategy, "GET", "/sso_strategies", params, options)
+
+
+def all(params=None, options=None):
+    list(params, options)
 
 
 # Parameters:
-#   path (required) - string - Path to operate on.
-#   mkdir_parents - boolean - Create parent directories if they do not exist?
-#   provided_mtime - string - User provided modification time.
-def create(path, params=None, options=None):
+#   id (required) - int64 - Sso Strategy ID.
+def find(id, params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
-    params["path"] = path
-    if "path" in params and not isinstance(params["path"], str):
-        raise InvalidParameterError("Bad parameter: path must be an str")
-    if "provided_mtime" in params and not isinstance(
-        params["provided_mtime"], str
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: provided_mtime must be an str"
-        )
-    if "path" not in params:
-        raise MissingParameterError("Parameter missing: path")
+    params["id"] = id
+    if "id" in params and not isinstance(params["id"], int):
+        raise InvalidParameterError("Bad parameter: id must be an int")
+    if "id" not in params:
+        raise MissingParameterError("Parameter missing: id")
     response, options = Api.send_request(
-        "POST", "/folders/{path}".format(path=params["path"]), params, options
+        "GET", "/sso_strategies/{id}".format(id=params["id"]), params, options
+    )
+    return SsoStrategy(response.data, options)
+
+
+def get(id, params=None, options=None):
+    find(id, params, options)
+
+
+# Synchronize provisioning data with the SSO remote server
+def sync(id, params=None, options=None):
+    if not isinstance(params, dict):
+        params = {}
+    if not isinstance(options, dict):
+        options = {}
+    params["id"] = id
+    if "id" in params and not isinstance(params["id"], int):
+        raise InvalidParameterError("Bad parameter: id must be an int")
+    if "id" not in params:
+        raise MissingParameterError("Parameter missing: id")
+    Api.send_request(
+        "POST",
+        "/sso_strategies/{id}/sync".format(id=params["id"]),
+        params,
+        options,
     )
-    return File(response.data, options)
 
 
 def new(*args, **kwargs):
-    return Folder(*args, **kwargs)
+    return SsoStrategy(*args, **kwargs)
```

### Comparing `Files.com-1.4.81/files_sdk/models/form_field.py` & `Files.com-1.4.9/files_sdk/models/remote_server_configuration_file.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,41 +3,48 @@
 from files_sdk.error import (  # noqa: F401
     InvalidParameterError,
     MissingParameterError,
     NotImplementedError,
 )
 
 
-class FormField:
+class RemoteServerConfigurationFile:
     default_attributes = {
-        "id": None,  # int64 - Form field id
-        "label": None,  # string - Label to be displayed
-        "required": None,  # boolean - Is this a required field?
-        "help_text": None,  # string - Help text to be displayed
-        "field_type": None,  # string - Type of Field
-        "options_for_select": None,  # array - Options to display for radio and dropdown
-        "default_option": None,  # string - Default option for radio and dropdown
-        "form_field_set_id": None,  # int64 - Form field set id
+        "id": None,  # int64 - Agent ID
+        "permission_set": None,  # string -
+        "private_key": None,  # string - private key
+        "subdomain": None,  # string
+        "root": None,  # string - Agent local root path
+        "api_token": None,  # string - Files Agent API Token
+        "port": None,  # int64 - Incoming port for files agent connections
+        "hostname": None,  # string
+        "public_key": None,  # string - public key
+        "status": None,  # string - either running or shutdown
+        "server_host_key": None,  # string
+        "config_version": None,  # string - agent config version
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
             options = {}
         self.set_attributes(attributes)
         self.options = options
 
     def set_attributes(self, attributes):
-        for attribute, default_value in FormField.default_attributes.items():
+        for (
+            attribute,
+            default_value,
+        ) in RemoteServerConfigurationFile.default_attributes.items():
             setattr(self, attribute, attributes.get(attribute, default_value))
 
     def get_attributes(self):
         return {
             k: getattr(self, k, None)
-            for k in FormField.default_attributes
+            for k in RemoteServerConfigurationFile.default_attributes
             if getattr(self, k, None) is not None
         }
 
 
 def new(*args, **kwargs):
-    return FormField(*args, **kwargs)
+    return RemoteServerConfigurationFile(*args, **kwargs)
```

### Comparing `Files.com-1.4.81/files_sdk/models/form_field_set.py` & `Files.com-1.4.9/files_sdk/models/form_field_set.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/gpg_key.py` & `Files.com-1.4.9/files_sdk/models/gpg_key.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/group.py` & `Files.com-1.4.9/files_sdk/models/group.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 )
 
 
 class Group:
     default_attributes = {
         "id": None,  # int64 - Group ID
         "name": None,  # string - Group name
-        "allowed_ips": None,  # string - A list of allowed IPs if applicable.  Newline delimited
         "admin_ids": None,  # string - Comma-delimited list of user IDs who are group administrators (separated by commas)
         "notes": None,  # string - Notes about this group
         "user_ids": None,  # string - Comma-delimited list of user IDs who belong to this group (separated by commas)
         "usernames": None,  # string - Comma-delimited list of usernames who belong to this group (separated by commas)
         "ftp_permission": None,  # boolean - If true, users in this group can use FTP to login.  This will override a false value of `ftp_permission` on the user level.
         "sftp_permission": None,  # boolean - If true, users in this group can use SFTP to login.  This will override a false value of `sftp_permission` on the user level.
         "dav_permission": None,  # boolean - If true, users in this group can use WebDAV to login.  This will override a false value of `dav_permission` on the user level.
@@ -46,15 +45,14 @@
     #   notes - string - Group notes.
     #   user_ids - string - A list of user ids. If sent as a string, should be comma-delimited.
     #   admin_ids - string - A list of group admin user ids. If sent as a string, should be comma-delimited.
     #   ftp_permission - boolean - If true, users in this group can use FTP to login.  This will override a false value of `ftp_permission` on the user level.
     #   sftp_permission - boolean - If true, users in this group can use SFTP to login.  This will override a false value of `sftp_permission` on the user level.
     #   dav_permission - boolean - If true, users in this group can use WebDAV to login.  This will override a false value of `dav_permission` on the user level.
     #   restapi_permission - boolean - If true, users in this group can use the REST API to login.  This will override a false value of `restapi_permission` on the user level.
-    #   allowed_ips - string - A list of allowed IPs if applicable.  Newline delimited
     #   name - string - Group name.
     def update(self, params=None):
         if not isinstance(params, dict):
             params = {}
 
         if hasattr(self, "id") and self.id:
             params["id"] = self.id
@@ -70,20 +68,14 @@
             raise InvalidParameterError(
                 "Bad parameter: user_ids must be an str"
             )
         if "admin_ids" in params and not isinstance(params["admin_ids"], str):
             raise InvalidParameterError(
                 "Bad parameter: admin_ids must be an str"
             )
-        if "allowed_ips" in params and not isinstance(
-            params["allowed_ips"], str
-        ):
-            raise InvalidParameterError(
-                "Bad parameter: allowed_ips must be an str"
-            )
         if "name" in params and not isinstance(params["name"], str):
             raise InvalidParameterError("Bad parameter: name must be an str")
         response, _options = Api.send_request(
             "PATCH",
             "/groups/{id}".format(id=params["id"]),
             params,
             self.options,
@@ -184,31 +176,26 @@
 #   notes - string - Group notes.
 #   user_ids - string - A list of user ids. If sent as a string, should be comma-delimited.
 #   admin_ids - string - A list of group admin user ids. If sent as a string, should be comma-delimited.
 #   ftp_permission - boolean - If true, users in this group can use FTP to login.  This will override a false value of `ftp_permission` on the user level.
 #   sftp_permission - boolean - If true, users in this group can use SFTP to login.  This will override a false value of `sftp_permission` on the user level.
 #   dav_permission - boolean - If true, users in this group can use WebDAV to login.  This will override a false value of `dav_permission` on the user level.
 #   restapi_permission - boolean - If true, users in this group can use the REST API to login.  This will override a false value of `restapi_permission` on the user level.
-#   allowed_ips - string - A list of allowed IPs if applicable.  Newline delimited
 #   name (required) - string - Group name.
 def create(params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     if "notes" in params and not isinstance(params["notes"], str):
         raise InvalidParameterError("Bad parameter: notes must be an str")
     if "user_ids" in params and not isinstance(params["user_ids"], str):
         raise InvalidParameterError("Bad parameter: user_ids must be an str")
     if "admin_ids" in params and not isinstance(params["admin_ids"], str):
         raise InvalidParameterError("Bad parameter: admin_ids must be an str")
-    if "allowed_ips" in params and not isinstance(params["allowed_ips"], str):
-        raise InvalidParameterError(
-            "Bad parameter: allowed_ips must be an str"
-        )
     if "name" in params and not isinstance(params["name"], str):
         raise InvalidParameterError("Bad parameter: name must be an str")
     if "name" not in params:
         raise MissingParameterError("Parameter missing: name")
     response, options = Api.send_request("POST", "/groups", params, options)
     return Group(response.data, options)
 
@@ -217,15 +204,14 @@
 #   notes - string - Group notes.
 #   user_ids - string - A list of user ids. If sent as a string, should be comma-delimited.
 #   admin_ids - string - A list of group admin user ids. If sent as a string, should be comma-delimited.
 #   ftp_permission - boolean - If true, users in this group can use FTP to login.  This will override a false value of `ftp_permission` on the user level.
 #   sftp_permission - boolean - If true, users in this group can use SFTP to login.  This will override a false value of `sftp_permission` on the user level.
 #   dav_permission - boolean - If true, users in this group can use WebDAV to login.  This will override a false value of `dav_permission` on the user level.
 #   restapi_permission - boolean - If true, users in this group can use the REST API to login.  This will override a false value of `restapi_permission` on the user level.
-#   allowed_ips - string - A list of allowed IPs if applicable.  Newline delimited
 #   name - string - Group name.
 def update(id, params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     params["id"] = id
@@ -233,18 +219,14 @@
         raise InvalidParameterError("Bad parameter: id must be an int")
     if "notes" in params and not isinstance(params["notes"], str):
         raise InvalidParameterError("Bad parameter: notes must be an str")
     if "user_ids" in params and not isinstance(params["user_ids"], str):
         raise InvalidParameterError("Bad parameter: user_ids must be an str")
     if "admin_ids" in params and not isinstance(params["admin_ids"], str):
         raise InvalidParameterError("Bad parameter: admin_ids must be an str")
-    if "allowed_ips" in params and not isinstance(params["allowed_ips"], str):
-        raise InvalidParameterError(
-            "Bad parameter: allowed_ips must be an str"
-        )
     if "name" in params and not isinstance(params["name"], str):
         raise InvalidParameterError("Bad parameter: name must be an str")
     if "id" not in params:
         raise MissingParameterError("Parameter missing: id")
     response, options = Api.send_request(
         "PATCH", "/groups/{id}".format(id=params["id"]), params, options
     )
```

### Comparing `Files.com-1.4.81/files_sdk/models/group_user.py` & `Files.com-1.4.9/files_sdk/models/group_user.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/history.py` & `Files.com-1.4.9/files_sdk/models/history.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/history_export.py` & `Files.com-1.4.9/files_sdk/models/history_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,21 @@
         "end_at": None,  # date-time - End date/time of export range.
         "status": None,  # string - Status of export.  Will be: `building`, `ready`, or `failed`
         "query_action": None,  # string - Filter results by this this action type. Valid values: `create`, `read`, `update`, `destroy`, `move`, `login`, `failedlogin`, `copy`, `user_create`, `user_update`, `user_destroy`, `group_create`, `group_update`, `group_destroy`, `permission_create`, `permission_destroy`, `api_key_create`, `api_key_update`, `api_key_destroy`
         "query_interface": None,  # string - Filter results by this this interface type. Valid values: `web`, `ftp`, `robot`, `jsapi`, `webdesktopapi`, `sftp`, `dav`, `desktop`, `restapi`, `scim`, `office`, `mobile`, `as2`, `inbound_email`, `remote`
         "query_user_id": None,  # string - Return results that are actions performed by the user indiciated by this User ID
         "query_file_id": None,  # string - Return results that are file actions related to the file indicated by this File ID
         "query_parent_id": None,  # string - Return results that are file actions inside the parent folder specified by this folder ID
-        "query_path": None,  # string - Return results that are file actions related to paths matching this pattern.
-        "query_folder": None,  # string - Return results that are file actions related to files or folders inside folder paths matching this pattern.
-        "query_src": None,  # string - Return results that are file moves originating from paths matching this pattern.
-        "query_destination": None,  # string - Return results that are file moves with paths matching this pattern as destination.
+        "query_path": None,  # string - Return results that are file actions related to this path.
+        "query_folder": None,  # string - Return results that are file actions related to files or folders inside this folder path.
+        "query_src": None,  # string - Return results that are file moves originating from this path.
+        "query_destination": None,  # string - Return results that are file moves with this path as destination.
         "query_ip": None,  # string - Filter results by this IP address.
         "query_username": None,  # string - Filter results by this username.
-        "query_failure_type": None,  # string - If searching for Histories about login failures, this parameter restricts results to failures of this specific type.  Valid values: `expired_trial`, `account_overdue`, `locked_out`, `ip_mismatch`, `password_mismatch`, `site_mismatch`, `username_not_found`, `none`, `no_ftp_permission`, `no_web_permission`, `no_directory`, `errno_enoent`, `no_sftp_permission`, `no_dav_permission`, `no_restapi_permission`, `key_mismatch`, `region_mismatch`, `expired_access`, `desktop_ip_mismatch`, `desktop_api_key_not_used_quickly_enough`, `disabled`, `country_mismatch`, `insecure_ftp`, `insecure_cipher`, `rate_limited`
+        "query_failure_type": None,  # string - If searching for Histories about login failures, this parameter restricts results to failures of this specific type.  Valid values: `expired_trial`, `account_overdue`, `locked_out`, `ip_mismatch`, `password_mismatch`, `site_mismatch`, `username_not_found`, `none`, `no_ftp_permission`, `no_web_permission`, `no_directory`, `errno_enoent`, `no_sftp_permission`, `no_dav_permission`, `no_restapi_permission`, `key_mismatch`, `region_mismatch`, `expired_access`, `desktop_ip_mismatch`, `desktop_api_key_not_used_quickly_enough`, `disabled`, `country_mismatch`
         "query_target_id": None,  # string - If searching for Histories about specific objects (such as Users, or API Keys), this paremeter restricts results to objects that match this ID.
         "query_target_name": None,  # string - If searching for Histories about Users, Groups or other objects with names, this parameter restricts results to objects with this name/username.
         "query_target_permission": None,  # string - If searching for Histories about Permisisons, this parameter restricts results to permissions of this level.
         "query_target_user_id": None,  # string - If searching for Histories about API keys, this parameter restricts results to API keys created by/for this user ID.
         "query_target_username": None,  # string - If searching for Histories about API keys, this parameter restricts results to API keys created by/for this username.
         "query_target_platform": None,  # string - If searching for Histories about API keys, this parameter restricts results to API keys associated with this platform.
         "query_target_permission_set": None,  # string - If searching for Histories about API keys, this parameter restricts results to API keys with this permission set.
@@ -97,21 +97,21 @@
 #   start_at - string - Start date/time of export range.
 #   end_at - string - End date/time of export range.
 #   query_action - string - Filter results by this this action type. Valid values: `create`, `read`, `update`, `destroy`, `move`, `login`, `failedlogin`, `copy`, `user_create`, `user_update`, `user_destroy`, `group_create`, `group_update`, `group_destroy`, `permission_create`, `permission_destroy`, `api_key_create`, `api_key_update`, `api_key_destroy`
 #   query_interface - string - Filter results by this this interface type. Valid values: `web`, `ftp`, `robot`, `jsapi`, `webdesktopapi`, `sftp`, `dav`, `desktop`, `restapi`, `scim`, `office`, `mobile`, `as2`, `inbound_email`, `remote`
 #   query_user_id - string - Return results that are actions performed by the user indiciated by this User ID
 #   query_file_id - string - Return results that are file actions related to the file indicated by this File ID
 #   query_parent_id - string - Return results that are file actions inside the parent folder specified by this folder ID
-#   query_path - string - Return results that are file actions related to paths matching this pattern.
-#   query_folder - string - Return results that are file actions related to files or folders inside folder paths matching this pattern.
-#   query_src - string - Return results that are file moves originating from paths matching this pattern.
-#   query_destination - string - Return results that are file moves with paths matching this pattern as destination.
+#   query_path - string - Return results that are file actions related to this path.
+#   query_folder - string - Return results that are file actions related to files or folders inside this folder path.
+#   query_src - string - Return results that are file moves originating from this path.
+#   query_destination - string - Return results that are file moves with this path as destination.
 #   query_ip - string - Filter results by this IP address.
 #   query_username - string - Filter results by this username.
-#   query_failure_type - string - If searching for Histories about login failures, this parameter restricts results to failures of this specific type.  Valid values: `expired_trial`, `account_overdue`, `locked_out`, `ip_mismatch`, `password_mismatch`, `site_mismatch`, `username_not_found`, `none`, `no_ftp_permission`, `no_web_permission`, `no_directory`, `errno_enoent`, `no_sftp_permission`, `no_dav_permission`, `no_restapi_permission`, `key_mismatch`, `region_mismatch`, `expired_access`, `desktop_ip_mismatch`, `desktop_api_key_not_used_quickly_enough`, `disabled`, `country_mismatch`, `insecure_ftp`, `insecure_cipher`, `rate_limited`
+#   query_failure_type - string - If searching for Histories about login failures, this parameter restricts results to failures of this specific type.  Valid values: `expired_trial`, `account_overdue`, `locked_out`, `ip_mismatch`, `password_mismatch`, `site_mismatch`, `username_not_found`, `none`, `no_ftp_permission`, `no_web_permission`, `no_directory`, `errno_enoent`, `no_sftp_permission`, `no_dav_permission`, `no_restapi_permission`, `key_mismatch`, `region_mismatch`, `expired_access`, `desktop_ip_mismatch`, `desktop_api_key_not_used_quickly_enough`, `disabled`, `country_mismatch`
 #   query_target_id - string - If searching for Histories about specific objects (such as Users, or API Keys), this paremeter restricts results to objects that match this ID.
 #   query_target_name - string - If searching for Histories about Users, Groups or other objects with names, this parameter restricts results to objects with this name/username.
 #   query_target_permission - string - If searching for Histories about Permisisons, this parameter restricts results to permissions of this level.
 #   query_target_user_id - string - If searching for Histories about API keys, this parameter restricts results to API keys created by/for this user ID.
 #   query_target_username - string - If searching for Histories about API keys, this parameter restricts results to API keys created by/for this username.
 #   query_target_platform - string - If searching for Histories about API keys, this parameter restricts results to API keys associated with this platform.
 #   query_target_permission_set - string - If searching for Histories about API keys, this parameter restricts results to API keys with this permission set.
```

### Comparing `Files.com-1.4.81/files_sdk/models/history_export_result.py` & `Files.com-1.4.9/files_sdk/models/history_export_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "path": None,  # string - Path of the related action This must be slash-delimited, but it must neither start nor end with a slash. Maximum of 5000 characters.
         "folder": None,  # string - Folder in which the action occurred
         "src": None,  # string - File move originated from this path
         "destination": None,  # string - File moved to this destination folder
         "ip": None,  # string - Client IP that performed the action
         "username": None,  # string - Username of the user that performed the action
         "action": None,  # string - What action was taken. Valid values: `create`, `read`, `update`, `destroy`, `move`, `login`, `failedlogin`, `copy`, `user_create`, `user_update`, `user_destroy`, `group_create`, `group_update`, `group_destroy`, `permission_create`, `permission_destroy`, `api_key_create`, `api_key_update`, `api_key_destroy`
-        "failure_type": None,  # string - The type of login failure, if applicable.  Valid values: `expired_trial`, `account_overdue`, `locked_out`, `ip_mismatch`, `password_mismatch`, `site_mismatch`, `username_not_found`, `none`, `no_ftp_permission`, `no_web_permission`, `no_directory`, `errno_enoent`, `no_sftp_permission`, `no_dav_permission`, `no_restapi_permission`, `key_mismatch`, `region_mismatch`, `expired_access`, `desktop_ip_mismatch`, `desktop_api_key_not_used_quickly_enough`, `disabled`, `country_mismatch`, `insecure_ftp`, `insecure_cipher`, `rate_limited`
+        "failure_type": None,  # string - The type of login failure, if applicable.  Valid values: `expired_trial`, `account_overdue`, `locked_out`, `ip_mismatch`, `password_mismatch`, `site_mismatch`, `username_not_found`, `none`, `no_ftp_permission`, `no_web_permission`, `no_directory`, `errno_enoent`, `no_sftp_permission`, `no_dav_permission`, `no_restapi_permission`, `key_mismatch`, `region_mismatch`, `expired_access`, `desktop_ip_mismatch`, `desktop_api_key_not_used_quickly_enough`, `disabled`, `country_mismatch`
         "interface": None,  # string - Inteface through which the action was taken. Valid values: `web`, `ftp`, `robot`, `jsapi`, `webdesktopapi`, `sftp`, `dav`, `desktop`, `restapi`, `scim`, `office`, `mobile`, `as2`, `inbound_email`, `remote`
         "target_id": None,  # int64 - ID of the object (such as Users, or API Keys) on which the action was taken
         "target_name": None,  # string - Name of the User, Group or other object with a name related to this action
         "target_permission": None,  # string - Permission level of the action
         "target_recursive": None,  # boolean - Whether or not the action was recursive
         "target_expires_at": None,  # int64 - If searching for Histories about API keys, this is when the API key will expire. Represented as a Unix timestamp.
         "target_expires_at_iso8601": None,  # string - If searching for Histories about API keys, this is when the API key will expire. Represented in ISO8601 format.
```

### Comparing `Files.com-1.4.81/files_sdk/models/image.py` & `Files.com-1.4.9/files_sdk/models/image.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/inbox_recipient.py` & `Files.com-1.4.9/files_sdk/models/inbox_recipient.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/inbox_registration.py` & `Files.com-1.4.9/files_sdk/models/inbox_registration.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/inbox_upload.py` & `Files.com-1.4.9/files_sdk/models/remote_bandwidth_snapshot.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,52 +4,55 @@
 from files_sdk.error import (  # noqa: F401
     InvalidParameterError,
     MissingParameterError,
     NotImplementedError,
 )
 
 
-class InboxUpload:
+class RemoteBandwidthSnapshot:
     default_attributes = {
-        "inbox_registration": None,  # InboxRegistration
-        "path": None,  # string - Upload path This must be slash-delimited, but it must neither start nor end with a slash. Maximum of 5000 characters.
-        "created_at": None,  # date-time - Upload date/time
+        "id": None,  # int64 - Site bandwidth ID
+        "sync_bytes_received": None,  # double - Site sync bandwidth report bytes received
+        "sync_bytes_sent": None,  # double - Site sync bandwidth report bytes sent
+        "logged_at": None,  # date-time - Time the site bandwidth report was logged
+        "remote_server_id": None,  # int64 - ID of related Remote Server
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
             options = {}
         self.set_attributes(attributes)
         self.options = options
 
     def set_attributes(self, attributes):
-        for attribute, default_value in InboxUpload.default_attributes.items():
+        for (
+            attribute,
+            default_value,
+        ) in RemoteBandwidthSnapshot.default_attributes.items():
             setattr(self, attribute, attributes.get(attribute, default_value))
 
     def get_attributes(self):
         return {
             k: getattr(self, k, None)
-            for k in InboxUpload.default_attributes
+            for k in RemoteBandwidthSnapshot.default_attributes
             if getattr(self, k, None) is not None
         }
 
 
 # Parameters:
 #   cursor - string - Used for pagination.  When a list request has more records available, cursors are provided in the response headers `X-Files-Cursor-Next` and `X-Files-Cursor-Prev`.  Send one of those cursor value here to resume an existing list from the next available record.  Note: many of our SDKs have iterator methods that will automatically handle cursor-based pagination.
 #   per_page - int64 - Number of records to show per page.  (Max: 10,000, 1,000 or less is recommended).
-#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[created_at]=desc`). Valid fields are `created_at`.
-#   filter - object - If set, return records where the specified field is equal to the supplied value. Valid fields are `created_at`.
-#   filter_gt - object - If set, return records where the specified field is greater than the supplied value. Valid fields are `created_at`.
-#   filter_gteq - object - If set, return records where the specified field is greater than or equal the supplied value. Valid fields are `created_at`.
-#   filter_lt - object - If set, return records where the specified field is less than the supplied value. Valid fields are `created_at`.
-#   filter_lteq - object - If set, return records where the specified field is less than or equal the supplied value. Valid fields are `created_at`.
-#   inbox_registration_id - int64 - InboxRegistration ID
-#   inbox_id - int64 - Inbox ID
+#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[logged_at]=desc`). Valid fields are `logged_at`.
+#   filter - object - If set, return records where the specified field is equal to the supplied value. Valid fields are `logged_at`.
+#   filter_gt - object - If set, return records where the specified field is greater than the supplied value. Valid fields are `logged_at`.
+#   filter_gteq - object - If set, return records where the specified field is greater than or equal the supplied value. Valid fields are `logged_at`.
+#   filter_lt - object - If set, return records where the specified field is less than the supplied value. Valid fields are `logged_at`.
+#   filter_lteq - object - If set, return records where the specified field is less than or equal the supplied value. Valid fields are `logged_at`.
 def list(params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     if "cursor" in params and not isinstance(params["cursor"], str):
         raise InvalidParameterError("Bad parameter: cursor must be an str")
@@ -67,24 +70,22 @@
         )
     if "filter_lt" in params and not isinstance(params["filter_lt"], dict):
         raise InvalidParameterError("Bad parameter: filter_lt must be an dict")
     if "filter_lteq" in params and not isinstance(params["filter_lteq"], dict):
         raise InvalidParameterError(
             "Bad parameter: filter_lteq must be an dict"
         )
-    if "inbox_registration_id" in params and not isinstance(
-        params["inbox_registration_id"], int
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: inbox_registration_id must be an int"
-        )
-    if "inbox_id" in params and not isinstance(params["inbox_id"], int):
-        raise InvalidParameterError("Bad parameter: inbox_id must be an int")
-    return ListObj(InboxUpload, "GET", "/inbox_uploads", params, options)
+    return ListObj(
+        RemoteBandwidthSnapshot,
+        "GET",
+        "/remote_bandwidth_snapshots",
+        params,
+        options,
+    )
 
 
 def all(params=None, options=None):
     list(params, options)
 
 
 def new(*args, **kwargs):
-    return InboxUpload(*args, **kwargs)
+    return RemoteBandwidthSnapshot(*args, **kwargs)
```

### Comparing `Files.com-1.4.81/files_sdk/models/invoice.py` & `Files.com-1.4.9/files_sdk/models/invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         "invoice_line_items": None,  # array - Associated invoice line items
         "method": None,  # string - Line item payment method
         "payment_line_items": None,  # array - Associated payment line items
         "payment_reversed_at": None,  # date-time - Date/time payment was reversed if applicable
         "payment_type": None,  # string - Type of payment if applicable
         "site_name": None,  # string - Site name this line item is for
         "type": None,  # string - Type of line item, either payment or invoice
+        "updated_at": None,  # date-time - Line item updated at
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
             options = {}
```

### Comparing `Files.com-1.4.81/files_sdk/models/invoice_line_item.py` & `Files.com-1.4.9/files_sdk/models/invoice_line_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     default_attributes = {
         "amount": None,  # double - Invoice line item amount
         "created_at": None,  # date-time - Invoice line item created at date/time
         "description": None,  # string - Invoice line item description
         "type": None,  # string - Invoice line item type
         "service_end_at": None,  # date-time - Invoice line item service end date/time
         "service_start_at": None,  # date-time - Invoice line item service start date/time
+        "updated_at": None,  # date-time - Invoice line item updated date/time
         "plan": None,  # string - Plan name
         "site": None,  # string - Site name
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
```

### Comparing `Files.com-1.4.81/files_sdk/models/ip_address.py` & `Files.com-1.4.9/files_sdk/models/ip_address.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,35 +55,14 @@
 def all(params=None, options=None):
     list(params, options)
 
 
 # Parameters:
 #   cursor - string - Used for pagination.  When a list request has more records available, cursors are provided in the response headers `X-Files-Cursor-Next` and `X-Files-Cursor-Prev`.  Send one of those cursor value here to resume an existing list from the next available record.  Note: many of our SDKs have iterator methods that will automatically handle cursor-based pagination.
 #   per_page - int64 - Number of records to show per page.  (Max: 10,000, 1,000 or less is recommended).
-def get_smartfile_reserved(params=None, options=None):
-    if not isinstance(params, dict):
-        params = {}
-    if not isinstance(options, dict):
-        options = {}
-    if "cursor" in params and not isinstance(params["cursor"], str):
-        raise InvalidParameterError("Bad parameter: cursor must be an str")
-    if "per_page" in params and not isinstance(params["per_page"], int):
-        raise InvalidParameterError("Bad parameter: per_page must be an int")
-    return ListObj(
-        PublicIpAddress,
-        "GET",
-        "/ip_addresses/smartfile-reserved",
-        params,
-        options,
-    )
-
-
-# Parameters:
-#   cursor - string - Used for pagination.  When a list request has more records available, cursors are provided in the response headers `X-Files-Cursor-Next` and `X-Files-Cursor-Prev`.  Send one of those cursor value here to resume an existing list from the next available record.  Note: many of our SDKs have iterator methods that will automatically handle cursor-based pagination.
-#   per_page - int64 - Number of records to show per page.  (Max: 10,000, 1,000 or less is recommended).
 def get_exavault_reserved(params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     if "cursor" in params and not isinstance(params["cursor"], str):
         raise InvalidParameterError("Bad parameter: cursor must be an str")
```

### Comparing `Files.com-1.4.81/files_sdk/models/lock.py` & `Files.com-1.4.9/files_sdk/models/lock.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/message.py` & `Files.com-1.4.9/files_sdk/models/message.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/message_comment.py` & `Files.com-1.4.9/files_sdk/models/message_comment.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/message_comment_reaction.py` & `Files.com-1.4.9/files_sdk/models/message_comment_reaction.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/message_reaction.py` & `Files.com-1.4.9/files_sdk/models/message_reaction.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/notification.py` & `Files.com-1.4.9/files_sdk/models/notification.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 )
 
 
 class Notification:
     default_attributes = {
         "id": None,  # int64 - Notification ID
         "path": None,  # string - Folder path to notify on This must be slash-delimited, but it must neither start nor end with a slash. Maximum of 5000 characters.
-        "group_id": None,  # int64 - ID of Group to receive notifications
-        "group_name": None,  # string - Group name, if a Group ID is set
-        "triggering_group_ids": None,  # array - If set, will only notify on actions made by a member of one of the specified groups
-        "triggering_user_ids": None,  # array - If set, will onlynotify on actions made one of the specified users
+        "group_id": None,  # int64 - Notification group id
+        "group_name": None,  # string - Group name if applicable
+        "triggering_group_ids": None,  # array - Only notify on actions made by a member of one of the specified groups
+        "triggering_user_ids": None,  # array - Only notify on actions made one of the specified users
         "trigger_by_share_recipients": None,  # boolean - Notify when actions are performed by a share recipient?
-        "notify_user_actions": None,  # boolean - If true, will send notifications about a user's own activity to that user.  If false, only activity performed by other users (or anonymous users) will be sent in notifications.
-        "notify_on_copy": None,  # boolean - Trigger on files copied to this path?
-        "notify_on_delete": None,  # boolean - Trigger on files deleted in this path?
-        "notify_on_download": None,  # boolean - Trigger on files downloaded in this path?
-        "notify_on_move": None,  # boolean - Trigger on files moved to this path?
-        "notify_on_upload": None,  # boolean - Trigger on files created/uploaded/updated/changed in this path?
-        "recursive": None,  # boolean - Apply notification recursively?  This will enable notifications for each subfolder.
+        "notify_user_actions": None,  # boolean - Trigger notification on notification user actions?
+        "notify_on_copy": None,  # boolean - Triggers notification when copying files to this path
+        "notify_on_delete": None,  # boolean - Triggers notification when deleting files from this path
+        "notify_on_download": None,  # boolean - Triggers notification when downloading files from this path
+        "notify_on_move": None,  # boolean - Triggers notification when moving files to this path
+        "notify_on_upload": None,  # boolean - Triggers notification when uploading new files to this path
+        "recursive": None,  # boolean - Enable notifications for each subfolder in this path
         "send_interval": None,  # string - The time interval that notifications are aggregated to
-        "message": None,  # string - Custom message to include in notification emails
-        "triggering_filenames": None,  # array - Array of filenames (possibly with wildcards) to scope trigger
+        "message": None,  # string - Custom message to include in notification emails.
+        "triggering_filenames": None,  # array - Array of filenames (possibly with wildcards) to match for action path
         "unsubscribed": None,  # boolean - Is the user unsubscribed from this notification?
         "unsubscribed_reason": None,  # string - The reason that the user unsubscribed
         "user_id": None,  # int64 - Notification user ID
         "username": None,  # string - Notification username
         "suppressed_email": None,  # boolean - If true, it means that the recipient at this user's email address has manually unsubscribed from all emails, or had their email "hard bounce", which means that we are unable to send mail to this user's current email address. Notifications will resume if the user changes their email address.
     }
 
@@ -54,25 +54,25 @@
             k: getattr(self, k, None)
             for k in Notification.default_attributes
             if getattr(self, k, None) is not None
         }
 
     # Parameters:
     #   notify_on_copy - boolean - If `true`, copying or moving resources into this path will trigger a notification, in addition to just uploads.
-    #   notify_on_delete - boolean - Trigger on files deleted in this path?
-    #   notify_on_download - boolean - Trigger on files downloaded in this path?
-    #   notify_on_move - boolean - Trigger on files moved to this path?
-    #   notify_on_upload - boolean - Trigger on files created/uploaded/updated/changed in this path?
+    #   notify_on_delete - boolean - Triggers notification when deleting files from this path
+    #   notify_on_download - boolean - Triggers notification when downloading files from this path
+    #   notify_on_move - boolean - Triggers notification when moving files to this path
+    #   notify_on_upload - boolean - Triggers notification when uploading new files to this path
     #   notify_user_actions - boolean - If `true` actions initiated by the user will still result in a notification
     #   recursive - boolean - If `true`, enable notifications for each subfolder in this path
     #   send_interval - string - The time interval that notifications are aggregated by.  Can be `five_minutes`, `fifteen_minutes`, `hourly`, or `daily`.
-    #   message - string - Custom message to include in notification emails
-    #   triggering_filenames - array(string) - Array of filenames (possibly with wildcards) to scope trigger
-    #   triggering_group_ids - array(int64) - If set, will only notify on actions made by a member of one of the specified groups
-    #   triggering_user_ids - array(int64) - If set, will onlynotify on actions made one of the specified users
+    #   message - string - Custom message to include in notification emails.
+    #   triggering_filenames - array(string) - Array of filenames (possibly with wildcards) to match for action path
+    #   triggering_group_ids - array(int64) - Only notify on actions made by a member of one of the specified groups
+    #   triggering_user_ids - array(int64) - Only notify on actions made one of the specified users
     #   trigger_by_share_recipients - boolean - Notify when actions are performed by a share recipient?
     def update(self, params=None):
         if not isinstance(params, dict):
             params = {}
 
         if hasattr(self, "id") and self.id:
             params["id"] = self.id
@@ -214,25 +214,25 @@
 def get(id, params=None, options=None):
     find(id, params, options)
 
 
 # Parameters:
 #   user_id - int64 - The id of the user to notify. Provide `user_id`, `username` or `group_id`.
 #   notify_on_copy - boolean - If `true`, copying or moving resources into this path will trigger a notification, in addition to just uploads.
-#   notify_on_delete - boolean - Trigger on files deleted in this path?
-#   notify_on_download - boolean - Trigger on files downloaded in this path?
-#   notify_on_move - boolean - Trigger on files moved to this path?
-#   notify_on_upload - boolean - Trigger on files created/uploaded/updated/changed in this path?
+#   notify_on_delete - boolean - Triggers notification when deleting files from this path
+#   notify_on_download - boolean - Triggers notification when downloading files from this path
+#   notify_on_move - boolean - Triggers notification when moving files to this path
+#   notify_on_upload - boolean - Triggers notification when uploading new files to this path
 #   notify_user_actions - boolean - If `true` actions initiated by the user will still result in a notification
 #   recursive - boolean - If `true`, enable notifications for each subfolder in this path
 #   send_interval - string - The time interval that notifications are aggregated by.  Can be `five_minutes`, `fifteen_minutes`, `hourly`, or `daily`.
-#   message - string - Custom message to include in notification emails
-#   triggering_filenames - array(string) - Array of filenames (possibly with wildcards) to scope trigger
-#   triggering_group_ids - array(int64) - If set, will only notify on actions made by a member of one of the specified groups
-#   triggering_user_ids - array(int64) - If set, will onlynotify on actions made one of the specified users
+#   message - string - Custom message to include in notification emails.
+#   triggering_filenames - array(string) - Array of filenames (possibly with wildcards) to match for action path
+#   triggering_group_ids - array(int64) - Only notify on actions made by a member of one of the specified groups
+#   triggering_user_ids - array(int64) - Only notify on actions made one of the specified users
 #   trigger_by_share_recipients - boolean - Notify when actions are performed by a share recipient?
 #   group_id - int64 - The ID of the group to notify.  Provide `user_id`, `username` or `group_id`.
 #   path - string - Path
 #   username - string - The username of the user to notify.  Provide `user_id`, `username` or `group_id`.
 def create(params=None, options=None):
     if not isinstance(params, dict):
         params = {}
@@ -276,25 +276,25 @@
         "POST", "/notifications", params, options
     )
     return Notification(response.data, options)
 
 
 # Parameters:
 #   notify_on_copy - boolean - If `true`, copying or moving resources into this path will trigger a notification, in addition to just uploads.
-#   notify_on_delete - boolean - Trigger on files deleted in this path?
-#   notify_on_download - boolean - Trigger on files downloaded in this path?
-#   notify_on_move - boolean - Trigger on files moved to this path?
-#   notify_on_upload - boolean - Trigger on files created/uploaded/updated/changed in this path?
+#   notify_on_delete - boolean - Triggers notification when deleting files from this path
+#   notify_on_download - boolean - Triggers notification when downloading files from this path
+#   notify_on_move - boolean - Triggers notification when moving files to this path
+#   notify_on_upload - boolean - Triggers notification when uploading new files to this path
 #   notify_user_actions - boolean - If `true` actions initiated by the user will still result in a notification
 #   recursive - boolean - If `true`, enable notifications for each subfolder in this path
 #   send_interval - string - The time interval that notifications are aggregated by.  Can be `five_minutes`, `fifteen_minutes`, `hourly`, or `daily`.
-#   message - string - Custom message to include in notification emails
-#   triggering_filenames - array(string) - Array of filenames (possibly with wildcards) to scope trigger
-#   triggering_group_ids - array(int64) - If set, will only notify on actions made by a member of one of the specified groups
-#   triggering_user_ids - array(int64) - If set, will onlynotify on actions made one of the specified users
+#   message - string - Custom message to include in notification emails.
+#   triggering_filenames - array(string) - Array of filenames (possibly with wildcards) to match for action path
+#   triggering_group_ids - array(int64) - Only notify on actions made by a member of one of the specified groups
+#   triggering_user_ids - array(int64) - Only notify on actions made one of the specified users
 #   trigger_by_share_recipients - boolean - Notify when actions are performed by a share recipient?
 def update(id, params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     params["id"] = id
```

### Comparing `Files.com-1.4.81/files_sdk/models/payment.py` & `Files.com-1.4.9/files_sdk/models/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         "invoice_line_items": None,  # array - Associated invoice line items
         "method": None,  # string - Line item payment method
         "payment_line_items": None,  # array - Associated payment line items
         "payment_reversed_at": None,  # date-time - Date/time payment was reversed if applicable
         "payment_type": None,  # string - Type of payment if applicable
         "site_name": None,  # string - Site name this line item is for
         "type": None,  # string - Type of line item, either payment or invoice
+        "updated_at": None,  # date-time - Line item updated at
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
             options = {}
```

### Comparing `Files.com-1.4.81/files_sdk/models/payment_line_item.py` & `Files.com-1.4.9/files_sdk/models/payment_line_item.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/permission.py` & `Files.com-1.4.9/files_sdk/models/permission.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/preview.py` & `Files.com-1.4.9/files_sdk/models/preview.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/priority.py` & `Files.com-1.4.9/files_sdk/models/priority.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/project.py` & `Files.com-1.4.9/files_sdk/models/project.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/public_ip_address.py` & `Files.com-1.4.9/files_sdk/models/public_ip_address.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/public_key.py` & `Files.com-1.4.9/files_sdk/models/public_key.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/remote_bandwidth_snapshot.py` & `Files.com-1.4.9/files_sdk/models/usage_daily_snapshot.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,55 +4,61 @@
 from files_sdk.error import (  # noqa: F401
     InvalidParameterError,
     MissingParameterError,
     NotImplementedError,
 )
 
 
-class RemoteBandwidthSnapshot:
+class UsageDailySnapshot:
     default_attributes = {
-        "id": None,  # int64 - Site bandwidth ID
-        "sync_bytes_received": None,  # double - Site sync bandwidth report bytes received
-        "sync_bytes_sent": None,  # double - Site sync bandwidth report bytes sent
-        "logged_at": None,  # date-time - Time the site bandwidth report was logged
-        "remote_server_id": None,  # int64 - ID of related Remote Server
+        "id": None,  # int64 - ID of the usage record
+        "date": None,  # date - The date of this usage record
+        "api_usage_available": None,  # boolean - True if the API usage fields `read_api_usage` and `write_api_usage` can be relied upon.  If this is false, we suggest hiding that value from any UI.
+        "read_api_usage": None,  # int64 - Read API Calls used on this day. Note: only updated for days before the current day.
+        "write_api_usage": None,  # int64 - Write API Calls used on this day. Note: only updated for days before the current day.
+        "user_count": None,  # int64 - Number of billable users as of this day.
+        "current_storage": None,  # int64 - GB of Files Native Storage used on this day.
+        "deleted_files_storage": None,  # int64 - GB of Files Native Storage used on this day for files that have been deleted and are stored as backups.
+        "deleted_files_counted_in_minimum": None,  # int64 - GB of Files Native Storage used on this day for files that have been permanently deleted but were uploaded less than 30 days ago, and are still billable.
+        "root_storage": None,  # int64 - GB of Files Native Storage used for the root folder.  Included here because this value will not be part of `usage_by_top_level_dir`
+        "usage_by_top_level_dir": None,  # object - Usage broken down by each top-level folder
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
             options = {}
         self.set_attributes(attributes)
         self.options = options
 
     def set_attributes(self, attributes):
         for (
             attribute,
             default_value,
-        ) in RemoteBandwidthSnapshot.default_attributes.items():
+        ) in UsageDailySnapshot.default_attributes.items():
             setattr(self, attribute, attributes.get(attribute, default_value))
 
     def get_attributes(self):
         return {
             k: getattr(self, k, None)
-            for k in RemoteBandwidthSnapshot.default_attributes
+            for k in UsageDailySnapshot.default_attributes
             if getattr(self, k, None) is not None
         }
 
 
 # Parameters:
 #   cursor - string - Used for pagination.  When a list request has more records available, cursors are provided in the response headers `X-Files-Cursor-Next` and `X-Files-Cursor-Prev`.  Send one of those cursor value here to resume an existing list from the next available record.  Note: many of our SDKs have iterator methods that will automatically handle cursor-based pagination.
 #   per_page - int64 - Number of records to show per page.  (Max: 10,000, 1,000 or less is recommended).
-#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[logged_at]=desc`). Valid fields are `logged_at`.
-#   filter - object - If set, return records where the specified field is equal to the supplied value. Valid fields are `logged_at`.
-#   filter_gt - object - If set, return records where the specified field is greater than the supplied value. Valid fields are `logged_at`.
-#   filter_gteq - object - If set, return records where the specified field is greater than or equal the supplied value. Valid fields are `logged_at`.
-#   filter_lt - object - If set, return records where the specified field is less than the supplied value. Valid fields are `logged_at`.
-#   filter_lteq - object - If set, return records where the specified field is less than or equal the supplied value. Valid fields are `logged_at`.
+#   sort_by - object - If set, sort records by the specified field in either `asc` or `desc` direction (e.g. `sort_by[date]=desc`). Valid fields are `date` and `usage_snapshot_id`.
+#   filter - object - If set, return records where the specified field is equal to the supplied value. Valid fields are `date` and `usage_snapshot_id`. Valid field combinations are `[ usage_snapshot_id, date ]`.
+#   filter_gt - object - If set, return records where the specified field is greater than the supplied value. Valid fields are `date`.
+#   filter_gteq - object - If set, return records where the specified field is greater than or equal the supplied value. Valid fields are `date`.
+#   filter_lt - object - If set, return records where the specified field is less than the supplied value. Valid fields are `date`.
+#   filter_lteq - object - If set, return records where the specified field is less than or equal the supplied value. Valid fields are `date`.
 def list(params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     if "cursor" in params and not isinstance(params["cursor"], str):
         raise InvalidParameterError("Bad parameter: cursor must be an str")
@@ -71,21 +77,17 @@
     if "filter_lt" in params and not isinstance(params["filter_lt"], dict):
         raise InvalidParameterError("Bad parameter: filter_lt must be an dict")
     if "filter_lteq" in params and not isinstance(params["filter_lteq"], dict):
         raise InvalidParameterError(
             "Bad parameter: filter_lteq must be an dict"
         )
     return ListObj(
-        RemoteBandwidthSnapshot,
-        "GET",
-        "/remote_bandwidth_snapshots",
-        params,
-        options,
+        UsageDailySnapshot, "GET", "/usage_daily_snapshots", params, options
     )
 
 
 def all(params=None, options=None):
     list(params, options)
 
 
 def new(*args, **kwargs):
-    return RemoteBandwidthSnapshot(*args, **kwargs)
+    return UsageDailySnapshot(*args, **kwargs)
```

### Comparing `Files.com-1.4.81/files_sdk/models/remote_server.py` & `Files.com-1.4.9/files_sdk/models/remote_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,17 +42,19 @@
         "rackspace_region": None,  # string - Three letter airport code for Rackspace region. See https://support.rackspace.com/how-to/about-regions/
         "rackspace_container": None,  # string - The name of the container (top level directory) where files will sync.
         "auth_setup_link": None,  # string - Returns link to login with an Oauth provider
         "auth_status": None,  # string - Either `in_setup` or `complete`
         "auth_account_name": None,  # string - Describes the authorized account
         "one_drive_account_type": None,  # string - Either personal or business_other account types
         "azure_blob_storage_account": None,  # string - Azure Blob Storage Account name
+        "azure_blob_storage_sas_token": None,  # string - Shared Access Signature (SAS) token
         "azure_blob_storage_container": None,  # string - Azure Blob Storage Container name
         "azure_blob_storage_hierarchical_namespace": None,  # boolean - Enable when storage account has hierarchical namespace feature enabled
         "azure_files_storage_account": None,  # string - Azure File Storage Account name
+        "azure_files_storage_sas_token": None,  # string - Shared Access Signature (SAS) token
         "azure_files_storage_share_name": None,  # string - Azure File Storage Share name
         "s3_compatible_bucket": None,  # string - S3-compatible Bucket name
         "s3_compatible_endpoint": None,  # string - S3-compatible endpoint
         "s3_compatible_region": None,  # string - S3-compatible endpoint
         "s3_compatible_access_key": None,  # string - S3-compatible Access Key.
         "enable_dedicated_ips": None,  # boolean - `true` if remote server only accepts connections from dedicated IPs
         "files_agent_permission_set": None,  # string - Local permissions for files agent. read_only, write_only, or read_write
@@ -77,15 +79,14 @@
         "wasabi_secret_key": None,  # string - Wasabi secret key.
         "backblaze_b2_key_id": None,  # string - Backblaze B2 Cloud Storage keyID.
         "backblaze_b2_application_key": None,  # string - Backblaze B2 Cloud Storage applicationKey.
         "rackspace_api_key": None,  # string - Rackspace API key from the Rackspace Cloud Control Panel.
         "reset_authentication": None,  # boolean - Reset authenticated account
         "azure_blob_storage_access_key": None,  # string - Azure Blob Storage secret key.
         "azure_files_storage_access_key": None,  # string - Azure File Storage access key.
-        "azure_blob_storage_sas_token": None,  # string - Shared Access Signature (SAS) token
         "s3_compatible_secret_key": None,  # string - S3-compatible secret key
         "filebase_secret_key": None,  # string - Filebase secret key
         "cloudflare_secret_key": None,  # string - Cloudflare secret key
         "linode_secret_key": None,  # string - Linode secret key
     }
 
     def __init__(self, attributes=None, options=None):
@@ -110,24 +111,24 @@
             if getattr(self, k, None) is not None
         }
 
     # Post local changes, check in, and download configuration file (used by some Remote Server integrations, such as the Files.com Agent)
     #
     # Parameters:
     #   api_token - string - Files Agent API Token
-    #   permission_set - string - The permission set for the agent ['read_write', 'read_only', 'write_only']
-    #   root - string - The root directory for the agent
+    #   permission_set - string -
+    #   root - string - Agent local root path
     #   hostname - string
     #   port - int64 - Incoming port for files agent connections
     #   status - string - either running or shutdown
     #   config_version - string - agent config version
-    #   private_key - string - The private key for the agent
+    #   private_key - string - private key
     #   public_key - string - public key
     #   server_host_key - string
-    #   subdomain - string - Files.com subdomain site name
+    #   subdomain - string
     def configuration_file(self, params=None):
         if not isinstance(params, dict):
             params = {}
 
         if hasattr(self, "id") and self.id:
             params["id"] = self.id
         else:
@@ -232,14 +233,15 @@
     #   one_drive_account_type - string - Either personal or business_other account types
     #   azure_blob_storage_account - string - Azure Blob Storage Account name
     #   azure_blob_storage_container - string - Azure Blob Storage Container name
     #   azure_blob_storage_hierarchical_namespace - boolean - Enable when storage account has hierarchical namespace feature enabled
     #   azure_blob_storage_sas_token - string - Shared Access Signature (SAS) token
     #   azure_files_storage_account - string - Azure File Storage Account name
     #   azure_files_storage_share_name - string - Azure File Storage Share name
+    #   azure_files_storage_sas_token - string - Shared Access Signature (SAS) token
     #   s3_compatible_bucket - string - S3-compatible Bucket name
     #   s3_compatible_endpoint - string - S3-compatible endpoint
     #   s3_compatible_region - string - S3-compatible endpoint
     #   enable_dedicated_ips - boolean - `true` if remote server only accepts connections from dedicated IPs
     #   s3_compatible_access_key - string - S3-compatible Access Key.
     #   s3_compatible_secret_key - string - S3-compatible secret key
     #   files_agent_root - string - Agent local root path
@@ -486,14 +488,20 @@
             )
         if "azure_files_storage_share_name" in params and not isinstance(
             params["azure_files_storage_share_name"], str
         ):
             raise InvalidParameterError(
                 "Bad parameter: azure_files_storage_share_name must be an str"
             )
+        if "azure_files_storage_sas_token" in params and not isinstance(
+            params["azure_files_storage_sas_token"], str
+        ):
+            raise InvalidParameterError(
+                "Bad parameter: azure_files_storage_sas_token must be an str"
+            )
         if "s3_compatible_bucket" in params and not isinstance(
             params["s3_compatible_bucket"], str
         ):
             raise InvalidParameterError(
                 "Bad parameter: s3_compatible_bucket must be an str"
             )
         if "s3_compatible_endpoint" in params and not isinstance(
@@ -747,14 +755,15 @@
 #   one_drive_account_type - string - Either personal or business_other account types
 #   azure_blob_storage_account - string - Azure Blob Storage Account name
 #   azure_blob_storage_container - string - Azure Blob Storage Container name
 #   azure_blob_storage_hierarchical_namespace - boolean - Enable when storage account has hierarchical namespace feature enabled
 #   azure_blob_storage_sas_token - string - Shared Access Signature (SAS) token
 #   azure_files_storage_account - string - Azure File Storage Account name
 #   azure_files_storage_share_name - string - Azure File Storage Share name
+#   azure_files_storage_sas_token - string - Shared Access Signature (SAS) token
 #   s3_compatible_bucket - string - S3-compatible Bucket name
 #   s3_compatible_endpoint - string - S3-compatible endpoint
 #   s3_compatible_region - string - S3-compatible endpoint
 #   enable_dedicated_ips - boolean - `true` if remote server only accepts connections from dedicated IPs
 #   s3_compatible_access_key - string - S3-compatible Access Key.
 #   s3_compatible_secret_key - string - S3-compatible secret key
 #   files_agent_root - string - Agent local root path
@@ -977,14 +986,20 @@
         )
     if "azure_files_storage_share_name" in params and not isinstance(
         params["azure_files_storage_share_name"], str
     ):
         raise InvalidParameterError(
             "Bad parameter: azure_files_storage_share_name must be an str"
         )
+    if "azure_files_storage_sas_token" in params and not isinstance(
+        params["azure_files_storage_sas_token"], str
+    ):
+        raise InvalidParameterError(
+            "Bad parameter: azure_files_storage_sas_token must be an str"
+        )
     if "s3_compatible_bucket" in params and not isinstance(
         params["s3_compatible_bucket"], str
     ):
         raise InvalidParameterError(
             "Bad parameter: s3_compatible_bucket must be an str"
         )
     if "s3_compatible_endpoint" in params and not isinstance(
@@ -1101,24 +1116,24 @@
     return RemoteServer(response.data, options)
 
 
 # Post local changes, check in, and download configuration file (used by some Remote Server integrations, such as the Files.com Agent)
 #
 # Parameters:
 #   api_token - string - Files Agent API Token
-#   permission_set - string - The permission set for the agent ['read_write', 'read_only', 'write_only']
-#   root - string - The root directory for the agent
+#   permission_set - string -
+#   root - string - Agent local root path
 #   hostname - string
 #   port - int64 - Incoming port for files agent connections
 #   status - string - either running or shutdown
 #   config_version - string - agent config version
-#   private_key - string - The private key for the agent
+#   private_key - string - private key
 #   public_key - string - public key
 #   server_host_key - string
-#   subdomain - string - Files.com subdomain site name
+#   subdomain - string
 def configuration_file(id, params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     params["id"] = id
     if "id" in params and not isinstance(params["id"], int):
@@ -1210,14 +1225,15 @@
 #   one_drive_account_type - string - Either personal or business_other account types
 #   azure_blob_storage_account - string - Azure Blob Storage Account name
 #   azure_blob_storage_container - string - Azure Blob Storage Container name
 #   azure_blob_storage_hierarchical_namespace - boolean - Enable when storage account has hierarchical namespace feature enabled
 #   azure_blob_storage_sas_token - string - Shared Access Signature (SAS) token
 #   azure_files_storage_account - string - Azure File Storage Account name
 #   azure_files_storage_share_name - string - Azure File Storage Share name
+#   azure_files_storage_sas_token - string - Shared Access Signature (SAS) token
 #   s3_compatible_bucket - string - S3-compatible Bucket name
 #   s3_compatible_endpoint - string - S3-compatible endpoint
 #   s3_compatible_region - string - S3-compatible endpoint
 #   enable_dedicated_ips - boolean - `true` if remote server only accepts connections from dedicated IPs
 #   s3_compatible_access_key - string - S3-compatible Access Key.
 #   s3_compatible_secret_key - string - S3-compatible secret key
 #   files_agent_root - string - Agent local root path
@@ -1443,14 +1459,20 @@
         )
     if "azure_files_storage_share_name" in params and not isinstance(
         params["azure_files_storage_share_name"], str
     ):
         raise InvalidParameterError(
             "Bad parameter: azure_files_storage_share_name must be an str"
         )
+    if "azure_files_storage_sas_token" in params and not isinstance(
+        params["azure_files_storage_sas_token"], str
+    ):
+        raise InvalidParameterError(
+            "Bad parameter: azure_files_storage_sas_token must be an str"
+        )
     if "s3_compatible_bucket" in params and not isinstance(
         params["s3_compatible_bucket"], str
     ):
         raise InvalidParameterError(
             "Bad parameter: s3_compatible_bucket must be an str"
         )
     if "s3_compatible_endpoint" in params and not isinstance(
```

### Comparing `Files.com-1.4.81/files_sdk/models/remote_server_configuration_file.py` & `Files.com-1.4.9/files_sdk/models/session.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,70 +3,98 @@
 from files_sdk.error import (  # noqa: F401
     InvalidParameterError,
     MissingParameterError,
     NotImplementedError,
 )
 
 
-class RemoteServerConfigurationFile:
+class Session:
     default_attributes = {
-        "id": None,  # int64 - The remote server ID of the agent
-        "permission_set": None,  # string - The permission set for the agent ['read_write', 'read_only', 'write_only']
-        "private_key": None,  # string - The private key for the agent
-        "subdomain": None,  # string - Files.com subdomain site name
-        "root": None,  # string - The root directory for the agent
-        "follow_links": None,  # boolean - Follow symlinks when traversing directories
-        "prefer_protocol": None,  # string - Preferred network protocol ['udp', 'tcp']
-        "dns": None,  # string - DNS lookup method ['auto','doh','system']
-        "proxy_all_outbound": None,  # boolean - Proxy all outbound traffic through files.com proxy server
-        "endpoint_override": None,  # string - Custom site endpoint URL
-        "log_file": None,  # string - Log file name and location
-        "log_level": None,  # string - Log level for the agent logs ['debug', 'info', 'warn', 'error', 'fatal']
-        "log_rotate_num": None,  # int64 - Log route for agent logs. (default 5)
-        "log_rotate_size": None,  # int64 - Log route size in MB for agent logs. (default 20MB)
-        "max_concurrent_jobs": None,  # int64 - Maximum number of concurrent jobs (default CPU Count * 4)
-        "graceful_shutdown_timeout": None,  # int64 - Graceful shutdown timeout in seconds
-        "transfer_rate_limit": None,  # string - File transfer (upload/download) rate limit
-        #  `<limit>-<period>`, with the given periods:
-        # * 'S': second
-        # * 'M': minute
-        # * 'H': hour
-        # * 'D': day
-        # Examples:
-        # * 5 requests/second: '5-S'
-        # * 10 requests/minute: '10-M'
-        # * 1000 requests/hour: '1000-H'
-        # * 2000 requests/day: '2000-D'
-        "api_token": None,  # string - Files Agent API Token
-        "port": None,  # int64 - Incoming port for files agent connections
-        "hostname": None,  # string
-        "public_key": None,  # string - public key
-        "status": None,  # string - either running or shutdown
-        "server_host_key": None,  # string
-        "config_version": None,  # string - agent config version
+        "id": None,  # string - Session ID
+        "language": None,  # string - Session language
+        "read_only": None,  # boolean - Is this session read only?
+        "sftp_insecure_ciphers": None,  # boolean - Are insecure SFTP ciphers allowed for this user? (If this is set to true, the site administrator has signaled that it is ok to use less secure SSH ciphers for this user.)
+        "username": None,  # string - Username to sign in as
+        "password": None,  # string - Password for sign in
+        "otp": None,  # string - If this user has a 2FA device, provide its OTP or code here.
+        "partial_session_id": None,  # string - Identifier for a partially-completed login
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
             options = {}
         self.set_attributes(attributes)
         self.options = options
 
     def set_attributes(self, attributes):
-        for (
-            attribute,
-            default_value,
-        ) in RemoteServerConfigurationFile.default_attributes.items():
+        for attribute, default_value in Session.default_attributes.items():
             setattr(self, attribute, attributes.get(attribute, default_value))
 
     def get_attributes(self):
         return {
             k: getattr(self, k, None)
-            for k in RemoteServerConfigurationFile.default_attributes
+            for k in Session.default_attributes
             if getattr(self, k, None) is not None
         }
 
+    def destroy(self, params=None, options=None):
+        if not isinstance(params, dict):
+            params = {}
+        if not isinstance(options, dict):
+            options = {}
+        options.pop("session_id", None)
+        options["session"] = self
+        Session.destroy(params, options)
+
+    def save(self):
+        if hasattr(self, "id") and self.id:
+            raise NotImplementedError(
+                "The Session object doesn't support updates."
+            )
+        else:
+            new_obj = create(self.get_attributes(), self.options)
+            self.set_attributes(new_obj.get_attributes())
+            return True
+
+
+# Parameters:
+#   username - string - Username to sign in as
+#   password - string - Password for sign in
+#   otp - string - If this user has a 2FA device, provide its OTP or code here.
+#   partial_session_id - string - Identifier for a partially-completed login
+def create(params=None, options=None):
+    if not isinstance(params, dict):
+        params = {}
+    if not isinstance(options, dict):
+        options = {}
+    if "username" in params and not isinstance(params["username"], str):
+        raise InvalidParameterError("Bad parameter: username must be an str")
+    if "password" in params and not isinstance(params["password"], str):
+        raise InvalidParameterError("Bad parameter: password must be an str")
+    if "otp" in params and not isinstance(params["otp"], str):
+        raise InvalidParameterError("Bad parameter: otp must be an str")
+    if "partial_session_id" in params and not isinstance(
+        params["partial_session_id"], str
+    ):
+        raise InvalidParameterError(
+            "Bad parameter: partial_session_id must be an str"
+        )
+    response, options = Api.send_request("POST", "/sessions", params, options)
+    return Session(response.data, options)
+
+
+def delete(params=None, options=None):
+    if not isinstance(params, dict):
+        params = {}
+    if not isinstance(options, dict):
+        options = {}
+    Api.send_request("DELETE", "/sessions", params, options)
+
+
+def destroy(params=None, options=None):
+    delete(params, options)
+
 
 def new(*args, **kwargs):
-    return RemoteServerConfigurationFile(*args, **kwargs)
+    return Session(*args, **kwargs)
```

### Comparing `Files.com-1.4.81/files_sdk/models/request.py` & `Files.com-1.4.9/files_sdk/models/request.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/settings_change.py` & `Files.com-1.4.9/files_sdk/models/settings_change.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/sftp_host_key.py` & `Files.com-1.4.9/files_sdk/models/sftp_host_key.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/share_group.py` & `Files.com-1.4.9/files_sdk/models/share_group.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/share_group_member.py` & `Files.com-1.4.9/files_sdk/models/share_group_member.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/site.py` & `Files.com-1.4.9/files_sdk/models/site.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,25 @@
     NotImplementedError,
 )
 
 
 class Site:
     default_attributes = {
         "name": None,  # string - Site name
-        "additional_text_file_types": None,  # array - Additional extensions that are considered text files
         "allowed_2fa_method_sms": None,  # boolean - Is SMS two factor authentication allowed?
         "allowed_2fa_method_totp": None,  # boolean - Is TOTP two factor authentication allowed?
         "allowed_2fa_method_u2f": None,  # boolean - Is U2F two factor authentication allowed?
         "allowed_2fa_method_webauthn": None,  # boolean - Is WebAuthn two factor authentication allowed?
         "allowed_2fa_method_yubi": None,  # boolean - Is yubikey two factor authentication allowed?
-        "allowed_2fa_method_email": None,  # boolean - Is OTP via email two factor authentication allowed?
-        "allowed_2fa_method_static": None,  # boolean - Is OTP via static codes for two factor authentication allowed?
         "allowed_2fa_method_bypass_for_ftp_sftp_dav": None,  # boolean - Are users allowed to configure their two factor authentication to be bypassed for FTP/SFTP/WebDAV?
         "admin_user_id": None,  # int64 - User ID for the main site administrator
         "admins_bypass_locked_subfolders": None,  # boolean - Allow admins to bypass the locked subfolders setting.
         "allow_bundle_names": None,  # boolean - Are manual Bundle names allowed?
         "allowed_countries": None,  # string - Comma seperated list of allowed Country codes
         "allowed_ips": None,  # string - List of allowed IP addresses
-        "always_mkdir_parents": None,  # boolean - Create parent directories if they do not exist during uploads?  This is primarily used to work around broken upload clients that assume servers will perform this step.
         "ask_about_overwrites": None,  # boolean - If false, rename conflicting files instead of asking for overwrite confirmation.  Only applies to web interface.
         "bundle_activity_notifications": None,  # string - Do Bundle owners receive activity notifications?
         "bundle_expiration": None,  # int64 - Site-wide Bundle expiration in days
         "bundle_not_found_message": None,  # string - Custom error message to show when bundle is not found.
         "bundle_password_required": None,  # boolean - Do Bundles require password protection?
         "bundle_recipient_blacklist_domains": None,  # array - List of email domains to disallow when entering a Bundle/Inbox recipients
         "bundle_recipient_blacklist_free_email_domains": None,  # boolean - Disallow free email domains for Bundle/Inbox recipients?
@@ -45,16 +41,14 @@
         "color2_text": None,  # string - Page link and button color
         "color2_top": None,  # string - Top bar background color
         "color2_top_text": None,  # string - Top bar text color
         "contact_name": None,  # string - Site main contact name
         "created_at": None,  # date-time - Time this site was created
         "currency": None,  # string - Preferred currency
         "custom_namespace": None,  # boolean - Is this site using a custom namespace for users?
-        "dav_enabled": None,  # boolean - Is WebDAV enabled?
-        "dav_user_root_enabled": None,  # boolean - Use user FTP roots also for WebDAV?
         "days_to_retain_backups": None,  # int64 - Number of days to keep deleted files
         "default_time_zone": None,  # string - Site default time zone
         "desktop_app": None,  # boolean - Is the desktop app enabled?
         "desktop_app_session_ip_pinning": None,  # boolean - Is desktop app session IP pinning enabled?
         "desktop_app_session_lifetime": None,  # int64 - Desktop app session lifetime (in hours)
         "mobile_app": None,  # boolean - Is the mobile app enabled?
         "mobile_app_session_ip_pinning": None,  # boolean - Is mobile app session IP pinning enabled?
@@ -117,26 +111,24 @@
         "password_require_special": None,  # boolean - Require special characters in password?
         "password_require_unbreached": None,  # boolean - Require passwords that have not been previously breached? (see https://haveibeenpwned.com/)
         "password_requirements_apply_to_bundles": None,  # boolean - Require bundles' passwords, and passwords for other items (inboxes, public shares, etc.) to conform to the same requirements as users' passwords?
         "password_validity_days": None,  # int64 - Number of days password is valid
         "phone": None,  # string - Site phone number
         "pin_all_remote_servers_to_site_region": None,  # boolean - If true, we will ensure that all internal communications with any remote server are made through the primary region of the site. This setting overrides individual remote server settings.
         "prevent_root_permissions_for_non_site_admins": None,  # boolean - If true, we will prevent non-administrators from receiving any permissions directly on the root folder.  This is commonly used to prevent the accidental application of permissions.
-        "protocol_access_groups_only": None,  # boolean - If true, protocol access permissions on users will be ignored, and only protocol access permissions set on Groups will be honored.  Make sure that your current user is a member of a group with API permission when changing this value to avoid locking yourself out of your site.
         "require_2fa": None,  # boolean - Require two-factor authentication for all users?
         "require_2fa_stop_time": None,  # date-time - If set, requirement for two-factor authentication has been scheduled to end on this date-time.
         "require_2fa_user_type": None,  # string - What type of user is required to use two-factor authentication (when require_2fa is set to `true` for this site)?
         "require_logout_from_bundles_and_inboxes": None,  # boolean - If true, we will hide the 'Remember Me' box on Inbox and Bundle registration pages, requiring that the user logout and log back in every time they visit the page.
         "session": None,  # Session - Current session
         "session_pinned_by_ip": None,  # boolean - Are sessions locked to the same IP? (i.e. do users need to log in again if they change IPs?)
         "sftp_enabled": None,  # boolean - Is SFTP enabled?
         "sftp_host_key_type": None,  # string - Sftp Host Key Type
         "active_sftp_host_key_id": None,  # int64 - Id of the currently selected custom SFTP Host Key
-        "sftp_insecure_ciphers": None,  # boolean - If true, we will allow weak and known insecure ciphers to be used for SFTP connections.  Enabling this setting severly weakens the security of your site and it is not recommend, except as a last resort for compatibility.
-        "sftp_insecure_diffie_hellman": None,  # boolean - If true, we will allow weak Diffie Hellman parameters to be used within ciphers for SFTP that are otherwise on our secure list.  This has the effect of making the cipher weaker than our normal threshold for security, but is required to support certain legacy or broken SSH and MFT clients.  Enabling this weakens security, but not nearly as much as enabling the full `sftp_insecure_ciphers` option.
+        "sftp_insecure_ciphers": None,  # boolean - Are Insecure Ciphers allowed for SFTP?  Note:  Settting TLS Disabled -> True will always allow insecure ciphers for SFTP as well.  Enabling this is insecure.
         "sftp_user_root_enabled": None,  # boolean - Use user FTP roots also for SFTP?
         "sharing_enabled": None,  # boolean - Allow bundle creation
         "show_request_access_link": None,  # boolean - Show request access link for users without access?  Currently unused.
         "site_footer": None,  # string - Custom site footer text
         "site_header": None,  # string - Custom site header text
         "smtp_address": None,  # string - SMTP server hostname or IP
         "smtp_authentication": None,  # string - SMTP server authentication type
@@ -144,27 +136,26 @@
         "smtp_port": None,  # int64 - SMTP server port
         "smtp_username": None,  # string - SMTP server username
         "session_expiry": None,  # double - Session expiry in hours
         "session_expiry_minutes": None,  # int64 - Session expiry in minutes
         "ssl_required": None,  # boolean - Is SSL required?  Disabling this is insecure.
         "subdomain": None,  # string - Site subdomain
         "switch_to_plan_date": None,  # date-time - If switching plans, when does the new plan take effect?
-        "tls_disabled": None,  # boolean - DO NOT ENABLE. This setting allows TLSv1.0 and TLSv1.1 to be used on your site.  We intend to remove this capability entirely in early 2024.  If set, the `sftp_insecure_ciphers` flag will be automatically set to true.
+        "tls_disabled": None,  # boolean - Are Insecure TLS and SFTP Ciphers allowed?  Enabling this is insecure.
         "trial_days_left": None,  # int64 - Number of days left in trial
         "trial_until": None,  # date-time - When does this Site trial expire?
+        "updated_at": None,  # date-time - Last time this Site was updated
         "use_provided_modified_at": None,  # boolean - Allow uploaders to set `provided_modified_at` for uploaded files?
         "user": None,  # User - User of current session
         "user_lockout": None,  # boolean - Will users be locked out after incorrect login attempts?
         "user_lockout_lock_period": None,  # int64 - How many hours to lock user out for failed password?
         "user_lockout_tries": None,  # int64 - Number of login tries within `user_lockout_within` hours before users are locked out
         "user_lockout_within": None,  # int64 - Number of hours for user lockout window
         "user_requests_enabled": None,  # boolean - Enable User Requests feature
         "user_requests_notify_admins": None,  # boolean - Send email to site admins when a user request is received?
-        "users_can_create_api_keys": None,  # boolean - Allow users to create their own API keys?
-        "users_can_create_ssh_keys": None,  # boolean - Allow users to create their own SSH keys?
         "welcome_custom_text": None,  # string - Custom text send in user welcome email
         "welcome_email_cc": None,  # email - Include this email in welcome emails if enabled
         "welcome_email_subject": None,  # string - Include this email subject in welcome emails if enabled
         "welcome_email_enabled": None,  # boolean - Will the welcome email be sent to new users?
         "welcome_screen": None,  # string - Does the welcome screen appear?
         "windows_mode_ftp": None,  # boolean - Does FTP user Windows emulation mode?
         "disable_users_from_inactivity_period_days": None,  # int64 - If greater than zero, users will unable to login if they do not show activity within this number of days.
@@ -218,15 +209,14 @@
 #   email - string - Main email for this site
 #   reply_to_email - string - Reply-to email for this site
 #   allow_bundle_names - boolean - Are manual Bundle names allowed?
 #   bundle_expiration - int64 - Site-wide Bundle expiration in days
 #   welcome_email_enabled - boolean - Will the welcome email be sent to new users?
 #   ask_about_overwrites - boolean - If false, rename conflicting files instead of asking for overwrite confirmation.  Only applies to web interface.
 #   show_request_access_link - boolean - Show request access link for users without access?  Currently unused.
-#   always_mkdir_parents - boolean - Create parent directories if they do not exist during uploads?  This is primarily used to work around broken upload clients that assume servers will perform this step.
 #   welcome_email_cc - string - Include this email in welcome emails if enabled
 #   welcome_email_subject - string - Include this email subject in welcome emails if enabled
 #   welcome_custom_text - string - Custom text send in user welcome email
 #   language - string - Site default language
 #   windows_mode_ftp - boolean - Does FTP user Windows emulation mode?
 #   default_time_zone - string - Site default time zone
 #   desktop_app - boolean - Is the desktop app enabled?
@@ -239,21 +229,18 @@
 #   welcome_screen - string - Does the welcome screen appear?
 #   office_integration_available - boolean - Allow users to use Office for the web?
 #   office_integration_type - string - Office integration application used to edit and view the MS Office documents
 #   pin_all_remote_servers_to_site_region - boolean - If true, we will ensure that all internal communications with any remote server are made through the primary region of the site. This setting overrides individual remote server settings.
 #   motd_text - string - A message to show users when they connect via FTP or SFTP.
 #   motd_use_for_ftp - boolean - Show message to users connecting via FTP
 #   motd_use_for_sftp - boolean - Show message to users connecting via SFTP
-#   left_navigation_visibility - object - Visibility settings for account navigation
-#   additional_text_file_types - array(string) - Additional extensions that are considered text files
 #   session_expiry - double - Session expiry in hours
 #   ssl_required - boolean - Is SSL required?  Disabling this is insecure.
-#   tls_disabled - boolean - DO NOT ENABLE. This setting allows TLSv1.0 and TLSv1.1 to be used on your site.  We intend to remove this capability entirely in early 2024.  If set, the `sftp_insecure_ciphers` flag will be automatically set to true.
-#   sftp_insecure_ciphers - boolean - If true, we will allow weak and known insecure ciphers to be used for SFTP connections.  Enabling this setting severly weakens the security of your site and it is not recommend, except as a last resort for compatibility.
-#   sftp_insecure_diffie_hellman - boolean - If true, we will allow weak Diffie Hellman parameters to be used within ciphers for SFTP that are otherwise on our secure list.  This has the effect of making the cipher weaker than our normal threshold for security, but is required to support certain legacy or broken SSH and MFT clients.  Enabling this weakens security, but not nearly as much as enabling the full `sftp_insecure_ciphers` option.
+#   tls_disabled - boolean - Are Insecure TLS and SFTP Ciphers allowed?  Enabling this is insecure.
+#   sftp_insecure_ciphers - boolean - Are Insecure Ciphers allowed for SFTP?  Note:  Settting TLS Disabled -> True will always allow insecure ciphers for SFTP as well.  Enabling this is insecure.
 #   disable_files_certificate_generation - boolean - If set, Files.com will not set the CAA records required to generate future SSL certificates for this domain.
 #   user_lockout - boolean - Will users be locked out after incorrect login attempts?
 #   user_lockout_tries - int64 - Number of login tries within `user_lockout_within` hours before users are locked out
 #   user_lockout_within - int64 - Number of hours for user lockout window
 #   user_lockout_lock_period - int64 - How many hours to lock user out for failed password?
 #   include_password_in_welcome_email - boolean - Include password in emails to new users?
 #   allowed_countries - string - Comma seperated list of allowed Country codes
@@ -265,15 +252,14 @@
 #   password_min_length - int64 - Shortest password length for users
 #   password_require_letter - boolean - Require a letter in passwords?
 #   password_require_mixed - boolean - Require lower and upper case letters in passwords?
 #   password_require_special - boolean - Require special characters in password?
 #   password_require_number - boolean - Require a number in passwords?
 #   password_require_unbreached - boolean - Require passwords that have not been previously breached? (see https://haveibeenpwned.com/)
 #   require_logout_from_bundles_and_inboxes - boolean - If true, we will hide the 'Remember Me' box on Inbox and Bundle registration pages, requiring that the user logout and log back in every time they visit the page.
-#   dav_user_root_enabled - boolean - Use user FTP roots also for WebDAV?
 #   sftp_user_root_enabled - boolean - Use user FTP roots also for SFTP?
 #   disable_password_reset - boolean - Is password reset disabled?
 #   immutable_files - boolean - Are files protected from modification?
 #   session_pinned_by_ip - boolean - Are sessions locked to the same IP? (i.e. do users need to log in again if they change IPs?)
 #   bundle_not_found_message - string - Custom error message to show when bundle is not found.
 #   bundle_password_required - boolean - Do Bundles require password protection?
 #   bundle_require_registration - boolean - Do Bundles require registration?
@@ -288,34 +274,29 @@
 #   custom_namespace - boolean - Is this site using a custom namespace for users?
 #   disable_users_from_inactivity_period_days - int64 - If greater than zero, users will unable to login if they do not show activity within this number of days.
 #   non_sso_groups_allowed - boolean - If true, groups can be manually created / modified / deleted by Site Admins. Otherwise, groups can only be managed via your SSO provider.
 #   non_sso_users_allowed - boolean - If true, users can be manually created / modified / deleted by Site Admins. Otherwise, users can only be managed via your SSO provider.
 #   sharing_enabled - boolean - Allow bundle creation
 #   user_requests_enabled - boolean - Enable User Requests feature
 #   user_requests_notify_admins - boolean - Send email to site admins when a user request is received?
-#   dav_enabled - boolean - Is WebDAV enabled?
 #   ftp_enabled - boolean - Is FTP enabled?
 #   sftp_enabled - boolean - Is SFTP enabled?
-#   users_can_create_api_keys - boolean - Allow users to create their own API keys?
-#   users_can_create_ssh_keys - boolean - Allow users to create their own SSH keys?
 #   sftp_host_key_type - string - Sftp Host Key Type
 #   active_sftp_host_key_id - int64 - Id of the currently selected custom SFTP Host Key
-#   protocol_access_groups_only - boolean - If true, protocol access permissions on users will be ignored, and only protocol access permissions set on Groups will be honored.  Make sure that your current user is a member of a group with API permission when changing this value to avoid locking yourself out of your site.
+#   protocol_access_groups_only - boolean - If `true`, protocol access permissions on users will be ignored, and only protocol access permissions set on Groups will be honored.  Make sure that your current user is a member of a group with API permission when changing this value to avoid locking yourself out of your site.
 #   bundle_watermark_value - object - Preview watermark settings applied to all bundle items. Uses the same keys as Behavior.value
 #   group_admins_can_set_user_password - boolean - Allow group admins set password authentication method
 #   bundle_recipient_blacklist_free_email_domains - boolean - Disallow free email domains for Bundle/Inbox recipients?
 #   bundle_recipient_blacklist_domains - array(string) - List of email domains to disallow when entering a Bundle/Inbox recipients
 #   admins_bypass_locked_subfolders - boolean - Allow admins to bypass the locked subfolders setting.
 #   allowed_2fa_method_sms - boolean - Is SMS two factor authentication allowed?
 #   allowed_2fa_method_u2f - boolean - Is U2F two factor authentication allowed?
 #   allowed_2fa_method_totp - boolean - Is TOTP two factor authentication allowed?
 #   allowed_2fa_method_webauthn - boolean - Is WebAuthn two factor authentication allowed?
 #   allowed_2fa_method_yubi - boolean - Is yubikey two factor authentication allowed?
-#   allowed_2fa_method_email - boolean - Is OTP via email two factor authentication allowed?
-#   allowed_2fa_method_static - boolean - Is OTP via static codes for two factor authentication allowed?
 #   allowed_2fa_method_bypass_for_ftp_sftp_dav - boolean - Are users allowed to configure their two factor authentication to be bypassed for FTP/SFTP/WebDAV?
 #   require_2fa - boolean - Require two-factor authentication for all users?
 #   require_2fa_user_type - string - What type of user is required to use two-factor authentication (when require_2fa is set to `true` for this site)?
 #   color2_top - string - Top bar background color
 #   color2_left - string - Page link and button color
 #   color2_link - string - Top bar link color
 #   color2_text - string - Page link and button color
@@ -443,26 +424,14 @@
         params["office_integration_type"], str
     ):
         raise InvalidParameterError(
             "Bad parameter: office_integration_type must be an str"
         )
     if "motd_text" in params and not isinstance(params["motd_text"], str):
         raise InvalidParameterError("Bad parameter: motd_text must be an str")
-    if "left_navigation_visibility" in params and not isinstance(
-        params["left_navigation_visibility"], dict
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: left_navigation_visibility must be an dict"
-        )
-    if "additional_text_file_types" in params and not isinstance(
-        params["additional_text_file_types"], builtins.list
-    ):
-        raise InvalidParameterError(
-            "Bad parameter: additional_text_file_types must be an list"
-        )
     if "session_expiry" in params and not isinstance(
         params["session_expiry"], float
     ):
         raise InvalidParameterError(
             "Bad parameter: session_expiry must be an float"
         )
     if "user_lockout_tries" in params and not isinstance(
```

### Comparing `Files.com-1.4.81/files_sdk/models/snapshot.py` & `Files.com-1.4.9/files_sdk/models/snapshot.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,34 +34,14 @@
     def get_attributes(self):
         return {
             k: getattr(self, k, None)
             for k in Snapshot.default_attributes
             if getattr(self, k, None) is not None
         }
 
-    # Finalize Snapshot
-    def finalize(self, params=None):
-        if not isinstance(params, dict):
-            params = {}
-
-        if hasattr(self, "id") and self.id:
-            params["id"] = self.id
-        else:
-            raise MissingParameterError("Current object doesn't have a id")
-        if "id" not in params:
-            raise MissingParameterError("Parameter missing: id")
-        if "id" in params and not isinstance(params["id"], int):
-            raise InvalidParameterError("Bad parameter: id must be an int")
-        Api.send_request(
-            "POST",
-            "/snapshots/{id}/finalize".format(id=params["id"]),
-            params,
-            self.options,
-        )
-
     # Parameters:
     #   expires_at - string - When the snapshot expires.
     #   name - string - A name for the snapshot.
     #   paths - array(string) - An array of paths to add to the snapshot.
     def update(self, params=None):
         if not isinstance(params, dict):
             params = {}
@@ -183,33 +163,14 @@
         raise InvalidParameterError("Bad parameter: name must be an str")
     if "paths" in params and not isinstance(params["paths"], builtins.list):
         raise InvalidParameterError("Bad parameter: paths must be an list")
     response, options = Api.send_request("POST", "/snapshots", params, options)
     return Snapshot(response.data, options)
 
 
-# Finalize Snapshot
-def finalize(id, params=None, options=None):
-    if not isinstance(params, dict):
-        params = {}
-    if not isinstance(options, dict):
-        options = {}
-    params["id"] = id
-    if "id" in params and not isinstance(params["id"], int):
-        raise InvalidParameterError("Bad parameter: id must be an int")
-    if "id" not in params:
-        raise MissingParameterError("Parameter missing: id")
-    Api.send_request(
-        "POST",
-        "/snapshots/{id}/finalize".format(id=params["id"]),
-        params,
-        options,
-    )
-
-
 # Parameters:
 #   expires_at - string - When the snapshot expires.
 #   name - string - A name for the snapshot.
 #   paths - array(string) - An array of paths to add to the snapshot.
 def update(id, params=None, options=None):
     if not isinstance(params, dict):
         params = {}
```

### Comparing `Files.com-1.4.81/files_sdk/models/status.py` & `Files.com-1.4.9/files_sdk/models/status.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/style.py` & `Files.com-1.4.9/files_sdk/models/style.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/usage_snapshot.py` & `Files.com-1.4.9/files_sdk/models/usage_snapshot.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/user.py` & `Files.com-1.4.9/files_sdk/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,15 @@
         "authentication_method": None,  # string - How is this user authenticated?
         "avatar_url": None,  # string - URL holding the user's avatar
         "billing_permission": None,  # boolean - Allow this user to perform operations on the account, payments, and invoices?
         "bypass_site_allowed_ips": None,  # boolean - Allow this user to skip site-wide IP blacklists?
         "bypass_inactive_disable": None,  # boolean - Exempt this user from being disabled based on inactivity?
         "created_at": None,  # date-time - When this user was created
         "dav_permission": None,  # boolean - Can the user connect with WebDAV?
-        "disabled": None,  # boolean - Is user disabled? Disabled users cannot log in, and do not count for billing purposes. Users can be automatically disabled after an inactivity period via a Site setting or schedule to be deactivated after specific date.
-        "disabled_expired_or_inactive": None,  # boolean - Computed property that returns true if user disabled or expired or inactive.
+        "disabled": None,  # boolean - Is user disabled? Disabled users cannot log in, and do not count for billing purposes.  Users can be automatically disabled after an inactivity period via a Site setting.
         "email": None,  # email - User email address
         "first_login_at": None,  # date-time - User's first login time
         "ftp_permission": None,  # boolean - Can the user access with FTP/FTPS?
         "group_ids": None,  # string - Comma-separated list of group IDs of which this user is a member
         "header_text": None,  # string - Text to display to the user in the header of the UI
         "language": None,  # string - Preferred language
         "last_login_at": None,  # date-time - User's most recent login time via any protocol
@@ -53,26 +52,25 @@
         "public_keys_count": None,  # int64 - Number of public keys associated with this user
         "receive_admin_alerts": None,  # boolean - Should the user receive admin alerts such a certificate expiration notifications and overages?
         "require_2fa": None,  # string - 2FA required setting
         "require_login_by": None,  # date-time - Require user to login by specified date otherwise it will be disabled.
         "active_2fa": None,  # boolean - Is 2fa active for the user?
         "require_password_change": None,  # boolean - Is a password change required upon next user login?
         "password_expired": None,  # boolean - Is user's password expired?
-        "restapi_permission": None,  # boolean - Can this user access the Web app, Desktop app, SDKs, or REST API?  (All of these tools use the API internally, so this is one unified permission set.)
+        "restapi_permission": None,  # boolean - Can this user access the REST API?
         "self_managed": None,  # boolean - Does this user manage it's own credentials or is it a shared/bot user?
         "sftp_permission": None,  # boolean - Can the user access with SFTP?
         "site_admin": None,  # boolean - Is the user an administrator for this site?
         "skip_welcome_screen": None,  # boolean - Skip Welcome page in the UI?
         "ssl_required": None,  # string - SSL required setting
         "sso_strategy_id": None,  # int64 - SSO (Single Sign On) strategy ID for the user, if applicable.
         "subscribe_to_newsletter": None,  # boolean - Is the user subscribed to the newsletter?
         "externally_managed": None,  # boolean - Is this user managed by a SsoStrategy?
         "time_zone": None,  # string - User time zone
-        "type_of_2fa": None,  # string - Type(s) of 2FA methods in use, for programmatic use.  Will be either `sms`, `totp`, `u2f`, `yubi`, or multiple values sorted alphabetically and joined by an underscore.  Does not specify whether user has more than one of a given method.
-        "type_of_2fa_for_display": None,  # string - Type(s) of 2FA methods in use, formatted for displaying in the UI.  Unlike `type_of_2fa`, this value will make clear when a user has more than 1 of the same type of method.
+        "type_of_2fa": None,  # string - Type(s) of 2FA methods in use.  Will be either `sms`, `totp`, `u2f`, `yubi`, or multiple values sorted alphabetically and joined by an underscore.
         "user_root": None,  # string - Root folder for FTP (and optionally SFTP if the appropriate site-wide setting is set.)  Note that this is not used for API, Desktop, or Web interface.
         "days_remaining_until_password_expire": None,  # int64 - Number of days remaining until password expires
         "password_expire_at": None,  # date-time - Password expiration datetime
         "avatar_file": None,  # file - An image file for your user avatar.
         "avatar_delete": None,  # boolean - If true, the avatar will be deleted.
         "change_password": None,  # string - Used for changing a password on an existing user.
         "change_password_confirmation": None,  # string - Optional, but if provided, we will ensure that it matches the value sent in `change_password`.
@@ -180,28 +178,28 @@
     #   attachments_permission - boolean - DEPRECATED: Can the user create Bundles (aka Share Links)? Use the bundle permission instead.
     #   authenticate_until - string - Scheduled Date/Time at which user will be deactivated
     #   authentication_method - string - How is this user authenticated?
     #   billing_permission - boolean - Allow this user to perform operations on the account, payments, and invoices?
     #   bypass_inactive_disable - boolean - Exempt this user from being disabled based on inactivity?
     #   bypass_site_allowed_ips - boolean - Allow this user to skip site-wide IP blacklists?
     #   dav_permission - boolean - Can the user connect with WebDAV?
-    #   disabled - boolean - Is user disabled? Disabled users cannot log in, and do not count for billing purposes. Users can be automatically disabled after an inactivity period via a Site setting or schedule to be deactivated after specific date.
+    #   disabled - boolean - Is user disabled? Disabled users cannot log in, and do not count for billing purposes.  Users can be automatically disabled after an inactivity period via a Site setting.
     #   ftp_permission - boolean - Can the user access with FTP/FTPS?
     #   header_text - string - Text to display to the user in the header of the UI
     #   language - string - Preferred language
     #   notification_daily_send_time - int64 - Hour of the day at which daily notifications should be sent. Can be in range 0 to 23
     #   name - string - User's full name
     #   company - string - User's company
     #   notes - string - Any internal notes on the user
     #   office_integration_enabled - boolean - Enable integration with Office for the web?
     #   password_validity_days - int64 - Number of days to allow user to use the same password
     #   receive_admin_alerts - boolean - Should the user receive admin alerts such a certificate expiration notifications and overages?
     #   require_login_by - string - Require user to login by specified date otherwise it will be disabled.
     #   require_password_change - boolean - Is a password change required upon next user login?
-    #   restapi_permission - boolean - Can this user access the Web app, Desktop app, SDKs, or REST API?  (All of these tools use the API internally, so this is one unified permission set.)
+    #   restapi_permission - boolean - Can this user access the REST API?
     #   self_managed - boolean - Does this user manage it's own credentials or is it a shared/bot user?
     #   sftp_permission - boolean - Can the user access with SFTP?
     #   site_admin - boolean - Is the user an administrator for this site?
     #   skip_welcome_screen - boolean - Skip Welcome page in the UI?
     #   ssl_required - string - SSL required setting
     #   sso_strategy_id - int64 - SSO (Single Sign On) strategy ID for the user, if applicable.
     #   subscribe_to_newsletter - boolean - Is the user subscribed to the newsletter?
@@ -483,28 +481,28 @@
 #   attachments_permission - boolean - DEPRECATED: Can the user create Bundles (aka Share Links)? Use the bundle permission instead.
 #   authenticate_until - string - Scheduled Date/Time at which user will be deactivated
 #   authentication_method - string - How is this user authenticated?
 #   billing_permission - boolean - Allow this user to perform operations on the account, payments, and invoices?
 #   bypass_inactive_disable - boolean - Exempt this user from being disabled based on inactivity?
 #   bypass_site_allowed_ips - boolean - Allow this user to skip site-wide IP blacklists?
 #   dav_permission - boolean - Can the user connect with WebDAV?
-#   disabled - boolean - Is user disabled? Disabled users cannot log in, and do not count for billing purposes. Users can be automatically disabled after an inactivity period via a Site setting or schedule to be deactivated after specific date.
+#   disabled - boolean - Is user disabled? Disabled users cannot log in, and do not count for billing purposes.  Users can be automatically disabled after an inactivity period via a Site setting.
 #   ftp_permission - boolean - Can the user access with FTP/FTPS?
 #   header_text - string - Text to display to the user in the header of the UI
 #   language - string - Preferred language
 #   notification_daily_send_time - int64 - Hour of the day at which daily notifications should be sent. Can be in range 0 to 23
 #   name - string - User's full name
 #   company - string - User's company
 #   notes - string - Any internal notes on the user
 #   office_integration_enabled - boolean - Enable integration with Office for the web?
 #   password_validity_days - int64 - Number of days to allow user to use the same password
 #   receive_admin_alerts - boolean - Should the user receive admin alerts such a certificate expiration notifications and overages?
 #   require_login_by - string - Require user to login by specified date otherwise it will be disabled.
 #   require_password_change - boolean - Is a password change required upon next user login?
-#   restapi_permission - boolean - Can this user access the Web app, Desktop app, SDKs, or REST API?  (All of these tools use the API internally, so this is one unified permission set.)
+#   restapi_permission - boolean - Can this user access the REST API?
 #   self_managed - boolean - Does this user manage it's own credentials or is it a shared/bot user?
 #   sftp_permission - boolean - Can the user access with SFTP?
 #   site_admin - boolean - Is the user an administrator for this site?
 #   skip_welcome_screen - boolean - Skip Welcome page in the UI?
 #   ssl_required - string - SSL required setting
 #   sso_strategy_id - int64 - SSO (Single Sign On) strategy ID for the user, if applicable.
 #   subscribe_to_newsletter - boolean - Is the user subscribed to the newsletter?
@@ -700,28 +698,28 @@
 #   attachments_permission - boolean - DEPRECATED: Can the user create Bundles (aka Share Links)? Use the bundle permission instead.
 #   authenticate_until - string - Scheduled Date/Time at which user will be deactivated
 #   authentication_method - string - How is this user authenticated?
 #   billing_permission - boolean - Allow this user to perform operations on the account, payments, and invoices?
 #   bypass_inactive_disable - boolean - Exempt this user from being disabled based on inactivity?
 #   bypass_site_allowed_ips - boolean - Allow this user to skip site-wide IP blacklists?
 #   dav_permission - boolean - Can the user connect with WebDAV?
-#   disabled - boolean - Is user disabled? Disabled users cannot log in, and do not count for billing purposes. Users can be automatically disabled after an inactivity period via a Site setting or schedule to be deactivated after specific date.
+#   disabled - boolean - Is user disabled? Disabled users cannot log in, and do not count for billing purposes.  Users can be automatically disabled after an inactivity period via a Site setting.
 #   ftp_permission - boolean - Can the user access with FTP/FTPS?
 #   header_text - string - Text to display to the user in the header of the UI
 #   language - string - Preferred language
 #   notification_daily_send_time - int64 - Hour of the day at which daily notifications should be sent. Can be in range 0 to 23
 #   name - string - User's full name
 #   company - string - User's company
 #   notes - string - Any internal notes on the user
 #   office_integration_enabled - boolean - Enable integration with Office for the web?
 #   password_validity_days - int64 - Number of days to allow user to use the same password
 #   receive_admin_alerts - boolean - Should the user receive admin alerts such a certificate expiration notifications and overages?
 #   require_login_by - string - Require user to login by specified date otherwise it will be disabled.
 #   require_password_change - boolean - Is a password change required upon next user login?
-#   restapi_permission - boolean - Can this user access the Web app, Desktop app, SDKs, or REST API?  (All of these tools use the API internally, so this is one unified permission set.)
+#   restapi_permission - boolean - Can this user access the REST API?
 #   self_managed - boolean - Does this user manage it's own credentials or is it a shared/bot user?
 #   sftp_permission - boolean - Can the user access with SFTP?
 #   site_admin - boolean - Is the user an administrator for this site?
 #   skip_welcome_screen - boolean - Skip Welcome page in the UI?
 #   ssl_required - string - SSL required setting
 #   sso_strategy_id - int64 - SSO (Single Sign On) strategy ID for the user, if applicable.
 #   subscribe_to_newsletter - boolean - Is the user subscribed to the newsletter?
```

### Comparing `Files.com-1.4.81/files_sdk/models/user_cipher_use.py` & `Files.com-1.4.9/files_sdk/models/user_cipher_use.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/models/user_request.py` & `Files.com-1.4.9/files_sdk/models/user_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 class UserRequest:
     default_attributes = {
         "id": None,  # int64 - ID
         "name": None,  # string - User's full name
         "email": None,  # email - User email address
         "details": None,  # string - Details of the user's request
-        "company": None,  # string - User's company name
     }
 
     def __init__(self, attributes=None, options=None):
         if not isinstance(attributes, dict):
             attributes = {}
         if not isinstance(options, dict):
             options = {}
@@ -110,28 +109,25 @@
     find(id, params, options)
 
 
 # Parameters:
 #   name (required) - string - Name of user requested
 #   email (required) - string - Email of user requested
 #   details (required) - string - Details of the user request
-#   company - string - Company of the user requested
 def create(params=None, options=None):
     if not isinstance(params, dict):
         params = {}
     if not isinstance(options, dict):
         options = {}
     if "name" in params and not isinstance(params["name"], str):
         raise InvalidParameterError("Bad parameter: name must be an str")
     if "email" in params and not isinstance(params["email"], str):
         raise InvalidParameterError("Bad parameter: email must be an str")
     if "details" in params and not isinstance(params["details"], str):
         raise InvalidParameterError("Bad parameter: details must be an str")
-    if "company" in params and not isinstance(params["company"], str):
-        raise InvalidParameterError("Bad parameter: company must be an str")
     if "name" not in params:
         raise MissingParameterError("Parameter missing: name")
     if "email" not in params:
         raise MissingParameterError("Parameter missing: email")
     if "details" not in params:
         raise MissingParameterError("Parameter missing: details")
     response, options = Api.send_request(
```

### Comparing `Files.com-1.4.81/files_sdk/models/webhook_test.py` & `Files.com-1.4.9/files_sdk/models/webhook_test.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/path_util.py` & `Files.com-1.4.9/files_sdk/path_util.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/files_sdk/util.py` & `Files.com-1.4.9/files_sdk/util.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.81/setup.py` & `Files.com-1.4.9/setup.py`

 * *Files identical despite different names*

