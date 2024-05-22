# Comparing `tmp/alphaz-next-0.6.6.tar.gz` & `tmp/alphaz-next-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.6.6.tar", last modified: Mon May 13 11:49:57 2024, max compression
+gzip compressed data, was "alphaz-next-0.7.0.tar", last modified: Wed May 22 13:28:27 2024, max compression
```

## Comparing `alphaz-next-0.6.6.tar` & `alphaz-next-0.7.0.tar`

### file list

```diff
@@ -1,66 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.481963 alphaz-next-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-13 11:49:57.477963 alphaz-next-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.473962 alphaz-next-0.6.6/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.473962 alphaz-next-0.6.6/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/asyncio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.473962 alphaz-next-0.6.6/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.473962 alphaz-next-0.6.6/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.477963 alphaz-next-0.6.6/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/core/responses/ujson_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.477963 alphaz-next-0.6.6/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.469962 alphaz-next-0.6.6/alphaz_next/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.477963 alphaz-next-0.6.6/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.477963 alphaz-next-0.6.6/alphaz_next/models/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.477963 alphaz-next-0.6.6/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/models/config/directories_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/models/config/openapi_config_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.469962 alphaz-next-0.6.6/alphaz_next/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.477963 alphaz-next-0.6.6/alphaz_next/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.477963 alphaz-next-0.6.6/alphaz_next/tests/utils/mocking/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/tests/utils/mocking/mock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/tests/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.477963 alphaz-next-0.6.6/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/utils/logging_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-13 11:49:55.000000 alphaz-next-0.6.6/alphaz_next/utils/loguru.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:49:57.473962 alphaz-next-0.6.6/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-13 11:49:57.000000 alphaz-next-0.6.6/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-13 11:49:57.000000 alphaz-next-0.6.6/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:49:57.000000 alphaz-next-0.6.6/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-13 11:49:57.000000 alphaz-next-0.6.6/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 11:49:57.000000 alphaz-next-0.6.6/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:49:57.481963 alphaz-next-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-13 11:49:56.000000 alphaz-next-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.458244 alphaz-next-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-22 13:28:27.458244 alphaz-next-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.450245 alphaz-next-0.7.0/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/asyncio/async_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/ujson_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.458244 alphaz-next-0.7.0/alphaz_next/models/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.458244 alphaz-next-0.7.0/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/directories_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/openapi_config_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.458244 alphaz-next-0.7.0/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/utils/logging_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/utils/loguru.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.450245 alphaz-next-0.7.0/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-22 13:28:27.000000 alphaz-next-0.7.0/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-22 13:28:27.000000 alphaz-next-0.7.0/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:28:27.000000 alphaz-next-0.7.0/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 13:28:27.000000 alphaz-next-0.7.0/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 13:28:27.000000 alphaz-next-0.7.0/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:28:27.458244 alphaz-next-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-22 13:28:25.000000 alphaz-next-0.7.0/setup.py
```

### Comparing `alphaz-next-0.6.6/PKG-INFO` & `alphaz-next-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.6.6
-Summary: A project to make a lib to start FASTAPI quickly
+Version: 0.7.0
+Summary: A project to make a lib to start FastAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.6.6.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.0.tar.gz
 Author: Maxime MARTIN
-Author-email: maxime.martin02@hotmail.fr
+Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dependency-injector
 
 ## Alphaz-Next
 Alphaz-Next is a Python library designed to simplify the setup of REST APIs using FastAPI & Pydantic. It provides a useful toolkit for setting up Logger, Config, and more.
 
 ## Installing
```

### Comparing `alphaz-next-0.6.6/README.md` & `alphaz-next-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.6/alphaz_next/auth/auth.py` & `alphaz-next-0.7.0/alphaz_next/auth/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # MODULES
 from typing import (
     Annotated as _Annotated,
     Any as _Any,
     Dict as _Dict,
     List as _List,
-    Type,
-    TypeVar,
+    Type as _Type,
+    TypeVar as _TypeVar,
+    cast as _cast,
 )
 
 # FASTAPI
 from fastapi import Depends as _Depends, status as _status
 from fastapi.security import (
     APIKeyHeader as _APIKeyHeader,
     OAuth2PasswordBearer as _OAuth2PasswordBearer,
@@ -39,15 +40,15 @@
 )
 
 INTERNAL_CONFIG = _create_internal_config()
 
 API_KEY_HEADER = _APIKeyHeader(name="api_key", auto_error=False)
 OAUTH2_SCHEME = _OAuth2PasswordBearer(tokenUrl=INTERNAL_CONFIG.token_url)
 
-_T = TypeVar("_T", bound=_UserBaseSchema)
+_T = _TypeVar("_T", bound=_UserBaseSchema)
 
 
 def decode_token(token: str) -> _Dict[str, _Any]:
     """
     Decode a JWT token and return the payload.
 
     Args:
@@ -64,22 +65,22 @@
             token,
             INTERNAL_CONFIG.secret_key,
             algorithms=[INTERNAL_CONFIG.algorithm],
         )
     except _JWTError:
         raise _InvalidCredentialsError()
 
-    username: str = payload.get("sub")
+    username = _cast(str, payload.get("sub"))
     if username is None:
         raise _InvalidCredentialsError()
 
     return payload
 
 
-async def get_user(token: str, schema: Type[_T]) -> _T:
+async def get_user(token: str, schema: _Type[_T]) -> _T:
     """
     Retrieves user information using the provided token.
 
     Args:
         token (str): The authentication token.
         schema (Type[_T]): The schema type to validate the response against.
 
@@ -94,26 +95,27 @@
     headers = {
         "Authorization": f"Bearer {token}",
     }
 
     response = await _make_async_request_with_retry(
         method="POST",
         url=INTERNAL_CONFIG.user_me_url,
-        **{
-            "headers": headers,
-        },
+        headers=headers,
     )
 
