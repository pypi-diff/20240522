# Comparing `tmp/holdup-5.1.0.tar.gz` & `tmp/holdup-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holdup-5.1.0.tar", last modified: Thu Apr 11 23:39:06 2024, max compression
+gzip compressed data, was "holdup-5.1.1.tar", last modified: Wed May 22 00:25:13 2024, max compression
```

## Comparing `holdup-5.1.0.tar` & `holdup-5.1.1.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.864210 holdup-5.1.0/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      735 2024-04-11 23:38:56.000000 holdup-5.1.0/.bumpversion.cfg
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1606 2024-04-11 23:38:56.000000 holdup-5.1.0/.cookiecutterrc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      174 2024-04-11 23:28:23.000000 holdup-5.1.0/.coveragerc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       22 2019-05-22 22:01:47.000000 holdup-5.1.0/.dockerignore
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2024-04-11 23:28:23.000000 holdup-5.1.0/.editorconfig
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.858210 holdup-5.1.0/.github/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.861210 holdup-5.1.0/.github/workflows/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     7585 2024-04-11 23:28:43.000000 holdup-5.1.0/.github/workflows/github-actions.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      702 2024-04-11 23:28:43.000000 holdup-5.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      282 2024-04-11 23:28:23.000000 holdup-5.1.0/.readthedocs.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      162 2024-04-11 23:28:43.000000 holdup-5.1.0/AUTHORS.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3114 2024-04-11 23:28:43.000000 holdup-5.1.0/CHANGELOG.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2341 2024-04-11 23:28:23.000000 holdup-5.1.0/CONTRIBUTING.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)      482 2024-04-10 23:12:41.000000 holdup-5.1.0/Dockerfile
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1330 2024-04-11 23:28:43.000000 holdup-5.1.0/LICENSE
--rw-r--r--   0 ionel     (1000) ionel     (1000)      519 2024-04-11 23:28:43.000000 holdup-5.1.0/MANIFEST.in
--rw-r--r--   0 ionel     (1000) ionel     (1000)     7886 2024-04-11 23:39:06.864210 holdup-5.1.0/PKG-INFO
--rw-r--r--   0 ionel     (1000) ionel     (1000)     4834 2024-04-11 23:38:56.000000 holdup-5.1.0/README.rst
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.861210 holdup-5.1.0/ci/
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2867 2024-04-11 23:28:23.000000 holdup-5.1.0/ci/bootstrap.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       72 2024-04-11 23:28:23.000000 holdup-5.1.0/ci/requirements.txt
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.858210 holdup-5.1.0/ci/templates/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.858210 holdup-5.1.0/ci/templates/.github/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.861210 holdup-5.1.0/ci/templates/.github/workflows/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2142 2024-04-11 23:28:23.000000 holdup-5.1.0/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.862210 holdup-5.1.0/docs/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       28 2024-04-11 23:28:24.000000 holdup-5.1.0/docs/authors.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       30 2024-04-11 23:28:24.000000 holdup-5.1.0/docs/changelog.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)      967 2024-04-11 23:38:56.000000 holdup-5.1.0/docs/conf.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       33 2024-04-11 23:28:24.000000 holdup-5.1.0/docs/contributing.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)      219 2024-04-11 23:28:43.000000 holdup-5.1.0/docs/index.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       27 2024-04-11 23:28:24.000000 holdup-5.1.0/docs/readme.rst
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.862210 holdup-5.1.0/docs/reference/
--rw-r--r--   0 ionel     (1000) ionel     (1000)      196 2024-04-11 23:28:43.000000 holdup-5.1.0/docs/reference/index.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       17 2024-04-11 23:28:23.000000 holdup-5.1.0/docs/requirements.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      109 2024-04-11 23:28:23.000000 holdup-5.1.0/docs/spelling_wordlist.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)      684 2024-04-10 23:05:47.000000 holdup-5.1.0/holdup.spec
--rw-r--r--   0 ionel     (1000) ionel     (1000)      526 2024-04-10 23:13:07.000000 holdup-5.1.0/pyinstaller.Dockerfile
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1352 2024-04-11 23:28:23.000000 holdup-5.1.0/pyproject.toml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      825 2024-04-11 23:28:43.000000 holdup-5.1.0/pytest.ini
--rw-r--r--   0 ionel     (1000) ionel     (1000)       38 2024-04-11 23:39:06.864210 holdup-5.1.0/setup.cfg
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2907 2024-04-11 23:38:56.000000 holdup-5.1.0/setup.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.859210 holdup-5.1.0/src/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.862210 holdup-5.1.0/src/holdup/
--rw-r--r--   0 ionel     (1000) ionel     (1000)       22 2024-04-11 23:38:56.000000 holdup-5.1.0/src/holdup/__init__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      382 2024-04-11 23:28:43.000000 holdup-5.1.0/src/holdup/__main__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     8071 2024-04-11 23:25:03.000000 holdup-5.1.0/src/holdup/checks.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     7329 2024-04-11 23:28:43.000000 holdup-5.1.0/src/holdup/cli.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      447 2024-04-11 23:13:41.000000 holdup-5.1.0/src/holdup/pg.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.864210 holdup-5.1.0/src/holdup.egg-info/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     7886 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/PKG-INFO
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1031 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/SOURCES.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/dependency_links.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)       43 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/entry_points.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/not-zip-safe
--rw-r--r--   0 ionel     (1000) ionel     (1000)       14 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/requires.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)        7 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/top_level.txt
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.864210 holdup-5.1.0/tests/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3024 2022-03-20 15:20:45.000000 holdup-5.1.0/tests/Dockerfile
--rw-r--r--   0 ionel     (1000) ionel     (1000)      233 2023-02-13 20:53:55.000000 holdup-5.1.0/tests/conftest.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      299 2024-04-10 23:15:17.000000 holdup-5.1.0/tests/docker-compose.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)    10663 2024-04-11 23:01:11.000000 holdup-5.1.0/tests/test_holdup.py
--rwxrwxr-x   0 ionel     (1000) ionel     (1000)      650 2019-05-26 20:51:27.000000 holdup-5.1.0/tests/test_pg.py
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)      520 2024-04-10 19:37:57.000000 holdup-5.1.0/tests/test_pg.sh
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1830 2024-04-11 23:28:43.000000 holdup-5.1.0/tox.ini
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-22 00:25:13.028031 holdup-5.1.1/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      735 2024-05-22 00:25:04.000000 holdup-5.1.1/.bumpversion.cfg
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1606 2024-05-22 00:25:04.000000 holdup-5.1.1/.cookiecutterrc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      174 2024-05-21 11:29:19.000000 holdup-5.1.1/.coveragerc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       22 2019-05-22 22:01:47.000000 holdup-5.1.1/.dockerignore
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2024-05-21 11:29:19.000000 holdup-5.1.1/.editorconfig
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-22 00:25:13.021031 holdup-5.1.1/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-22 00:25:13.024031 holdup-5.1.1/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     7553 2024-05-21 15:34:06.000000 holdup-5.1.1/.github/workflows/github-actions.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      678 2024-05-21 11:29:19.000000 holdup-5.1.1/.gitignore
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      702 2024-05-21 11:30:28.000000 holdup-5.1.1/.pre-commit-config.yaml
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      282 2024-05-21 11:29:19.000000 holdup-5.1.1/.readthedocs.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      162 2024-05-21 11:30:28.000000 holdup-5.1.1/AUTHORS.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3259 2024-05-21 11:35:41.000000 holdup-5.1.1/CHANGELOG.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2341 2024-05-21 11:29:19.000000 holdup-5.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      482 2024-04-10 23:12:41.000000 holdup-5.1.1/Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1330 2024-05-21 11:30:28.000000 holdup-5.1.1/LICENSE
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      519 2024-05-21 11:30:28.000000 holdup-5.1.1/MANIFEST.in
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     8031 2024-05-22 00:25:13.027031 holdup-5.1.1/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     4834 2024-05-22 00:25:04.000000 holdup-5.1.1/README.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-22 00:25:13.024031 holdup-5.1.1/ci/
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2867 2024-05-21 11:29:19.000000 holdup-5.1.1/ci/bootstrap.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       72 2024-05-21 11:29:19.000000 holdup-5.1.1/ci/requirements.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-22 00:25:13.022031 holdup-5.1.1/ci/templates/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-22 00:25:13.022031 holdup-5.1.1/ci/templates/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-22 00:25:13.024031 holdup-5.1.1/ci/templates/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2174 2024-05-21 15:31:09.000000 holdup-5.1.1/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-22 00:25:13.025031 holdup-5.1.1/docs/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       28 2024-05-21 11:29:19.000000 holdup-5.1.1/docs/authors.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       30 2024-05-21 11:29:19.000000 holdup-5.1.1/docs/changelog.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      967 2024-05-22 00:25:04.000000 holdup-5.1.1/docs/conf.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       33 2024-05-21 11:29:19.000000 holdup-5.1.1/docs/contributing.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      219 2024-05-21 11:30:28.000000 holdup-5.1.1/docs/index.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       27 2024-05-21 11:29:19.000000 holdup-5.1.1/docs/readme.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-22 00:25:13.025031 holdup-5.1.1/docs/reference/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      196 2024-05-21 11:30:28.000000 holdup-5.1.1/docs/reference/index.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       17 2024-05-21 11:29:19.000000 holdup-5.1.1/docs/requirements.txt
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      109 2024-05-21 11:29:19.000000 holdup-5.1.1/docs/spelling_wordlist.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      684 2024-04-10 23:05:47.000000 holdup-5.1.1/holdup.spec
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      526 2024-04-10 23:13:07.000000 holdup-5.1.1/pyinstaller.Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1352 2024-05-21 11:29:19.000000 holdup-5.1.1/pyproject.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      825 2024-05-21 11:30:28.000000 holdup-5.1.1/pytest.ini
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       38 2024-05-22 00:25:13.028031 holdup-5.1.1/setup.cfg
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2907 2024-05-22 00:25:04.000000 holdup-5.1.1/setup.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-22 00:25:13.022031 holdup-5.1.1/src/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-22 00:25:13.026031 holdup-5.1.1/src/holdup/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       22 2024-05-22 00:25:04.000000 holdup-5.1.1/src/holdup/__init__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      382 2024-05-21 11:30:28.000000 holdup-5.1.1/src/holdup/__main__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     8088 2024-05-21 11:32:19.000000 holdup-5.1.1/src/holdup/checks.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     7329 2024-05-21 11:30:28.000000 holdup-5.1.1/src/holdup/cli.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      447 2024-04-11 23:13:41.000000 holdup-5.1.1/src/holdup/pg.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-22 00:25:13.027031 holdup-5.1.1/src/holdup.egg-info/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     8031 2024-05-22 00:25:12.000000 holdup-5.1.1/src/holdup.egg-info/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1042 2024-05-22 00:25:12.000000 holdup-5.1.1/src/holdup.egg-info/SOURCES.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-05-22 00:25:12.000000 holdup-5.1.1/src/holdup.egg-info/dependency_links.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       43 2024-05-22 00:25:12.000000 holdup-5.1.1/src/holdup.egg-info/entry_points.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-05-22 00:25:11.000000 holdup-5.1.1/src/holdup.egg-info/not-zip-safe
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       14 2024-05-22 00:25:12.000000 holdup-5.1.1/src/holdup.egg-info/requires.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        7 2024-05-22 00:25:12.000000 holdup-5.1.1/src/holdup.egg-info/top_level.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-22 00:25:13.027031 holdup-5.1.1/tests/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3024 2022-03-20 15:20:45.000000 holdup-5.1.1/tests/Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      233 2023-02-13 20:53:55.000000 holdup-5.1.1/tests/conftest.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      299 2024-04-10 23:15:17.000000 holdup-5.1.1/tests/docker-compose.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    10779 2024-05-21 15:34:46.000000 holdup-5.1.1/tests/test_holdup.py
+-rwxrwxr-x   0 ionel     (1000) ionel     (1000)      650 2019-05-26 20:51:27.000000 holdup-5.1.1/tests/test_pg.py
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)      520 2024-04-10 19:37:57.000000 holdup-5.1.1/tests/test_pg.sh
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1830 2024-05-21 11:30:28.000000 holdup-5.1.1/tox.ini
```

### Comparing `holdup-5.1.0/.bumpversion.cfg` & `holdup-5.1.1/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 5.1.0
+current_version = 5.1.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `holdup-5.1.0/.cookiecutterrc` & `holdup-5.1.1/.cookiecutterrc`

 * *Files 5% similar despite different names*

