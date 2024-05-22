# Comparing `tmp/qbraid_core-0.1.8.tar.gz` & `tmp/qbraid_core-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid_core-0.1.8.tar", last modified: Wed May 22 18:25:55 2024, max compression
+gzip compressed data, was "qbraid_core-0.1.9.tar", last modified: Wed May 22 19:53:24 2024, max compression
```

## Comparing `qbraid_core-0.1.8.tar` & `qbraid_core-0.1.9.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.750844 qbraid_core-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.730844 qbraid_core-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.730844 qbraid_core-0.1.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.730844 qbraid_core-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/.github/workflows/pre-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-05-22 18:25:55.750844 qbraid_core-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.730844 qbraid_core-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.730844 qbraid_core-0.1.8/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.730844 qbraid_core-0.1.8/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.734844 qbraid_core-0.1.8/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/_static/css/s4defs-roles.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.734844 qbraid_core-0.1.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/api/qbraid_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/api/qbraid_core.services.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/api/qbraid_core.system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.734844 qbraid_core-0.1.8/qbraid_core/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-22 18:25:55.000000 qbraid_core-0.1.8/qbraid_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.738844 qbraid_core-0.1.8/qbraid_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.738844 qbraid_core-0.1.8/qbraid_core/services/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/admin/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.738844 qbraid_core-0.1.8/qbraid_core/services/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/environments/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/environments/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/environments/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/environments/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/environments/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/environments/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.738844 qbraid_core-0.1.8/qbraid_core/services/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/quantum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/quantum/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/quantum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/quantum/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/quantum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/quantum/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/quantum/proxy_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/services/quantum/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.742844 qbraid_core-0.1.8/qbraid_core/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/system/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/system/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.742844 qbraid_core-0.1.8/qbraid_core/system/magic/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/system/magic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/system/magic/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/system/magic/qbraid_magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/system/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/system/threader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8742 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/qbraid_core/system/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.746844 qbraid_core-0.1.8/qbraid_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-05-22 18:25:55.000000 qbraid_core-0.1.8/qbraid_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-22 18:25:55.000000 qbraid_core-0.1.8/qbraid_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:25:55.000000 qbraid_core-0.1.8/qbraid_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-22 18:25:55.000000 qbraid_core-0.1.8/qbraid_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 18:25:55.000000 qbraid_core-0.1.8/qbraid_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:25:55.750844 qbraid_core-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.742844 qbraid_core-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.742844 qbraid_core-0.1.8/tests/environments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/environments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.742844 qbraid_core-0.1.8/tests/environments/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/environments/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/environments/fixtures/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/environments/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/environments/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/environments/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/environments/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/environments/test_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.742844 qbraid_core-0.1.8/tests/quantum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.746844 qbraid_core-0.1.8/tests/quantum/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/quantum/resources/qir_program.bc
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/quantum/resources/qir_runner_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/quantum/test_aws_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/quantum/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/quantum/test_qir_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.746844 qbraid_core-0.1.8/tests/system/
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/system/test_executables.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/system/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/system/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/system/test_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.746844 qbraid_core-0.1.8/tests/top_level/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/top_level/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/top_level/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/top_level/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/top_level/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/top_level/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/top_level/test_lazy_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tests/top_level/test_sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:25:55.746844 qbraid_core-0.1.8/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2584 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tools/create_dev_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1402 2024-05-22 18:25:51.000000 qbraid_core-0.1.8/tools/stamp_pre_release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.702890 qbraid_core-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.682890 qbraid_core-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.682890 qbraid_core-0.1.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.686890 qbraid_core-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/.github/workflows/pre-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-05-22 19:53:24.702890 qbraid_core-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.686890 qbraid_core-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.686890 qbraid_core-0.1.9/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.686890 qbraid_core-0.1.9/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.686890 qbraid_core-0.1.9/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/_static/css/s4defs-roles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.686890 qbraid_core-0.1.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/api/qbraid_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/api/qbraid_core.services.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/api/qbraid_core.system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.690890 qbraid_core-0.1.9/qbraid_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-22 19:53:24.000000 qbraid_core-0.1.9/qbraid_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.690890 qbraid_core-0.1.9/qbraid_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.690890 qbraid_core-0.1.9/qbraid_core/services/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/admin/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.694890 qbraid_core-0.1.9/qbraid_core/services/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/environments/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/environments/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/environments/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/environments/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/environments/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/environments/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.694890 qbraid_core-0.1.9/qbraid_core/services/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/quantum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/quantum/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/quantum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/quantum/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/quantum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/quantum/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/quantum/proxy_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/services/quantum/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13148 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.694890 qbraid_core-0.1.9/qbraid_core/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/system/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/system/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.694890 qbraid_core-0.1.9/qbraid_core/system/magic/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/system/magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/system/magic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/system/magic/qbraid_magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/system/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/system/threader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8742 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/qbraid_core/system/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.702890 qbraid_core-0.1.9/qbraid_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-05-22 19:53:24.000000 qbraid_core-0.1.9/qbraid_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-22 19:53:24.000000 qbraid_core-0.1.9/qbraid_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:53:24.000000 qbraid_core-0.1.9/qbraid_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-22 19:53:24.000000 qbraid_core-0.1.9/qbraid_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 19:53:24.000000 qbraid_core-0.1.9/qbraid_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 19:53:24.702890 qbraid_core-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.698890 qbraid_core-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.698890 qbraid_core-0.1.9/tests/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/environments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.698890 qbraid_core-0.1.9/tests/environments/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/environments/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/environments/fixtures/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/environments/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/environments/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/environments/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/environments/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/environments/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.698890 qbraid_core-0.1.9/tests/quantum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.698890 qbraid_core-0.1.9/tests/quantum/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/quantum/resources/qir_program.bc
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/quantum/resources/qir_runner_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/quantum/test_aws_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/quantum/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/quantum/test_qir_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.702890 qbraid_core-0.1.9/tests/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/system/test_executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/system/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/system/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/system/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.702890 qbraid_core-0.1.9/tests/top_level/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/top_level/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/top_level/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/top_level/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/top_level/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/top_level/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/top_level/test_lazy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tests/top_level/test_sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:24.702890 qbraid_core-0.1.9/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2584 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tools/create_dev_build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1402 2024-05-22 19:53:20.000000 qbraid_core-0.1.9/tools/stamp_pre_release.py
```

### Comparing `qbraid_core-0.1.8/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid_core-0.1.9/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid_core-0.1.9/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/.github/workflows/docs.yml` & `qbraid_core-0.1.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/.github/workflows/format.yml` & `qbraid_core-0.1.9/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/.github/workflows/main.yml` & `qbraid_core-0.1.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/.github/workflows/pre-release.yml` & `qbraid_core-0.1.9/.github/workflows/pre-release.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/.github/workflows/publish.yml` & `qbraid_core-0.1.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/.gitignore` & `qbraid_core-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/LICENSE` & `qbraid_core-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/PKG-INFO` & `qbraid_core-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author: qBraid Development Team
 Author-email: contact@qbraid.com
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
```

### Comparing `qbraid_core-0.1.8/README.md` & `qbraid_core-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/docs/Makefile` & `qbraid_core-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/docs/_static/cards/jupyter.png` & `qbraid_core-0.1.9/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/docs/_static/cards/python.png` & `qbraid_core-0.1.9/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/docs/_static/cards/terminal.png` & `qbraid_core-0.1.9/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/docs/_static/css/custom.css` & `qbraid_core-0.1.9/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/docs/_static/css/s4defs-roles.css` & `qbraid_core-0.1.9/docs/_static/css/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/docs/_static/favicon.ico` & `qbraid_core-0.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/docs/_static/logo.png` & `qbraid_core-0.1.9/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/docs/conf.py` & `qbraid_core-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/docs/index.rst` & `qbraid_core-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/docs/make.bat` & `qbraid_core-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/pyproject.toml` & `qbraid_core-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-core"
-version = "0.1.8"
+version = "0.1.9"
 authors = [{name = "qBraid Development Team"}, {email = "contact@qbraid.com"}]
 description = "Python library with core abstractions for software development in the qBraid ecosystem."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["qbraid", "quantum", "cloud"]
 license = {text = "Proprietary"}
 classifiers = [
```

### Comparing `qbraid_core-0.1.8/qbraid_core/__init__.py` & `qbraid_core-0.1.9/qbraid_core/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/_compat.py` & `qbraid_core-0.1.9/qbraid_core/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/_import.py` & `qbraid_core-0.1.9/qbraid_core/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/annotations.py` & `qbraid_core-0.1.9/qbraid_core/annotations.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/client.py` & `qbraid_core-0.1.9/qbraid_core/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/config.py` & `qbraid_core-0.1.9/qbraid_core/config.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/context.py` & `qbraid_core-0.1.9/qbraid_core/context.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/exceptions.py` & `qbraid_core-0.1.9/qbraid_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/registry.py` & `qbraid_core-0.1.9/qbraid_core/registry.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/retry.py` & `qbraid_core-0.1.9/qbraid_core/retry.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/admin/client.py` & `qbraid_core-0.1.9/qbraid_core/services/admin/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/environments/__init__.py` & `qbraid_core-0.1.9/qbraid_core/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/environments/client.py` & `qbraid_core-0.1.9/qbraid_core/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/environments/create.py` & `qbraid_core-0.1.9/qbraid_core/services/environments/create.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/environments/magic.py` & `qbraid_core-0.1.9/qbraid_core/services/environments/magic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/environments/paths.py` & `qbraid_core-0.1.9/qbraid_core/services/environments/paths.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/environments/state.py` & `qbraid_core-0.1.9/qbraid_core/services/environments/state.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/environments/validate.py` & `qbraid_core-0.1.9/qbraid_core/services/environments/validate.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/quantum/__init__.py` & `qbraid_core-0.1.9/qbraid_core/services/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/quantum/adapter.py` & `qbraid_core-0.1.9/qbraid_core/services/quantum/adapter.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/quantum/client.py` & `qbraid_core-0.1.9/qbraid_core/services/quantum/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/quantum/compat.py` & `qbraid_core-0.1.9/qbraid_core/services/quantum/compat.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/quantum/proxy.py` & `qbraid_core-0.1.9/qbraid_core/services/quantum/proxy.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/quantum/proxy_braket.py` & `qbraid_core-0.1.9/qbraid_core/services/quantum/proxy_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/services/quantum/runner.py` & `qbraid_core-0.1.9/qbraid_core/services/quantum/runner.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/sessions.py` & `qbraid_core-0.1.9/qbraid_core/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,17 @@
 
         section = DEFAULT_CONFIG_SECTION
         if section not in config.sections():
             config.add_section(section)
 
         # Helper function to set config options only if different or not set
         def update_config_option(section, option, value):
-            if not config.has_option(section, option) or config.get(section, option) != value:
+            if option and (
+                not config.has_option(section, option) or config.get(section, option) != value
+            ):
                 config.set(section, option, value)
 
         # Set or update configurations
         update_config_option(section, "email", self._user_email)
         update_config_option(section, "api-key", self._api_key)
         update_config_option(
             section, "refresh-token", kwargs.get("refresh_token", self._refresh_token)
```

### Comparing `qbraid_core-0.1.8/qbraid_core/system/__init__.py` & `qbraid_core-0.1.9/qbraid_core/system/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/system/exceptions.py` & `qbraid_core-0.1.9/qbraid_core/system/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/system/executables.py` & `qbraid_core-0.1.9/qbraid_core/system/executables.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/system/generic.py` & `qbraid_core-0.1.9/qbraid_core/system/generic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/system/magic/manager.py` & `qbraid_core-0.1.9/qbraid_core/system/magic/manager.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/system/magic/qbraid_magic.py` & `qbraid_core-0.1.9/qbraid_core/system/magic/qbraid_magic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/system/packages.py` & `qbraid_core-0.1.9/qbraid_core/system/packages.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/system/threader.py` & `qbraid_core-0.1.9/qbraid_core/system/threader.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core/system/versions.py` & `qbraid_core-0.1.9/qbraid_core/system/versions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/qbraid_core.egg-info/PKG-INFO` & `qbraid_core-0.1.9/qbraid_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author: qBraid Development Team
 Author-email: contact@qbraid.com
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
```

### Comparing `qbraid_core-0.1.8/qbraid_core.egg-info/SOURCES.txt` & `qbraid_core-0.1.9/qbraid_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/environments/fixtures/environments.py` & `qbraid_core-0.1.9/tests/environments/fixtures/environments.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/environments/test_client.py` & `qbraid_core-0.1.9/tests/environments/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/environments/test_create.py` & `qbraid_core-0.1.9/tests/environments/test_create.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/environments/test_paths.py` & `qbraid_core-0.1.9/tests/environments/test_paths.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/environments/test_state.py` & `qbraid_core-0.1.9/tests/environments/test_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/environments/test_validate.py` & `qbraid_core-0.1.9/tests/environments/test_validate.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/quantum/resources/qir_program.bc` & `qbraid_core-0.1.9/tests/quantum/resources/qir_program.bc`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/quantum/resources/qir_runner_stdout.txt` & `qbraid_core-0.1.9/tests/quantum/resources/qir_runner_stdout.txt`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/quantum/test_aws_configure.py` & `qbraid_core-0.1.9/tests/quantum/test_aws_configure.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/quantum/test_proxy.py` & `qbraid_core-0.1.9/tests/quantum/test_proxy.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/quantum/test_qir_runner.py` & `qbraid_core-0.1.9/tests/quantum/test_qir_runner.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/system/test_executables.py` & `qbraid_core-0.1.9/tests/system/test_executables.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/system/test_generic.py` & `qbraid_core-0.1.9/tests/system/test_generic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/system/test_packages.py` & `qbraid_core-0.1.9/tests/system/test_packages.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/system/test_versions.py` & `qbraid_core-0.1.9/tests/system/test_versions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/top_level/test_annotations.py` & `qbraid_core-0.1.9/tests/top_level/test_annotations.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/top_level/test_client.py` & `qbraid_core-0.1.9/tests/top_level/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/top_level/test_compat.py` & `qbraid_core-0.1.9/tests/top_level/test_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/top_level/test_config.py` & `qbraid_core-0.1.9/tests/top_level/test_config.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/top_level/test_context.py` & `qbraid_core-0.1.9/tests/top_level/test_context.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/top_level/test_lazy_loader.py` & `qbraid_core-0.1.9/tests/top_level/test_lazy_loader.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tests/top_level/test_sessions.py` & `qbraid_core-0.1.9/tests/top_level/test_sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tools/create_dev_build.sh` & `qbraid_core-0.1.9/tools/create_dev_build.sh`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.8/tools/stamp_pre_release.py` & `qbraid_core-0.1.9/tools/stamp_pre_release.py`

 * *Files identical despite different names*

