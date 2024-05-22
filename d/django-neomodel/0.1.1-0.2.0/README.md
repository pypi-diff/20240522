# Comparing `tmp/django_neomodel-0.1.1.tar.gz` & `tmp/django_neomodel-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_neomodel-0.1.1.tar", last modified: Mon Aug 21 12:46:33 2023, max compression
+gzip compressed data, was "django_neomodel-0.2.0.tar", last modified: Wed May 22 12:42:11 2024, max compression
```

## Comparing `django_neomodel-0.1.1.tar` & `django_neomodel-0.2.0.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:32.994554 django_neomodel-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:32.982554 django_neomodel-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:32.986554 django_neomodel-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/.github/workflows/integration-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/Changelog
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-08-21 12:46:32.994554 django_neomodel-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/TODO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:32.986554 django_neomodel-0.1.1/django_neomodel/
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/django_neomodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/django_neomodel/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/django_neomodel/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:32.986554 django_neomodel-0.1.1/django_neomodel/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/django_neomodel/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:32.990554 django_neomodel-0.1.1/django_neomodel/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/django_neomodel/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/django_neomodel/management/commands/clear_neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/django_neomodel/management/commands/install_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:32.986554 django_neomodel-0.1.1/django_neomodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-08-21 12:46:32.000000 django_neomodel-0.1.1/django_neomodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-21 12:46:32.000000 django_neomodel-0.1.1/django_neomodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 12:46:32.000000 django_neomodel-0.1.1/django_neomodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-21 12:46:32.000000 django_neomodel-0.1.1/django_neomodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-21 12:46:32.000000 django_neomodel-0.1.1/django_neomodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:32.990554 django_neomodel-0.1.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/scripts/docker-neo4j.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-21 12:46:32.994554 django_neomodel-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/test.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:32.990554 django_neomodel-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/.env
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      512 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/docker-entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:32.994554 django_neomodel-0.1.1/tests/someapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/someapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/someapp/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:32.994554 django_neomodel-0.1.1/tests/someapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/someapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/someapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/someapp/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:32.994554 django_neomodel-0.1.1/tests/someapp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/someapp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/someapp/tests/test_atomicity.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/someapp/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/someapp/tests/test_model_form.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/someapp/tests/test_sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/someapp/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/someapp/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-21 12:46:14.000000 django_neomodel-0.1.1/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:11.758079 django_neomodel-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:11.746080 django_neomodel-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:11.750079 django_neomodel-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/.github/workflows/integration-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/Changelog
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7695 2024-05-22 12:42:11.758079 django_neomodel-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/TODO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:11.750079 django_neomodel-0.2.0/django_neomodel/
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/django_neomodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/django_neomodel/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/django_neomodel/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:11.754079 django_neomodel-0.2.0/django_neomodel/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/django_neomodel/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:11.754079 django_neomodel-0.2.0/django_neomodel/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/django_neomodel/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/django_neomodel/management/commands/clear_neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/django_neomodel/management/commands/install_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:11.758079 django_neomodel-0.2.0/django_neomodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7695 2024-05-22 12:42:11.000000 django_neomodel-0.2.0/django_neomodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-22 12:42:11.000000 django_neomodel-0.2.0/django_neomodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:42:11.000000 django_neomodel-0.2.0/django_neomodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-22 12:42:11.000000 django_neomodel-0.2.0/django_neomodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 12:42:11.000000 django_neomodel-0.2.0/django_neomodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:11.754079 django_neomodel-0.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/scripts/docker-neo4j.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:42:11.758079 django_neomodel-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)   151552 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/test.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:11.754079 django_neomodel-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/.env
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      512 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/docker-entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:11.754079 django_neomodel-0.2.0/tests/someapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/someapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/someapp/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:11.754079 django_neomodel-0.2.0/tests/someapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/someapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/someapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/someapp/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:11.758079 django_neomodel-0.2.0/tests/someapp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/someapp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/someapp/tests/test_atomicity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/someapp/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/someapp/tests/test_model_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/someapp/tests/test_sanity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/someapp/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/someapp/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-22 12:42:07.000000 django_neomodel-0.2.0/tests/urls.py
```

### Comparing `django_neomodel-0.1.1/.github/workflows/codeql-analysis.yml` & `django_neomodel-0.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `django_neomodel-0.1.1/.github/workflows/integration-tests.yml` & `django_neomodel-0.2.0/.github/workflows/integration-tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
 name: Integration tests
 
 on:
   push:
-    branches: [ "master", "rc/**" ]
+    branches: [ "rc/**" ]
   pull_request:
     branches: [ "master", "rc/**" ]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.11", "3.10", "3.9", "3.8", "3.7"]
+        python-version: ["3.12", "3.11", "3.10", "3.9", "3.8"]
         neo4j-version: ["community", "4.4-community"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
```

### Comparing `django_neomodel-0.1.1/.github/workflows/python-publish.yml` & `django_neomodel-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `django_neomodel-0.1.1/Changelog` & `django_neomodel-0.2.0/Changelog`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+Version 0.2.0 2024-05
+* Bump neomodel to 5.3.0
+* Bump Django to 4.2.8 LTS
+
 Version 0.1.1 2023-08
 * Bump neomodel to 5.1.0 - full support of Neo4j version 5.x (and 4.4 LTS)
 * Support higher versions of Django (> 2.2)
 
 Version 0.1.0 2023-04
 * Upgrade neomodel dependency to version 5.0.0
 * Adds support for all Neo4j 5.x versions, and 4.4 (LTS)
