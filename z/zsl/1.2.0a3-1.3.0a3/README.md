# Comparing `tmp/zsl-1.2.0a3.tar.gz` & `tmp/zsl-1.3.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zsl-1.2.0a3.tar", last modified: Wed Mar 13 17:40:33 2024, max compression
+gzip compressed data, was "zsl-1.3.0a3.tar", last modified: Wed May 22 19:09:06 2024, max compression
```

## Comparing `zsl-1.2.0a3.tar` & `zsl-1.3.0a3.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.494232 zsl-1.2.0a3/
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-03-13 17:39:03.000000 zsl-1.2.0a3/.bumpversion.cfg
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-02-02 13:20:01.000000 zsl-1.2.0a3/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-02-02 13:20:01.000000 zsl-1.2.0a3/.editorconfig
--rw-rw-rw-   0 root         (0) root         (0)      585 2024-02-06 15:02:49.000000 zsl-1.2.0a3/.readthedocs.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-02-02 13:20:01.000000 zsl-1.2.0a3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      477 2024-02-06 15:02:49.000000 zsl-1.2.0a3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5302 2024-03-13 17:40:33.494232 zsl-1.2.0a3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4459 2024-02-06 15:02:49.000000 zsl-1.2.0a3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.474232 zsl-1.2.0a3/docs/
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-02-02 13:20:01.000000 zsl-1.2.0a3/docs/caching.rst
--rw-rw-rw-   0 root         (0) root         (0)     7485 2024-03-13 17:39:03.000000 zsl-1.2.0a3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     4261 2024-02-02 13:20:01.000000 zsl-1.2.0a3/docs/configuration.rst
--rw-rw-rw-   0 root         (0) root         (0)     2021 2024-02-06 15:02:49.000000 zsl-1.2.0a3/docs/database.rst
--rw-rw-rw-   0 root         (0) root         (0)      642 2024-02-02 13:20:01.000000 zsl-1.2.0a3/docs/developing.rst
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-02-02 13:20:01.000000 zsl-1.2.0a3/docs/error_handling.rst
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-02-02 13:20:01.000000 zsl-1.2.0a3/docs/extending.rst
--rw-rw-rw-   0 root         (0) root         (0)     1932 2024-02-06 15:02:49.000000 zsl-1.2.0a3/docs/getting_started.rst
--rw-rw-rw-   0 root         (0) root         (0)     1454 2024-03-13 17:39:03.000000 zsl-1.2.0a3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-02-02 13:20:01.000000 zsl-1.2.0a3/docs/modules_and_containers.rst
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-02-06 15:02:49.000000 zsl-1.2.0a3/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-02-02 13:20:01.000000 zsl-1.2.0a3/docs/spelling_wordlist.txt
--rw-rw-rw-   0 root         (0) root         (0)     4350 2024-02-02 13:20:01.000000 zsl-1.2.0a3/docs/unit_testing.rst
--rw-rw-rw-   0 root         (0) root         (0)     4873 2024-02-06 15:02:49.000000 zsl-1.2.0a3/docs/workers.rst
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-03-13 17:40:33.494232 zsl-1.2.0a3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1566 2024-03-13 17:39:03.000000 zsl-1.2.0a3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.466232 zsl-1.2.0a3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.474232 zsl-1.2.0a3/src/zsl/
--rw-rw-rw-   0 root         (0) root         (0)      878 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.474232 zsl-1.2.0a3/src/zsl/application/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/application/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.474232 zsl-1.2.0a3/src/zsl/application/containers/
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/application/containers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      738 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/containers/celery_container.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/containers/container.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/containers/core_container.py
--rw-rw-rw-   0 root         (0) root         (0)      362 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/containers/gearman_container.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/containers/web_container.py
--rw-rw-rw-   0 root         (0) root         (0)     4811 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/initialization_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.474232 zsl-1.2.0a3/src/zsl/application/initializers/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/application/initializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/initializers/library_initializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2114 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/initializers/service_initializer.py
--rw-rw-rw-   0 root         (0) root         (0)      781 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/initializers/unittest_initializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.474232 zsl-1.2.0a3/src/zsl/application/modules/
--rw-rw-rw-   0 root         (0) root         (0)       94 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/application/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3603 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/modules/alchemy_module.py
--rw-rw-rw-   0 root         (0) root         (0)     1603 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/modules/cache_module.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/modules/celery_module.py
--rw-rw-rw-   0 root         (0) root         (0)     4205 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/modules/cli_module.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/modules/context_module.py
--rw-rw-rw-   0 root         (0) root         (0)      849 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/modules/error_handler_module.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/modules/gearman_module.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/modules/logger_module.py
--rw-rw-rw-   0 root         (0) root         (0)      947 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/modules/task_router.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.478232 zsl-1.2.0a3/src/zsl/application/modules/web/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/application/modules/web/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/modules/web/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/modules/web/cors.py
--rw-rw-rw-   0 root         (0) root         (0)     3347 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/modules/web/web_context_module.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/application/service_application.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.478232 zsl-1.2.0a3/src/zsl/cache/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/cache/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1435 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/cache/cache_module.py
--rw-rw-rw-   0 root         (0) root         (0)     3672 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/cache/id_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     2630 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/cache/redis_cache_module.py
--rw-rw-rw-   0 root         (0) root         (0)     2991 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/cache/redis_id_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.478232 zsl-1.2.0a3/src/zsl/configuration/
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.478232 zsl-1.2.0a3/src/zsl/contrib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/contrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.478232 zsl-1.2.0a3/src/zsl/contrib/alembic/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/contrib/alembic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/contrib/alembic/alembic_config.py
--rw-rw-rw-   0 root         (0) root         (0)     5246 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/contrib/alembic/alembic_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.478232 zsl-1.2.0a3/src/zsl/contrib/sentry/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/contrib/sentry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/contrib/sentry/sentry_config.py
--rw-rw-rw-   0 root         (0) root         (0)     4144 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/contrib/sentry/sentry_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.478232 zsl-1.2.0a3/src/zsl/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.478232 zsl-1.2.0a3/src/zsl/db/helpers/
--rw-rw-rw-   0 root         (0) root         (0)      956 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/db/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/db/helpers/nested.py
--rw-rw-rw-   0 root         (0) root         (0)     4182 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/db/helpers/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     3697 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/db/helpers/query_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/db/helpers/query_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     3518 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/db/helpers/sorter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.478232 zsl-1.2.0a3/src/zsl/db/model/
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/db/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2555 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/db/model/app_model.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/db/model/app_model_json_decoder.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/db/model/app_model_json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/db/model/raw_model.py
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/db/model/sql_alchemy.py
--rw-rw-rw-   0 root         (0) root         (0)     2640 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/errors.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/gearman.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.478232 zsl-1.2.0a3/src/zsl/interface/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.478232 zsl-1.2.0a3/src/zsl/interface/celery/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/interface/celery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3099 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/celery/worker.py
--rw-rw-rw-   0 root         (0) root         (0)     1328 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.478232 zsl-1.2.0a3/src/zsl/interface/gearman/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/interface/gearman/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      519 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/gearman/json_data_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/gearman/task_filler.py
--rw-rw-rw-   0 root         (0) root         (0)     2009 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/gearman/worker.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     4500 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/task.py
--rw-rw-rw-   0 root         (0) root         (0)     3675 2024-03-13 17:32:20.000000 zsl-1.2.0a3/src/zsl/interface/task_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.478232 zsl-1.2.0a3/src/zsl/interface/web/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/interface/web/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/web/importer.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/interface/web/index.cgi
--rw-rw-rw-   0 root         (0) root         (0)      874 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/interface/web/index.wsgi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.482232 zsl-1.2.0a3/src/zsl/interface/web/performers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/interface/web/performers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/web/performers/default.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/web/performers/method.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/web/performers/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/web/performers/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.482232 zsl-1.2.0a3/src/zsl/interface/web/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/interface/web/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/web/utils/execution.py
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/web/utils/request_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1685 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/interface/web/utils/response_headers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.482232 zsl-1.2.0a3/src/zsl/resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/resource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13348 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/resource/guard.py
--rw-rw-rw-   0 root         (0) root         (0)     8329 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/resource/json_server_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    19415 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/resource/model_resource.py
--rw-rw-rw-   0 root         (0) root         (0)     6756 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/resource/resource_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.482232 zsl-1.2.0a3/src/zsl/router/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/router/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2816 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/router/method.py
--rw-rw-rw-   0 root         (0) root         (0)     7739 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/router/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.482232 zsl-1.2.0a3/src/zsl/service/
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3818 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/service/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.482232 zsl-1.2.0a3/src/zsl/task/
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/task/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4668 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/task/job_context.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/task/task_data.py
--rw-rw-rw-   0 root         (0) root         (0)    14882 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/task/task_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/task/task_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.482232 zsl-1.2.0a3/src/zsl/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.482232 zsl-1.2.0a3/src/zsl/tasks/zsl/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/tasks/zsl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/tasks/zsl/cors_test_task.py
--rw-rw-rw-   0 root         (0) root         (0)      831 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/tasks/zsl/db_test_task.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/tasks/zsl/kill_worker_task.py
--rw-rw-rw-   0 root         (0) root         (0)      593 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/tasks/zsl/schedule_celery_task.py
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/tasks/zsl/schedule_gearman_task.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/tasks/zsl/schedule_kill_worker_task.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/tasks/zsl/sum_task.py
--rw-rw-rw-   0 root         (0) root         (0)      301 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/tasks/zsl/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/tasks/zsl/version_task.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/tasks/zsl/with_request_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.486232 zsl-1.2.0a3/src/zsl/testing/
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/testing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6206 2024-02-21 08:27:36.000000 zsl-1.2.0a3/src/zsl/testing/db.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/testing/http.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/testing/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2190 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/testing/zsl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.486232 zsl-1.2.0a3/src/zsl/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2660 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/background_task.py
--rw-rw-rw-   0 root         (0) root         (0)     5779 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/cache_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     2015 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/command_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1114 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/date_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.490232 zsl-1.2.0a3/src/zsl/utils/deploy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/src/zsl/utils/deploy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3783 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/deploy/apiari_doc_generator.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/deploy/integrator.py
--rw-rw-rw-   0 root         (0) root         (0)     6867 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/deploy/js_model_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     5030 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/dict_to_object_conversion.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/documentation.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/email_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/file_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/gearman_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/http.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/import_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     2452 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/injection_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1525 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/model_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1608 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/nginx_push_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1574 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/params_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/php_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1306 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/redis_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/reflection_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/request_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     5009 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/resource_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     2827 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/rss.py
--rw-rw-rw-   0 root         (0) root         (0)     2364 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/security_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     4746 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/string_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/task_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/testing.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/type_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/url_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/warnings.py
--rw-rw-rw-   0 root         (0) root         (0)     4305 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/xml_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     5520 2024-02-06 15:02:49.000000 zsl-1.2.0a3/src/zsl/utils/xml_to_json.py
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-03-13 17:39:03.000000 zsl-1.2.0a3/src/zsl/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.474232 zsl-1.2.0a3/src/zsl.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5302 2024-03-13 17:40:33.000000 zsl-1.2.0a3/src/zsl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7551 2024-03-13 17:40:33.000000 zsl-1.2.0a3/src/zsl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 17:40:33.000000 zsl-1.2.0a3/src/zsl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      319 2024-03-13 17:40:33.000000 zsl-1.2.0a3/src/zsl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-03-13 17:40:33.000000 zsl-1.2.0a3/src/zsl.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.490232 zsl-1.2.0a3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.490232 zsl-1.2.0a3/tests/application/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2284 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/application/error_handling_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1569 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/application/version_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.490232 zsl-1.2.0a3/tests/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.490232 zsl-1.2.0a3/tests/db/helpers/
--rw-rw-rw-   0 root         (0) root         (0)     2890 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/db/helpers/pagination_parsing_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.490232 zsl-1.2.0a3/tests/db/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/db/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1201 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/db/model/app_model_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.490232 zsl-1.2.0a3/tests/interface/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.490232 zsl-1.2.0a3/tests/interface/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/interface/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/interface/cli/exec_task_from_cli_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/interface/create_simple_model_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/interface/exec_task_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.490232 zsl-1.2.0a3/tests/interface/web/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/interface/web/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2607 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/interface/web/cors_test.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/interface/web/task_configuration_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2123 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/interface/web/task_router_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.490232 zsl-1.2.0a3/tests/interface/worker/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/interface/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/interface/worker/run_dummy_worker_with_params_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1370 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/interface/worker/run_dummy_worker_without_params_test.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/mocks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.490232 zsl-1.2.0a3/tests/resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/resource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4466 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/resource/guarded_resource_test.py
--rw-rw-rw-   0 root         (0) root         (0)    14873 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/resource/json_server_model_resource_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3152 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/resource/model_resource_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1470 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/resource/read_only_resource.py
--rw-rw-rw-   0 root         (0) root         (0)     9532 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/resource/resource_guard_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2140 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/resource/resource_helper_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5637 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/resource/resource_policy_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2817 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/resource/resource_test_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     3772 2024-02-12 16:12:39.000000 zsl-1.2.0a3/tests/resource/transactional_guard_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.490232 zsl-1.2.0a3/tests/service/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3209 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/service/service__tx_session_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.494232 zsl-1.2.0a3/tests/task_decorators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/task_decorators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1424 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/task_decorators/forbid_web_access_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2187 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/task_decorators/secured_task_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.494232 zsl-1.2.0a3/tests/testing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/testing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4193 2024-02-02 14:24:56.000000 zsl-1.2.0a3/tests/testing/db_test.py
--rw-rw-rw-   0 root         (0) root         (0)     7740 2024-02-20 17:25:55.000000 zsl-1.2.0a3/tests/testing/db_test_case__schema_initialization_and_querying__test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:40:33.494232 zsl-1.2.0a3/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/utils/background_task_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2024-02-06 15:02:49.000000 zsl-1.2.0a3/tests/utils/command_dispatcher_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2174 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/utils/redis_helper_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1625 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/utils/request_helper_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/utils/string_helper_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tests/utils/xml_to_json_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2215 2024-02-02 13:20:01.000000 zsl-1.2.0a3/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.346885 zsl-1.3.0a3/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-05-22 19:07:39.000000 zsl-1.3.0a3/.bumpversion.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-01-31 10:44:04.000000 zsl-1.3.0a3/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-01-31 10:44:04.000000 zsl-1.3.0a3/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      585 2024-02-06 15:02:49.000000 zsl-1.3.0a3/.readthedocs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-01-31 10:44:04.000000 zsl-1.3.0a3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      477 2024-02-06 15:02:49.000000 zsl-1.3.0a3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5302 2024-05-22 19:09:06.350885 zsl-1.3.0a3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4459 2024-02-06 15:02:49.000000 zsl-1.3.0a3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.322885 zsl-1.3.0a3/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-01-31 10:44:04.000000 zsl-1.3.0a3/docs/caching.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7485 2024-05-22 19:07:39.000000 zsl-1.3.0a3/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2024-01-31 10:44:04.000000 zsl-1.3.0a3/docs/configuration.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2021 2024-02-06 15:02:49.000000 zsl-1.3.0a3/docs/database.rst
+-rw-rw-rw-   0 root         (0) root         (0)      642 2024-01-31 10:44:04.000000 zsl-1.3.0a3/docs/developing.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-01-31 10:44:04.000000 zsl-1.3.0a3/docs/error_handling.rst
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-01-31 10:44:04.000000 zsl-1.3.0a3/docs/extending.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1932 2024-02-06 15:02:49.000000 zsl-1.3.0a3/docs/getting_started.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2024-03-13 17:38:59.000000 zsl-1.3.0a3/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-01-31 10:44:04.000000 zsl-1.3.0a3/docs/modules_and_containers.rst
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-02-06 15:02:49.000000 zsl-1.3.0a3/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-01-31 10:44:04.000000 zsl-1.3.0a3/docs/spelling_wordlist.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4350 2024-01-31 10:44:04.000000 zsl-1.3.0a3/docs/unit_testing.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4873 2024-02-06 15:02:49.000000 zsl-1.3.0a3/docs/workers.rst
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-22 19:09:06.350885 zsl-1.3.0a3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2024-05-22 19:07:39.000000 zsl-1.3.0a3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.314885 zsl-1.3.0a3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.322885 zsl-1.3.0a3/src/zsl/
+-rw-rw-rw-   0 root         (0) root         (0)      878 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.326885 zsl-1.3.0a3/src/zsl/application/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/application/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.326885 zsl-1.3.0a3/src/zsl/application/containers/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/application/containers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      738 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/containers/celery_container.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/containers/container.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/containers/core_container.py
+-rw-rw-rw-   0 root         (0) root         (0)      362 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/containers/gearman_container.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/containers/web_container.py
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)      850 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/initialization_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.326885 zsl-1.3.0a3/src/zsl/application/initializers/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/application/initializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/initializers/library_initializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/initializers/service_initializer.py
+-rw-rw-rw-   0 root         (0) root         (0)      781 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/initializers/unittest_initializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.326885 zsl-1.3.0a3/src/zsl/application/modules/
+-rw-rw-rw-   0 root         (0) root         (0)       94 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/application/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3603 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/modules/alchemy_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/modules/cache_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/modules/celery_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     4205 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/modules/cli_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/modules/context_module.py
+-rw-rw-rw-   0 root         (0) root         (0)      849 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/modules/error_handler_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/modules/gearman_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/modules/logger_module.py
+-rw-rw-rw-   0 root         (0) root         (0)      947 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/modules/task_router.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.326885 zsl-1.3.0a3/src/zsl/application/modules/web/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/application/modules/web/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/modules/web/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/modules/web/cors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3347 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/application/modules/web/web_context_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     7348 2024-05-22 11:18:52.000000 zsl-1.3.0a3/src/zsl/application/service_application.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.326885 zsl-1.3.0a3/src/zsl/cache/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/cache/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1435 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/cache/cache_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     3672 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/cache/id_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2630 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/cache/redis_cache_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/cache/redis_id_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.326885 zsl-1.3.0a3/src/zsl/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.326885 zsl-1.3.0a3/src/zsl/contrib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/contrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.330885 zsl-1.3.0a3/src/zsl/contrib/alembic/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/contrib/alembic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/contrib/alembic/alembic_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     5246 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/contrib/alembic/alembic_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.330885 zsl-1.3.0a3/src/zsl/contrib/sentry/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/contrib/sentry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/contrib/sentry/sentry_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4144 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/contrib/sentry/sentry_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.330885 zsl-1.3.0a3/src/zsl/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.330885 zsl-1.3.0a3/src/zsl/db/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)      956 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/db/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/db/helpers/nested.py
+-rw-rw-rw-   0 root         (0) root         (0)     4182 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/db/helpers/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     3697 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/db/helpers/query_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/db/helpers/query_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3518 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/db/helpers/sorter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.330885 zsl-1.3.0a3/src/zsl/db/model/
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/db/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2555 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/db/model/app_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/db/model/app_model_json_decoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/db/model/app_model_json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/db/model/raw_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/db/model/sql_alchemy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/gearman.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.330885 zsl-1.3.0a3/src/zsl/interface/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.330885 zsl-1.3.0a3/src/zsl/interface/celery/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/interface/celery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3099 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/celery/worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.330885 zsl-1.3.0a3/src/zsl/interface/gearman/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/interface/gearman/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      519 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/gearman/json_data_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/gearman/task_filler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2009 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/gearman/worker.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     4500 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     3675 2024-03-13 17:27:01.000000 zsl-1.3.0a3/src/zsl/interface/task_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.334885 zsl-1.3.0a3/src/zsl/interface/web/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/interface/web/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/web/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/interface/web/index.cgi
+-rw-rw-rw-   0 root         (0) root         (0)      874 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/interface/web/index.wsgi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.334885 zsl-1.3.0a3/src/zsl/interface/web/performers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/interface/web/performers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/web/performers/default.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/web/performers/method.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/web/performers/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/web/performers/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.334885 zsl-1.3.0a3/src/zsl/interface/web/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/interface/web/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/web/utils/execution.py
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/web/utils/request_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/interface/web/utils/response_headers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.334885 zsl-1.3.0a3/src/zsl/resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13348 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/resource/guard.py
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/resource/json_server_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    19415 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/resource/model_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     6756 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/resource/resource_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.334885 zsl-1.3.0a3/src/zsl/router/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/router/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2816 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/router/method.py
+-rw-rw-rw-   0 root         (0) root         (0)     7739 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/router/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.334885 zsl-1.3.0a3/src/zsl/service/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3818 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/service/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.334885 zsl-1.3.0a3/src/zsl/task/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/task/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4668 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/task/job_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/task/task_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    14882 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/task/task_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/task/task_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.334885 zsl-1.3.0a3/src/zsl/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.338885 zsl-1.3.0a3/src/zsl/tasks/zsl/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/tasks/zsl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/tasks/zsl/cors_test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      831 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/tasks/zsl/db_test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/tasks/zsl/kill_worker_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      593 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/tasks/zsl/schedule_celery_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/tasks/zsl/schedule_gearman_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/tasks/zsl/schedule_kill_worker_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/tasks/zsl/sum_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/tasks/zsl/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/tasks/zsl/version_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/tasks/zsl/with_request_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.338885 zsl-1.3.0a3/src/zsl/testing/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/testing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6206 2024-02-21 08:27:39.000000 zsl-1.3.0a3/src/zsl/testing/db.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/testing/http.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/testing/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/testing/zsl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.342885 zsl-1.3.0a3/src/zsl/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2660 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/background_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     5779 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/cache_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2015 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/command_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/date_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.342885 zsl-1.3.0a3/src/zsl/utils/deploy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/src/zsl/utils/deploy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3783 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/deploy/apiari_doc_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/deploy/integrator.py
+-rw-rw-rw-   0 root         (0) root         (0)     6867 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/deploy/js_model_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5030 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/dict_to_object_conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/documentation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/email_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/file_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/gearman_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/http.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/import_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/injection_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1525 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/model_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1608 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/nginx_push_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/params_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      397 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/php_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/redis_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/reflection_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/request_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     5009 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/resource_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2827 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/rss.py
+-rw-rw-rw-   0 root         (0) root         (0)     2364 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/security_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4746 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/string_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/task_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/testing.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/type_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/url_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/warnings.py
+-rw-rw-rw-   0 root         (0) root         (0)     4305 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/xml_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     5520 2024-02-06 15:02:49.000000 zsl-1.3.0a3/src/zsl/utils/xml_to_json.py
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-22 19:07:39.000000 zsl-1.3.0a3/src/zsl/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.322885 zsl-1.3.0a3/src/zsl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5302 2024-05-22 19:09:06.000000 zsl-1.3.0a3/src/zsl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7551 2024-05-22 19:09:06.000000 zsl-1.3.0a3/src/zsl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 19:09:06.000000 zsl-1.3.0a3/src/zsl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      319 2024-05-22 19:09:06.000000 zsl-1.3.0a3/src/zsl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-05-22 19:09:06.000000 zsl-1.3.0a3/src/zsl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.342885 zsl-1.3.0a3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.342885 zsl-1.3.0a3/tests/application/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/application/error_handling_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/application/version_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.342885 zsl-1.3.0a3/tests/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.342885 zsl-1.3.0a3/tests/db/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)     2890 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/db/helpers/pagination_parsing_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.342885 zsl-1.3.0a3/tests/db/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/db/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/db/model/app_model_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.342885 zsl-1.3.0a3/tests/interface/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.342885 zsl-1.3.0a3/tests/interface/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/interface/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/interface/cli/exec_task_from_cli_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/interface/create_simple_model_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/interface/exec_task_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.346885 zsl-1.3.0a3/tests/interface/web/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/interface/web/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2607 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/interface/web/cors_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/interface/web/task_configuration_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2123 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/interface/web/task_router_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.346885 zsl-1.3.0a3/tests/interface/worker/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/interface/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/interface/worker/run_dummy_worker_with_params_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/interface/worker/run_dummy_worker_without_params_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/mocks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.346885 zsl-1.3.0a3/tests/resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4466 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/resource/guarded_resource_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    14873 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/resource/json_server_model_resource_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3152 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/resource/model_resource_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1470 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/resource/read_only_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     9532 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/resource/resource_guard_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2140 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/resource/resource_helper_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5637 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/resource/resource_policy_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/resource/resource_test_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3772 2024-02-12 16:12:38.000000 zsl-1.3.0a3/tests/resource/transactional_guard_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.346885 zsl-1.3.0a3/tests/service/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3209 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/service/service__tx_session_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.346885 zsl-1.3.0a3/tests/task_decorators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/task_decorators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/task_decorators/forbid_web_access_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/task_decorators/secured_task_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.346885 zsl-1.3.0a3/tests/testing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/testing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4193 2024-02-02 14:25:29.000000 zsl-1.3.0a3/tests/testing/db_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     7740 2024-02-21 08:27:39.000000 zsl-1.3.0a3/tests/testing/db_test_case__schema_initialization_and_querying__test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:09:06.346885 zsl-1.3.0a3/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/utils/background_task_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2024-02-06 15:02:49.000000 zsl-1.3.0a3/tests/utils/command_dispatcher_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2174 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/utils/redis_helper_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/utils/request_helper_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/utils/string_helper_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tests/utils/xml_to_json_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2215 2024-01-31 10:44:04.000000 zsl-1.3.0a3/tox.ini
```

### Comparing `zsl-1.2.0a3/.readthedocs.yaml` & `zsl-1.3.0a3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/LICENSE` & `zsl-1.3.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/PKG-INFO` & `zsl-1.3.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zsl
-Version: 1.2.0a3
+Version: 1.3.0a3
 Summary: zsl application framework for web based services
 Home-page: https://github.com/AtteqCom/zsl
 Author: Atteq s.r.o.
 Author-email: open.source@atteq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `zsl-1.2.0a3/README.md` & `zsl-1.3.0a3/README.md`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/docs/conf.py` & `zsl-1.3.0a3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,17 +61,17 @@
 author = "Atteq s.r.o."
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "1.2.0a3"
+version = "1.3.0a3"
 # The full version, including alpha/beta/rc tags.
