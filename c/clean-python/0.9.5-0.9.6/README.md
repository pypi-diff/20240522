# Comparing `tmp/clean-python-0.9.5.tar.gz` & `tmp/clean-python-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean-python-0.9.5.tar", last modified: Mon Dec 18 13:01:44 2023, max compression
+gzip compressed data, was "clean-python-0.9.6.tar", last modified: Wed Dec 20 10:34:10 2023, max compression
```

## Comparing `clean-python-0.9.5.tar` & `clean-python-0.9.6.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.511981 clean-python-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)     6440 2023-12-18 13:01:36.000000 clean-python-0.9.5/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-12-18 13:01:36.000000 clean-python-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-18 13:01:36.000000 clean-python-0.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2023-12-18 13:01:44.511981 clean-python-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2023-12-18 13:01:36.000000 clean-python-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.491981 clean-python-0.9.5/clean_python/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.495981 clean-python-0.9.5/clean_python/amqp/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/amqp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/amqp/celery_rmq_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.495981 clean-python-0.9.5/clean_python/api_client/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/api_client/api_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/api_client/api_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/api_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/api_client/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/api_client/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/api_client/sync_api_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.495981 clean-python-0.9.5/clean_python/base/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.495981 clean-python-0.9.5/clean_python/base/application/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/application/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.499981 clean-python-0.9.5/clean_python/base/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/domain/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/domain/domain_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/domain/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/domain/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/domain/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/domain/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/domain/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/domain/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/domain/root_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/domain/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/domain/value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/domain/value_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.499981 clean-python-0.9.5/clean_python/base/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/infrastructure/in_memory_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/infrastructure/internal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/infrastructure/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/infrastructure/tmpdir_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/infrastructure/typed_internal_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.499981 clean-python-0.9.5/clean_python/base/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/presentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/base/presentation/link.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.499981 clean-python-0.9.5/clean_python/celery/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/celery/base_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/celery/celery_task_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/celery/kubernetes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.499981 clean-python-0.9.5/clean_python/dramatiq/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/dramatiq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/dramatiq/async_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/dramatiq/dramatiq_task_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/dramatiq/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.503981 clean-python-0.9.5/clean_python/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/fastapi/error_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/fastapi/fastapi_access_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/fastapi/request_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/fastapi/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/fastapi/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/fastapi/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.503981 clean-python-0.9.5/clean_python/fluentbit/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/fluentbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/fluentbit/fluentbit_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.503981 clean-python-0.9.5/clean_python/oauth2/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/oauth2/client_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/oauth2/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/oauth2/token_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.503981 clean-python-0.9.5/clean_python/s3/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/s3/key_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/s3/s3_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/s3/s3_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.503981 clean-python-0.9.5/clean_python/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12098 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/sql/sql_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/sql/sql_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/sql/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.503981 clean-python-0.9.5/clean_python/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/testing/attr_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/testing/debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/testing/dramatiq_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-12-18 13:01:36.000000 clean-python-0.9.5/clean_python/testing/fastapi_profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.507981 clean-python-0.9.5/clean_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2023-12-18 13:01:44.000000 clean-python-0.9.5/clean_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2023-12-18 13:01:44.000000 clean-python-0.9.5/clean_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 13:01:44.000000 clean-python-0.9.5/clean_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 13:01:44.000000 clean-python-0.9.5/clean_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-12-18 13:01:44.000000 clean-python-0.9.5/clean_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-18 13:01:44.000000 clean-python-0.9.5/clean_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-12-18 13:01:36.000000 clean-python-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-12-18 13:01:44.511981 clean-python-0.9.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:01:44.507981 clean-python-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2023-12-18 13:01:36.000000 clean-python-0.9.5/tests/test_async_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-18 13:01:36.000000 clean-python-0.9.5/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2023-12-18 13:01:36.000000 clean-python-0.9.5/tests/test_dramatiq_task_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-12-18 13:01:36.000000 clean-python-0.9.5/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2023-12-18 13:01:36.000000 clean-python-0.9.5/tests/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2023-12-18 13:01:36.000000 clean-python-0.9.5/tests/test_internal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2023-12-18 13:01:36.000000 clean-python-0.9.5/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2023-12-18 13:01:36.000000 clean-python-0.9.5/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2023-12-18 13:01:36.000000 clean-python-0.9.5/tests/test_root_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2023-12-18 13:01:36.000000 clean-python-0.9.5/tests/test_sync_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2023-12-18 13:01:36.000000 clean-python-0.9.5/tests/test_sync_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2023-12-18 13:01:36.000000 clean-python-0.9.5/tests/test_typed_internal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-12-18 13:01:36.000000 clean-python-0.9.5/tests/test_value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.955536 clean-python-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2023-12-20 10:34:01.000000 clean-python-0.9.6/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-12-20 10:34:01.000000 clean-python-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-20 10:34:01.000000 clean-python-0.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2023-12-20 10:34:10.955536 clean-python-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2023-12-20 10:34:01.000000 clean-python-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.935536 clean-python-0.9.6/clean_python/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.939535 clean-python-0.9.6/clean_python/amqp/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/amqp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/amqp/celery_rmq_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.939535 clean-python-0.9.6/clean_python/api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/api_client/api_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/api_client/api_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/api_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/api_client/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/api_client/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/api_client/sync_api_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.939535 clean-python-0.9.6/clean_python/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.939535 clean-python-0.9.6/clean_python/base/application/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/application/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.943535 clean-python-0.9.6/clean_python/base/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/domain/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/domain/domain_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/domain/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/domain/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/domain/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/domain/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/domain/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/domain/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/domain/root_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/domain/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/domain/value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/domain/value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.943535 clean-python-0.9.6/clean_python/base/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/infrastructure/in_memory_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/infrastructure/internal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/infrastructure/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/infrastructure/tmpdir_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/infrastructure/typed_internal_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.943535 clean-python-0.9.6/clean_python/base/presentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/presentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/base/presentation/link.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.943535 clean-python-0.9.6/clean_python/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/celery/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/celery/celery_task_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/celery/kubernetes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.943535 clean-python-0.9.6/clean_python/dramatiq/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/dramatiq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/dramatiq/async_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/dramatiq/dramatiq_task_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/dramatiq/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.947536 clean-python-0.9.6/clean_python/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/fastapi/error_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/fastapi/fastapi_access_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/fastapi/request_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/fastapi/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/fastapi/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/fastapi/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.947536 clean-python-0.9.6/clean_python/fluentbit/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/fluentbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/fluentbit/fluentbit_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.947536 clean-python-0.9.6/clean_python/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/oauth2/client_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/oauth2/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/oauth2/token_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.947536 clean-python-0.9.6/clean_python/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/s3/key_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/s3/s3_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/s3/s3_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.947536 clean-python-0.9.6/clean_python/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12098 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/sql/sql_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/sql/sql_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/sql/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.947536 clean-python-0.9.6/clean_python/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/testing/attr_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/testing/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/testing/dramatiq_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-12-20 10:34:01.000000 clean-python-0.9.6/clean_python/testing/fastapi_profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.951536 clean-python-0.9.6/clean_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2023-12-20 10:34:10.000000 clean-python-0.9.6/clean_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2023-12-20 10:34:10.000000 clean-python-0.9.6/clean_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 10:34:10.000000 clean-python-0.9.6/clean_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 10:34:10.000000 clean-python-0.9.6/clean_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2023-12-20 10:34:10.000000 clean-python-0.9.6/clean_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-20 10:34:10.000000 clean-python-0.9.6/clean_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-12-20 10:34:01.000000 clean-python-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-12-20 10:34:10.955536 clean-python-0.9.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:34:10.951536 clean-python-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2023-12-20 10:34:01.000000 clean-python-0.9.6/tests/test_async_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-20 10:34:01.000000 clean-python-0.9.6/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2023-12-20 10:34:01.000000 clean-python-0.9.6/tests/test_dramatiq_task_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2023-12-20 10:34:01.000000 clean-python-0.9.6/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2023-12-20 10:34:01.000000 clean-python-0.9.6/tests/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2023-12-20 10:34:01.000000 clean-python-0.9.6/tests/test_internal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2023-12-20 10:34:01.000000 clean-python-0.9.6/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2023-12-20 10:34:01.000000 clean-python-0.9.6/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2023-12-20 10:34:01.000000 clean-python-0.9.6/tests/test_root_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2023-12-20 10:34:01.000000 clean-python-0.9.6/tests/test_sync_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2023-12-20 10:34:01.000000 clean-python-0.9.6/tests/test_sync_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2023-12-20 10:34:01.000000 clean-python-0.9.6/tests/test_typed_internal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-12-20 10:34:01.000000 clean-python-0.9.6/tests/test_value_object.py
```

### Comparing `clean-python-0.9.5/CHANGES.md` & `clean-python-0.9.6/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # Changelog of clean-python
 
 
+0.9.6 (2023-12-20)
+------------------
+
+- Fixed celery task_failure_log in case of a crashed worker.
+
+
 0.9.5 (2023-12-18)
 ------------------
 
 - SyncApiProvider: also retry when the Retry-After response header is missing.
 
 - ApiProvider: (sync and async) retry on all methods except POST.
