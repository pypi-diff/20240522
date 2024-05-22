# Comparing `tmp/swh.vault-1.9.2.tar.gz` & `tmp/swh.vault-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.vault-1.9.2.tar", last modified: Mon Oct 23 09:37:39 2023, max compression
+gzip compressed data, was "swh.vault-1.9.3.tar", last modified: Wed Oct 25 11:52:31 2023, max compression
```

## Comparing `swh.vault-1.9.2.tar` & `swh.vault-1.9.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:39.095187 swh.vault-1.9.2/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2023-10-23 09:37:31.000000 swh.vault-1.9.2/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      113 2023-10-23 09:37:31.000000 swh.vault-1.9.2/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      848 2023-10-23 09:37:31.000000 swh.vault-1.9.2/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2023-10-23 09:37:31.000000 swh.vault-1.9.2/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2023-10-23 09:37:31.000000 swh.vault-1.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2023-10-23 09:37:31.000000 swh.vault-1.9.2/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2023-10-23 09:37:31.000000 swh.vault-1.9.2/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      248 2023-10-23 09:37:31.000000 swh.vault-1.9.2/MANIFEST.in
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2023-10-23 09:37:31.000000 swh.vault-1.9.2/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2384 2023-10-23 09:37:39.095187 swh.vault-1.9.2/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)      412 2023-10-23 09:37:31.000000 swh.vault-1.9.2/README.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      305 2023-10-23 09:37:31.000000 swh.vault-1.9.2/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:39.075188 swh.vault-1.9.2/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2023-10-23 09:37:31.000000 swh.vault-1.9.2/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       39 2023-10-23 09:37:31.000000 swh.vault-1.9.2/docs/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      412 2023-10-23 09:37:31.000000 swh.vault-1.9.2/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:39.075188 swh.vault-1.9.2/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:31.000000 swh.vault-1.9.2/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:39.075188 swh.vault-1.9.2/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:31.000000 swh.vault-1.9.2/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5190 2023-10-23 09:37:31.000000 swh.vault-1.9.2/docs/api.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      133 2023-10-23 09:37:31.000000 swh.vault-1.9.2/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2023-10-23 09:37:31.000000 swh.vault-1.9.2/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1791 2023-10-23 09:37:31.000000 swh.vault-1.9.2/docs/getting-started.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1606 2023-10-23 09:37:31.000000 swh.vault-1.9.2/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      458 2023-10-23 09:37:31.000000 swh.vault-1.9.2/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)      237 2023-10-23 09:37:31.000000 swh.vault-1.9.2/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      122 2023-10-23 09:37:31.000000 swh.vault-1.9.2/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2023-10-23 09:37:31.000000 swh.vault-1.9.2/requirements-swh-graph.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      102 2023-10-23 09:37:31.000000 swh.vault-1.9.2/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      200 2023-10-23 09:37:31.000000 swh.vault-1.9.2/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       77 2023-10-23 09:37:31.000000 swh.vault-1.9.2/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2023-10-23 09:37:39.099187 swh.vault-1.9.2/setup.cfg
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     2413 2023-10-23 09:37:31.000000 swh.vault-1.9.2/setup.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:39.079187 swh.vault-1.9.2/swh/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       76 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:39.083187 swh.vault-1.9.2/swh/vault/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1709 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:39.083187 swh.vault-1.9.2/swh/vault/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/api/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      655 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/api/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      499 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/api/serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3312 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/api/server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    19048 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/backend.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1959 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/cache.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5322 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/cli.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:39.087187 swh.vault-1.9.2/swh/vault/cookers/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4154 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/cookers/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5429 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/cookers/base.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1046 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/cookers/directory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    30066 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/cookers/git_bare.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1435 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/cookers/revision_flat.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9075 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/cookers/revision_gitfast.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1869 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/cookers/utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      821 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/cooking_tasks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      287 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/exc.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1917 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/in_memory_backend.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2668 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/py.typed
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:39.087187 swh.vault-1.9.2/swh/vault/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1728 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/sql/30-schema.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:39.087187 swh.vault-1.9.2/swh/vault/sql/upgrades/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      975 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/sql/upgrades/002.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      879 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/sql/upgrades/003.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:39.091187 swh.vault-1.9.2/swh/vault/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      100 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2661 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/tests/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16565 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/tests/test_backend.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2585 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/tests/test_cache.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5143 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    44985 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/tests/test_cookers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2929 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/tests/test_cookers_base.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20291 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/tests/test_git_bare_cooker.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1848 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/tests/test_init.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3403 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/tests/test_init_cookers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6196 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/tests/test_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5132 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/tests/test_to_disk.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      586 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/tests/vault_testing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5479 2023-10-23 09:37:31.000000 swh.vault-1.9.2/swh/vault/to_disk.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-23 09:37:39.079187 swh.vault-1.9.2/swh.vault.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2384 2023-10-23 09:37:39.000000 swh.vault-1.9.2/swh.vault.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1770 2023-10-23 09:37:39.000000 swh.vault-1.9.2/swh.vault.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2023-10-23 09:37:39.000000 swh.vault-1.9.2/swh.vault.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       44 2023-10-23 09:37:39.000000 swh.vault-1.9.2/swh.vault.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2023-10-23 09:37:39.000000 swh.vault-1.9.2/swh.vault.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (115) jenkins    (120)      398 2023-10-23 09:37:39.000000 swh.vault-1.9.2/swh.vault.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2023-10-23 09:37:39.000000 swh.vault-1.9.2/swh.vault.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1507 2023-10-23 09:37:31.000000 swh.vault-1.9.2/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:31.587351 swh.vault-1.9.3/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2023-10-25 11:52:24.000000 swh.vault-1.9.3/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      113 2023-10-25 11:52:24.000000 swh.vault-1.9.3/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      848 2023-10-25 11:52:24.000000 swh.vault-1.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2023-10-25 11:52:24.000000 swh.vault-1.9.3/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2023-10-25 11:52:24.000000 swh.vault-1.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2023-10-25 11:52:24.000000 swh.vault-1.9.3/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2023-10-25 11:52:24.000000 swh.vault-1.9.3/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      248 2023-10-25 11:52:24.000000 swh.vault-1.9.3/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2023-10-25 11:52:24.000000 swh.vault-1.9.3/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2384 2023-10-25 11:52:31.587351 swh.vault-1.9.3/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      412 2023-10-25 11:52:24.000000 swh.vault-1.9.3/README.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      305 2023-10-25 11:52:24.000000 swh.vault-1.9.3/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:31.563351 swh.vault-1.9.3/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2023-10-25 11:52:24.000000 swh.vault-1.9.3/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       39 2023-10-25 11:52:24.000000 swh.vault-1.9.3/docs/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      412 2023-10-25 11:52:24.000000 swh.vault-1.9.3/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:31.563351 swh.vault-1.9.3/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:24.000000 swh.vault-1.9.3/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:31.563351 swh.vault-1.9.3/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:24.000000 swh.vault-1.9.3/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5190 2023-10-25 11:52:24.000000 swh.vault-1.9.3/docs/api.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      133 2023-10-25 11:52:24.000000 swh.vault-1.9.3/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2023-10-25 11:52:24.000000 swh.vault-1.9.3/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1791 2023-10-25 11:52:24.000000 swh.vault-1.9.3/docs/getting-started.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1606 2023-10-25 11:52:24.000000 swh.vault-1.9.3/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      458 2023-10-25 11:52:24.000000 swh.vault-1.9.3/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      237 2023-10-25 11:52:24.000000 swh.vault-1.9.3/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      122 2023-10-25 11:52:24.000000 swh.vault-1.9.3/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2023-10-25 11:52:24.000000 swh.vault-1.9.3/requirements-swh-graph.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      102 2023-10-25 11:52:24.000000 swh.vault-1.9.3/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      200 2023-10-25 11:52:24.000000 swh.vault-1.9.3/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       77 2023-10-25 11:52:24.000000 swh.vault-1.9.3/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2023-10-25 11:52:31.587351 swh.vault-1.9.3/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     2413 2023-10-25 11:52:24.000000 swh.vault-1.9.3/setup.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:31.571351 swh.vault-1.9.3/swh/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       76 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:31.575351 swh.vault-1.9.3/swh/vault/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1709 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:31.575351 swh.vault-1.9.3/swh/vault/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/api/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      655 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/api/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      499 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/api/serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3312 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/api/server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    19048 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/backend.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1959 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/cache.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5322 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/cli.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:31.579351 swh.vault-1.9.3/swh/vault/cookers/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4154 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/cookers/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5429 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/cookers/base.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1046 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/cookers/directory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    30073 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/cookers/git_bare.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1435 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/cookers/revision_flat.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9075 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/cookers/revision_gitfast.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1869 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/cookers/utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      821 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/cooking_tasks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      287 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/exc.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1917 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/in_memory_backend.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2668 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/py.typed
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:31.579351 swh.vault-1.9.3/swh/vault/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1728 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/sql/30-schema.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:31.579351 swh.vault-1.9.3/swh/vault/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      975 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/sql/upgrades/002.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      879 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/sql/upgrades/003.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:31.583351 swh.vault-1.9.3/swh/vault/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      100 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2661 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16565 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/tests/test_backend.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2585 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/tests/test_cache.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5143 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    44985 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/tests/test_cookers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2929 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/tests/test_cookers_base.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20728 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/tests/test_git_bare_cooker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1848 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3403 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/tests/test_init_cookers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6196 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5132 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/tests/test_to_disk.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      586 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/tests/vault_testing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5479 2023-10-25 11:52:24.000000 swh.vault-1.9.3/swh/vault/to_disk.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-10-25 11:52:31.571351 swh.vault-1.9.3/swh.vault.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2384 2023-10-25 11:52:31.000000 swh.vault-1.9.3/swh.vault.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1770 2023-10-25 11:52:31.000000 swh.vault-1.9.3/swh.vault.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2023-10-25 11:52:31.000000 swh.vault-1.9.3/swh.vault.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       44 2023-10-25 11:52:31.000000 swh.vault-1.9.3/swh.vault.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2023-10-25 11:52:31.000000 swh.vault-1.9.3/swh.vault.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      398 2023-10-25 11:52:31.000000 swh.vault-1.9.3/swh.vault.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2023-10-25 11:52:31.000000 swh.vault-1.9.3/swh.vault.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1507 2023-10-25 11:52:24.000000 swh.vault-1.9.3/tox.ini
```

### Comparing `swh.vault-1.9.2/.pre-commit-config.yaml` & `swh.vault-1.9.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/CODE_OF_CONDUCT.md` & `swh.vault-1.9.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/LICENSE` & `swh.vault-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/PKG-INFO` & `swh.vault-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.vault
-Version: 1.9.2
+Version: 1.9.3
 Summary: Software Heritage vault
 Home-page: https://forge.softwareheritage.org/diffusion/DVAU/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-vault
