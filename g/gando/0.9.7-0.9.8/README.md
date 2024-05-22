# Comparing `tmp/gando-0.9.7.tar.gz` & `tmp/gando-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gando-0.9.7.tar", last modified: Sun Jan 21 10:08:33 2024, max compression
+gzip compressed data, was "gando-0.9.8.tar", last modified: Sun Jan 21 11:12:35 2024, max compression
```

## Comparing `gando-0.9.7.tar` & `gando-0.9.8.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.203433 gando-0.9.7/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)     1072 2024-01-03 03:41:35.000000 gando-0.9.7/LICENSE
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       52 2024-01-03 03:41:35.000000 gando-0.9.7/MANIFEST.in
--rw-r--r--   0 nvd       (1000) nvd       (1000)     1590 2024-01-21 10:08:33.203433 gando-0.9.7/PKG-INFO
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      315 2024-01-03 03:41:35.000000 gando-0.9.7/README.md
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       98 2024-01-03 03:41:35.000000 gando-0.9.7/pyproject.toml
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      108 2024-01-21 10:08:33.203433 gando-0.9.7/setup.cfg
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)     1583 2024-01-10 05:52:02.000000 gando-0.9.7/setup.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.176766 gando-0.9.7/src/
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.183433 gando-0.9.7/src/gando/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       22 2024-01-21 10:07:57.000000 gando-0.9.7/src/gando/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.183433 gando-0.9.7/src/gando/admin/
--rw-r--r--   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/admin/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.183433 gando-0.9.7/src/gando/admin/models/
--rw-r--r--   0 nvd       (1000) nvd       (1000)     7864 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/admin/models/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.183433 gando-0.9.7/src/gando/architectures/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/architectures/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.186766 gando-0.9.7/src/gando/architectures/apis/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)    15069 2024-01-21 10:07:57.000000 gando-0.9.7/src/gando/architectures/apis/__base.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      134 2024-01-14 20:49:34.000000 gando-0.9.7/src/gando/architectures/apis/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.186766 gando-0.9.7/src/gando/architectures/interfaces/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)     1548 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/architectures/interfaces/__base.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       34 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/architectures/interfaces/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.186766 gando-0.9.7/src/gando/architectures/services/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)     5564 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/architectures/services/__base.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      997 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/architectures/services/__creator.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)     1031 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/architectures/services/__database_manager.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)     3178 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/architectures/services/__getter.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      531 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/architectures/services/__getter_creator.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      273 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/architectures/services/__init__.py
--rw-r--r--   0 nvd       (1000) nvd       (1000)     1085 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/architectures/services/__updater.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.186766 gando-0.9.7/src/gando/auth/
--rw-r--r--   0 nvd       (1000) nvd       (1000)      823 2024-01-07 19:23:56.000000 gando-0.9.7/src/gando/auth/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.186766 gando-0.9.7/src/gando/config/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      537 2024-01-07 18:53:03.000000 gando-0.9.7/src/gando/config/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.186766 gando-0.9.7/src/gando/http/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.190100 gando-0.9.7/src/gando/http/requests/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/requests/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.190100 gando-0.9.7/src/gando/http/requests/func/
--rw-r--r--   0 nvd       (1000) nvd       (1000)     4564 2024-01-10 11:56:25.000000 gando-0.9.7/src/gando/http/requests/func/__asyncio.py
--rw-r--r--   0 nvd       (1000) nvd       (1000)       44 2024-01-10 05:50:44.000000 gando-0.9.7/src/gando/http/requests/func/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.190100 gando-0.9.7/src/gando/http/requests/methods/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      122 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/requests/methods/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.190100 gando-0.9.7/src/gando/http/requests/schemas/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       37 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/requests/schemas/__init__.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      553 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/requests/schemas/__request.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.190100 gando-0.9.7/src/gando/http/responses/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       42 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/responses/__init__.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)     4243 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/responses/__json_response.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.190100 gando-0.9.7/src/gando/http/responses/middlewares/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       48 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/responses/middlewares/__init__.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      304 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/responses/middlewares/__request_monitor.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)     1545 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/responses/middlewares/__request_response_message.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      980 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/responses/middlewares/__response_structured.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.193433 gando-0.9.7/src/gando/http/responses/schemas/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       88 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/responses/schemas/__data_many_false.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      163 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/responses/schemas/__data_many_true.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      204 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/responses/schemas/__init__.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      359 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/responses/schemas/__messages.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      358 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/responses/schemas/__response.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.193433 gando-0.9.7/src/gando/http/responses/string_messages/
--rw-r--r--   0 nvd       (1000) nvd       (1000)     4042 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/http/responses/string_messages/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.193433 gando-0.9.7/src/gando/management/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/management/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.193433 gando-0.9.7/src/gando/management/commands/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/management/commands/__init__.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)     7246 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/management/commands/startapi.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)     7220 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/management/commands/startinterface.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)    11382 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/management/commands/startmodel.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)     7122 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/management/commands/startservice.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.193433 gando-0.9.7/src/gando/models/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)     1583 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/models/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.193433 gando-0.9.7/src/gando/models/fields/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)    10714 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/models/fields/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.193433 gando-0.9.7/src/gando/models/serializers/
--rw-r--r--   0 nvd       (1000) nvd       (1000)     2743 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/models/serializers/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.196766 gando-0.9.7/src/gando/schemas/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       42 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/schemas/__init__.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      269 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/schemas/base.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.196766 gando-0.9.7/src/gando/schemas/relations/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/schemas/relations/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.196766 gando-0.9.7/src/gando/schemas/relations/object_relation/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      249 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/schemas/relations/object_relation/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.196766 gando-0.9.7/src/gando/schemas/structures/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      313 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/schemas/structures/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.196766 gando-0.9.7/src/gando/utils/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.196766 gando-0.9.7/src/gando/utils/converters/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/converters/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.196766 gando-0.9.7/src/gando/utils/converters/images/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       51 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/converters/images/__init__.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      623 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/converters/images/__small_blur_base64.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.196766 gando-0.9.7/src/gando/utils/db/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/db/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.196766 gando-0.9.7/src/gando/utils/db/uploaders/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/db/uploaders/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.196766 gando-0.9.7/src/gando/utils/db/uploaders/images/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      408 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/db/uploaders/images/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.196766 gando-0.9.7/src/gando/utils/hashers/
--rw-r--r--   0 nvd       (1000) nvd       (1000)      951 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/hashers/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.200100 gando-0.9.7/src/gando/utils/json/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       25 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/json/__init__.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      265 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/json/__json.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.200100 gando-0.9.7/src/gando/utils/json/encoders/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      202 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/json/encoders/__encoder.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       31 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/json/encoders/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.200100 gando-0.9.7/src/gando/utils/parsers/
--rw-r--r--   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/parsers/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.200100 gando-0.9.7/src/gando/utils/parsers/images/
--rw-r--r--   0 nvd       (1000) nvd       (1000)     2503 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/parsers/images/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.200100 gando-0.9.7/src/gando/utils/strings/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/strings/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.200100 gando-0.9.7/src/gando/utils/strings/casings/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       98 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/strings/casings/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.200100 gando-0.9.7/src/gando/utils/strings/converters/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)     4898 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/strings/converters/__casing.py
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)       29 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/strings/converters/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.200100 gando-0.9.7/src/gando/utils/uploaders/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/uploaders/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.200100 gando-0.9.7/src/gando/utils/uploaders/files/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      405 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/uploaders/files/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.200100 gando-0.9.7/src/gando/utils/uploaders/images/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      407 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/uploaders/images/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.200100 gando-0.9.7/src/gando/utils/validators/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      344 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/validators/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.200100 gando-0.9.7/src/gando/utils/validators/slug/
--rwxr-xr-x   0 nvd       (1000) nvd       (1000)      547 2024-01-03 03:41:35.000000 gando-0.9.7/src/gando/utils/validators/slug/__init__.py
-drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 10:08:33.183433 gando-0.9.7/src/gando.egg-info/
--rw-r--r--   0 nvd       (1000) nvd       (1000)     1590 2024-01-21 10:08:33.000000 gando-0.9.7/src/gando.egg-info/PKG-INFO
--rw-r--r--   0 nvd       (1000) nvd       (1000)     3296 2024-01-21 10:08:33.000000 gando-0.9.7/src/gando.egg-info/SOURCES.txt
--rw-r--r--   0 nvd       (1000) nvd       (1000)        1 2024-01-21 10:08:33.000000 gando-0.9.7/src/gando.egg-info/dependency_links.txt
--rw-r--r--   0 nvd       (1000) nvd       (1000)       94 2024-01-21 10:08:33.000000 gando-0.9.7/src/gando.egg-info/requires.txt
--rw-r--r--   0 nvd       (1000) nvd       (1000)        6 2024-01-21 10:08:33.000000 gando-0.9.7/src/gando.egg-info/top_level.txt
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.246676 gando-0.9.8/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)     1072 2024-01-03 03:41:35.000000 gando-0.9.8/LICENSE
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       52 2024-01-03 03:41:35.000000 gando-0.9.8/MANIFEST.in
+-rw-r--r--   0 nvd       (1000) nvd       (1000)     1590 2024-01-21 11:12:35.246676 gando-0.9.8/PKG-INFO
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      315 2024-01-03 03:41:35.000000 gando-0.9.8/README.md
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       98 2024-01-03 03:41:35.000000 gando-0.9.8/pyproject.toml
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      108 2024-01-21 11:12:35.246676 gando-0.9.8/setup.cfg
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)     1583 2024-01-10 05:52:02.000000 gando-0.9.8/setup.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.220009 gando-0.9.8/src/
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.226676 gando-0.9.8/src/gando/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       22 2024-01-21 11:12:18.000000 gando-0.9.8/src/gando/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.230009 gando-0.9.8/src/gando/admin/
+-rw-r--r--   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/admin/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.230009 gando-0.9.8/src/gando/admin/models/
+-rw-r--r--   0 nvd       (1000) nvd       (1000)     7864 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/admin/models/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.230009 gando-0.9.8/src/gando/architectures/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/architectures/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.230009 gando-0.9.8/src/gando/architectures/apis/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)    16462 2024-01-21 11:11:53.000000 gando-0.9.8/src/gando/architectures/apis/__base.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      134 2024-01-14 20:49:34.000000 gando-0.9.8/src/gando/architectures/apis/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.230009 gando-0.9.8/src/gando/architectures/interfaces/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)     1548 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/architectures/interfaces/__base.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       34 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/architectures/interfaces/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.233343 gando-0.9.8/src/gando/architectures/services/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)     5564 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/architectures/services/__base.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      997 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/architectures/services/__creator.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)     1031 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/architectures/services/__database_manager.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)     3178 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/architectures/services/__getter.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      531 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/architectures/services/__getter_creator.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      273 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/architectures/services/__init__.py
+-rw-r--r--   0 nvd       (1000) nvd       (1000)     1085 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/architectures/services/__updater.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.233343 gando-0.9.8/src/gando/auth/
+-rw-r--r--   0 nvd       (1000) nvd       (1000)      823 2024-01-07 19:23:56.000000 gando-0.9.8/src/gando/auth/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.233343 gando-0.9.8/src/gando/config/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      925 2024-01-21 10:53:07.000000 gando-0.9.8/src/gando/config/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.233343 gando-0.9.8/src/gando/http/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.233343 gando-0.9.8/src/gando/http/requests/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/requests/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.233343 gando-0.9.8/src/gando/http/requests/func/
+-rw-r--r--   0 nvd       (1000) nvd       (1000)     4564 2024-01-10 11:56:25.000000 gando-0.9.8/src/gando/http/requests/func/__asyncio.py
+-rw-r--r--   0 nvd       (1000) nvd       (1000)       44 2024-01-10 05:50:44.000000 gando-0.9.8/src/gando/http/requests/func/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.233343 gando-0.9.8/src/gando/http/requests/methods/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      122 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/requests/methods/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.233343 gando-0.9.8/src/gando/http/requests/schemas/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       37 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/requests/schemas/__init__.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      553 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/requests/schemas/__request.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.233343 gando-0.9.8/src/gando/http/responses/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       42 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/responses/__init__.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)     4243 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/responses/__json_response.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.236676 gando-0.9.8/src/gando/http/responses/middlewares/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       48 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/responses/middlewares/__init__.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      304 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/responses/middlewares/__request_monitor.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)     1545 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/responses/middlewares/__request_response_message.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      980 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/responses/middlewares/__response_structured.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.236676 gando-0.9.8/src/gando/http/responses/schemas/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       88 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/responses/schemas/__data_many_false.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      163 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/responses/schemas/__data_many_true.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      204 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/responses/schemas/__init__.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      359 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/responses/schemas/__messages.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      358 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/responses/schemas/__response.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.236676 gando-0.9.8/src/gando/http/responses/string_messages/
+-rw-r--r--   0 nvd       (1000) nvd       (1000)     4042 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/http/responses/string_messages/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.236676 gando-0.9.8/src/gando/management/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/management/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.236676 gando-0.9.8/src/gando/management/commands/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/management/commands/__init__.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)     7246 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/management/commands/startapi.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)     7220 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/management/commands/startinterface.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)    11382 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/management/commands/startmodel.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)     7122 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/management/commands/startservice.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.236676 gando-0.9.8/src/gando/models/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)     1583 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/models/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.236676 gando-0.9.8/src/gando/models/fields/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)    10714 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/models/fields/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.240009 gando-0.9.8/src/gando/models/serializers/
+-rw-r--r--   0 nvd       (1000) nvd       (1000)     2743 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/models/serializers/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.240009 gando-0.9.8/src/gando/schemas/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       42 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/schemas/__init__.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      269 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/schemas/base.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.240009 gando-0.9.8/src/gando/schemas/relations/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/schemas/relations/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.240009 gando-0.9.8/src/gando/schemas/relations/object_relation/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      249 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/schemas/relations/object_relation/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.240009 gando-0.9.8/src/gando/schemas/structures/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      313 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/schemas/structures/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.240009 gando-0.9.8/src/gando/utils/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.240009 gando-0.9.8/src/gando/utils/converters/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/converters/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.240009 gando-0.9.8/src/gando/utils/converters/images/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       51 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/converters/images/__init__.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      623 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/converters/images/__small_blur_base64.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.240009 gando-0.9.8/src/gando/utils/db/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/db/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.240009 gando-0.9.8/src/gando/utils/db/uploaders/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/db/uploaders/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.240009 gando-0.9.8/src/gando/utils/db/uploaders/images/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      408 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/db/uploaders/images/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.240009 gando-0.9.8/src/gando/utils/hashers/
+-rw-r--r--   0 nvd       (1000) nvd       (1000)      951 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/hashers/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.243342 gando-0.9.8/src/gando/utils/json/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       25 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/json/__init__.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      265 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/json/__json.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.243342 gando-0.9.8/src/gando/utils/json/encoders/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      202 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/json/encoders/__encoder.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       31 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/json/encoders/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.243342 gando-0.9.8/src/gando/utils/parsers/
+-rw-r--r--   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/parsers/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.243342 gando-0.9.8/src/gando/utils/parsers/images/
+-rw-r--r--   0 nvd       (1000) nvd       (1000)     2503 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/parsers/images/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.243342 gando-0.9.8/src/gando/utils/strings/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/strings/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.243342 gando-0.9.8/src/gando/utils/strings/casings/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       98 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/strings/casings/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.243342 gando-0.9.8/src/gando/utils/strings/converters/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)     4898 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/strings/converters/__casing.py
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)       29 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/strings/converters/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.243342 gando-0.9.8/src/gando/utils/uploaders/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/uploaders/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.243342 gando-0.9.8/src/gando/utils/uploaders/files/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      405 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/uploaders/files/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.243342 gando-0.9.8/src/gando/utils/uploaders/images/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      407 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/uploaders/images/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.243342 gando-0.9.8/src/gando/utils/validators/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      344 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/validators/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.246676 gando-0.9.8/src/gando/utils/validators/slug/
+-rwxr-xr-x   0 nvd       (1000) nvd       (1000)      547 2024-01-03 03:41:35.000000 gando-0.9.8/src/gando/utils/validators/slug/__init__.py
+drwxr-xr-x   0 nvd       (1000) nvd       (1000)        0 2024-01-21 11:12:35.226676 gando-0.9.8/src/gando.egg-info/
+-rw-r--r--   0 nvd       (1000) nvd       (1000)     1590 2024-01-21 11:12:35.000000 gando-0.9.8/src/gando.egg-info/PKG-INFO
+-rw-r--r--   0 nvd       (1000) nvd       (1000)     3296 2024-01-21 11:12:35.000000 gando-0.9.8/src/gando.egg-info/SOURCES.txt
+-rw-r--r--   0 nvd       (1000) nvd       (1000)        1 2024-01-21 11:12:35.000000 gando-0.9.8/src/gando.egg-info/dependency_links.txt
+-rw-r--r--   0 nvd       (1000) nvd       (1000)       94 2024-01-21 11:12:35.000000 gando-0.9.8/src/gando.egg-info/requires.txt
+-rw-r--r--   0 nvd       (1000) nvd       (1000)        6 2024-01-21 11:12:35.000000 gando-0.9.8/src/gando.egg-info/top_level.txt
```

### Comparing `gando-0.9.7/LICENSE` & `gando-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/PKG-INFO` & `gando-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gando
-Version: 0.9.7
+Version: 0.9.8
 Summary: A framework based on Django that has tried to gather together the tools needed in the process of creating a large project.
 Home-page: https://github.com/navidsoleymani/gando.git
 Author: Hydra
 Author-email: navidsoleymani@ymail.com
 Project-URL: Documentation, https://github.com/navidsoleymani/gando.git
 Project-URL: Bug Reports, https://github.com/navidsoleymani/gando.git/issues
 Project-URL: Source Code, https://github.com/navidsoleymani/gando.git
