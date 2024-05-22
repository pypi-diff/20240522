# Comparing `tmp/cornflow-1.1.0a1.tar.gz` & `tmp/cornflow-1.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornflow-1.1.0a1.tar", last modified: Wed May 15 17:22:07 2024, max compression
+gzip compressed data, was "cornflow-1.1.0a2.tar", last modified: Wed May 22 10:53:28 2024, max compression
```

## Comparing `cornflow-1.1.0a1.tar` & `cornflow-1.1.0a2.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.271705 cornflow-1.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-15 17:22:07.271705 cornflow-1.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.247704 cornflow-1.1.0a1/airflow_config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/airflow_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/airflow_config/airflow_local_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.247704 cornflow-1.1.0a1/airflow_config/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.247704 cornflow-1.1.0a1/airflow_config/plugins/XCom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/airflow_config/plugins/XCom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/airflow_config/plugins/XCom/gce_xcom_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/airflow_config/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/airflow_config/webserver_ldap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.247704 cornflow-1.1.0a1/cornflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.251704 cornflow-1.1.0a1/cornflow/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.251704 cornflow-1.1.0a1/cornflow/cli/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16344 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/api_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12640 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/endpoint_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/models_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/schema_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/schemas_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/tools/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/users.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/cli/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.251704 cornflow-1.1.0a1/cornflow/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/commands/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.255704 cornflow-1.1.0a1/cornflow/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/apiview.py
--rw-r--r--   0 runner    (1001) docker     (127)    18670 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/case.py
--rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/data_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    27998 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    11615 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/meta_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/signup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/endpoints/user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/gunicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.255704 cornflow-1.1.0a1/cornflow/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/README
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.255704 cornflow-1.1.0a1/cornflow/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/00757b557b02_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/1af47a419bbd_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/4aac5e0c6e66_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/7c3ea5ab5501_.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/991b98e24225_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/a472b5ad50b7_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/c2db9409cb5f_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/c8a6c762e818_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/ca449af8034c_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/d0e0700dcd8e_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/d1b5be1f0549_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/e1a50dae1ac9_.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/e937a5234ce4_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/ebdd955fcc5e_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/migrations/versions/f3bee20314a2_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.259704 cornflow-1.1.0a1/cornflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/base_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/dag_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/meta_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/models/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.263704 cornflow-1.1.0a1/cornflow/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/case.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/model_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/role.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/solution_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/schemas/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.263704 cornflow-1.1.0a1/cornflow/shared/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.263704 cornflow-1.1.0a1/cornflow/shared/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18664 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/authentication/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/authentication/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/authentication/ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/query_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/utils_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/shared/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.263704 cornflow-1.1.0a1/cornflow/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/custom_liveServer.py
--rw-r--r--   0 runner    (1001) docker     (127)    25147 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/custom_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.263704 cornflow-1.1.0a1/cornflow/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/integration/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    20963 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/integration/test_cornflowclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.267705 cornflow-1.1.0a1/cornflow/tests/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/ldap/test_ldap_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.267705 cornflow-1.1.0a1/cornflow/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_apiview.py
--rw-r--r--   0 runner    (1001) docker     (127)    25974 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_dags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_data_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17501 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_executions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15376 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_generate_from_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_health.py
--rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_instances_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_log_in.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16581 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_schema_from_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_sign_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    22430 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/cornflow/tests/unit/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:22:07.247704 cornflow-1.1.0a1/cornflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-15 17:22:06.000000 cornflow-1.1.0a1/cornflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-15 17:22:07.000000 cornflow-1.1.0a1/cornflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:22:06.000000 cornflow-1.1.0a1/cornflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 17:22:06.000000 cornflow-1.1.0a1/cornflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-15 17:22:06.000000 cornflow-1.1.0a1/cornflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 17:22:06.000000 cornflow-1.1.0a1/cornflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 17:22:07.271705 cornflow-1.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-15 17:22:04.000000 cornflow-1.1.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.828822 cornflow-1.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-22 10:53:28.828822 cornflow-1.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.804822 cornflow-1.1.0a2/airflow_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/airflow_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/airflow_config/airflow_local_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.804822 cornflow-1.1.0a2/airflow_config/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.804822 cornflow-1.1.0a2/airflow_config/plugins/XCom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/airflow_config/plugins/XCom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/airflow_config/plugins/XCom/gce_xcom_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/airflow_config/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/airflow_config/webserver_ldap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.808822 cornflow-1.1.0a2/cornflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.808822 cornflow-1.1.0a2/cornflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.808822 cornflow-1.1.0a2/cornflow/cli/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16344 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/tools/api_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12640 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/tools/endpoint_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/tools/models_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/tools/schema_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/tools/schemas_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/tools/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/cli/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.812821 cornflow-1.1.0a2/cornflow/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/commands/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/commands/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/commands/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/commands/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/commands/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/commands/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/commands/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/commands/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.816822 cornflow-1.1.0a2/cornflow/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/apiview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18670 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/data_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27998 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11615 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/meta_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/signup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/endpoints/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/gunicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.816822 cornflow-1.1.0a2/cornflow/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/README
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.816822 cornflow-1.1.0a2/cornflow/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/00757b557b02_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/1af47a419bbd_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/4aac5e0c6e66_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/7c3ea5ab5501_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/991b98e24225_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/a472b5ad50b7_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/c2db9409cb5f_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/c8a6c762e818_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/ca449af8034c_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/d0e0700dcd8e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/d1b5be1f0549_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/e1a50dae1ac9_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/e937a5234ce4_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/ebdd955fcc5e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/migrations/versions/f3bee20314a2_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.820822 cornflow-1.1.0a2/cornflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/base_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/dag_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/meta_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/models/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.824822 cornflow-1.1.0a2/cornflow/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/model_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/solution_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/schemas/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.824822 cornflow-1.1.0a2/cornflow/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.824822 cornflow-1.1.0a2/cornflow/shared/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18664 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/authentication/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/authentication/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/authentication/ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/query_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/utils_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/shared/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.824822 cornflow-1.1.0a2/cornflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/custom_liveServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25147 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/custom_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.824822 cornflow-1.1.0a2/cornflow/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/integration/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20963 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/integration/test_cornflowclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.824822 cornflow-1.1.0a2/cornflow/tests/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/ldap/test_ldap_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.828822 cornflow-1.1.0a2/cornflow/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_apiview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25974 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_dags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_data_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17501 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_executions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15376 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_generate_from_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_instances_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_log_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16581 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_schema_from_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22430 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/cornflow/tests/unit/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:53:28.808822 cornflow-1.1.0a2/cornflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-22 10:53:28.000000 cornflow-1.1.0a2/cornflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-22 10:53:28.000000 cornflow-1.1.0a2/cornflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:53:28.000000 cornflow-1.1.0a2/cornflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 10:53:28.000000 cornflow-1.1.0a2/cornflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-22 10:53:28.000000 cornflow-1.1.0a2/cornflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 10:53:28.000000 cornflow-1.1.0a2/cornflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:53:28.828822 cornflow-1.1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-22 10:53:26.000000 cornflow-1.1.0a2/setup.py
```

### Comparing `cornflow-1.1.0a1/PKG-INFO` & `cornflow-1.1.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cornflow
-Version: 1.1.0a1
+Version: 1.1.0a2
 Summary: Cornflow is an open source multi-solver optimization server with a REST API built using flask.
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: cornflow@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow
         =========