```diff
@@ -36,12 +36,12 @@
     setup_py_uses_setuptools_scm: 'no'
     sphinx_docs: 'yes'
     sphinx_docs_hosting: https://python-holdup.readthedocs.io/
     sphinx_doctest: 'no'
     sphinx_theme: furo
     test_matrix_separate_coverage: 'no'
     tests_inside_package: 'no'
-    version: 5.1.0
+    version: 5.1.1
     version_manager: bump2version
     website: https://blog.ionelmc.ro
     year_from: '2016'
     year_to: '2024'
```

### Comparing `holdup-5.1.0/.github/workflows/github-actions.yml` & `holdup-5.1.1/.github/workflows/github-actions.yml`

 * *Files 3% similar despite different names*

```diff
@@ -24,196 +24,196 @@
             toxpython: 'python3.8'
             python_arch: 'x64'
             tox_env: 'py38-pg2'
             os: 'ubuntu-latest'
           - name: 'py38-pg2 (macos)'
             python: '3.8'
             toxpython: 'python3.8'
-            python_arch: 'x64'
-            tox_env: 'py38-pg2'
+            python_arch: 'arm64'
+            tox_env: 'py38'
             os: 'macos-latest'
           - name: 'py38-pg3 (ubuntu)'
             python: '3.8'
             toxpython: 'python3.8'
             python_arch: 'x64'
             tox_env: 'py38-pg3'
             os: 'ubuntu-latest'
           - name: 'py38-pg3 (macos)'
             python: '3.8'
             toxpython: 'python3.8'
-            python_arch: 'x64'
-            tox_env: 'py38-pg3'
+            python_arch: 'arm64'
+            tox_env: 'py38'
             os: 'macos-latest'
           - name: 'py39-pg2 (ubuntu)'
             python: '3.9'
             toxpython: 'python3.9'
             python_arch: 'x64'
             tox_env: 'py39-pg2'
             os: 'ubuntu-latest'
           - name: 'py39-pg2 (macos)'
             python: '3.9'
             toxpython: 'python3.9'
-            python_arch: 'x64'
-            tox_env: 'py39-pg2'
+            python_arch: 'arm64'
+            tox_env: 'py39'
             os: 'macos-latest'
           - name: 'py39-pg3 (ubuntu)'
             python: '3.9'
             toxpython: 'python3.9'
             python_arch: 'x64'
             tox_env: 'py39-pg3'
             os: 'ubuntu-latest'
           - name: 'py39-pg3 (macos)'
             python: '3.9'
             toxpython: 'python3.9'
-            python_arch: 'x64'
-            tox_env: 'py39-pg3'
+            python_arch: 'arm64'
+            tox_env: 'py39'
             os: 'macos-latest'
           - name: 'py310-pg2 (ubuntu)'
             python: '3.10'
             toxpython: 'python3.10'
             python_arch: 'x64'
             tox_env: 'py310-pg2'
             os: 'ubuntu-latest'
           - name: 'py310-pg2 (macos)'
             python: '3.10'
             toxpython: 'python3.10'
-            python_arch: 'x64'
-            tox_env: 'py310-pg2'
+            python_arch: 'arm64'
+            tox_env: 'py310'
             os: 'macos-latest'
           - name: 'py310-pg3 (ubuntu)'
             python: '3.10'
             toxpython: 'python3.10'
             python_arch: 'x64'
             tox_env: 'py310-pg3'
             os: 'ubuntu-latest'
           - name: 'py310-pg3 (macos)'
             python: '3.10'
             toxpython: 'python3.10'
-            python_arch: 'x64'
-            tox_env: 'py310-pg3'
+            python_arch: 'arm64'
+            tox_env: 'py310'
             os: 'macos-latest'
           - name: 'py311-pg2 (ubuntu)'
             python: '3.11'
             toxpython: 'python3.11'
             python_arch: 'x64'
             tox_env: 'py311-pg2'
             os: 'ubuntu-latest'
           - name: 'py311-pg2 (macos)'
             python: '3.11'
             toxpython: 'python3.11'
-            python_arch: 'x64'
-            tox_env: 'py311-pg2'
+            python_arch: 'arm64'
+            tox_env: 'py311'
             os: 'macos-latest'
           - name: 'py311-pg3 (ubuntu)'
             python: '3.11'
             toxpython: 'python3.11'
             python_arch: 'x64'
             tox_env: 'py311-pg3'
             os: 'ubuntu-latest'
           - name: 'py311-pg3 (macos)'
             python: '3.11'
             toxpython: 'python3.11'
-            python_arch: 'x64'
-            tox_env: 'py311-pg3'
+            python_arch: 'arm64'
+            tox_env: 'py311'
             os: 'macos-latest'
           - name: 'py312-pg2 (ubuntu)'
             python: '3.12'
             toxpython: 'python3.12'
             python_arch: 'x64'
             tox_env: 'py312-pg2'
             os: 'ubuntu-latest'
           - name: 'py312-pg2 (macos)'
             python: '3.12'
             toxpython: 'python3.12'
-            python_arch: 'x64'
-            tox_env: 'py312-pg2'
+            python_arch: 'arm64'
+            tox_env: 'py312'
             os: 'macos-latest'
           - name: 'py312-pg3 (ubuntu)'
             python: '3.12'
             toxpython: 'python3.12'
             python_arch: 'x64'
             tox_env: 'py312-pg3'
             os: 'ubuntu-latest'
           - name: 'py312-pg3 (macos)'
             python: '3.12'
             toxpython: 'python3.12'
-            python_arch: 'x64'
-            tox_env: 'py312-pg3'
+            python_arch: 'arm64'
+            tox_env: 'py312'
             os: 'macos-latest'
           - name: 'pypy38-pg2 (ubuntu)'
             python: 'pypy-3.8'
             toxpython: 'pypy3.8'
             python_arch: 'x64'
             tox_env: 'pypy38-pg2'
             os: 'ubuntu-latest'
           - name: 'pypy38-pg2 (macos)'
             python: 'pypy-3.8'
             toxpython: 'pypy3.8'
-            python_arch: 'x64'
-            tox_env: 'pypy38-pg2'
+            python_arch: 'arm64'
+            tox_env: 'pypy38'
             os: 'macos-latest'
           - name: 'pypy38-pg3 (ubuntu)'
             python: 'pypy-3.8'
             toxpython: 'pypy3.8'
             python_arch: 'x64'
             tox_env: 'pypy38-pg3'
             os: 'ubuntu-latest'
           - name: 'pypy38-pg3 (macos)'
             python: 'pypy-3.8'
             toxpython: 'pypy3.8'
-            python_arch: 'x64'
-            tox_env: 'pypy38-pg3'
+            python_arch: 'arm64'
+            tox_env: 'pypy38'
             os: 'macos-latest'
           - name: 'pypy39-pg2 (ubuntu)'
             python: 'pypy-3.9'
             toxpython: 'pypy3.9'
             python_arch: 'x64'
             tox_env: 'pypy39-pg2'
             os: 'ubuntu-latest'
           - name: 'pypy39-pg2 (macos)'
             python: 'pypy-3.9'
             toxpython: 'pypy3.9'
-            python_arch: 'x64'
-            tox_env: 'pypy39-pg2'
+            python_arch: 'arm64'
+            tox_env: 'pypy39'
             os: 'macos-latest'
           - name: 'pypy39-pg3 (ubuntu)'
             python: 'pypy-3.9'
             toxpython: 'pypy3.9'
             python_arch: 'x64'
             tox_env: 'pypy39-pg3'
             os: 'ubuntu-latest'
           - name: 'pypy39-pg3 (macos)'
             python: 'pypy-3.9'
             toxpython: 'pypy3.9'
-            python_arch: 'x64'
-            tox_env: 'pypy39-pg3'
+            python_arch: 'arm64'
+            tox_env: 'pypy39'
             os: 'macos-latest'
           - name: 'pypy310-pg2 (ubuntu)'
             python: 'pypy-3.10'
             toxpython: 'pypy3.10'
             python_arch: 'x64'
             tox_env: 'pypy310-pg2'
             os: 'ubuntu-latest'
           - name: 'pypy310-pg2 (macos)'
             python: 'pypy-3.10'
             toxpython: 'pypy3.10'
-            python_arch: 'x64'
-            tox_env: 'pypy310-pg2'
+            python_arch: 'arm64'
+            tox_env: 'pypy310'
             os: 'macos-latest'
           - name: 'pypy310-pg3 (ubuntu)'
             python: 'pypy-3.10'
             toxpython: 'pypy3.10'
             python_arch: 'x64'
             tox_env: 'pypy310-pg3'
             os: 'ubuntu-latest'
           - name: 'pypy310-pg3 (macos)'
             python: 'pypy-3.10'
             toxpython: 'pypy3.10'
-            python_arch: 'x64'
-            tox_env: 'pypy310-pg3'
+            python_arch: 'arm64'
+            tox_env: 'pypy310'
             os: 'macos-latest'
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - uses: actions/setup-python@v5
       with:
```

