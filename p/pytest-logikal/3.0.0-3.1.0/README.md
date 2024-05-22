# Comparing `tmp/pytest_logikal-3.0.0.tar.gz` & `tmp/pytest_logikal-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_logikal-3.0.0.tar", last modified: Sat May 18 17:00:43 2024, max compression
+gzip compressed data, was "pytest_logikal-3.1.0.tar", last modified: Wed May 22 09:35:09 2024, max compression
```

## Comparing `pytest_logikal-3.0.0.tar` & `pytest_logikal-3.1.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:43.371421 pytest_logikal-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-18 17:00:43.371421 pytest_logikal-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/entry_points.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:43.367421 pytest_logikal-3.0.0/pytest_logikal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/bandit.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/bandit_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/black.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:43.367421 pytest_logikal-3.0.0/pytest_logikal/browser/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/chrome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/chromium.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/browser/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/css.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/css_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/file_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/isort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/js.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/js_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/migration.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/node_install.py
--rw-r--r--   0 runner    (1001) docker     (127)    98728 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/pylint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/svg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/translations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/pytest_logikal/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:43.371421 pytest_logikal-3.0.0/pytest_logikal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-18 17:00:43.000000 pytest_logikal-3.0.0/pytest_logikal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-18 17:00:43.000000 pytest_logikal-3.0.0/pytest_logikal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 17:00:43.000000 pytest_logikal-3.0.0/pytest_logikal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-18 17:00:43.000000 pytest_logikal-3.0.0/pytest_logikal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-18 17:00:43.000000 pytest_logikal-3.0.0/pytest_logikal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 17:00:43.000000 pytest_logikal-3.0.0/pytest_logikal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:43.367421 pytest_logikal-3.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:00:43.367421 pytest_logikal-3.0.0/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/extras/black.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/extras/browser.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-18 17:00:25.000000 pytest_logikal-3.0.0/requirements/extras/django.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 17:00:43.371421 pytest_logikal-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:35:09.255418 pytest_logikal-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-22 09:35:09.255418 pytest_logikal-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/entry_points.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:35:09.247418 pytest_logikal-3.1.0/pytest_logikal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/bandit_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/black.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:35:09.247418 pytest_logikal-3.1.0/pytest_logikal/browser/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/browser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/browser/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/browser/chromium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/browser/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/browser/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/browser/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/browser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/css.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/css_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/file_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/isort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/js.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/js_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/node_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98728 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/translations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/pytest_logikal/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:35:09.251418 pytest_logikal-3.1.0/pytest_logikal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-22 09:35:09.000000 pytest_logikal-3.1.0/pytest_logikal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-22 09:35:09.000000 pytest_logikal-3.1.0/pytest_logikal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:35:09.000000 pytest_logikal-3.1.0/pytest_logikal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-22 09:35:09.000000 pytest_logikal-3.1.0/pytest_logikal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-22 09:35:09.000000 pytest_logikal-3.1.0/pytest_logikal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 09:35:09.000000 pytest_logikal-3.1.0/pytest_logikal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:35:09.251418 pytest_logikal-3.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:35:09.251418 pytest_logikal-3.1.0/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/requirements/extras/black.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/requirements/extras/browser.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 09:34:53.000000 pytest_logikal-3.1.0/requirements/extras/django.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:35:09.255418 pytest_logikal-3.1.0/setup.cfg
```

### Comparing `pytest_logikal-3.0.0/LICENSE.txt` & `pytest_logikal-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/PKG-INFO` & `pytest_logikal-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 3.0.0
+Version: 3.1.0
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -40,46 +40,46 @@
 Requires-Dist: bandit==1.7.8
 Requires-Dist: coverage[toml]==7.5.1
 Requires-Dist: isort[colors]==5.13.2
 Requires-Dist: mypy==1.10.0
 Requires-Dist: pip-licenses==4.4.0
 Requires-Dist: pycodestyle==2.11.1
 Requires-Dist: pydocstyle[toml]==6.3.0