-release = "1.2.0 alpha 3"
+release = "1.3.0 alpha 3"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
```

### Comparing `zsl-1.2.0a3/docs/configuration.rst` & `zsl-1.3.0a3/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/docs/database.rst` & `zsl-1.3.0a3/docs/database.rst`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/docs/developing.rst` & `zsl-1.3.0a3/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/docs/error_handling.rst` & `zsl-1.3.0a3/docs/error_handling.rst`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/docs/getting_started.rst` & `zsl-1.3.0a3/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/docs/index.rst` & `zsl-1.3.0a3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/docs/modules_and_containers.rst` & `zsl-1.3.0a3/docs/modules_and_containers.rst`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/docs/unit_testing.rst` & `zsl-1.3.0a3/docs/unit_testing.rst`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/docs/workers.rst` & `zsl-1.3.0a3/docs/workers.rst`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/setup.py` & `zsl-1.3.0a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'typing>=3.7'
 ]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='zsl',
-      version='1.2.0a3',
+      version='1.3.0a3',
       description='zsl application framework for web based services',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Atteq s.r.o.',
       author_email='open.source@atteq.com',
       url='https://github.com/AtteqCom/zsl',
       license='MIT',
```

### Comparing `zsl-1.2.0a3/src/zsl/__init__.py` & `zsl-1.3.0a3/src/zsl/__init__.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/containers/celery_container.py` & `zsl-1.3.0a3/src/zsl/application/containers/celery_container.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/containers/container.py` & `zsl-1.3.0a3/src/zsl/application/containers/container.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/containers/core_container.py` & `zsl-1.3.0a3/src/zsl/application/containers/core_container.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/error_handler.py` & `zsl-1.3.0a3/src/zsl/application/error_handler.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/initialization_context.py` & `zsl-1.3.0a3/src/zsl/application/initialization_context.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/initializers/library_initializer.py` & `zsl-1.3.0a3/src/zsl/application/initializers/library_initializer.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/initializers/service_initializer.py` & `zsl-1.3.0a3/src/zsl/application/initializers/service_initializer.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/initializers/unittest_initializer.py` & `zsl-1.3.0a3/src/zsl/application/initializers/unittest_initializer.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/modules/alchemy_module.py` & `zsl-1.3.0a3/src/zsl/application/modules/alchemy_module.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/modules/cache_module.py` & `zsl-1.3.0a3/src/zsl/application/modules/cache_module.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/modules/celery_module.py` & `zsl-1.3.0a3/src/zsl/application/modules/celery_module.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/modules/cli_module.py` & `zsl-1.3.0a3/src/zsl/application/modules/cli_module.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/modules/context_module.py` & `zsl-1.3.0a3/src/zsl/application/modules/context_module.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/modules/error_handler_module.py` & `zsl-1.3.0a3/src/zsl/application/modules/error_handler_module.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/modules/gearman_module.py` & `zsl-1.3.0a3/src/zsl/application/modules/gearman_module.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/modules/logger_module.py` & `zsl-1.3.0a3/src/zsl/application/modules/logger_module.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/modules/task_router.py` & `zsl-1.3.0a3/src/zsl/application/modules/task_router.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/modules/web/configuration.py` & `zsl-1.3.0a3/src/zsl/application/modules/web/configuration.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/modules/web/cors.py` & `zsl-1.3.0a3/src/zsl/application/modules/web/cors.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/modules/web/web_context_module.py` & `zsl-1.3.0a3/src/zsl/application/modules/web/web_context_module.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/application/service_application.py` & `zsl-1.3.0a3/src/zsl/application/service_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,46 +15,48 @@
 
 .. data:: SETTINGS_ENV_VAR_NAME
 
     Name of the environment variable to be read for the profile configuration
     file.
 
 """
+
 import os
 from typing import Any, Callable
 
 from flask import Config, Flask
 from injector import Binder, Injector, singleton
 
 from zsl._state import set_current_app
 from zsl.application.initialization_context import InitializationContext
 from zsl.utils.warnings import deprecated
 from zsl.version import version
 
 # Name of the environment variable to be read for the profile configuration.
-SETTINGS_ENV_VAR_NAME = 'ZSL_SETTINGS'
+SETTINGS_ENV_VAR_NAME = "ZSL_SETTINGS"
 
 
 def get_settings_from_profile(profile, profile_dir=None):
     # type: (str, Any)->str
-    """"Returns the  configuration file path for the given profile.
+    """ "Returns the  configuration file path for the given profile.
 
     :param profile: Profile name to be used.
     :param profile_dir: The directory where the profile configuration file should reside. It
                         may be also a module, and then the directory of the module is used.
     :return: Configuration file path.
     """
     if profile_dir is None:
         import settings
