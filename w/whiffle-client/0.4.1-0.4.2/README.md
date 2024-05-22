# Comparing `tmp/whiffle_client-0.4.1.tar.gz` & `tmp/whiffle_client-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whiffle_client-0.4.1.tar", last modified: Tue May 21 12:37:55 2024, max compression
+gzip compressed data, was "whiffle_client-0.4.2.tar", last modified: Wed May 22 15:34:53 2024, max compression
```

## Comparing `whiffle_client-0.4.1.tar` & `whiffle_client-0.4.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.460646 whiffle_client-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/LICENCE.txt
--rw-r--r--   0 root         (0) root         (0)    11095 2024-05-21 12:37:55.459645 whiffle_client-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)    10139 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/USER_README.md
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 12:37:55.460646 whiffle_client-0.4.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.449645 whiffle_client-0.4.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2506 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2096 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/tests/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.450645 whiffle_client-0.4.1/whiffle_client/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.453645 whiffle_client-0.4.1/whiffle_client/analysis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7628 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/analysis/io.py
--rw-rw-rw-   0 root         (0) root         (0)    16433 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/analysis/plot.py
--rw-rw-rw-   0 root         (0) root         (0)     4854 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/analysis/scatter.py
--rw-rw-rw-   0 root         (0) root         (0)     4957 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/analysis/skill.py
--rw-rw-rw-   0 root         (0) root         (0)     3231 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/analysis/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3995 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/base_client.py
--rw-rw-rw-   0 root         (0) root         (0)     6260 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1400 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     3218 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/entrypoints.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.453645 whiffle_client-0.4.1/whiffle_client/loaders/
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/loaders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1226 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/loaders/csv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.454645 whiffle_client-0.4.1/whiffle_client/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/resources/example_generic_params.json
--rw-rw-rw-   0 root         (0) root         (0)     1015 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/resources/example_yaml_include.yaml
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/resources/example_yaml_include_metmasts.yaml
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/resources/whiffle_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.454645 whiffle_client-0.4.1/whiffle_client/snippets/
--rw-rw-rw-   0 root         (0) root         (0)     2401 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/snippets/create_mock_powercurve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.455645 whiffle_client-0.4.1/whiffle_client/wind/
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.457646 whiffle_client-0.4.1/whiffle_client/wind/components/
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      183 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/dates.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/domain.py
--rw-rw-rw-   0 root         (0) root         (0)      212 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/geometries.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/metmast.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/turbine.py
--rw-rw-rw-   0 root         (0) root         (0)     1166 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/turbine_model_specs.py
--rw-rw-rw-   0 root         (0) root         (0)     5240 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/wind_simulation_task.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/components/windfarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.458645 whiffle_client-0.4.1/whiffle_client/wind/mapping/
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/mapping/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/mapping/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4808 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/mapping/turbine_model_specs.py
--rw-rw-rw-   0 root         (0) root         (0)     6023 2024-05-21 12:37:52.000000 whiffle_client-0.4.1/whiffle_client/wind/mapping/wind_simulation_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:37:55.458645 whiffle_client-0.4.1/whiffle_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11095 2024-05-21 12:37:55.000000 whiffle_client-0.4.1/whiffle_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1652 2024-05-21 12:37:55.000000 whiffle_client-0.4.1/whiffle_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 12:37:55.000000 whiffle_client-0.4.1/whiffle_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-05-21 12:37:55.000000 whiffle_client-0.4.1/whiffle_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      189 2024-05-21 12:37:55.000000 whiffle_client-0.4.1/whiffle_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-21 12:37:55.000000 whiffle_client-0.4.1/whiffle_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:34:53.734245 whiffle_client-0.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)    11095 2024-05-22 15:34:53.733245 whiffle_client-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    10139 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/USER_README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 15:34:53.734245 whiffle_client-0.4.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:34:53.723245 whiffle_client-0.4.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:34:53.724245 whiffle_client-0.4.2/whiffle_client/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:34:53.727245 whiffle_client-0.4.2/whiffle_client/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7628 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/analysis/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    16433 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/analysis/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     4854 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/analysis/scatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4957 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/analysis/skill.py
+-rw-rw-rw-   0 root         (0) root         (0)     3231 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/analysis/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3995 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/base_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3218 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/entrypoints.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:34:53.727245 whiffle_client-0.4.2/whiffle_client/loaders/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/loaders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/loaders/csv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:34:53.728245 whiffle_client-0.4.2/whiffle_client/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/resources/example_generic_params.json
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/resources/example_yaml_include.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/resources/example_yaml_include_metmasts.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/resources/whiffle_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:34:53.729245 whiffle_client-0.4.2/whiffle_client/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/snippets/create_mock_powercurve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:34:53.729245 whiffle_client-0.4.2/whiffle_client/wind/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:34:53.731245 whiffle_client-0.4.2/whiffle_client/wind/components/
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      183 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/components/dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/components/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/components/geometries.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/components/metmast.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/components/turbine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/components/turbine_model_specs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5252 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/components/wind_simulation_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/components/windfarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:34:53.732245 whiffle_client-0.4.2/whiffle_client/wind/mapping/
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/mapping/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/mapping/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4808 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/mapping/turbine_model_specs.py
+-rw-rw-rw-   0 root         (0) root         (0)     6023 2024-05-22 15:34:50.000000 whiffle_client-0.4.2/whiffle_client/wind/mapping/wind_simulation_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:34:53.732245 whiffle_client-0.4.2/whiffle_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11095 2024-05-22 15:34:53.000000 whiffle_client-0.4.2/whiffle_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1652 2024-05-22 15:34:53.000000 whiffle_client-0.4.2/whiffle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 15:34:53.000000 whiffle_client-0.4.2/whiffle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-05-22 15:34:53.000000 whiffle_client-0.4.2/whiffle_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2024-05-22 15:34:53.000000 whiffle_client-0.4.2/whiffle_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-22 15:34:53.000000 whiffle_client-0.4.2/whiffle_client.egg-info/top_level.txt
```

### Comparing `whiffle_client-0.4.1/LICENCE.txt` & `whiffle_client-0.4.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/PKG-INFO` & `whiffle_client-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `whiffle_client-0.4.1/README.md` & `whiffle_client-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/USER_README.md` & `whiffle_client-0.4.2/USER_README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/pyproject.toml` & `whiffle_client-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/tests/test_cli.py` & `whiffle_client-0.4.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/tests/test_client.py` & `whiffle_client-0.4.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/analysis/io.py` & `whiffle_client-0.4.2/whiffle_client/analysis/io.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/analysis/plot.py` & `whiffle_client-0.4.2/whiffle_client/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/analysis/scatter.py` & `whiffle_client-0.4.2/whiffle_client/analysis/scatter.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/analysis/skill.py` & `whiffle_client-0.4.2/whiffle_client/analysis/skill.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/analysis/utils.py` & `whiffle_client-0.4.2/whiffle_client/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/base_client.py` & `whiffle_client-0.4.2/whiffle_client/base_client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/client.py` & `whiffle_client-0.4.2/whiffle_client/client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/decorators.py` & `whiffle_client-0.4.2/whiffle_client/decorators.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/entrypoints.py` & `whiffle_client-0.4.2/whiffle_client/entrypoints.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/io.py` & `whiffle_client-0.4.2/whiffle_client/io.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/loaders/csv.py` & `whiffle_client-0.4.2/whiffle_client/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/resources/example_generic_params.json` & `whiffle_client-0.4.2/whiffle_client/resources/example_generic_params.json`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/resources/example_yaml_include.yaml` & `whiffle_client-0.4.2/whiffle_client/resources/example_yaml_include.yaml`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/snippets/create_mock_powercurve.py` & `whiffle_client-0.4.2/whiffle_client/snippets/create_mock_powercurve.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/wind/client.py` & `whiffle_client-0.4.2/whiffle_client/wind/client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/wind/components/__init__.py` & `whiffle_client-0.4.2/whiffle_client/wind/components/__init__.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/wind/components/turbine_model_specs.py` & `whiffle_client-0.4.2/whiffle_client/wind/components/turbine_model_specs.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/wind/components/wind_simulation_task.py` & `whiffle_client-0.4.2/whiffle_client/wind/components/wind_simulation_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         "test_run",
         "price",
         "price_overview",
         "reference_number",
         "configuration_valid",
         "geometries",
         "domain",
+        "progress",
     ]
 )
 
 
 @dataclass
 class WindSimulationTask:
     # Metadata attributes
@@ -64,15 +65,15 @@
     metmasts: list[Metmast] = field(default_factory=list)
     metmasts_heights: list[float] = field(default_factory=list)
 
     # Output attributes
     wind_resource_grid_heights: list[float] = field(default_factory=list)
     fields_heights: list[float] = field(default_factory=list)
 
-    progress: dict = field(default_factory=dict)
+    progress: dict = field(default=None)
 
     @classmethod
     def from_dict(cls, env):
         return cls(
             **{k: v for k, v in env.items() if k in inspect.signature(cls).parameters}
         )
```

### Comparing `whiffle_client-0.4.1/whiffle_client/wind/mapping/base.py` & `whiffle_client-0.4.2/whiffle_client/wind/mapping/base.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/wind/mapping/turbine_model_specs.py` & `whiffle_client-0.4.2/whiffle_client/wind/mapping/turbine_model_specs.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client/wind/mapping/wind_simulation_tasks.py` & `whiffle_client-0.4.2/whiffle_client/wind/mapping/wind_simulation_tasks.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.4.1/whiffle_client.egg-info/PKG-INFO` & `whiffle_client-0.4.2/whiffle_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `whiffle_client-0.4.1/whiffle_client.egg-info/SOURCES.txt` & `whiffle_client-0.4.2/whiffle_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

