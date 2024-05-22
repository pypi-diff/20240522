# Comparing `tmp/cornflow-client-1.1.0a1.tar.gz` & `tmp/cornflow-client-1.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornflow-client-1.1.0a1.tar", last modified: Wed May 15 17:14:43 2024, max compression
+gzip compressed data, was "cornflow-client-1.1.0a2.tar", last modified: Tue May 21 19:00:34 2024, max compression
```

## Comparing `cornflow-client-1.1.0a1.tar` & `cornflow-client-1.1.0a2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.127325 cornflow-client-1.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-15 17:14:43.127325 cornflow-client-1.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.115325 cornflow-client-1.1.0a1/cornflow_client/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.119325 cornflow-client-1.1.0a1/cornflow_client/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/airflow/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/airflow/dag_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.119325 cornflow-client-1.1.0a1/cornflow_client/core/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    14822 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/instance_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/read_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/core/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/cornflow_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.119325 cornflow-client-1.1.0a1/cornflow_client/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/data/empty_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/data/pulp_json_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/data/schema_validator.json
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/data/solver_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/data/vrp_solution_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    29980 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/raw_cornflow_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.119325 cornflow-client-1.1.0a1/cornflow_client/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/schema/dictSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/schema/dict_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/schema/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/schema/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.119325 cornflow-client-1.1.0a1/cornflow_client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.123325 cornflow-client-1.1.0a1/cornflow_client/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30894 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/data_input_bad.json
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/data_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/endpoints_access.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/endpoints_methods.json
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/gc_input.json
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/gc_output.json
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/graph_coloring_input.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/graph_coloring_output.json
--rw-r--r--   0 runner    (1001) docker     (127)    30946 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/hk_data_input.json
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/hk_data_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/hk_solution_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/instance-hackathon2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/name_problem_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)   550476 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/pulp_example_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/schema_with_fk.json
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/schema_without_fk.json
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/test_mps.mps
--rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/xl_with_access.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/xl_with_fk.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    12361 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/xl_with_methods.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/data/xl_without_fk.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.123325 cornflow-client-1.1.0a1/cornflow_client/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/integration/test_airflow_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    21169 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/integration/test_cornflow_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    24798 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/integration/test_raw_cornflow_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.127325 cornflow-client-1.1.0a1/cornflow_client/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_dag_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    15639 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_instance_solution_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_schema_from_excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_schema_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_varnames.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:14:43.115325 cornflow-client-1.1.0a1/cornflow_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-15 17:14:42.000000 cornflow-client-1.1.0a1/cornflow_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-15 17:14:42.000000 cornflow-client-1.1.0a1/cornflow_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:14:42.000000 cornflow-client-1.1.0a1/cornflow_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 17:14:42.000000 cornflow-client-1.1.0a1/cornflow_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 17:14:42.000000 cornflow-client-1.1.0a1/cornflow_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 17:14:43.127325 cornflow-client-1.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-15 17:14:41.000000 cornflow-client-1.1.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:34.882633 cornflow-client-1.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-21 19:00:34.882633 cornflow-client-1.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:34.870633 cornflow-client-1.1.0a2/cornflow_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:34.870633 cornflow-client-1.1.0a2/cornflow_client/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/airflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/airflow/dag_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:34.870633 cornflow-client-1.1.0a2/cornflow_client/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/core/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14822 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/core/instance_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/core/read_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/core/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/core/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/cornflow_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:34.874633 cornflow-client-1.1.0a2/cornflow_client/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/data/empty_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/data/pulp_json_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/data/schema_validator.json
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/data/solver_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/data/vrp_solution_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30417 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/raw_cornflow_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:34.874633 cornflow-client-1.1.0a2/cornflow_client/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/schema/dictSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/schema/dict_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/schema/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/schema/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:34.874633 cornflow-client-1.1.0a2/cornflow_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:34.878633 cornflow-client-1.1.0a2/cornflow_client/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30894 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/data_input_bad.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/data_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/endpoints_access.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/endpoints_methods.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/gc_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/gc_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/graph_coloring_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/graph_coloring_output.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30946 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/hk_data_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/hk_data_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/hk_solution_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/instance-hackathon2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/name_problem_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)   550476 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/pulp_example_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/schema_with_fk.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/schema_without_fk.json
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/test_mps.mps
+-rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/xl_with_access.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/xl_with_fk.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    12361 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/xl_with_methods.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/data/xl_without_fk.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:34.878633 cornflow-client-1.1.0a2/cornflow_client/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/integration/test_airflow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/integration/test_cornflow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24798 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/integration/test_raw_cornflow_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:34.882633 cornflow-client-1.1.0a2/cornflow_client/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_dag_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15639 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_instance_solution_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_schema_from_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_schema_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_varnames.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:00:34.870633 cornflow-client-1.1.0a2/cornflow_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-21 19:00:34.000000 cornflow-client-1.1.0a2/cornflow_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-21 19:00:34.000000 cornflow-client-1.1.0a2/cornflow_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:00:34.000000 cornflow-client-1.1.0a2/cornflow_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-21 19:00:34.000000 cornflow-client-1.1.0a2/cornflow_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 19:00:34.000000 cornflow-client-1.1.0a2/cornflow_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:00:34.882633 cornflow-client-1.1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-21 19:00:33.000000 cornflow-client-1.1.0a2/setup.py
```

### Comparing `cornflow-client-1.1.0a1/LICENSE` & `cornflow-client-1.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/PKG-INFO` & `cornflow-client-1.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornflow-client
-Version: 1.1.0a1
+Version: 1.1.0a2
 Summary: Client to connect to a cornflow server
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow client
         ================