+
         profile_dir = settings
 
-    if hasattr(profile_dir, '__file__'):
+    if hasattr(profile_dir, "__file__"):
         profile_dir = os.path.dirname(profile_dir.__file__)
 
-    return os.path.join(profile_dir, '{0}.cfg'.format(profile))
+    return os.path.join(profile_dir, "{0}.cfg".format(profile))
 
 
 def set_profile(profile):
     # type (str)->None
     """Sets the current profile.
 
     :param profile: The profile to be used."""
@@ -77,46 +79,47 @@
         template_folder="templates",
         instance_path=None,
         instance_relative_config=False,
         root_path=None,
         modules=None,
         version=None,
         config_object=None,
-        default_settings_module='settings.default_settings'
+        default_settings_module="settings.default_settings",
     ):
         super().__init__(
             import_name,
             static_url_path,
             static_folder,
             static_host,
             host_matching,
             subdomain_matching,
             template_folder,
             instance_path,
             instance_relative_config,
-            root_path
+            root_path,
         )
         self._dependencies_initialized = False
         self._default_settings_module = default_settings_module
         self._is_initialized = False
         self._injector = None
         self._worker = None
         self._configure(config_object)
         self._app_version = version
         if not modules:
             from zsl.application.containers.core_container import CoreContainer