### Comparing `holdup-5.1.0/.pre-commit-config.yaml` & `holdup-5.1.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #   pre-commit install --install-hooks
 # To update the versions:
 #   pre-commit autoupdate
 exclude: '^(\.tox|ci/templates|\.bumpversion\.cfg)(/|$)'
 # Note the order is intentional to avoid multiple passes of the hooks
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.4.4
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix, --show-fixes, --unsafe-fixes]
   - repo: https://github.com/psf/black
-    rev: 24.3.0
+    rev: 24.4.2
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.6.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
```

### Comparing `holdup-5.1.0/CHANGELOG.rst` & `holdup-5.1.1/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 
 Changelog
 =========
 
+5.1.1 (2024-05-21)
+------------------
+
+* Do not display an authentication mask for http protocols if there are no actual credentials specified.
+
 5.1.0 (2024-04-12)
 ------------------
 
 * Fixed buggy handling when http checks are specified with a port.
 * Changed User-Agent header and stripped port from Host header for http checks.
 * Refactored a bunch of code into a separate ``holdup.checks`` module.
```

### Comparing `holdup-5.1.0/CONTRIBUTING.rst` & `holdup-5.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `holdup-5.1.0/LICENSE` & `holdup-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `holdup-5.1.0/MANIFEST.in` & `holdup-5.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `holdup-5.1.0/PKG-INFO` & `holdup-5.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holdup
-Version: 5.1.0
+Version: 5.1.1
 Summary: A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services (like almost everything).
 Home-page: https://github.com/ionelmc/python-holdup
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Documentation, https://python-holdup.readthedocs.io/
 Project-URL: Changelog, https://python-holdup.readthedocs.io/en/latest/changelog.html
@@ -135,14 +135,19 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+5.1.1 (2024-05-21)
+------------------
+
+* Do not display an authentication mask for http protocols if there are no actual credentials specified.
+
 5.1.0 (2024-04-12)
 ------------------
 
 * Fixed buggy handling when http checks are specified with a port.
 * Changed User-Agent header and stripped port from Host header for http checks.
 * Refactored a bunch of code into a separate ``holdup.checks`` module.
```