```

### Comparing `django_neomodel-0.1.1/LICENSE` & `django_neomodel-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_neomodel-0.1.1/PKG-INFO` & `django_neomodel-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,101 @@
 Metadata-Version: 2.1
 Name: django_neomodel
-Version: 0.1.1
+Version: 0.2.0
 Summary: Use Neo4j with Django!
 Author-email: Robin Edwards <robin.ge@gmail.com>
-Maintainer: Cristina Escalante
-Maintainer-email: Athanasios Anastasiou <athanastasiou@gmail.com>, Marius Conjeaud <marius.conjeaud@outlook.com>
+Maintainer-email: Marius Conjeaud <marius.conjeaud@outlook.com>
 License: MIT
 Project-URL: repository, http://github.com/robinedwards/django-neomodel
 Keywords: graph,neo4j,django,plugin,neomodel
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
+Requires-Dist: neomodel~=5.3.0
+Requires-Dist: django>=4.2.8
+Provides-Extra: dev
+Requires-Dist: pytest>=7.1; extra == "dev"
+Requires-Dist: pytest-django>=4.5.2; extra == "dev"
+Requires-Dist: pytest-cov>=4.0; extra == "dev"
 
-Django Neomodel (beta!)
-=======================
+# Django Neomodel (beta!)
 