-    return _post_process_http_response(
-        response,
-        schema=schema,
+    return _cast(
+        _T,
+        _post_process_http_response(
+            response,
+            schema=schema,
+        ),
     )
 
 
-async def get_api_key(api_key: str, schema: Type[_T]) -> _T:
+async def get_api_key(api_key: str, schema: _Type[_T]) -> _T:
     """
     Retrieves the API key using the provided `api_key` and returns the processed response.
 
     Args:
         api_key (str): The API key to be used for authentication.
         schema (Type[_T]): The type of the response schema.
 
@@ -123,22 +125,23 @@
     headers = {
         "api_key": api_key,
     }
 
     response = await _make_async_request_with_retry(
         method="POST",
         url=INTERNAL_CONFIG.api_key_me_url,
-        **{
-            "headers": headers,
-        },
+        headers=headers,
     )
 
-    return _post_process_http_response(
-        response,
-        schema=schema,
+    return _cast(
+        _T,
+        _post_process_http_response(
+            response,
+            schema=schema,
+        ),
     )
 
 
 def check_user_permissions(
     permissions: _List[str],
     user_permissions: _List[str],
 ) -> None:
@@ -155,15 +158,15 @@
     if len(permissions) > 0 and not any(
         [user_permission in permissions for user_permission in user_permissions]
     ):
         raise _NotEnoughPermissionsError()
 
 
 async def get_user_from_jwt(
-    schema: Type[_T],
+    schema: _Type[_T],
     security_scopes: _SecurityScopes,
     token: _Annotated[str, _Depends(OAUTH2_SCHEME)],
 ) -> _T:
     """
     Retrieves a user from a JWT token and performs permission checks.
 
     Args:
@@ -191,31 +194,31 @@
     except _InvalidCredentialsError as ex:
         raise _HTTPException(
             status_code=_status.HTTP_401_UNAUTHORIZED,
             headers={
                 "WWW-Authenticate": "Bearer",
             },
             ext_headers={
-                "status_description": ex.args,
+                "status_description": [str(item) for item in ex.args],
             },
         )
     except _NotEnoughPermissionsError as ex:
         raise _HTTPException(
             status_code=_status.HTTP_403_FORBIDDEN,
             headers={
                 "WWW-Authenticate": "Bearer",
             },
             ext_headers={
-                "status_description": ex.args,
+                "status_description": [str(item) for item in ex.args],
             },
         )
 
 
 async def get_user_from_api_key(
-    schema: Type[_T],
+    schema: _Type[_T],
     security_scopes: _SecurityScopes,
     api_key: _Annotated[
         str,
         _Depends(API_KEY_HEADER),
     ],
 ) -> _T:
     """
@@ -249,20 +252,20 @@
     except _InvalidCredentialsError as ex:
         raise _HTTPException(
             status_code=_status.HTTP_401_UNAUTHORIZED,
             headers={
                 "WWW-Authenticate": "Bearer",
             },
             ext_headers={
-                "status_description": ex.args,
+                "status_description": [str(item) for item in ex.args],
             },
         )
     except _NotEnoughPermissionsError as ex:
         raise _HTTPException(
             status_code=_status.HTTP_403_FORBIDDEN,
             headers={
                 "WWW-Authenticate": "Bearer",
             },
             ext_headers={
-                "status_description": ex.args,
+                "status_description": [str(item) for item in ex.args],
             },
         )
```

### Comparing `alphaz-next-0.6.6/alphaz_next/core/_base.py` & `alphaz-next-0.7.0/alphaz_next/core/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.6/alphaz_next/core/_middleware.py` & `alphaz-next-0.7.0/alphaz_next/core/_middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # MODULES
 import http
 import logging as _logging
 import time
-from typing import Optional, Sequence
+from typing import (
+    Any as _Any,
+    Callable as _Callable,
+    Optional as _Optional,
+    Sequence as _Sequence,
+)
 
 # FASTAPI
 from fastapi import Request, Response
 from fastapi.middleware.cors import CORSMiddleware as _CORSMiddleware
 
 # STARLETTE
 from starlette.types import ASGIApp
@@ -17,21 +22,21 @@
 uvicorn_logger = _logging.getLogger("uvicorn")
 
 
 class CORSMiddleware(_CORSMiddleware):
     def __init__(
         self,
         app: ASGIApp,
-        allow_origins: Sequence[str] = (),
-        allow_methods: Sequence[str] = ("GET",),
-        allow_headers: Sequence[str] = (),
+        allow_origins: _Sequence[str] = (),
+        allow_methods: _Sequence[str] = ("GET",),
+        allow_headers: _Sequence[str] = (),
         allow_credentials: bool = False,
         allow_private_network: bool = False,
-        allow_origin_regex: Optional[str] = None,
-        expose_headers: Sequence[str] = (),
+        allow_origin_regex: _Optional[str] = None,
+        expose_headers: _Sequence[str] = (),
         max_age: int = 600,
     ) -> None:
         super().__init__(
             app,
             allow_origins,
             allow_methods,
             allow_headers,
@@ -46,15 +51,18 @@
                 HeaderEnum.ACCESS_CONTROL_ALLOW_PRIVATE_NETWORK.value
             ] = "true"
             self.preflight_headers[
                 HeaderEnum.ACCESS_CONTROL_ALLOW_PRIVATE_NETWORK.value
             ] = "true"
 
 
-async def log_request_middleware(request: Request, call_next):
+async def log_request_middleware(
+    request: Request,
+    call_next: _Callable[..., _Any],
+) -> Response:
     """
     This middleware will log all requests and their processing time.
     E.g. log:
     0.0.0.0:1234 - GET /ping 200 OK 1.00ms
     """
     url = (
         f"{request.url.path}?{request.query_params}"
```

### Comparing `alphaz-next-0.6.6/alphaz_next/core/_telemetry.py` & `alphaz-next-0.7.0/alphaz_next/core/_telemetry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # MODULES
 import os as _os
 import logging as _logging
 import platform as _platform
 import psutil as _psutil
 from typing import (
+    Any as _Any,
     Dict as _Dict,
+    Generator as _Generator,
     Optional as _Optional,
     List as _List,
+    Tuple as _Tuple,
+    NamedTuple as _NamedTuple,
+    cast,
 )
 
 # FASTAPI
 from fastapi import FastAPI as _FastAPI
 
 # OPENTELEMETRY
 from opentelemetry import metrics, trace, _logs
@@ -19,179 +24,223 @@
 from opentelemetry.exporter.otlp.proto.http._log_exporter import OTLPLogExporter
 from opentelemetry.sdk.metrics import MeterProvider
 from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.sdk.resources import (
+    Attributes,
     Resource,
     SERVICE_NAME,
     SERVICE_VERSION,
     DEPLOYMENT_ENVIRONMENT,
     SERVICE_INSTANCE_ID,
 )
 from opentelemetry.sdk._logs import LoggerProvider, LoggingHandler
 from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
 from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
 from opentelemetry.instrumentation.system_metrics import (
     SystemMetricsInstrumentor as _SystemMetricsInstrumentor,
 )
 from opentelemetry.metrics import (
+    Meter,
     CallbackOptions,
     Observation,
 )
 
 # MODELS
 from alphaz_next.models.config.alpha_config import (
     AlphaConfigSchema as _AlphaConfigSchema,
 )
 
 
+class MemoryInfo(_NamedTuple):
+    vms: int
+    rss: int
+
+
 class SystemMetricsInstrumentor(_SystemMetricsInstrumentor):
 
     def __init__(
         self,
         labels: _Dict[str, str] | None = None,
-        config: _Dict[str, _List[str]] | None = None,
+        config: _Dict[str, _Optional[_List[str]]] | None = None,
     ):
-        super().__init__(labels, config)
+        super().__init__(labels, cast(_Dict[str, _List[str]], config))
 
         self._process = _psutil.Process()
         self._process.cpu_percent(interval=None)
 
         self._system_cpu_total_norm_pct_labels = self._labels.copy()
         self._system_memory_actual_free_labels = self._labels.copy()
         self._system_memory_total_labels = self._labels.copy()
         self._system_process_cpu_total_norm_pct_labels = self._labels.copy()
         self._system_process_memory_size_labels = self._labels.copy()
         self._system_process_memory_rss_byte_labels = self._labels.copy()
 
-    def _instrument(self, **kwargs):
-        super()._instrument(**kwargs)
+    def _instrument(self, **kwargs: _Any) -> None:
+        super()._instrument(**kwargs) # type: ignore
+
+        meter = cast(Meter, self._meter)
 
         if "system.cpu.total.norm.pct" in self._config:
-            self._meter.create_observable_gauge(
+            meter.create_observable_gauge(
                 name="system.cpu.total.norm.pct",
                 callbacks=[self._get_system_cpu_total_norm_pct],
                 description="System CPU total normalized percent",
             )
 
         if "system.memory.actual.free" in self._config:
-            self._meter.create_observable_gauge(
+            meter.create_observable_gauge(
                 name="system.memory.actual.free",
                 callbacks=[self._get_system_memory_actual_free],
                 description="System memory actual free",
             )
 
         if "system.memory.total" in self._config:
-            self._meter.create_observable_gauge(
+            meter.create_observable_gauge(
                 name="system.memory.total",
                 callbacks=[self._get_system_memory_total],
                 description="System memory total",
             )
 
         if "system.process.cpu.total.norm.pct" in self._config:
-            self._meter.create_observable_gauge(
+            meter.create_observable_gauge(
                 name="system.process.cpu.total.norm.pct",
                 callbacks=[self._get_system_process_cpu_total_norm_pct],
                 description="System process CPU total normalized percent",
             )
 
         if "system.process.memory.size" in self._config:
-            self._meter.create_observable_gauge(
+            meter.create_observable_gauge(
                 name="system.process.memory.size",
                 callbacks=[self._get_system_process_memory_size],
                 description="System process memory size",
             )
 
         if "system.process.memory.rss.byte" in self._config:
-            self._meter.create_observable_gauge(
+            meter.create_observable_gauge(
                 name="system.process.memory.rss.bytes",
                 callbacks=[self._get_system_process_memory_rss_byte],
                 description="System process memory rss bytes",
             )
 
-    def _get_process_infos(self, p: _psutil.Process):
+    def _get_process_infos(self, p: _psutil.Process) -> _Tuple[float, MemoryInfo]:
         if hasattr(p, "oneshot"):  # new in psutil 5.0
             with p.oneshot():
                 cpu_percent = p.cpu_percent(interval=None)
                 memory_info = p.memory_info()
         else:
             cpu_percent = p.cpu_percent(interval=None)
             memory_info = p.memory_info()
 
-        return cpu_percent, memory_info
+        return cpu_percent, cast(MemoryInfo, memory_info)
 
-    def _get_system_cpu_total_norm_pct(self, options: CallbackOptions):
+    def _get_system_cpu_total_norm_pct(
+        self,
+        options: CallbackOptions,
+    ) -> _Generator[Observation, None, None]:
         cpu_norm_percent = _psutil.cpu_percent(interval=None) / 100.0
         yield Observation(
             cpu_norm_percent,
             self._system_cpu_total_norm_pct_labels,
         )
 
-    def _get_system_memory_actual_free(self, options: CallbackOptions):
+    def _get_system_memory_actual_free(
+        self,
+        options: CallbackOptions,
+    ) -> _Generator[Observation, None, None]:
         memory = _psutil.virtual_memory()
         yield Observation(
             memory.available,
             self._system_memory_actual_free_labels,
         )
 
-    def _get_system_memory_total(self, options: CallbackOptions):
+    def _get_system_memory_total(
+        self,
+        options: CallbackOptions,
+    ) -> _Generator[Observation, None, None]:
         memory = _psutil.virtual_memory()
         yield Observation(
             memory.total,
             self._system_memory_total_labels,
         )
 
-    def _get_system_process_cpu_total_norm_pct(self, options: CallbackOptions):
+    def _get_system_process_cpu_total_norm_pct(
+        self,
+        options: CallbackOptions,
+    ) -> _Generator[Observation, None, None]:
         cpu_percent, _ = self._get_process_infos(p=self._process)
         yield Observation(
             cpu_percent / 100.0 / _psutil.cpu_count(),
             self._system_process_cpu_total_norm_pct_labels,
         )
 
-    def _get_system_process_memory_size(self, options: CallbackOptions):
+    def _get_system_process_memory_size(
+        self,
+        options: CallbackOptions,
+    ) -> _Generator[Observation, None, None]:
         _, memory_info = self._get_process_infos(p=self._process)
         yield Observation(
             memory_info.vms,
             self._system_process_memory_size_labels,
         )
 
-    def _get_system_process_memory_rss_byte(self, options: CallbackOptions):
+    def _get_system_process_memory_rss_byte(
+        self, options: CallbackOptions
+    ) -> _Generator[Observation, None, None]:
         _, memory_info = self._get_process_infos(p=self._process)
         yield Observation(
             memory_info.rss,
             self._system_process_memory_rss_byte_labels,
         )
 
 
+def _convert_os_headers(
+    env_variable_name: str,
+    default_headers: _Optional[_Dict[str, str]] = None,
+) -> _Optional[_Dict[str, str]]:
+    env_headers = _os.getenv(env_variable_name)
+    if env_headers is None:
+        return default_headers
+
+    key_value_pairs = env_headers.split(",")
+    result_dict: _Dict[str, str] = {}
+
+    for pair in key_value_pairs:
+        key, value = pair.split("=")
+        result_dict[key] = value
+
+    return result_dict
+
+
 def _setup_traces(
     default_endpoint: str,
-    default_headers: _Optional[str] = None,
+    resource: Resource,
+    default_headers: _Optional[_Dict[str, str]] = None,
     certificate_file: _Optional[str] = None,
-    resource: _Optional[Resource] = None,
 ) -> None:
     """
     Set up traces for telemetry.
 
     Args:
         default_endpoint (str): The default endpoint for exporting traces.
-        default_headers (str, optional): The default headers for exporting traces. Defaults to None.
+        resource (Resource): The resource for exporting traces.
+        default_headers (Dict[str, str], optional): The default headers for exporting traces.
         certificate_file (str, optional): The certificate file for exporting traces. Defaults to None.
-        resource (Resource, optional): The resource for exporting traces. Defaults to None.
     """
 
     endpoint = _os.environ.get(
         "OTEL_EXPORTER_OTLP_TRACES_ENDPOINT",
         f"{default_endpoint}/v1/traces",
     )
 
-    headers = _os.environ.get(
-        "OTEL_EXPORTER_OTLP_TRACES_HEADERS",
-        default_headers,
+    headers = _convert_os_headers(
+        env_variable_name="OTEL_EXPORTER_OTLP_TRACES_HEADERS",
+        default_headers=default_headers,
     )
 
     exporter = OTLPSpanExporter(
         endpoint=endpoint,
         certificate_file=certificate_file,
         headers=headers,
     )
@@ -202,40 +251,41 @@
     trace.set_tracer_provider(provider)
 
     provider = TracerProvider(resource=resource)
     provider.add_span_processor(processor)
 
 
 def _setup_metrics(
-    export_interval_millis: int,
     default_endpoint: str,
-    default_headers: _Optional[str] = None,
+    resource: Resource,
+    export_interval_millis: _Optional[float] = None,
+    default_headers: _Optional[_Dict[str, str]] = None,
     certificate_file: _Optional[str] = None,
-    resource: _Optional[Resource] = None,
     configuration: _Optional[_Dict[str, _Optional[_List[str]]]] = None,
-):
+) -> None:
     """
     Set up metrics configuration for telemetry.
 
     Args:
         default_endpoint (str): The default endpoint for exporting metrics.
-        default_headers (str, optional): The default headers for exporting metrics. Defaults to None.
+        resource (Resource): The resource for exporting traces.
+        export_interval_millis (float, optional): The interval for exporting metrics. Defaults to None.
+        default_headers (Dict[str, str], optional): The default headers for exporting traces.
         certificate_file (str, optional): The path to the certificate file. Defaults to None.
-        resource (Resource, optional): The resource associated with the metrics. Defaults to None.
         configuration (Dict[str, List[str]], optional): The configuration for the metrics. Defaults to None.
     """
 
     endpoint = _os.environ.get(
         "OTEL_EXPORTER_OTLP_METRICS_ENDPOINT",
         f"{default_endpoint}/v1/metrics",
     )
 
-    headers = _os.environ.get(
-        "OTEL_EXPORTER_OTLP_METRICS_HEADERS",
-        default_headers,
+    headers = _convert_os_headers(
+        env_variable_name="OTEL_EXPORTER_OTLP_METRICS_HEADERS",
+        default_headers=default_headers,
     )
 
     exporter = OTLPMetricExporter(
         endpoint=endpoint,
         certificate_file=certificate_file,
         headers=headers,
     )
@@ -250,54 +300,54 @@
     metrics.set_meter_provider(provider)
 
     SystemMetricsInstrumentor(config=configuration).instrument()
 
 
 def _setup_logs(
     default_endpoint: str,
-    default_headers: _Optional[str] = None,
+    resource: Resource,
+    default_headers: _Optional[_Dict[str, str]] = None,
     certificate_file: _Optional[str] = None,
-    resource: _Optional[Resource] = None,
 ) -> LoggingHandler:
     """
     Set up logs for telemetry.
 
     Args:
         default_endpoint (str): The default endpoint for exporting logs.
+        resource (Resource): The resource associated with the logs.
         default_headers (str, optional): The default headers for exporting logs. Defaults to None.
         certificate_file (str, optional): The path to the certificate file. Defaults to None.
-        resource (Resource, optional): The resource associated with the logs. Defaults to None.
 
     Returns:
         LoggingHandler: The logging handler for the telemetry logs.
     """
 
     endpoint = _os.environ.get(
         "OTEL_EXPORTER_OTLP_LOGS_ENDPOINT",
         f"{default_endpoint}/v1/logs",
     )
 
-    headers = _os.environ.get(
-        "OTEL_EXPORTER_OTLP_LOGS_HEADERS",
-        default_headers,
+    headers = _convert_os_headers(
+        env_variable_name="OTEL_EXPORTER_OTLP_LOGS_HEADERS",
+        default_headers=default_headers,
     )
 
     exporter = OTLPLogExporter(
         endpoint=endpoint,
         certificate_file=certificate_file,
         headers=headers,
     )
     logger_provider = LoggerProvider(resource=resource)
     logger_provider.add_log_record_processor(BatchLogRecordProcessor(exporter))
     _logs.set_logger_provider(logger_provider)
 
     return LoggingHandler(level=_logging.INFO, logger_provider=logger_provider)
 
 
-def setup_telemetry(config: _AlphaConfigSchema, app: _FastAPI):
+def setup_telemetry(config: _AlphaConfigSchema, app: _FastAPI) -> None:
     """
     Sets up OpenTelemetry for the application.
 
     Args:
         config (_AlphaConfigSchema): The configuration object.
         app (_FastAPI): The FastAPI application object.
 
@@ -310,17 +360,16 @@
 
     otel_service_name = config.project_name
     apm_server_url = config.api_config.apm.server_url
     certificate_path = config.api_config.apm.certificate_file
     environment = config.environment.lower()
     version = config.version
 
-    otel_exporter_otlp_headers = _os.environ.get(
-        "OTEL_EXPORTER_OTLP_HEADERS",
-        None,
+    otel_exporter_otlp_headers = _convert_os_headers(
+        env_variable_name="OTEL_EXPORTER_OTLP_HEADERS"
     )
 
     otel_exporter_otlp_endpoint = _os.environ.get(
         "OTEL_EXPORTER_OTLP_ENDPOINT",
         apm_server_url,
     )
 
@@ -336,15 +385,15 @@
     key_value_pairs = resource_attributes.split(",")
     result_dict = {}
 
     for pair in key_value_pairs:
         key, value = pair.split("=")
         result_dict[key] = value
 
-    resourceAttributes = {
+    resourceAttributes: Attributes = {
         SERVICE_NAME: otel_service_name,
         SERVICE_INSTANCE_ID: _platform.node(),
         SERVICE_VERSION: result_dict["service.version"],
         DEPLOYMENT_ENVIRONMENT: result_dict["deployment.environment"],
     }
 
     resource = Resource.create(resourceAttributes)
```

### Comparing `alphaz-next-0.6.6/alphaz_next/core/application.py` & `alphaz-next-0.7.0/alphaz_next/core/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # MODULES
 from logging.handlers import TimedRotatingFileHandler
 from pathlib import Path
 import sys as _sys
 from typing import (
+    Annotated,
     Any as _Any,
-    AsyncContextManager as _AsyncContextManager,
     Dict as _Dict,
     List as _List,
     Optional as _Optional,
     Sequence as _Sequence,
     Union as _Union,
 )
 import logging as _logging
@@ -26,22 +26,26 @@
 from fastapi.exception_handlers import (
     request_validation_exception_handler as _request_validation_exception_handler,
 )
 from fastapi.openapi.docs import (
     get_swagger_ui_html as _get_swagger_ui_html,
     get_redoc_html as _get_redoc_html,
 )
-from fastapi.openapi.utils import get_openapi as _get_openapi, BaseRoute as _BaseRoute
+from fastapi.openapi.utils import get_openapi as _get_openapi
 from fastapi.responses import (
     HTMLResponse as _HTMLResponse,
     JSONResponse as _JSONResponse,
     PlainTextResponse as _PlainTextResponse,
     RedirectResponse as _RedirectResponse,
 )
 
+# STARLETTE
+from starlette.routing import BaseRoute as _BaseRoute
+from starlette.types import Lifespan as _Lifespan
+
 # MODELS
 from alphaz_next.models.config.alpha_config import (
     AlphaConfigSchema as _AlphaConfigSchema,
 )
 
 # CORE
 from alphaz_next.core._middleware import (
@@ -61,15 +65,16 @@
 _uvicorn_access = _logging.getLogger("uvicorn.access")
 _uvicorn_access.disabled = True
 
 uvicorn_logger = _logging.getLogger("uvicorn")
 
 
 def _custom_openapi(
-    config: _AlphaConfigSchema, routes: _List[_BaseRoute]
+    config: _AlphaConfigSchema,
+    routes: _List[_BaseRoute],
 ) -> _Dict[str, _Any]:
     """
     Generate a custom OpenAPI schema based on the provided configuration and routes.
 
     Args:
         config (AlphaConfigSchema): The configuration object containing project settings.
         routes (List[BaseRoute]): The list of routes to include in the OpenAPI schema.
@@ -77,23 +82,23 @@
     Returns:
         Dict[str, Any]: The generated OpenAPI schema.
     """
     title = config.project_name.upper()
     if config.environment.lower() != "prod":
         title = f"{title} [{config.environment.upper()}]"
 
-    openapi_dict = {}
+    openapi_dict: _Dict[str, _Any] = {}
     if (openapi_config := config.api_config.openapi) is not None:
         openapi_dict["description"] = openapi_config.description
         openapi_dict["tags"] = openapi_config.tags
 
         if openapi_config.contact is not None:
             openapi_dict["contact"] = {
-                "name": config.api_config.openapi.contact.name,
-                "email": config.api_config.openapi.contact.email,
+                "name": openapi_config.contact.name,
+                "email": openapi_config.contact.email,
             }
 
     openapi_schema = _get_openapi(
         title=title,
         version=config.version,
         routes=routes,
         **openapi_dict,
@@ -102,21 +107,21 @@
     return openapi_schema
 
 
 def create_app(
     config: _AlphaConfigSchema,
     routes: _Optional[_List[_BaseRoute]] = None,
     routers: _Optional[_List[_APIRouter]] = None,
-    lifespan: _Optional[_AsyncContextManager] = None,
+    lifespan: _Optional[_Lifespan[_FastAPI]] = None,
     allow_origins: _Sequence[str] = (),
     allow_methods: _Sequence[str] = ("GET",),
     allow_headers: _Sequence[str] = (),
     allow_credentials: bool = False,
     allow_private_network: bool = False,
-    status_response: _Dict = {"status": "OK"},
+    status_response: _Dict[str, _Any] = {"status": "OK"},
 ) -> _FastAPI:
     """
     Create a FastAPI application with the specified configuration.
 
     Args:
         config (AlphaConfigSchema): The configuration for the application.
         routes (Optional[List[BaseRoute]]): The list of routes to include in the application. Defaults to None.
@@ -152,15 +157,16 @@
         allow_private_network=allow_private_network,
     )
 
     app.middleware("http")(_log_request_middleware)
 
     setup_telemetry(config=config, app=app)
 
-    [app.include_router(router) for router in routers or []]
+    for router in routers or []:
+        app.include_router(router)
 
     app.openapi_schema = _custom_openapi(config=config, routes=app.routes)
 
     swagger_favicon_url = _DEFAULT_FAVICON_URL
     redoc_favicon_url = _DEFAULT_FAVICON_URL
     if (openapi_config := config.api_config.openapi) is not None:
         if openapi_config.swagger_favicon_url:
@@ -168,14 +174,15 @@
 
         if openapi_config.redoc_favicon_url:
             redoc_favicon_url = openapi_config.redoc_favicon_url
 
     if (
         config.api_config.logging is not None
         and config.api_config.logging.rotation is not None
+        and config.api_config.logging.retention is not None
     ):
         uvicorn_formatter = _logging.Formatter(
             config.api_config.logging.uvicorn_format,
             datefmt=config.api_config.logging.date_format,
         )
 
         directory_path = Path(config.api_config.directories.logs)
@@ -249,40 +256,48 @@
 
         uvicorn_logger.error(
             f'{host}:{port} - "{request.method} {url}" 500 Internal Server Error <{exception_name}: {exception_value}>'
         )
         return _PlainTextResponse(str(exc), status_code=500)
 
     @app.get("/status", include_in_schema=False)
-    async def get_api_status():
+    async def get_api_status() -> _Dict[str, _Any]:
         return status_response
 
     @app.get("/docs", include_in_schema=False)
     def swagger_ui_html(req: _Request) -> _HTMLResponse:
         root_path = req.scope.get("root_path", "").rstrip("/")
-        openapi_url = root_path + app.openapi_url
+
+        openapi_url = root_path
+        if app.openapi_url is not None:
+            openapi_url += app.openapi_url
+
         oauth2_redirect_url = app.swagger_ui_oauth2_redirect_url
         if oauth2_redirect_url:
             oauth2_redirect_url = root_path + oauth2_redirect_url
 
         return _get_swagger_ui_html(
             openapi_url=openapi_url,
             title=app.title + " - Swagger UI",
             oauth2_redirect_url=oauth2_redirect_url,
             init_oauth=app.swagger_ui_init_oauth,
             swagger_favicon_url=swagger_favicon_url,
             swagger_ui_parameters=app.swagger_ui_parameters,
         )
 
     @app.get("/redoc", include_in_schema=False)
-    async def redoc_html():
+    async def redoc_html() -> _HTMLResponse:
+        if app.openapi_url is None:
+            raise _HTTPException(
+                status_code=404, detail="No OpenAPI URL has been provided."
+            )
         return _get_redoc_html(
             openapi_url=app.openapi_url,
             title=app.title + " - ReDoc",
             redoc_favicon_url=redoc_favicon_url,
         )
 
     @app.get("/")
-    async def home():
+    async def home() -> _RedirectResponse:
         return _RedirectResponse("/docs")
 
     return app
```

### Comparing `alphaz-next-0.6.6/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.7.0/alphaz_next/core/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.6/alphaz_next/core/exceptions.py` & `alphaz-next-0.7.0/alphaz_next/core/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 class InvalidCredentialsError(Exception):
     """Exception raised for invalid credentials.
 
     Attributes:
         None
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__("Could not validate credentials")
 
 
 class NotEnoughPermissionsError(Exception):
     """Exception raised when there are not enough permissions."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__("Not enough permissions")
 
 
 class HTTPException(_HTTPException):
 
     def __init__(
         self,
```

### Comparing `alphaz-next-0.6.6/alphaz_next/core/responses/__init__.py` & `alphaz-next-0.7.0/alphaz_next/core/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.6/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.7.0/alphaz_next/core/responses/file_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MODULES
 from os import PathLike as _PathLike, stat_result as _stat_result
-from typing import Mapping as _Mapping
+from typing import Dict as _Dict
 
 # FASTAPI
 from fastapi.responses import FileResponse as _FileResponse
 
 # STARLETTE
 from starlette.background import BackgroundTask as _BackgroundTask
 
@@ -20,15 +20,15 @@
     Represents a file response that can be returned by an HTTP endpoint.
     """
 
     def __init__(
         self,
         path: str | _PathLike[str],
         status_code: int = 200,
-        headers: _Mapping[str, str] | None = None,
+        headers: _Dict[str, str] | None = None,
         ext_headers: _ExtHeaders | None = None,
         media_type: str | None = None,
         background: _BackgroundTask | None = None,
         filename: str | None = None,
         stat_result: _stat_result | None = None,
         method: str | None = None,
         content_disposition_type: str = "attachment",
```

### Comparing `alphaz-next-0.6.6/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.7.0/alphaz_next/core/responses/html_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MODULES
-from typing import Any as _Any, Mapping as _Mapping
+from typing import Any as _Any, Dict as _Dict
 
 # FASTAPI
 from fastapi.responses import HTMLResponse as _HTMLResponse
 
 # STARLETTE
 from starlette.background import BackgroundTask as _BackgroundTask
 
@@ -19,15 +19,15 @@
     Represents a HTML response that can be returned by an HTTP endpoint.
     """
 
     def __init__(
         self,
         content: _Any = None,
         status_code: int = 200,
-        headers: _Mapping[str, str] | None = None,
+        headers: _Dict[str, str] | None = None,
         ext_headers: _ExtHeaders | None = None,
         media_type: str | None = None,
         background: _BackgroundTask | None = None,
     ) -> None:
         """
         Initializes a new instance of the HTMLResponse class.
```

### Comparing `alphaz-next-0.6.6/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.7.0/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.6/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.7.0/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.6/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.7.0/alphaz_next/core/responses/plaintext_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MODULES
-from typing import Any as _Any, Mapping as _Mapping
+from typing import Any as _Any, Dict as _Dict
 
 # FASTAPI
 from fastapi.responses import PlainTextResponse as _PlainTextResponse
 
 # STARLETTE
 from starlette.background import BackgroundTask as _BackgroundTask
 
@@ -19,15 +19,15 @@
     Represents a Plain Text response that can be returned by an HTTP endpoint.
     """
 
     def __init__(
         self,
         content: _Any = None,
         status_code: int = 200,
-        headers: _Mapping[str, str] | None = None,
+        headers: _Dict[str, str] | None = None,
         ext_headers: _ExtHeaders | None = None,
         media_type: str | None = None,
         background: _BackgroundTask | None = None,
     ) -> None:
         """
         Initializes a new instance of the PlainTextResponse class.
```

### Comparing `alphaz-next-0.6.6/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.7.0/alphaz_next/core/responses/redirect_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MODULES
-from typing import Mapping as _Mapping
+from typing import Dict as _Dict
 
 # FASTAPI
 from fastapi.responses import RedirectResponse as _RedirectResponse
 
 # STARLETTE
 from starlette.background import BackgroundTask as _BackgroundTask
 from starlette.datastructures import URL as _URL
@@ -20,15 +20,15 @@
     Represents a Redirect response that can be returned by an HTTP endpoint.
     """
 
     def __init__(
         self,
         url: str | _URL,
         status_code: int = 307,
-        headers: _Mapping[str, str] | None = None,
+        headers: _Dict[str, str] | None = None,
         ext_headers: _ExtHeaders | None = None,
         background: _BackgroundTask | None = None,
     ) -> None:
         """
         Initializes a new instance of the RedirectResponse class.
 
         Args:
```

### Comparing `alphaz-next-0.6.6/alphaz_next/core/responses/response.py` & `alphaz-next-0.7.0/alphaz_next/core/responses/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MODULES
-from typing import Any as _Any, Mapping as _Mapping
+from typing import Any as _Any, Dict as _Dict
 
 # FASTAPI
 from fastapi.responses import Response as _Response
 
 # STARLETTE
 from starlette.background import BackgroundTask as _BackgroundTask
 
@@ -19,15 +19,15 @@
     Represents a Response that can be returned by an HTTP endpoint.
     """
 
     def __init__(
         self,
         content: _Any = None,
         status_code: int = 200,
-        headers: _Mapping[str, str] | None = None,
+        headers: _Dict[str, str] | None = None,
         ext_headers: _ExtHeaders | None = None,
         media_type: str | None = None,
         background: _BackgroundTask | None = None,
     ) -> None:
         """
         Initializes a new instance of the Response class.
```

### Comparing `alphaz-next-0.6.6/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.7.0/alphaz_next/core/responses/streaming_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MODULES
-from typing import Mapping as _Mapping
+from typing import Dict as _Dict
 
 # FASTAPI
 from fastapi.responses import StreamingResponse as _StreamingResponse
 
 # STARLETTE
 from starlette.background import BackgroundTask as _BackgroundTask
 from starlette.responses import ContentStream as _ContentStream
@@ -20,15 +20,15 @@
     Represents a StreamingResponse that can be returned by an HTTP endpoint.
     """
 
     def __init__(
         self,
         content: _ContentStream,
         status_code: int = 200,
-        headers: _Mapping[str, str] | None = None,
+        headers: _Dict[str, str] | None = None,
         ext_headers: _ExtHeaders | None = None,
         media_type: str | None = None,
         background: _BackgroundTask | None = None,
     ) -> None:
         """
         Initializes a new instance of the StreamingResponse class.
```

### Comparing `alphaz-next-0.6.6/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.7.0/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.6/alphaz_next/libs/httpx.py` & `alphaz-next-0.7.0/alphaz_next/libs/httpx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 # MODULES
 import asyncio
 import time
-from typing import Any, List, Literal, Optional, Type, TypeVar, Union
+from typing import (
+    Any as _Any,
+    Dict as _Dict,
+    List as _List,
+    Literal as _Literal,
+    Optional as _Optional,
+    Type as _Type,
+    TypeVar as _TypeVar,
+    Union as _Union,
+)
 
 # FASTAPI
 from fastapi import HTTPException
 
+# PYDANTIC
+from pydantic import BaseModel
+
 # HTTPX
 import httpx
-from pydantic import BaseModel
 
 
 def make_request_with_retry(
-    method: Literal["POST", "PATCH", "PUT", "DELETE", "GET"],
+    method: _Literal["POST", "PATCH", "PUT", "DELETE", "GET"],
     url: str,
     max_retries: int = 3,
-    retry_on_status: Optional[List[int]] = None,
-    timeout: Optional[float] = None,
-    **kwargs,
+    retry_on_status: _Optional[_List[int]] = None,
+    timeout: _Optional[float] = None,
+    **kwargs: _Any,
 ) -> httpx.Response:
     """
     Makes an HTTP request with retries in case of a timeout error.
 
     Args:
         method (Literal["POST", "PATCH", "PUT", "DELETE", "GET"]): The HTTP method to use.
         url (str): The URL to make the request to.
@@ -71,20 +82,20 @@
         else:
             return response
 
     raise RuntimeError(f"Maximum number of retries exceeded {item_repr}")
 
 
 async def make_async_request_with_retry(
-    method: Literal["POST", "PATCH", "PUT", "DELETE", "GET"],
+    method: _Literal["POST", "PATCH", "PUT", "DELETE", "GET"],
     url: str,
     max_retries: int = 3,
-    retry_on_status: Optional[List[int]] = None,
-    timeout: Optional[float] = None,
-    **kwargs,
+    retry_on_status: _Optional[_List[int]] = None,
+    timeout: _Optional[float] = None,
+    **kwargs: _Any,
 ) -> httpx.Response:
     """
     Makes an HTTP request with retries in case of a timeout error.
 
     Args:
         method (Literal["POST", "PATCH", "PUT", "DELETE", "GET"]): The HTTP method to use.
         url (str): The URL to make the request to.
@@ -133,22 +144,22 @@
             ) from ex
         else:
             return response
 
     raise RuntimeError(f"Maximum number of retries exceeded {item_repr}")
 
 
-T = TypeVar("T", bound=BaseModel)
+_T = _TypeVar("_T", bound=BaseModel)
 
 
 def post_process_http_response(
     response: httpx.Response,
-    schema: Type[T] = None,
+    schema: _Optional[_Type[_T]] = None,
     mode_alpha: bool = False,
-) -> Union[T, List[T], Any]:
+) -> _Union[_T, _List[_T], _Any]:
     """
     Processes an HTTP response and returns the response body as a validated object or a list of validated objects.
 
     Args:
         response: The HTTP response to process.
         schema: The schema to use for validating the response body.
         mode_alpha: Whether to use the "data" key in the response body for validation.
@@ -159,15 +170,15 @@
     Raises:
         HTTPException: If the response is not a success.
     """
     if not response.is_success:
         raise HTTPException(
             status_code=response.status_code,
             detail=response.text,
-            headers=response.headers,
+            headers={k: v for k, v in response.headers.items()},
         )
 
     response_json = response.json()
     if mode_alpha:
         response_json = response_json.get("data")
 
     if schema is None:
```

### Comparing `alphaz-next-0.6.6/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.7.0/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,44 @@
+from typing import Protocol as _Protocol
+
 # PYDANTIC
 from pydantic import Field
 from pydantic_settings import BaseSettings
 
 
+class AlphaInternalConfigProtocol(_Protocol):
+    token_url: str
+    user_me_url: str
+    api_key_me_url: str
+    secret_key: str
+    algorithm: str
+
+
 def create_internal_config(
     token_url_alias: str = "ALPHA_TOKEN_URL",
     user_me_url_alias: str = "ALPHA_USER_ME_URL",
     api_key_me_url_alias: str = "ALPHA_API_KEY_ME_URL",
     secret_key_alias: str = "ALPHA_SECRET_KEY",
     algorithm_alias: str = "ALPHA_ALGORITHM",
-):
+) -> AlphaInternalConfigProtocol:
     """
     Create an instance of the AlphaInternalConfigSettingsSchema class with the provided configuration settings.
 
     Args:
         token_url_alias (str, optional): The alias for the token URL. Defaults to "ALPHA_TOKEN_URL".
         user_me_url_alias (str, optional): The alias for the user me URL. Defaults to "ALPHA_USER_ME_URL".
         api_key_me_url_alias (str, optional): The alias for the API key me URL. Defaults to "ALPHA_API_KEY_ME_URL".
         secret_key_alias (str, optional): The alias for the secret key. Defaults to "ALPHA_SECRET_KEY".
         algorithm_alias (str, optional): The alias for the algorithm. Defaults to "ALPHA_ALGORITHM".
 
     Returns:
         AlphaInternalConfigSettingsSchema: An instance of the AlphaInternalConfigSettingsSchema class.
     """
 
-    class AlphaInternalConfigSettingsSchema(BaseSettings):
+    class AlphaInternalConfigSettingsSchema(BaseSettings, AlphaInternalConfigProtocol):
         token_url: str = Field(
             default="/auth",
             validation_alias=token_url_alias,
         )
         user_me_url: str = Field(
             default="user/me",
             validation_alias=user_me_url_alias,
```

### Comparing `alphaz-next-0.6.6/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.7.0/alphaz_next/models/config/_base/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # MODULES
 import getpass
 import os
 import re
-from typing import Any, Dict, TypedDict
+from typing import Any, Dict, List, TypeVar, TypedDict, Union, cast
 from pathlib import Path
 
 # LIBS
 from alphaz_next.libs.file_lib import open_json_file
 
 
 _CONFIG_PATTERN = r"\$config\(([^)]*)\)"
 
+_T = TypeVar("_T", bound=Union[List[Dict[str, Any]], Dict[str, Any]])
+
 
 class ReservedConfigItem(TypedDict):
     """
     Represents a reserved configuration item.
 
     Attributes:
         environment (str): The environment.
@@ -24,17 +26,17 @@
 
     environment: str
     root: str
     project_name: str
 
 
 def replace_reserved_config(
-    config: Dict,
+    config: _T,
     reserved_config: ReservedConfigItem,
-) -> Dict:
+) -> _T:
     """
     Replaces reserved variables in the configuration dictionary with their corresponding values.
 
     Args:
         config (Dict): The original configuration dictionary.
         reserved_config (ReservedConfigItem): The reserved configuration item containing the values for the reserved variables.
 
@@ -55,28 +57,39 @@
         result = match.group(1)
 
         result = open_json_file(Path(result))
 
         return traverse(result)
 
     def replace_variable(value: Any) -> Any:
+        if not isinstance(value, str):
+            return value
+
+        root = reserved_config.get("root")
+        project_name = reserved_config.get("project_name")
+        environment = reserved_config.get("environment")
+
+        if root is not None:
+            value.replace("{{root}}", root)
+
+        if project_name is not None:
+            value.replace("{{project_name}}", project_name)
+
+        if environment is not None:
+            value.replace("{{environment}}", environment)
+
         return (
-            (
-                value.replace("{{root}}", reserved_config.get("root"))
-                .replace("{{home}}", os.path.expanduser("~"))
-                .replace("{{project_name}}", reserved_config.get("project_name"))
-                .replace("{{user}}", getpass.getuser())
-                .replace("{{project}}", os.path.abspath(os.getcwd()))
-                .replace("{{environment}}", reserved_config.get("environment"))
-            )
-            if isinstance(value, str)
-            else value
+            value.replace("{{home}}", os.path.expanduser("~"))
+            .replace("{{user}}", getpass.getuser())
+            .replace("{{project}}", os.path.abspath(os.getcwd()))
         )
 
-    def traverse(obj: Any) -> Any:
+    def traverse(
+        obj: Union[List[Dict[str, Any]], Dict[str, Any]]
+    ) -> Union[List[Dict[str, Any]], Dict[str, Any]]:
         if isinstance(obj, dict):
             for key, value in obj.items():
                 if isinstance(value, (dict, list)):
                     traverse(value)
                 else:
                     replaced_variable = replace_variable(value)
                     obj[key] = open_child_config(replaced_variable)
@@ -86,8 +99,8 @@
                     traverse(value)
                 else:
                     replaced_variable = replace_variable(value)
                     obj[i] = open_child_config(replaced_variable)
 
         return obj
 
-    return traverse(replaced_config)
+    return cast(_T, traverse(replaced_config))
```

### Comparing `alphaz-next-0.6.6/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.7.0/alphaz_next/models/config/alpha_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,28 +42,41 @@
     port: int
     workers: int
 
     api_config: _AlphaApiConfigSchema
 
     @_model_validator(mode="before")
     @classmethod
-    def validate_model(cls, data: _Dict[str, _Any]) -> _Dict:
+    def validate_model(cls, data: _Dict[str, _Any]) -> _Dict[str, _Any]:
+        environment = data.get("environment")
+        root = data.get("root")
+        project_name = data.get("project_name")
+
+        if environment is None or root is None or project_name is None:
+            raise ValueError("Environment, root, and project name must be provided.")
+
         tmp = _replace_reserved_config(
             data,
             reserved_config=_ReservedConfigItem(
-                environment=data.get("environment"),
-                root=data.get("root"),
-                project_name=data.get("project_name"),
+                environment=environment,
+                root=root,
+                project_name=project_name,
             ),
         )
 
+        root = tmp.get("root")
+        project_name = tmp.get("project_name")
+
+        if root is None or project_name is None:
+            raise ValueError("Root and project name must be provided.")
+
         reserved_fields = _ReservedConfigItem(
-            environment=data.get("environment"),
-            root=tmp.get("root"),
-            project_name=tmp.get("project_name"),
+            environment=environment,
+            root=root,
+            project_name=project_name,
         )
 
         for key, value in tmp.items():
             if isinstance(value, dict):
                 tmp[key]["__reserved_fields__"] = reserved_fields
 
         return tmp
```

### Comparing `alphaz-next-0.6.6/alphaz_next/models/config/api_config.py` & `alphaz-next-0.7.0/alphaz_next/models/config/api_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.6/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.7.0/alphaz_next/models/config/apm_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.6/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.7.0/alphaz_next/models/config/config_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MODULES
 from pathlib import Path as _Path
-from typing import Type as _Type, TypeVar as _TypeVar
+from typing import Any, Dict, Type as _Type, TypeVar as _TypeVar, cast
 
 # PYDANTIC
 from pydantic import Field as _Field, computed_field as _computed_field
 from pydantic_settings import BaseSettings as _BaseSettings
 
 # LIBS
 from alphaz_next.libs.file_lib import open_json_file as _open_json_file
@@ -18,15 +18,15 @@
 def create_config_settings(
     path: _Path,
     model: _Type[_T],
     environment_alias: str = "ALPHA_ENV",
     root_alias: str = "ALPHA_ROOT",
     port_alias: str = "ALPHA_PORT",
     workers_alias: str = "ALPHA_WORKERS",
-):
+) -> _T:
     """
     Create configuration settings based on the provided parameters.
 
     Args:
         path (Path): The path to the JSON file containing the configuration data.
         model (Type[_T]): The model class used for validating the configuration data.
         environment_alias (str, optional): The alias for the environment field in the JSON file. Defaults to "ALPHA_ENV".
@@ -40,18 +40,18 @@
 
     class AlphaConfigSettingsSchema(_BaseSettings):
         environment: str = _Field(default="local", validation_alias=environment_alias)
         root: str = _Field(default=str(_Path.cwd()), validation_alias=root_alias)
         port: int = _Field(default=8000, validation_alias=port_alias)
         workers: int = _Field(default=1, validation_alias=workers_alias)
 
-        @_computed_field
         @property
+        @_computed_field
         def main_config(self) -> _T:
-            data = _open_json_file(path=_Path(path))
+            data = cast(Dict[str, Any], _open_json_file(path=_Path(path)))
 
             data_ext = {
                 "environment": self.environment,
                 "root": self.root,
                 "port": self.port,
                 "workers": self.workers,
             }
```

### Comparing `alphaz-next-0.6.6/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.7.0/alphaz_next/models/config/logging_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# PYDANTIC
+# MODULES
+import logging as _logging
 from typing import Annotated as _Annotated, List as _List, Optional as _Optional
-from loguru import _defaults
+
+# OPENTELEMETRY
 from opentelemetry.instrumentation.logging import LoggingInstrumentor
 
 # PYDANTIC
 from pydantic_core.core_schema import FieldValidationInfo as _FieldValidationInfo
 from pydantic import (
     BaseModel as _BaseModel,
     ConfigDict as _ConfigDict,
     Field as _Field,
     StringConstraints as _StringConstraints,
     computed_field as _computed_field,
     field_validator as _field_validator,
 )
 
 LOGGING_LEVEL = {
-    "CRITICAL": _defaults.LOGURU_CRITICAL_NO,
-    "ERROR": _defaults.LOGURU_ERROR_NO,
-    "WARNING": _defaults.LOGURU_WARNING_NO,
-    "SUCCESS": _defaults.LOGURU_SUCCESS_NO,
-    "INFO": _defaults.LOGURU_INFO_NO,
-    "DEBUG": _defaults.LOGURU_DEBUG_NO,
-    "TRACE": _defaults.LOGURU_TRACE_NO,
+    "CRITICAL": _logging.CRITICAL,
+    "ERROR": _logging.ERROR,
+    "WARNING": _logging.WARNING,
+    "INFO": _logging.INFO,
+    "DEBUG": _logging.DEBUG,
 }
 
 
 class LoggingSchema(_BaseModel):
     """
     Represents the configuration schema for logging.
 
@@ -53,25 +53,25 @@
     date_format: str
     rotation: _Optional[str] = _Field(default=None)
     retention: _Optional[int] = _Field(default=None)
     excluded_routers: _List[str] = _Field(default_factory=lambda: [])
 
     @_field_validator("format")
     @classmethod
-    def validate_format(cls, value: str, info: _FieldValidationInfo):
+    def validate_format(cls, value: str, info: _FieldValidationInfo) -> str:
         if value is not None:
             LoggingInstrumentor().instrument(logging_format=value)
 
         return value
 
     @_field_validator("level")
     @classmethod
-    def validate_level(cls, value: str, info: _FieldValidationInfo):
+    def validate_level(cls, value: str, info: _FieldValidationInfo) -> str:
         if value not in LOGGING_LEVEL:
             raise ValueError(f"{info.field_name} is not valid")
 
         return value
 
-    @_computed_field
     @property
+    @_computed_field
     def level_code(self) -> int:
         return LOGGING_LEVEL.get(self.level.upper(), 0)
```

### Comparing `alphaz-next-0.6.6/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.7.0/alphaz_next/models/config/openapi_config_schema.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.6.6/alphaz_next/utils/format.py` & `alphaz-next-0.7.0/alphaz_next/utils/format.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # MODULES
 from enum import Enum as _Enum
 from typing import (
     Any as _Any,
     Dict as _Dict,
     List as _List,
     Optional as _Optional,
+    Set as _Set,
     Tuple as _Tuple,
     Type as _Type,
     TypeVar as _TypeVar,
     Union as _Union,
 )
 
 # PYDANTIC
 from pydantic import BaseModel as _BaseModel
 
 # SQLALCHEMY
 from sqlalchemy.orm import (
+    DeclarativeBase,
     InstrumentedAttribute as _InstrumentedAttribute,
     RelationshipProperty as _RelationshipProperty,
-    declarative_base as _declarative_base,
 )
 
-_T = _TypeVar("_T", bound=_declarative_base())
+_T = _TypeVar("_T", bound=DeclarativeBase)
 
 
-def uppercase(items: _List[str] | str) -> _List[str] | str:
+def uppercase(
+    items: _Optional[_Union[_List[str], _Set[str], str]],
+) -> _Optional[_Union[_List[str], _Set[str], str]]:
     """
     Converts the given string or list of strings to uppercase.
 
     Args:
         items (list[str] | str): The string or list of strings to be converted.
 
     Returns:
@@ -38,15 +41,15 @@
         >>> uppercase("hello")
         'HELLO'
 
         >>> uppercase(["hello", "world"])
         ['HELLO', 'WORLD']
     """
     if items is None:
-        return
+        return None
 
     if isinstance(items, list):
         return [item.strip().upper() for item in items]
     if isinstance(items, set):
         return {item.strip().upper() for item in items}
     else:
         return items.strip().upper()
@@ -119,15 +122,15 @@
         and not isinstance(attr.property, _RelationshipProperty)
     ]
     return item in base_model_fields
 
 
 def get_mapper_enum(
     model: _Type[_T],
-    schema: _BaseModel,
+    schema: _Type[_BaseModel],
 ) -> _Tuple[_Dict[str, _Optional[str]], _Enum]:
     """
     Get the mapper alias dictionary and enum for the given model and schema.
 
     Args:
         model: The model object.
         schema: The schema object.
```

### Comparing `alphaz-next-0.6.6/alphaz_next/utils/logger.py` & `alphaz-next-0.7.0/alphaz_next/utils/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             stream_output=stream_output,
             telemetry_handler=telemetry_handler,
         )
 
     def info(
         self,
         message: str,
-        exc_info: Exception = None,
+        exc_info: _Optional[Exception] = None,
         stack_level: int = 1,
         monitor: _Optional[str] = None,
     ) -> None:
         """
         Logs an informational message.
 
         Args:
@@ -103,15 +103,15 @@
                 "monitor": monitor,
             },
         )
 
     def warning(
         self,
         message: str,
-        exc_info: Exception = None,
+        exc_info: _Optional[Exception] = None,
         stack_level: int = 1,
         monitor: _Optional[str] = None,
     ) -> None:
         """
         Log a warning message.
 
         Args:
@@ -131,15 +131,15 @@
                 "monitor": monitor,
             },
         )
 
     def error(
         self,
         message: str,
-        exc_info: Exception = None,
+        exc_info: _Optional[Exception] = None,
         stack_level: int = 1,
         monitor: _Optional[str] = None,
     ) -> None:
         """
         Log an error message.
 
         Args:
