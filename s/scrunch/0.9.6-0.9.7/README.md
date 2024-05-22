# Comparing `tmp/scrunch-0.9.6.tar.gz` & `tmp/scrunch-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scrunch-0.9.6.tar", last modified: Mon Jun 28 15:21:25 2021, max compression
+gzip compressed data, was "dist/scrunch-0.9.7.tar", last modified: Thu Sep  2 20:49:12 2021, max compression
```

## Comparing `scrunch-0.9.6.tar` & `scrunch-0.9.7.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:21:25.000000 scrunch-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-06-28 15:21:20.000000 scrunch-0.9.6/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      122 2021-06-28 15:21:20.000000 scrunch-0.9.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:21:25.000000 scrunch-0.9.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:21:25.000000 scrunch-0.9.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1926 2021-06-28 15:21:20.000000 scrunch-0.9.6/.github/workflows/test-and-deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-06-28 15:21:20.000000 scrunch-0.9.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-06-28 15:21:20.000000 scrunch-0.9.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-28 15:21:20.000000 scrunch-0.9.6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2021-06-28 15:21:20.000000 scrunch-0.9.6/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-06-28 15:21:20.000000 scrunch-0.9.6/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2021-06-28 15:21:20.000000 scrunch-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2021-06-28 15:21:25.000000 scrunch-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2021-06-28 15:21:20.000000 scrunch-0.9.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      454 2021-06-28 15:21:20.000000 scrunch-0.9.6/appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-06-28 15:21:20.000000 scrunch-0.9.6/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:21:25.000000 scrunch-0.9.6/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2021-06-28 15:21:20.000000 scrunch-0.9.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-06-28 15:21:20.000000 scrunch-0.9.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      287 2021-06-28 15:21:20.000000 scrunch-0.9.6/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:21:25.000000 scrunch-0.9.6/integration/
--rw-r--r--   0 runner    (1001) docker     (121)     4364 2021-06-28 15:21:20.000000 scrunch-0.9.6/integration/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)    12036 2021-06-28 15:21:20.000000 scrunch-0.9.6/integration/test_backfill.py
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2021-06-28 15:21:20.000000 scrunch-0.9.6/integration/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    12609 2021-06-28 15:21:20.000000 scrunch-0.9.6/integration/test_folders.py
--rw-r--r--   0 runner    (1001) docker     (121)     4148 2021-06-28 15:21:20.000000 scrunch-0.9.6/integration/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (121)    10870 2021-06-28 15:21:20.000000 scrunch-0.9.6/integration/test_recodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2021-06-28 15:21:20.000000 scrunch-0.9.6/integration/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-06-28 15:21:20.000000 scrunch-0.9.6/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-06-28 15:21:20.000000 scrunch-0.9.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:21:25.000000 scrunch-0.9.6/scrunch/
--rw-r--r--   0 runner    (1001) docker     (121)      455 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3444 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/categories.py
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/cubes.py
--rw-r--r--   0 runner    (1001) docker     (121)   131960 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    29072 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/expressions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8158 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/folders.py
--rw-r--r--   0 runner    (1001) docker     (121)     8151 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    13202 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/mutable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    18644 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/order.py
--rw-r--r--   0 runner    (1001) docker     (121)     2142 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/scripts.py
--rw-r--r--   0 runner    (1001) docker     (121)      820 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/session.py
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/streaming_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     8879 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/subentity.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:21:25.000000 scrunch-0.9.6/scrunch/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/crunch_test.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:21:25.000000 scrunch-0.9.6/scrunch/tests/integration/
--rwxr-xr-x   0 runner    (1001) docker     (121)    38590 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/integration/scrunch_workflow_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2057 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/mock_session.py
--rw-r--r--   0 runner    (1001) docker     (121)     9190 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/test_categories.py
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/test_cubes.py
--rw-r--r--   0 runner    (1001) docker     (121)   283939 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)   100707 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6095 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/test_folders.py
--rw-r--r--   0 runner    (1001) docker     (121)    17431 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (121)    20596 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/test_recodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3663 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/test_teams.py
--rw-r--r--   0 runner    (1001) docker     (121)    10989 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     2453 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/variables.py
--rw-r--r--   0 runner    (1001) docker     (121)      206 2021-06-28 15:21:20.000000 scrunch-0.9.6/scrunch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:21:25.000000 scrunch-0.9.6/scrunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2021-06-28 15:21:24.000000 scrunch-0.9.6/scrunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2021-06-28 15:21:25.000000 scrunch-0.9.6/scrunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-28 15:21:24.000000 scrunch-0.9.6/scrunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-28 15:21:24.000000 scrunch-0.9.6/scrunch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-06-28 15:21:24.000000 scrunch-0.9.6/scrunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-06-28 15:21:24.000000 scrunch-0.9.6/scrunch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-06-28 15:21:25.000000 scrunch-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1975 2021-06-28 15:21:20.000000 scrunch-0.9.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2021-06-28 15:21:20.000000 scrunch-0.9.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 20:49:12.000000 scrunch-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-09-02 20:49:05.000000 scrunch-0.9.7/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2021-09-02 20:49:05.000000 scrunch-0.9.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 20:49:12.000000 scrunch-0.9.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 20:49:12.000000 scrunch-0.9.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1926 2021-09-02 20:49:05.000000 scrunch-0.9.7/.github/workflows/test-and-deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-09-02 20:49:05.000000 scrunch-0.9.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2021-09-02 20:49:05.000000 scrunch-0.9.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-02 20:49:05.000000 scrunch-0.9.7/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    35148 2021-09-02 20:49:05.000000 scrunch-0.9.7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-09-02 20:49:05.000000 scrunch-0.9.7/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (121)     7651 2021-09-02 20:49:05.000000 scrunch-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2021-09-02 20:49:12.000000 scrunch-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2021-09-02 20:49:05.000000 scrunch-0.9.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2021-09-02 20:49:05.000000 scrunch-0.9.7/appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-09-02 20:49:05.000000 scrunch-0.9.7/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 20:49:12.000000 scrunch-0.9.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2021-09-02 20:49:05.000000 scrunch-0.9.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-09-02 20:49:05.000000 scrunch-0.9.7/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2021-09-02 20:49:05.000000 scrunch-0.9.7/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 20:49:12.000000 scrunch-0.9.7/integration/
+-rw-r--r--   0 runner    (1001) docker     (121)     4364 2021-09-02 20:49:05.000000 scrunch-0.9.7/integration/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12036 2021-09-02 20:49:05.000000 scrunch-0.9.7/integration/test_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2710 2021-09-02 20:49:05.000000 scrunch-0.9.7/integration/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12014 2021-09-02 20:49:05.000000 scrunch-0.9.7/integration/test_folders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4148 2021-09-02 20:49:05.000000 scrunch-0.9.7/integration/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10870 2021-09-02 20:49:05.000000 scrunch-0.9.7/integration/test_recodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3075 2021-09-02 20:49:05.000000 scrunch-0.9.7/integration/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2021-09-02 20:49:05.000000 scrunch-0.9.7/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-09-02 20:49:05.000000 scrunch-0.9.7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 20:49:12.000000 scrunch-0.9.7/scrunch/
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3444 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/categories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1425 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/cubes.py
+-rw-r--r--   0 runner    (1001) docker     (121)   131960 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29072 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8158 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/folders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8151 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13202 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/mutable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18334 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/order.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2142 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      820 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/session.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1979 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/streaming_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8879 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/subentity.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 20:49:12.000000 scrunch-0.9.7/scrunch/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/crunch_test.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 20:49:12.000000 scrunch-0.9.7/scrunch/tests/integration/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    38590 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/integration/scrunch_workflow_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2057 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/mock_session.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9190 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/test_categories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/test_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (121)   283939 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)   100707 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6095 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/test_folders.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17431 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20596 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/test_recodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2724 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3663 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/test_teams.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10774 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2453 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/variables.py
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2021-09-02 20:49:05.000000 scrunch-0.9.7/scrunch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 20:49:12.000000 scrunch-0.9.7/scrunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2021-09-02 20:49:12.000000 scrunch-0.9.7/scrunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1443 2021-09-02 20:49:12.000000 scrunch-0.9.7/scrunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-02 20:49:12.000000 scrunch-0.9.7/scrunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-02 20:49:12.000000 scrunch-0.9.7/scrunch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2021-09-02 20:49:12.000000 scrunch-0.9.7/scrunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-09-02 20:49:12.000000 scrunch-0.9.7/scrunch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2021-09-02 20:49:12.000000 scrunch-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1982 2021-09-02 20:49:05.000000 scrunch-0.9.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1001 2021-09-02 20:49:05.000000 scrunch-0.9.7/tox.ini
```

### Comparing `scrunch-0.9.6/.github/workflows/test-and-deploy.yaml` & `scrunch-0.9.7/.github/workflows/test-and-deploy.yaml`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/.gitignore` & `scrunch-0.9.7/.gitignore`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/COPYING` & `scrunch-0.9.7/COPYING`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/COPYING.LESSER` & `scrunch-0.9.7/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/LICENSE` & `scrunch-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/PKG-INFO` & `scrunch-0.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrunch
-Version: 0.9.6
+Version: 0.9.7
 Summary: Pythonic scripting library for cleaning data in Crunch
 Home-page: https://github.com/Crunch-io/scrunch
 Author: Crunch.io
 Author-email: dev@crunch.io
 License: UNKNOWN
 Description: .. image:: https://img.shields.io/pypi/v/scrunch.svg
            :target: https://pypi.org/project/scrunch
```

