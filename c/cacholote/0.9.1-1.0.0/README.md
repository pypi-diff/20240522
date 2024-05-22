# Comparing `tmp/cacholote-0.9.1.tar.gz` & `tmp/cacholote-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacholote-0.9.1.tar", last modified: Fri Mar 22 15:36:51 2024, max compression
+gzip compressed data, was "cacholote-1.0.0.tar", last modified: Wed May 22 11:35:24 2024, max compression
```

## Comparing `cacholote-0.9.1.tar` & `cacholote-1.0.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.158450 cacholote-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-22 15:36:40.000000 cacholote-0.9.1/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.150450 cacholote-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.150450 cacholote-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-03-22 15:36:40.000000 cacholote-0.9.1/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-03-22 15:36:40.000000 cacholote-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-22 15:36:40.000000 cacholote-0.9.1/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-22 15:36:40.000000 cacholote-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-22 15:36:40.000000 cacholote-0.9.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-03-22 15:36:40.000000 cacholote-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-22 15:36:40.000000 cacholote-0.9.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    17003 2024-03-22 15:36:51.158450 cacholote-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-22 15:36:40.000000 cacholote-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.154450 cacholote-0.9.1/cacholote/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/encode.py
--rw-r--r--   0 runner    (1001) docker     (127)    14391 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/extra_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-03-22 15:36:40.000000 cacholote-0.9.1/cacholote/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-22 15:36:51.000000 cacholote-0.9.1/cacholote/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.158450 cacholote-0.9.1/cacholote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17003 2024-03-22 15:36:51.000000 cacholote-0.9.1/cacholote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-22 15:36:51.000000 cacholote-0.9.1/cacholote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 15:36:51.000000 cacholote-0.9.1/cacholote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 15:36:51.000000 cacholote-0.9.1/cacholote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-22 15:36:51.000000 cacholote-0.9.1/cacholote.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.154450 cacholote-0.9.1/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-22 15:36:40.000000 cacholote-0.9.1/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-22 15:36:40.000000 cacholote-0.9.1/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.154450 cacholote-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/DESIGN.rst
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/OBJECT-STORAGE-DESIGN.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.154450 cacholote-0.9.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.154450 cacholote-0.9.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-22 15:36:40.000000 cacholote-0.9.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-22 15:36:40.000000 cacholote-0.9.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-22 15:36:40.000000 cacholote-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 15:36:51.158450 cacholote-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:36:51.158450 cacholote-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_01_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_02_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_10_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_20_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_30_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_40_xarray_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_50_io_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-03-22 15:36:40.000000 cacholote-0.9.1/tests/test_60_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.951754 cacholote-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-22 11:35:15.000000 cacholote-1.0.0/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.939754 cacholote-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.943754 cacholote-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-22 11:35:15.000000 cacholote-1.0.0/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-05-22 11:35:15.000000 cacholote-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-22 11:35:15.000000 cacholote-1.0.0/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-22 11:35:15.000000 cacholote-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-22 11:35:15.000000 cacholote-1.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-22 11:35:15.000000 cacholote-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-22 11:35:15.000000 cacholote-1.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-22 11:35:24.951754 cacholote-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-22 11:35:15.000000 cacholote-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.943754 cacholote-1.0.0/cacholote/
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12756 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13947 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/extra_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-22 11:35:15.000000 cacholote-1.0.0/cacholote/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 11:35:24.000000 cacholote-1.0.0/cacholote/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.951754 cacholote-1.0.0/cacholote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-22 11:35:24.000000 cacholote-1.0.0/cacholote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-22 11:35:24.000000 cacholote-1.0.0/cacholote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:35:24.000000 cacholote-1.0.0/cacholote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-22 11:35:24.000000 cacholote-1.0.0/cacholote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:35:24.000000 cacholote-1.0.0/cacholote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.947754 cacholote-1.0.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-22 11:35:15.000000 cacholote-1.0.0/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-22 11:35:15.000000 cacholote-1.0.0/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.947754 cacholote-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/DESIGN.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/OBJECT-STORAGE-DESIGN.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.947754 cacholote-1.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.947754 cacholote-1.0.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 11:35:15.000000 cacholote-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 11:35:15.000000 cacholote-1.0.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-22 11:35:15.000000 cacholote-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:35:24.951754 cacholote-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:24.951754 cacholote-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_01_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_02_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_10_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_20_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_30_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_40_xarray_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_50_io_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-22 11:35:15.000000 cacholote-1.0.0/tests/test_60_clean.py
```

### Comparing `cacholote-0.9.1/.cruft.json` & `cacholote-1.0.0/.cruft.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'22f52dd88a2ec84dfa380d8e2c655e0b3752a10a'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "327e5d7bd991fe1b4a2e6ae1f398a8babb84ca7d",
+    "commit": "22f52dd88a2ec84dfa380d8e2c655e0b3752a10a",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/ecmwf-projects/cookiecutter-conda-package",
             "copyright_holder": "B-Open Solutions srl",
             "copyright_year": "2019",
             "integration_tests": "True",
             "mypy_strict": "True",