@@ -156,15 +156,15 @@
                 "monitor": monitor,
             },
         )
 
     def critical(
         self,
         message: str,
-        exc_info: Exception = None,
+        exc_info: _Optional[Exception] = None,
         stack_level: int = 1,
         monitor: _Optional[str] = None,
     ) -> None:
         """
         Log a critical message.
 
         Args:
```

### Comparing `alphaz-next-0.6.6/alphaz_next/utils/logging_filters.py` & `alphaz-next-0.7.0/alphaz_next/utils/logging_filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         bool: True if the log record's level is in the allowed levels, False otherwise.
     """
 
     def __init__(self, levels: _List[int]) -> None:
         super().__init__()
         self._levels = levels
 
-    def filter(self, record):
+    def filter(self, record: _logging.LogRecord) -> bool:
         return record.levelno in self._levels
 
 
 class AttributeFilter(_logging.Filter):
     """
     A logging filter that filters log records based on the presence of a specified attribute.
 
@@ -34,42 +34,42 @@
         bool: True if the log record has the specified attribute, False otherwise.
     """
 
     def __init__(self, param: str) -> None:
         super().__init__()
         self.param_ = param
 
-    def filter(self, record):
+    def filter(self, record: _logging.LogRecord) -> bool:
         monitor = record.__dict__.get(self.param_, None)
         return monitor is not None
 
 
 class ExcludeRoutersFilter(_logging.Filter):
     """
     A logging filter that excludes log records based on the router names.
     """
 
     def __init__(
         self,
         router_names: _List[str],
         pattern: str = r'"([A-Z]+) ([^"]+)"',
-    ):
+    ) -> None:
         """
         Initialize the LoggingFilter object.
 
         Args:
             router_names (List[str]): A list of router names.
             pattern (str): A regular expression pattern used for filtering log messages.
                 Defaults to r'"([A-Z]+) ([^"]+)"'.
         """
         super().__init__()
         self.router_names = router_names
         self._pattern = pattern
 