### Comparing `scrunch-0.9.6/README.rst` & `scrunch-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/docs/conf.py` & `scrunch-0.9.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/integration/fixtures.py` & `scrunch-0.9.7/integration/fixtures.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/integration/test_backfill.py` & `scrunch-0.9.7/integration/test_backfill.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/integration/test_dataset.py` & `scrunch-0.9.7/integration/test_dataset.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/integration/test_folders.py` & `scrunch-0.9.7/integration/test_folders.py`

 * *Files 7% similar despite different names*

```diff
@@ -273,29 +273,14 @@
         var1_id = var1.resource.body.id
         var2_id = var2.resource.body.id
         self.assertTrue(var2_id in self._ds.folders.hidden.by('id'))
         self.assertTrue(var2_id not in self._ds.folders.by('id'))
         self.assertTrue(var1_id in self._ds.folders.by('id'))
         self.assertTrue(var1_id not in self._ds.folders.hidden.by('id'))
 
-    def test_trash_variables(self):
-        trash = self.ds.folders.trash
-        root = self.ds.folders.root
-        var1 = self.ds['testvar4']
-        var2 = self.ds['testvar5']
-        root.move_here(var1, var2)
-        trash.move_here(var2)
-
-        var1_id = var1.resource.body.id
-        var2_id = var2.resource.body.id
-        self.assertTrue(var2_id in self._ds.folders.trash.by('id'))
-        self.assertTrue(var2_id not in self._ds.folders.by('id'))
-        self.assertTrue(var1_id in self._ds.folders.by('id'))
-        self.assertTrue(var1_id not in self._ds.folders.trash.by('id'))
-
     def test_rename(self):
         root = self.ds.folders.root
         sf = root.create_folder('rename me')
         sf.rename("renamed")
         self.assertTrue('renamed' in [c.name for c in root.children])
         self.assertEqual(sf.name, 'renamed')
```