### Comparing `holdup-5.1.0/README.rst` & `holdup-5.1.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/holdup
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/holdup.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/holdup
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-holdup/v5.1.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-holdup/v5.1.1.svg
     :alt: Commits since latest release
-    :target: https://github.com/ionelmc/python-holdup/compare/v5.1.0...master
+    :target: https://github.com/ionelmc/python-holdup/compare/v5.1.1...master
 
 
 
 .. end-badges
 
 A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services
 (like almost everything).
```

### Comparing `holdup-5.1.0/ci/bootstrap.py` & `holdup-5.1.1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `holdup-5.1.0/ci/templates/.github/workflows/github-actions.yml` & `holdup-5.1.1/ci/templates/.github/workflows/github-actions.yml`

 * *Files 6% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 {% else %}
 {% set python %}{{ prefix[2] }}.{{ prefix[3:] }}{% endset %}
 {% set cpython %}cp{{ prefix[2:] }}{% endset %}
 {% set toxpython %}python{{ prefix[2] }}.{{ prefix[3:] }}{% endset %}
 {% endif %}
 {% for os, python_arch in [
     ['ubuntu', 'x64'],
-    ['macos', 'x64'],
+    ['macos', 'arm64'],
 ] %}
           - name: '{{ env }} ({{ os }})'
             python: '{{ python }}'
             toxpython: '{{ toxpython }}'
             python_arch: '{{ python_arch }}'