-Requires-Dist: pylint==3.2.0
-Requires-Dist: pytest==8.2.0
+Requires-Dist: pylint==3.2.2
+Requires-Dist: pytest==8.2.1
 Requires-Dist: pytest-cov==5.0.0
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: pytest-mypy==0.10.3
 Requires-Dist: pytest-xdist[psutil]==3.6.1
 Requires-Dist: pillow~=10.3
 Requires-Dist: Pygments~=2.17
-Requires-Dist: logikal-utils~=1.0
+Requires-Dist: logikal-utils~=1.1
 Requires-Dist: pyorbs~=2.1
 Requires-Dist: termcolor~=2.4
 Provides-Extra: black
 Requires-Dist: black==24.4.2; extra == "black"
 Provides-Extra: browser
-Requires-Dist: requests~=2.31; extra == "browser"
-Requires-Dist: types-requests~=2.31; extra == "browser"
+Requires-Dist: requests<2.32; extra == "browser"
+Requires-Dist: types-requests<2.32; extra == "browser"
 Requires-Dist: tqdm~=4.66; extra == "browser"
 Requires-Dist: types-tqdm~=4.66; extra == "browser"
 Requires-Dist: selenium==4.21.0; extra == "browser"
 Requires-Dist: xdg~=5.1; extra == "browser"
 Provides-Extra: django
 Requires-Dist: Babel~=2.14; extra == "django"
 Requires-Dist: Django~=4.2; extra == "django"
 Requires-Dist: django-stubs~=4.2; extra == "django"
 Requires-Dist: django-migration-linter~=5.1; extra == "django"
 Requires-Dist: djlint==1.34.1; extra == "django"
 Requires-Dist: pylint-django==2.5.5; extra == "django"
 Requires-Dist: pytest-django==4.8.0; extra == "django"
 Requires-Dist: pytest-factoryboy==2.7.0; extra == "django"
-Requires-Dist: requests~=2.31; extra == "django"
-Requires-Dist: types-requests~=2.31; extra == "django"
-Requires-Dist: logikal-utils[docker]~=1.0; extra == "django"
+Requires-Dist: requests<2.32; extra == "django"
+Requires-Dist: types-requests<2.32; extra == "django"
+Requires-Dist: logikal-utils[docker]~=1.1; extra == "django"
 
 pytest-logikal
 ==============
 Common tools for Python testing implemented as a `pytest <https://docs.pytest.org/>`_ plugin.
 
 Getting Started
 ---------------
```

### Comparing `pytest_logikal-3.0.0/entry_points.ini` & `pytest_logikal-3.1.0/entry_points.ini`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pyproject.toml` & `pytest_logikal-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/bandit.py` & `pytest_logikal-3.1.0/pytest_logikal/bandit.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/black.py` & `pytest_logikal-3.1.0/pytest_logikal/black.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/browser/base.py` & `pytest_logikal-3.1.0/pytest_logikal/browser/base.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/browser/chrome.py` & `pytest_logikal-3.1.0/pytest_logikal/browser/chrome.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/browser/chromium.py` & `pytest_logikal-3.1.0/pytest_logikal/browser/chromium.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/browser/edge.py` & `pytest_logikal-3.1.0/pytest_logikal/browser/edge.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/browser/plugin.py` & `pytest_logikal-3.1.0/pytest_logikal/browser/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/browser/scenarios.py` & `pytest_logikal-3.1.0/pytest_logikal/browser/scenarios.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/browser/utils.py` & `pytest_logikal-3.1.0/pytest_logikal/browser/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/build.py` & `pytest_logikal-3.1.0/pytest_logikal/build.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/core.py` & `pytest_logikal-3.1.0/pytest_logikal/core.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/css.py` & `pytest_logikal-3.1.0/pytest_logikal/css.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/css_config.yml` & `pytest_logikal-3.1.0/pytest_logikal/css_config.yml`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/django.py` & `pytest_logikal-3.1.0/pytest_logikal/django.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def pytest_sessionstart(session: pytest.Session) -> None:
     if not session.config.getoption('no_install'):
         install_node_packages()
 
     if not session.config.getoption('no_css') and not session.config.getoption('no_svg'):
         # We start the validator service here to avoid pytest's output capturing