```

### Comparing `cacholote-0.9.1/.github/workflows/on-push.yml` & `cacholote-1.0.0/.github/workflows/on-push.yml`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/.gitignore` & `cacholote-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/.pre-commit-config.yaml` & `cacholote-1.0.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-json
   - id: check-yaml
   - id: check-toml
   - id: check-added-large-files
@@ -13,25 +13,25 @@
   - id: mixed-line-ending
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.9
   hooks:
   - id: blackdoc
     additional_dependencies: [black==23.11.0]
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.3.3
+  rev: v0.4.4
   hooks:
   - id: ruff
     args: [--fix, --show-fixes]
   - id: ruff-format
 - repo: https://github.com/executablebooks/mdformat
   rev: 0.7.17
   hooks:
   - id: mdformat
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.12.0
+  rev: v2.13.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --preserve-quotes]
   - id: pretty-format-toml
     args: [--autofix]
 - repo: https://github.com/gitleaks/gitleaks
   rev: v8.18.2
```

### Comparing `cacholote-0.9.1/LICENSE` & `cacholote-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/Makefile` & `cacholote-1.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/PKG-INFO` & `cacholote-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.9.1
+Version: 1.0.0
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -206,18 +206,18 @@
         
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fsspec
 Requires-Dist: pydantic
 Requires-Dist: pydantic-settings
 Requires-Dist: sqlalchemy>=2.0.9
```

### Comparing `cacholote-0.9.1/README.md` & `cacholote-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/cacholote/__init__.py` & `cacholote-1.0.0/cacholote/__init__.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/cacholote/cache.py` & `cacholote-1.0.0/cacholote/cache.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/cacholote/clean.py` & `cacholote-1.0.0/cacholote/clean.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,63 +102,63 @@
         for path, size in self.fs.du(self.dirname, total=False).items():
             # Group dirs
             urlpath = self.fs.unstrip_protocol(path)
             basename, *_ = urlpath.replace(urldir, "", 1).strip("/").split("/")
             if basename:
                 self.file_sizes[posixpath.join(urldir, basename)] += size
 
+        self.disk_usage = sum(self.file_sizes.values())
         self.log_disk_usage()
 
-    @property
-    def disk_usage(self) -> int:
-        return sum(self.file_sizes.values())
+    def pop_file_size(self, file: str) -> int:
+        size = self.file_sizes.pop(file, 0)
+        self.disk_usage -= size
+        return size
 
     def log_disk_usage(self) -> None:
-        self.logger.info("disk usage check", disk_usage=self.disk_usage)
+        self.logger.info("check disk usage", disk_usage=self.disk_usage)
 
     def stop_cleaning(self, maxsize: int) -> bool:
         return self.disk_usage <= maxsize
 
-    def get_unknown_sizes(self, lock_validity_period: float | None) -> dict[str, int]:
+    def get_unknown_files(self, lock_validity_period: float | None) -> set[str]:
         self.logger.info("getting unknown files")
 
         utcnow = utils.utcnow()
-        files_to_skip = []
+        locked_files = set()
         for urlpath in self.file_sizes:
             if urlpath.endswith(".lock"):
                 modified = self.fs.modified(urlpath)
                 if modified.tzinfo is None:
                     modified = modified.replace(tzinfo=datetime.timezone.utc)
                 delta = utcnow - modified
                 if lock_validity_period is None or delta < datetime.timedelta(
                     seconds=lock_validity_period
                 ):
-                    files_to_skip.append(urlpath)
-                    files_to_skip.append(urlpath.rsplit(".lock", 1)[0])
+                    locked_files.add(urlpath)
+                    locked_files.add(urlpath.rsplit(".lock", 1)[0])
 
-        unknown_sizes = {
-            k: v for k, v in self.file_sizes.items() if k not in files_to_skip
-        }
-        if unknown_sizes:
+        if unknown_files := (set(self.file_sizes) - locked_files):
             with config.get().instantiated_sessionmaker() as session:
                 for cache_entry in session.scalars(sa.select(database.CacheEntry)):
-                    for file in _get_files_from_cache_entry(cache_entry):
-                        unknown_sizes.pop(file, 0)
-        return unknown_sizes
+                    for known_file in _get_files_from_cache_entry(cache_entry):
+                        unknown_files.discard(known_file)
+                    if not unknown_files:
+                        break
+        return unknown_files
 
     def delete_unknown_files(
         self, lock_validity_period: float | None, recursive: bool
     ) -> None:
-        unknown_sizes = self.get_unknown_sizes(lock_validity_period)
-        for urlpath in unknown_sizes:
-            self.file_sizes.pop(urlpath, 0)
+        unknown_files = self.get_unknown_files(lock_validity_period)
+        for urlpath in unknown_files:
+            self.pop_file_size(urlpath)
         self.remove_files(
-            list(unknown_sizes),
+            list(unknown_files),
             recursive=recursive,
-            msg="deleting unknown files",
         )
         self.log_disk_usage()
 
     @staticmethod
     @pydantic.validate_call
     def _get_tag_filters(
         tags_to_clean: Optional[list[Optional[str]]],
@@ -203,33 +203,30 @@
         sorters.append(database.CacheEntry.expiration)
         return sorters
 
     def remove_files(
         self,
         files: list[str],
         max_tries: int = 10,
-        msg: str = "deleting cache files",
         **kwargs: Any,
     ) -> None:
         assert max_tries >= 1
+        if not files:
+            return
 
-        if files:
-            self.logger.info(
-                msg,
-                number_of_files=len(files),
-                recursive=kwargs.get("recursive", False),
-            )
+        self.logger.info("deleting files", n_files_to_delete=len(files), **kwargs)
 
         n_tries = 0
         while files:
             n_tries += 1
             try:
                 self.fs.rm(files, **kwargs)
                 return
             except FileNotFoundError:
+                # Another concurrent process might have deleted files
                 if n_tries >= max_tries:
                     raise
                 files = [file for file in files if self.fs.exists(file)]
 
     def delete_cache_files(
         self,
         maxsize: int,
@@ -242,51 +239,50 @@
 
         if self.stop_cleaning(maxsize):
             return
 
         files_to_delete = []
         dirs_to_delete = []
         self.logger.info("getting cache entries to delete")
-        number_of_cache_entries = 0
+        n_entries_to_delete = 0
         with config.get().instantiated_sessionmaker() as session:
             for cache_entry in session.scalars(
                 sa.select(database.CacheEntry).filter(*filters).order_by(*sorters)
             ):
                 files = _get_files_from_cache_entry(cache_entry)
                 if files:
-                    number_of_cache_entries += 1
+                    n_entries_to_delete += 1
                     session.delete(cache_entry)
 
                 for file, file_type in files.items():
-                    self.file_sizes.pop(file, 0)
+                    self.pop_file_size(file)
                     if file_type == "application/vnd+zarr":
                         dirs_to_delete.append(file)
                     else:
                         files_to_delete.append(file)
 
                 if self.stop_cleaning(maxsize):
                     break
 
-            if number_of_cache_entries:
+            if n_entries_to_delete:
                 self.logger.info(
-                    "deleting cache entries",
-                    number_of_cache_entries=number_of_cache_entries,
+                    "deleting cache entries", n_entries_to_delete=n_entries_to_delete
                 )
             database._commit_or_rollback(session)
 
         self.remove_files(files_to_delete, recursive=False)
         self.remove_files(dirs_to_delete, recursive=True)
         self.log_disk_usage()
 
         if not self.stop_cleaning(maxsize):
             raise ValueError(
                 (
                     f"Unable to clean {self.dirname!r}."
                     f" Final disk usage: {self.disk_usage!r}."
-                    f" Expected disk usage: {maxsize!r}"
+                    f" Target disk usage: {maxsize!r}"
                 )
             )
 
 
 def clean_cache_files(
     maxsize: int,
     method: Literal["LRU", "LFU"] = "LRU",
```

### Comparing `cacholote-0.9.1/cacholote/config.py` & `cacholote-1.0.0/cacholote/config.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/cacholote/database.py` & `cacholote-1.0.0/cacholote/database.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/cacholote/decode.py` & `cacholote-1.0.0/cacholote/decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/cacholote/encode.py` & `cacholote-1.0.0/cacholote/encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/cacholote/extra_encoders.py` & `cacholote-1.0.0/cacholote/extra_encoders.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,17 +81,16 @@
 
 
 def _guess_type(
     fs: fsspec.AbstractFileSystem,
     local_path: str,
     default: str = "application/octet-stream",
 ) -> str:
-    content_type: str = fs.info(local_path).get("ContentType", "")
-    if content_type:
-        return content_type
+    if content_type := fs.info(local_path).get("ContentType", ""):
+        return str(content_type)
 
     filetype, *_ = mimetypes.guess_type(local_path, strict=False)
     if filetype is None and _HAS_MAGIC:
         with fs.open(local_path, "rb") as f:
             filetype = magic.from_buffer(f.read(), mime=True)
     return filetype or default
 
@@ -128,37 +127,38 @@
     href: str
     file_checksum: str = pydantic.Field(..., alias="file:checksum")
     file_size: int = pydantic.Field(..., alias="file:size")
     file_local_path: str = pydantic.Field(..., alias="file:local_path")
 
 
 def _dictify_file(fs: fsspec.AbstractFileSystem, local_path: str) -> dict[str, Any]:
+    settings = config.get()
     href = posixpath.join(
-        config.get().cache_files_urlpath_readonly or config.get().cache_files_urlpath,
+        settings.cache_files_urlpath_readonly or settings.cache_files_urlpath,
         posixpath.basename(local_path),
     )
     file_dict = {
         "type": _guess_type(fs, local_path),
         "href": href,
         "file:checksum": f"{fs.checksum(local_path):x}",
         "file:size": fs.size(local_path),
         "file:local_path": local_path,
     }
-
     return FileInfoModel(**file_dict).model_dump(by_alias=True)
 
 
 def _get_fs_and_urlpath(
     file_json: dict[str, Any],
     storage_options: dict[str, Any] | None = None,
     validate: bool = False,
 ) -> tuple[fsspec.AbstractFileSystem, str]:
+    settings = config.get()
     urlpath = file_json["file:local_path"]
     if storage_options is None:
-        storage_options = config.get().cache_files_storage_options
+        storage_options = settings.cache_files_storage_options
 
     if not validate:
         fs, *_ = fsspec.get_fs_token_paths(urlpath, storage_options=storage_options)
         return (fs, urlpath)
 
     # Attempt to read from local_path
     try:
@@ -171,15 +171,15 @@
             actual = (
                 fs.checksum(urlpath)  # Just for backward compatibility.
                 if isinstance(expected, int)
                 else f"{fs.checksum(urlpath):x}"
             )
             if expected != actual:
                 raise ValueError(f"checksum mismatch: {urlpath=} {expected=} {actual=}")
-            config.get().logger.info(
+            settings.logger.info(
                 "retrieve cache file", urlpath=fs.unstrip_protocol(urlpath)
             )
             return (fs, urlpath)
 
     # Attempt to read from href
     urlpath = file_json["href"]
     fs, *_ = fsspec.get_fs_token_paths(urlpath)
@@ -258,169 +258,171 @@
     fs, urlpath = _get_fs_and_urlpath(
         file_json, storage_options=storage_options, validate=True
     )
     return fs.open(urlpath, **kwargs)
 
 
 @_requires_xarray_and_dask
-def _maybe_store_xr_object(
+def _store_xr_object(
     obj: xr.Dataset | xr.DataArray,
     fs: fsspec.AbstractFileSystem,
     urlpath: str,
     filetype: str,
 ) -> None:
     if filetype == "application/vnd+zarr":
-        with utils.FileLock(
-            fs, urlpath, timeout=config.get().lock_timeout
-        ) as file_exists:
-            if not file_exists:
-                # Write directly on any filesystem
-                mapper = fs.get_mapper(urlpath)
-                with _logging_timer("upload", urlpath=fs.unstrip_protocol(urlpath)):
-                    obj.to_zarr(mapper, consolidated=True)
-    elif not fs.exists(urlpath):
-        # Need a tmp local copy to write on a different filesystem
-        with tempfile.TemporaryDirectory() as tmpdirname:
-            tmpfilename = str(pathlib.Path(tmpdirname) / pathlib.Path(urlpath).name)
-
-            with _logging_timer("write tmp file", urlpath=tmpfilename):
-                if filetype == "application/netcdf":
-                    obj.to_netcdf(tmpfilename)
-                elif filetype == "application/x-grib":
-                    import cfgrib.xarray_to_grib
-
-                    cfgrib.xarray_to_grib.to_grib(obj, tmpfilename)
-                else:
-                    # Should never get here! xarray_cache_type is checked in config.py
-                    raise ValueError(f"type {filetype!r} is NOT supported.")
-
-            _maybe_store_file_object(
-                fs if _filesystem_is_local(fs) else fsspec.filesystem("file"),
-                tmpfilename,
-                fs,
-                urlpath,
-                io_delete_original=True,
-            )
+        # Write directly on any filesystem
+        mapper = fs.get_mapper(urlpath)
+        with _logging_timer("upload", urlpath=fs.unstrip_protocol(urlpath)):
+            obj.to_zarr(mapper, consolidated=True)
+        return
+
+    # Need a tmp local copy to write on a different filesystem
+    with tempfile.TemporaryDirectory() as tmpdirname:
+        tmpfilename = str(pathlib.Path(tmpdirname) / pathlib.Path(urlpath).name)
+
+        with _logging_timer("write tmp file", urlpath=tmpfilename):
+            if filetype == "application/netcdf":
+                obj.to_netcdf(tmpfilename)
+            elif filetype == "application/x-grib":
+                import cfgrib.xarray_to_grib
+
+                cfgrib.xarray_to_grib.to_grib(obj, tmpfilename)
+            else:
+                # Should never get here! xarray_cache_type is checked in config.py
+                raise ValueError(f"type {filetype!r} is NOT supported.")
+
+        _store_file_object(
+            fs if _filesystem_is_local(fs) else fsspec.filesystem("file"),
+            tmpfilename,
+            fs,
+            urlpath,
+            io_delete_original=True,
+        )
 
 
 @_requires_xarray_and_dask
 def dictify_xr_object(obj: xr.Dataset | xr.DataArray) -> dict[str, Any]:
     """Encode a ``xr.Dataset`` to JSON deserialized data (``dict``)."""
+    settings = config.get()
     with dask.config.set({"tokenize.ensure-deterministic": True}):
         root = dask.base.tokenize(obj)
 
-    filetype = config.get().xarray_cache_type
-    ext = mimetypes.guess_extension(filetype, strict=False)
-    urlpath_out = posixpath.join(config.get().cache_files_urlpath, f"{root}{ext}")
+    ext = mimetypes.guess_extension(settings.xarray_cache_type, strict=False)
+    urlpath_out = posixpath.join(settings.cache_files_urlpath, f"{root}{ext}")
 
     fs_out, *_ = fsspec.get_fs_token_paths(
         urlpath_out,
-        storage_options=config.get().cache_files_storage_options,
+        storage_options=settings.cache_files_storage_options,
     )
-    _maybe_store_xr_object(obj, fs_out, urlpath_out, filetype)
+    with utils.FileLock(
+        fs_out, urlpath_out, timeout=settings.lock_timeout
+    ) as file_exists:
+        if not file_exists:
+            _store_xr_object(obj, fs_out, urlpath_out, settings.xarray_cache_type)
 
-    file_json = _dictify_file(fs_out, urlpath_out)
-    kwargs: dict[str, Any] = {"chunks": {}}
-    if filetype == "application/vnd+zarr":
-        kwargs.update({"engine": "zarr", "consolidated": True})
+        file_json = _dictify_file(fs_out, urlpath_out)
 
-    return encode.dictify_python_call(
-        decode_xr_dataset if isinstance(obj, xr.Dataset) else decode_xr_dataarray,
-        file_json,
-        storage_options=config.get().cache_files_storage_options,
-        **kwargs,
-    )
+        kwargs: dict[str, Any] = {"chunks": {}}
+        if settings.xarray_cache_type == "application/vnd+zarr":
+            kwargs.update({"engine": "zarr", "consolidated": True})
+
+        return encode.dictify_python_call(
+            decode_xr_dataset if isinstance(obj, xr.Dataset) else decode_xr_dataarray,
+            file_json,
+            storage_options=settings.cache_files_storage_options,
+            **kwargs,
+        )
 
 
-def _maybe_store_file_object(
+def _store_file_object(
     fs_in: fsspec.AbstractFileSystem,
     urlpath_in: str,
     fs_out: fsspec.AbstractFileSystem,
     urlpath_out: str,
     io_delete_original: bool | None = None,
 ) -> None:
     if io_delete_original is None:
         io_delete_original = config.get().io_delete_original
-    with utils.FileLock(
-        fs_out, urlpath_out, timeout=config.get().lock_timeout
-    ) as file_exists:
-        if not file_exists:
-            kwargs = {}
-            content_type = _guess_type(fs_in, urlpath_in)
-            if content_type:
-                kwargs["ContentType"] = content_type
-            with _logging_timer(
-                "upload",
-                urlpath=fs_out.unstrip_protocol(urlpath_out),
-                size=fs_in.size(urlpath_in),
-            ):
-                if fs_in == fs_out:
-                    if io_delete_original:
-                        fs_in.mv(urlpath_in, urlpath_out, **kwargs)
-                    else:
-                        fs_in.cp(urlpath_in, urlpath_out, **kwargs)
-                elif _filesystem_is_local(fs_in):
-                    fs_out.put(urlpath_in, urlpath_out, **kwargs)
-                else:
-                    with fs_in.open(urlpath_in, "rb") as f_in:
-                        with fs_out.open(urlpath_out, "wb") as f_out:
-                            utils.copy_buffered_file(f_in, f_out)
+
+    kwargs = {}
+    if content_type := _guess_type(fs_in, urlpath_in):
+        kwargs["ContentType"] = content_type
+    with _logging_timer(
+        "upload",
+        urlpath=fs_out.unstrip_protocol(urlpath_out),
+        size=fs_in.size(urlpath_in),
+    ):
+        if fs_in == fs_out:
+            func = fs_in.mv if io_delete_original else fs_in.cp
+            func(urlpath_in, urlpath_out, **kwargs)
+        elif _filesystem_is_local(fs_in):
+            fs_out.put(urlpath_in, urlpath_out, **kwargs)
+        else:
+            with fs_in.open(urlpath_in, "rb") as f_in:
+                with fs_out.open(urlpath_out, "wb") as f_out:
+                    utils.copy_buffered_file(f_in, f_out)
+
     if io_delete_original and fs_in.exists(urlpath_in):
         with _logging_timer(
             "remove",
             urlpath=fs_in.unstrip_protocol(urlpath_in),
             size=fs_in.size(urlpath_in),
         ):
             fs_in.rm(urlpath_in)
 
 
-def _maybe_store_io_object(
+def _store_io_object(
     f_in: _UNION_IO_TYPES,
     fs_out: fsspec.AbstractFileSystem,
     urlpath_out: str,
 ) -> None:
-    with utils.FileLock(
-        fs_out, urlpath_out, timeout=config.get().lock_timeout
-    ) as file_exists:
-        if not file_exists:
-            f_out = fs_out.open(urlpath_out, "wb")
-            with _logging_timer("upload", urlpath=fs_out.unstrip_protocol(urlpath_out)):
-                utils.copy_buffered_file(f_in, f_out)
+    f_out = fs_out.open(urlpath_out, "wb")
+    with _logging_timer("upload", urlpath=fs_out.unstrip_protocol(urlpath_out)):
+        utils.copy_buffered_file(f_in, f_out)
 
 
 def dictify_io_object(obj: _UNION_IO_TYPES) -> dict[str, Any]:
     """Encode a file object to JSON deserialized data (``dict``)."""
-    cache_files_urlpath = config.get().cache_files_urlpath
+    settings = config.get()
+
+    cache_files_urlpath = settings.cache_files_urlpath
     fs_out, *_ = fsspec.get_fs_token_paths(
         cache_files_urlpath,
-        storage_options=config.get().cache_files_storage_options,
+        storage_options=settings.cache_files_storage_options,
     )
 
-    if hasattr(obj, "path") or hasattr(obj, "name"):
-        urlpath_in = obj.path if hasattr(obj, "path") else obj.name  # type: ignore[union-attr]
+    if urlpath_in := getattr(obj, "path", getattr(obj, "name", "")):
         fs_in = getattr(obj, "fs", fsspec.filesystem("file"))
         root = f"{fs_in.checksum(urlpath_in):x}"
         ext = pathlib.Path(urlpath_in).suffix
         urlpath_out = posixpath.join(cache_files_urlpath, f"{root}{ext}")
-        _maybe_store_file_object(fs_in, urlpath_in, fs_out, urlpath_out)
     else:
         root = hashlib.md5(f"{hash(obj)}".encode()).hexdigest()  # fsspec uses md5
         urlpath_out = posixpath.join(cache_files_urlpath, root)
-        _maybe_store_io_object(obj, fs_out, urlpath_out)
 
-    file_json = _dictify_file(fs_out, urlpath_out)
-    params = inspect.signature(open).parameters
-    kwargs = {k: getattr(obj, k) for k in params.keys() if hasattr(obj, k)}
-
-    return encode.dictify_python_call(
-        decode_io_object,
-        file_json,
-        storage_options=config.get().cache_files_storage_options,
-        **kwargs,
-    )
+    with utils.FileLock(
+        fs_out, urlpath_out, timeout=settings.lock_timeout
+    ) as file_exists:
+        if not file_exists:
+            if urlpath_in:
+                _store_file_object(fs_in, urlpath_in, fs_out, urlpath_out)
+            else:
+                _store_io_object(obj, fs_out, urlpath_out)
+
+        file_json = _dictify_file(fs_out, urlpath_out)
+
+        params = inspect.signature(open).parameters
+        kwargs = {k: getattr(obj, k) for k in params.keys() if hasattr(obj, k)}
+
+        return encode.dictify_python_call(
+            decode_io_object,
+            file_json,
+            storage_options=settings.cache_files_storage_options,
+            **kwargs,
+        )
 
 
 def register_all() -> None:
     """Register extra encoders if optional dependencies are installed."""
     for type_ in (
         io.RawIOBase,
         io.BufferedIOBase,
```

### Comparing `cacholote-0.9.1/cacholote/utils.py` & `cacholote-1.0.0/cacholote/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,21 +80,29 @@
     @functools.cached_property
     def lockfile(self) -> str:
         return self.urlpath + ".lock"
 
     def acquire(self) -> None:
         self.fs.touch(self.lockfile)
 
+    @property
+    def exists(self) -> bool:
+        return bool(self.fs.exists(self.urlpath))
+
+    @property
+    def lock_exists(self) -> bool:
+        return bool(self.fs.exists(self.lockfile))
+
     def release(self) -> None:
         if self.fs.exists(self.lockfile):
             self.fs.rm(self.lockfile)
 
     @property
     def is_locked(self) -> bool:
-        return bool(self.fs.exists(self.lockfile))
+        return self.lock_exists and self.exists
 
     def wait_until_released(self) -> None:
         warned = False
         message = f"{self.urlpath!r} is locked: {self.lockfile!r}"
         start = time.perf_counter()
         while self.is_locked:
             if self.timeout is not None and time.perf_counter() - start > self.timeout:
@@ -103,15 +111,15 @@
                 warnings.warn(message, UserWarning)
                 warned = True
             time.sleep(min(1, self.timeout or 1))
 
     def __enter__(self) -> bool:
         self.wait_until_released()
         self.acquire()
-        return bool(self.fs.exists(self.urlpath))
+        return self.exists
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
```

### Comparing `cacholote-0.9.1/cacholote.egg-info/PKG-INFO` & `cacholote-1.0.0/cacholote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.9.1
+Version: 1.0.0
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -206,18 +206,18 @@
         
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fsspec
 Requires-Dist: pydantic
 Requires-Dist: pydantic-settings
 Requires-Dist: sqlalchemy>=2.0.9
```

### Comparing `cacholote-0.9.1/cacholote.egg-info/SOURCES.txt` & `cacholote-1.0.0/cacholote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/ci/environment-ci.yml` & `cacholote-1.0.0/ci/environment-ci.yml`

 * *Files 17% similar despite different names*

```diff
@@ -27,7 +27,9 @@
 - python-magic
 - requests
 - s3fs
 - sqlalchemy[mypy]
 - types-requests
 - xarray>=2022.6.0
 - zarr
+- pip:
+  - pytest-structlog
```

### Comparing `cacholote-0.9.1/docs/DESIGN.rst` & `cacholote-1.0.0/docs/DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/docs/Makefile` & `cacholote-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/docs/OBJECT-STORAGE-DESIGN.rst` & `cacholote-1.0.0/docs/OBJECT-STORAGE-DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/docs/conf.py` & `cacholote-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/docs/make.bat` & `cacholote-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/pyproject.toml` & `cacholote-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
-requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
+build-backend = "setuptools.build_meta"
+requires = ["setuptools>=64", "setuptools_scm>=8"]
 
 [project]
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering"
 ]
 dependencies = [
   "fsspec",
   "pydantic",
   "pydantic-settings",
   "sqlalchemy>=2.0.9",
```

### Comparing `cacholote-0.9.1/tests/conftest.py` & `cacholote-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/tests/test_01_settings.py` & `cacholote-1.0.0/tests/test_01_settings.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/tests/test_02_utils.py` & `cacholote-1.0.0/tests/test_02_utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/tests/test_10_decode.py` & `cacholote-1.0.0/tests/test_10_decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/tests/test_20_encode.py` & `cacholote-1.0.0/tests/test_20_encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/tests/test_30_cache.py` & `cacholote-1.0.0/tests/test_30_cache.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.9.1/tests/test_40_xarray_encoder.py` & `cacholote-1.0.0/tests/test_40_xarray_encoder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import pathlib
 from typing import TYPE_CHECKING
 
 import fsspec
 import pytest
+import pytest_structlog
 import structlog
 
 from cacholote import cache, config, decode, encode, extra_encoders, utils
 
 if TYPE_CHECKING:
     import xarray as xr
 else:
@@ -159,45 +160,56 @@
     fs.rm(cached_path, recursive=True)
     with pytest.warns(UserWarning, match="No such file or directory"):
         actual = cfunc()
     xr.testing.assert_identical(actual, expected)
     assert fs.exists(cached_path)
 
 
-def test_xr_logging(capsys: pytest.CaptureFixture[str]) -> None:
+def test_xr_logging(log: pytest_structlog.StructuredLogCapture) -> None:
     config.set(logger=structlog.get_logger(), raise_all_encoding_errors=True)
 
     # Cache dataset
     cfunc = cache.cacheable(get_grib_ds)
     cached_ds = cfunc()
-    captured = iter(capsys.readouterr().out.splitlines())
-
-    line = next(captured)
-    assert "start write tmp file" in line
-    assert "urlpath=" in line
-
-    line = next(captured)
-    assert "end write tmp file" in line
-    assert "urlpath=" in line
-    assert "write_tmp_file_time=" in line
-
-    line = next(captured)
-    assert "start upload" in line
-    assert f"urlpath=file://{cached_ds.encoding['source']}" in line
-    assert "size=22597" in line
-
-    line = next(captured)
-    assert "end upload" in line
-    assert f"urlpath=file://{cached_ds.encoding['source']}" in line
-    assert "upload_time=" in line
-    assert "size=22597" in line
-
-    line = next(captured)
-    assert "retrieve cache file" in line
-    assert f"urlpath=file://{cached_ds.encoding['source']}" in line
+    urlpath = f"file://{cached_ds.encoding['source']}"
+    tmpfile = log.events[0]["urlpath"]
+    assert urlpath.rsplit("/", 1)[1] == tmpfile.rsplit("/", 1)[1]
+
+    expected = [
+        {
+            "urlpath": tmpfile,
+            "event": "start write tmp file",
+            "level": "info",
+        },
+        {
+            "urlpath": tmpfile,
+            "write_tmp_file_time": log.events[1]["write_tmp_file_time"],
+            "event": "end write tmp file",
+            "level": "info",
+        },
+        {
+            "urlpath": urlpath,
+            "size": 22597,
+            "event": "start upload",
+            "level": "info",
+        },
+        {
+            "urlpath": urlpath,
+            "size": 22597,
+            "upload_time": log.events[3]["upload_time"],
+            "event": "end upload",
+            "level": "info",
+        },
+        {
+            "urlpath": urlpath,
+            "event": "retrieve cache file",
+            "level": "info",
+        },
+    ]
+    assert log.events == expected
 
 
 @pytest.mark.parametrize(
     "original_obj",
     (
         xr.DataArray([0], name="foo"),
         xr.DataArray([0], name="foo").to_dataset(),
```

### Comparing `cacholote-0.9.1/tests/test_50_io_encoder.py` & `cacholote-1.0.0/tests/test_50_io_encoder.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pathlib
 import subprocess
 from typing import Any
 
 import fsspec
 import pytest
 import pytest_httpserver
+import pytest_structlog
 import structlog
 
 from cacholote import cache, config, decode, encode, extra_encoders, utils
 
 
 @cache.cacheable
 def cached_open(*args: Any, **kwargs: Any) -> fsspec.spec.AbstractBufferedFile:
@@ -165,14 +166,15 @@
     # Create tmpfile
     tmpfile = tmp_path / "test.txt"
     fsspec.filesystem("file").touch(tmpfile)
 
     # Acquire lock
     fs, dirname = utils.get_cache_files_fs_dirname()
     file_path = f"{dirname}/{fsspec.filesystem('file').checksum(tmpfile):x}.txt"
+    fs.touch(file_path)
     fs.touch(f"{file_path}.lock")
 
     process = subprocess.Popen(f"sleep 0.1; rm {file_path}.lock", shell=True)
     with raises_or_warns:
         cached_open(tmpfile)
     assert process.wait() == 0
 
@@ -183,41 +185,53 @@
     fsspec.filesystem("file").touch(tmpfile)
     fs, _ = utils.get_cache_files_fs_dirname()
     cached_grib = cached_open(tmpfile)
     assert fs.info(cached_grib)["ContentType"] == "application/x-grib"
 
 
 @pytest.mark.parametrize("set_cache", ["cads"], indirect=True)
-def test_io_logging(capsys: pytest.CaptureFixture[str], tmp_path: pathlib.Path) -> None:
+def test_io_logging(
+    log: pytest_structlog.StructuredLogCapture, tmp_path: pathlib.Path
+) -> None:
     config.set(logger=structlog.get_logger(), io_delete_original=True)
 
     # Cache file
     tmpfile = tmp_path / "test.txt"
     fsspec.filesystem("file").touch(tmpfile)
     cached_file = cached_open(tmpfile)
-    captured = iter(capsys.readouterr().out.splitlines())
 
-    line = next(captured)
-    assert "start upload" in line
-    assert f"urlpath=s3://{cached_file.path}" in line
-    assert "size=0" in line
-
-    line = next(captured)
-    assert "end upload" in line
-    assert f"urlpath=s3://{cached_file.path}" in line
-    assert "upload_time=" in line
-    assert "size=0" in line
-
-    line = next(captured)
-    assert "start remove" in line
-    assert f"urlpath=file://{tmpfile}" in line
-    assert "size=0" in line
-
-    line = next(captured)
-    assert "end remove" in line
-    assert f"urlpath=file://{tmpfile}" in line
-    assert "remove_time=" in line
-    assert "size=0" in line
-
-    line = next(captured)
-    assert "retrieve cache file" in line
-    assert f"urlpath=s3://{cached_file.path}" in line
+    tmp_urlpath = f"file://{tmpfile!s}"
+    cached_urlpath = f"s3://{cached_file.path}"
+    expected = [
+        {
+            "urlpath": cached_urlpath,
+            "size": 0,
+            "event": "start upload",
+            "level": "info",
+        },
+        {
+            "urlpath": cached_urlpath,
+            "size": 0,
+            "upload_time": log.events[1]["upload_time"],
+            "event": "end upload",
+            "level": "info",
+        },
+        {
+            "urlpath": tmp_urlpath,
+            "size": 0,
+            "event": "start remove",
+            "level": "info",
+        },
+        {
+            "urlpath": tmp_urlpath,
+            "size": 0,
+            "remove_time": log.events[3]["remove_time"],
+            "event": "end remove",
+            "level": "info",
+        },
+        {
+            "urlpath": cached_urlpath,
+            "event": "retrieve cache file",
+            "level": "info",
+        },
+    ]
+    assert log.events == expected
```

### Comparing `cacholote-0.9.1/tests/test_60_clean.py` & `cacholote-1.0.0/tests/test_60_clean.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pathlib
 import time
 from typing import Any, Literal
 
 import fsspec
 import pydantic
 import pytest
+import pytest_structlog
 import structlog
 
 from cacholote import cache, clean, config, utils
 
 ONE_BYTE = os.urandom(1)
 does_not_raise = contextlib.nullcontext
 
@@ -249,57 +250,48 @@
     con = config.get().engine.raw_connection()
     cur = con.cursor()
     cur.execute("SELECT COUNT(*) FROM cache_entries", ())
     assert cur.fetchone() == (3 - check_expiration - try_decode,)
 
 
 def test_cleaner_logging(
-    capsys: pytest.CaptureFixture[str], tmp_path: pathlib.Path
+    log: pytest_structlog.StructuredLogCapture, tmp_path: pathlib.Path
 ) -> None:
     # Cache file and create unknown
     tmpfile = tmp_path / "test.txt"
     fsspec.filesystem("file").pipe_file(tmpfile, ONE_BYTE)
     open_url(tmpfile)
     fs, dirname = utils.get_cache_files_fs_dirname()
     fs.pipe_file(f"{dirname}/unknown.txt", ONE_BYTE)
 
     # Clean
     config.set(logger=structlog.get_logger())
     clean.clean_cache_files(0, delete_unknown_files=True)
-    captured = iter(capsys.readouterr().out.splitlines())
 
-    sep = " " * 15
-    line = next(captured)
-    assert "getting disk usage" in line
-
-    line = next(captured)
-    assert line.endswith(f"disk usage check{sep}disk_usage=2")
-
-    line = next(captured)
-    assert "getting unknown files" in line
-
-    line = next(captured)
-    line.endswith(f"deleting unknown files{sep}number_of_files=1{sep}recursive=False")
-
-    line = next(captured)
-    line.endswith(f"disk usage check{sep}disk_usage=1")
-
-    line = next(captured)
-    assert "getting cache entries to delete" in line
-
-    line = next(captured)
-    line.endswith(f"deleting cache entries{sep}number_of_cache_entries=1")
-
-    line = next(captured)
-    line.endswith(f"deleting cache files{sep}number_of_files=1{sep}recursive=False")
-
-    line = next(captured)
-    line.endswith(f"disk usage check{sep}disk_usage=0")
-
-    assert next(captured, None) is None
+    assert log.events == [
+        {"event": "getting disk usage", "level": "info"},
+        {"disk_usage": 2, "event": "check disk usage", "level": "info"},
+        {"event": "getting unknown files", "level": "info"},
+        {
+            "n_files_to_delete": 1,
+            "recursive": False,
+            "event": "deleting files",
+            "level": "info",
+        },
+        {"disk_usage": 1, "event": "check disk usage", "level": "info"},
+        {"event": "getting cache entries to delete", "level": "info"},
+        {"n_entries_to_delete": 1, "event": "deleting cache entries", "level": "info"},
+        {
+            "n_files_to_delete": 1,
+            "recursive": False,
+            "event": "deleting files",
+            "level": "info",
+        },
+        {"disk_usage": 0, "event": "check disk usage", "level": "info"},
+    ]
 
 
 def test_clean_multiple_files(tmp_path: pathlib.Path) -> None:
     fs, dirname = utils.get_cache_files_fs_dirname()
 
     fsspec.filesystem("file").pipe_file(tmp_path / "test1.txt", ONE_BYTE)
     fsspec.filesystem("file").pipe_file(tmp_path / "test2.txt", ONE_BYTE)
```