```

### Comparing `cornflow-1.1.0a1/README.rst` & `cornflow-1.1.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/airflow_config/airflow_local_settings.py` & `cornflow-1.1.0a2/airflow_config/airflow_local_settings.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/airflow_config/plugins/XCom/gce_xcom_backend.py` & `cornflow-1.1.0a2/airflow_config/plugins/XCom/gce_xcom_backend.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/airflow_config/webserver_ldap.py` & `cornflow-1.1.0a2/airflow_config/webserver_ldap.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/app.py` & `cornflow-1.1.0a2/cornflow/app.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/__init__.py` & `cornflow-1.1.0a2/cornflow/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/arguments.py` & `cornflow-1.1.0a2/cornflow/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/config.py` & `cornflow-1.1.0a2/cornflow/cli/config.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/migrations.py` & `cornflow-1.1.0a2/cornflow/cli/migrations.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/permissions.py` & `cornflow-1.1.0a2/cornflow/cli/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/schemas.py` & `cornflow-1.1.0a2/cornflow/cli/schemas.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/service.py` & `cornflow-1.1.0a2/cornflow/cli/service.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/tools/api_generator.py` & `cornflow-1.1.0a2/cornflow/cli/tools/api_generator.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/tools/endpoint_tools.py` & `cornflow-1.1.0a2/cornflow/cli/tools/endpoint_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/tools/models_tools.py` & `cornflow-1.1.0a2/cornflow/cli/tools/models_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/tools/schema_generator.py` & `cornflow-1.1.0a2/cornflow/cli/tools/schema_generator.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/tools/schemas_tools.py` & `cornflow-1.1.0a2/cornflow/cli/tools/schemas_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/tools/tools.py` & `cornflow-1.1.0a2/cornflow/cli/tools/tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/users.py` & `cornflow-1.1.0a2/cornflow/cli/users.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/utils.py` & `cornflow-1.1.0a2/cornflow/cli/utils.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/cli/views.py` & `cornflow-1.1.0a2/cornflow/cli/views.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/commands/__init__.py` & `cornflow-1.1.0a2/cornflow/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/commands/access.py` & `cornflow-1.1.0a2/cornflow/commands/access.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/commands/actions.py` & `cornflow-1.1.0a2/cornflow/commands/actions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/commands/dag.py` & `cornflow-1.1.0a2/cornflow/commands/dag.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/commands/permissions.py` & `cornflow-1.1.0a2/cornflow/commands/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/commands/roles.py` & `cornflow-1.1.0a2/cornflow/commands/roles.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/commands/schemas.py` & `cornflow-1.1.0a2/cornflow/commands/schemas.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/commands/users.py` & `cornflow-1.1.0a2/cornflow/commands/users.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/commands/views.py` & `cornflow-1.1.0a2/cornflow/commands/views.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/config.py` & `cornflow-1.1.0a2/cornflow/config.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/__init__.py` & `cornflow-1.1.0a2/cornflow/endpoints/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,72 +1,62 @@
 """
 Initialization file for the endpoints module
 All references to endpoints should be imported from here
 The login resource gets created on app startup as it depends on configuration
 """
 from .action import ActionListEndpoint