```

### Comparing `cornflow-client-1.1.0a1/README.rst` & `cornflow-client-1.1.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/airflow/api.py` & `cornflow-client-1.1.0a2/cornflow_client/airflow/api.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/airflow/dag_utilities.py` & `cornflow-client-1.1.0a2/cornflow_client/airflow/dag_utilities.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/constants.py` & `cornflow-client-1.1.0a2/cornflow_client/constants.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/core/application.py` & `cornflow-client-1.1.0a2/cornflow_client/core/application.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/core/experiment.py` & `cornflow-client-1.1.0a2/cornflow_client/core/experiment.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/core/instance.py` & `cornflow-client-1.1.0a2/cornflow_client/core/instance.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/core/instance_solution.py` & `cornflow-client-1.1.0a2/cornflow_client/core/instance_solution.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/core/read_tools.py` & `cornflow-client-1.1.0a2/cornflow_client/core/read_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/core/tools.py` & `cornflow-client-1.1.0a2/cornflow_client/core/tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/cornflow_client.py` & `cornflow-client-1.1.0a2/cornflow_client/cornflow_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,86 +4,104 @@
 class CornFlow:
     def __init__(self, url, token=None):
         self.raw = RawCornFlow(url, token)
 
         self.sign_up = self.expect_status(self.raw.sign_up, 201)
         self.create_instance = self.expect_status(self.raw.create_instance, 201)
         self.create_case = self.expect_status(self.raw.create_case, 201)
-        self.create_instance_file = self.expect_status(self.raw.create_instance_file, 201)
+        self.create_instance_file = self.expect_status(
+            self.raw.create_instance_file, 201
+        )
         self.create_execution = self.expect_status(self.raw.create_execution, 201)
         self.relaunch_execution = self.expect_status(self.raw.relaunch_execution, 201)
-        self.create_execution_data_check = self.expect_status(self.raw.create_execution_data_check, 201)
-        self.create_instance_data_check = self.expect_status(self.raw.create_instance_data_check, 201)
-        self.create_case_data_check = self.expect_status(self.raw.create_case_data_check, 201)
+        self.create_execution_data_check = self.expect_status(
+            self.raw.create_execution_data_check, 201
+        )
+        self.create_instance_data_check = self.expect_status(
+            self.raw.create_instance_data_check, 201
+        )
+        self.create_case_data_check = self.expect_status(
+            self.raw.create_case_data_check, 201
+        )
         self.get_data = self.expect_status(self.raw.get_data, 200)
         self.write_solution = self.expect_status(self.raw.write_solution, 200)
-        self.write_instance_checks = self.expect_status(self.raw.write_instance_checks, 200)
+        self.write_instance_checks = self.expect_status(
+            self.raw.write_instance_checks, 200
+        )
         self.write_case_checks = self.expect_status(self.raw.write_case_checks, 200)
         self.stop_execution = self.expect_status(self.raw.stop_execution, 200)
         self.manual_execution = self.expect_status(self.raw.manual_execution, 201)
         self.get_results = self.expect_status(self.raw.get_results, 200)
         self.get_status = self.expect_status(self.raw.get_status, 200)
         self.update_status = self.expect_status(self.raw.update_status, 200)
         self.get_log = self.expect_status(self.raw.get_log, 200)
         self.get_solution = self.expect_status(self.raw.get_solution, 200)
         self.get_all_instances = self.expect_status(self.raw.get_all_instances, 200)
         self.get_all_cases = self.expect_status(self.raw.get_all_cases, 200)
         self.get_all_executions = self.expect_status(self.raw.get_all_executions, 200)
         self.get_all_users = self.expect_status(self.raw.get_all_users, 200)
         self.get_one_user = self.expect_status(self.raw.get_one_user, 200)
         self.get_one_instance = self.expect_status(self.raw.get_one_instance, 200)