+
             modules = CoreContainer.modules()
         self._configure_injector(modules)
         self._initialize()
         self._dependencies_initialized = True
 
     def __str__(self):
         return "ZSL(application={0}, zsl_version={1}, app_version={2})".format(
-            self.name, self.VERSION,
-            self._app_version)
+            self.name, self.VERSION, self._app_version
+        )
 
     def _configure(self, config_object=None):
         # type: (Any) -> None
         """Read the configuration from config files.
         Loads the default settings and the profile settings if available.
         Check :func:`.set_profile`.
 
@@ -129,15 +132,20 @@
         if config_object:
             self.config.from_mapping(config_object)
         else:
             self.config.from_object(self._default_settings_module)
 
         zsl_settings = os.environ.get(SETTINGS_ENV_VAR_NAME)
         if zsl_settings is not None:
-            self.config.from_envvar(SETTINGS_ENV_VAR_NAME)
+            if os.path.exists(zsl_settings):
+                self.config.from_envvar(SETTINGS_ENV_VAR_NAME)
+            else:
+                self.logger.warning(
+                    f"Warning: The settings file '{zsl_settings}' does not exist. Using default settings."
+                )
 
     def _initialize(self):
         """Run the initializers."""
         ctx = self.injector.get(InitializationContext)
         ctx.initialize()
 
     def _register(self):
@@ -209,15 +217,15 @@
         return ServiceApplication.VERSION
 
     @property
     def app_version(self):
         return self._app_version
 
     def _create_injector(self):
-        self.logger.debug('Creating injector')
+        self.logger.debug("Creating injector")
         self._injector = Injector()
 
     def _bind_core(self):
         self._injector.binder.bind(ServiceApplication, self, singleton)
         self._injector.binder.bind(Config, self.config, singleton)
 
     def _bind_modules(self, modules):
```

### Comparing `zsl-1.2.0a3/src/zsl/cache/cache_module.py` & `zsl-1.3.0a3/src/zsl/cache/cache_module.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/cache/id_helper.py` & `zsl-1.3.0a3/src/zsl/cache/id_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/cache/redis_cache_module.py` & `zsl-1.3.0a3/src/zsl/cache/redis_cache_module.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/cache/redis_id_helper.py` & `zsl-1.3.0a3/src/zsl/cache/redis_id_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/contrib/alembic/alembic_module.py` & `zsl-1.3.0a3/src/zsl/contrib/alembic/alembic_module.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/contrib/sentry/sentry_config.py` & `zsl-1.3.0a3/src/zsl/contrib/sentry/sentry_config.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/contrib/sentry/sentry_module.py` & `zsl-1.3.0a3/src/zsl/contrib/sentry/sentry_module.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/db/helpers/__init__.py` & `zsl-1.3.0a3/src/zsl/db/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/db/helpers/nested.py` & `zsl-1.3.0a3/src/zsl/db/helpers/nested.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/db/helpers/pagination.py` & `zsl-1.3.0a3/src/zsl/db/helpers/pagination.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/db/helpers/query_filter.py` & `zsl-1.3.0a3/src/zsl/db/helpers/query_filter.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/db/helpers/query_helper.py` & `zsl-1.3.0a3/src/zsl/db/helpers/query_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/db/helpers/sorter.py` & `zsl-1.3.0a3/src/zsl/db/helpers/sorter.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/db/model/app_model.py` & `zsl-1.3.0a3/src/zsl/db/model/app_model.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/db/model/app_model_json_decoder.py` & `zsl-1.3.0a3/src/zsl/db/model/app_model_json_decoder.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/db/model/raw_model.py` & `zsl-1.3.0a3/src/zsl/db/model/raw_model.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/errors.py` & `zsl-1.3.0a3/src/zsl/errors.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/celery/worker.py` & `zsl-1.3.0a3/src/zsl/interface/celery/worker.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/cli.py` & `zsl-1.3.0a3/src/zsl/interface/cli.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/gearman/json_data_encoder.py` & `zsl-1.3.0a3/src/zsl/interface/gearman/json_data_encoder.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/gearman/task_filler.py` & `zsl-1.3.0a3/src/zsl/interface/gearman/task_filler.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/gearman/worker.py` & `zsl-1.3.0a3/src/zsl/interface/gearman/worker.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/task.py` & `zsl-1.3.0a3/src/zsl/interface/task.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/task_queue.py` & `zsl-1.3.0a3/src/zsl/interface/task_queue.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/web/index.wsgi` & `zsl-1.3.0a3/src/zsl/interface/web/index.wsgi`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/web/performers/default.py` & `zsl-1.3.0a3/src/zsl/interface/web/performers/default.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/web/performers/method.py` & `zsl-1.3.0a3/src/zsl/interface/web/performers/method.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/web/performers/resource.py` & `zsl-1.3.0a3/src/zsl/interface/web/performers/resource.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/web/performers/task.py` & `zsl-1.3.0a3/src/zsl/interface/web/performers/task.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/web/utils/execution.py` & `zsl-1.3.0a3/src/zsl/interface/web/utils/execution.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/interface/web/utils/response_headers.py` & `zsl-1.3.0a3/src/zsl/interface/web/utils/response_headers.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/resource/guard.py` & `zsl-1.3.0a3/src/zsl/resource/guard.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/resource/json_server_resource.py` & `zsl-1.3.0a3/src/zsl/resource/json_server_resource.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/resource/model_resource.py` & `zsl-1.3.0a3/src/zsl/resource/model_resource.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/resource/resource_helper.py` & `zsl-1.3.0a3/src/zsl/resource/resource_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/router/method.py` & `zsl-1.3.0a3/src/zsl/router/method.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/router/task.py` & `zsl-1.3.0a3/src/zsl/router/task.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/service/service.py` & `zsl-1.3.0a3/src/zsl/service/service.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/task/job_context.py` & `zsl-1.3.0a3/src/zsl/task/job_context.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/task/task_data.py` & `zsl-1.3.0a3/src/zsl/task/task_data.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/task/task_decorator.py` & `zsl-1.3.0a3/src/zsl/task/task_decorator.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/tasks/zsl/db_test_task.py` & `zsl-1.3.0a3/src/zsl/tasks/zsl/db_test_task.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/tasks/zsl/kill_worker_task.py` & `zsl-1.3.0a3/src/zsl/tasks/zsl/kill_worker_task.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/tasks/zsl/schedule_celery_task.py` & `zsl-1.3.0a3/src/zsl/tasks/zsl/schedule_celery_task.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/tasks/zsl/sum_task.py` & `zsl-1.3.0a3/src/zsl/tasks/zsl/sum_task.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/tasks/zsl/version_task.py` & `zsl-1.3.0a3/src/zsl/tasks/zsl/version_task.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/tasks/zsl/with_request_task.py` & `zsl-1.3.0a3/src/zsl/tasks/zsl/with_request_task.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/testing/db.py` & `zsl-1.3.0a3/src/zsl/testing/db.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/testing/http.py` & `zsl-1.3.0a3/src/zsl/testing/http.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/testing/test_utils.py` & `zsl-1.3.0a3/src/zsl/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/testing/zsl.py` & `zsl-1.3.0a3/src/zsl/testing/zsl.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/background_task.py` & `zsl-1.3.0a3/src/zsl/utils/background_task.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/cache_helper.py` & `zsl-1.3.0a3/src/zsl/utils/cache_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/command_dispatcher.py` & `zsl-1.3.0a3/src/zsl/utils/command_dispatcher.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/date_helper.py` & `zsl-1.3.0a3/src/zsl/utils/date_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/deploy/apiari_doc_generator.py` & `zsl-1.3.0a3/src/zsl/utils/deploy/apiari_doc_generator.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/deploy/integrator.py` & `zsl-1.3.0a3/src/zsl/utils/deploy/integrator.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/deploy/js_model_generator.py` & `zsl-1.3.0a3/src/zsl/utils/deploy/js_model_generator.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/dict_to_object_conversion.py` & `zsl-1.3.0a3/src/zsl/utils/dict_to_object_conversion.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/documentation.py` & `zsl-1.3.0a3/src/zsl/utils/documentation.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/email_helper.py` & `zsl-1.3.0a3/src/zsl/utils/email_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/gearman_helper.py` & `zsl-1.3.0a3/src/zsl/utils/gearman_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/injection_helper.py` & `zsl-1.3.0a3/src/zsl/utils/injection_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/model_helper.py` & `zsl-1.3.0a3/src/zsl/utils/model_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/nginx_push_helper.py` & `zsl-1.3.0a3/src/zsl/utils/nginx_push_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/params_helper.py` & `zsl-1.3.0a3/src/zsl/utils/params_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/redis_helper.py` & `zsl-1.3.0a3/src/zsl/utils/redis_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/reflection_helper.py` & `zsl-1.3.0a3/src/zsl/utils/reflection_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/request_helper.py` & `zsl-1.3.0a3/src/zsl/utils/request_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/resource_helper.py` & `zsl-1.3.0a3/src/zsl/utils/resource_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/rss.py` & `zsl-1.3.0a3/src/zsl/utils/rss.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/security_helper.py` & `zsl-1.3.0a3/src/zsl/utils/security_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/string_helper.py` & `zsl-1.3.0a3/src/zsl/utils/string_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/task_helper.py` & `zsl-1.3.0a3/src/zsl/utils/task_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/testing.py` & `zsl-1.3.0a3/src/zsl/utils/testing.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/url_helper.py` & `zsl-1.3.0a3/src/zsl/utils/url_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/warnings.py` & `zsl-1.3.0a3/src/zsl/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/xml_helper.py` & `zsl-1.3.0a3/src/zsl/utils/xml_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl/utils/xml_to_json.py` & `zsl-1.3.0a3/src/zsl/utils/xml_to_json.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/src/zsl.egg-info/PKG-INFO` & `zsl-1.3.0a3/src/zsl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zsl
-Version: 1.2.0a3
+Version: 1.3.0a3
 Summary: zsl application framework for web based services
 Home-page: https://github.com/AtteqCom/zsl
 Author: Atteq s.r.o.
 Author-email: open.source@atteq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `zsl-1.2.0a3/src/zsl.egg-info/SOURCES.txt` & `zsl-1.3.0a3/src/zsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/application/error_handling_test.py` & `zsl-1.3.0a3/tests/application/error_handling_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/application/version_test.py` & `zsl-1.3.0a3/tests/application/version_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/db/helpers/pagination_parsing_test.py` & `zsl-1.3.0a3/tests/db/helpers/pagination_parsing_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/db/model/app_model_test.py` & `zsl-1.3.0a3/tests/db/model/app_model_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/interface/cli/exec_task_from_cli_test.py` & `zsl-1.3.0a3/tests/interface/cli/exec_task_from_cli_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/interface/create_simple_model_test.py` & `zsl-1.3.0a3/tests/interface/create_simple_model_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/interface/exec_task_test.py` & `zsl-1.3.0a3/tests/interface/exec_task_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/interface/web/cors_test.py` & `zsl-1.3.0a3/tests/interface/web/cors_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/interface/web/task_configuration_test.py` & `zsl-1.3.0a3/tests/interface/web/task_configuration_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/interface/web/task_router_test.py` & `zsl-1.3.0a3/tests/interface/web/task_router_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/interface/worker/run_dummy_worker_with_params_test.py` & `zsl-1.3.0a3/tests/interface/worker/run_dummy_worker_with_params_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/interface/worker/run_dummy_worker_without_params_test.py` & `zsl-1.3.0a3/tests/interface/worker/run_dummy_worker_without_params_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/mocks.py` & `zsl-1.3.0a3/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/resource/guarded_resource_test.py` & `zsl-1.3.0a3/tests/resource/guarded_resource_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/resource/json_server_model_resource_test.py` & `zsl-1.3.0a3/tests/resource/json_server_model_resource_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/resource/model_resource_test.py` & `zsl-1.3.0a3/tests/resource/model_resource_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/resource/read_only_resource.py` & `zsl-1.3.0a3/tests/resource/read_only_resource.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/resource/resource_guard_test.py` & `zsl-1.3.0a3/tests/resource/resource_guard_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/resource/resource_helper_test.py` & `zsl-1.3.0a3/tests/resource/resource_helper_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/resource/resource_policy_test.py` & `zsl-1.3.0a3/tests/resource/resource_policy_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/resource/resource_test_helper.py` & `zsl-1.3.0a3/tests/resource/resource_test_helper.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/resource/transactional_guard_test.py` & `zsl-1.3.0a3/tests/resource/transactional_guard_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/service/service__tx_session_test.py` & `zsl-1.3.0a3/tests/service/service__tx_session_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/task_decorators/forbid_web_access_test.py` & `zsl-1.3.0a3/tests/task_decorators/forbid_web_access_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/task_decorators/secured_task_test.py` & `zsl-1.3.0a3/tests/task_decorators/secured_task_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/testing/db_test.py` & `zsl-1.3.0a3/tests/testing/db_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/testing/db_test_case__schema_initialization_and_querying__test.py` & `zsl-1.3.0a3/tests/testing/db_test_case__schema_initialization_and_querying__test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/utils/command_dispatcher_test.py` & `zsl-1.3.0a3/tests/utils/command_dispatcher_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/utils/redis_helper_test.py` & `zsl-1.3.0a3/tests/utils/redis_helper_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/utils/request_helper_test.py` & `zsl-1.3.0a3/tests/utils/request_helper_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/utils/string_helper_test.py` & `zsl-1.3.0a3/tests/utils/string_helper_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tests/utils/xml_to_json_test.py` & `zsl-1.3.0a3/tests/utils/xml_to_json_test.py`

 * *Files identical despite different names*

### Comparing `zsl-1.2.0a3/tox.ini` & `zsl-1.3.0a3/tox.ini`

 * *Files identical despite different names*