```

### Comparing `gando-0.9.7/setup.py` & `gando-0.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/admin/models/__init__.py` & `gando-0.9.8/src/gando/admin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/architectures/apis/__base.py` & `gando-0.9.8/src/gando/architectures/apis/__base.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,19 @@
         self.__cookies_for_set: list = list()
         self.__cookies_for_delete: list = list()
 
         self.__content_type: str | None = None
         self.__exception_status: bool = False
 
     def handle_exception(self, exc):
+        if self.__debug_status is False or SETTINGS.EXCEPTION_HANDLER.HANDLING is False:
+            return self._handle_exception_gando_handling_false(exc)
+        return self._handle_exception_gando_handling_true(exc)
+
+    def _handle_exception_gando_handling_true(self, exc):
         """
         Handle any exception that occurs, by returning an appropriate response,
         or re-raising the error.
         """
         if isinstance(exc, (exceptions.NotAuthenticated,
                             exceptions.AuthenticationFailed)):
             # WWW-Authenticate header for 401 responses, else coerce to 403
@@ -69,34 +74,65 @@
         context = self.get_exception_handler_context()
         response = exception_handler(exc, context)
 
         if response is None:
             response = Response()
 
         self.set_exception_message(
-                key='unexpectedError',
-                value=exc.args[0]
-            )
+            key='unexpectedError',
+            value=exc.args[0]
+        )
         self.set_error_message(
-                key='unexpectedError',
-                value=(
-                    "An unexpected error has occurred based on your request type.\n"
-                    "Please do not repeat this request without changing your request.\n"
-                    "Be sure to read the documents on how to use this service correctly.\n"
-                    "In any case, discuss the issue with software support.\n"
-                )
+            key='unexpectedError',
+            value=(
+                "An unexpected error has occurred based on your request type.\n"
+                "Please do not repeat this request without changing your request.\n"
+                "Be sure to read the documents on how to use this service correctly.\n"
+                "In any case, discuss the issue with software support.\n"
             )
+        )
         self.set_warning_message(
-                key='unexpectedError',
-                value='Please discuss this matter with software support.',
+            key='unexpectedError',
+            value='Please discuss this matter with software support.',
+        )
+        if SETTINGS.EXCEPTION_HANDLER.COMMUNICATION_WITH_SOFTWARE_SUPPORT:
+            self.set_warning_message(
+                key='communicationWithSoftwareSupport',
+                value=f'{SETTINGS.EXCEPTION_HANDLER.COMMUNICATION_WITH_SOFTWARE_SUPPORT}',
             )
         self.set_status_code(421)
         response.exception = True
         return response
 