+from .alarms import AlarmsEndpoint
 from .apiview import ApiViewListEndpoint
-
 from .case import (
     CaseEndpoint,
     CaseFromInstanceExecutionEndpoint,
     CaseCopyEndpoint,
     CaseDetailsEndpoint,
     CaseDataEndpoint,
     CaseToInstance,
     CaseCompare,
 )
-
 from .dag import (
     DAGDetailEndpoint,
     DAGEndpointManual,
     DAGCaseEndpoint,
     DAGInstanceEndpoint,
     DeployedDAGEndpoint,
     DeployedDagDetailEndpoint,
 )
-
+from .data_check import (
+    DataCheckExecutionEndpoint,
+    DataCheckInstanceEndpoint,
+    DataCheckCaseEndpoint,
+)
+from .example_data import ExampleDataListEndpoint, ExampleDataDetailEndpoint
 from .execution import (
     ExecutionEndpoint,
     ExecutionDetailsEndpoint,
     ExecutionStatusEndpoint,
     ExecutionDataEndpoint,
     ExecutionLogEndpoint,
     ExecutionRelaunchEndpoint,
 )
-
 from .health import HealthEndpoint
-
 from .instance import (
     InstanceEndpoint,
     InstanceDetailsEndpoint,
     InstanceFileEndpoint,
     InstanceDataEndpoint,
 )
-
-from .data_check import (
-    DataCheckExecutionEndpoint,
-    DataCheckInstanceEndpoint,
-    DataCheckCaseEndpoint,
-)
 from .licenses import LicensesEndpoint
+from .main_alarms import MainAlarmsEndpoint
 from .permission import PermissionsViewRoleEndpoint, PermissionsViewRoleDetailEndpoint
-
 from .roles import RolesListEndpoint, RoleDetailEndpoint
-
 from .schemas import SchemaDetailsEndpoint, SchemaEndpoint
+from .tables import TablesEndpoint, TablesDetailsEndpoint
 from .token import TokenEndpoint
-from .example_data import ExampleDataDetailsEndpoint
 from .user import UserEndpoint, UserDetailsEndpoint, ToggleUserAdmin, RecoverPassword
 from .user_role import UserRoleListEndpoint, UserRoleDetailEndpoint