-            tox_env: '{{ env }}'
+            tox_env: '{{ env if os == 'ubuntu' else prefix }}'
             os: '{{ os }}-latest'
 {% endfor %}
 {% endfor %}
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
```

### Comparing `holdup-5.1.0/docs/conf.py` & `holdup-5.1.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "Holdup"
 year = "2016-2024"
 author = "Ionel Cristian Mărieș"
 copyright = f"{year}, {author}"
-version = release = "5.1.0"
+version = release = "5.1.1"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/ionelmc/python-holdup/issues/%s", "#%s"),
     "pr": ("https://github.com/ionelmc/python-holdup/pull/%s", "PR #%s"),
 }
```

### Comparing `holdup-5.1.0/holdup.spec` & `holdup-5.1.1/holdup.spec`

 * *Files identical despite different names*

### Comparing `holdup-5.1.0/pyinstaller.Dockerfile` & `holdup-5.1.1/pyinstaller.Dockerfile`

 * *Files identical despite different names*

### Comparing `holdup-5.1.0/pyproject.toml` & `holdup-5.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `holdup-5.1.0/pytest.ini` & `holdup-5.1.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `holdup-5.1.0/setup.py` & `holdup-5.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="holdup",
-    version="5.1.0",
+    version="5.1.1",
     license="BSD-2-Clause",
     description="A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services (like almost everything).",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="Ionel Cristian Mărieș",
