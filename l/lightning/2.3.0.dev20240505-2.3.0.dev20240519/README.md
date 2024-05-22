# Comparing `tmp/lightning-2.3.0.dev20240505.tar.gz` & `tmp/lightning-2.3.0.dev20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-2.3.0.dev20240505.tar", last modified: Sun May  5 00:20:12 2024, max compression
+gzip compressed data, was "lightning-2.3.0.dev20240519.tar", last modified: Sun May 19 00:20:51 2024, max compression
```

## Comparing `lightning-2.3.0.dev20240505.tar` & `lightning-2.3.0.dev20240519.tar`

### file list

```diff
@@ -1,681 +1,683 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.626881 lightning-2.3.0.dev20240505/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.546880 lightning-2.3.0.dev20240505/.actions/
--rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24254 2024-05-05 00:20:12.626881 lightning-2.3.0.dev20240505/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22984 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.546880 lightning-2.3.0.dev20240505/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.546880 lightning-2.3.0.dev20240505/requirements/app/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/app/app.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/app/cloud.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/app/components.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/app/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/app/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/app/ui.txt
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-05 00:20:11.000000 lightning-2.3.0.dev20240505/requirements/base.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.546880 lightning-2.3.0.dev20240505/requirements/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/fabric/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/fabric/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/fabric/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/fabric/strategies.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/fabric/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.546880 lightning-2.3.0.dev20240505/requirements/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/pytorch/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/pytorch/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/pytorch/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/pytorch/extra.txt
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/pytorch/strategies.txt
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/requirements/pytorch/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 00:20:12.626881 lightning-2.3.0.dev20240505/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     7935 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.546880 lightning-2.3.0.dev20240505/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.550880 lightning-2.3.0.dev20240505/src/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.550880 lightning-2.3.0.dev20240505/src/lightning/app/
--rw-r--r--   0 runner    (1001) docker     (127)    37365 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.550880 lightning-2.3.0.dev20240505/src/lightning/app/api/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/api/http_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/api/request_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.550880 lightning-2.3.0.dev20240505/src/lightning/app/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.554880 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.554880 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/placeholdername/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.534880 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/placeholdername/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.554880 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/placeholdername/components/component_a/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/placeholdername/components/component_a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/placeholdername/components/component_a/component_a.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.554880 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/placeholdername/components/component_b/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/placeholdername/components/component_b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/placeholdername/components/component_b/component_a.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.554880 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/tests/test_placeholdername_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/cmd_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    21517 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/cmd_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/cmd_pl_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/cmd_react_ui_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.554880 lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/cd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/pwd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/rm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.554880 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.538880 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.554880 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/.github/workflows/ci-testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.554880 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/placeholdername/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/placeholdername/component.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.558880 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/tests/test_placeholdername_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.558880 lightning-2.3.0.dev20240505/src/lightning/app/cli/connect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/connect/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/connect/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12669 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/lightning_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/lightning_cli_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/lightning_cli_launch.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/lightning_cli_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.558880 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/.lightningignore
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.558880 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.558880 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/components/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.558880 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/components/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/components/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/components/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/components/logger/weights_and_biases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.558880 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/components/script_runner/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/components/script_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/components/script_runner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.558880 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.558880 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/tests/core/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/tests/test_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.558880 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/craco.config.js
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.562881 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/public/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/public/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.562881 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/App.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.562881 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/Launcher.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/Timer.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.562881 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/index.tsx
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/lightning-colors.ts
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/react-app-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/reportWebVitals.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.562881 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.562881 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/example_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.562881 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.566881 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/App.css
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/App.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/favicon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.566881 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/main.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.566881 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/vite-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/tsconfig.node.json
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/vite.config.ts
--rw-r--r--   0 runner    (1001) docker     (127)    62319 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.566881 lightning-2.3.0.dev20240505/src/lightning/app/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.566881 lightning-2.3.0.dev20240505/src/lightning/app/components/database/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/database/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/database/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/database/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.566881 lightning-2.3.0.dev20240505/src/lightning/app/components/multi_node/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/multi_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/multi_node/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/multi_node/fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/multi_node/pytorch_spawn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/multi_node/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.566881 lightning-2.3.0.dev20240505/src/lightning/app/components/python/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/python/popen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/python/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.566881 lightning-2.3.0.dev20240505/src/lightning/app/components/serve/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30437 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/serve/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)    20105 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/serve/catimage.png
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/serve/cold_start_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/serve/gradio_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/serve/python_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/serve/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/serve/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.570881 lightning-2.3.0.dev20240505/src/lightning/app/components/serve/types/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/serve/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/serve/types/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/serve/types/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/components/training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.570881 lightning-2.3.0.dev20240505/src/lightning/app/core/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/core/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29931 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/core/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    33041 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    21814 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/core/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/core/work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.570881 lightning-2.3.0.dev20240505/src/lightning/app/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.570881 lightning-2.3.0.dev20240505/src/lightning/app/frontend/just_py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/just_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/just_py/just_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/just_py/just_py_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.570881 lightning-2.3.0.dev20240505/src/lightning/app/frontend/panel/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/panel/app_state_comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/panel/app_state_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/panel/panel_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/panel/panel_serve_render_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/stream_lit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/streamlit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/frontend/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.570881 lightning-2.3.0.dev20240505/src/lightning/app/launcher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15316 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/launcher/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    21529 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/launcher/lightning_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/launcher/lightning_hybrid_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.570881 lightning-2.3.0.dev20240505/src/lightning/app/pdb/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/pdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/pdb/pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.570881 lightning-2.3.0.dev20240505/src/lightning/app/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.574881 lightning-2.3.0.dev20240505/src/lightning/app/runners/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.574881 lightning-2.3.0.dev20240505/src/lightning/app/runners/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/runners/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/runners/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/runners/backends/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/runners/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/runners/backends/mp_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    47781 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/runners/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/runners/multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/runners/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/runners/runtime_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.574881 lightning-2.3.0.dev20240505/src/lightning/app/source_code/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/source_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/source_code/copytree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/source_code/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/source_code/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/source_code/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/source_code/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.574881 lightning-2.3.0.dev20240505/src/lightning/app/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/storage/copier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/storage/drive.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/storage/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/storage/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/storage/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18320 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/storage/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/storage/payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/storage/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.574881 lightning-2.3.0.dev20240505/src/lightning/app/structures/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/structures/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/structures/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.578881 lightning-2.3.0.dev20240505/src/lightning/app/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/testing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19345 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.578881 lightning-2.3.0.dev20240505/src/lightning/app/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.578881 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.578881 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/css/main.fb7060be.css
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/css/main.fb7060be.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.578881 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/js/787.418637a8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/js/787.418637a8.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   503634 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/js/main.c1f02aeb.js
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/js/main.c1f02aeb.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2068175 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/js/main.c1f02aeb.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/lightningState.js
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.582881 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/static/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240505/src/lightning/app/ui/version.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.586881 lightning-2.3.0.dev20240505/src/lightning/app/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/app_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/app_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/app_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/cli_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.586881 lightning-2.3.0.dev20240505/src/lightning/app/utilities/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/dependency_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10724 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/load_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/log_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/logs_socket_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    60256 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.590881 lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/app_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/build_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/cloud_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/tarfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/port.py
--rw-r--r--   0 runner    (1001) docker     (127)    30254 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/safe_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/app/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-05 00:20:11.000000 lightning-2.3.0.dev20240505/src/lightning/c475c1d37e4559adf497c85932243ae1fb375cfdcf0fabf9
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.590881 lightning-2.3.0.dev20240505/src/lightning/data/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.590881 lightning-2.3.0.dev20240505/src/lightning/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)    33002 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.590881 lightning-2.3.0.dev20240505/src/lightning/fabric/_graveyard/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/_graveyard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/_graveyard/tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.590881 lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    49945 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/fabric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.590881 lightning-2.3.0.dev20240505/src/lightning/fabric/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.590881 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.590881 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/collectives/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/collectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/collectives/collective.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/collectives/single_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/collectives/torch_collective.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.594881 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/cluster_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/kubeflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/torchelastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.594881 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/io/checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/io/torch_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/io/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.594881 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/amp.py
--rw-r--r--   0 runner    (1001) docker     (127)    20991 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/bitsandbytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/half.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/transformer_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.598881 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/dp.py
--rw-r--r--   0 runner    (1001) docker     (127)    42701 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.598881 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/single_xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    18307 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/xla_fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.602881 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/consolidate_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/device_dtype_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/device_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16775 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/spike.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.602881 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/testing/_runif.py
--rw-r--r--   0 runner    (1001) docker     (127)    27517 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/throughput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/fabric/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.602881 lightning-2.3.0.dev20240505/src/lightning/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)   456911 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.602881 lightning-2.3.0.dev20240505/src/lightning/pytorch/_graveyard/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/_graveyard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/_graveyard/_torchmetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/_graveyard/hpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/_graveyard/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/_graveyard/tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.602881 lightning-2.3.0.dev20240505/src/lightning/pytorch/accelerators/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/accelerators/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.606881 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/batch_size_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11022 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/device_stats_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)    19095 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/gradient_accumulation_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/lr_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    38563 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/model_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/on_exception_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/prediction_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.606881 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/progress/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/progress/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)    25511 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/progress/rich_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/progress/tqdm_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/pruning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/rich_model_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/spike.py
--rw-r--r--   0 runner    (1001) docker     (127)    17914 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/stochastic_weight_avg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/throughput_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    38235 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.610881 lightning-2.3.0.dev20240505/src/lightning/pytorch/core/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/core/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)    26793 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/core/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.610881 lightning-2.3.0.dev20240505/src/lightning/pytorch/core/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/core/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/core/mixins/hparams_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    70673 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/core/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/core/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/core/saving.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.610881 lightning-2.3.0.dev20240505/src/lightning/pytorch/demos/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/demos/boring_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/demos/mnist_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/demos/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.610881 lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    23271 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24944 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.610881 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25464 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/evaluation_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/fetchers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19179 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/fit_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.614881 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/optimization/automatic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/optimization/closure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/optimization/manual.py
--rw-r--r--   0 runner    (1001) docker     (127)    18682 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/prediction_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    23209 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/training_epoch_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.614881 lightning-2.3.0.dev20240505/src/lightning/pytorch/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/overrides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/overrides/distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.614881 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.614881 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/environments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.614881 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/io/async_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/io/checkpoint_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/io/torch_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/io/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/io/xla_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/layer_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.614881 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/amp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/bitsandbytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/half.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/transformer_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.618881 lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    23778 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.618881 lightning-2.3.0.dev20240505/src/lightning/pytorch/serve/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/serve/servable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/serve/servable_module_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.618881 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19061 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)    41000 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)    29961 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.618881 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/single_xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    25567 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.618881 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/configuration_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.622881 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31275 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/accelerator_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10663 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/callback_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    24486 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/checkpoint_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    22488 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/data_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.622881 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/logger_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/logger_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/logger_connector/fx_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/logger_connector/logger_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    20802 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/logger_connector/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/signal_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/states.py
--rw-r--r--   0 runner    (1001) docker     (127)    72654 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.622881 lightning-2.3.0.dev20240505/src/lightning/pytorch/tuner/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/tuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12868 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/tuner/batch_size_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/tuner/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/tuner/tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.626881 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/_pytree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/combined_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/consolidate_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/grads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.626881 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/migration/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/migration/migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/migration/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/model_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.626881 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/model_summary/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/model_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/model_summary/model_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/model_summary/model_summary_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/parameter_tying.py
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/signature_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.626881 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/testing/_runif.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/upgrade_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.626881 lightning-2.3.0.dev20240505/src/lightning/store/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/store/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-05 00:19:53.000000 lightning-2.3.0.dev20240505/src/lightning/store/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 00:19:56.000000 lightning-2.3.0.dev20240505/src/lightning/version.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:20:12.550880 lightning-2.3.0.dev20240505/src/lightning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24254 2024-05-05 00:20:12.000000 lightning-2.3.0.dev20240505/src/lightning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26370 2024-05-05 00:20:12.000000 lightning-2.3.0.dev20240505/src/lightning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 00:20:12.000000 lightning-2.3.0.dev20240505/src/lightning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-05 00:20:12.000000 lightning-2.3.0.dev20240505/src/lightning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 00:20:12.000000 lightning-2.3.0.dev20240505/src/lightning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-05 00:20:12.000000 lightning-2.3.0.dev20240505/src/lightning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 00:20:12.000000 lightning-2.3.0.dev20240505/src/lightning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 00:19:56.000000 lightning-2.3.0.dev20240505/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.584530 lightning-2.3.0.dev20240519/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.492530 lightning-2.3.0.dev20240519/.actions/
+-rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24254 2024-05-19 00:20:51.584530 lightning-2.3.0.dev20240519/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22984 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.496530 lightning-2.3.0.dev20240519/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.496530 lightning-2.3.0.dev20240519/requirements/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/app/app.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/app/cloud.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/app/components.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/app/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/app/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/app/ui.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-19 00:20:50.000000 lightning-2.3.0.dev20240519/requirements/base.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.496530 lightning-2.3.0.dev20240519/requirements/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/fabric/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/fabric/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/fabric/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/fabric/strategies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/fabric/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.496530 lightning-2.3.0.dev20240519/requirements/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/pytorch/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/pytorch/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/pytorch/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/pytorch/extra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/pytorch/strategies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/requirements/pytorch/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 00:20:51.584530 lightning-2.3.0.dev20240519/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7935 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.496530 lightning-2.3.0.dev20240519/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.496530 lightning-2.3.0.dev20240519/src/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-19 00:20:50.000000 lightning-2.3.0.dev20240519/src/lightning/03b460d403e09cdf43eab937b2d65f81d750629927cf0e82
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.500530 lightning-2.3.0.dev20240519/src/lightning/app/
+-rw-r--r--   0 runner    (1001) docker     (127)    37365 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.500530 lightning-2.3.0.dev20240519/src/lightning/app/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/api/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/api/request_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.500530 lightning-2.3.0.dev20240519/src/lightning/app/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.504530 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.504530 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/placeholdername/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.484530 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/placeholdername/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.504530 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/placeholdername/components/component_a/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/placeholdername/components/component_a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/placeholdername/components/component_a/component_a.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.504530 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/placeholdername/components/component_b/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/placeholdername/components/component_b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/placeholdername/components/component_b/component_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.504530 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/tests/test_placeholdername_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/cmd_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21517 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/cmd_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/cmd_pl_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/cmd_react_ui_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.504530 lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/cd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/rm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.508530 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.484530 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.508530 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/.github/workflows/ci-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.508530 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/placeholdername/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/placeholdername/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.508530 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/tests/test_placeholdername_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.508530 lightning-2.3.0.dev20240519/src/lightning/app/cli/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/connect/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/connect/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12669 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/lightning_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/lightning_cli_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/lightning_cli_launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/lightning_cli_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.508530 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/.lightningignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.508530 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.512530 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.512530 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/components/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/components/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/components/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/components/logger/weights_and_biases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.512530 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/components/script_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/components/script_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/components/script_runner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.512530 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.512530 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/tests/core/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.512530 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/craco.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.512530 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/public/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/public/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.512530 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/App.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.512530 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/Launcher.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/Timer.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.516530 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/lightning-colors.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/react-app-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/reportWebVitals.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.516530 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.516530 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/example_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.516530 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.516530 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/App.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/favicon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.516530 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/main.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.516530 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/vite-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/tsconfig.node.json
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/vite.config.ts
+-rw-r--r--   0 runner    (1001) docker     (127)    62319 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.516530 lightning-2.3.0.dev20240519/src/lightning/app/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.516530 lightning-2.3.0.dev20240519/src/lightning/app/components/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/database/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/database/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/database/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.520530 lightning-2.3.0.dev20240519/src/lightning/app/components/multi_node/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/multi_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/multi_node/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/multi_node/fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/multi_node/pytorch_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/multi_node/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.520530 lightning-2.3.0.dev20240519/src/lightning/app/components/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/python/popen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/python/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.520530 lightning-2.3.0.dev20240519/src/lightning/app/components/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30437 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/serve/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20105 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/serve/catimage.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/serve/cold_start_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/serve/gradio_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/serve/python_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/serve/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/serve/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.520530 lightning-2.3.0.dev20240519/src/lightning/app/components/serve/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/serve/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/serve/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/serve/types/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/components/training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.520530 lightning-2.3.0.dev20240519/src/lightning/app/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30160 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33041 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21814 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/core/queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/core/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.524530 lightning-2.3.0.dev20240519/src/lightning/app/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.524530 lightning-2.3.0.dev20240519/src/lightning/app/frontend/just_py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/just_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/just_py/just_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/just_py/just_py_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.524530 lightning-2.3.0.dev20240519/src/lightning/app/frontend/panel/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/panel/app_state_comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/panel/app_state_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/panel/panel_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/panel/panel_serve_render_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/stream_lit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/streamlit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/frontend/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.524530 lightning-2.3.0.dev20240519/src/lightning/app/launcher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15316 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/launcher/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21529 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/launcher/lightning_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/launcher/lightning_hybrid_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.524530 lightning-2.3.0.dev20240519/src/lightning/app/pdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/pdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/pdb/pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.524530 lightning-2.3.0.dev20240519/src/lightning/app/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.528530 lightning-2.3.0.dev20240519/src/lightning/app/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.528530 lightning-2.3.0.dev20240519/src/lightning/app/runners/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/runners/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/runners/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/runners/backends/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/runners/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/runners/backends/mp_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/runners/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/runners/multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/runners/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/runners/runtime_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.528530 lightning-2.3.0.dev20240519/src/lightning/app/source_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/source_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/source_code/copytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/source_code/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/source_code/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/source_code/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/source_code/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.528530 lightning-2.3.0.dev20240519/src/lightning/app/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/storage/copier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/storage/drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/storage/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/storage/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/storage/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18320 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/storage/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/storage/payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/storage/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.528530 lightning-2.3.0.dev20240519/src/lightning/app/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/structures/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/structures/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.532530 lightning-2.3.0.dev20240519/src/lightning/app/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19345 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.532530 lightning-2.3.0.dev20240519/src/lightning/app/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.532530 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.532530 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/css/main.fb7060be.css
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/css/main.fb7060be.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.532530 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/js/787.418637a8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/js/787.418637a8.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   503634 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/js/main.c1f02aeb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/js/main.c1f02aeb.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2068175 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/js/main.c1f02aeb.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/lightningState.js
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.536530 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240519/src/lightning/app/ui/version.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.544530 lightning-2.3.0.dev20240519/src/lightning/app/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/app_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/app_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/app_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/cli_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.544530 lightning-2.3.0.dev20240519/src/lightning/app/utilities/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/dependency_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10724 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/load_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/logs_socket_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60256 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.544530 lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/cloud_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/tarfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30254 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/safe_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/app/utilities/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.544530 lightning-2.3.0.dev20240519/src/lightning/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.544530 lightning-2.3.0.dev20240519/src/lightning/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)    33530 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.544530 lightning-2.3.0.dev20240519/src/lightning/fabric/_graveyard/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/_graveyard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/_graveyard/tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.548530 lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49977 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.548530 lightning-2.3.0.dev20240519/src/lightning/fabric/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.548530 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.548530 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/collectives/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/collectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/collectives/collective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/collectives/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/collectives/torch_collective.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.548530 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/cluster_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/kubeflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/torchelastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.548530 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/io/checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/io/torch_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/io/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.552530 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/amp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20991 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/bitsandbytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/half.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/transformer_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.552530 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/dp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40789 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.552530 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26396 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/model_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/single_xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18307 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/xla_fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.556530 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/consolidate_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/device_dtype_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/device_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16775 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/spike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.556530 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/testing/_runif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27517 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/throughput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17584 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/fabric/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.556530 lightning-2.3.0.dev20240519/src/lightning/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)   456911 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.556530 lightning-2.3.0.dev20240519/src/lightning/pytorch/_graveyard/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/_graveyard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/_graveyard/_torchmetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/_graveyard/hpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/_graveyard/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/_graveyard/tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.560530 lightning-2.3.0.dev20240519/src/lightning/pytorch/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/accelerators/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.564530 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/batch_size_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11022 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/device_stats_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19095 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/gradient_accumulation_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/lr_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38563 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/on_exception_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/prediction_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.564530 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/progress/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/progress/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25511 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/progress/rich_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/progress/tqdm_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/pruning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/rich_model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/spike.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17914 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/stochastic_weight_avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/throughput_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38235 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.564530 lightning-2.3.0.dev20240519/src/lightning/pytorch/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/core/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26793 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/core/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.564530 lightning-2.3.0.dev20240519/src/lightning/pytorch/core/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/core/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/core/mixins/hparams_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71237 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/core/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/core/saving.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.568530 lightning-2.3.0.dev20240519/src/lightning/pytorch/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/demos/boring_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/demos/mnist_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/demos/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.568530 lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23271 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24944 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.568530 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25464 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/evaluation_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/fetchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19179 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/fit_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.572530 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/optimization/automatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/optimization/closure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/optimization/manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18682 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/prediction_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23209 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/training_epoch_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.572530 lightning-2.3.0.dev20240519/src/lightning/pytorch/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/overrides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/overrides/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.572530 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.572530 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/environments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.572530 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/io/async_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/io/checkpoint_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/io/torch_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/io/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/io/xla_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/layer_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.572530 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/amp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/bitsandbytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/half.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/transformer_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.576530 lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23778 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.576530 lightning-2.3.0.dev20240519/src/lightning/pytorch/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/serve/servable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/serve/servable_module_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.576530 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19061 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41000 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.576530 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14177 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/model_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/single_xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25567 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.580530 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/configuration_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.580530 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31337 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/accelerator_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10663 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/callback_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24486 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/checkpoint_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22488 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/data_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.580530 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/logger_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/logger_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/logger_connector/fx_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/logger_connector/logger_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20802 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/logger_connector/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/signal_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72654 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.580530 lightning-2.3.0.dev20240519/src/lightning/pytorch/tuner/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/tuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12868 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/tuner/batch_size_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/tuner/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/tuner/tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.584530 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/_pytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/combined_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/consolidate_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/grads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.584530 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/migration/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/migration/migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/migration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/model_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.584530 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/model_summary/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/model_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/model_summary/model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/model_summary/model_summary_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/parameter_tying.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/signature_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.584530 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/testing/_runif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/upgrade_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.584530 lightning-2.3.0.dev20240519/src/lightning/store/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-19 00:20:31.000000 lightning-2.3.0.dev20240519/src/lightning/store/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 00:20:36.000000 lightning-2.3.0.dev20240519/src/lightning/version.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:20:51.500530 lightning-2.3.0.dev20240519/src/lightning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24254 2024-05-19 00:20:51.000000 lightning-2.3.0.dev20240519/src/lightning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26471 2024-05-19 00:20:51.000000 lightning-2.3.0.dev20240519/src/lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 00:20:51.000000 lightning-2.3.0.dev20240519/src/lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-19 00:20:51.000000 lightning-2.3.0.dev20240519/src/lightning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 00:20:51.000000 lightning-2.3.0.dev20240519/src/lightning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-19 00:20:51.000000 lightning-2.3.0.dev20240519/src/lightning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 00:20:51.000000 lightning-2.3.0.dev20240519/src/lightning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 00:20:36.000000 lightning-2.3.0.dev20240519/src/version.info
```

### Comparing `lightning-2.3.0.dev20240505/.actions/assistant.py` & `lightning-2.3.0.dev20240519/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/CITATION.cff` & `lightning-2.3.0.dev20240519/CITATION.cff`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/LICENSE` & `lightning-2.3.0.dev20240519/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/PKG-INFO` & `lightning-2.3.0.dev20240519/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning
-Version: 2.3.0.dev20240505
+Version: 2.3.0.dev20240519
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -23,42 +23,42 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: app-components
-Provides-Extra: app-cloud
+Provides-Extra: fabric-examples
+Provides-Extra: fabric-strategies
+Provides-Extra: fabric-test
+Provides-Extra: store-test
 Provides-Extra: app-ui
+Provides-Extra: app-cloud
 Provides-Extra: app-test
-Provides-Extra: store-test
+Provides-Extra: app-components
+Provides-Extra: pytorch-examples
 Provides-Extra: pytorch-strategies
-Provides-Extra: pytorch-test
 Provides-Extra: pytorch-extra
-Provides-Extra: pytorch-examples
-Provides-Extra: fabric-strategies
-Provides-Extra: fabric-test
-Provides-Extra: fabric-examples
+Provides-Extra: pytorch-test
 Provides-Extra: fabric-all
 Provides-Extra: fabric-dev
 Provides-Extra: pytorch-all
 Provides-Extra: pytorch-dev
 Provides-Extra: app-extra
 Provides-Extra: app-all
 Provides-Extra: app-dev
-Provides-Extra: components
-Provides-Extra: cloud
+Provides-Extra: data
+Provides-Extra: examples
+Provides-Extra: strategies
+Provides-Extra: test
 Provides-Extra: ui
+Provides-Extra: cloud
 Provides-Extra: app
-Provides-Extra: test
-Provides-Extra: strategies
+Provides-Extra: components
 Provides-Extra: extra
-Provides-Extra: examples
-Provides-Extra: data
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: store
 License-File: LICENSE
 
 <div align="center">
 
@@ -74,15 +74,15 @@
 ______________________________________________________________________
 
 <p align="center">
   <a href="https://lightning.ai/">Lightning.ai</a> •
   <a href="https://lightning.ai/docs/pytorch/stable/">PyTorch Lightning</a> •
   <a href="https://lightning.ai/docs/fabric/stable/">Fabric</a> •
   <a href="https://lightning.ai/docs/app/stable/">Lightning Apps</a> •
-  <a href="https://pytorch-lightning.readthedocs.io/en/2.3.0.dev20240505">Docs</a> •
+  <a href="https://pytorch-lightning.readthedocs.io/en/2.3.0.dev20240519">Docs</a> •
   <a href="#community">Community</a> •
   <a href="https://lightning.ai/docs/pytorch/stable/generated/CONTRIBUTING.html">Contribute</a> •
 </p>
 
 <!-- DO NOT ADD CONDA DOWNLOADS... README CHANGES MUST BE APPROVED BY EDEN OR WILL -->
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)](https://pypi.org/project/pytorch-lightning/)
@@ -619,15 +619,15 @@
 <details>
   <summary>Current build statuses</summary>
 
 <center>
 
 |       System / PyTorch ver.        | 1.13                                                                                                                                                                                                                            | 2.0                                                                                                                                                                                                                             |                                                                                                               2.1                                                                                                               |
 | :--------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-|        Linux py3.9 \[GPUs\]        |  |  | [![Build Status](https://dev.azure.com/Lightning-AI/lightning/_apis/build/status%2Fpytorch-lightning%20%28GPUs%29?branchName=refs%2Ftags%2F2.3.0.dev20240505)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=24&branchName=master) |
+|        Linux py3.9 \[GPUs\]        |  |  | [![Build Status](https://dev.azure.com/Lightning-AI/lightning/_apis/build/status%2Fpytorch-lightning%20%28GPUs%29?branchName=refs%2Ftags%2F2.3.0.dev20240519)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=24&branchName=master) |
 |        Linux py3.9 \[TPUs\]        |                                                                                                                                                                                                                                 |  [![Test PyTorch - TPU](https://github.com/Lightning-AI/lightning/actions/workflows/tpu-tests.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/tpu-tests.yml)     |      |
 |  Linux (multiple Python versions)  | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 |                 [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                 |
 |   OSX (multiple Python versions)   | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 |                 [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                 |
 | Windows (multiple Python versions) | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 |                 [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                 |
 
 </center>
 </details>
```