-    def filter(self, record):
+    def filter(self, record: _logging.LogRecord) -> bool:
         """
         Filters the log record based on the configured pattern and router names.
 
         Args:
             record (LogRecord): The log record to be filtered.
 
         Returns:
```

### Comparing `alphaz-next-0.6.6/alphaz_next/utils/loguru.py` & `alphaz-next-0.7.0/alphaz_next/utils/loguru.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # MODULES
 import sys as _sys
-from typing import Dict, Optional as _Optional
-from loguru import logger as _logger
+from typing import Dict, Optional as _Optional, cast as _cast
+from loguru import logger as _logger, Logger as _Logger, _defaults
+
+# OPENTELEMETRY
 from opentelemetry import trace as _trace
 
 _LOGGERS: Dict[str, "Logger"] = {}
 
 
 class Logger:
 
     def __init__(
         self,
         name: str,
         level: str = "INFO",
         enqueue: bool = False,
         stream_output: bool = False,
-        colorize=True,
+        colorize: bool = True,
         format: _Optional[str] = None,
-    ):
+    ) -> None:
         self._is_new = True
         if name in _LOGGERS:
             saved_logger = _LOGGERS[name]
             self._logger = saved_logger.sub_logger
             self._name = saved_logger.name
             self._level = saved_logger.level
             self._is_new = False
@@ -31,16 +33,16 @@
         self._level = level
 
         self._logger = _logger.bind(service=name)
 
         if stream_output:
             self._logger.add(
                 _sys.stderr,
-                format=format,
                 level=level,
+                format=format or _cast(str, _defaults.LOGURU_FORMAT),
                 colorize=colorize,
                 filter=lambda record: record["extra"].get("service") == name,
                 enqueue=enqueue,
             )
 
         _LOGGERS[name] = self
 
@@ -53,47 +55,47 @@
         return self._level
 
     @property
     def is_new(self) -> bool:
         return self._is_new
 
     @property
-    def sub_logger(self):
+    def sub_logger(self) -> _Logger:
         return self._logger
 
-    def _log(self, level: str, message: str):
+    def _log(self, level: str, message: str) -> None:
         span = _trace.get_current_span()
         otelSpanID = _trace.format_span_id(span.get_span_context().span_id)
         otelTraceID = _trace.format_trace_id(span.get_span_context().trace_id)
 
         with self._logger.contextualize(
             otelTraceID=otelTraceID,
             otelSpanID=otelSpanID,
         ):
             getattr(self._logger.opt(depth=2), level)(message)
 
-    def info(self, message: str):
+    def info(self, message: str) -> None:
         self._log("info", message)
 
-    def error(self, message: str):
+    def error(self, message: str) -> None:
         self._log("error", message)
 
-    def warning(self, message: str):
+    def warning(self, message: str) -> None:
         self._log("warning", message)
 
-    def debug(self, message: str):
+    def debug(self, message: str) -> None:
         self._log("debug", message)
 
-    def trace(self, message: str):
+    def trace(self, message: str) -> None:
         self._log("trace", message)
 
-    def success(self, message: str):
+    def success(self, message: str) -> None:
         self._log("success", message)
 
-    def critical(self, message: str):
+    def critical(self, message: str) -> None:
         self._log("critical", message)
 
-    def exception(self, message: str):
+    def exception(self, message: str) -> None:
         self._log("exception", message)
 
-    def catch(self, message: str):
+    def catch(self, message: str) -> None:
         self._log("catch", message)
```

### Comparing `alphaz-next-0.6.6/alphaz_next.egg-info/PKG-INFO` & `alphaz-next-0.7.0/alphaz_next.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.6.6
-Summary: A project to make a lib to start FASTAPI quickly
+Version: 0.7.0
+Summary: A project to make a lib to start FastAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.6.6.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.0.tar.gz
 Author: Maxime MARTIN
-Author-email: maxime.martin02@hotmail.fr
+Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dependency-injector
 
 ## Alphaz-Next
 Alphaz-Next is a Python library designed to simplify the setup of REST APIs using FastAPI & Pydantic. It provides a useful toolkit for setting up Logger, Config, and more.
 
 ## Installing
```

### Comparing `alphaz-next-0.6.6/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.7.0/alphaz_next.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 README.md
+pyproject.toml
 setup.py
 alphaz_next/__init__.py
 alphaz_next.egg-info/PKG-INFO
 alphaz_next.egg-info/SOURCES.txt
 alphaz_next.egg-info/dependency_links.txt
 alphaz_next.egg-info/requires.txt
 alphaz_next.egg-info/top_level.txt
 alphaz_next/asyncio/__init__.py
+alphaz_next/asyncio/async_database.py
+alphaz_next/auth/__init__.py
 alphaz_next/auth/auth.py
 alphaz_next/core/__init__.py
 alphaz_next/core/_base.py
 alphaz_next/core/_middleware.py
 alphaz_next/core/_telemetry.py
 alphaz_next/core/application.py
 alphaz_next/core/constants.py
@@ -22,27 +25,31 @@
 alphaz_next/core/responses/json_response.py
 alphaz_next/core/responses/orjson_response.py
 alphaz_next/core/responses/plaintext_response.py
 alphaz_next/core/responses/redirect_response.py
 alphaz_next/core/responses/response.py
 alphaz_next/core/responses/streaming_response.py
 alphaz_next/core/responses/ujson_response.py
+alphaz_next/libs/__init__.py
 alphaz_next/libs/file_lib.py
 alphaz_next/libs/httpx.py
+alphaz_next/models/__init__.py
+alphaz_next/models/auth/__init__.py
 alphaz_next/models/auth/user.py
+alphaz_next/models/config/__init__.py
 alphaz_next/models/config/alpha_config.py
 alphaz_next/models/config/api_config.py
 alphaz_next/models/config/apm_config.py
 alphaz_next/models/config/config_settings.py
 alphaz_next/models/config/database_config.py
 alphaz_next/models/config/directories_config.py
 alphaz_next/models/config/logging_config.py
 alphaz_next/models/config/openapi_config_schema.py
+alphaz_next/models/config/_base/__init__.py
 alphaz_next/models/config/_base/internal_config_settings.py
 alphaz_next/models/config/_base/utils.py
-alphaz_next/tests/utils/utils.py
-alphaz_next/tests/utils/mocking/mock_user.py
+alphaz_next/utils/__init__.py
 alphaz_next/utils/database.py
 alphaz_next/utils/format.py
 alphaz_next/utils/logger.py
 alphaz_next/utils/logging_filters.py
 alphaz_next/utils/loguru.py
```