-from .alarms import AlarmsEndpoint
-from .main_alarms import MainAlarmsEndpoint
-
-from .tables import TablesEndpoint, TablesDetailsEndpoint
-
 
 resources = [
     dict(resource=InstanceEndpoint, urls="/instance/", endpoint="instance"),
     dict(
         resource=InstanceDetailsEndpoint,
         urls="/instance/<string:idx>/",
         endpoint="instances-detail",
@@ -153,18 +143,23 @@
     dict(resource=SchemaEndpoint, urls="/schema/", endpoint="schema"),
     dict(
         resource=SchemaDetailsEndpoint,
         urls="/schema/<string:dag_name>/",
         endpoint="schema-details",
     ),
     dict(
-        resource=ExampleDataDetailsEndpoint,
+        resource=ExampleDataListEndpoint,
         urls="/example/<string:dag_name>/",
         endpoint="example-data",
     ),
+    dict(
+        resource=ExampleDataDetailEndpoint,
+        urls="/example/<string:dag_name>/<string:example_name>/",
+        endpoint="example-data-detail",
+    ),
     dict(resource=HealthEndpoint, urls="/health/", endpoint="health"),
     dict(
         resource=CaseFromInstanceExecutionEndpoint,
         urls="/case/instance/",
         endpoint="case-instance-execution",
     ),
     dict(resource=CaseCopyEndpoint, urls="/case/<int:idx>/copy/", endpoint="case-copy"),
```

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/action.py` & `cornflow-1.1.0a2/cornflow/endpoints/action.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/alarms.py` & `cornflow-1.1.0a2/cornflow/endpoints/alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/apiview.py` & `cornflow-1.1.0a2/cornflow/endpoints/apiview.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/case.py` & `cornflow-1.1.0a2/cornflow/endpoints/case.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/dag.py` & `cornflow-1.1.0a2/cornflow/endpoints/dag.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/data_check.py` & `cornflow-1.1.0a2/cornflow/endpoints/data_check.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/example_data.py` & `cornflow-1.1.0a2/cornflow/endpoints/example_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,82 @@
 """
 Endpoints to get the example data from a DAG
 """
+import json
 
-# Import from libraries
 from cornflow_client.airflow.api import Airflow
 from flask import current_app, request
 from flask_apispec import marshal_with, doc
-import json
 
-# Import from internal modules
 from cornflow.endpoints.meta_resource import BaseMetaResource
 from cornflow.models import PermissionsDAG
-from cornflow.schemas.example_data import ExampleData
+from cornflow.schemas.example_data import ExampleListData, ExampleDetailData
 from cornflow.shared.authentication import Auth, authenticate
 from cornflow.shared.const import VIEWER_ROLE, PLANNER_ROLE, ADMIN_ROLE
-from cornflow.shared.exceptions import AirflowError, NoPermission
+from cornflow.shared.exceptions import AirflowError, NoPermission, ObjectDoesNotExist
 
 
-class ExampleDataDetailsEndpoint(BaseMetaResource):
+class ExampleDataListEndpoint(BaseMetaResource):
     """
     Endpoint used to obtain schemas for one app
     """
 
     ROLES_WITH_ACCESS = [VIEWER_ROLE, PLANNER_ROLE, ADMIN_ROLE]
 
-    @doc(description="Get example data from DAG", tags=["DAG"])
+    @doc(description="Get lsit of example data from DAG", tags=["DAG"])
     @authenticate(auth_class=Auth())
-    @marshal_with(ExampleData)
+    @marshal_with(ExampleListData(many=True))
     def get(self, dag_name):
         """
         API method to get example data for a given dag
 
+        :return: A dictionary with the names and descriptions of available data examples
+            and an integer with the HTTP status code
+        :rtype: Tuple(dict, integer)
+        """
+        user = Auth().get_user_from_header(request.headers)
+        permission = PermissionsDAG.check_if_has_permissions(
+            user_id=user.id, dag_id=dag_name
+        )
+
+        if permission:
+            af_client = Airflow.from_config(current_app.config)
+            if not af_client.is_alive():
+                current_app.logger.error(
+                    "Airflow not accessible when getting data {}".format(dag_name)
+                )
+                raise AirflowError(error="Airflow is not accessible")
+
+            # try airflow and see if dag_name exists
+            af_client.get_dag_info(dag_name)
+
+            current_app.logger.info("User gets example data from {}".format(dag_name))
+
+            variable_name = f"z_{dag_name}_examples"
+            response = af_client.get_one_variable(variable_name)
+
+            return json.loads(response["value"])
+        else:
+            err = "User does not have permission to access this dag."
+            raise NoPermission(
+                error=err,
+                status_code=403,
+                log_txt=f"Error while user {user} tries to get example data for dag {dag_name}. "
+                + err,
+            )
+
+
+class ExampleDataDetailEndpoint(BaseMetaResource):
+    @doc(description="Get example data from DAG", tags=["DAG"])
+    @authenticate(auth_class=Auth())
+    @marshal_with(ExampleDetailData)
+    def get(self, dag_name, example_name):
+        """
+        API method to get one example data for a given dag
+
         :return: A dictionary with a message and a integer with the HTTP status code
         :rtype: Tuple(dict, integer)
         """
         user = Auth().get_user_from_header(request.headers)
         permission = PermissionsDAG.check_if_has_permissions(
             user_id=user.id, dag_id=dag_name
         )
@@ -50,19 +92,28 @@
             # try airflow and see if dag_name exists
             af_client.get_dag_info(dag_name)
 
             current_app.logger.info("User gets example data from {}".format(dag_name))
 
             variable_name = f"z_{dag_name}_examples"
             response = af_client.get_one_variable(variable_name)
-            result = dict()
-            result["examples"] = json.loads(response["value"])
-            result["name"] = response["key"]
 
-            return result
+            example = None
+            for item in json.loads(response["value"]):
+                if item["name"] == example_name:
+                    example = item
+                    break
+
+            if example is None:
+                raise ObjectDoesNotExist(
+                    error="The example does not exist", status_code=404
+                )
+
+            return example
         else:
             err = "User does not have permission to access this dag."
             raise NoPermission(
                 error=err,
                 status_code=403,
-                log_txt=f"Error while user {user} tries to get example data for dag {dag_name}. " + err
+                log_txt=f"Error while user {user} tries to get example data for dag {dag_name}. "
+                + err,
             )
```

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/execution.py` & `cornflow-1.1.0a2/cornflow/endpoints/execution.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/health.py` & `cornflow-1.1.0a2/cornflow/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/instance.py` & `cornflow-1.1.0a2/cornflow/endpoints/instance.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/licenses.py` & `cornflow-1.1.0a2/cornflow/endpoints/licenses.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/login.py` & `cornflow-1.1.0a2/cornflow/endpoints/login.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/main_alarms.py` & `cornflow-1.1.0a2/cornflow/endpoints/main_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/meta_resource.py` & `cornflow-1.1.0a2/cornflow/endpoints/meta_resource.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/permission.py` & `cornflow-1.1.0a2/cornflow/endpoints/permission.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/roles.py` & `cornflow-1.1.0a2/cornflow/endpoints/roles.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/schemas.py` & `cornflow-1.1.0a2/cornflow/endpoints/schemas.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/signup.py` & `cornflow-1.1.0a2/cornflow/endpoints/signup.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/tables.py` & `cornflow-1.1.0a2/cornflow/endpoints/tables.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/token.py` & `cornflow-1.1.0a2/cornflow/endpoints/token.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/user.py` & `cornflow-1.1.0a2/cornflow/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/endpoints/user_role.py` & `cornflow-1.1.0a2/cornflow/endpoints/user_role.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/alembic.ini` & `cornflow-1.1.0a2/cornflow/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/env.py` & `cornflow-1.1.0a2/cornflow/migrations/env.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/00757b557b02_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/00757b557b02_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/1af47a419bbd_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/1af47a419bbd_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/4aac5e0c6e66_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/4aac5e0c6e66_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/7c3ea5ab5501_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/7c3ea5ab5501_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/991b98e24225_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/991b98e24225_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/a472b5ad50b7_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/a472b5ad50b7_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/c2db9409cb5f_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/c2db9409cb5f_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/c8a6c762e818_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/c8a6c762e818_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/ca449af8034c_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/ca449af8034c_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/d0e0700dcd8e_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/d0e0700dcd8e_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/d1b5be1f0549_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/d1b5be1f0549_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/e1a50dae1ac9_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/e1a50dae1ac9_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/e937a5234ce4_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/e937a5234ce4_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/ebdd955fcc5e_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/ebdd955fcc5e_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/migrations/versions/f3bee20314a2_.py` & `cornflow-1.1.0a2/cornflow/migrations/versions/f3bee20314a2_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/action.py` & `cornflow-1.1.0a2/cornflow/models/action.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/alarms.py` & `cornflow-1.1.0a2/cornflow/models/alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/base_data_model.py` & `cornflow-1.1.0a2/cornflow/models/base_data_model.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/case.py` & `cornflow-1.1.0a2/cornflow/models/case.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/dag.py` & `cornflow-1.1.0a2/cornflow/models/dag.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/dag_permissions.py` & `cornflow-1.1.0a2/cornflow/models/dag_permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/execution.py` & `cornflow-1.1.0a2/cornflow/models/execution.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/instance.py` & `cornflow-1.1.0a2/cornflow/models/instance.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/main_alarms.py` & `cornflow-1.1.0a2/cornflow/models/main_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/meta_models.py` & `cornflow-1.1.0a2/cornflow/models/meta_models.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/permissions.py` & `cornflow-1.1.0a2/cornflow/models/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/role.py` & `cornflow-1.1.0a2/cornflow/models/role.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/user.py` & `cornflow-1.1.0a2/cornflow/models/user.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/user_role.py` & `cornflow-1.1.0a2/cornflow/models/user_role.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/models/view.py` & `cornflow-1.1.0a2/cornflow/models/view.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/schemas/alarms.py` & `cornflow-1.1.0a2/cornflow/schemas/alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/schemas/case.py` & `cornflow-1.1.0a2/cornflow/schemas/case.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/schemas/dag.py` & `cornflow-1.1.0a2/cornflow/schemas/dag.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/schemas/execution.py` & `cornflow-1.1.0a2/cornflow/schemas/execution.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/schemas/instance.py` & `cornflow-1.1.0a2/cornflow/schemas/instance.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/schemas/main_alarms.py` & `cornflow-1.1.0a2/cornflow/schemas/main_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/schemas/permissions.py` & `cornflow-1.1.0a2/cornflow/schemas/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/schemas/query.py` & `cornflow-1.1.0a2/cornflow/schemas/query.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/schemas/solution_log.py` & `cornflow-1.1.0a2/cornflow/schemas/solution_log.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/schemas/user.py` & `cornflow-1.1.0a2/cornflow/schemas/user.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/schemas/user_role.py` & `cornflow-1.1.0a2/cornflow/schemas/user_role.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/shared/authentication/auth.py` & `cornflow-1.1.0a2/cornflow/shared/authentication/auth.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/shared/authentication/decorators.py` & `cornflow-1.1.0a2/cornflow/shared/authentication/decorators.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/shared/authentication/ldap.py` & `cornflow-1.1.0a2/cornflow/shared/authentication/ldap.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/shared/compress.py` & `cornflow-1.1.0a2/cornflow/shared/compress.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/shared/const.py` & `cornflow-1.1.0a2/cornflow/shared/const.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/shared/email.py` & `cornflow-1.1.0a2/cornflow/shared/email.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/shared/exceptions.py` & `cornflow-1.1.0a2/cornflow/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/shared/licenses.py` & `cornflow-1.1.0a2/cornflow/shared/licenses.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/shared/log_config.py` & `cornflow-1.1.0a2/cornflow/shared/log_config.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/shared/query_tools.py` & `cornflow-1.1.0a2/cornflow/shared/query_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/shared/utils.py` & `cornflow-1.1.0a2/cornflow/shared/utils.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/shared/utils_tables.py` & `cornflow-1.1.0a2/cornflow/shared/utils_tables.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/shared/validators.py` & `cornflow-1.1.0a2/cornflow/shared/validators.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/const.py` & `cornflow-1.1.0a2/cornflow/tests/const.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/custom_liveServer.py` & `cornflow-1.1.0a2/cornflow/tests/custom_liveServer.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/custom_test_case.py` & `cornflow-1.1.0a2/cornflow/tests/custom_test_case.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/integration/test_commands.py` & `cornflow-1.1.0a2/cornflow/tests/integration/test_commands.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/integration/test_cornflowclient.py` & `cornflow-1.1.0a2/cornflow/tests/integration/test_cornflowclient.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/ldap/test_ldap_authentication.py` & `cornflow-1.1.0a2/cornflow/tests/ldap/test_ldap_authentication.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_actions.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_actions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_alarms.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_apiview.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_apiview.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_cases.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_cases.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_cli.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         self.assertIn("Initialize the views", result.output)
 
     def test_views_init_command(self):
         runner = CliRunner()
         result = runner.invoke(cli, ["views", "init", "-v"])
         self.assertEqual(result.exit_code, 0)
         views = ViewModel.get_all_objects().all()
-        self.assertEqual(len(views), 48)
+        self.assertEqual(len(views), 49)
 
     def test_permissions_entrypoint(self):
         runner = CliRunner()
         result = runner.invoke(cli, ["permissions", "--help"])
         self.assertEqual(result.exit_code, 0)
         self.assertIn("Commands to manage the permissions", result.output)
         self.assertIn("init", result.output)
@@ -151,32 +151,32 @@
         self.assertEqual(result.exit_code, 0)
         actions = ActionModel.get_all_objects().all()
         roles = RoleModel.get_all_objects().all()
         views = ViewModel.get_all_objects().all()
         permissions = PermissionViewRoleModel.get_all_objects().all()
         self.assertEqual(len(actions), 5)
         self.assertEqual(len(roles), 4)
-        self.assertEqual(len(views), 48)
-        self.assertEqual(len(permissions), 530)
+        self.assertEqual(len(views), 49)
+        self.assertEqual(len(permissions), 546)
 
     def test_permissions_base_command(self):
         runner = CliRunner()
         runner.invoke(cli, ["actions", "init", "-v"])
         runner.invoke(cli, ["roles", "init", "-v"])
         runner.invoke(cli, ["views", "init", "-v"])
         result = runner.invoke(cli, ["permissions", "base", "-v"])
         self.assertEqual(result.exit_code, 0)
         actions = ActionModel.get_all_objects().all()
         roles = RoleModel.get_all_objects().all()
         views = ViewModel.get_all_objects().all()
         permissions = PermissionViewRoleModel.get_all_objects().all()
         self.assertEqual(len(actions), 5)
         self.assertEqual(len(roles), 4)
-        self.assertEqual(len(views), 48)
-        self.assertEqual(len(permissions), 530)
+        self.assertEqual(len(views), 49)
+        self.assertEqual(len(permissions), 546)
 
     def test_service_entrypoint(self):
         runner = CliRunner()
         result = runner.invoke(cli, ["service", "--help"])
         self.assertEqual(result.exit_code, 0)
         self.assertIn("Commands to run the cornflow service", result.output)
         self.assertIn("init", result.output)
```

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_commands.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_commands.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_dags.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_dags.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_data_checks.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_data_checks.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_executions.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_executions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_generate_from_schema.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_generate_from_schema.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_health.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_health.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_instances.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_instances.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_instances_file.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_instances_file.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_licenses.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_licenses.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_log_in.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_log_in.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_main_alarms.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_main_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_permissions.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_roles.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_roles.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_schema_from_models.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_schema_from_models.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_schemas.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_schemas.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_sign_up.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_sign_up.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_tables.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_tables.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_token.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_token.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/test_users.py` & `cornflow-1.1.0a2/cornflow/tests/unit/test_users.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow/tests/unit/tools.py` & `cornflow-1.1.0a2/cornflow/tests/unit/tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow.egg-info/PKG-INFO` & `cornflow-1.1.0a2/cornflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cornflow
-Version: 1.1.0a1
+Version: 1.1.0a2
 Summary: Cornflow is an open source multi-solver optimization server with a REST API built using flask.
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: cornflow@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow
         =========
```

### Comparing `cornflow-1.1.0a1/cornflow.egg-info/SOURCES.txt` & `cornflow-1.1.0a2/cornflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cornflow-1.1.0a1/cornflow.egg-info/requires.txt` & `cornflow-1.1.0a2/cornflow.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 alembic==1.9.2
 apispec<=6.2.0
 click<=8.1.3
-cornflow-client==1.1.0a1
+cornflow-client==1.1.0a2
 cryptography<=42.0.5
 disposable-email-domains>=0.0.86
 Flask==2.3.2
 flask-apispec<=0.11.4
 Flask-Bcrypt<=1.0.1
 Flask-Compress<=1.13
 flask-cors<=4.0.1
```

### Comparing `cornflow-1.1.0a1/setup.py` & `cornflow-1.1.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 required = []
 with open("requirements.txt", "r") as fh:
     required.append(fh.read().splitlines())
 
 setuptools.setup(
     name="cornflow",
-    version="1.1.0a1",
+    version="1.1.0a2",
     author="baobab soluciones",
     author_email="cornflow@baobabsoluciones.es",
     description="Cornflow is an open source multi-solver optimization server with a REST API built using flask.",
     long_description=long_description,
     url="https://github.com/baobabsoluciones/cornflow",
     packages=setuptools.find_packages(),
     install_requires=required,
```