-.. image:: https://raw.githubusercontent.com/robinedwards/neomodel/master/doc/source/_static/neomodel-300.png
-   :alt: neomodel
+![neomodel](https://raw.githubusercontent.com/neo4j-contrib/neomodel/master/doc/source/_static/neomodel-300.png)
 
-This module allows you to use the neo4j_ graph database with Django using neomodel_
+This module allows you to use the [neo4j](https://www.neo4j.org) graph database with Django using [neomodel](http://neomodel.readthedocs.org)
 
-.. _neo4j: https://www.neo4j.org
-.. _neomodel: http://neomodel.readthedocs.org
 
-Warnings
-=======================
+## Warnings
 
-* Admin functionality is very experimental. `Please see todos / issues here <https://github.com/neo4j-contrib/django-neomodel/projects/1>`_
+* Admin functionality is very experimental. [Please see todos / issues here](https://github.com/neo4j-contrib/django-neomodel/projects/1)
 
-Live Examples (add yours here)
-===============================
+## Live Examples (add yours here)
 
-* `ResoTrack <https://resotrack.herokuapp.com/>`_
+* [Syracuse](https://syracuse.1145.am>): a database of company linkages created from unstructured text. Repo at [syracuse-neo](https://github.com/alanbuxton/syracuse-neo.git)
 
-Getting started
-===============
+# Getting started
 
-Install the module::
+Install the module:
 
     $ pip install django_neomodel
 
-Add the following settings to your `settings.py`::
+Add the following settings to your `settings.py`:
 
     NEOMODEL_NEO4J_BOLT_URL = os.environ.get('NEO4J_BOLT_URL', 'bolt://neo4j:foobarbaz@localhost:7687')
 
     # Make sure django_neomodel comes before your own apps
     INSTALLED_APPS = (
         # django.contrib.auth etc
         'django_neomodel',
         'yourapp'
     )
 
-Write your first node definition in `yourapp/models.py`::
+Write your first node definition in `yourapp/models.py`:
 
     from neomodel import StructuredNode, StringProperty, DateProperty
 
     class Book(StructuredNode):
         title = StringProperty(unique_index=True)
         published = DateProperty()
 
 Create any constraints or indexes for your labels. This needs to be done after you change your node definitions
-much like `manage.py migrate`::
+much like `manage.py migrate`:
 
     $ python manage.py install_labels
 
-Now in a view `yourapp/views.py`::
+Now in a view `yourapp/views.py`:
 
     from .models import Book
 
     def get_books(request):
         return render('yourapp/books.html', request, {'books': Book.nodes.all()})
 
-In your `yourapp/admin.py`::
+In your `yourapp/admin.py`:
 
     from django_neomodel import admin as neo_admin
     from .models import Book
 
     class BookAdmin(dj_admin.ModelAdmin):
         list_display = ("title", "created")
     neo_admin.register(Book, BookAdmin)
 
 And you're ready to go. Don't forget to check the neomodel_ documentation.
 
-Model forms
-===========
+## Model forms
 
-Switch the base class from `StructuredNode` to `DjangoNode` and add a 'Meta' class::
+Switch the base class from `StructuredNode` to `DjangoNode` and add a 'Meta' class:
 
     from datetime import datetime
     from django_neomodel import DjangoNode
     from neomodel import StructuredNode, StringProperty, DateTimeProperty, UniqueIdProperty
 
     class Book(DjangoNode):
         uid = UniqueIdProperty()
@@ -110,36 +106,34 @@
                 ('Damaged', 'D'),
             ), default='Available')
         created = DateTimeProperty(default=datetime.utcnow)
 
         class Meta:
             app_label = 'library'
 
-Create a model form class for your `DjangoNode`::
+Create a model form class for your `DjangoNode`:
 
     class BookForm(ModelForm):
         class Meta:
             model = Book
             fields = ['title', 'status']
 
 This class may now be used just like any other Django form.
 
-Settings
-========
+## Settings
 The following config options are available in django settings (default values shown).
-These are mapped to neomodel.config as django is started::
+These are mapped to neomodel.config as django is started:
 
     NEOMODEL_NEO4J_BOLT_URL = 'bolt://neo4j:neo4j@localhost:7687'
     NEOMODEL_SIGNALS = True
     NEOMODEL_FORCE_TIMEZONE = False
     NEOMODEL_MAX_CONNECTION_POOL_SIZE = 50
 
-Signals
-=======
-Signals work with `DjangoNode` sub-classes::
+## Signals
+Signals work with `DjangoNode` sub-classes:
 
     from django.db.models import signals
     from django_neomodel import DjangoNode
     from neomodel import StringProperty
 
     class Book(DjangoNode):
       title = StringProperty(unique_index=True)
@@ -148,83 +142,71 @@
         pass
 
     signals.post_save.connect(your_signal_func, sender=Book)
 
 The following are supported: `pre_save`, `post_save`, `pre_delete`, `post_delete`.
 On freshly created nodes `created=True` in the `post_save` signal argument.
 
-Testing
-=======
+## Testing
 
-You can create a setup method which clears the database before executing each test::
+You can create a setup method which clears the database before executing each test:
 
     from neomodel import db, clear_neo4j_database
 
     class YourTestClass(DjangoTestCase):
         def setUp(self):
             clear_neo4j_database(db)
 
         def test_something(self):
             pass
 
-Management Commands
-===================
+## Management Commands
 
 The following django management commands have been included.
 
-install_labels
---------------
-Setup constraints and indexes on labels for your node definitions. This should be executed after any schema changes::
+### install_labels
+Setup constraints and indexes on labels for your node definitions. This should be executed after any schema changes:
 
     $ python manage.py install_labels
     Setting up labels and constraints...
 
     Found tests.someapp.models.Book
     + Creating unique constraint for title on label Book for class tests.someapp.models.Book
     Finished 1 class(es).
 
-clear_neo4j
------------
+### clear_neo4j
 Delete all nodes in your database, warning there is no confirmation!
 
-Requirements
-============
+## Requirements
 
-- Python 3.7+
+- Python 3.8+
 - neo4j 5.x, 4.4 (LTS)
 
-.. image:: https://badges.gitter.im/Join%20Chat.svg
-   :alt: Join the chat at https://gitter.im/robinedwards/neomodel
-   :target: https://gitter.im/robinedwards/neomodel?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-
-Docker Example
-===================
-
+## Docker Example
 
 Using Docker Compose.
 
-Commands to setup Docker Container docker-entrypoint.sh::
+Commands to setup Docker Container docker-entrypoint.sh:
 
     # Go to tests
     $ cd tests/
     # Docker Command (Make sure Docker is running and up to date)
     $ docker-compose up
     # login in admin with username=admin password=1234
 
 Go to http://localhost:7474/browser/
 
 Go to http://localhost:8000/admin/
 
 
-Running Tests
-===================
+## Running Tests
 
 Setup Neo4j Desktop with a local database with password 'foobarbaz' and version 5.x or 4.4.x (Neo4j LTS version).
 
-Commands to run tests::
+Commands to run tests:
 
     # create local venv and install dependencies.
     $ pip install -e '.[dev]'; export DJANGO_SETTINGS_MODULE=tests.settings;
     $ tests/manage.py install_labels
     $ tests/manage.py migrate
     $ pytest
```

### Comparing `django_neomodel-0.1.1/README.rst` & `django_neomodel-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,81 +1,73 @@
-Django Neomodel (beta!)
-=======================
+# Django Neomodel (beta!)
 
-.. image:: https://raw.githubusercontent.com/robinedwards/neomodel/master/doc/source/_static/neomodel-300.png
-   :alt: neomodel
+![neomodel](https://raw.githubusercontent.com/neo4j-contrib/neomodel/master/doc/source/_static/neomodel-300.png)
 
-This module allows you to use the neo4j_ graph database with Django using neomodel_
+This module allows you to use the [neo4j](https://www.neo4j.org) graph database with Django using [neomodel](http://neomodel.readthedocs.org)
 
-.. _neo4j: https://www.neo4j.org
-.. _neomodel: http://neomodel.readthedocs.org
 
-Warnings
-=======================
+## Warnings
 
-* Admin functionality is very experimental. `Please see todos / issues here <https://github.com/neo4j-contrib/django-neomodel/projects/1>`_
+* Admin functionality is very experimental. [Please see todos / issues here](https://github.com/neo4j-contrib/django-neomodel/projects/1)
 
-Live Examples (add yours here)
-===============================
+## Live Examples (add yours here)
 
-* `ResoTrack <https://resotrack.herokuapp.com/>`_
+* [Syracuse](https://syracuse.1145.am>): a database of company linkages created from unstructured text. Repo at [syracuse-neo](https://github.com/alanbuxton/syracuse-neo.git)
 
-Getting started
-===============
+# Getting started
 
-Install the module::
+Install the module:
 
     $ pip install django_neomodel
 
-Add the following settings to your `settings.py`::
+Add the following settings to your `settings.py`:
 
     NEOMODEL_NEO4J_BOLT_URL = os.environ.get('NEO4J_BOLT_URL', 'bolt://neo4j:foobarbaz@localhost:7687')
 
     # Make sure django_neomodel comes before your own apps
     INSTALLED_APPS = (
         # django.contrib.auth etc
         'django_neomodel',
         'yourapp'
     )
 
-Write your first node definition in `yourapp/models.py`::
+Write your first node definition in `yourapp/models.py`:
 
     from neomodel import StructuredNode, StringProperty, DateProperty
 
     class Book(StructuredNode):
         title = StringProperty(unique_index=True)
         published = DateProperty()
 
 Create any constraints or indexes for your labels. This needs to be done after you change your node definitions
-much like `manage.py migrate`::
+much like `manage.py migrate`:
 
     $ python manage.py install_labels
 
-Now in a view `yourapp/views.py`::
+Now in a view `yourapp/views.py`:
 
     from .models import Book
 
     def get_books(request):
         return render('yourapp/books.html', request, {'books': Book.nodes.all()})
 
-In your `yourapp/admin.py`::
+In your `yourapp/admin.py`:
 
     from django_neomodel import admin as neo_admin
     from .models import Book
 
     class BookAdmin(dj_admin.ModelAdmin):
         list_display = ("title", "created")
     neo_admin.register(Book, BookAdmin)
 
 And you're ready to go. Don't forget to check the neomodel_ documentation.
 
-Model forms
-===========
+## Model forms
 
-Switch the base class from `StructuredNode` to `DjangoNode` and add a 'Meta' class::
+Switch the base class from `StructuredNode` to `DjangoNode` and add a 'Meta' class:
 
     from datetime import datetime
     from django_neomodel import DjangoNode
     from neomodel import StructuredNode, StringProperty, DateTimeProperty, UniqueIdProperty
 
     class Book(DjangoNode):
         uid = UniqueIdProperty()
@@ -86,36 +78,34 @@
                 ('Damaged', 'D'),
             ), default='Available')
         created = DateTimeProperty(default=datetime.utcnow)
 
         class Meta:
             app_label = 'library'
 
-Create a model form class for your `DjangoNode`::
+Create a model form class for your `DjangoNode`:
 
     class BookForm(ModelForm):
         class Meta:
             model = Book
             fields = ['title', 'status']
 
 This class may now be used just like any other Django form.
 
-Settings
-========
+## Settings
 The following config options are available in django settings (default values shown).
-These are mapped to neomodel.config as django is started::
+These are mapped to neomodel.config as django is started:
 
     NEOMODEL_NEO4J_BOLT_URL = 'bolt://neo4j:neo4j@localhost:7687'
     NEOMODEL_SIGNALS = True
     NEOMODEL_FORCE_TIMEZONE = False
     NEOMODEL_MAX_CONNECTION_POOL_SIZE = 50
 
-Signals
-=======
-Signals work with `DjangoNode` sub-classes::
+## Signals
+Signals work with `DjangoNode` sub-classes:
 
     from django.db.models import signals
     from django_neomodel import DjangoNode
     from neomodel import StringProperty
 
     class Book(DjangoNode):
       title = StringProperty(unique_index=True)
@@ -124,83 +114,71 @@
         pass
 
     signals.post_save.connect(your_signal_func, sender=Book)
 
 The following are supported: `pre_save`, `post_save`, `pre_delete`, `post_delete`.
 On freshly created nodes `created=True` in the `post_save` signal argument.
 
-Testing
-=======
+## Testing
 
-You can create a setup method which clears the database before executing each test::
+You can create a setup method which clears the database before executing each test:
 
     from neomodel import db, clear_neo4j_database
 
     class YourTestClass(DjangoTestCase):
         def setUp(self):
             clear_neo4j_database(db)
 
         def test_something(self):
             pass
 
-Management Commands
-===================
+## Management Commands
 
 The following django management commands have been included.
 
-install_labels
---------------
-Setup constraints and indexes on labels for your node definitions. This should be executed after any schema changes::
+### install_labels
+Setup constraints and indexes on labels for your node definitions. This should be executed after any schema changes:
 
     $ python manage.py install_labels
     Setting up labels and constraints...
 
     Found tests.someapp.models.Book
     + Creating unique constraint for title on label Book for class tests.someapp.models.Book
     Finished 1 class(es).
 
-clear_neo4j
------------
+### clear_neo4j
 Delete all nodes in your database, warning there is no confirmation!
 
-Requirements
-============
+## Requirements
 
-- Python 3.7+
+- Python 3.8+
 - neo4j 5.x, 4.4 (LTS)
 
-.. image:: https://badges.gitter.im/Join%20Chat.svg
-   :alt: Join the chat at https://gitter.im/robinedwards/neomodel
-   :target: https://gitter.im/robinedwards/neomodel?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-
-Docker Example
-===================
-
+## Docker Example
 
 Using Docker Compose.
 
-Commands to setup Docker Container docker-entrypoint.sh::
+Commands to setup Docker Container docker-entrypoint.sh:
 
     # Go to tests
     $ cd tests/
     # Docker Command (Make sure Docker is running and up to date)
     $ docker-compose up
     # login in admin with username=admin password=1234
 
 Go to http://localhost:7474/browser/
 
 Go to http://localhost:8000/admin/
 
 
-Running Tests
-===================
+## Running Tests
 
 Setup Neo4j Desktop with a local database with password 'foobarbaz' and version 5.x or 4.4.x (Neo4j LTS version).
 
-Commands to run tests::
+Commands to run tests:
 
     # create local venv and install dependencies.
     $ pip install -e '.[dev]'; export DJANGO_SETTINGS_MODULE=tests.settings;
     $ tests/manage.py install_labels
     $ tests/manage.py migrate
     $ pytest
```

### Comparing `django_neomodel-0.1.1/django_neomodel/__init__.py` & `django_neomodel-0.2.0/django_neomodel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from django.db.models.fields import BLANK_CHOICE_DASH
 from django.conf import settings
 from django.forms import fields as form_fields
 from django.db.models.options import Options
 from django.core.exceptions import ValidationError
 
 from neomodel import RequiredProperty, DeflateError, StructuredNode, UniqueIdProperty
-from neomodel.core import NodeMeta
-from neomodel.match import NodeSet
+from neomodel.sync_.core import NodeMeta
+from neomodel.sync_.match import NodeSet
 
 
 __author__ = "Robin Edwards"
 __email__ = "robin.ge@gmail.com"
 __license__ = "MIT"
 __package__ = "django_neomodel"
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 
 default_app_config = "django_neomodel.apps.NeomodelConfig"
 
 
 def classproperty(f):
     class cpf(object):
```

### Comparing `django_neomodel-0.1.1/django_neomodel.egg-info/PKG-INFO` & `django_neomodel-0.2.0/django_neomodel.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,105 +1,101 @@
 Metadata-Version: 2.1
-Name: django-neomodel
-Version: 0.1.1
+Name: django_neomodel
+Version: 0.2.0
 Summary: Use Neo4j with Django!
 Author-email: Robin Edwards <robin.ge@gmail.com>
-Maintainer: Cristina Escalante
-Maintainer-email: Athanasios Anastasiou <athanastasiou@gmail.com>, Marius Conjeaud <marius.conjeaud@outlook.com>
+Maintainer-email: Marius Conjeaud <marius.conjeaud@outlook.com>
 License: MIT
 Project-URL: repository, http://github.com/robinedwards/django-neomodel
 Keywords: graph,neo4j,django,plugin,neomodel
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
+Requires-Dist: neomodel~=5.3.0
+Requires-Dist: django>=4.2.8
+Provides-Extra: dev
+Requires-Dist: pytest>=7.1; extra == "dev"
+Requires-Dist: pytest-django>=4.5.2; extra == "dev"
+Requires-Dist: pytest-cov>=4.0; extra == "dev"
 
-Django Neomodel (beta!)
-=======================
+# Django Neomodel (beta!)
 
-.. image:: https://raw.githubusercontent.com/robinedwards/neomodel/master/doc/source/_static/neomodel-300.png
-   :alt: neomodel
+![neomodel](https://raw.githubusercontent.com/neo4j-contrib/neomodel/master/doc/source/_static/neomodel-300.png)
 
-This module allows you to use the neo4j_ graph database with Django using neomodel_
+This module allows you to use the [neo4j](https://www.neo4j.org) graph database with Django using [neomodel](http://neomodel.readthedocs.org)
 
-.. _neo4j: https://www.neo4j.org
-.. _neomodel: http://neomodel.readthedocs.org
 
-Warnings
-=======================
+## Warnings
 
-* Admin functionality is very experimental. `Please see todos / issues here <https://github.com/neo4j-contrib/django-neomodel/projects/1>`_
+* Admin functionality is very experimental. [Please see todos / issues here](https://github.com/neo4j-contrib/django-neomodel/projects/1)
 
-Live Examples (add yours here)
-===============================
+## Live Examples (add yours here)
 
-* `ResoTrack <https://resotrack.herokuapp.com/>`_
+* [Syracuse](https://syracuse.1145.am>): a database of company linkages created from unstructured text. Repo at [syracuse-neo](https://github.com/alanbuxton/syracuse-neo.git)
 
-Getting started
-===============
+# Getting started
 
-Install the module::
+Install the module:
 
     $ pip install django_neomodel
 
-Add the following settings to your `settings.py`::
+Add the following settings to your `settings.py`:
 
     NEOMODEL_NEO4J_BOLT_URL = os.environ.get('NEO4J_BOLT_URL', 'bolt://neo4j:foobarbaz@localhost:7687')
 
     # Make sure django_neomodel comes before your own apps
     INSTALLED_APPS = (
         # django.contrib.auth etc
         'django_neomodel',
         'yourapp'
     )
 
-Write your first node definition in `yourapp/models.py`::
+Write your first node definition in `yourapp/models.py`:
 
     from neomodel import StructuredNode, StringProperty, DateProperty
 
     class Book(StructuredNode):
         title = StringProperty(unique_index=True)
         published = DateProperty()
 
 Create any constraints or indexes for your labels. This needs to be done after you change your node definitions
-much like `manage.py migrate`::
+much like `manage.py migrate`:
 
     $ python manage.py install_labels
 
-Now in a view `yourapp/views.py`::
+Now in a view `yourapp/views.py`:
 
     from .models import Book
 
     def get_books(request):
         return render('yourapp/books.html', request, {'books': Book.nodes.all()})
 
-In your `yourapp/admin.py`::
+In your `yourapp/admin.py`:
 
     from django_neomodel import admin as neo_admin
     from .models import Book
 
     class BookAdmin(dj_admin.ModelAdmin):
         list_display = ("title", "created")
     neo_admin.register(Book, BookAdmin)
 
 And you're ready to go. Don't forget to check the neomodel_ documentation.
 
-Model forms
-===========
+## Model forms
 
-Switch the base class from `StructuredNode` to `DjangoNode` and add a 'Meta' class::
+Switch the base class from `StructuredNode` to `DjangoNode` and add a 'Meta' class:
 
     from datetime import datetime
     from django_neomodel import DjangoNode
     from neomodel import StructuredNode, StringProperty, DateTimeProperty, UniqueIdProperty
 
     class Book(DjangoNode):
         uid = UniqueIdProperty()
@@ -110,36 +106,34 @@
                 ('Damaged', 'D'),
             ), default='Available')
         created = DateTimeProperty(default=datetime.utcnow)
 
         class Meta:
             app_label = 'library'
 
-Create a model form class for your `DjangoNode`::
+Create a model form class for your `DjangoNode`:
 
     class BookForm(ModelForm):
         class Meta:
             model = Book
             fields = ['title', 'status']
 
 This class may now be used just like any other Django form.
 
-Settings
-========
+## Settings
 The following config options are available in django settings (default values shown).
-These are mapped to neomodel.config as django is started::
+These are mapped to neomodel.config as django is started:
 
     NEOMODEL_NEO4J_BOLT_URL = 'bolt://neo4j:neo4j@localhost:7687'
     NEOMODEL_SIGNALS = True
     NEOMODEL_FORCE_TIMEZONE = False
     NEOMODEL_MAX_CONNECTION_POOL_SIZE = 50
 
-Signals
-=======
-Signals work with `DjangoNode` sub-classes::
+## Signals
+Signals work with `DjangoNode` sub-classes:
 
     from django.db.models import signals
     from django_neomodel import DjangoNode
     from neomodel import StringProperty
 
     class Book(DjangoNode):
       title = StringProperty(unique_index=True)
@@ -148,83 +142,71 @@
         pass
 
     signals.post_save.connect(your_signal_func, sender=Book)
 
 The following are supported: `pre_save`, `post_save`, `pre_delete`, `post_delete`.
 On freshly created nodes `created=True` in the `post_save` signal argument.
 
-Testing
-=======
+## Testing
 
-You can create a setup method which clears the database before executing each test::
+You can create a setup method which clears the database before executing each test:
 
     from neomodel import db, clear_neo4j_database
 
     class YourTestClass(DjangoTestCase):
         def setUp(self):
             clear_neo4j_database(db)
 
         def test_something(self):
             pass
 
-Management Commands
-===================
+## Management Commands
 
 The following django management commands have been included.
 
-install_labels
---------------
-Setup constraints and indexes on labels for your node definitions. This should be executed after any schema changes::
+### install_labels
+Setup constraints and indexes on labels for your node definitions. This should be executed after any schema changes:
 
     $ python manage.py install_labels
     Setting up labels and constraints...
 
     Found tests.someapp.models.Book
     + Creating unique constraint for title on label Book for class tests.someapp.models.Book
     Finished 1 class(es).
 
-clear_neo4j
------------
+### clear_neo4j
 Delete all nodes in your database, warning there is no confirmation!
 
-Requirements
-============
+## Requirements
 
-- Python 3.7+
+- Python 3.8+
 - neo4j 5.x, 4.4 (LTS)
 
-.. image:: https://badges.gitter.im/Join%20Chat.svg
-   :alt: Join the chat at https://gitter.im/robinedwards/neomodel
-   :target: https://gitter.im/robinedwards/neomodel?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-
-Docker Example
-===================
-
+## Docker Example
 
 Using Docker Compose.
 
-Commands to setup Docker Container docker-entrypoint.sh::
+Commands to setup Docker Container docker-entrypoint.sh:
 
     # Go to tests
     $ cd tests/
     # Docker Command (Make sure Docker is running and up to date)
     $ docker-compose up
     # login in admin with username=admin password=1234
 
 Go to http://localhost:7474/browser/
 
 Go to http://localhost:8000/admin/
 
 
-Running Tests
-===================
+## Running Tests
 
 Setup Neo4j Desktop with a local database with password 'foobarbaz' and version 5.x or 4.4.x (Neo4j LTS version).
 
-Commands to run tests::
+Commands to run tests:
 
     # create local venv and install dependencies.
     $ pip install -e '.[dev]'; export DJANGO_SETTINGS_MODULE=tests.settings;
     $ tests/manage.py install_labels
     $ tests/manage.py migrate
     $ pytest
```

### Comparing `django_neomodel-0.1.1/django_neomodel.egg-info/SOURCES.txt` & `django_neomodel-0.2.0/django_neomodel.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 .gitignore
 AUTHORS.txt
 Changelog
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 TODO
 pyproject.toml
+requirements-dev.txt
+requirements.txt
 test.db
 .github/workflows/codeql-analysis.yml
 .github/workflows/integration-tests.yml
 .github/workflows/python-publish.yml
 django_neomodel/__init__.py
 django_neomodel/admin.py
 django_neomodel/apps.py
```

### Comparing `django_neomodel-0.1.1/pyproject.toml` & `django_neomodel-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,49 +5,43 @@
 [tool.setuptools_scm]
 
 [tool.setuptools.packages.find]
 where = ["./"]
 
 [project]
 name = "django_neomodel"
-authors = [
-    {name = "Robin Edwards", email = "robin.ge@gmail.com"},
-]
-maintainers = [
-    {name = "Athanasios Anastasiou", email = "athanastasiou@gmail.com"},
-    {name = "Cristina Escalante"},
-    {name = "Marius Conjeaud", email = "marius.conjeaud@outlook.com"},
-]
+authors = [{name = "Robin Edwards", email = "robin.ge@gmail.com"}]
+maintainers = [{name = "Marius Conjeaud", email = "marius.conjeaud@outlook.com"}]
 description = "Use Neo4j with Django!"
-readme = "README.rst"
-requires-python = ">=3.7"
+readme = "README.md"
+requires-python = ">=3.8"
 keywords = ["graph", "neo4j", "django", "plugin", "neomodel"]
-license = {text = "MIT"}
+license = { text = "MIT" }
 classifiers = [
     "Development Status :: 4 - Beta",
     'Intended Audience :: Developers',
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     'Topic :: Software Development :: Libraries :: Python Modules',
     "Programming Language :: Python :: 3",
     "Topic :: Database",
 ]
 dependencies = [
-    "neomodel~=5.1.0",
-    'django>=2.2'
+    "neomodel~=5.3.0",
+    'django>=4.2.8'
 ]
-version='0.1.1'
+version='0.2.0'
 
 [project.urls]
 repository = "http://github.com/robinedwards/django-neomodel"
 
 [project.optional-dependencies]
 dev = [
     "pytest>=7.1",
-    "pytest-django>=3.10.0",
+    "pytest-django>=4.5.2",
     "pytest-cov>=4.0",
 ]
 
 [tool.pytest.ini_options]
 addopts = "--ds=tests.settings"
 testpaths = "tests"
```

### Comparing `django_neomodel-0.1.1/test.db` & `django_neomodel-0.2.0/test.db`

 * *Files 3% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -17,14 +17,15 @@
 INSERT INTO django_migrations VALUES(14,'auth','0009_alter_user_last_name_max_length','2023-03-23 17:01:35.550174');
 INSERT INTO django_migrations VALUES(15,'auth','0010_alter_group_name_max_length','2023-03-23 17:01:35.557084');
 INSERT INTO django_migrations VALUES(16,'auth','0011_update_proxy_permissions','2023-03-23 17:01:35.562829');
 INSERT INTO django_migrations VALUES(17,'sessions','0001_initial','2023-03-23 17:01:35.565378');
 INSERT INTO django_migrations VALUES(18,'sites','0001_initial','2023-03-23 17:01:35.568064');
 INSERT INTO django_migrations VALUES(19,'sites','0002_alter_domain_unique','2023-03-23 17:01:35.572162');
 INSERT INTO django_migrations VALUES(20,'someapp','0001_initial','2023-03-23 17:01:35.574710');
+INSERT INTO django_migrations VALUES(21,'auth','0012_alter_user_first_name_max_length','2024-05-21 16:00:36.430125');
 CREATE TABLE IF NOT EXISTS "auth_group_permissions" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "group_id" integer NOT NULL REFERENCES "auth_group" ("id") DEFERRABLE INITIALLY DEFERRED, "permission_id" integer NOT NULL REFERENCES "auth_permission" ("id") DEFERRABLE INITIALLY DEFERRED);
 CREATE TABLE IF NOT EXISTS "auth_user_groups" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "user_id" integer NOT NULL REFERENCES "auth_user" ("id") DEFERRABLE INITIALLY DEFERRED, "group_id" integer NOT NULL REFERENCES "auth_group" ("id") DEFERRABLE INITIALLY DEFERRED);
 CREATE TABLE IF NOT EXISTS "auth_user_user_permissions" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "user_id" integer NOT NULL REFERENCES "auth_user" ("id") DEFERRABLE INITIALLY DEFERRED, "permission_id" integer NOT NULL REFERENCES "auth_permission" ("id") DEFERRABLE INITIALLY DEFERRED);
 CREATE TABLE IF NOT EXISTS "django_admin_log" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "action_time" datetime NOT NULL, "object_id" text NULL, "object_repr" varchar(200) NOT NULL, "change_message" text NOT NULL, "content_type_id" integer NULL REFERENCES "django_content_type" ("id") DEFERRABLE INITIALLY DEFERRED, "user_id" integer NOT NULL REFERENCES "auth_user" ("id") DEFERRABLE INITIALLY DEFERRED, "action_flag" smallint unsigned NOT NULL CHECK ("action_flag" >= 0));
 CREATE TABLE IF NOT EXISTS "django_content_type" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "app_label" varchar(100) NOT NULL, "model" varchar(100) NOT NULL);
 INSERT INTO django_content_type VALUES(1,'admin','logentry');
 INSERT INTO django_content_type VALUES(2,'auth','permission');
@@ -63,28 +64,28 @@
 INSERT INTO auth_permission VALUES(26,7,'change_site','Can change site');
 INSERT INTO auth_permission VALUES(27,7,'delete_site','Can delete site');
 INSERT INTO auth_permission VALUES(28,7,'view_site','Can view site');
 INSERT INTO auth_permission VALUES(29,8,'add_library','Can add library');
 INSERT INTO auth_permission VALUES(30,8,'change_library','Can change library');
 INSERT INTO auth_permission VALUES(31,8,'delete_library','Can delete library');
 INSERT INTO auth_permission VALUES(32,8,'view_library','Can view library');
-CREATE TABLE IF NOT EXISTS "auth_user" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "password" varchar(128) NOT NULL, "last_login" datetime NULL, "is_superuser" bool NOT NULL, "username" varchar(150) NOT NULL UNIQUE, "first_name" varchar(30) NOT NULL, "email" varchar(254) NOT NULL, "is_staff" bool NOT NULL, "is_active" bool NOT NULL, "date_joined" datetime NOT NULL, "last_name" varchar(150) NOT NULL);
 CREATE TABLE IF NOT EXISTS "auth_group" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(150) NOT NULL UNIQUE);
 CREATE TABLE IF NOT EXISTS "django_session" ("session_key" varchar(40) NOT NULL PRIMARY KEY, "session_data" text NOT NULL, "expire_date" datetime NOT NULL);
 CREATE TABLE IF NOT EXISTS "django_site" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(50) NOT NULL, "domain" varchar(100) NOT NULL UNIQUE);
 INSERT INTO django_site VALUES(300,'example.com','example.com');
 CREATE TABLE IF NOT EXISTS "someapp_library" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(10) NOT NULL);
+CREATE TABLE IF NOT EXISTS "auth_user" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "password" varchar(128) NOT NULL, "last_login" datetime NULL, "is_superuser" bool NOT NULL, "username" varchar(150) NOT NULL UNIQUE, "last_name" varchar(150) NOT NULL, "email" varchar(254) NOT NULL, "is_staff" bool NOT NULL, "is_active" bool NOT NULL, "date_joined" datetime NOT NULL, "first_name" varchar(150) NOT NULL);
 DELETE FROM sqlite_sequence;
-INSERT INTO sqlite_sequence VALUES('django_migrations',20);
+INSERT INTO sqlite_sequence VALUES('django_migrations',21);
 INSERT INTO sqlite_sequence VALUES('django_admin_log',0);
 INSERT INTO sqlite_sequence VALUES('django_content_type',8);
 INSERT INTO sqlite_sequence VALUES('auth_permission',32);
-INSERT INTO sqlite_sequence VALUES('auth_user',0);
 INSERT INTO sqlite_sequence VALUES('auth_group',0);
 INSERT INTO sqlite_sequence VALUES('django_site',300);
+INSERT INTO sqlite_sequence VALUES('auth_user',0);
 CREATE UNIQUE INDEX "auth_group_permissions_group_id_permission_id_0cd325b0_uniq" ON "auth_group_permissions" ("group_id", "permission_id");
 CREATE INDEX "auth_group_permissions_group_id_b120cbf9" ON "auth_group_permissions" ("group_id");
 CREATE INDEX "auth_group_permissions_permission_id_84c5c92e" ON "auth_group_permissions" ("permission_id");
 CREATE UNIQUE INDEX "auth_user_groups_user_id_group_id_94350c0c_uniq" ON "auth_user_groups" ("user_id", "group_id");
 CREATE INDEX "auth_user_groups_user_id_6a12ed8b" ON "auth_user_groups" ("user_id");
 CREATE INDEX "auth_user_groups_group_id_97559544" ON "auth_user_groups" ("group_id");
 CREATE UNIQUE INDEX "auth_user_user_permissions_user_id_permission_id_14a6b632_uniq" ON "auth_user_user_permissions" ("user_id", "permission_id");
```

### Comparing `django_neomodel-0.1.1/tests/docker-compose.yml` & `django_neomodel-0.2.0/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `django_neomodel-0.1.1/tests/docker-entrypoint.sh` & `django_neomodel-0.2.0/tests/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `django_neomodel-0.1.1/tests/settings.py` & `django_neomodel-0.2.0/tests/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,71 +5,72 @@
 here = os.path.abspath(os.path.dirname(__file__))
 sys.path.insert(0, here)
 sys.path.insert(0, os.path.join(here, os.pardir))
 SITE_ID = 300
 
 DEBUG = True
 
-ROOT_URLCONF = 'tests.urls'
-SECRET_KEY = 'skskqlqlaskdsd'
+ROOT_URLCONF = "tests.urls"
+SECRET_KEY = "skskqlqlaskdsd"
 
 AUTOCOMMIT = True
 
 
 DATABASES = {
-    'default': {
-        'NAME': 'test.db',
-        'ENGINE': 'django.db.backends.sqlite3',
-        'USER': '',
-        'PASSWORD': '',
-        'PORT': '',
+    "default": {
+        "NAME": "test.db",
+        "ENGINE": "django.db.backends.sqlite3",
+        "USER": "",
+        "PASSWORD": "",
+        "PORT": "",
     },
 }
 
-NEOMODEL_NEO4J_BOLT_URL = os.environ.get('NEO4J_BOLT_URL', 'bolt://neo4j:foobarbaz@localhost:7687')
+NEOMODEL_NEO4J_BOLT_URL = os.environ.get(
+    "NEO4J_BOLT_URL", "bolt://neo4j:foobarbaz@localhost:7687"
+)
 NEOMODEL_SIGNALS = True
 NEOMODEL_FORCE_TIMEZONE = False
 NEOMODEL_MAX_CONNECTION_POOL_SIZE = 50
 
 TEMPLATES = [
     {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'APP_DIRS': True,
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "APP_DIRS": True,
         "OPTIONS": {
             "context_processors": [
                 "django.template.context_processors.debug",
                 "django.contrib.auth.context_processors.auth",
                 "django.template.context_processors.request",
                 "django.contrib.messages.context_processors.messages",
             ]
         },
     },
 ]
 
 INSTALLED_APPS = [
     # Django
-    'django.contrib.admin',
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.messages',
-    'django.contrib.sites',
-    'django.contrib.staticfiles',
-
+    "django.contrib.admin",
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.messages",
+    "django.contrib.sites",
+    "django.contrib.staticfiles",
     # Third party
-    'django_neomodel',
-
+    "django_neomodel",
     # Test
-    'tests.someapp',
+    "tests.someapp",
 ]
 
 USE_TZ = True
-TIME_ZONE = 'UTC'
+TIME_ZONE = "UTC"
 MIDDLEWARE = [
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
 ]
 
 STATIC_ROOT = "./static/"
-STATIC_URL = '/static/'
+STATIC_URL = "/static/"
 
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
```

### Comparing `django_neomodel-0.1.1/tests/someapp/models.py` & `django_neomodel-0.2.0/tests/someapp/models.py`

 * *Files identical despite different names*

### Comparing `django_neomodel-0.1.1/tests/someapp/tests/test_atomicity.py` & `django_neomodel-0.2.0/tests/someapp/tests/test_atomicity.py`

 * *Files identical despite different names*

### Comparing `django_neomodel-0.1.1/tests/someapp/tests/test_commands.py` & `django_neomodel-0.2.0/tests/someapp/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_neomodel-0.1.1/tests/someapp/tests/test_model_form.py` & `django_neomodel-0.2.0/tests/someapp/tests/test_model_form.py`

 * *Files identical despite different names*

### Comparing `django_neomodel-0.1.1/tests/someapp/tests/test_signals.py` & `django_neomodel-0.2.0/tests/someapp/tests/test_signals.py`

 * *Files identical despite different names*

