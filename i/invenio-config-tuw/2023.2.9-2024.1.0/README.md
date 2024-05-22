# Comparing `tmp/invenio-config-tuw-2023.2.9.tar.gz` & `tmp/invenio_config_tuw-2024.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-config-tuw-2023.2.9.tar", last modified: Fri Sep  8 09:26:24 2023, max compression
+gzip compressed data, was "invenio_config_tuw-2024.1.0.tar", last modified: Wed May 22 14:22:44 2024, max compression
```

## Comparing `invenio-config-tuw-2023.2.9.tar` & `invenio_config_tuw-2024.1.0.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-09-08 09:26:24.132809 invenio-config-tuw-2023.2.9/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/.dockerignore
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.9/.editorconfig
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.9/.git-blame-ignore-revs
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-09-08 09:26:24.128809 invenio-config-tuw-2023.2.9/.tx/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/.tx/config
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.9/AUTHORS.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2730 2023-09-08 09:24:48.000000 invenio-config-tuw-2023.2.9/CHANGES.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.9/CONTRIBUTING.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/INSTALL.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/LICENSE
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.9/MANIFEST.in
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     6246 2023-09-08 09:26:24.132809 invenio-config-tuw-2023.2.9/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-08-09 11:57:39.000000 invenio-config-tuw-2023.2.9/README.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/babel.ini
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-09-08 09:26:24.128809 invenio-config-tuw-2023.2.9/docs/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/docs/Makefile
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/docs/api.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/docs/authors.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/docs/changes.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.9/docs/conf.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/docs/configuration.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/docs/contributing.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/docs/index.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/docs/installation.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/docs/license.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/docs/make.bat
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/docs/requirements.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/docs/usage.rst
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-09-08 09:26:24.128809 invenio-config-tuw-2023.2.9/invenio_config_tuw/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2023-09-08 09:24:48.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/__init__.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-09-08 09:26:24.132809 invenio-config-tuw-2023.2.9/invenio_config_tuw/auth/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/auth/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1495 2023-08-23 15:58:23.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/auth/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8967 2023-08-23 15:58:23.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/auth/handlers.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-10-04 14:54:28.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/auth/utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8150 2023-08-23 15:58:23.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2022-11-24 12:57:07.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/ext.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1337 2023-05-26 12:34:11.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/formatters.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3219 2023-09-08 09:24:48.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/forms.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-09-08 09:26:24.132809 invenio-config-tuw-2023.2.9/invenio_config_tuw/permissions/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-07-18 13:04:23.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/permissions/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3758 2023-09-08 09:24:48.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/permissions/generators.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11152 2023-09-08 09:24:48.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/permissions/policies.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3862 2022-10-28 12:03:49.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/startup.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4599 2023-07-26 20:31:27.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/tasks.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-09-08 09:26:24.132809 invenio-config-tuw-2023.2.9/invenio_config_tuw/tiss/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      409 2023-07-26 14:21:51.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/tiss/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2404 2023-07-26 14:21:51.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/tiss/models.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1794 2023-07-26 14:21:51.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/tiss/utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2739 2023-04-24 16:03:59.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw/utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-09-08 09:26:24.132809 invenio-config-tuw-2023.2.9/invenio_config_tuw.egg-info/
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     6246 2023-09-08 09:26:24.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1401 2023-09-08 09:26:24.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-09-08 09:26:24.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      491 2023-09-08 09:26:24.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-09-08 09:26:12.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw.egg-info/not-zip-safe
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2023-09-08 09:26:24.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2023-09-08 09:26:24.000000 invenio-config-tuw-2023.2.9/invenio_config_tuw.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.9/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/requirements-devel.txt
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.9/run-tests.sh
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2838 2023-09-08 09:26:24.132809 invenio-config-tuw-2023.2.9/setup.cfg
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.9/setup.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-09-08 09:26:24.132809 invenio-config-tuw-2023.2.9/tests/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2023-08-07 11:43:58.000000 invenio-config-tuw-2023.2.9/tests/conftest.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.9/tests/test_invenio_config_tuw.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 14:22:44.554835 invenio_config_tuw-2024.1.0/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/.dockerignore
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2022-11-23 16:27:25.000000 invenio_config_tuw-2024.1.0/.editorconfig
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2022-11-23 16:27:25.000000 invenio_config_tuw-2024.1.0/.git-blame-ignore-revs
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 14:22:44.546835 invenio_config_tuw-2024.1.0/.tx/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/.tx/config
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-07-15 09:46:09.000000 invenio_config_tuw-2024.1.0/AUTHORS.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3077 2024-05-22 14:20:44.000000 invenio_config_tuw-2024.1.0/CHANGES.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-07-15 09:46:09.000000 invenio_config_tuw-2024.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/INSTALL.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/LICENSE
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2022-11-23 16:27:25.000000 invenio_config_tuw-2024.1.0/MANIFEST.in
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     6593 2024-05-22 14:22:44.554835 invenio_config_tuw-2024.1.0/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-08-09 11:57:39.000000 invenio_config_tuw-2024.1.0/README.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/babel.ini
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 14:22:44.546835 invenio_config_tuw-2024.1.0/docs/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/docs/Makefile
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/docs/api.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/docs/authors.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/docs/changes.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2022-11-23 16:27:25.000000 invenio_config_tuw-2024.1.0/docs/conf.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/docs/configuration.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/docs/contributing.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/docs/index.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/docs/installation.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/docs/license.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/docs/make.bat
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/docs/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/docs/usage.rst
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 14:22:44.550835 invenio_config_tuw-2024.1.0/invenio_config_tuw/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2024-05-22 14:20:44.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/__init__.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 14:22:44.550835 invenio_config_tuw-2024.1.0/invenio_config_tuw/auth/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-07-15 09:46:09.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/auth/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1491 2023-09-25 11:45:12.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/auth/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     9926 2024-05-22 14:20:44.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/auth/handlers.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-10-04 14:54:28.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/auth/utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8606 2024-05-22 14:20:44.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2220 2023-12-22 14:08:02.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/curation.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2022-11-24 12:57:07.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/ext.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1337 2023-05-26 12:34:11.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/formatters.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3923 2024-05-22 14:20:44.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/forms.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 14:22:44.550835 invenio_config_tuw-2024.1.0/invenio_config_tuw/permissions/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-07-18 13:04:23.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/permissions/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3758 2023-09-08 09:24:48.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/permissions/generators.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11152 2023-09-08 09:24:48.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/permissions/policies.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1388 2024-05-22 14:20:44.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/schemas.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5579 2023-12-22 14:54:23.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/startup.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4599 2023-07-26 20:31:27.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/tasks.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 14:22:44.550835 invenio_config_tuw-2024.1.0/invenio_config_tuw/tiss/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      409 2023-07-26 14:21:51.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/tiss/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2404 2023-07-26 14:21:51.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/tiss/models.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1794 2023-07-26 14:21:51.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/tiss/utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3590 2024-05-22 14:20:44.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw/utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 14:22:44.554835 invenio_config_tuw-2024.1.0/invenio_config_tuw.egg-info/
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     6593 2024-05-22 14:22:44.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1462 2024-05-22 14:22:44.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-05-22 14:22:44.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      583 2024-05-22 14:22:44.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-05-22 14:22:38.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw.egg-info/not-zip-safe
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2024-05-22 14:22:44.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2024-05-22 14:22:44.000000 invenio_config_tuw-2024.1.0/invenio_config_tuw.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2022-11-23 16:27:25.000000 invenio_config_tuw-2024.1.0/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/requirements-devel.txt
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2022-11-23 16:27:25.000000 invenio_config_tuw-2024.1.0/run-tests.sh
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2931 2024-05-22 14:22:44.554835 invenio_config_tuw-2024.1.0/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2022-11-23 16:27:25.000000 invenio_config_tuw-2024.1.0/setup.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 14:22:44.554835 invenio_config_tuw-2024.1.0/tests/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2023-08-07 11:43:58.000000 invenio_config_tuw-2024.1.0/tests/conftest.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-07-02 11:25:37.000000 invenio_config_tuw-2024.1.0/tests/test_invenio_config_tuw.py
```

### Comparing `invenio-config-tuw-2023.2.9/.editorconfig` & `invenio_config_tuw-2024.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/.tx/config` & `invenio_config_tuw-2024.1.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/CHANGES.rst` & `invenio_config_tuw-2024.1.0/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 ..
-    Copyright (C) 2020-2023 TU Wien.
+    Copyright (C) 2020-2024 TU Wien.
 
     Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24, updated 2023-09-08)
 