-        self.get_one_instance_data = self.expect_status(self.raw.get_one_instance_data, 200)
+        self.get_one_instance_data = self.expect_status(
+            self.raw.get_one_instance_data, 200
+        )
         self.get_one_case = self.expect_status(self.raw.get_one_case, 200)
         self.get_one_case_data = self.expect_status(self.raw.get_one_case_data, 200)
         self.put_one_case = self.expect_status(self.raw.put_one_case, 200)
         self.put_one_instance = self.expect_status(self.raw.put_one_instance, 200)
         self.put_one_execution = self.expect_status(self.raw.put_one_execution, 200)
         self.patch_one_case = self.expect_status(self.raw.patch_one_case, 200)
         self.delete_one_instance = self.expect_status(self.raw.delete_one_instance, 200)
         self.delete_one_case = self.expect_status(self.raw.delete_one_case, 200)
-        self.delete_one_execution = self.expect_status(self.raw.delete_one_execution, 200)
+        self.delete_one_execution = self.expect_status(
+            self.raw.delete_one_execution, 200
+        )
         self.get_schema = self.expect_status(self.raw.get_schema, 200)
         self.get_all_schemas = self.expect_status(self.raw.get_all_schemas, 200)
         self.get_deployed_dags = self.expect_status(self.raw.get_deployed_dags, 200)
         self.create_deployed_dag = self.expect_status(self.raw.create_deployed_dag, 201)
         self.put_deployed_dag = self.expect_status(self.raw.put_deployed_dag, 200)
+        self.get_example_list = self.expect_status(self.raw.get_example_list, 200)
+        self.get_one_example = self.expect_status(self.raw.get_one_example, 200)
 
     @property
     def url(self):
-        """ Gets the url of the server """
+        """Gets the url of the server"""
         return self.raw.url
 
     @url.setter
     def url(self, url):
-        """ Sets the url of the server """
+        """Sets the url of the server"""
         self.raw.url = url
 
     @property
     def token(self):
-        """ Gets the token """
+        """Gets the token"""
         return self.raw.token
 
     @token.setter
     def token(self, token):
-        """ Sets the token """
+        """Sets the token"""
         self.raw.token = token
 
     @staticmethod
     def expect_status(func, expected_status=None):
         """
         Gets the response of the call
         and raise an exception if the status of the response is not the expected
         """
+
         def decorator(*args, **kwargs):
             response = func(*args, **kwargs)
             if expected_status is not None and response.status_code != expected_status:
                 raise CornFlowApiError(
                     f"Expected a code {expected_status}, got a {response.status_code} error instead: {response.text}"
                 )
             return response.json()
+
         return decorator
 
     def is_alive(self):
         """
         Asks the server if it's alive
         """
         response = self.raw.is_alive()
```

### Comparing `cornflow-client-1.1.0a1/cornflow_client/data/pulp_json_schema.json` & `cornflow-client-1.1.0a2/cornflow_client/data/pulp_json_schema.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/data/schema_validator.json` & `cornflow-client-1.1.0a2/cornflow_client/data/schema_validator.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/data/solver_config.json` & `cornflow-client-1.1.0a2/cornflow_client/data/solver_config.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/raw_cornflow_client.py` & `cornflow-client-1.1.0a2/cornflow_client/raw_cornflow_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -891,14 +891,28 @@
     @ask_token
     @prepare_encoding
     def put_deployed_dag(self, dag_id, data, encoding=None):
         return self.put_api_for_id(
             "dag/deployed/", dag_id, payload=data, encoding=encoding
         )
 
+    @log_call
+    @ask_token
+    @prepare_encoding
+    def get_example_list(self, dag_name, encoding=None):
+        return self.get_api_for_id(api="example", id=dag_name, encoding=encoding)
+
+    @log_call
+    @ask_token
+    @prepare_encoding
+    def get_one_example(self, dag_name, example_name, encoding=None):
+        return self.get_api_for_id(
+            api="example", id=f"{dag_name}/{example_name}", encoding=encoding
+        )
+
 
 class CornFlowApiError(Exception):
     """
     CornFlow returns an error
     """
 
     pass