### Comparing `lightning-2.3.0.dev20240505/README.md` & `lightning-2.3.0.dev20240519/README.md`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/pyproject.toml` & `lightning-2.3.0.dev20240519/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/requirements/app/app.txt` & `lightning-2.3.0.dev20240519/requirements/app/app.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-lightning-cloud == 0.5.68  # Must be pinned to ensure compatibility
+lightning-cloud == 0.5.69  # Must be pinned to ensure compatibility
 packaging
 typing-extensions >=4.4.0, <4.10.0
 deepdiff >=5.7.0, <6.6.0
 fsspec[http] >=2022.5.0, <2023.11.0
 croniter >=1.3.0, <1.5.0  # strict; TODO: for now until we find something more robust.
 traitlets >=5.3.0, <5.12.0
 arrow >=1.2.0, <1.3.0
```

### Comparing `lightning-2.3.0.dev20240505/requirements/fabric/strategies.txt` & `lightning-2.3.0.dev20240519/requirements/fabric/strategies.txt`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/requirements/pytorch/base.txt` & `lightning-2.3.0.dev20240519/requirements/pytorch/base.txt`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/requirements/pytorch/extra.txt` & `lightning-2.3.0.dev20240519/requirements/pytorch/extra.txt`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/requirements/pytorch/test.txt` & `lightning-2.3.0.dev20240519/requirements/pytorch/test.txt`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/setup.py` & `lightning-2.3.0.dev20240519/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/__about__.py` & `lightning-2.3.0.dev20240519/src/lightning/__about__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/__setup__.py` & `lightning-2.3.0.dev20240519/src/lightning/__setup__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/CHANGELOG.md` & `lightning-2.3.0.dev20240519/src/lightning/app/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/app/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/api/http_methods.py` & `lightning-2.3.0.dev20240519/src/lightning/app/api/http_methods.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/api/request_types.py` & `lightning-2.3.0.dev20240519/src/lightning/app/api/request_types.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/.gitignore` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/LICENSE` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/README.md` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/app-template/tests/test_placeholdername_app.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/app-template/tests/test_placeholdername_app.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/cmd_apps.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/cmd_apps.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/cmd_init.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/cmd_init.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/cmd_install.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/cmd_install.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/cmd_pl_init.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/cmd_pl_init.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/cmd_react_ui_init.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/cmd_react_ui_init.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/app_commands.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/cd.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/cd.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/cp.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/cp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/logs.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/logs.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/ls.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/ls.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/pwd.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/pwd.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/commands/rm.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/commands/rm.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/.github/workflows/ci-testing.yml` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/.github/workflows/ci-testing.yml`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/.gitignore` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/LICENSE` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/component-template/README.md` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/component-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/connect/app.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/connect/app.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/connect/data.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/connect/data.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/core.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/core.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/lightning_cli.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/lightning_cli.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/lightning_cli_delete.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/lightning_cli_delete.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/lightning_cli_launch.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/lightning_cli_launch.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/lightning_cli_list.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/lightning_cli_list.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/app.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/app.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/callbacks.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/components/logger/tensorboard.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/components/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/components/logger/weights_and_biases.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/components/logger/weights_and_biases.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/components/script_runner/script_runner.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/components/script_runner/script_runner.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/core/state.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/core/state.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/setup.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/tests/core/test_callbacks.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/tests/core/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/.prettierrc` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/.prettierrc`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/craco.config.js` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/craco.config.js`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/package.json` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/public/favicon.svg` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/public/index.html` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/public/index.html`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/App.tsx` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/Launcher.tsx` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/Launcher.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBar.tsx` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBar.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/components/Timer.tsx` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/components/Timer.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/hooks/useLightningState.ts` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/index.tsx` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/index.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/src/types/lightning.ts` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/pl-app-template/ui/tsconfig.json` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/pl-app-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/README.md` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/example_app.py` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/example_app.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/package.json` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/App.tsx` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/favicon.svg` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/hooks/useLightningState.ts` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/src/types/lightning.ts` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/tsconfig.json` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/cli/react-ui-template/ui/yarn.lock` & `lightning-2.3.0.dev20240519/src/lightning/app/cli/react-ui-template/ui/yarn.lock`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/database/client.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/database/client.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/database/server.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/database/server.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/database/utilities.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/database/utilities.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/multi_node/base.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/multi_node/base.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/multi_node/fabric.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/multi_node/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/multi_node/pytorch_spawn.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/multi_node/pytorch_spawn.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/multi_node/trainer.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/multi_node/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/python/popen.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/python/popen.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/python/tracer.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/python/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/serve/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/serve/auto_scaler.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/serve/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/serve/catimage.png` & `lightning-2.3.0.dev20240519/src/lightning/app/components/serve/catimage.png`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/serve/cold_start_proxy.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/serve/cold_start_proxy.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/serve/gradio_server.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/serve/gradio_server.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/serve/python_server.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/serve/python_server.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/serve/serve.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/serve/serve.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/serve/streamlit.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/serve/streamlit.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/serve/types/image.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/serve/types/image.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/serve/types/type.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/serve/types/type.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/components/training.py` & `lightning-2.3.0.dev20240519/src/lightning/app/components/training.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/core/api.py` & `lightning-2.3.0.dev20240519/src/lightning/app/core/api.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/core/app.py` & `lightning-2.3.0.dev20240519/src/lightning/app/core/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from lightning_utilities.core.apply_func import apply_to_collection
 
 import lightning.app
 from lightning.app import _console
 from lightning.app.api.request_types import _APIRequest, _CommandRequest, _DeltaRequest
 from lightning.app.core.constants import (
     BATCH_DELTA_COUNT,
+    CHECK_ERROR_QUEUE_INTERVAL,
     DEBUG_ENABLED,
     FLOW_DURATION_SAMPLES,
     FLOW_DURATION_THRESHOLD,
     FRONTEND_DIR,
     STATE_ACCUMULATE_WAIT,
 )
 from lightning.app.core.queues import BaseQueue
