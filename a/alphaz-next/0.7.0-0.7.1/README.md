# Comparing `tmp/alphaz-next-0.7.0.tar.gz` & `tmp/alphaz-next-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.7.0.tar", last modified: Wed May 22 13:28:27 2024, max compression
+gzip compressed data, was "alphaz-next-0.7.1.tar", last modified: Wed May 22 13:40:20 2024, max compression
```

## Comparing `alphaz-next-0.7.0.tar` & `alphaz-next-0.7.1.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.458244 alphaz-next-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-22 13:28:27.458244 alphaz-next-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.450245 alphaz-next-0.7.0/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/asyncio/async_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/core/responses/ujson_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.454244 alphaz-next-0.7.0/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.458244 alphaz-next-0.7.0/alphaz_next/models/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.458244 alphaz-next-0.7.0/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/directories_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/models/config/openapi_config_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.458244 alphaz-next-0.7.0/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/utils/logging_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/alphaz_next/utils/loguru.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:28:27.450245 alphaz-next-0.7.0/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-22 13:28:27.000000 alphaz-next-0.7.0/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-22 13:28:27.000000 alphaz-next-0.7.0/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:28:27.000000 alphaz-next-0.7.0/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 13:28:27.000000 alphaz-next-0.7.0/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 13:28:27.000000 alphaz-next-0.7.0/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-22 13:28:21.000000 alphaz-next-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:28:27.458244 alphaz-next-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-22 13:28:25.000000 alphaz-next-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:20.161730 alphaz-next-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-22 13:40:20.161730 alphaz-next-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:20.153730 alphaz-next-0.7.1/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:20.153730 alphaz-next-0.7.1/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/asyncio/async_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:20.157730 alphaz-next-0.7.1/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:20.157730 alphaz-next-0.7.1/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:20.157730 alphaz-next-0.7.1/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/core/responses/ujson_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:20.157730 alphaz-next-0.7.1/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:20.157730 alphaz-next-0.7.1/alphaz_next/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:20.157730 alphaz-next-0.7.1/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:20.161730 alphaz-next-0.7.1/alphaz_next/models/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:20.161730 alphaz-next-0.7.1/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/config/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/config/directories_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/models/config/openapi_config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:20.161730 alphaz-next-0.7.1/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/utils/logging_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/alphaz_next/utils/loguru.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:40:20.153730 alphaz-next-0.7.1/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-22 13:40:20.000000 alphaz-next-0.7.1/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-22 13:40:20.000000 alphaz-next-0.7.1/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:40:20.000000 alphaz-next-0.7.1/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 13:40:20.000000 alphaz-next-0.7.1/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 13:40:20.000000 alphaz-next-0.7.1/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-22 13:40:16.000000 alphaz-next-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:40:20.161730 alphaz-next-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-22 13:40:18.000000 alphaz-next-0.7.1/setup.py
```

### Comparing `alphaz-next-0.7.0/PKG-INFO` & `alphaz-next-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.7.0
+Version: 0.7.1
 Summary: A project to make a lib to start FastAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.0.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.1.tar.gz
 Author: Maxime MARTIN
 Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.7.0/README.md` & `alphaz-next-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/asyncio/async_database.py` & `alphaz-next-0.7.1/alphaz_next/asyncio/async_database.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/auth/auth.py` & `alphaz-next-0.7.1/alphaz_next/auth/auth.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/_base.py` & `alphaz-next-0.7.1/alphaz_next/core/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/_middleware.py` & `alphaz-next-0.7.1/alphaz_next/core/_middleware.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/_telemetry.py` & `alphaz-next-0.7.1/alphaz_next/core/_telemetry.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/application.py` & `alphaz-next-0.7.1/alphaz_next/core/application.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.7.1/alphaz_next/core/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/exceptions.py` & `alphaz-next-0.7.1/alphaz_next/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/responses/__init__.py` & `alphaz-next-0.7.1/alphaz_next/core/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.7.1/alphaz_next/core/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.7.1/alphaz_next/core/responses/html_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.7.1/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.7.1/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.7.1/alphaz_next/core/responses/plaintext_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.7.1/alphaz_next/core/responses/redirect_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/responses/response.py` & `alphaz-next-0.7.1/alphaz_next/core/responses/response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.7.1/alphaz_next/core/responses/streaming_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.7.1/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/libs/httpx.py` & `alphaz-next-0.7.1/alphaz_next/libs/httpx.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.7.1/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.7.1/alphaz_next/models/config/_base/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.7.1/alphaz_next/models/config/alpha_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/models/config/api_config.py` & `alphaz-next-0.7.1/alphaz_next/models/config/api_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.7.1/alphaz_next/models/config/apm_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.7.1/alphaz_next/models/config/config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/models/config/database_config.py` & `alphaz-next-0.7.1/alphaz_next/models/config/database_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.7.1/alphaz_next/models/config/logging_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.7.1/alphaz_next/models/config/openapi_config_schema.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/utils/database.py` & `alphaz-next-0.7.1/alphaz_next/utils/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/utils/format.py` & `alphaz-next-0.7.1/alphaz_next/utils/format.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/utils/logger.py` & `alphaz-next-0.7.1/alphaz_next/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/utils/logging_filters.py` & `alphaz-next-0.7.1/alphaz_next/utils/logging_filters.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next/utils/loguru.py` & `alphaz-next-0.7.1/alphaz_next/utils/loguru.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.0/alphaz_next.egg-info/PKG-INFO` & `alphaz-next-0.7.1/alphaz_next.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.7.0
+Version: 0.7.1
 Summary: A project to make a lib to start FastAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.0.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.1.tar.gz
 Author: Maxime MARTIN
 Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.7.0/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.7.1/alphaz_next.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 pyproject.toml
 setup.py
 alphaz_next/__init__.py
+alphaz_next/py.typed
 alphaz_next.egg-info/PKG-INFO
 alphaz_next.egg-info/SOURCES.txt
 alphaz_next.egg-info/dependency_links.txt
 alphaz_next.egg-info/requires.txt
 alphaz_next.egg-info/top_level.txt
 alphaz_next/asyncio/__init__.py
 alphaz_next/asyncio/async_database.py
```