```

### Comparing `cornflow-client-1.1.0a1/cornflow_client/schema/dictSchema.py` & `cornflow-client-1.1.0a2/cornflow_client/schema/dictSchema.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/schema/dict_functions.py` & `cornflow-client-1.1.0a2/cornflow_client/schema/dict_functions.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/schema/manager.py` & `cornflow-client-1.1.0a2/cornflow_client/schema/manager.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/schema/tools.py` & `cornflow-client-1.1.0a2/cornflow_client/schema/tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/const.py` & `cornflow-client-1.1.0a2/cornflow_client/tests/const.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/data_input_bad.json` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/data_input_bad.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/data_schema.json` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/data_schema.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/gc_input.json` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/gc_input.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/gc_output.json` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/gc_output.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/graph_coloring_input.json` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/graph_coloring_input.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/hk_data_input.json` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/hk_data_input.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/hk_data_schema.json` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/hk_data_schema.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/instance-hackathon2.json` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/instance-hackathon2.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/name_problem_schema.json` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/name_problem_schema.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/pulp_example_data.json` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/pulp_example_data.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/schema_with_fk.json` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/schema_with_fk.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/schema_without_fk.json` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/schema_without_fk.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/test_mps.mps` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/test_mps.mps`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/xl_with_access.xlsx` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/xl_with_access.xlsx`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/xl_with_fk.xlsx` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/xl_with_fk.xlsx`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/xl_with_methods.xlsx` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/xl_with_methods.xlsx`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/data/xl_without_fk.xlsx` & `cornflow-client-1.1.0a2/cornflow_client/tests/data/xl_without_fk.xlsx`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/integration/test_airflow_integration.py` & `cornflow-client-1.1.0a2/cornflow_client/tests/integration/test_airflow_integration.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/integration/test_cornflow_integration.py` & `cornflow-client-1.1.0a2/cornflow_client/tests/integration/test_cornflow_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -531,14 +531,23 @@
     def test_get_all_schemas(self):
         response = self.client.get_all_schemas()
         read_schemas = [dag for v in response for (_, dag) in v.items()]
 
         for schema in PUBLIC_DAGS:
             self.assertIn(schema, read_schemas)
 
+    def test_get_example_list(self):
+        response = self.client.get_example_list("rostering")
+        self.assertEqual(7, len(response))
+
+    def test_get_one_example(self):
+        response = self.client.get_one_example("rostering", "Base case")
+        self.assertIn("instance", response)
+        self.assertIn("solution", response)
+
 
 class TestCornflowClientAdmin(TestCase):
     def setUp(self):
         self.client = CornFlow(url="http://127.0.0.1:5050/")
         login_result = self.client.login("admin", "Adminpassword1!")
         self.assertIn("id", login_result.keys())
         self.assertIn("token", login_result.keys())
```

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/integration/test_raw_cornflow_integration.py` & `cornflow-client-1.1.0a2/cornflow_client/tests/integration/test_raw_cornflow_integration.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_abc.py` & `cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_abc.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_core.py` & `cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_dag_utilities.py` & `cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_dag_utilities.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_instance_solution_methods.py` & `cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_instance_solution_methods.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_schema_from_excel.py` & `cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_schema_from_excel.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_schema_manager.py` & `cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client/tests/unit/test_varnames.py` & `cornflow-client-1.1.0a2/cornflow_client/tests/unit/test_varnames.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/cornflow_client.egg-info/PKG-INFO` & `cornflow-client-1.1.0a2/cornflow_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornflow-client
-Version: 1.1.0a1
+Version: 1.1.0a2
 Summary: Client to connect to a cornflow server
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow client
         ================
```

### Comparing `cornflow-client-1.1.0a1/cornflow_client.egg-info/SOURCES.txt` & `cornflow-client-1.1.0a2/cornflow_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.1.0a1/setup.py` & `cornflow-client-1.1.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     required.append(fh.read().splitlines())
 
 extra_required = {"excel": ["openpyxl", "pandas"]}
 
 
 setuptools.setup(
     name="cornflow-client",
-    version="1.1.0a1",
+    version="1.1.0a2",
     author="baobab soluciones",
     author_email="sistemas@baobabsoluciones.es",
     description="Client to connect to a cornflow server",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/baobabsoluciones/cornflow",
     packages=setuptools.find_packages(),
```