+    def _handle_exception_gando_handling_false(self, exc):
+        """
+        Handle any exception that occurs, by returning an appropriate response,
+        or re-raising the error.
+        """
+        if isinstance(exc, (exceptions.NotAuthenticated,
+                            exceptions.AuthenticationFailed)):
+            # WWW-Authenticate header for 401 responses, else coerce to 403
+            auth_header = self.get_authenticate_header(self.request)
+
+            if auth_header:
+                exc.auth_header = auth_header
+            else:
+                exc.status_code = status.HTTP_403_FORBIDDEN
+
+        exception_handler = self.get_exception_handler()
+
+        context = self.get_exception_handler_context()
+        response = exception_handler(exc, context)
+
+        if response is None:
+            self.raise_uncaught_exception(exc)
+
+        response.exception = True
+        return response
+
     def finalize_response(self, request, response, *args, **kwargs):
         if isinstance(response, Response):
             self.helper()
 
             tmp = response.template_name if hasattr(response, 'template_name') else None
             template_name = tmp
 
@@ -219,19 +255,19 @@
         ret = tmp
         return ret
 
     def __many(self):
         if isinstance(self.__data, list):
             return True
         if (
-                isinstance(self.__data, dict) and
-                'count' in self.__data and
-                'next' in self.__data and
-                'previous' in self.__data and
-                'results' in self.__data
+            isinstance(self.__data, dict) and
+            'count' in self.__data and
+            'next' in self.__data and
+            'previous' in self.__data and
+            'results' in self.__data
         ):
             return True
         return False
 
     def __success(self):
         if len(self.__errors_message) == 0 and len(self.__exceptions_message) == 0 and not self.__exception_status:
             return True