### Comparing `scrunch-0.9.6/integration/test_projects.py` & `scrunch-0.9.7/integration/test_projects.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/integration/test_recodes.py` & `scrunch-0.9.7/integration/test_recodes.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/integration/test_scripts.py` & `scrunch-0.9.7/integration/test_scripts.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/categories.py` & `scrunch-0.9.7/scrunch/categories.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/cubes.py` & `scrunch-0.9.7/scrunch/cubes.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/datasets.py` & `scrunch-0.9.7/scrunch/datasets.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/expressions.py` & `scrunch-0.9.7/scrunch/expressions.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/folders.py` & `scrunch-0.9.7/scrunch/folders.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/helpers.py` & `scrunch-0.9.7/scrunch/helpers.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/mutable_dataset.py` & `scrunch-0.9.7/scrunch/mutable_dataset.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/order.py` & `scrunch-0.9.7/scrunch/order.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,14 @@
 
 
 class Path(object):
     def __init__(self, path):
         if not isinstance(path, six.string_types):
             raise TypeError('The path must be a string object')
 
-        if six.PY2:
-            regex_match = re.match(NAME_REGEX, path.decode('utf-8'))
-        else:
-            regex_match = re.match(NAME_REGEX, path)
-
-        if not regex_match:
-            raise InvalidPathError(
-                'Invalid path %s: it contains invalid characters.' % path
-            )
-
         self.path = path
 
     @property
     def is_root(self):
         return self.path == '|'
 
     @property
