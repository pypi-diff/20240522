# Comparing `tmp/energy_base-1.7.7.tar.gz` & `tmp/energy_base-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energy_base-1.7.7.tar", max compression
+gzip compressed data, was "energy_base-1.7.8.tar", max compression
```

## Comparing `energy_base-1.7.7.tar` & `energy_base-1.7.8.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0      705 2024-05-07 12:27:34.580278 energy_base-1.7.7/pyproject.toml
--rw-r--r--   0        0        0       19 2024-03-11 05:37:22.917248 energy_base-1.7.7/README.md
--rw-r--r--   0        0        0        0 2024-03-11 05:37:22.917248 energy_base-1.7.7/src/energy_base/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 05:37:22.917248 energy_base-1.7.7/src/energy_base/api/__init__.py
--rw-r--r--   0        0        0     2423 2024-04-01 07:42:22.627511 energy_base-1.7.7/src/energy_base/api/base.py
--rw-r--r--   0        0        0      886 2024-03-29 08:55:52.301726 energy_base-1.7.7/src/energy_base/api/pagination.py
--rw-r--r--   0        0        0       65 2024-04-01 07:42:22.611897 energy_base-1.7.7/src/energy_base/api/permissions/__init__.py
--rw-r--r--   0        0        0      334 2024-03-29 05:31:12.838377 energy_base-1.7.7/src/energy_base/api/permissions/superuser.py
--rw-r--r--   0        0        0      186 2024-03-11 05:37:22.917248 energy_base-1.7.7/src/energy_base/api/routers.py
--rw-r--r--   0        0        0      483 2024-03-29 08:59:36.574149 energy_base-1.7.7/src/energy_base/api/views.py
--rw-r--r--   0        0        0      245 2024-03-11 05:37:22.917248 energy_base-1.7.7/src/energy_base/authentications/__init__.py
--rw-r--r--   0        0        0     1031 2024-03-11 05:37:22.917248 energy_base-1.7.7/src/energy_base/authentications/microservice_authentication.py
--rw-r--r--   0        0        0     2588 2024-03-11 05:37:22.917248 energy_base-1.7.7/src/energy_base/authentications/models.py
--rw-r--r--   0        0        0        0 2024-04-08 10:08:34.149579 energy_base-1.7.7/src/energy_base/external_api/__init__.py
--rw-r--r--   0        0        0       81 2024-04-08 10:08:34.150579 energy_base-1.7.7/src/energy_base/external_api/serializers/__init__.py
--rw-r--r--   0        0        0      414 2024-04-08 10:08:34.150579 energy_base-1.7.7/src/energy_base/external_api/serializers/api_status.py
--rw-r--r--   0        0        0       73 2024-04-08 10:08:34.151579 energy_base-1.7.7/src/energy_base/external_api/views/__init__.py
--rw-r--r--   0        0        0     1068 2024-04-19 11:37:53.597951 energy_base-1.7.7/src/energy_base/external_api/views/api_status.py
--rw-r--r--   0        0        0        0 2024-03-29 10:44:11.508892 energy_base-1.7.7/src/energy_base/file_upload/__init__.py
--rw-r--r--   0        0        0      351 2024-04-08 10:11:07.315086 energy_base-1.7.7/src/energy_base/file_upload/admin.py
--rw-r--r--   0        0        0      171 2024-03-29 10:58:14.727096 energy_base-1.7.7/src/energy_base/file_upload/apps.py
--rw-r--r--   0        0        0      160 2024-03-29 10:57:55.998201 energy_base-1.7.7/src/energy_base/file_upload/data_processors/__init__.py
--rw-r--r--   0        0        0     1569 2024-03-29 10:48:14.069159 energy_base-1.7.7/src/energy_base/file_upload/data_processors/base_sheet_processor.py
--rw-r--r--   0        0        0      789 2024-03-29 10:44:11.509889 energy_base-1.7.7/src/energy_base/file_upload/data_processors/xls_processor.py
--rw-r--r--   0        0        0       73 2024-05-06 07:24:47.742571 energy_base-1.7.7/src/energy_base/file_upload/filters/__init__.py
--rw-r--r--   0        0        0      338 2024-03-29 10:48:14.051821 energy_base-1.7.7/src/energy_base/file_upload/filters/file.py
--rw-r--r--   0        0        0        0 2024-03-29 10:44:11.509889 energy_base-1.7.7/src/energy_base/file_upload/migrations/__init__.py
--rw-r--r--   0        0        0      138 2024-03-29 10:57:56.002202 energy_base-1.7.7/src/energy_base/file_upload/models/__init__.py
--rw-r--r--   0        0        0     1125 2024-03-29 10:48:14.058943 energy_base-1.7.7/src/energy_base/file_upload/models/import_file.py
--rw-r--r--   0        0        0      823 2024-04-08 10:12:23.795678 energy_base-1.7.7/src/energy_base/file_upload/models/temporary_data.py
--rw-r--r--   0        0        0      416 2024-05-06 07:24:47.742571 energy_base-1.7.7/src/energy_base/file_upload/serializers/__init__.py
--rw-r--r--   0        0        0      737 2024-03-29 10:48:14.046819 energy_base-1.7.7/src/energy_base/file_upload/serializers/file.py
--rw-r--r--   0        0        0      368 2024-05-06 07:24:47.742571 energy_base-1.7.7/src/energy_base/file_upload/serializers/file_upload_status.py
--rw-r--r--   0        0        0       74 2024-03-29 10:51:10.661193 energy_base-1.7.7/src/energy_base/file_upload/services/__init__.py
--rw-r--r--   0        0        0      258 2024-03-29 10:51:10.676832 energy_base-1.7.7/src/energy_base/file_upload/services/minio.py
--rw-r--r--   0        0        0      699 2024-05-06 06:55:37.565569 energy_base-1.7.7/src/energy_base/file_upload/urls.py
--rw-r--r--   0        0        0      305 2024-05-06 06:55:37.528252 energy_base-1.7.7/src/energy_base/file_upload/views/__init__.py
--rw-r--r--   0        0        0     5820 2024-03-29 10:53:38.129538 energy_base-1.7.7/src/energy_base/file_upload/views/file.py
--rw-r--r--   0        0        0     1256 2024-05-06 07:24:47.742571 energy_base-1.7.7/src/energy_base/file_upload/views/file_upload_status.py
--rw-r--r--   0        0        0       82 2024-03-11 05:37:22.917248 energy_base-1.7.7/src/energy_base/models/__init__.py
--rw-r--r--   0        0        0      308 2024-03-11 05:37:22.917248 energy_base-1.7.7/src/energy_base/models/jwt_user.py
--rw-r--r--   0        0        0        0 2024-03-29 05:31:12.838377 energy_base-1.7.7/src/energy_base/q_api/__init__.py
--rw-r--r--   0        0        0      159 2024-03-29 05:31:12.838377 energy_base-1.7.7/src/energy_base/q_api/apps.py
--rw-r--r--   0        0        0       97 2024-03-29 05:31:12.838377 energy_base-1.7.7/src/energy_base/q_api/filters/__init__.py
--rw-r--r--   0        0        0      138 2024-03-29 05:31:12.838377 energy_base-1.7.7/src/energy_base/q_api/filters/task.py
--rw-r--r--   0        0        0      201 2024-03-29 05:31:12.838377 energy_base-1.7.7/src/energy_base/q_api/serializers/__init__.py
--rw-r--r--   0        0        0      396 2024-03-29 05:31:12.838377 energy_base-1.7.7/src/energy_base/q_api/serializers/schedule.py
--rw-r--r--   0        0        0      617 2024-03-29 05:31:12.838377 energy_base-1.7.7/src/energy_base/q_api/serializers/task.py
--rw-r--r--   0        0        0      483 2024-03-29 05:31:12.838377 energy_base-1.7.7/src/energy_base/q_api/urls.py
--rw-r--r--   0        0        0      224 2024-03-29 05:31:12.838377 energy_base-1.7.7/src/energy_base/q_api/views/__init__.py
--rw-r--r--   0        0        0      863 2024-03-29 05:31:12.838377 energy_base-1.7.7/src/energy_base/q_api/views/schedule.py
--rw-r--r--   0        0        0      532 2024-03-29 05:31:12.838377 energy_base-1.7.7/src/energy_base/q_api/views/task.py
--rw-r--r--   0        0        0        0 2024-03-29 05:31:16.931816 energy_base-1.7.7/src/energy_base/references_api/__init__.py
--rw-r--r--   0        0        0       66 2024-03-29 05:31:16.911760 energy_base-1.7.7/src/energy_base/references_api/admin.py
--rw-r--r--   0        0        0      177 2024-03-29 08:47:27.971536 energy_base-1.7.7/src/energy_base/references_api/apps.py
--rw-r--r--   0        0        0        0 2024-03-29 05:31:16.932321 energy_base-1.7.7/src/energy_base/references_api/migrations/__init__.py
--rw-r--r--   0        0        0       60 2024-03-29 05:31:16.918805 energy_base-1.7.7/src/energy_base/references_api/models.py
--rw-r--r--   0        0        0       63 2024-03-29 05:31:16.926923 energy_base-1.7.7/src/energy_base/references_api/tests.py
--rw-r--r--   0        0        0      403 2024-03-29 08:29:14.326841 energy_base-1.7.7/src/energy_base/references_api/urls.py
--rw-r--r--   0        0        0     3889 2024-05-07 12:26:16.406348 energy_base-1.7.7/src/energy_base/references_api/utils.py
--rw-r--r--   0        0        0      183 2024-04-08 10:08:34.153661 energy_base-1.7.7/src/energy_base/services/__init__.py
--rw-r--r--   0        0        0     5312 2024-04-25 06:06:01.686923 energy_base-1.7.7/src/energy_base/services/base_api.py
--rw-r--r--   0        0        0     1508 2024-03-11 05:37:22.917248 energy_base-1.7.7/src/energy_base/services/minio.py
--rw-r--r--   0        0        0      784 2024-04-08 10:08:34.154658 energy_base-1.7.7/src/energy_base/services/telnet.py
--rw-r--r--   0        0        0      527 2024-03-29 10:53:38.129538 energy_base-1.7.7/src/energy_base/services/user.py
--rw-r--r--   0        0        0      208 2024-03-11 05:37:22.932870 energy_base-1.7.7/src/energy_base/translation/__init__.py
--rw-r--r--   0        0        0      358 2024-03-11 05:37:22.932870 energy_base-1.7.7/src/energy_base/translation/utils.py
--rw-r--r--   0        0        0      206 2024-04-25 06:05:45.414431 energy_base-1.7.7/src/energy_base/utils/__init__.py
--rw-r--r--   0        0        0     1402 2024-03-11 10:56:13.497068 energy_base-1.7.7/src/energy_base/utils/data.py
--rw-r--r--   0        0        0     3354 2024-04-25 06:05:07.967181 energy_base-1.7.7/src/energy_base/utils/date.py
--rw-r--r--   0        0        0      778 2024-03-11 05:37:22.932870 energy_base-1.7.7/src/energy_base/utils/dict_util.py
--rw-r--r--   0        0        0      632 2024-04-08 10:08:34.155696 energy_base-1.7.7/src/energy_base/utils/response_processors.py
--rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 energy_base-1.7.7/PKG-INFO
+-rw-r--r--   0        0        0      705 2024-05-22 10:52:10.919368 energy_base-1.7.8/pyproject.toml
+-rw-r--r--   0        0        0       19 2024-03-11 05:37:22.917248 energy_base-1.7.8/README.md
+-rw-r--r--   0        0        0        0 2024-03-11 05:37:22.917248 energy_base-1.7.8/src/energy_base/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 05:37:22.917248 energy_base-1.7.8/src/energy_base/api/__init__.py
+-rw-r--r--   0        0        0     2423 2024-04-01 07:42:22.627511 energy_base-1.7.8/src/energy_base/api/base.py
+-rw-r--r--   0        0        0      886 2024-03-29 08:55:52.301726 energy_base-1.7.8/src/energy_base/api/pagination.py
+-rw-r--r--   0        0        0       65 2024-04-01 07:42:22.611897 energy_base-1.7.8/src/energy_base/api/permissions/__init__.py
+-rw-r--r--   0        0        0      334 2024-03-29 05:31:12.838377 energy_base-1.7.8/src/energy_base/api/permissions/superuser.py
+-rw-r--r--   0        0        0      186 2024-03-11 05:37:22.917248 energy_base-1.7.8/src/energy_base/api/routers.py
+-rw-r--r--   0        0        0      483 2024-03-29 08:59:36.574149 energy_base-1.7.8/src/energy_base/api/views.py
+-rw-r--r--   0        0        0      245 2024-03-11 05:37:22.917248 energy_base-1.7.8/src/energy_base/authentications/__init__.py
+-rw-r--r--   0        0        0     1031 2024-03-11 05:37:22.917248 energy_base-1.7.8/src/energy_base/authentications/microservice_authentication.py
+-rw-r--r--   0        0        0     2588 2024-03-11 05:37:22.917248 energy_base-1.7.8/src/energy_base/authentications/models.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:08:34.149579 energy_base-1.7.8/src/energy_base/external_api/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-08 10:08:34.150579 energy_base-1.7.8/src/energy_base/external_api/serializers/__init__.py
+-rw-r--r--   0        0        0      414 2024-04-08 10:08:34.150579 energy_base-1.7.8/src/energy_base/external_api/serializers/api_status.py
+-rw-r--r--   0        0        0       73 2024-04-08 10:08:34.151579 energy_base-1.7.8/src/energy_base/external_api/views/__init__.py
+-rw-r--r--   0        0        0     1068 2024-04-19 11:37:53.597951 energy_base-1.7.8/src/energy_base/external_api/views/api_status.py
+-rw-r--r--   0        0        0        0 2024-03-29 10:44:11.508892 energy_base-1.7.8/src/energy_base/file_upload/__init__.py
+-rw-r--r--   0        0        0      351 2024-04-08 10:11:07.315086 energy_base-1.7.8/src/energy_base/file_upload/admin.py
+-rw-r--r--   0        0        0      171 2024-03-29 10:58:14.727096 energy_base-1.7.8/src/energy_base/file_upload/apps.py
+-rw-r--r--   0        0        0      160 2024-03-29 10:57:55.998201 energy_base-1.7.8/src/energy_base/file_upload/data_processors/__init__.py
+-rw-r--r--   0        0        0     1569 2024-03-29 10:48:14.069159 energy_base-1.7.8/src/energy_base/file_upload/data_processors/base_sheet_processor.py
+-rw-r--r--   0        0        0      789 2024-03-29 10:44:11.509889 energy_base-1.7.8/src/energy_base/file_upload/data_processors/xls_processor.py
+-rw-r--r--   0        0        0       73 2024-05-06 07:24:47.742571 energy_base-1.7.8/src/energy_base/file_upload/filters/__init__.py
+-rw-r--r--   0        0        0      338 2024-03-29 10:48:14.051821 energy_base-1.7.8/src/energy_base/file_upload/filters/file.py
+-rw-r--r--   0        0        0        0 2024-03-29 10:44:11.509889 energy_base-1.7.8/src/energy_base/file_upload/migrations/__init__.py
+-rw-r--r--   0        0        0      138 2024-03-29 10:57:56.002202 energy_base-1.7.8/src/energy_base/file_upload/models/__init__.py
+-rw-r--r--   0        0        0     1125 2024-03-29 10:48:14.058943 energy_base-1.7.8/src/energy_base/file_upload/models/import_file.py
+-rw-r--r--   0        0        0      823 2024-04-08 10:12:23.795678 energy_base-1.7.8/src/energy_base/file_upload/models/temporary_data.py
+-rw-r--r--   0        0        0      416 2024-05-06 07:24:47.742571 energy_base-1.7.8/src/energy_base/file_upload/serializers/__init__.py
+-rw-r--r--   0        0        0      737 2024-03-29 10:48:14.046819 energy_base-1.7.8/src/energy_base/file_upload/serializers/file.py
+-rw-r--r--   0        0        0      368 2024-05-06 07:24:47.742571 energy_base-1.7.8/src/energy_base/file_upload/serializers/file_upload_status.py
+-rw-r--r--   0        0        0       74 2024-03-29 10:51:10.661193 energy_base-1.7.8/src/energy_base/file_upload/services/__init__.py
+-rw-r--r--   0        0        0      258 2024-03-29 10:51:10.676832 energy_base-1.7.8/src/energy_base/file_upload/services/minio.py
+-rw-r--r--   0        0        0      699 2024-05-06 06:55:37.565569 energy_base-1.7.8/src/energy_base/file_upload/urls.py
+-rw-r--r--   0        0        0      305 2024-05-06 06:55:37.528252 energy_base-1.7.8/src/energy_base/file_upload/views/__init__.py
+-rw-r--r--   0        0        0     5820 2024-03-29 10:53:38.129538 energy_base-1.7.8/src/energy_base/file_upload/views/file.py
+-rw-r--r--   0        0        0     1256 2024-05-06 07:24:47.742571 energy_base-1.7.8/src/energy_base/file_upload/views/file_upload_status.py
+-rw-r--r--   0        0        0       82 2024-03-11 05:37:22.917248 energy_base-1.7.8/src/energy_base/models/__init__.py
+-rw-r--r--   0        0        0      308 2024-03-11 05:37:22.917248 energy_base-1.7.8/src/energy_base/models/jwt_user.py
+-rw-r--r--   0        0        0        0 2024-03-29 05:31:12.838377 energy_base-1.7.8/src/energy_base/q_api/__init__.py
+-rw-r--r--   0        0        0      159 2024-03-29 05:31:12.838377 energy_base-1.7.8/src/energy_base/q_api/apps.py
+-rw-r--r--   0        0        0       97 2024-03-29 05:31:12.838377 energy_base-1.7.8/src/energy_base/q_api/filters/__init__.py
+-rw-r--r--   0        0        0      138 2024-03-29 05:31:12.838377 energy_base-1.7.8/src/energy_base/q_api/filters/task.py
+-rw-r--r--   0        0        0      201 2024-03-29 05:31:12.838377 energy_base-1.7.8/src/energy_base/q_api/serializers/__init__.py
+-rw-r--r--   0        0        0      396 2024-03-29 05:31:12.838377 energy_base-1.7.8/src/energy_base/q_api/serializers/schedule.py
+-rw-r--r--   0        0        0      617 2024-03-29 05:31:12.838377 energy_base-1.7.8/src/energy_base/q_api/serializers/task.py
+-rw-r--r--   0        0        0      483 2024-03-29 05:31:12.838377 energy_base-1.7.8/src/energy_base/q_api/urls.py
+-rw-r--r--   0        0        0      224 2024-03-29 05:31:12.838377 energy_base-1.7.8/src/energy_base/q_api/views/__init__.py
+-rw-r--r--   0        0        0      863 2024-03-29 05:31:12.838377 energy_base-1.7.8/src/energy_base/q_api/views/schedule.py
+-rw-r--r--   0        0        0      532 2024-03-29 05:31:12.838377 energy_base-1.7.8/src/energy_base/q_api/views/task.py
+-rw-r--r--   0        0        0        0 2024-03-29 05:31:16.931816 energy_base-1.7.8/src/energy_base/references_api/__init__.py
+-rw-r--r--   0        0        0       66 2024-03-29 05:31:16.911760 energy_base-1.7.8/src/energy_base/references_api/admin.py
+-rw-r--r--   0        0        0      177 2024-03-29 08:47:27.971536 energy_base-1.7.8/src/energy_base/references_api/apps.py
+-rw-r--r--   0        0        0        0 2024-03-29 05:31:16.932321 energy_base-1.7.8/src/energy_base/references_api/migrations/__init__.py
+-rw-r--r--   0        0        0       60 2024-03-29 05:31:16.918805 energy_base-1.7.8/src/energy_base/references_api/models.py
+-rw-r--r--   0        0        0       63 2024-03-29 05:31:16.926923 energy_base-1.7.8/src/energy_base/references_api/tests.py
+-rw-r--r--   0        0        0      403 2024-03-29 08:29:14.326841 energy_base-1.7.8/src/energy_base/references_api/urls.py
+-rw-r--r--   0        0        0     3889 2024-05-07 12:26:16.406348 energy_base-1.7.8/src/energy_base/references_api/utils.py
+-rw-r--r--   0        0        0      183 2024-04-08 10:08:34.153661 energy_base-1.7.8/src/energy_base/services/__init__.py
+-rw-r--r--   0        0        0     5312 2024-04-25 06:06:01.686923 energy_base-1.7.8/src/energy_base/services/base_api.py
+-rw-r--r--   0        0        0     1508 2024-03-11 05:37:22.917248 energy_base-1.7.8/src/energy_base/services/minio.py
+-rw-r--r--   0        0        0      784 2024-04-08 10:08:34.154658 energy_base-1.7.8/src/energy_base/services/telnet.py
+-rw-r--r--   0        0        0      527 2024-03-29 10:53:38.129538 energy_base-1.7.8/src/energy_base/services/user.py
+-rw-r--r--   0        0        0      208 2024-03-11 05:37:22.932870 energy_base-1.7.8/src/energy_base/translation/__init__.py
+-rw-r--r--   0        0        0      358 2024-03-11 05:37:22.932870 energy_base-1.7.8/src/energy_base/translation/utils.py
+-rw-r--r--   0        0        0      206 2024-04-25 06:05:45.414431 energy_base-1.7.8/src/energy_base/utils/__init__.py
+-rw-r--r--   0        0        0     1402 2024-03-11 10:56:13.497068 energy_base-1.7.8/src/energy_base/utils/data.py
+-rw-r--r--   0        0        0     3690 2024-05-22 10:40:26.775036 energy_base-1.7.8/src/energy_base/utils/date.py
+-rw-r--r--   0        0        0      778 2024-03-11 05:37:22.932870 energy_base-1.7.8/src/energy_base/utils/dict_util.py
+-rw-r--r--   0        0        0      632 2024-04-08 10:08:34.155696 energy_base-1.7.8/src/energy_base/utils/response_processors.py
+-rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 energy_base-1.7.8/PKG-INFO
```

### Comparing `energy_base-1.7.7/pyproject.toml` & `energy_base-1.7.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "energy-base"
-version = "1.7.7"
+version = "1.7.8"
 description = "Energy Base Package"
 authors = ["Olimboy <shavkatov.olimboy@mail.ru>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 djangorestframework = "^3.14.0"
```

### Comparing `energy_base-1.7.7/src/energy_base/api/base.py` & `energy_base-1.7.8/src/energy_base/api/base.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/api/pagination.py` & `energy_base-1.7.8/src/energy_base/api/pagination.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/authentications/microservice_authentication.py` & `energy_base-1.7.8/src/energy_base/authentications/microservice_authentication.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/authentications/models.py` & `energy_base-1.7.8/src/energy_base/authentications/models.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/external_api/views/api_status.py` & `energy_base-1.7.8/src/energy_base/external_api/views/api_status.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/file_upload/data_processors/base_sheet_processor.py` & `energy_base-1.7.8/src/energy_base/file_upload/data_processors/base_sheet_processor.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/file_upload/data_processors/xls_processor.py` & `energy_base-1.7.8/src/energy_base/file_upload/data_processors/xls_processor.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/file_upload/models/import_file.py` & `energy_base-1.7.8/src/energy_base/file_upload/models/import_file.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/file_upload/models/temporary_data.py` & `energy_base-1.7.8/src/energy_base/file_upload/models/temporary_data.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/file_upload/serializers/file.py` & `energy_base-1.7.8/src/energy_base/file_upload/serializers/file.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/file_upload/urls.py` & `energy_base-1.7.8/src/energy_base/file_upload/urls.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/file_upload/views/file.py` & `energy_base-1.7.8/src/energy_base/file_upload/views/file.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/file_upload/views/file_upload_status.py` & `energy_base-1.7.8/src/energy_base/file_upload/views/file_upload_status.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/q_api/serializers/task.py` & `energy_base-1.7.8/src/energy_base/q_api/serializers/task.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/q_api/views/schedule.py` & `energy_base-1.7.8/src/energy_base/q_api/views/schedule.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/q_api/views/task.py` & `energy_base-1.7.8/src/energy_base/q_api/views/task.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/references_api/utils.py` & `energy_base-1.7.8/src/energy_base/references_api/utils.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/services/base_api.py` & `energy_base-1.7.8/src/energy_base/services/base_api.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/services/minio.py` & `energy_base-1.7.8/src/energy_base/services/minio.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/services/telnet.py` & `energy_base-1.7.8/src/energy_base/services/telnet.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/services/user.py` & `energy_base-1.7.8/src/energy_base/services/user.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/utils/data.py` & `energy_base-1.7.8/src/energy_base/utils/data.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/utils/date.py` & `energy_base-1.7.8/src/energy_base/utils/date.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,54 +55,66 @@
         return to_edate(datetime.strptime(__date_string, __format))
 
     def __str__(self):
         return self.strftime()
 
 
 class EDateTime(datetime):
+    def first_second_of_day(self):
+        return self.replace(hour=0, minute=0, second=0)
+
+    def last_second_of_day(self):
+        return self.replace(hour=23, minute=59, second=59)
+
     def first_second_of_hour(self):
         return self.replace(minute=0, second=0)
 
     def last_second_of_hour(self):
         return self.replace(minute=59, second=59)
 
     def first_second_of_minute(self):
         return self.replace(second=0)
 
     def last_second_of_minute(self):
         return self.replace(second=59)
 
+    def one_hour_later(self):
+        return self + timedelta(hours=1)
+
+    def hour_ago(self):
+        return self - timedelta(hours=1)
+
     def tomorrow(self):
         return self + timedelta(days=1)
 
     def yesterday(self):
         return self - timedelta(days=1)
 
     def first_day_of_month(self):
         return self.replace(day=1)
 
-    def first_day_of_year(self):
-        return self.replace(day=1, month=1)
-
     def last_day_of_month(self):
         _, ndays = monthrange(self.year, self.month)
         return self.replace(day=ndays)
 
+    def first_day_of_year(self):
+        return self.replace(day=1, month=1)
+
     def last_day_of_year(self):
         return self.replace(day=31, month=12)
 
     def first_day_of_last_month(self):
         return self.replace(day=1).yesterday().replace(day=1)
 
-    def first_day_of_last_year(self):
-        return self.replace(day=1, month=1, year=self.year - 1)
-
     def last_day_of_last_month(self):
         return self.replace(day=1).yesterday()
 
+    def first_day_of_last_year(self):
+        return self.replace(day=1, month=1, year=self.year - 1)
+
     def last_day_of_last_year(self):
         return self.replace(day=31, month=12, year=self.year - 1)
 
     def strftime(self, __format=DEFAULT_DATETIME_FORMAT):
         return super().strftime(__format)
 
     @staticmethod
```

### Comparing `energy_base-1.7.7/src/energy_base/utils/dict_util.py` & `energy_base-1.7.8/src/energy_base/utils/dict_util.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/src/energy_base/utils/response_processors.py` & `energy_base-1.7.8/src/energy_base/utils/response_processors.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.7.7/PKG-INFO` & `energy_base-1.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energy-base
-Version: 1.7.7
+Version: 1.7.8
 Summary: Energy Base Package
 Author: Olimboy
 Author-email: shavkatov.olimboy@mail.ru
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: croniter (>=2.0.3,<3.0.0)
 Requires-Dist: django (==4.2.9)
```