-        Validator.start_service()
+        Validator.service_url()
 
 
 def pytest_configure(config: pytest.Config) -> None:
     # Patching django-stubs
     def parse_toml_file(self: Any, *_args: Any, **_kwargs: Any) -> None:
         self.django_settings_module = str(config.inicfg['DJANGO_SETTINGS_MODULE'])
         self.strict_settings = True
```

### Comparing `pytest_logikal-3.0.0/pytest_logikal/docs.py` & `pytest_logikal-3.1.0/pytest_logikal/docs.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/file_checker.py` & `pytest_logikal-3.1.0/pytest_logikal/file_checker.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/html.py` & `pytest_logikal-3.1.0/pytest_logikal/html.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/isort.py` & `pytest_logikal-3.1.0/pytest_logikal/isort.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/js.py` & `pytest_logikal-3.1.0/pytest_logikal/js.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/js_config.yml` & `pytest_logikal-3.1.0/pytest_logikal/js_config.yml`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/licenses.py` & `pytest_logikal-3.1.0/pytest_logikal/licenses.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/migration.py` & `pytest_logikal-3.1.0/pytest_logikal/migration.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/node_install.py` & `pytest_logikal-3.1.0/pytest_logikal/node_install.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/package-lock.json` & `pytest_logikal-3.1.0/pytest_logikal/package-lock.json`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/plugin.py` & `pytest_logikal-3.1.0/pytest_logikal/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/pylint.py` & `pytest_logikal-3.1.0/pytest_logikal/pylint.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/requirements.py` & `pytest_logikal-3.1.0/pytest_logikal/requirements.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/style.py` & `pytest_logikal-3.1.0/pytest_logikal/style.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/svg.py` & `pytest_logikal-3.1.0/pytest_logikal/svg.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/translations.py` & `pytest_logikal-3.1.0/pytest_logikal/translations.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal/utils.py` & `pytest_logikal-3.1.0/pytest_logikal/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal.egg-info/PKG-INFO` & `pytest_logikal-3.1.0/pytest_logikal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 3.0.0
+Version: 3.1.0
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -40,46 +40,46 @@
 Requires-Dist: bandit==1.7.8
 Requires-Dist: coverage[toml]==7.5.1
 Requires-Dist: isort[colors]==5.13.2
 Requires-Dist: mypy==1.10.0
 Requires-Dist: pip-licenses==4.4.0
 Requires-Dist: pycodestyle==2.11.1
 Requires-Dist: pydocstyle[toml]==6.3.0
-Requires-Dist: pylint==3.2.0
-Requires-Dist: pytest==8.2.0
+Requires-Dist: pylint==3.2.2
+Requires-Dist: pytest==8.2.1
 Requires-Dist: pytest-cov==5.0.0
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: pytest-mypy==0.10.3
 Requires-Dist: pytest-xdist[psutil]==3.6.1
 Requires-Dist: pillow~=10.3
 Requires-Dist: Pygments~=2.17
-Requires-Dist: logikal-utils~=1.0
+Requires-Dist: logikal-utils~=1.1
 Requires-Dist: pyorbs~=2.1
 Requires-Dist: termcolor~=2.4
 Provides-Extra: black
 Requires-Dist: black==24.4.2; extra == "black"
 Provides-Extra: browser