```

### Comparing `gando-0.9.7/src/gando/architectures/interfaces/__base.py` & `gando-0.9.8/src/gando/architectures/interfaces/__base.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/architectures/services/__base.py` & `gando-0.9.8/src/gando/architectures/services/__base.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/architectures/services/__creator.py` & `gando-0.9.8/src/gando/architectures/services/__creator.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/architectures/services/__database_manager.py` & `gando-0.9.8/src/gando/architectures/services/__database_manager.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/architectures/services/__getter.py` & `gando-0.9.8/src/gando/architectures/services/__getter.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/architectures/services/__getter_creator.py` & `gando-0.9.8/src/gando/architectures/services/__getter_creator.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/architectures/services/__updater.py` & `gando-0.9.8/src/gando/architectures/services/__updater.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/auth/__init__.py` & `gando-0.9.8/src/gando/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/http/requests/func/__asyncio.py` & `gando-0.9.8/src/gando/http/requests/func/__asyncio.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/http/requests/schemas/__request.py` & `gando-0.9.8/src/gando/http/requests/schemas/__request.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/http/responses/__json_response.py` & `gando-0.9.8/src/gando/http/responses/__json_response.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/http/responses/middlewares/__request_response_message.py` & `gando-0.9.8/src/gando/http/responses/middlewares/__request_response_message.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/http/responses/middlewares/__response_structured.py` & `gando-0.9.8/src/gando/http/responses/middlewares/__response_structured.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/http/responses/string_messages/__init__.py` & `gando-0.9.8/src/gando/http/responses/string_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/management/commands/startapi.py` & `gando-0.9.8/src/gando/management/commands/startapi.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/management/commands/startinterface.py` & `gando-0.9.8/src/gando/management/commands/startinterface.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/management/commands/startmodel.py` & `gando-0.9.8/src/gando/management/commands/startmodel.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/management/commands/startservice.py` & `gando-0.9.8/src/gando/management/commands/startservice.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/models/__init__.py` & `gando-0.9.8/src/gando/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/models/fields/__init__.py` & `gando-0.9.8/src/gando/models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/models/serializers/__init__.py` & `gando-0.9.8/src/gando/models/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/utils/converters/images/__small_blur_base64.py` & `gando-0.9.8/src/gando/utils/converters/images/__small_blur_base64.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/utils/hashers/__init__.py` & `gando-0.9.8/src/gando/utils/hashers/__init__.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/utils/parsers/images/__init__.py` & `gando-0.9.8/src/gando/utils/parsers/images/__init__.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/utils/strings/converters/__casing.py` & `gando-0.9.8/src/gando/utils/strings/converters/__casing.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando/utils/validators/slug/__init__.py` & `gando-0.9.8/src/gando/utils/validators/slug/__init__.py`

 * *Files identical despite different names*

### Comparing `gando-0.9.7/src/gando.egg-info/PKG-INFO` & `gando-0.9.8/src/gando.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gando
-Version: 0.9.7
+Version: 0.9.8
 Summary: A framework based on Django that has tried to gather together the tools needed in the process of creating a large project.
 Home-page: https://github.com/navidsoleymani/gando.git
 Author: Hydra
 Author-email: navidsoleymani@ymail.com
 Project-URL: Documentation, https://github.com/navidsoleymani/gando.git
 Project-URL: Bug Reports, https://github.com/navidsoleymani/gando.git/issues
 Project-URL: Source Code, https://github.com/navidsoleymani/gando.git
```

### Comparing `gando-0.9.7/src/gando.egg-info/SOURCES.txt` & `gando-0.9.8/src/gando.egg-info/SOURCES.txt`

 * *Files identical despite different names*