```

### Comparing `holdup-5.1.0/src/holdup/checks.py` & `holdup-5.1.1/src/holdup/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                 raise Exception(f"Expected status code 200, got {status!r}")
 
     def __repr__(self):
         return f"HttpCheck({self.url}, insecure={self.insecure}, status={self.status})"
 
     def display_definition(self, *, verbose_passwords):
         url = self.parsed_url
-        if not verbose_passwords:
+        if url.username and not verbose_passwords:
             if not url.password:
                 mask = "******"
             else:
                 mask = f"{url.username}:******"
             url = url._replace(netloc=f"{mask}@{self.netloc}")
         return urlunparse(url)
```

### Comparing `holdup-5.1.0/src/holdup/cli.py` & `holdup-5.1.1/src/holdup/cli.py`

 * *Files identical despite different names*

### Comparing `holdup-5.1.0/src/holdup.egg-info/PKG-INFO` & `holdup-5.1.1/src/holdup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holdup
-Version: 5.1.0
+Version: 5.1.1
 Summary: A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services (like almost everything).
 Home-page: https://github.com/ionelmc/python-holdup
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Documentation, https://python-holdup.readthedocs.io/
 Project-URL: Changelog, https://python-holdup.readthedocs.io/en/latest/changelog.html
@@ -135,14 +135,19 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+5.1.1 (2024-05-21)
+------------------
+
+* Do not display an authentication mask for http protocols if there are no actual credentials specified.
+
 5.1.0 (2024-04-12)
 ------------------
 
 * Fixed buggy handling when http checks are specified with a port.
 * Changed User-Agent header and stripped port from Host header for http checks.
 * Refactored a bunch of code into a separate ``holdup.checks`` module.