```

### Comparing `clean-python-0.9.5/LICENSE` & `clean-python-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/PKG-INFO` & `clean-python-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-python
-Version: 0.9.5
+Version: 0.9.6
 Summary: Clean architecture in Python
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: homepage, https://github.com/nens/clean-python
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `clean-python-0.9.5/README.md` & `clean-python-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/amqp/celery_rmq_broker.py` & `clean-python-0.9.6/clean_python/amqp/celery_rmq_broker.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/api_client/api_gateway.py` & `clean-python-0.9.6/clean_python/api_client/api_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/api_client/api_provider.py` & `clean-python-0.9.6/clean_python/api_client/api_provider.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/api_client/files.py` & `clean-python-0.9.6/clean_python/api_client/files.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/api_client/sync_api_provider.py` & `clean-python-0.9.6/clean_python/api_client/sync_api_provider.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/base/application/manage.py` & `clean-python-0.9.6/clean_python/base/application/manage.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/base/domain/context.py` & `clean-python-0.9.6/clean_python/base/domain/context.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/base/domain/domain_event.py` & `clean-python-0.9.6/clean_python/base/domain/domain_event.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/base/domain/exceptions.py` & `clean-python-0.9.6/clean_python/base/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/base/domain/gateway.py` & `clean-python-0.9.6/clean_python/base/domain/gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/base/domain/pagination.py` & `clean-python-0.9.6/clean_python/base/domain/pagination.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/base/domain/repository.py` & `clean-python-0.9.6/clean_python/base/domain/repository.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/base/domain/root_entity.py` & `clean-python-0.9.6/clean_python/base/domain/root_entity.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/base/domain/value_object.py` & `clean-python-0.9.6/clean_python/base/domain/value_object.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/base/infrastructure/in_memory_gateway.py` & `clean-python-0.9.6/clean_python/base/infrastructure/in_memory_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/base/infrastructure/internal_gateway.py` & `clean-python-0.9.6/clean_python/base/infrastructure/internal_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/base/infrastructure/typed_internal_gateway.py` & `clean-python-0.9.6/clean_python/base/infrastructure/typed_internal_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/celery/base_task.py` & `clean-python-0.9.6/clean_python/celery/base_task.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/celery/celery_task_logger.py` & `clean-python-0.9.6/clean_python/celery/celery_task_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         try:
             request = task.request
         except AttributeError:
             request = None
 
         try:
             headers, kwargs = TaskHeaders.from_kwargs(request.kwargs)
-        except AttributeError:
+        except (AttributeError, TypeError):
             headers = kwargs = None  # type: ignore
 
         try:
             tenant_id = headers.tenant.id  # type: ignore
         except AttributeError:
             tenant_id = None
```