```

### Comparing `swh.vault-1.9.2/docs/api.rst` & `swh.vault-1.9.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/docs/getting-started.rst` & `swh.vault-1.9.3/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/docs/index.rst` & `swh.vault-1.9.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/setup.py` & `swh.vault-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/__init__.py` & `swh.vault-1.9.3/swh/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/api/client.py` & `swh.vault-1.9.3/swh/vault/api/client.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/api/server.py` & `swh.vault-1.9.3/swh/vault/api/server.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/backend.py` & `swh.vault-1.9.3/swh/vault/backend.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/cache.py` & `swh.vault-1.9.3/swh/vault/cache.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/cli.py` & `swh.vault-1.9.3/swh/vault/cli.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/cookers/__init__.py` & `swh.vault-1.9.3/swh/vault/cookers/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/cookers/base.py` & `swh.vault-1.9.3/swh/vault/cookers/base.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/cookers/directory.py` & `swh.vault-1.9.3/swh/vault/cookers/directory.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/cookers/git_bare.py` & `swh.vault-1.9.3/swh/vault/cookers/git_bare.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,17 +297,17 @@
             else:
                 release_name = b"release"
 
             refs = {
                 b"refs/tags/" + release_name: hash_to_bytehex(self.obj_id),
             }
 
-            if release.target_type.value == ModelObjectType.REVISION:
+            if release.target_type.value == ModelObjectType.REVISION.value:
                 # Not necessary, but makes it easier to browse
