# Comparing `tmp/jupyterlab_server-2.8.2.tar.gz` & `tmp/jupyterlab_server-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_server-2.8.2.tar", last modified: Sat Sep 25 15:45:13 2021, max compression
+gzip compressed data, was "jupyterlab_server-2.9.0.tar", last modified: Mon Dec 13 13:03:09 2021, max compression
```

## Comparing `jupyterlab_server-2.8.2.tar` & `jupyterlab_server-2.9.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.462953 jupyterlab_server-2.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)    30605 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      661 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      529 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2021-09-25 15:45:13.462953 jupyterlab_server-2.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      913 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      606 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/RELEASE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.454953 jupyterlab_server-2.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/docs/autogen_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      234 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.454953 jupyterlab_server-2.8.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.454953 jupyterlab_server-2.8.2/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (121)      273 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/docs/source/api/app.rst
--rw-r--r--   0 runner    (1001) docker     (121)      457 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/docs/source/api/config.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/docs/source/api/handlers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/docs/source/api/process.rst
--rw-r--r--   0 runner    (1001) docker     (121)      516 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/docs/source/api/rest.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3062 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.458953 jupyterlab_server-2.8.2/jupyterlab_server/
--rw-r--r--   0 runner    (1001) docker     (121)      654 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2021-09-25 15:44:55.000000 jupyterlab_server-2.8.2/jupyterlab_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3759 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/app.py
--rw-r--r--   0 runner    (1001) docker     (121)    12279 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/config.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11740 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/licenses_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     9296 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/licenses_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3177 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/listings_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     8293 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/process.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/process_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     4439 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     9784 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/rest-api.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)      451 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/server.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2971 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/settings_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15233 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/settings_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.458953 jupyterlab_server-2.8.2/jupyterlab_server/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/templates/403.html
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.462953 jupyterlab_server-2.8.2/jupyterlab_server/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.462953 jupyterlab_server-2.8.2/jupyterlab_server/tests/app-settings/
--rw-r--r--   0 runner    (1001) docker     (121)      843 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/app-settings/overrides.json
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.450953 jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.450953 jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.462953 jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/apputils-extension/
--rw-r--r--   0 runner    (1001) docker     (121)      850 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/apputils-extension/themes.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.462953 jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/codemirror-extension/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/codemirror-extension/commands.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.462953 jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/shortcuts-extension/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/shortcuts-extension/package.json.orig
--rw-r--r--   0 runner    (1001) docker     (121)    18750 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/shortcuts-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.462953 jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/translation-extension/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/translation-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.462953 jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/unicode-extension/
--rw-r--r--   0 runner    (1001) docker     (121)      962 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/unicode-extension/plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/test_labapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4353 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/test_licenses_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/test_listings_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6352 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/test_settings_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/test_themes_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     7394 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/test_translation_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4611 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/test_workspaces_api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5446 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.462953 jupyterlab_server-2.8.2/jupyterlab_server/tests/workspaces/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/workspaces/foo-2c26.jupyterlab-workspace
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/tests/workspaces/foo-92dd.jupyterlab-workspace
--rw-r--r--   0 runner    (1001) docker     (121)     3070 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/themes_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    22536 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/translation_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/translations_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     7059 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/jupyterlab_server/workspaces_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 15:45:13.458953 jupyterlab_server-2.8.2/jupyterlab_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2021-09-25 15:45:13.000000 jupyterlab_server-2.8.2/jupyterlab_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2021-09-25 15:45:13.000000 jupyterlab_server-2.8.2/jupyterlab_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-25 15:45:13.000000 jupyterlab_server-2.8.2/jupyterlab_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-25 15:44:36.000000 jupyterlab_server-2.8.2/jupyterlab_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      250 2021-09-25 15:45:13.000000 jupyterlab_server-2.8.2/jupyterlab_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-09-25 15:45:13.000000 jupyterlab_server-2.8.2/jupyterlab_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      904 2021-09-25 15:44:55.000000 jupyterlab_server-2.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2021-09-25 15:45:13.462953 jupyterlab_server-2.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-09-25 15:44:23.000000 jupyterlab_server-2.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    33049 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1519 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      529 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2171 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.638177 jupyterlab_server-2.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/docs/autogen_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      234 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.638177 jupyterlab_server-2.9.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.638177 jupyterlab_server-2.9.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/docs/source/api/app.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      457 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/docs/source/api/config.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1732 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/docs/source/api/handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/docs/source/api/process.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/docs/source/api/rest.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3062 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/jupyterlab_server/
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2021-12-13 13:02:49.000000 jupyterlab_server-2.9.0/jupyterlab_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3759 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12279 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12100 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2828 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/licenses_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9296 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/licenses_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3177 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/listings_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8293 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/process.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/process_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4439 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9784 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/rest-api.yml
+-rwxr-xr-x   0 runner    (1001) docker     (121)      451 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/server.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2971 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/settings_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    16141 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/settings_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/jupyterlab_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/templates/403.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/jupyterlab_server/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/jupyterlab_server/tests/app-settings/
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/app-settings/overrides.json
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.634177 jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.634177 jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/apputils-extension/
+-rw-r--r--   0 runner    (1001) docker     (121)      850 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/apputils-extension/themes.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/codemirror-extension/
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/codemirror-extension/commands.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/shortcuts-extension/
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/shortcuts-extension/package.json.orig
+-rw-r--r--   0 runner    (1001) docker     (121)    18750 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/shortcuts-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/translation-extension/
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/translation-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/unicode-extension/
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/unicode-extension/plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1145 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/test_labapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4353 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/test_licenses_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/test_listings_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7361 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/test_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/test_themes_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7394 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/test_translation_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4611 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/test_workspaces_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5446 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/jupyterlab_server/tests/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/workspaces/foo-2c26.jupyterlab-workspace
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/tests/workspaces/foo-92dd.jupyterlab-workspace
+-rw-r--r--   0 runner    (1001) docker     (121)     3070 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/themes_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22536 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/translation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1659 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/translations_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7059 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/jupyterlab_server/workspaces_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/jupyterlab_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2171 2021-12-13 13:03:09.000000 jupyterlab_server-2.9.0/jupyterlab_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2468 2021-12-13 13:03:09.000000 jupyterlab_server-2.9.0/jupyterlab_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-13 13:03:09.000000 jupyterlab_server-2.9.0/jupyterlab_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-13 13:02:31.000000 jupyterlab_server-2.9.0/jupyterlab_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2021-12-13 13:03:09.000000 jupyterlab_server-2.9.0/jupyterlab_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-13 13:03:09.000000 jupyterlab_server-2.9.0/jupyterlab_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2021-12-13 13:02:49.000000 jupyterlab_server-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1306 2021-12-13 13:03:09.642178 jupyterlab_server-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-12-13 13:02:18.000000 jupyterlab_server-2.9.0/setup.py
```

### Comparing `jupyterlab_server-2.8.2/CHANGELOG.md` & `jupyterlab_server-2.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,42 @@
 github_url: 'https://github.com/jupyterlab/jupyterlab_server/blob/master/CHANGELOG.md'
 ---
 
 # Change Log
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 2.9.0
+
+([Full Changelog](https://github.com/jupyterlab/jupyterlab_server/compare/v2.8.2...ea75fc04f9a4d29b9c22c9ec769835df3ba6a0e4))
+
+### Enhancements made
+
+- Add `overrides.d` for settings defaults [#224](https://github.com/jupyterlab/jupyterlab_server/pull/224) ([@bollwyvl](https://github.com/bollwyvl))
+- Add `page_config_hook` [#220](https://github.com/jupyterlab/jupyterlab_server/pull/220) ([@minrk](https://github.com/minrk))
+
+### Maintenance and upkeep improvements
+
+- Enforce labels on PRs [#221](https://github.com/jupyterlab/jupyterlab_server/pull/221) ([@blink1073](https://github.com/blink1073))
+- Fix caching of conda env in CI [#218](https://github.com/jupyterlab/jupyterlab_server/pull/218) ([@blink1073](https://github.com/blink1073))
+- `pyproject.toml`: clarify build system version [#222](https://github.com/jupyterlab/jupyterlab_server/pull/222) ([@adamjstewart](https://github.com/adamjstewart))
+
+### Documentation improvements
+
+- Fix typo in README [#216](https://github.com/jupyterlab/jupyterlab_server/pull/216) ([@Mithil467](https://github.com/Mithil467))
+- Clean up Readme [#215](https://github.com/jupyterlab/jupyterlab_server/pull/215) ([@blink1073](https://github.com/blink1073))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab/jupyterlab_server/graphs/contributors?from=2021-09-25&to=2021-12-13&type=c))
+
+[@adamjstewart](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyterlab_server+involves%3Aadamjstewart+updated%3A2021-09-25..2021-12-13&type=Issues) | [@blink1073](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyterlab_server+involves%3Ablink1073+updated%3A2021-09-25..2021-12-13&type=Issues) | [@bollwyvl](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyterlab_server+involves%3Abollwyvl+updated%3A2021-09-25..2021-12-13&type=Issues) | [@codecov-commenter](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyterlab_server+involves%3Acodecov-commenter+updated%3A2021-09-25..2021-12-13&type=Issues) | [@minrk](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyterlab_server+involves%3Aminrk+updated%3A2021-09-25..2021-12-13&type=Issues) | [@Mithil467](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyterlab_server+involves%3AMithil467+updated%3A2021-09-25..2021-12-13&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyterlab_server+involves%3Awelcome+updated%3A2021-09-25..2021-12-13&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 2.8.2
 
 ([Full Changelog](https://github.com/jupyterlab/jupyterlab_server/compare/v2.8.1...27cead5e506882c1cf999cb8ca48a94031064c9a))
 
 ### Bugs fixed
 
 - Fallback to context-less translation on Python 3.7 [#213](https://github.com/jupyterlab/jupyterlab_server/pull/213) ([@krassowski](https://github.com/krassowski))
@@ -17,16 +45,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlab/jupyterlab_server/graphs/contributors?from=2021-09-07&to=2021-09-25&type=c))
 
 [@codecov-commenter](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyterlab_server+involves%3Acodecov-commenter+updated%3A2021-09-07..2021-09-25&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyterlab_server+involves%3Afcollonval+updated%3A2021-09-07..2021-09-25&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyterlab_server+involves%3Akrassowski+updated%3A2021-09-07..2021-09-25&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 2.8.1
 
 ([Full Changelog](https://github.com/jupyterlab/jupyterlab_server/compare/v2.8.0...680f4fe1c8c7d1d7841e14562720d81a27e6d0ad))
 
 ### Bugs fixed
 
 - Fall back to `DEFAULT_LOCALE` when translation settings schema is invalid in `get_current_locale` [#207](https://github.com/jupyterlab/jupyterlab_server/pull/207) ([@telamonian](https://github.com/telamonian))
```

### Comparing `jupyterlab_server-2.8.2/CONTRIBUTING.md` & `jupyterlab_server-2.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/LICENSE` & `jupyterlab_server-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/MANIFEST.in` & `jupyterlab_server-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/RELEASE.md` & `jupyterlab_server-2.9.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/docs/Makefile` & `jupyterlab_server-2.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/docs/autogen_config.py` & `jupyterlab_server-2.9.0/docs/autogen_config.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/docs/make.bat` & `jupyterlab_server-2.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/docs/source/api/handlers.rst` & `jupyterlab_server-2.9.0/docs/source/api/handlers.rst`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/docs/source/api/process.rst` & `jupyterlab_server-2.9.0/docs/source/api/process.rst`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/docs/source/api/rest.rst` & `jupyterlab_server-2.9.0/docs/source/api/rest.rst`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/docs/source/conf.py` & `jupyterlab_server-2.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/__init__.py` & `jupyterlab_server-2.9.0/jupyterlab_server/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/app.py` & `jupyterlab_server-2.9.0/jupyterlab_server/app.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/config.py` & `jupyterlab_server-2.9.0/jupyterlab_server/config.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/handlers.py` & `jupyterlab_server-2.9.0/jupyterlab_server/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # coding: utf-8
 """JupyterLab Server handlers"""
 
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 import os
 from urllib.parse import urlparse
+from functools import lru_cache
 
 from tornado import template, web
 
 from jupyter_server.extension.handler import ExtensionHandlerMixin, ExtensionHandlerJinjaMixin
 
 from .config import LabConfig, get_page_config, recursive_update
 from .listings_handler import ListingsHandler, fetch_listings
@@ -53,34 +54,29 @@
     return False
 
 
 
 class LabHandler(ExtensionHandlerJinjaMixin, ExtensionHandlerMixin, JupyterHandler):
     """Render the JupyterLab View."""
 
-    @web.authenticated
-    @web.removeslash
-    def get(self, mode = None, workspace = None, tree = None):
-        """Get the JupyterLab html page."""
-        workspace = 'default' if workspace is None else workspace.replace('/workspaces/','')
-        tree_path = '' if tree is None else tree.replace('/tree/','')
-
+    @lru_cache()
+    def get_page_config(self):
+        """Construct the page config object"""
         self.application.store_id = getattr(self.application, 'store_id', 0)
         config = LabConfig()
         app = self.extensionapp
         settings_dir = app.app_settings_dir
-
         # Handle page config data.
         page_config = self.settings.setdefault('page_config_data', {})
         terminals = self.settings.get('terminals_available', False)
         server_root = self.settings.get('server_root_dir', '')
         server_root = server_root.replace(os.sep, '/')
         base_url = self.settings.get('base_url')
 
-        # Remove the trailing slash for compatibiity with html-webpack-plugin.
+        # Remove the trailing slash for compatibility with html-webpack-plugin.
         full_static_url = self.static_url_prefix.rstrip('/')
         page_config.setdefault('fullStaticUrl', full_static_url)
 
         page_config.setdefault('terminalsAvailable', terminals)
         page_config.setdefault('ignorePlugins', [])
         page_config.setdefault('serverRoot', server_root)
         page_config['store_id'] = self.application.store_id
@@ -101,22 +97,14 @@
         mathjax_url = self.mathjax_url
         if not mathjax_url:
             mathjax_url = 'https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js'
 
         page_config.setdefault('mathjaxConfig', mathjax_config)
         page_config.setdefault('fullMathjaxUrl', mathjax_url)
 
-        # Add parameters parsed from the URL
-        if mode == 'doc':
-            page_config['mode'] = 'single-document'
-        else:
-            page_config['mode'] = 'multiple-document'
-        page_config['workspace'] = workspace
-        page_config['treePath'] = tree_path
-
         # Put all our config in page_config
         for name in config.trait_names():
             page_config[_camelCase(name)] = getattr(app, name)
 
         # Add full versions of all the urls
         for name in config.trait_names():
             if not name.endswith('_url'):
@@ -128,25 +116,51 @@
                 full_url = ujoin(base_url, full_url)
             page_config[full_name] = full_url
 
         # Update the page config with the data from disk
         labextensions_path = app.extra_labextensions_path + app.labextensions_path
         recursive_update(page_config, get_page_config(labextensions_path, settings_dir, logger=self.log))
 
+        # modify page config with custom hook
+        page_config_hook = self.settings.get("page_config_hook", None)
+        if page_config_hook:
+            page_config = page_config_hook(self, page_config)
+
+        return page_config
+
+    @web.authenticated
+    @web.removeslash
+    def get(self, mode=None, workspace=None, tree=None):
+        """Get the JupyterLab html page."""
+        workspace = (
+            "default" if workspace is None else workspace.replace("/workspaces/", "")
+        )
+        tree_path = "" if tree is None else tree.replace("/tree/", "")
+
+        page_config = self.get_page_config()
+
+        # Add parameters parsed from the URL
+        if mode == "doc":
+            page_config["mode"] = "single-document"
+        else:
+            page_config["mode"] = "multiple-document"
+        page_config["workspace"] = workspace
+        page_config["treePath"] = tree_path
+
         # Write the template with the config.
         tpl = self.render_template('index.html', page_config=page_config)
         self.write(tpl)
 
 
 class NotFoundHandler(LabHandler):
-    def render_template(self, name, **ns):
-        if 'page_config' in ns:
-            ns['page_config'] = ns['page_config'].copy()
-            ns['page_config']['notFoundUrl'] = self.request.path
-        return super().render_template(name, **ns)
+    @lru_cache()
+    def get_page_config(self):
+        page_config = super().get_page_config()
+        page_config["notFoundUrl"] = self.request.path
+        return page_config
 
 
 def add_handlers(handlers, extension_app):
     """Add the appropriate handlers to the web app.
     """
     # Normalize directories.
     for name in LabConfig.class_trait_names():
```

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/licenses_app.py` & `jupyterlab_server-2.9.0/jupyterlab_server/licenses_app.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/licenses_handler.py` & `jupyterlab_server-2.9.0/jupyterlab_server/licenses_handler.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/listings_handler.py` & `jupyterlab_server-2.9.0/jupyterlab_server/listings_handler.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/process.py` & `jupyterlab_server-2.9.0/jupyterlab_server/process.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/process_app.py` & `jupyterlab_server-2.9.0/jupyterlab_server/process_app.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/pytest_plugin.py` & `jupyterlab_server-2.9.0/jupyterlab_server/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/rest-api.yml` & `jupyterlab_server-2.9.0/jupyterlab_server/rest-api.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/settings_handler.py` & `jupyterlab_server-2.9.0/jupyterlab_server/settings_handler.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/settings_utils.py` & `jupyterlab_server-2.9.0/jupyterlab_server/settings_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,34 +262,58 @@
         try:
             os.makedirs(parent_dir)
         except Exception as e:
             raise web.HTTPError(500, write_error % (schema_name, str(e)))
 
     return path
 
-
 def _get_overrides(app_settings_dir):
-    """Get overrides settings from `app_settings_dir`."""
+    """Get overrides settings from `app_settings_dir`.
+
+    The ordering of paths is:
+    - {app_settings_dir}/overrides.d/*.{json,json5} (many, namespaced by package)
+    - {app_settings_dir}/overrides.{json,json5} (singleton, owned by the user)
+    """
     overrides, error = {}, ""
-    overrides_path = os.path.join(app_settings_dir, 'overrides.json')
 
-    if not os.path.exists(overrides_path):
-        overrides_path = os.path.join(app_settings_dir, 'overrides.json5')
+    overrides_d = os.path.join(app_settings_dir, 'overrides.d')
+
+    # find (and sort) the conf.d overrides files
+    all_override_paths = sorted([
+        *(glob(os.path.join(overrides_d, '*.json'))),
+        *(glob(os.path.join(overrides_d, '*.json5'))),
+    ])
+
+    all_override_paths += [
+        os.path.join(app_settings_dir, 'overrides.json'),
+        os.path.join(app_settings_dir, 'overrides.json5')
+    ]
+
+    for overrides_path in all_override_paths:
+        if not os.path.exists(overrides_path):
+            continue
 
-    if os.path.exists(overrides_path):
         with open(overrides_path, encoding='utf-8') as fid:
             try:
-                overrides = json5.load(fid)
+                if overrides_path.endswith('.json5'):
+                    path_overrides = json5.load(fid)
+                else:
+                    path_overrides = json.load(fid)
+                for plugin_id, config in path_overrides.items():
+                    recursive_update(overrides.setdefault(plugin_id, {}), config)
+                print(overrides_path, overrides)
             except Exception as e:
                 error = e
 
     # Allow `default_settings_overrides.json` files in <jupyter_config>/labconfig dirs
     # to allow layering of defaults
     cm = ConfigManager(config_dir_name="labconfig")
-    recursive_update(overrides, cm.get('default_setting_overrides'))
+
+    for plugin_id, config in cm.get('default_setting_overrides').items():
+        recursive_update(overrides.setdefault(plugin_id, {}), config)
 
     return overrides, error
 
 
 def get_settings(
     app_settings_dir,
     schemas_dir,
```

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/templates/error.html` & `jupyterlab_server-2.9.0/jupyterlab_server/templates/error.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/templates/index.html` & `jupyterlab_server-2.9.0/jupyterlab_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/tests/app-settings/overrides.json` & `jupyterlab_server-2.9.0/jupyterlab_server/tests/app-settings/overrides.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/apputils-extension/themes.json` & `jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/apputils-extension/themes.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/shortcuts-extension/plugin.json` & `jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/shortcuts-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/tests/schemas/@jupyterlab/unicode-extension/plugin.json` & `jupyterlab_server-2.9.0/jupyterlab_server/tests/schemas/@jupyterlab/unicode-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/tests/test_labapp.py` & `jupyterlab_server-2.9.0/jupyterlab_server/tests/test_labapp.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/tests/test_licenses_api.py` & `jupyterlab_server-2.9.0/jupyterlab_server/tests/test_licenses_api.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/tests/test_settings_api.py` & `jupyterlab_server-2.9.0/jupyterlab_server/tests/test_settings_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Test the Settings service API.
 """
+from pathlib import Path
+import json
 
 import pytest
-import json
 import json5
 import tornado
 
 from strict_rfc3339 import rfc3339_to_timestamp
 
 from .utils import expected_http_error
 from .utils import maybe_patch_ioloop, big_unicode_string
@@ -24,14 +25,36 @@
     assert data['id'] == id
     schema = data['schema']
     # Check that overrides.json file is respected.
     assert schema['properties']['codeCellConfig']['default']["lineNumbers"] is True
     assert len(schema['properties']['codeCellConfig']['default']) == 15
 
 
+@pytest.mark.parametrize('ext', ['json', 'json5'])
+async def test_get_settings_overrides_d_dicts(jp_fetch, labserverapp, ext):
+    # Check that values that are dictionaries in overrides.d/*.json are
+    # merged with the schema.
+    id = '@jupyterlab/apputils-extension:themes'
+    overrides_d = Path(labserverapp.app_settings_dir) / "overrides.d"
+    overrides_d.mkdir(exist_ok=True, parents=True)
+    for i in range(10):
+        text = json.dumps({id: {'codeCellConfig': {'cursorBlinkRate': 530 + i}}})
+        if ext == 'json5':
+            text += '\n// a comment'
+        (overrides_d / f"foo-{i}.{ext}").write_text(text, encoding='utf-8')
+    r = await jp_fetch('lab', 'api', 'settings', id)
+    validate_request(r)
+    res = r.body.decode()
+    data = json.loads(res)
+    assert data['id'] == id
+    schema = data['schema']
+    # Check that the last overrides.d/*.json file is respected.
+    assert schema['properties']['codeCellConfig']['default']['cursorBlinkRate'] == 539
+
+
 async def test_get_settings(jp_fetch, labserverapp):
     id = '@jupyterlab/apputils-extension:themes'
     r = await jp_fetch('lab', 'api', 'settings', id)
     validate_request(r)
     res = r.body.decode()
     data = json.loads(res)
     assert data['id'] == id
```

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/tests/test_translation_api.py` & `jupyterlab_server-2.9.0/jupyterlab_server/tests/test_translation_api.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/tests/test_workspaces_api.py` & `jupyterlab_server-2.9.0/jupyterlab_server/tests/test_workspaces_api.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/tests/utils.py` & `jupyterlab_server-2.9.0/jupyterlab_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/themes_handler.py` & `jupyterlab_server-2.9.0/jupyterlab_server/themes_handler.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/translation_utils.py` & `jupyterlab_server-2.9.0/jupyterlab_server/translation_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/translations_handler.py` & `jupyterlab_server-2.9.0/jupyterlab_server/translations_handler.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server/workspaces_handler.py` & `jupyterlab_server-2.9.0/jupyterlab_server/workspaces_handler.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/jupyterlab_server.egg-info/SOURCES.txt` & `jupyterlab_server-2.9.0/jupyterlab_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_server-2.8.2/pyproject.toml` & `jupyterlab_server-2.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
-requires = ["jupyter_packaging~=0.9,<2", "jupyter_server"]
+requires = ["jupyter_packaging>0.9,<2", "jupyter_server"]
 build-backend = "setuptools.build_meta"
 
 [tool.jupyter-releaser]
 skip = ["check-links"]
 
 [tool.check-manifest]
 ignore = ["tbump.toml", ".*", "*.yml", "docs/source/api/app-config.rst", "docs/source/changelog.md"]
 ignore-bad-ideas = ["jupyterlab_server/tests/translations/**/*.mo"]
 
 [tool.tbump.version]
-current = "2.8.2"
+current = "2.9.0"
 regex = '''
   (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)
   ((?P<channel>a|b|rc|.dev)(?P<release>\d+))?
 '''
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
```

### Comparing `jupyterlab_server-2.8.2/setup.cfg` & `jupyterlab_server-2.9.0/setup.cfg`

 * *Files identical despite different names*