```

### Comparing `holdup-5.1.0/src/holdup.egg-info/SOURCES.txt` & `holdup-5.1.1/src/holdup.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .bumpversion.cfg
 .cookiecutterrc
 .coveragerc
 .dockerignore
 .editorconfig
+.gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 Dockerfile
 LICENSE
```

### Comparing `holdup-5.1.0/tests/Dockerfile` & `holdup-5.1.1/tests/Dockerfile`

 * *Files identical despite different names*

### Comparing `holdup-5.1.0/tests/test_holdup.py` & `holdup-5.1.1/tests/test_holdup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # ruff: noqa: PTH110, PTH120, PTH123
 import os
+import platform
 import shutil
 import socket
 import threading
 
 import pytest
 
 pytest_plugins = ("pytester",)
@@ -179,20 +180,20 @@
 
 
 def test_any_failed(testdir):
     tcp = socket.socket()
     tcp.bind(("127.0.0.1", 0))
     _, port = tcp.getsockname()
 
-    result = testdir.run("holdup", "-t", "0.5", "tcp://localhost:%s/,path:///doesnt/exist,unix:///doesnt/exist" % port)
+    result = testdir.run("holdup", "-t", "0.5", f"tcp://localhost:{port}/,path:///doesnt/exist,unix:///doesnt/exist")
     result.stderr.fnmatch_lines(
         [
-            "holdup: Failed checks: any('tcp://localhost:%s' -> *, 'path:///doesnt/exist' -> *, "
+            f"holdup: Failed checks: any('tcp://localhost:{port}' -> *, 'path:///doesnt/exist' -> *, "
             "'unix:///doesnt/exist' -> *) -> ALL FAILED. "
-            "Aborting!" % port,
+            "Aborting!",
         ]
     )
     tcp.close()
 
 
 def test_no_abort(testdir, extra):
     result = testdir.run(
@@ -207,15 +208,15 @@
     )
 
 
 @pytest.mark.skipif(os.path.exists("/.dockerenv"), reason="chmod(0) does not work in docker")
 def test_not_readable(testdir, extra):
     foobar = testdir.maketxtfile(foobar="")
     foobar.chmod(0)