-                refs[b"ref/heads/master"] = hash_to_bytehex(release.target)
+                refs[b"refs/heads/master"] = hash_to_bytehex(release.target)
             # TODO: synthesize a master branch for other target types
 
         elif self.obj_type is RootObjectType.SNAPSHOT:
             if snapshot is None:
                 # refs were already written in a previous step
                 return
             branches = []
```

### Comparing `swh.vault-1.9.2/swh/vault/cookers/revision_flat.py` & `swh.vault-1.9.3/swh/vault/cookers/revision_flat.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/cookers/revision_gitfast.py` & `swh.vault-1.9.3/swh/vault/cookers/revision_gitfast.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/cookers/utils.py` & `swh.vault-1.9.3/swh/vault/cookers/utils.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/cooking_tasks.py` & `swh.vault-1.9.3/swh/vault/cooking_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/in_memory_backend.py` & `swh.vault-1.9.3/swh/vault/in_memory_backend.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/interface.py` & `swh.vault-1.9.3/swh/vault/interface.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/sql/30-schema.sql` & `swh.vault-1.9.3/swh/vault/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/sql/upgrades/002.sql` & `swh.vault-1.9.3/swh/vault/sql/upgrades/002.sql`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/sql/upgrades/003.sql` & `swh.vault-1.9.3/swh/vault/sql/upgrades/003.sql`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/tests/conftest.py` & `swh.vault-1.9.3/swh/vault/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/tests/test_backend.py` & `swh.vault-1.9.3/swh/vault/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/tests/test_cache.py` & `swh.vault-1.9.3/swh/vault/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/tests/test_cli.py` & `swh.vault-1.9.3/swh/vault/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/tests/test_cookers.py` & `swh.vault-1.9.3/swh/vault/tests/test_cookers.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/tests/test_cookers_base.py` & `swh.vault-1.9.3/swh/vault/tests/test_cookers_base.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/tests/test_git_bare_cooker.py` & `swh.vault-1.9.3/swh/vault/tests/test_git_bare_cooker.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 run on the bare cooker.
 """
 
 import datetime
 import enum
 from functools import partial
 import io
+import os
 import subprocess
 import tarfile
 import tempfile
 import unittest.mock
 
 import attr
 import dulwich.repo
@@ -399,14 +400,23 @@
     bundle = backend.fetch("git_bare", cooked_swhid)
 
     # Extract bundle and make sure both revisions are in it
     with tempfile.TemporaryDirectory("swh-vault-test-bare") as tempdir:
         with tarfile.open(fileobj=io.BytesIO(bundle)) as tf:
             tf.extractall(tempdir)
 
+        if root_object != RootObjects.WEIRD_RELEASE:
+            # check master ref exists in repository
+            master_ref_path = os.path.join(
+                tempdir, f"{cooked_swhid}.git/refs/heads/master"
+            )
+            assert os.path.exists(master_ref_path)
+            with open(master_ref_path, "r") as master_ref:
+                assert master_ref.read() == branches[b"refs/heads/master"].target.hex()
+
         if root_object in (RootObjects.SNAPSHOT, RootObjects.REVISION):
             log_head = "master"
         elif root_object == RootObjects.RELEASE:
             log_head = "1.0.0"
         elif root_object == RootObjects.WEIRD_RELEASE:
             log_head = "release"
         else:
```

### Comparing `swh.vault-1.9.2/swh/vault/tests/test_init.py` & `swh.vault-1.9.3/swh/vault/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/tests/test_init_cookers.py` & `swh.vault-1.9.3/swh/vault/tests/test_init_cookers.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/tests/test_server.py` & `swh.vault-1.9.3/swh/vault/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/tests/test_to_disk.py` & `swh.vault-1.9.3/swh/vault/tests/test_to_disk.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/tests/vault_testing.py` & `swh.vault-1.9.3/swh/vault/tests/vault_testing.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh/vault/to_disk.py` & `swh.vault-1.9.3/swh/vault/to_disk.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/swh.vault.egg-info/PKG-INFO` & `swh.vault-1.9.3/swh.vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.vault
-Version: 1.9.2
+Version: 1.9.3
 Summary: Software Heritage vault
 Home-page: https://forge.softwareheritage.org/diffusion/DVAU/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-vault
```

### Comparing `swh.vault-1.9.2/swh.vault.egg-info/SOURCES.txt` & `swh.vault-1.9.3/swh.vault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.vault-1.9.2/tox.ini` & `swh.vault-1.9.3/tox.ini`

 * *Files identical despite different names*