+Version 2024.1 (released 2024-05-22
+
+- Store ``given_name`` and ``family_name`` in user profiles
+- Use these values to more accurately synthesize default values for creators in metadata
+
+
+Version 2023.2 (released 2023-04-24, updated 2023-12-22)
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
 - Add a null check for the current_user in the logging formatter
 - Prevent the logging formatter from blowing up outside of a request context
 - Add utilities and a celery task for updating the `names` vocabulary with information from TISS
 - Enable sending of registration mails
 - Allow edits to owners of published records even if they only have `trusted-user` role
+- Fix a typo in the config generated by the `TUWSSOSettingsHelper`
+- Fix function to fetch user by username
+- Add record curation preferences to user settings
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.9/CONTRIBUTING.rst` & `invenio_config_tuw-2024.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/LICENSE` & `invenio_config_tuw-2024.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/MANIFEST.in` & `invenio_config_tuw-2024.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/PKG-INFO` & `invenio_config_tuw-2024.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.2.9
+Version: 2024.1.0
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -97,34 +97,43 @@
 --------------------
 
 Last but not least, we also set some default configuration values for deployments
 of InvenioRDM at TU Wien.
 The relevant files here are ``config.py`` and ``ext.py``.
 
 ..
-    Copyright (C) 2020-2023 TU Wien.
+    Copyright (C) 2020-2024 TU Wien.
 
     Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24, updated 2023-09-08)
 