-Requires-Dist: requests~=2.31; extra == "browser"
-Requires-Dist: types-requests~=2.31; extra == "browser"
+Requires-Dist: requests<2.32; extra == "browser"
+Requires-Dist: types-requests<2.32; extra == "browser"
 Requires-Dist: tqdm~=4.66; extra == "browser"
 Requires-Dist: types-tqdm~=4.66; extra == "browser"
 Requires-Dist: selenium==4.21.0; extra == "browser"
 Requires-Dist: xdg~=5.1; extra == "browser"
 Provides-Extra: django
 Requires-Dist: Babel~=2.14; extra == "django"
 Requires-Dist: Django~=4.2; extra == "django"
 Requires-Dist: django-stubs~=4.2; extra == "django"
 Requires-Dist: django-migration-linter~=5.1; extra == "django"
 Requires-Dist: djlint==1.34.1; extra == "django"
 Requires-Dist: pylint-django==2.5.5; extra == "django"
 Requires-Dist: pytest-django==4.8.0; extra == "django"
 Requires-Dist: pytest-factoryboy==2.7.0; extra == "django"
-Requires-Dist: requests~=2.31; extra == "django"
-Requires-Dist: types-requests~=2.31; extra == "django"
-Requires-Dist: logikal-utils[docker]~=1.0; extra == "django"
+Requires-Dist: requests<2.32; extra == "django"
+Requires-Dist: types-requests<2.32; extra == "django"
+Requires-Dist: logikal-utils[docker]~=1.1; extra == "django"
 
 pytest-logikal
 ==============
 Common tools for Python testing implemented as a `pytest <https://docs.pytest.org/>`_ plugin.
 
 Getting Started
 ---------------
```

### Comparing `pytest_logikal-3.0.0/pytest_logikal.egg-info/SOURCES.txt` & `pytest_logikal-3.1.0/pytest_logikal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal.egg-info/entry_points.txt` & `pytest_logikal-3.1.0/pytest_logikal.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/pytest_logikal.egg-info/requires.txt` & `pytest_logikal-3.1.0/pytest_logikal.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 bandit==1.7.8
 coverage[toml]==7.5.1
 isort[colors]==5.13.2
 mypy==1.10.0
 pip-licenses==4.4.0
 pycodestyle==2.11.1
 pydocstyle[toml]==6.3.0
-pylint==3.2.0
-pytest==8.2.0
+pylint==3.2.2
+pytest==8.2.1
 pytest-cov==5.0.0
 pytest-mock==3.14.0
 pytest-mypy==0.10.3
 pytest-xdist[psutil]==3.6.1
 pillow~=10.3
 Pygments~=2.17
-logikal-utils~=1.0
+logikal-utils~=1.1
 pyorbs~=2.1
 termcolor~=2.4
 
 [black]
 black==24.4.2
 
 [browser]
-requests~=2.31
-types-requests~=2.31
+requests<2.32
+types-requests<2.32
 tqdm~=4.66
 types-tqdm~=4.66
 selenium==4.21.0
 xdg~=5.1
 
 [django]
 Babel~=2.14
 Django~=4.2
 django-stubs~=4.2
 django-migration-linter~=5.1
 djlint==1.34.1
 pylint-django==2.5.5
 pytest-django==4.8.0
 pytest-factoryboy==2.7.0