-    result = testdir.run("holdup", "-t", "0.1", "-n", "path://%s" % foobar, *extra)
+    result = testdir.run("holdup", "-t", "0.1", "-n", f"path://{foobar}", *extra)
     result.stderr.fnmatch_lines(
         [
             f"holdup: Failed checks: 'path://{foobar}' -> Failed access('{foobar}', R_OK) test. "
             "Treating as success because of --no-abort.",
         ]
     )
 
@@ -269,14 +270,15 @@
 def test_eval_comma_anycheck(testdir, extra):
     result = testdir.run("holdup", 'path://whatever123,eval://os.path.join("foo", "bar")', *extra)
     if extra:
         result.stdout.fnmatch_lines(["success !"])
     assert result.ret == 0
 
 
+@pytest.mark.skipif(platform.system() != "Linux", reason="too complicated to install psycopg on non-linux")
 @pytest.mark.parametrize("proto", ["postgresql", "postgres", "pg"])
 def test_pg_timeout(testdir, proto):
     result = testdir.run("holdup", "-t", "0.1", proto + "://0.0.0.0/foo")
     result.stderr.fnmatch_lines(
         [
             "holdup: Failed checks: 'postgresql://0.0.0.0/foo' -> *",
         ]
@@ -290,15 +292,15 @@
     testdir.tmpdir.join("psycopg2").ensure(dir=1)
     testdir.tmpdir.join("psycopg2/__init__.py").write('raise ImportError("Disabled for testing")')
     testdir.tmpdir.join("psycopg").ensure(dir=1)
     testdir.tmpdir.join("psycopg/__init__.py").write('raise ImportError("Disabled for testing")')
     result = testdir.run("holdup", "-t", "0.1", proto + ":///")
     result.stderr.fnmatch_lines(
         [
-            "holdup: error: argument service: Protocol %s unusable. Install holdup[[]pg[]]." % proto,
+            f"holdup: error: argument service: Protocol {proto} unusable. Install holdup[[]pg[]].",
         ]
     )
 
 
 @pytest.fixture
 def testdir2(testdir):
     os.chdir(os.path.dirname(__file__))
```

### Comparing `holdup-5.1.0/tests/test_pg.py` & `holdup-5.1.1/tests/test_pg.py`

 * *Files identical despite different names*

### Comparing `holdup-5.1.0/tests/test_pg.sh` & `holdup-5.1.1/tests/test_pg.sh`

 * *Files identical despite different names*

### Comparing `holdup-5.1.0/tox.ini` & `holdup-5.1.1/tox.ini`

 * *Files identical despite different names*