+Version 2024.1 (released 2024-05-22
+
+- Store ``given_name`` and ``family_name`` in user profiles
+- Use these values to more accurately synthesize default values for creators in metadata
+
+
+Version 2023.2 (released 2023-04-24, updated 2023-12-22)
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
 - Add a null check for the current_user in the logging formatter
 - Prevent the logging formatter from blowing up outside of a request context
 - Add utilities and a celery task for updating the `names` vocabulary with information from TISS
 - Enable sending of registration mails
 - Allow edits to owners of published records even if they only have `trusted-user` role
+- Fix a typo in the config generated by the `TUWSSOSettingsHelper`
+- Fix function to fetch user by username
+- Add record curation preferences to user settings
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.9/README.rst` & `invenio_config_tuw-2024.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/babel.ini` & `invenio_config_tuw-2024.1.0/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/docs/Makefile` & `invenio_config_tuw-2024.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/docs/conf.py` & `invenio_config_tuw-2024.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/docs/index.rst` & `invenio_config_tuw-2024.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/docs/make.bat` & `invenio_config_tuw-2024.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/auth/__init__.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/auth/config.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/auth/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         super().__init__(
             title, description, base_url, realm, app_key=None, icon=None, **kwargs
         )
 
     def get_handlers(self):
         return {
             "authorized_handler": "invenio_config_tuw.auth:authorized_signup_handler",
-            "disconnect_handlerdler": (
+            "disconnect_handler": (
                 "invenio_oauthclient.contrib.keycloak.handlers:disconnect_handler"
             ),
             "signup_handler": {
                 "info": "invenio_config_tuw.auth:info_handler",
                 "setup": "invenio_oauthclient.contrib.keycloak.handlers:setup_handler",
                 "view": "invenio_config_tuw.auth:signup_handler",
             },
```

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/auth/handlers.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/auth/handlers.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,25 +48,36 @@
 def info_handler(remote, resp):
     """Retrieve remote account information for finding matching local users."""
     # NOTE: for lookup of local users, only the 'external_id' and 'user.email' are used
     #       => calculation of the 'user.user_profile.username'
     #          here should actually be safe
     user_info = get_user_info(remote, resp)
 
+    # get or synthesize the name entries for the user profile
+    # note: we used to only get the "full_name"; it's unlikely that this would
+    #       need to be synthesized
+    given_name = user_info.get("given_name")
+    family_name = user_info.get("family_name")
+    full_name = user_info.get("name")
+    if not full_name:
+        full_name = f"{given_name} {family_name}"
+
     # fill out the information required by 'invenio-accounts'.
     #
     # note: "external_id": `preferred_username` should also work,
     #       as it is seemingly not editable in Keycloak
     result = {
         "user": {
             "active": True,
             "email": user_info["email"],
             "username": user_info.get("preferred_username"),
             "user_profile": {
-                "full_name": user_info.get("name"),
+                "full_name": full_name,
+                "given_name": given_name,
+                "family_name": family_name,
             },
         },
         "external_id": user_info["sub"],
         "external_method": remote.name,
     }
 
     return result
@@ -200,26 +211,39 @@
 
         if user_found:
             # the user already exists: update their details!
             user_info = account_info.get("user", {})
             new_email = user_info.get("email", user.email)
             new_profile = user_info.get("user_profile", {})
             new_full_name = new_profile.get("full_name")
+            new_given_name = new_profile.get("given_name")
+            new_family_name = new_profile.get("family_name")
 
             if user.email != new_email:
                 user.email = new_email
 
                 # our usernames are based on the users' email addresses;
                 # thus, we need to update the username if the email address changes
                 user.username = create_username_from_info(user_info)
 
-            # update the full name if it has changed
+            # update the user's name if it has changed
             old_profile = user.user_profile or {}
-            if new_full_name and new_full_name != user.user_profile["full_name"]:
-                user.user_profile = {"full_name": new_full_name, **old_profile}
+            _new_names = (new_given_name, new_family_name)
+            _old_names = (old_profile.get("given_name"), old_profile.get("family_name"))
+
+            if new_full_name and (
+                new_full_name != old_profile.get("full_name")
+                or _new_names != _old_names
+            ):
+                user.user_profile = {
+                    **old_profile,
+                    "full_name": new_full_name,
+                    "given_name": new_given_name,
+                    "family_name": new_family_name,
+                }
 
         # Hard code the affiliation to TU Wien, since we are currently
         # not accepting any externals. It is set on every login.
         user.user_profile = {**user.user_profile, "affiliations": "TU Wien"}
 
         # Link account
         # ------------
```

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/auth/utils.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/auth/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/config.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from flask_babelex import gettext as _
 from invenio_oauthclient.views.client import auto_redirect_login
 
 from .auth import TUWSSOSettingsHelper
 from .forms import tuw_registration_form
 from .permissions import TUWRecordPermissionPolicy, TUWRequestsPermissionPolicy
+from .schemas import TUWUserPreferencesSchema, TUWUserProfileSchema, TUWUserSchema
 from .utils import check_user_email_for_tuwien, current_user_as_creator
 
 # Invenio-Config-TUW
 # ==================
 
 CONFIG_TUW_AUTO_TRUST_USERS = True
 """Whether or not to auto-assign the 'trusted-user' role to new users."""
@@ -128,15 +129,20 @@
 OAUTHCLIENT_KEYCLOAK_AUD = "tu-data-test"
 OAUTHCLIENT_KEYCLOAK_VERIFY_AUD = True
 
 keycloak_remote_app = helper.remote_app
 keycloak_remote_app["precedence_mask"] = {
     "email": True,
     "username": True,
-    "user_profile": {"full_name": True, "affiliations": True},
+    "user_profile": {
+        "full_name": True,
+        "given_name": True,
+        "family_name": True,
+        "affiliations": True,
+    },
 }
 
 OAUTHCLIENT_REMOTE_APPS = {
     "keycloak": keycloak_remote_app,
 }
 
 
@@ -247,7 +253,16 @@
 RECAPTCHA_PUBLIC_KEY = None
 
 # Recaptcha private key (change to enable).
 RECAPTCHA_PRIVATE_KEY = None
 
 # Preferred URL scheme to use
 PREFERRED_URL_SCHEME = "https"
+
+# Extended schema for user preferences
+ACCOUNTS_USER_PREFERENCES_SCHEMA = TUWUserPreferencesSchema()
+
+# Extended schema for user preferences
+ACCOUNTS_USER_PROFILE_SCHEMA = TUWUserProfileSchema()
+
+# Extended schema for users in the users service
+USERS_RESOURCES_SERVICE_SCHEMA = TUWUserSchema
```

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/ext.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/formatters.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/formatters.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/forms.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/forms.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,52 +28,65 @@
     This means that we have to actually hold information in the forms and can't
     just set every field to ``None``.
     """
     # the url must contain the special characters rather than encoded values:
     # `Markup` escapes them
     terms_of_use_url = "https://www.tuwien.at/index.php?eID=dms&s=4&path=Directives and Regulations of the Rectorate/Research_Data_Terms_of_Use.pdf"  # noqa
     message = Markup(
-        f"Accept the <a href='{terms_of_use_url}' target='_blank'>Terms and Conditions</a>"  # noqa
+        f"Accept the <a href='{terms_of_use_url}' target='_blank'>Terms and Conditions</a> (<strong>required</strong>)"  # noqa
+    )
+    curation_consent_message = Markup(
+        "Allow the repository team to curate the metadata of my uploads after publication"
     )
 
     class UserProfileForm(Form):
         """Form for the user profile."""
 
         full_name = HiddenField()
+        given_name = HiddenField()
+        family_name = HiddenField()
         affiliations = HiddenField()
 
     class UserPreferenceForm(Form):
         """Form for the user preferences."""
 
         visibility = HiddenField(default="public")
         email_visibility = HiddenField(default="restricted")
 
     class UserRegistrationForm(_security.confirm_register_form):
         """Form for the basic user information."""
 
+        # the curation consent is listed here instead of in a sub-form,
+        # because that caused very quirky rendering
         email = HiddenField()
         username = HiddenField()
         user_profile = FormField(UserProfileForm, separator=".")
         preferences = FormField(UserPreferenceForm, separator=".")
         password = None
         recaptcha = None
         profile = None  # disable the default 'profile' form from invenio
         submit = None  # defined in the template
+        curation_consent = BooleanField(curation_consent_message, default="checked")
         terms_of_use = BooleanField(message, [validators.required()])
 
         def to_dict(self):
             """Turn the form into a dictionary."""
             return {
                 "email": self.email.data,
                 "username": self.username.data,
                 "password": None,
                 "user_profile": {
                     "full_name": self.user_profile.full_name.data,
+                    "given_name": self.user_profile.given_name.data,
+                    "family_name": self.user_profile.family_name.data,
                     "affiliations": self.user_profile.affiliations.data,
                 },
                 "preferences": {
                     "visibility": self.preferences.visibility.data,
                     "email_visibility": self.preferences.email_visibility.data,
+                    "curation": {
+                        "consent": self.curation_consent.data,
+                    },
                 },
             }
 
     return UserRegistrationForm(*args, **kwargs)
```

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/permissions/__init__.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/permissions/generators.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/permissions/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/permissions/policies.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/permissions/policies.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/tasks.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/tiss/models.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/tiss/models.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/tiss/utils.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/tiss/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw/utils.py` & `invenio_config_tuw-2024.1.0/invenio_config_tuw/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,33 +3,30 @@
 # Copyright (C) 2020-2022 TU Wien.
 #
 # Invenio-Config-TUW is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Utility functions."""
 
+from typing import Dict, Tuple
+
 from flask_principal import Identity
 from flask_security import current_user
 from invenio_access import any_user
 from invenio_access.utils import get_identity
 from invenio_accounts import current_accounts
 from invenio_accounts.models import User
 
 # Utilities for internal use
 # --------------------------
 
 
 def get_user_by_username(username):
     """Get the user identified by the username."""
-    profile = User.query.filter(User.username == username).one_or_none()
-
-    if profile is not None:
-        return profile.user
-
-    return None
+    return User.query.filter(User.username == username).one_or_none()
 
 
 def get_user(identifier):
     """Get the user identified by the given ID, email or username."""
     user = current_accounts.datastore.get_user(identifier)
     if user is None:
         get_user_by_username(identifier)
@@ -62,33 +59,54 @@
 
 def check_user_email_for_tuwien(user):
     """Check if the user's email belongs to TU Wien (but not as a student)."""
     domain = user.email.split("@")[-1]
     return domain.endswith("tuwien.ac.at") and "student" not in domain
 
 
+def _names_from_user_profile(profile: Dict) -> Tuple[str, str, str]:
+    """Get the ``given_name``, ``family_name`` and ``full_name`` of the user."""
+    given_name, family_name = profile.get("given_name"), profile.get("family_name")
+    full_name = profile.get("full_name")
+
+    if given_name and family_name:
+        full_name = full_name or f"{family_name}, {given_name}"
+
+    elif full_name:
+        if ", " in full_name:
+            # in case there's a comma in the name, we assume it's "FAMILY, GIVEN"
+            given_name, family_name = full_name.split(", ", 1)
+
+        else:
+            # otherwise, we assume it has the shape "GIVEN, FAMILY"
+            name_parts = full_name.split()
+
+            given_name = " ".join(name_parts[:-1])
+            family_name = name_parts[-1]
+            full_name = f"{family_name}, {given_name}"
+
+    return (given_name, family_name, full_name)
+
+
 def current_user_as_creator():
     """Use the currently logged-in user to populate a creator in the deposit form."""
     profile = current_user.user_profile or {}
-    if profile.get("full_name") is None:
-        return []
+    given_name, family_name, full_name = _names_from_user_profile(profile)
 
-    name_parts = profile["full_name"].split()
-    if len(name_parts) <= 1:
+    # if we have no clue about the name, we skip the creator
+    if not given_name and not family_name and not full_name:
         return []
 
-    first_name = " ".join(name_parts[:-1])
-    last_name = name_parts[-1]
-    full_name = "{}, {}".format(last_name, first_name)
     # TODO parse affiliation from user profile
+    # TODO add identifiers (e.g. ORCID from TISS, if available)
     creator = {
         "affiliations": [{"id": "04d836q62", "name": "TU Wien"}],
         "person_or_org": {
-            "family_name": last_name,
-            "given_name": first_name,
+            "family_name": family_name,
+            "given_name": given_name,
             "identifiers": [],
             "name": full_name,
             "type": "personal",
         },
         "role": "contactperson",
     }
```

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw.egg-info/PKG-INFO` & `invenio_config_tuw-2024.1.0/invenio_config_tuw.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.2.9
+Version: 2024.1.0
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -97,34 +97,43 @@
 --------------------
 
 Last but not least, we also set some default configuration values for deployments
 of InvenioRDM at TU Wien.
 The relevant files here are ``config.py`` and ``ext.py``.
 
 ..
-    Copyright (C) 2020-2023 TU Wien.
+    Copyright (C) 2020-2024 TU Wien.
 
     Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24, updated 2023-09-08)
 
+Version 2024.1 (released 2024-05-22
+
+- Store ``given_name`` and ``family_name`` in user profiles
+- Use these values to more accurately synthesize default values for creators in metadata
+
+
+Version 2023.2 (released 2023-04-24, updated 2023-12-22)
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
 - Add a null check for the current_user in the logging formatter
 - Prevent the logging formatter from blowing up outside of a request context
 - Add utilities and a celery task for updating the `names` vocabulary with information from TISS
 - Enable sending of registration mails
 - Allow edits to owners of published records even if they only have `trusted-user` role
+- Fix a typo in the config generated by the `TUWSSOSettingsHelper`
+- Fix function to fetch user by username
+- Add record curation preferences to user settings
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.9/invenio_config_tuw.egg-info/SOURCES.txt` & `invenio_config_tuw-2024.1.0/invenio_config_tuw.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,19 @@
 docs/installation.rst
 docs/license.rst
 docs/make.bat
 docs/requirements.txt
 docs/usage.rst
 invenio_config_tuw/__init__.py
 invenio_config_tuw/config.py
+invenio_config_tuw/curation.py
 invenio_config_tuw/ext.py
 invenio_config_tuw/formatters.py
 invenio_config_tuw/forms.py
+invenio_config_tuw/schemas.py
 invenio_config_tuw/startup.py
 invenio_config_tuw/tasks.py
 invenio_config_tuw/utils.py
 invenio_config_tuw.egg-info/PKG-INFO
 invenio_config_tuw.egg-info/SOURCES.txt
 invenio_config_tuw.egg-info/dependency_links.txt
 invenio_config_tuw.egg-info/entry_points.txt
```

### Comparing `invenio-config-tuw-2023.2.9/setup.cfg` & `invenio_config_tuw-2024.1.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 [options.entry_points]
 invenio_base.apps = 
 	invenio_config_tuw = invenio_config_tuw:InvenioConfigTUW
 invenio_base.api_apps = 
 	invenio_config_tuw = invenio_config_tuw:InvenioConfigTUW
 invenio_base.blueprints = 
 	invenio_config_tuw_hacks = invenio_config_tuw.startup:blueprint
+	invenio_config_tuw_settings = invenio_config_tuw.startup:create_curation_settings_blueprint
 invenio_base.api_blueprints = 
 	invenio_config_tuw_hacks = invenio_config_tuw.startup:blueprint
 invenio_celery.tasks = 
 	invenio_config_tuw = invenio_config_tuw.tasks
 invenio_config.module = 
 	zzz_invenio_config_tuw = invenio_config_tuw.config
```

### Comparing `invenio-config-tuw-2023.2.9/tests/conftest.py` & `invenio_config_tuw-2024.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.9/tests/test_invenio_config_tuw.py` & `invenio_config_tuw-2024.1.0/tests/test_invenio_config_tuw.py`

 * *Files identical despite different names*