-requests~=2.31
-types-requests~=2.31
-logikal-utils[docker]~=1.0
+requests<2.32
+types-requests<2.32
+logikal-utils[docker]~=1.1
```

### Comparing `pytest_logikal-3.0.0/requirements/build.txt.lock` & `pytest_logikal-3.1.0/requirements/build.txt.lock`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.0.0/requirements/dev.txt.lock` & `pytest_logikal-3.1.0/requirements/dev.txt.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: e16b777fdd8e5cefd14494a404036eff582b427f3c9d362c4ce52831d22696d4
+##  Requirements hash: f41544170eeafc53ce555705b2513ad9b8019d8fc81a71c2a9d656e0ccbc615c
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 appdirs==1.4.4
 asgiref==3.8.1
-astroid==3.2.1
+astroid==3.2.2
 attrs==23.2.0
 Babel==2.15.0
 backports.tarfile==1.1.1
 backports.zoneinfo==0.2.1
 bandit==1.7.8
 black==24.4.2
 build==1.2.1
@@ -55,15 +55,15 @@
 jaraco.functools==4.0.1
 jeepney==0.8.0
 Jinja2==3.1.4
 jsbeautifier==1.15.1
 json5==0.9.25
 keyring==25.2.1
 logikal-docs==1.1.4
-logikal-utils==1.0.1
+logikal-utils==1.1.0
 markdown-it-py==3.0.0
 MarkupSafe==2.1.5
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==10.2.0
 mypy==1.10.0
 mypy-extensions==1.0.0
@@ -80,21 +80,21 @@
 pluggy==1.5.0
 prettytable==3.10.0
 psutil==5.9.8
 pycodestyle==2.11.1
 pycparser==2.22
 pydocstyle==6.3.0
 Pygments==2.18.0
-pylint==3.2.0
+pylint==3.2.2
 pylint-django==2.5.5
 pylint-plugin-utils==0.8.2
 pyorbs==2.1.0
 pyproject_hooks==1.1.0
 PySocks==1.7.1
-pytest==8.2.0
+pytest==8.2.1
 pytest-cov==5.0.0
 pytest-django==4.8.0
 pytest-factoryboy==2.7.0
 pytest-mock==3.14.0
 pytest-mypy==0.10.3
 pytest-xdist==3.6.1
 python-dateutil==2.9.0.post0
@@ -104,15 +104,15 @@
 regex==2023.12.25
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
 SecretStorage==3.3.3
 selenium==4.21.0
-setuptools==69.5.1
+setuptools==70.0.0
 six==1.16.0
 sniffio==1.3.1
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 Sphinx==7.1.2
 sphinx-rtd-theme==2.0.0
 sphinxcontrib-applehelp==1.0.4
```

### Comparing `pytest_logikal-3.0.0/requirements/docs.txt.lock` & `pytest_logikal-3.1.0/requirements/docs.txt.lock`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 519a3e2a8b754a3421dbdacf6d29f65e9572b79571813a4602a86387be35784d
+##  Requirements hash: 49046982207a816fa7a4a207626836f702b212515e8a94283769de8473b710b3
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 appdirs==1.4.4
 asgiref==3.8.1
-astroid==3.2.1
+astroid==3.2.2
 attrs==23.2.0
 Babel==2.15.0
 backports.zoneinfo==0.2.1
 bandit==1.7.8
 black==24.4.2
 certifi==2024.2.2
 charset-normalizer==3.3.2
@@ -45,15 +45,15 @@
 inflection==0.5.1
 iniconfig==2.0.0
 isort==5.13.2
 Jinja2==3.1.4
 jsbeautifier==1.15.1
 json5==0.9.25
 logikal-docs==1.1.4
-logikal-utils==1.0.1
+logikal-utils==1.1.0
 markdown-it-py==3.0.0
 MarkupSafe==2.1.5
 mccabe==0.7.0
 mdurl==0.1.2
 mypy==1.10.0
 mypy-extensions==1.0.0
 outcome==1.3.0.post0
@@ -66,34 +66,34 @@
 platformdirs==4.2.2
 pluggy==1.5.0
 prettytable==3.10.0
 psutil==5.9.8
 pycodestyle==2.11.1
 pydocstyle==6.3.0
 Pygments==2.18.0
-pylint==3.2.0
+pylint==3.2.2
 pylint-django==2.5.5
 pylint-plugin-utils==0.8.2
 pyorbs==2.1.0
 PySocks==1.7.1
-pytest==8.2.0
+pytest==8.2.1
 pytest-cov==5.0.0
 pytest-django==4.8.0
 pytest-factoryboy==2.7.0
 pytest-mock==3.14.0
 pytest-mypy==0.10.3
 pytest-xdist==3.6.1
 python-dateutil==2.9.0.post0
 pytz==2024.1
 PyYAML==6.0.1
 regex==2023.12.25
 requests==2.31.0
 rich==13.7.1
 selenium==4.21.0
-setuptools==69.5.1
+setuptools==70.0.0
 six==1.16.0
 sniffio==1.3.1
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 Sphinx==7.1.2
 sphinx-rtd-theme==2.0.0
 sphinxcontrib-applehelp==1.0.4
```