@@ -161,14 +162,15 @@
 
         self._original_state: Optional[dict] = None
         self._last_state: dict = self.state
         self.state_accumulate_wait = STATE_ACCUMULATE_WAIT
 
         self._last_run_time: float = 0.0
         self._run_times: list = []
+        self._last_check_error_queue: float = 0.0
 
         # Path attributes can't get properly attached during the initialization, because the full name
         # is only available after all Flows and Works have been instantiated.
         _convert_paths_after_init(self.root)  # type: ignore[arg-type]
 
         if log_level not in ("debug", "info"):
             raise Exception(f"Log Level should be in ['debug', 'info']. Found {log_level}")
@@ -314,18 +316,20 @@
         try:
             timeout = timeout or q.default_timeout
             return q.batch_get(timeout=timeout, count=BATCH_DELTA_COUNT)
         except queue.Empty:
             return []
 
     def check_error_queue(self) -> None:
-        exception: Exception = self.get_state_changed_from_queue(self.error_queue)  # type: ignore[assignment,arg-type]
-        if isinstance(exception, Exception):
-            self.exception = exception
-            self.stage = AppStage.FAILED
+        if (time() - self._last_check_error_queue) > CHECK_ERROR_QUEUE_INTERVAL:
+            exception: Exception = self.get_state_changed_from_queue(self.error_queue)  # type: ignore[assignment,arg-type]
+            if isinstance(exception, Exception):
+                self.exception = exception
+                self.stage = AppStage.FAILED
+            self._last_check_error_queue = time()
 
     @property
     def flows(self) -> List[Union[LightningWork, "LightningFlow"]]:
         """Returns all the flows defined within this application."""
         return [self.root] + list(self.root.flows.values())
 
     @property
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/core/constants.py` & `lightning-2.3.0.dev20240519/src/lightning/app/core/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 LIGHTNING_CLOUD_PRINT_SPECS = os.getenv("LIGHTNING_CLOUD_PRINT_SPECS")
 LIGHTNING_DIR = os.getenv("LIGHTNING_DIR", str(Path.home() / ".lightning"))
 LIGHTNING_CREDENTIAL_PATH = os.getenv("LIGHTNING_CREDENTIAL_PATH", str(Path(LIGHTNING_DIR) / "credentials.json"))
 DOT_IGNORE_FILENAME = ".lightningignore"
 LIGHTNING_COMPONENT_PUBLIC_REGISTRY = "https://lightning.ai/v1/components"
 LIGHTNING_APPS_PUBLIC_REGISTRY = "https://lightning.ai/v1/apps"
 LIGHTNING_MODELS_PUBLIC_REGISTRY = "https://lightning.ai/v1/models"