### Comparing `clean-python-0.9.5/clean_python/celery/kubernetes.py` & `clean-python-0.9.6/clean_python/celery/kubernetes.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/dramatiq/async_actor.py` & `clean-python-0.9.6/clean_python/dramatiq/async_actor.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/dramatiq/dramatiq_task_logger.py` & `clean-python-0.9.6/clean_python/dramatiq/dramatiq_task_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/dramatiq/testing.py` & `clean-python-0.9.6/clean_python/dramatiq/testing.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/fastapi/error_responses.py` & `clean-python-0.9.6/clean_python/fastapi/error_responses.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/fastapi/fastapi_access_logger.py` & `clean-python-0.9.6/clean_python/fastapi/fastapi_access_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/fastapi/request_query.py` & `clean-python-0.9.6/clean_python/fastapi/request_query.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/fastapi/resource.py` & `clean-python-0.9.6/clean_python/fastapi/resource.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/fastapi/security.py` & `clean-python-0.9.6/clean_python/fastapi/security.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/fastapi/service.py` & `clean-python-0.9.6/clean_python/fastapi/service.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/fluentbit/fluentbit_gateway.py` & `clean-python-0.9.6/clean_python/fluentbit/fluentbit_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/oauth2/client_credentials.py` & `clean-python-0.9.6/clean_python/oauth2/client_credentials.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/oauth2/token.py` & `clean-python-0.9.6/clean_python/oauth2/token.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/oauth2/token_verifier.py` & `clean-python-0.9.6/clean_python/oauth2/token_verifier.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/s3/key_mapper.py` & `clean-python-0.9.6/clean_python/s3/key_mapper.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/s3/s3_gateway.py` & `clean-python-0.9.6/clean_python/s3/s3_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/s3/s3_provider.py` & `clean-python-0.9.6/clean_python/s3/s3_provider.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/sql/sql_gateway.py` & `clean-python-0.9.6/clean_python/sql/sql_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/sql/sql_provider.py` & `clean-python-0.9.6/clean_python/sql/sql_provider.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/sql/testing.py` & `clean-python-0.9.6/clean_python/sql/testing.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/testing/dramatiq_profiler.py` & `clean-python-0.9.6/clean_python/testing/dramatiq_profiler.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python/testing/fastapi_profiler.py` & `clean-python-0.9.6/clean_python/testing/fastapi_profiler.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/clean_python.egg-info/PKG-INFO` & `clean-python-0.9.6/clean_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-python
-Version: 0.9.5
+Version: 0.9.6
 Summary: Clean architecture in Python
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: homepage, https://github.com/nens/clean-python
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `clean-python-0.9.5/clean_python.egg-info/SOURCES.txt` & `clean-python-0.9.6/clean_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/pyproject.toml` & `clean-python-0.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/tests/test_async_actor.py` & `clean-python-0.9.6/tests/test_async_actor.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/tests/test_context.py` & `clean-python-0.9.6/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/tests/test_dramatiq_task_logger.py` & `clean-python-0.9.6/tests/test_dramatiq_task_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/tests/test_exceptions.py` & `clean-python-0.9.6/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/tests/test_gateway.py` & `clean-python-0.9.6/tests/test_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/tests/test_internal_gateway.py` & `clean-python-0.9.6/tests/test_internal_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/tests/test_manage.py` & `clean-python-0.9.6/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/tests/test_repository.py` & `clean-python-0.9.6/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/tests/test_root_entity.py` & `clean-python-0.9.6/tests/test_root_entity.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/tests/test_sync_gateway.py` & `clean-python-0.9.6/tests/test_sync_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/tests/test_sync_repository.py` & `clean-python-0.9.6/tests/test_sync_repository.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/tests/test_typed_internal_gateway.py` & `clean-python-0.9.6/tests/test_typed_internal_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.9.5/tests/test_value_object.py` & `clean-python-0.9.6/tests/test_value_object.py`

 * *Files identical despite different names*