```

### Comparing `scrunch-0.9.6/scrunch/scripts.py` & `scrunch-0.9.7/scrunch/scripts.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/session.py` & `scrunch-0.9.7/scrunch/session.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/streaming_dataset.py` & `scrunch-0.9.7/scrunch/streaming_dataset.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/subentity.py` & `scrunch-0.9.7/scrunch/subentity.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/tests/integration/scrunch_workflow_integration_test.py` & `scrunch-0.9.7/scrunch/tests/integration/scrunch_workflow_integration_test.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/tests/mock_session.py` & `scrunch-0.9.7/scrunch/tests/mock_session.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/tests/test_categories.py` & `scrunch-0.9.7/scrunch/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/tests/test_cubes.py` & `scrunch-0.9.7/scrunch/tests/test_cubes.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/tests/test_datasets.py` & `scrunch-0.9.7/scrunch/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/tests/test_expressions.py` & `scrunch-0.9.7/scrunch/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/tests/test_folders.py` & `scrunch-0.9.7/scrunch/tests/test_folders.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/tests/test_projects.py` & `scrunch-0.9.7/scrunch/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/tests/test_recodes.py` & `scrunch-0.9.7/scrunch/tests/test_recodes.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/tests/test_scripts.py` & `scrunch-0.9.7/scrunch/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/tests/test_teams.py` & `scrunch-0.9.7/scrunch/tests/test_teams.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch/tests/test_utilities.py` & `scrunch-0.9.7/scrunch/tests/test_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,18 +292,14 @@
         assert isinstance(user, User)
 
     def test_path(self):
         with pytest.raises(TypeError) as excinfo:
             Path(1234)
         assert str(excinfo.value) == 'The path must be a string object'
 
-        with pytest.raises(InvalidPathError) as excinfo:
-            Path('|If SkadefÃ¶rsÃ¤kring')
-        assert str(excinfo.value) == 'Invalid path |If SkadefÃ¶rsÃ¤kring: it contains invalid characters.'
-
         Path('|If Skadeförsäkring')
         Path('|æøå')
 
         path = Path('test')
         assert path.is_relative is True
         assert repr(path) == 'test'
```

### Comparing `scrunch-0.9.6/scrunch/variables.py` & `scrunch-0.9.7/scrunch/variables.py`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/scrunch.egg-info/PKG-INFO` & `scrunch-0.9.7/scrunch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrunch
-Version: 0.9.6
+Version: 0.9.7
 Summary: Pythonic scripting library for cleaning data in Crunch
 Home-page: https://github.com/Crunch-io/scrunch
 Author: Crunch.io
 Author-email: dev@crunch.io
 License: UNKNOWN
 Description: .. image:: https://img.shields.io/pypi/v/scrunch.svg
            :target: https://pypi.org/project/scrunch
```

### Comparing `scrunch-0.9.6/scrunch.egg-info/SOURCES.txt` & `scrunch-0.9.7/scrunch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrunch-0.9.6/setup.py` & `scrunch-0.9.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         else []
     ),
     python_requires='>=2.7',
     install_requires=[
         'pycrunch>=0.4.11',
         'requests',
         'six',
-        'cr.cube',
+        'cr.cube==2.3.9',
         'importlib_metadata',
     ],
     extras_require={
         'testing': [
             # upstream
             'pytest>=4.3',
             'collective.checkdocs',
```

### Comparing `scrunch-0.9.6/tox.ini` & `scrunch-0.9.7/tox.ini`

 * *Files identical despite different names*