+ENABLE_ORCHESTRATOR = bool(int(os.getenv("ENABLE_ORCHESTRATOR", "1")))
 
 LIGHTNING_CLOUDSPACE_HOST = os.getenv("LIGHTNING_CLOUDSPACE_HOST")
 LIGHTNING_CLOUDSPACE_EXPOSED_PORT_COUNT = int(os.getenv("LIGHTNING_CLOUDSPACE_EXPOSED_PORT_COUNT", "0"))
 
 # EXPERIMENTAL: ENV VARIABLES TO ENABLE MULTIPLE WORKS IN THE SAME MACHINE
 DEFAULT_NUMBER_OF_EXPOSED_PORTS = int(os.getenv("DEFAULT_NUMBER_OF_EXPOSED_PORTS", "50"))
 ENABLE_MULTIPLE_WORKS_IN_NON_DEFAULT_CONTAINER = bool(
@@ -95,14 +96,15 @@
 
 # directory where system customization sync files stored
 SYS_CUSTOMIZATIONS_SYNC_ROOT = "/tmp/sys-customizations-sync"  # todo
 # directory where system customization sync files will be copied to be packed into app tarball
 SYS_CUSTOMIZATIONS_SYNC_PATH = ".sys-customizations-sync"
 
 BATCH_DELTA_COUNT = int(os.getenv("BATCH_DELTA_COUNT", "128"))
+CHECK_ERROR_QUEUE_INTERVAL = float(os.getenv("CHECK_ERROR_QUEUE_INTERVAL", "30"))
 
 
 def enable_multiple_works_in_default_container() -> bool:
     return bool(int(os.getenv("ENABLE_MULTIPLE_WORKS_IN_DEFAULT_CONTAINER", "0")))
 
 
 def get_cloud_queue_type() -> Optional[str]:
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/core/flow.py` & `lightning-2.3.0.dev20240519/src/lightning/app/core/flow.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/core/queues.py` & `lightning-2.3.0.dev20240519/src/lightning/app/core/queues.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/core/work.py` & `lightning-2.3.0.dev20240519/src/lightning/app/core/work.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/frontend/frontend.py` & `lightning-2.3.0.dev20240519/src/lightning/app/frontend/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/frontend/just_py/just_py.py` & `lightning-2.3.0.dev20240519/src/lightning/app/frontend/just_py/just_py.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/frontend/just_py/just_py_base.py` & `lightning-2.3.0.dev20240519/src/lightning/app/frontend/just_py/just_py_base.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/frontend/panel/app_state_comm.py` & `lightning-2.3.0.dev20240519/src/lightning/app/frontend/panel/app_state_comm.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/frontend/panel/app_state_watcher.py` & `lightning-2.3.0.dev20240519/src/lightning/app/frontend/panel/app_state_watcher.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/frontend/panel/panel_frontend.py` & `lightning-2.3.0.dev20240519/src/lightning/app/frontend/panel/panel_frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/frontend/panel/panel_serve_render_fn.py` & `lightning-2.3.0.dev20240519/src/lightning/app/frontend/panel/panel_serve_render_fn.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/frontend/stream_lit.py` & `lightning-2.3.0.dev20240519/src/lightning/app/frontend/stream_lit.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/frontend/streamlit_base.py` & `lightning-2.3.0.dev20240519/src/lightning/app/frontend/streamlit_base.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/frontend/utils.py` & `lightning-2.3.0.dev20240519/src/lightning/app/frontend/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/frontend/web.py` & `lightning-2.3.0.dev20240519/src/lightning/app/frontend/web.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/launcher/launcher.py` & `lightning-2.3.0.dev20240519/src/lightning/app/launcher/launcher.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/launcher/lightning_backend.py` & `lightning-2.3.0.dev20240519/src/lightning/app/launcher/lightning_backend.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/launcher/lightning_hybrid_backend.py` & `lightning-2.3.0.dev20240519/src/lightning/app/launcher/lightning_hybrid_backend.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/pdb/pdb.py` & `lightning-2.3.0.dev20240519/src/lightning/app/pdb/pdb.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/plugin/plugin.py` & `lightning-2.3.0.dev20240519/src/lightning/app/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/runners/backends/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/app/runners/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/runners/backends/backend.py` & `lightning-2.3.0.dev20240519/src/lightning/app/runners/backends/backend.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/runners/backends/cloud.py` & `lightning-2.3.0.dev20240519/src/lightning/app/runners/backends/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/runners/backends/docker.py` & `lightning-2.3.0.dev20240519/src/lightning/app/runners/backends/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/runners/backends/mp_process.py` & `lightning-2.3.0.dev20240519/src/lightning/app/runners/backends/mp_process.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/runners/cloud.py` & `lightning-2.3.0.dev20240519/src/lightning/app/runners/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import rich
 from lightning_cloud.openapi import (
     Body3,
     Body4,
     CloudspaceIdRunsBody,
     Externalv1LightningappInstance,
     Gridv1ImageSpec,
-    IdGetBody1,
+    IdGetBody,
     ProjectIdCloudspacesBody,
     V1BuildSpec,
     V1CloudSpace,
     V1DataConnectionMount,
     V1DependencyFileInfo,
     V1Drive,
     V1DriveSpec,
@@ -1023,15 +1023,15 @@
         keep_machines_after_stop: Optional[bool] = None,
     ) -> Externalv1LightningappInstance:
         """Create a new instance of the given run with the given specification."""
         return self.backend.client.cloud_space_service_create_lightning_run_instance(
             project_id=project_id,
             cloudspace_id=cloudspace_id,
             id=run_id,
-            body=IdGetBody1(
+            body=IdGetBody(
                 cluster_id=cluster_id,
                 name=run_name,
                 desired_state=desired_state,
                 queue_server_type=queue_server_type,
                 env=env_vars,
                 auth=auth,
                 source_app=source_app,
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/runners/multiprocess.py` & `lightning-2.3.0.dev20240519/src/lightning/app/runners/multiprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,24 +77,25 @@
                 )
 
                 frontend.start_server(host=server_host, port=port)
                 frontend.flow._layout["target"] = f"{server_target}/{frontend.flow.name}"
 
             _set_flow_context()
 
-            storage_orchestrator = StorageOrchestrator(
-                self.app,
-                self.app.request_queues,
-                self.app.response_queues,
-                self.app.copy_request_queues,
-                self.app.copy_response_queues,
-            )
-            self.threads.append(storage_orchestrator)
-            storage_orchestrator.setDaemon(True)
-            storage_orchestrator.start()
+            if constants.ENABLE_ORCHESTRATOR:
+                storage_orchestrator = StorageOrchestrator(
+                    self.app,
+                    self.app.request_queues,
+                    self.app.response_queues,
+                    self.app.copy_request_queues,
+                    self.app.copy_response_queues,
+                )
+                self.threads.append(storage_orchestrator)
+                storage_orchestrator.setDaemon(True)
+                storage_orchestrator.start()
 
             if self.start_server:
                 self.app.should_publish_changes_to_api = True
                 has_started_queue = self.backend.queues.get_has_server_started_queue()
 
                 apis = []
                 if is_overridden("configure_api", self.app.root):
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/runners/runtime.py` & `lightning-2.3.0.dev20240519/src/lightning/app/runners/runtime.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/runners/runtime_type.py` & `lightning-2.3.0.dev20240519/src/lightning/app/runners/runtime_type.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/source_code/copytree.py` & `lightning-2.3.0.dev20240519/src/lightning/app/source_code/copytree.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/source_code/hashing.py` & `lightning-2.3.0.dev20240519/src/lightning/app/source_code/hashing.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/source_code/local.py` & `lightning-2.3.0.dev20240519/src/lightning/app/source_code/local.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/source_code/tar.py` & `lightning-2.3.0.dev20240519/src/lightning/app/source_code/tar.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/source_code/uploader.py` & `lightning-2.3.0.dev20240519/src/lightning/app/source_code/uploader.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/storage/copier.py` & `lightning-2.3.0.dev20240519/src/lightning/app/storage/copier.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/storage/drive.py` & `lightning-2.3.0.dev20240519/src/lightning/app/storage/drive.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/storage/filesystem.py` & `lightning-2.3.0.dev20240519/src/lightning/app/storage/filesystem.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/storage/mount.py` & `lightning-2.3.0.dev20240519/src/lightning/app/storage/mount.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/storage/orchestrator.py` & `lightning-2.3.0.dev20240519/src/lightning/app/storage/orchestrator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/storage/path.py` & `lightning-2.3.0.dev20240519/src/lightning/app/storage/path.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/storage/payload.py` & `lightning-2.3.0.dev20240519/src/lightning/app/storage/payload.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/storage/requests.py` & `lightning-2.3.0.dev20240519/src/lightning/app/storage/requests.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/structures/dict.py` & `lightning-2.3.0.dev20240519/src/lightning/app/structures/dict.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/structures/list.py` & `lightning-2.3.0.dev20240519/src/lightning/app/structures/list.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/testing/config.py` & `lightning-2.3.0.dev20240519/src/lightning/app/testing/config.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/testing/helpers.py` & `lightning-2.3.0.dev20240519/src/lightning/app/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/testing/testing.py` & `lightning-2.3.0.dev20240519/src/lightning/app/testing/testing.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/ui/asset-manifest.json` & `lightning-2.3.0.dev20240519/src/lightning/app/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/ui/index.html` & `lightning-2.3.0.dev20240519/src/lightning/app/ui/index.html`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/ui/static/css/main.fb7060be.css` & `lightning-2.3.0.dev20240519/src/lightning/app/ui/static/css/main.fb7060be.css`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/ui/static/css/main.fb7060be.css.map` & `lightning-2.3.0.dev20240519/src/lightning/app/ui/static/css/main.fb7060be.css.map`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/ui/static/favicon.ico` & `lightning-2.3.0.dev20240519/src/lightning/app/ui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/ui/static/js/787.418637a8.chunk.js` & `lightning-2.3.0.dev20240519/src/lightning/app/ui/static/js/787.418637a8.chunk.js`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/ui/static/js/787.418637a8.chunk.js.map` & `lightning-2.3.0.dev20240519/src/lightning/app/ui/static/js/787.418637a8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/ui/static/js/main.c1f02aeb.js` & `lightning-2.3.0.dev20240519/src/lightning/app/ui/static/js/main.c1f02aeb.js`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/ui/static/js/main.c1f02aeb.js.LICENSE.txt` & `lightning-2.3.0.dev20240519/src/lightning/app/ui/static/js/main.c1f02aeb.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/ui/static/js/main.c1f02aeb.js.map` & `lightning-2.3.0.dev20240519/src/lightning/app/ui/static/js/main.c1f02aeb.js.map`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/ui/static/lightningState.js` & `lightning-2.3.0.dev20240519/src/lightning/app/ui/static/lightningState.js`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg` & `lightning-2.3.0.dev20240519/src/lightning/app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg` & `lightning-2.3.0.dev20240519/src/lightning/app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/app_commands.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/app_helpers.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/app_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/app_logs.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/app_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/app_status.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/app_status.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/auth.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/cli_helpers.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/cli_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/cloud.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/clusters.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/clusters.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/commands/base.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/commands/base.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/component.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/component.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/data_structures.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/data_structures.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/dependency_caching.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/dependency_caching.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/enum.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/enum.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/exceptions.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/frontend.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/git.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/git.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/imports.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/introspection.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/introspection.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/layout.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/layout.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/load_app.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/load_app.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/log.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/log.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/log_helpers.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/log_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/login.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/login.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/logs_socket_api.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/logs_socket_api.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/name_generator.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/name_generator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/network.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/network.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/openapi.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/openapi.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/app_config.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/app_config.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/build_config.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/build_config.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/cloud_compute.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/cloud_compute.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/docker.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/lightning_utils.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/lightning_utils.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/packaging/tarfile.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/packaging/tarfile.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/port.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/port.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/proxies.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/proxies.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/redis.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/safe_pickle.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/safe_pickle.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/scheduler.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/secrets.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/secrets.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/state.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/state.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/tracer.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/tree.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/tree.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/types.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/app/utilities/warnings.py` & `lightning-2.3.0.dev20240519/src/lightning/app/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/c475c1d37e4559adf497c85932243ae1fb375cfdcf0fabf9` & `lightning-2.3.0.dev20240519/src/lightning/03b460d403e09cdf43eab937b2d65f81d750629927cf0e82`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/data/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/CHANGELOG.md` & `lightning-2.3.0.dev20240519/src/lightning/fabric/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
 
 ## [unReleased] - 2024-MM-DD
 
 ### Added
 
-- Enabled consolidating distributed checkpoints through `fabric consolidate` in the new CLI [#19560](https://github.com/Lightning-AI/pytorch-lightning/pull/19560))
+- Enabled consolidating distributed checkpoints through `fabric consolidate` in the new CLI ([#19560](https://github.com/Lightning-AI/pytorch-lightning/pull/19560))
+
+- Added the ability to explicitly mark forward methods in Fabric via `_FabricModule.mark_forward_method()` ([#19690](https://github.com/Lightning-AI/pytorch-lightning/pull/19690))
 
 - Added support for PyTorch 2.3 ([#19708](https://github.com/Lightning-AI/pytorch-lightning/pull/19708))
 
--
+- Added `ModelParallelStrategy` to support 2D parallelism ([#19846](https://github.com/Lightning-AI/pytorch-lightning/pull/19846), [#19852](https://github.com/Lightning-AI/pytorch-lightning/pull/19852), [#19870](https://github.com/Lightning-AI/pytorch-lightning/pull/19870), [#19872](https://github.com/Lightning-AI/pytorch-lightning/pull/19872))
+
 
 ### Changed
 
 - Renamed `lightning run model` to `fabric run` ([#19442](https://github.com/Lightning-AI/pytorch-lightning/pull/19442), [#19527](https://github.com/Lightning-AI/pytorch-lightning/pull/19527))
 
 
 - The `Fabric.rank_zero_first` context manager now uses a barrier without timeout to avoid long-running tasks to be interrupted ([#19448](https://github.com/Lightning-AI/lightning/pull/19448))
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/_graveyard/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/_graveyard/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/_graveyard/tpu.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/_graveyard/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/accelerator.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/cpu.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/cpu.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/cuda.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/cuda.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/mps.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/mps.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/registry.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/accelerators/xla.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/accelerators/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/cli.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/connector.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/connector.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/fabric.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/fabric.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,27 +49,27 @@
     DataParallelStrategy,
     DeepSpeedStrategy,
     FSDPStrategy,
     SingleDeviceStrategy,
     Strategy,
     XLAStrategy,
 )
-from lightning.fabric.strategies.fsdp import _has_meta_device_parameters
 from lightning.fabric.strategies.launchers import _MultiProcessingLauncher, _XLALauncher
 from lightning.fabric.strategies.strategy import TBroadcast, _Sharded
 from lightning.fabric.utilities import move_data_to_device
 from lightning.fabric.utilities.apply_func import convert_tensors_to_scalars, convert_to_tensors
 from lightning.fabric.utilities.data import (
     _auto_add_worker_init_fn,
     _replace_dunder_methods,
     _update_dataloader,
     has_iterable_dataset,
 )
 from lightning.fabric.utilities.device_dtype_mixin import _update_properties
 from lightning.fabric.utilities.distributed import DistributedSamplerWrapper, _InfiniteBarrier
+from lightning.fabric.utilities.init import _has_meta_device_parameters_or_buffers
 from lightning.fabric.utilities.rank_zero import rank_zero_deprecation, rank_zero_warn
 from lightning.fabric.utilities.registry import _load_external_callbacks
 from lightning.fabric.utilities.seed import seed_everything
 from lightning.fabric.utilities.types import ReduceOp
 from lightning.fabric.utilities.warnings import PossibleUserWarning
 from lightning.fabric.wrappers import (
     _FabricDataLoader,
@@ -1012,15 +1012,15 @@
         if isinstance(module, _FabricModule):
             raise ValueError("A model should be passed only once to the `setup` method.")
 
         if any(isinstance(opt, _FabricOptimizer) for opt in optimizers):
             raise ValueError("An optimizer should be passed only once to the `setup` method.")
 
         if isinstance(self._strategy, FSDPStrategy) and any(
-            _has_meta_device_parameters(optimizer) for optimizer in optimizers
+            _has_meta_device_parameters_or_buffers(optimizer) for optimizer in optimizers
         ):
             raise RuntimeError(
                 "The optimizer has references to the model's meta-device parameters. Materializing them is"
                 " is currently not supported unless you to set up the model and optimizer(s) separately."
                 " Create and set up the model first through `model = fabric.setup_module(model)`. Then create the"
                 " optimizer and set it up: `optimizer = fabric.setup_optimizers(optimizer)`."
             )
@@ -1040,15 +1040,15 @@
 
         if not optimizers:
             raise ValueError("`setup_optimizers` requires at least one optimizer as input.")
 
         if any(isinstance(opt, _FabricOptimizer) for opt in optimizers):
             raise ValueError("An optimizer should be passed only once to the `setup_optimizers` method.")
 
-        if any(_has_meta_device_parameters(optimizer) for optimizer in optimizers):
+        if any(_has_meta_device_parameters_or_buffers(optimizer) for optimizer in optimizers):
             raise RuntimeError(
                 "The optimizer has references to the model's meta-device parameters. Materializing them is"
                 " is currently not supported. Create the optimizer after setting up the model, then call"
                 " `fabric.setup_optimizers(optimizer)`."
             )
 
     def _validate_setup_dataloaders(self, dataloaders: Sequence[DataLoader]) -> None:
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/loggers/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/loggers/csv_logs.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/loggers/csv_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/loggers/logger.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/loggers/tensorboard.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/collectives/collective.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/collectives/collective.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/collectives/single_device.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/collectives/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/collectives/torch_collective.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/collectives/torch_collective.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/cluster_environment.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/cluster_environment.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/kubeflow.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/kubeflow.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/lightning.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/lightning.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/lsf.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/lsf.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/mpi.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/mpi.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/slurm.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/slurm.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/torchelastic.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/torchelastic.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/environments/xla.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/environments/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/io/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/io/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/io/checkpoint_io.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/io/checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/io/torch_io.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/io/torch_io.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/io/xla.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/io/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/amp.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/amp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/bitsandbytes.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/bitsandbytes.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/deepspeed.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/double.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/double.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/fsdp.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/half.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/half.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/precision.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/transformer_engine.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/transformer_engine.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/utils.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/plugins/precision/xla.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/plugins/precision/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 import sys
 
 from lightning.fabric.strategies.ddp import DDPStrategy  # noqa: F401
 from lightning.fabric.strategies.deepspeed import DeepSpeedStrategy  # noqa: F401
 from lightning.fabric.strategies.dp import DataParallelStrategy  # noqa: F401
 from lightning.fabric.strategies.fsdp import FSDPStrategy  # noqa: F401
+from lightning.fabric.strategies.model_parallel import ModelParallelStrategy  # noqa: F401
 from lightning.fabric.strategies.parallel import ParallelStrategy  # noqa: F401
 from lightning.fabric.strategies.registry import _StrategyRegistry
 from lightning.fabric.strategies.single_device import SingleDeviceStrategy  # noqa: F401
 from lightning.fabric.strategies.single_xla import SingleDeviceXLAStrategy  # noqa: F401
 from lightning.fabric.strategies.strategy import Strategy
 from lightning.fabric.strategies.xla import XLAStrategy  # noqa: F401
 from lightning.fabric.strategies.xla_fsdp import XLAFSDPStrategy  # noqa: F401
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/ddp.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/ddp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/deepspeed.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/dp.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/dp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/fsdp.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/fsdp.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     Union,
 )
 
 import torch
 from lightning_utilities.core.imports import RequirementCache
 from lightning_utilities.core.rank_zero import rank_zero_only as utils_rank_zero_only
 from torch import Tensor
-from torch.nn import Module, Parameter
+from torch.nn import Module
 from torch.optim import Optimizer
 from typing_extensions import TypeGuard, override
 
 from lightning.fabric.accelerators import Accelerator
 from lightning.fabric.plugins import CheckpointIO, ClusterEnvironment, Precision
 from lightning.fabric.plugins.collectives.torch_collective import default_pg_timeout
 from lightning.fabric.plugins.precision.fsdp import FSDPPrecision
@@ -63,15 +63,15 @@
 )
 from lightning.fabric.utilities.distributed import group as _group
 from lightning.fabric.utilities.imports import (
     _TORCH_GREATER_EQUAL_2_1,
     _TORCH_GREATER_EQUAL_2_2,
     _TORCH_GREATER_EQUAL_2_3,
 )
-from lightning.fabric.utilities.init import _EmptyInit
+from lightning.fabric.utilities.init import _EmptyInit, _has_meta_device_parameters_or_buffers
 from lightning.fabric.utilities.load import _METADATA_FILENAME, _lazy_load, _materialize_tensors, _move_state_into
 from lightning.fabric.utilities.rank_zero import rank_zero_deprecation, rank_zero_only, rank_zero_warn
 from lightning.fabric.utilities.seed import reset_seed
 from lightning.fabric.utilities.types import _PATH, _Stateful
 
 if TYPE_CHECKING:
     from torch.distributed.fsdp.fully_sharded_data_parallel import CPUOffload, MixedPrecision, ShardingStrategy
@@ -267,15 +267,15 @@
     def setup_module(self, module: Module) -> Module:
         """Wraps the model into a :class:`~torch.distributed.fsdp.fully_sharded_data_parallel.FullyShardedDataParallel`
         module."""
         from torch.distributed.fsdp import FullyShardedDataParallel
 
         if any(isinstance(mod, FullyShardedDataParallel) for mod in module.modules()):
             # The user has wrapped their submodules manually, don't apply the auto wrap policy.
-            if _has_meta_device_parameters(module):
+            if _has_meta_device_parameters_or_buffers(module):
                 rank_zero_warn(
                     "The model is already wrapped in `FSDP` but there are still parameters on the meta device."
                 )
             if "auto_wrap_policy" in self._fsdp_kwargs:
                 rank_zero_warn(
                     "A FSDP `auto_wrap_policy` is set, but the model is already wrapped. The policy will be ignored."
                 )
@@ -389,15 +389,15 @@
         """Clip gradients by norm."""
         from torch.distributed.fsdp.fully_sharded_data_parallel import FullyShardedDataParallel
 
         if not isinstance(module, FullyShardedDataParallel):
             # the root must be wrapped
             raise TypeError(
                 "Gradient clipping with FSDP is only possible if the module passed to"
-                f" `{self.__class__.__name__}.clip_gradients_norm` is wrapped in `FullyShardedDataParallel`."
+                f" `{type(self).__name__}.clip_gradients_norm` is wrapped in `FullyShardedDataParallel`."
                 f" Got: {module.__class__.__name__}."
             )
         self.precision.unscale_gradients(optimizer)
         return module.clip_grad_norm_(max_norm=max_norm, norm_type=norm_type)
 
     @override
     def save_checkpoint(
@@ -502,41 +502,37 @@
     @override
     def load_checkpoint(
         self,
         path: _PATH,
         state: Optional[Union[Module, Optimizer, Dict[str, Union[Module, Optimizer, Any]]]] = None,
         strict: bool = True,
     ) -> Dict[str, Any]:
-        """Load the contents from a checkpoint and restore the state of the given objects.
-
-        The strategy currently only supports saving and loading sharded checkpoints which are stored in form of a
-        directory of multiple files rather than a single file.
-
-        """
+        """Load the contents from a checkpoint and restore the state of the given objects."""
         if not state:
             raise ValueError(
                 f"Got FSDPStrategy.load_checkpoint(..., state={state!r}) but a state with at least "
                 f" a model instance to reload is required. Pass it in like so:"
                 " FSDPStrategy.load_checkpoint(..., state={'model': model, ...})"
             )
         # broadcast the path from rank 0 to ensure all the states are loaded from a common path
         path = Path(self.broadcast(path))
 
         if isinstance(state, Module):
+            from lightning.fabric.strategies.model_parallel import _load_raw_module_state_from_path
+
             _load_raw_module_state_from_path(path, module=state, world_size=self.world_size, strict=strict)
             return {}
 
         if isinstance(state, Optimizer):
             raise NotImplementedError(
                 "Loading a single optimizer object from a checkpoint is not supported yet with the FSDP strategy."
             )
 
         from torch.distributed.checkpoint.optimizer import load_sharded_optimizer_state_dict
         from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
-        from torch.distributed.fsdp import OptimStateKeyType
 
         modules = {key: module for key, module in state.items() if _has_fsdp_modules(module)}
         if len(modules) == 0:
             raise ValueError(
                 "Could not find a FSDP model in the provided checkpoint state. Please provide the model as"
                 " part of the state like so: `load_checkpoint(..., state={'model': model, ...})`. Make sure"
                 " you set up the model (and optimizers if any) through the strategy before loading the checkpoint."
@@ -588,35 +584,34 @@
                 state[key] = metadata.pop(key)
 
             # return the remaining metadata that wasn't requested as part of `state`
             return metadata
 
         if _is_full_checkpoint(path):
             checkpoint = _lazy_load(path)
+
+            from lightning.fabric.strategies.model_parallel import (
+                _load_raw_module_state,
+                _rekey_optimizer_state_if_needed,
+            )
+
             _load_raw_module_state(checkpoint.pop(module_key), module=module, world_size=self.world_size, strict=strict)
 
             if isinstance(state, Module):
                 return {}
 
             # Materialize lazy tensors if there are any left in the checkpoint
             # The `torch.Optimizer.load_state_dict` method can't load lazy tensors because of deepcopy pickle issues
             checkpoint = _materialize_tensors(checkpoint)
 
             # Load optimizer states
             for optim_key, optim in optimizers.items():
                 # rank0_only should be false because we need to load the optimizer state on all ranks
                 with _get_full_state_dict_context(module, world_size=self.world_size, rank0_only=False):
-                    temp_state_dict = checkpoint.pop(optim_key)
-
-                    # Handling the case where the optimizer state is saved from a normal optimizer
-                    if isinstance(list(temp_state_dict["state"].keys())[0], int):
-                        temp_state_dict = FSDP.rekey_optim_state_dict(
-                            temp_state_dict, OptimStateKeyType.PARAM_NAME, module
-                        )
-
+                    temp_state_dict = _rekey_optimizer_state_if_needed(checkpoint.pop(optim_key), module)
                     optim_state_dict = FSDP.optim_state_dict_to_load(
                         optim_state_dict=temp_state_dict,
                         model=module,
                         optim=optim,
                     )
                     optim.load_state_dict(optim_state_dict)
 
@@ -751,15 +746,15 @@
             return nullcontext()
         from torch.distributed.fsdp.fully_sharded_data_parallel import FullyShardedDataParallel
 
         if not isinstance(module, FullyShardedDataParallel):
             # the root must be wrapped
             raise TypeError(
                 "Blocking backward sync is only possible if the module passed to"
-                f" `{self.__class__.__name__}.no_backward_sync` is wrapped in `FullyShardedDataParallel`."
+                f" `{type(self).__name__}.no_backward_sync` is wrapped in `FullyShardedDataParallel`."
                 f" Got: {module.__class__.__name__}."
             )
         return module.no_sync()
 
 
 def _init_cpu_offload(cpu_offload: Optional[Union[bool, "CPUOffload"]]) -> "CPUOffload":
     from torch.distributed.fsdp import CPUOffload
@@ -844,46 +839,14 @@
 
 def _has_fsdp_modules(module: object) -> TypeGuard[Module]:
     from torch.distributed.fsdp import FullyShardedDataParallel
 
     return isinstance(module, Module) and any(isinstance(m, FullyShardedDataParallel) for m in module.modules())
 
 
-def _load_raw_module_state_from_path(path: Path, module: Module, world_size: int, strict: bool = True) -> None:
-    """Loads the state dict from a file path into the FSDP module."""
-    if not _is_full_checkpoint(path):
-        raise ValueError(
-            "Failed to load checkpoint directly into the model. The given path must be a single file containing the"
-            f" full state dict: {path}"
-        )
-    # Use `lazy_load` instead of `torch.load` here to avoid storing a copy of the full checkpoint per rank
-    _load_raw_module_state(state_dict=_lazy_load(path), module=module, world_size=world_size, strict=strict)
-
-
-def _load_raw_module_state(state_dict: Dict[str, Any], module: Module, world_size: int, strict: bool = True) -> None:
-    """Loads the state dict into the module by gathering all weights first and then and writing back to each shard."""
-    from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
-
-    if not isinstance(module, FSDP):
-        module.load_state_dict(state_dict, strict=strict)
-    else:
-        with _get_full_state_dict_context(module, world_size=world_size, rank0_only=False):
-            module.load_state_dict(state_dict, strict=strict)
-
-
-def _has_meta_device_parameters(obj: Union[Module, Optimizer]) -> bool:
-    if isinstance(obj, Optimizer):
-        return any(
-            t.is_meta for param_group in obj.param_groups for t in param_group["params"] if isinstance(t, Parameter)
-        )
-    if isinstance(obj, Module):
-        return any(t.is_meta for t in obj.parameters())
-    raise TypeError(f"Expected `torch.nn.Module` or `torch.optim.Optimizer`, got: {type(obj).__name__}")
-
-
 def _move_torchmetrics_to_device(module: torch.nn.Module, device: torch.device) -> None:
     # FSDP doesn't move modules without parameters (e.g. Metrics) to the device
     # https://github.com/pytorch/pytorch/issues/113113
     if not RequirementCache("torchmetrics"):
         return
 
     from torchmetrics import Metric
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/launchers/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/launchers/launcher.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/launchers/multiprocessing.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/launchers/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/launchers/subprocess_script.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/launchers/subprocess_script.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/launchers/xla.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/launchers/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/parallel.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/registry.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/single_device.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/single_xla.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/single_xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/strategy.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/xla.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/strategies/xla_fsdp.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/strategies/xla_fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/apply_func.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/apply_func.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/cloud_io.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/cloud_io.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/consolidate_checkpoint.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/consolidate_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/data.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/data.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/device_dtype_mixin.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/device_dtype_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/device_parser.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/device_parser.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/distributed.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/enums.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/exceptions.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/imports.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/imports.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 # There are two types of interactive mode we detect
 # 1. The interactive Python shell: https://stackoverflow.com/a/64523765
 # 2. The inspection mode via `python -i`: https://stackoverflow.com/a/6879085/1162383
 _IS_INTERACTIVE = hasattr(sys, "ps1") or bool(sys.flags.interactive)
 
 _TORCH_GREATER_EQUAL_2_1 = compare_version("torch", operator.ge, "2.1.0")
 _TORCH_GREATER_EQUAL_2_2 = compare_version("torch", operator.ge, "2.2.0")
-_TORCH_GREATER_EQUAL_2_3 = compare_version("torch", operator.ge, "2.3.0", use_base_version=True)
+_TORCH_GREATER_EQUAL_2_3 = compare_version("torch", operator.ge, "2.3.0")
+_TORCH_GREATER_EQUAL_2_4 = compare_version("torch", operator.ge, "2.4.0", use_base_version=True)
+
 _TORCH_EQUAL_2_0 = compare_version("torch", operator.ge, "2.0.0") and not _TORCH_GREATER_EQUAL_2_1
 
 _PYTHON_GREATER_EQUAL_3_8_0 = (sys.version_info.major, sys.version_info.minor) >= (3, 8)
 _PYTHON_GREATER_EQUAL_3_10_0 = (sys.version_info.major, sys.version_info.minor) >= (3, 10)
 
 _UTILITIES_GREATER_EQUAL_0_10 = compare_version("lightning_utilities", operator.ge, "0.10.0")
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/load.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/load.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/logger.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/optimizer.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/optimizer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/rank_zero.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/rank_zero.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/registry.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/seed.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/seed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/spike.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/spike.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/testing/_runif.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/testing/_runif.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/throughput.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/throughput.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/types.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/utilities/warnings.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/fabric/wrappers.py` & `lightning-2.3.0.dev20240519/src/lightning/fabric/wrappers.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import inspect
 from copy import deepcopy
 from functools import partial, wraps
+from types import MethodType
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     Iterator,
     List,
@@ -119,14 +120,15 @@
                 on this wrapper should pass through to the original module.
 
         """
         super().__init__()
         self._forward_module = forward_module
         self._original_module = original_module or forward_module
         self._strategy = strategy
+        self._forward_methods = set(_LIGHTNING_MODULE_STEP_METHODS)
         self._fabric_module_initialized = True
 
     @property
     def module(self) -> nn.Module:
         return self._original_module or self._forward_module
 
     @override
@@ -161,14 +163,28 @@
 
     @override
     def load_state_dict(  # type: ignore[override]
         self, state_dict: Mapping[str, Any], strict: bool = True, **kwargs: Any
     ) -> _IncompatibleKeys:
         return self._original_module.load_state_dict(state_dict=state_dict, strict=strict, **kwargs)
 
+    def mark_forward_method(self, method: Union[MethodType, str]) -> None:
+        """Mark a method as a 'forward' method to prevent it bypassing the strategy wrapper (e.g., DDP)."""
+        if not isinstance(method, (MethodType, str)):
+            raise TypeError(f"Expected a method or a string, but got: {type(method).__name__}")
+        name = method if isinstance(method, str) else method.__name__
+        if name == "forward":
+            raise ValueError("You cannot mark the forward method itself as a forward method.")
+        if not isinstance(getattr(self._original_module, name, None), MethodType):
+            raise AttributeError(
+                f"You marked '{name}' as a forward method, but `{type(self._original_module).__name__}.{name}` does not"
+                f" exist or is not a method."
+            )
+        self._forward_methods.add(name)
+
     def _redirection_through_forward(self, method_name: str) -> Callable:
         assert method_name != "forward"
         original_forward = self._original_module.forward
 
         def wrapped_forward(*args: Any, **kwargs: Any) -> Any:
             # Unpatch ourselves immediately before calling the method `method_name`
             # because itself may want to call the real `forward`
@@ -203,16 +219,16 @@
                 handles.append(module.register_forward_hook(hook))
 
             output = method(*args, **kwargs)
 
             if module_called:
                 raise RuntimeError(
                     f"You are calling the method `{type(self._original_module).__name__}.{name}()` from outside the"
-                    " model. This will bypass the wrapper from the strategy and result in incorrect behavior in"
-                    " `.backward()`. You should pass your inputs through `forward()`.",
+                    " model. To avoid issues with the currently selected strategy, explicitly mark it as a"
+                    f" forward method with `fabric_model.mark_forward_method({name!r})` after `fabric.setup()`."
                 )
             for handle in handles:
                 handle.remove()
             return output
 
         return _wrapped_method
 
@@ -227,16 +243,20 @@
         )
         hook = partial(_backward_hook, (strategy_requires or precision_requires))
         tensor.register_hook(hook)
         return tensor
 
     @override
     def __getattr__(self, item: Any) -> Any:
-        if item in _LIGHTNING_MODULE_STEP_METHODS and self._forward_module != self._original_module:
-            # Special support for `LightningModule`, to prevent bypassing DDP's forward
+        if (
+            item != "_forward_methods"
+            and item in self._forward_methods
+            and self._forward_module != self._original_module
+        ):
+            # Special support for methods marked by `mark_forward_method` to prevent bypassing DDP's forward
             return self._redirection_through_forward(item)
 
         try:
             # __getattr__ gets called as a last resort if the attribute does not exist
             # call nn.Module's implementation first
             return super().__getattr__(item)
         except AttributeError:
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/CHANGELOG.md` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/_graveyard/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/_graveyard/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/_graveyard/_torchmetrics.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/_graveyard/_torchmetrics.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/_graveyard/hpu.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/_graveyard/hpu.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/_graveyard/precision.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/_graveyard/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/_graveyard/tpu.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/_graveyard/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/accelerators/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/accelerators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/accelerators/accelerator.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/accelerators/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/accelerators/cpu.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/accelerators/cpu.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/accelerators/cuda.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/accelerators/cuda.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/accelerators/mps.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/accelerators/mps.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/accelerators/xla.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/accelerators/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/batch_size_finder.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/batch_size_finder.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/callback.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/device_stats_monitor.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/device_stats_monitor.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/early_stopping.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/finetuning.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/finetuning.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/gradient_accumulation_scheduler.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/gradient_accumulation_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/lambda_function.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/lr_finder.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/lr_finder.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/lr_monitor.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/lr_monitor.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/model_checkpoint.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/model_summary.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/model_summary.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/on_exception_checkpoint.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/on_exception_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/prediction_writer.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/prediction_writer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/progress/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/progress/progress_bar.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/progress/progress_bar.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/progress/rich_progress.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/progress/rich_progress.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/progress/tqdm_progress.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/progress/tqdm_progress.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/pruning.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/pruning.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/rich_model_summary.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/rich_model_summary.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/spike.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/spike.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/stochastic_weight_avg.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/stochastic_weight_avg.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/throughput_monitor.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/throughput_monitor.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/callbacks/timer.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/callbacks/timer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/cli.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/core/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/core/datamodule.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/core/datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/core/hooks.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/core/hooks.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/core/mixins/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/core/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/core/mixins/hparams_mixin.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/core/mixins/hparams_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/core/module.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/core/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import logging
 import numbers
 import weakref
 from contextlib import contextmanager
 from pathlib import Path
 from typing import (
     IO,
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Generator,
     List,
     Literal,
     Mapping,
@@ -72,14 +73,17 @@
     _METRIC,
     STEP_OUTPUT,
     LRSchedulerPLType,
     LRSchedulerTypeUnion,
     OptimizerLRScheduler,
 )
 
+if TYPE_CHECKING:
+    from torch.distributed.device_mesh import DeviceMesh
+
 _ONNX_AVAILABLE = RequirementCache("onnx")
 
 warning_cache = WarningCache()
 log = logging.getLogger(__name__)
 
 MODULE_OPTIMIZERS = Union[
     Optimizer, LightningOptimizer, _FabricOptimizer, List[Optimizer], List[LightningOptimizer], List[_FabricOptimizer]
@@ -106,14 +110,15 @@
             "local_rank",
             "logger",
             "loggers",
             "automatic_optimization",
             "trainer",
             "fabric",
             "strict_loading",
+            "device_mesh",
         ]
         + _DeviceDtypeModuleMixin.__jit_unused_properties__
         + HyperparametersMixin.__jit_unused_properties__
     )
     _jit_is_scripting = False
 
     CHECKPOINT_HYPER_PARAMS_KEY = "hyper_parameters"
@@ -138,14 +143,17 @@
         self._register_sharded_tensor_state_dict_hooks_if_available()
         self._compiler_ctx: Optional[Dict[str, Any]] = None
 
         # attributes only used when using fabric
         self._fabric: Optional["lf.Fabric"] = None
         self._fabric_optimizers: List[_FabricOptimizer] = []
 
+        # access to device mesh in `conigure_model()` hook
+        self._device_mesh: Optional["DeviceMesh"] = None
+
     @overload
     def optimizers(
         self, use_pl_optimizer: Literal[True] = True
     ) -> Union[LightningOptimizer, List[LightningOptimizer]]: ...
 
     @overload
     def optimizers(self, use_pl_optimizer: Literal[False]) -> Union[Optimizer, List[Optimizer]]: ...
@@ -315,14 +323,20 @@
         """Reference to the list of loggers in the Trainer."""
         if self._fabric is not None:
             return self._fabric.loggers
         if self._trainer is not None:
             return self._trainer.loggers
         return []
 
+    @property
+    def device_mesh(self) -> Optional["DeviceMesh"]:
+        """Strategies like ``ModelParallelStrategy`` will create a device mesh that can be accessed in the
+        :meth:`~lightning.pytorch.core.hooks.ModelHooks.configure_model` hook to parallelize the LightningModule."""
+        return self._device_mesh
+
     def _call_batch_hook(self, hook_name: str, *args: Any) -> Any:
         trainer = self._trainer
         if trainer:
             datahook_selector = trainer._data_connector._datahook_selector
             assert datahook_selector is not None
             obj = datahook_selector.get_instance(hook_name)
             if isinstance(obj, self.__class__):
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/core/optimizer.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/core/optimizer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/core/saving.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/core/saving.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/demos/boring_classes.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/demos/boring_classes.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/demos/mnist_datamodule.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/demos/mnist_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/demos/transformer.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/demos/transformer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/comet.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/comet.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/csv_logs.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/csv_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/logger.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/mlflow.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/mlflow.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/neptune.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/neptune.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/tensorboard.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/utilities.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/utilities.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loggers/wandb.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loggers/wandb.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/evaluation_loop.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/evaluation_loop.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/fetchers.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/fetchers.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/fit_loop.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/fit_loop.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/loop.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/loop.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/optimization/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/optimization/automatic.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/optimization/automatic.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/optimization/closure.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/optimization/closure.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/optimization/manual.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/optimization/manual.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/prediction_loop.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/prediction_loop.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/progress.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/progress.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/training_epoch_loop.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/training_epoch_loop.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/loops/utilities.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/loops/utilities.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/overrides/distributed.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/overrides/distributed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/environments/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/io/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/io/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/io/async_plugin.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/io/async_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/io/checkpoint_plugin.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/io/checkpoint_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/io/torch_plugin.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/io/torch_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/io/wrapper.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/io/wrapper.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/io/xla_plugin.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/io/xla_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/layer_sync.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/layer_sync.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/amp.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/amp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/bitsandbytes.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/bitsandbytes.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/deepspeed.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/double.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/double.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/fsdp.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/half.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/half.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/precision.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/transformer_engine.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/transformer_engine.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/plugins/precision/xla.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/plugins/precision/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/advanced.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/advanced.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/base.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/base.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/profiler.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/profiler.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/pytorch.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/pytorch.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/simple.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/simple.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/profilers/xla.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/profilers/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/serve/servable_module.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/serve/servable_module.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/serve/servable_module_validator.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/serve/servable_module_validator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 import sys
 
 from lightning.fabric.strategies.registry import _StrategyRegistry
 from lightning.fabric.utilities.registry import _register_classes
 from lightning.pytorch.strategies.ddp import DDPStrategy
 from lightning.pytorch.strategies.deepspeed import DeepSpeedStrategy
 from lightning.pytorch.strategies.fsdp import FSDPStrategy
+from lightning.pytorch.strategies.model_parallel import ModelParallelStrategy
 from lightning.pytorch.strategies.parallel import ParallelStrategy
 from lightning.pytorch.strategies.single_device import SingleDeviceStrategy
 from lightning.pytorch.strategies.single_xla import SingleDeviceXLAStrategy  # noqa: F401
 from lightning.pytorch.strategies.strategy import Strategy
 from lightning.pytorch.strategies.xla import XLAStrategy  # noqa: F401
 
 StrategyRegistry = _StrategyRegistry()
 _register_classes(StrategyRegistry, "register_strategies", sys.modules[__name__], Strategy)
 
 __all__ = [
     "DDPStrategy",
     "DeepSpeedStrategy",
     "FSDPStrategy",
+    "ModelParallelStrategy",
     "ParallelStrategy",
     "SingleDeviceStrategy",
     "Strategy",
 ]
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/ddp.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/ddp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/deepspeed.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/fsdp.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/fsdp.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,33 +33,32 @@
     _METADATA_FILENAME,
     _activation_checkpointing_kwargs,
     _auto_wrap_policy_kwargs,
     _distributed_checkpoint_load,
     _distributed_checkpoint_save,
     _get_full_state_dict_context,
     _get_sharded_state_dict_context,
-    _has_meta_device_parameters,
     _init_cpu_offload,
     _init_sharding_strategy,
     _is_full_checkpoint,
     _is_sharded_checkpoint,
-    _load_raw_module_state,
     _move_torchmetrics_to_device,
     _optimizer_has_flat_params,
     _setup_activation_checkpointing,
 )
+from lightning.fabric.strategies.model_parallel import _load_raw_module_state
 from lightning.fabric.utilities.distributed import (
     _distributed_is_initialized,
     _get_default_process_group_backend_for_device,
     _init_dist_connection,
     _sync_ddp_if_available,
 )
 from lightning.fabric.utilities.distributed import group as _group
 from lightning.fabric.utilities.imports import _TORCH_GREATER_EQUAL_2_1
-from lightning.fabric.utilities.init import _EmptyInit
+from lightning.fabric.utilities.init import _EmptyInit, _has_meta_device_parameters_or_buffers
 from lightning.fabric.utilities.load import _lazy_load, _materialize_tensors
 from lightning.fabric.utilities.optimizer import _optimizers_to_device
 from lightning.fabric.utilities.seed import reset_seed
 from lightning.fabric.utilities.types import _PATH, ReduceOp
 from lightning.pytorch.core.optimizer import LightningOptimizer
 from lightning.pytorch.plugins.precision import Precision
 from lightning.pytorch.plugins.precision.fsdp import FSDPPrecision
@@ -265,15 +264,15 @@
     @override
     def _setup_model(self, model: Module) -> Module:
         """Wraps the model into a :class:`~torch.distributed.fsdp.fully_sharded_data_parallel.FullyShardedDataParallel`
         module."""
         from torch.distributed.fsdp import FullyShardedDataParallel
 
         if any(isinstance(mod, FullyShardedDataParallel) for mod in model.modules()):
-            if _has_meta_device_parameters(model):
+            if _has_meta_device_parameters_or_buffers(model):
                 rank_zero_warn(
                     "The model is already wrapped in `FSDP` but there are still parameters on the meta device."
                 )
             if "auto_wrap_policy" in self.kwargs:
                 # The user has wrapped their submodules manually, don't apply the auto wrap policy.
                 rank_zero_warn(
                     "A FSDP `auto_wrap_policy` is set, but the model is already wrapped. The policy will be ignored."
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/launchers/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/launchers/launcher.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/launchers/multiprocessing.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/launchers/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/launchers/subprocess_script.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/launchers/subprocess_script.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/launchers/xla.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/launchers/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/parallel.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/single_device.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/single_xla.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/single_xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/strategy.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/strategies/xla.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/strategies/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/call.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/call.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/configuration_validator.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/configuration_validator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/accelerator_connector.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/accelerator_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     XLAPrecision,
 )
 from lightning.pytorch.plugins.layer_sync import LayerSync, TorchSyncBatchNorm
 from lightning.pytorch.strategies import (
     DDPStrategy,
     DeepSpeedStrategy,
     FSDPStrategy,
+    ModelParallelStrategy,
     ParallelStrategy,
     SingleDeviceStrategy,
     SingleDeviceXLAStrategy,
     Strategy,
     StrategyRegistry,
     XLAStrategy,
 )
@@ -596,14 +597,15 @@
 
     @property
     def is_distributed(self) -> bool:
         distributed_strategies = [
             DDPStrategy,
             FSDPStrategy,
             DeepSpeedStrategy,
+            ModelParallelStrategy,
             XLAStrategy,
         ]
         if _habana_available_and_importable():
             from lightning_habana import HPUParallelStrategy
 
             distributed_strategies.append(HPUParallelStrategy)
         if isinstance(self.strategy, tuple(distributed_strategies)):
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/callback_connector.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/callback_connector.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/checkpoint_connector.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/checkpoint_connector.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/data_connector.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/data_connector.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/logger_connector/fx_validator.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/logger_connector/fx_validator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/logger_connector/logger_connector.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/logger_connector/logger_connector.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/logger_connector/result.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/logger_connector/result.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/connectors/signal_connector.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/connectors/signal_connector.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/setup.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/states.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/states.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/trainer/trainer.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/tuner/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/tuner/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/tuner/batch_size_scaling.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/tuner/batch_size_scaling.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/tuner/lr_finder.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/tuner/lr_finder.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/tuner/tuning.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/tuner/tuning.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/_pytree.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/_pytree.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/argparse.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/argparse.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/combined_loader.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/combined_loader.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/compile.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/compile.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/consolidate_checkpoint.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/consolidate_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/data.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/data.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/deepspeed.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/enums.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/exceptions.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/grads.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/grads.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/imports.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/memory.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/memory.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/migration/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/migration/migration.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/migration/migration.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/migration/utils.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/migration/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/model_helpers.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/model_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/model_summary/__init__.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/model_summary/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/model_summary/model_summary.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/model_summary/model_summary.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/model_summary/model_summary_deepspeed.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/model_summary/model_summary_deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/parameter_tying.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/parameter_tying.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/parsing.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/parsing.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/rank_zero.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/rank_zero.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/seed.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/seed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/signature_utils.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/signature_utils.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/testing/_runif.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/testing/_runif.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/types.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/upgrade_checkpoint.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/upgrade_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/pytorch/utilities/warnings.py` & `lightning-2.3.0.dev20240519/src/lightning/pytorch/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/store/store.py` & `lightning-2.3.0.dev20240519/src/lightning/store/store.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning/store/utils.py` & `lightning-2.3.0.dev20240519/src/lightning/store/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240505/src/lightning.egg-info/PKG-INFO` & `lightning-2.3.0.dev20240519/src/lightning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning
-Version: 2.3.0.dev20240505
+Version: 2.3.0.dev20240519
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -23,42 +23,42 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: app-components
-Provides-Extra: app-cloud
+Provides-Extra: fabric-examples
+Provides-Extra: fabric-strategies
+Provides-Extra: fabric-test
+Provides-Extra: store-test
 Provides-Extra: app-ui
+Provides-Extra: app-cloud
 Provides-Extra: app-test
-Provides-Extra: store-test
+Provides-Extra: app-components
+Provides-Extra: pytorch-examples
 Provides-Extra: pytorch-strategies
-Provides-Extra: pytorch-test
 Provides-Extra: pytorch-extra
-Provides-Extra: pytorch-examples
-Provides-Extra: fabric-strategies
-Provides-Extra: fabric-test
-Provides-Extra: fabric-examples
+Provides-Extra: pytorch-test
 Provides-Extra: fabric-all
 Provides-Extra: fabric-dev
 Provides-Extra: pytorch-all
 Provides-Extra: pytorch-dev
 Provides-Extra: app-extra
 Provides-Extra: app-all
 Provides-Extra: app-dev
-Provides-Extra: components
-Provides-Extra: cloud
+Provides-Extra: data
+Provides-Extra: examples
+Provides-Extra: strategies
+Provides-Extra: test
 Provides-Extra: ui
+Provides-Extra: cloud
 Provides-Extra: app
-Provides-Extra: test
-Provides-Extra: strategies
+Provides-Extra: components
 Provides-Extra: extra
-Provides-Extra: examples
-Provides-Extra: data
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: store
 License-File: LICENSE
 
 <div align="center">
 
@@ -74,15 +74,15 @@
 ______________________________________________________________________
 
 <p align="center">
   <a href="https://lightning.ai/">Lightning.ai</a> •
   <a href="https://lightning.ai/docs/pytorch/stable/">PyTorch Lightning</a> •
   <a href="https://lightning.ai/docs/fabric/stable/">Fabric</a> •
   <a href="https://lightning.ai/docs/app/stable/">Lightning Apps</a> •
-  <a href="https://pytorch-lightning.readthedocs.io/en/2.3.0.dev20240505">Docs</a> •
+  <a href="https://pytorch-lightning.readthedocs.io/en/2.3.0.dev20240519">Docs</a> •
   <a href="#community">Community</a> •
   <a href="https://lightning.ai/docs/pytorch/stable/generated/CONTRIBUTING.html">Contribute</a> •
 </p>
 
 <!-- DO NOT ADD CONDA DOWNLOADS... README CHANGES MUST BE APPROVED BY EDEN OR WILL -->
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)](https://pypi.org/project/pytorch-lightning/)
@@ -619,15 +619,15 @@
 <details>
   <summary>Current build statuses</summary>
 
 <center>
 
 |       System / PyTorch ver.        | 1.13                                                                                                                                                                                                                            | 2.0                                                                                                                                                                                                                             |                                                                                                               2.1                                                                                                               |
 | :--------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-|        Linux py3.9 \[GPUs\]        |  |  | [![Build Status](https://dev.azure.com/Lightning-AI/lightning/_apis/build/status%2Fpytorch-lightning%20%28GPUs%29?branchName=refs%2Ftags%2F2.3.0.dev20240505)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=24&branchName=master) |
+|        Linux py3.9 \[GPUs\]        |  |  | [![Build Status](https://dev.azure.com/Lightning-AI/lightning/_apis/build/status%2Fpytorch-lightning%20%28GPUs%29?branchName=refs%2Ftags%2F2.3.0.dev20240519)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=24&branchName=master) |
 |        Linux py3.9 \[TPUs\]        |                                                                                                                                                                                                                                 |  [![Test PyTorch - TPU](https://github.com/Lightning-AI/lightning/actions/workflows/tpu-tests.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/tpu-tests.yml)     |      |
 |  Linux (multiple Python versions)  | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 |                 [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                 |
 |   OSX (multiple Python versions)   | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 |                 [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                 |
 | Windows (multiple Python versions) | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 |                 [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                 |
 
 </center>
 </details>
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning.egg-info/SOURCES.txt` & `lightning-2.3.0.dev20240519/src/lightning.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 requirements/pytorch/base.txt
 requirements/pytorch/docs.txt
 requirements/pytorch/examples.txt
 requirements/pytorch/extra.txt
 requirements/pytorch/strategies.txt
 requirements/pytorch/test.txt
 src/version.info
+src/lightning/03b460d403e09cdf43eab937b2d65f81d750629927cf0e82
 src/lightning/__about__.py
 src/lightning/__init__.py
 src/lightning/__main__.py
 src/lightning/__setup__.py
 src/lightning/__version__.py
-src/lightning/c475c1d37e4559adf497c85932243ae1fb375cfdcf0fabf9
 src/lightning/py.typed
 src/lightning/version.info
 src/lightning.egg-info/PKG-INFO
 src/lightning.egg-info/SOURCES.txt
 src/lightning.egg-info/dependency_links.txt
 src/lightning.egg-info/entry_points.txt
 src/lightning.egg-info/not-zip-safe
@@ -353,14 +353,15 @@
 src/lightning/fabric/plugins/precision/utils.py
 src/lightning/fabric/plugins/precision/xla.py
 src/lightning/fabric/strategies/__init__.py
 src/lightning/fabric/strategies/ddp.py
 src/lightning/fabric/strategies/deepspeed.py
 src/lightning/fabric/strategies/dp.py
 src/lightning/fabric/strategies/fsdp.py
+src/lightning/fabric/strategies/model_parallel.py
 src/lightning/fabric/strategies/parallel.py
 src/lightning/fabric/strategies/registry.py
 src/lightning/fabric/strategies/single_device.py
 src/lightning/fabric/strategies/single_xla.py
 src/lightning/fabric/strategies/strategy.py
 src/lightning/fabric/strategies/xla.py
 src/lightning/fabric/strategies/xla_fsdp.py
@@ -497,14 +498,15 @@
 src/lightning/pytorch/serve/__init__.py
 src/lightning/pytorch/serve/servable_module.py
 src/lightning/pytorch/serve/servable_module_validator.py
 src/lightning/pytorch/strategies/__init__.py
 src/lightning/pytorch/strategies/ddp.py
 src/lightning/pytorch/strategies/deepspeed.py
 src/lightning/pytorch/strategies/fsdp.py
+src/lightning/pytorch/strategies/model_parallel.py
 src/lightning/pytorch/strategies/parallel.py
 src/lightning/pytorch/strategies/single_device.py
 src/lightning/pytorch/strategies/single_xla.py
 src/lightning/pytorch/strategies/strategy.py
 src/lightning/pytorch/strategies/xla.py
 src/lightning/pytorch/strategies/launchers/__init__.py
 src/lightning/pytorch/strategies/launchers/launcher.py
```

### Comparing `lightning-2.3.0.dev20240505/src/lightning.egg-info/requires.txt` & `lightning-2.3.0.dev20240519/src/lightning.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 docker<7.0,>=5.0.0
 fastapi<1.0,>=0.92.0
 fsspec[http]<2024.0,>=2022.5.0
 hydra-core<2.0,>=1.0.5
 inquirer<4.0,>=2.10.0
 ipython[all]<9.0
 jsonargparse[signatures]<5.0,>=4.27.7
-lightning-cloud==0.5.68
+lightning-cloud==0.5.69
 lightning-fabric>=1.9.0
 lightning-utilities<1.0,>=0.8.0
 lightning_api_access>=0.0.3
 matplotlib<4.0,>3.1
 omegaconf<3.0,>=2.0.5
 packaging
 psutil<6.0
@@ -66,15 +66,15 @@
 click<9.0
 croniter<1.5.0,>=1.3.0
 dateutils<1.0
 deepdiff<7.0,>=5.7.0
 fastapi<1.0,>=0.92.0
 fsspec[http]<2024.0,>=2022.5.0
 inquirer<4.0,>=2.10.0
-lightning-cloud==0.5.68
+lightning-cloud==0.5.69
 lightning-utilities<1.0,>=0.8.0
 packaging
 psutil<6.0
 pydantic>=1.7.4
 python-multipart<1.0,>=0.0.5
 requests<3.0
 rich<14.0,>=12.3.0
@@ -97,15 +97,15 @@
 croniter<1.5.0,>=1.3.0
 dateutils<1.0
 deepdiff<7.0,>=5.7.0
 docker<7.0,>=5.0.0
 fastapi<1.0,>=0.92.0
 fsspec[http]<2024.0,>=2022.5.0
 inquirer<4.0,>=2.10.0
-lightning-cloud==0.5.68
+lightning-cloud==0.5.69
 lightning-fabric>=1.9.0
 lightning-utilities<1.0,>=0.8.0
 lightning_api_access>=0.0.3
 packaging
 psutil<6.0
 pydantic>=1.7.4
 python-multipart<1.0,>=0.0.5
@@ -146,15 +146,15 @@
 dateutils<1.0
 deepdiff<7.0,>=5.7.0
 docker<7.0,>=5.0.0
 fastapi<1.0,>=0.92.0
 fsspec[http]<2024.0,>=2022.5.0
 httpx==0.25.0
 inquirer<4.0,>=2.10.0
-lightning-cloud==0.5.68
+lightning-cloud==0.5.69
 lightning-fabric>=1.9.0
 lightning-utilities<1.0,>=0.8.0
 lightning_api_access>=0.0.3
 packaging
 pandas
 playwright==1.38.0
 psutil<6.0
@@ -195,15 +195,15 @@
 croniter<1.5.0,>=1.3.0
 dateutils<1.0
 deepdiff<7.0,>=5.7.0
 docker<7.0,>=5.0.0
 fastapi<1.0,>=0.92.0
 fsspec[http]<2024.0,>=2022.5.0
 inquirer<4.0,>=2.10.0
-lightning-cloud==0.5.68
+lightning-cloud==0.5.69
 lightning-fabric>=1.9.0
 lightning-utilities<1.0,>=0.8.0
 lightning_api_access>=0.0.3
 packaging
 psutil<6.0
 pydantic>=1.7.4
 python-multipart<1.0,>=0.0.5
@@ -274,15 +274,15 @@
 fastapi<1.0,>=0.92.0
 fsspec[http]<2024.0,>=2022.5.0
 httpx==0.25.0
 hydra-core<2.0,>=1.0.5
 inquirer<4.0,>=2.10.0
 ipython[all]<9.0
 jsonargparse[signatures]<5.0,>=4.27.7
-lightning-cloud==0.5.68
+lightning-cloud==0.5.69
 lightning-fabric>=1.9.0
 lightning-utilities<1.0,>=0.8.0
 lightning_api_access>=0.0.3
 matplotlib<4.0,>3.1
 omegaconf<3.0,>=2.0.5
 onnx<2.0,>=0.14.0
 onnxruntime<2.0,>=0.15.0
@@ -349,15 +349,15 @@
 deepdiff<7.0,>=5.7.0
 docker<7.0,>=5.0.0
 fastapi<1.0,>=0.92.0
 fsspec[http]<2024.0,>=2022.5.0
 hydra-core<2.0,>=1.0.5
 inquirer<4.0,>=2.10.0
 jsonargparse[signatures]<5.0,>=4.27.7
-lightning-cloud==0.5.68
+lightning-cloud==0.5.69
 lightning-fabric>=1.9.0
 lightning-utilities<1.0,>=0.8.0
 lightning_api_access>=0.0.3
 matplotlib<4.0,>3.1
 omegaconf<3.0,>=2.0.5
 packaging
 psutil<6.0
@@ -522,15 +522,15 @@
 click<9.0
 croniter<1.5.0,>=1.3.0
 dateutils<1.0
 deepdiff<7.0,>=5.7.0
 fastapi<1.0,>=0.92.0
 fsspec[http]<2024.0,>=2022.5.0
 inquirer<4.0,>=2.10.0
-lightning-cloud==0.5.68
+lightning-cloud==0.5.69
 lightning-utilities<1.0,>=0.8.0
 packaging
 psutil<6.0
 pydantic>=1.7.4
 python-multipart<1.0,>=0.0.5
 requests<3.0
 rich<14.0,>=12.3.0
```

