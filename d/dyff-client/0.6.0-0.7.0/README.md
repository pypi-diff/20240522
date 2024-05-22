# Comparing `tmp/dyff_client-0.6.0.tar.gz` & `tmp/dyff_client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_client-0.6.0.tar", last modified: Fri May 17 04:25:40 2024, max compression
+gzip compressed data, was "dyff_client-0.7.0.tar", last modified: Wed May 22 20:49:48 2024, max compression
```

## Comparing `dyff_client-0.6.0.tar` & `dyff_client-0.7.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:25:40.255783 dyff_client-0.6.0/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-17 04:25:34.000000 dyff_client-0.6.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1778 2024-05-17 04:25:34.000000 dyff_client-0.6.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-05-17 04:25:34.000000 dyff_client-0.6.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-17 04:25:34.000000 dyff_client-0.6.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-17 04:25:34.000000 dyff_client-0.6.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-17 04:25:34.000000 dyff_client-0.6.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-17 04:25:34.000000 dyff_client-0.6.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-17 04:25:34.000000 dyff_client-0.6.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-17 04:25:34.000000 dyff_client-0.6.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4008 2024-05-17 04:25:40.255783 dyff_client-0.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2781 2024-05-17 04:25:34.000000 dyff_client-0.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:25:40.238783 dyff_client-0.6.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:25:40.243784 dyff_client-0.6.0/dyff/client/
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:25:40.245783 dyff_client-0.6.0/dyff/client/_generated/
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)    80932 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/_serialization.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:25:40.246784 dyff_client-0.6.0/dyff/client/_generated/aio/
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/aio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6649 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/aio/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/aio/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/aio/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/aio/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:25:40.248783 dyff_client-0.6.0/dyff/client/_generated/aio/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/aio/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   830715 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/aio/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/aio/operations/_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:25:40.251783 dyff_client-0.6.0/dyff/client/_generated/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   888637 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/operations/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/_generated/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    82979 2024-05-17 04:25:34.000000 dyff_client-0.6.0/dyff/client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:25:40.254783 dyff_client-0.6.0/dyff_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4008 2024-05-17 04:25:40.000000 dyff_client-0.6.0/dyff_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1464 2024-05-17 04:25:40.000000 dyff_client-0.6.0/dyff_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 04:25:40.000000 dyff_client-0.6.0/dyff_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2024-05-17 04:25:40.000000 dyff_client-0.6.0/dyff_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-17 04:25:40.000000 dyff_client-0.6.0/dyff_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-17 04:25:34.000000 dyff_client-0.6.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-17 04:25:34.000000 dyff_client-0.6.0/package-lock.json
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-05-17 04:25:34.000000 dyff_client-0.6.0/package.json
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-17 04:25:34.000000 dyff_client-0.6.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:25:40.240784 dyff_client-0.6.0/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:25:40.253784 dyff_client-0.6.0/scripts/inferenceservices/
--rw-rw-rw-   0 root         (0) root         (0)     2529 2024-05-17 04:25:34.000000 dyff_client-0.6.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
--rw-rw-rw-   0 root         (0) root         (0)     2537 2024-05-17 04:25:34.000000 dyff_client-0.6.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:25:40.254783 dyff_client-0.6.0/scripts/models/
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-17 04:25:34.000000 dyff_client-0.6.0/scripts/models/databricks--dolly-v2-3b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-17 04:25:34.000000 dyff_client-0.6.0/scripts/models/databricks--dolly-v2-3b.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-17 04:25:34.000000 dyff_client-0.6.0/scripts/models/tiiuae--falcon-7b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1356 2024-05-17 04:25:34.000000 dyff_client-0.6.0/scripts/models/tiiuae--falcon-7b.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 04:25:40.255783 dyff_client-0.6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:25:40.254783 dyff_client-0.6.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-17 04:25:34.000000 dyff_client-0.6.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.377713 dyff_client-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-22 20:49:41.000000 dyff_client-0.7.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2024-05-22 20:49:41.000000 dyff_client-0.7.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-05-22 20:49:41.000000 dyff_client-0.7.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-22 20:49:41.000000 dyff_client-0.7.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-22 20:49:41.000000 dyff_client-0.7.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-22 20:49:41.000000 dyff_client-0.7.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-22 20:49:41.000000 dyff_client-0.7.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-22 20:49:41.000000 dyff_client-0.7.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-22 20:49:41.000000 dyff_client-0.7.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-05-22 20:49:48.376713 dyff_client-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2024-05-22 20:49:41.000000 dyff_client-0.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.361713 dyff_client-0.7.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.366713 dyff_client-0.7.0/dyff/client/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.368713 dyff_client-0.7.0/dyff/client/_generated/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    80932 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/_serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.369713 dyff_client-0.7.0/dyff/client/_generated/aio/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6649 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.371713 dyff_client-0.7.0/dyff/client/_generated/aio/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   842746 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/operations/_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.373713 dyff_client-0.7.0/dyff/client/_generated/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   900914 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/operations/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    83364 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.376713 dyff_client-0.7.0/dyff_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-05-22 20:49:48.000000 dyff_client-0.7.0/dyff_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-05-22 20:49:48.000000 dyff_client-0.7.0/dyff_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 20:49:48.000000 dyff_client-0.7.0/dyff_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-05-22 20:49:48.000000 dyff_client-0.7.0/dyff_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-22 20:49:48.000000 dyff_client-0.7.0/dyff_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-22 20:49:41.000000 dyff_client-0.7.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-22 20:49:41.000000 dyff_client-0.7.0/package-lock.json
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-05-22 20:49:41.000000 dyff_client-0.7.0/package.json
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-22 20:49:41.000000 dyff_client-0.7.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.362713 dyff_client-0.7.0/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.374713 dyff_client-0.7.0/scripts/inferenceservices/
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2024-05-22 20:49:41.000000 dyff_client-0.7.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2024-05-22 20:49:41.000000 dyff_client-0.7.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.375713 dyff_client-0.7.0/scripts/models/
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-22 20:49:41.000000 dyff_client-0.7.0/scripts/models/databricks--dolly-v2-3b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-22 20:49:41.000000 dyff_client-0.7.0/scripts/models/databricks--dolly-v2-3b.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-22 20:49:41.000000 dyff_client-0.7.0/scripts/models/tiiuae--falcon-7b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2024-05-22 20:49:41.000000 dyff_client-0.7.0/scripts/models/tiiuae--falcon-7b.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 20:49:48.377713 dyff_client-0.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.375713 dyff_client-0.7.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-22 20:49:41.000000 dyff_client-0.7.0/tests/test_import.py
```

### Comparing `dyff_client-0.6.0/.gitlab-ci.yml` & `dyff_client-0.7.0/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     file:
       - detect-secrets.yml
   - project: buildgarden/pipelines/prettier
     ref: 0.3.2
     file:
       - prettier.yml
   - project: buildgarden/pipelines/python
-    ref: 0.10.0
+    ref: 0.12.0
     file:
       - python-autoflake.yml
       - python-black.yml
       - python-isort.yml
       - python-build-sdist.yml
       - python-build-wheel.yml
       - python-pyroma.yml
```

### Comparing `dyff_client-0.6.0/.licenserc.yaml` & `dyff_client-0.7.0/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/.pre-commit-config.yaml` & `dyff_client-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/.secrets.baseline` & `dyff_client-0.7.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/CODE_OF_CONDUCT.md` & `dyff_client-0.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/LICENSE` & `dyff_client-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/PKG-INFO` & `dyff_client-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_client-0.6.0/README.md` & `dyff_client-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/__init__.py` & `dyff_client-0.7.0/dyff/client/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/_client.py` & `dyff_client-0.7.0/dyff/client/_generated/_client.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/_configuration.py` & `dyff_client-0.7.0/dyff/client/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/_patch.py` & `dyff_client-0.7.0/dyff/client/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/_serialization.py` & `dyff_client-0.7.0/dyff/client/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/_vendor.py` & `dyff_client-0.7.0/dyff/client/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/aio/__init__.py` & `dyff_client-0.7.0/dyff/client/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/aio/_client.py` & `dyff_client-0.7.0/dyff/client/_generated/aio/_client.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/aio/_configuration.py` & `dyff_client-0.7.0/dyff/client/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/aio/_patch.py` & `dyff_client-0.7.0/dyff/client/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/aio/_vendor.py` & `dyff_client-0.7.0/dyff/client/_generated/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/aio/operations/__init__.py` & `dyff_client-0.7.0/dyff/client/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/aio/operations/_operations.py` & `dyff_client-0.7.0/dyff/client/_generated/aio/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -266,15 +268,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -1696,14 +1700,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -1804,25 +1810,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -1870,14 +1880,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -1917,25 +1929,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -2074,15 +2090,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -2163,15 +2181,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -2486,14 +2506,17 @@
                                   for detailed naming rules. Required.
                                 "value": "str"  # The annotation value. An arbitrary
                                   string. Required.
                             }
                         ],
                         "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation
                           time (assigned by system).
+                        "inferenceSessionReference": "str",  # Optional. ID of a running
+                          inference session that will be used for the evaluation instead of starting a
+                          new one.
                         "kind": "Evaluation",  # Optional. Default value is "Evaluation".
                           Kind. "Evaluation"
                         "labels": {
                             "str": "str"  # Optional. A set of key-value labels for the
                               resource. Used to specify identifying attributes of resources that are
                               meaningful to users but do not imply semantics in the dyff system.  The
                               keys are DNS labels with an optional DNS domain prefix. For example:
@@ -2636,14 +2659,17 @@
                           the session. Use of this field is recommended to avoid accidental compute
                           costs.
                         "replicas": 1,  # Optional. Default value is 1. Number of model
                           replicas.
                         "useSpotPods": True  # Optional. Default value is True. Use 'spot
                           pods' for cheaper computation.
                     },
+                    "inferenceSessionReference": "str",  # Optional. The ID of a running
+                      inference session that will be used for the evaluation, instead of starting a new
+                      one.
                     "replications": 1,  # Optional. Default value is 1. Number of replications to
                       run.
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                     "workersPerReplica": 0  # Optional. Number of data workers per inference
                       service replica.
                 }
@@ -2821,14 +2847,16 @@
                               for detailed naming rules. Required.
                             "value": "str"  # The annotation value. An arbitrary string.
                               Required.
                         }
                     ],
                     "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
                       (assigned by system).
+                    "inferenceSessionReference": "str",  # Optional. ID of a running inference
+                      session that will be used for the evaluation instead of starting a new one.
                     "kind": "Evaluation",  # Optional. Default value is "Evaluation". Kind.
                       "Evaluation"
                     "labels": {
                         "str": "str"  # Optional. A set of key-value labels for the resource.
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
@@ -3054,14 +3082,16 @@
                               for detailed naming rules. Required.
                             "value": "str"  # The annotation value. An arbitrary string.
                               Required.
                         }
                     ],
                     "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
                       (assigned by system).
+                    "inferenceSessionReference": "str",  # Optional. ID of a running inference
+                      session that will be used for the evaluation instead of starting a new one.
                     "kind": "Evaluation",  # Optional. Default value is "Evaluation". Kind.
                       "Evaluation"
                     "labels": {
                         "str": "str"  # Optional. A set of key-value labels for the resource.
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
@@ -3133,14 +3163,17 @@
                           the session. Use of this field is recommended to avoid accidental compute
                           costs.
                         "replicas": 1,  # Optional. Default value is 1. Number of model
                           replicas.
                         "useSpotPods": True  # Optional. Default value is True. Use 'spot
                           pods' for cheaper computation.
                     },
+                    "inferenceSessionReference": "str",  # Optional. The ID of a running
+                      inference session that will be used for the evaluation, instead of starting a new
+                      one.
                     "replications": 1,  # Optional. Default value is 1. Number of replications to
                       run.
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                     "workersPerReplica": 0  # Optional. Number of data workers per inference
                       service replica.
                 }
@@ -3318,14 +3351,16 @@
                               for detailed naming rules. Required.
                             "value": "str"  # The annotation value. An arbitrary string.
                               Required.
                         }
                     ],
                     "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
                       (assigned by system).
+                    "inferenceSessionReference": "str",  # Optional. ID of a running inference
+                      session that will be used for the evaluation instead of starting a new one.
                     "kind": "Evaluation",  # Optional. Default value is "Evaluation". Kind.
                       "Evaluation"
                     "labels": {
                         "str": "str"  # Optional. A set of key-value labels for the resource.
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
@@ -3614,14 +3649,16 @@
                               for detailed naming rules. Required.
                             "value": "str"  # The annotation value. An arbitrary string.
                               Required.
                         }
                     ],
                     "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
                       (assigned by system).
+                    "inferenceSessionReference": "str",  # Optional. ID of a running inference
+                      session that will be used for the evaluation instead of starting a new one.
                     "kind": "Evaluation",  # Optional. Default value is "Evaluation". Kind.
                       "Evaluation"
                     "labels": {
                         "str": "str"  # Optional. A set of key-value labels for the resource.
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
@@ -3956,15 +3993,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -4045,15 +4084,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -5604,14 +5645,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -5712,25 +5755,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -5778,14 +5825,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -5825,25 +5874,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -5982,15 +6035,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -6071,15 +6126,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -7812,29 +7869,133 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
+    @overload
+    async def token(
+        self,
+        session_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[str, JSON]:
+        # pylint: disable=line-too-long
+        """Get an access token for an existing InferenceSession.
+
+        Get an access token for an existing InferenceSession.
+
+        :param session_id: Required.
+        :type session_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: str or JSON object
+        :rtype: str or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "expires": "2020-02-20 00:00:00",  # Optional. Expiration time of the token.
+                      Must be <= expiration time of session. Default: expiration time of session.
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    async def token(
+        self,
+        session_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[str, JSON]:
+        """Get an access token for an existing InferenceSession.
+
+        Get an access token for an existing InferenceSession.
+
+        :param session_id: Required.
+        :type session_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: str or JSON object
+        :rtype: str or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
     @distributed_trace_async
-    async def token(self, session_id: str, **kwargs: Any) -> Union[str, JSON]:
+    async def token(
+        self, session_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> Union[str, JSON]:
+        # pylint: disable=line-too-long
         """Get an access token for an existing InferenceSession.
 
         Get an access token for an existing InferenceSession.
 
         :param session_id: Required.
         :type session_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
         :return: str or JSON object
         :rtype: str or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "expires": "2020-02-20 00:00:00",  # Optional. Expiration time of the token.
+                      Must be <= expiration time of session. Default: expiration time of session.
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
                                 {}
                             ],
@@ -7848,21 +8009,35 @@
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = kwargs.pop("headers", {}) or {}
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = kwargs.pop("params", {}) or {}
 
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
         cls: ClsType[Union[str, JSON]] = kwargs.pop("cls", None)
 
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
         _request = build_inferencesessions_token_request(
             session_id=session_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = (
@@ -8042,15 +8217,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -8131,15 +8308,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -9756,15 +9935,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -9845,15 +10026,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -11149,14 +11332,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -11257,25 +11442,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -11323,14 +11512,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -11370,25 +11561,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -11527,15 +11722,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -11616,15 +11813,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -12788,14 +12987,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -12896,25 +13097,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -12962,14 +13167,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -13009,25 +13216,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -13166,15 +13377,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -13255,15 +13468,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -14365,14 +14580,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -14473,25 +14690,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -14539,14 +14760,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -14586,25 +14809,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -14743,15 +14970,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -14832,15 +15061,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -16110,15 +16341,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -16199,15 +16432,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
```

### Comparing `dyff_client-0.6.0/dyff/client/_generated/aio/operations/_patch.py` & `dyff_client-0.7.0/dyff/client/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/operations/__init__.py` & `dyff_client-0.7.0/dyff/client/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/_generated/operations/_operations.py` & `dyff_client-0.7.0/dyff/client/_generated/operations/_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -820,28 +820,35 @@
 
 
 def build_inferencesessions_token_request(
     session_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
+    content_type: Optional[str] = kwargs.pop(
+        "content_type", _headers.pop("Content-Type", None)
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/inferencesessions/{session_id}/token"
     path_format_arguments = {
         "session_id": _SERIALIZER.url("session_id", session_id, "str"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header(
+            "content_type", content_type, "str"
+        )
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
 def build_inferencesessions_ready_request(
     session_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
@@ -1990,15 +1997,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -2079,15 +2088,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -3507,14 +3518,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -3615,25 +3628,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -3681,14 +3698,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -3728,25 +3747,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -3885,15 +3908,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -3974,15 +3999,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -4297,14 +4324,17 @@
                                   for detailed naming rules. Required.
                                 "value": "str"  # The annotation value. An arbitrary
                                   string. Required.
                             }
                         ],
                         "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation
                           time (assigned by system).
+                        "inferenceSessionReference": "str",  # Optional. ID of a running
+                          inference session that will be used for the evaluation instead of starting a
+                          new one.
                         "kind": "Evaluation",  # Optional. Default value is "Evaluation".
                           Kind. "Evaluation"
                         "labels": {
                             "str": "str"  # Optional. A set of key-value labels for the
                               resource. Used to specify identifying attributes of resources that are
                               meaningful to users but do not imply semantics in the dyff system.  The
                               keys are DNS labels with an optional DNS domain prefix. For example:
@@ -4447,14 +4477,17 @@
                           the session. Use of this field is recommended to avoid accidental compute
                           costs.
                         "replicas": 1,  # Optional. Default value is 1. Number of model
                           replicas.
                         "useSpotPods": True  # Optional. Default value is True. Use 'spot
                           pods' for cheaper computation.
                     },
+                    "inferenceSessionReference": "str",  # Optional. The ID of a running
+                      inference session that will be used for the evaluation, instead of starting a new
+                      one.
                     "replications": 1,  # Optional. Default value is 1. Number of replications to
                       run.
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                     "workersPerReplica": 0  # Optional. Number of data workers per inference
                       service replica.
                 }
@@ -4632,14 +4665,16 @@
                               for detailed naming rules. Required.
                             "value": "str"  # The annotation value. An arbitrary string.
                               Required.
                         }
                     ],
                     "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
                       (assigned by system).
+                    "inferenceSessionReference": "str",  # Optional. ID of a running inference
+                      session that will be used for the evaluation instead of starting a new one.
                     "kind": "Evaluation",  # Optional. Default value is "Evaluation". Kind.
                       "Evaluation"
                     "labels": {
                         "str": "str"  # Optional. A set of key-value labels for the resource.
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
@@ -4865,14 +4900,16 @@
                               for detailed naming rules. Required.
                             "value": "str"  # The annotation value. An arbitrary string.
                               Required.
                         }
                     ],
                     "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
                       (assigned by system).
+                    "inferenceSessionReference": "str",  # Optional. ID of a running inference
+                      session that will be used for the evaluation instead of starting a new one.
                     "kind": "Evaluation",  # Optional. Default value is "Evaluation". Kind.
                       "Evaluation"
                     "labels": {
                         "str": "str"  # Optional. A set of key-value labels for the resource.
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
@@ -4944,14 +4981,17 @@
                           the session. Use of this field is recommended to avoid accidental compute
                           costs.
                         "replicas": 1,  # Optional. Default value is 1. Number of model
                           replicas.
                         "useSpotPods": True  # Optional. Default value is True. Use 'spot
                           pods' for cheaper computation.
                     },
+                    "inferenceSessionReference": "str",  # Optional. The ID of a running
+                      inference session that will be used for the evaluation, instead of starting a new
+                      one.
                     "replications": 1,  # Optional. Default value is 1. Number of replications to
                       run.
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                     "workersPerReplica": 0  # Optional. Number of data workers per inference
                       service replica.
                 }
@@ -5129,14 +5169,16 @@
                               for detailed naming rules. Required.
                             "value": "str"  # The annotation value. An arbitrary string.
                               Required.
                         }
                     ],
                     "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
                       (assigned by system).
+                    "inferenceSessionReference": "str",  # Optional. ID of a running inference
+                      session that will be used for the evaluation instead of starting a new one.
                     "kind": "Evaluation",  # Optional. Default value is "Evaluation". Kind.
                       "Evaluation"
                     "labels": {
                         "str": "str"  # Optional. A set of key-value labels for the resource.
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
@@ -5425,14 +5467,16 @@
                               for detailed naming rules. Required.
                             "value": "str"  # The annotation value. An arbitrary string.
                               Required.
                         }
                     ],
                     "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
                       (assigned by system).
+                    "inferenceSessionReference": "str",  # Optional. ID of a running inference
+                      session that will be used for the evaluation instead of starting a new one.
                     "kind": "Evaluation",  # Optional. Default value is "Evaluation". Kind.
                       "Evaluation"
                     "labels": {
                         "str": "str"  # Optional. A set of key-value labels for the resource.
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
@@ -5765,15 +5809,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -5854,15 +5900,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -7413,14 +7461,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -7521,25 +7571,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -7587,14 +7641,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -7634,25 +7690,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -7791,15 +7851,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -7880,15 +7942,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -9621,29 +9685,133 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
+    @overload
+    def token(
+        self,
+        session_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[str, JSON]:
+        # pylint: disable=line-too-long
+        """Get an access token for an existing InferenceSession.
+
+        Get an access token for an existing InferenceSession.
+
+        :param session_id: Required.
+        :type session_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: str or JSON object
+        :rtype: str or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "expires": "2020-02-20 00:00:00",  # Optional. Expiration time of the token.
+                      Must be <= expiration time of session. Default: expiration time of session.
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    def token(
+        self,
+        session_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[str, JSON]:
+        """Get an access token for an existing InferenceSession.
+
+        Get an access token for an existing InferenceSession.
+
+        :param session_id: Required.
+        :type session_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: str or JSON object
+        :rtype: str or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
     @distributed_trace
-    def token(self, session_id: str, **kwargs: Any) -> Union[str, JSON]:
+    def token(
+        self, session_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> Union[str, JSON]:
+        # pylint: disable=line-too-long
         """Get an access token for an existing InferenceSession.
 
         Get an access token for an existing InferenceSession.
 
         :param session_id: Required.
         :type session_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
         :return: str or JSON object
         :rtype: str or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "expires": "2020-02-20 00:00:00",  # Optional. Expiration time of the token.
+                      Must be <= expiration time of session. Default: expiration time of session.
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
                                 {}
                             ],
@@ -9657,21 +9825,35 @@
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = kwargs.pop("headers", {}) or {}
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = kwargs.pop("params", {}) or {}
 
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
         cls: ClsType[Union[str, JSON]] = kwargs.pop("cls", None)
 
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
         _request = build_inferencesessions_token_request(
             session_id=session_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = (
@@ -9851,15 +10033,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -9940,15 +10124,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -11563,15 +11749,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -11652,15 +11840,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -12956,14 +13146,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -13064,25 +13256,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -13130,14 +13326,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -13177,25 +13375,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -13334,15 +13536,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -13423,15 +13627,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -14595,14 +14801,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -14703,25 +14911,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -14769,14 +14981,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -14816,25 +15030,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -14973,15 +15191,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -15062,15 +15282,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -16172,14 +16394,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -16280,25 +16504,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -16346,14 +16574,16 @@
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -16393,25 +16623,29 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
                       Markdown. There are no length constraints, but be reasonable.
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                     "summary": "str",  # Optional. A brief summary, suitable for display in small
                       UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
                       in the UI, especially on small displays.
                     "title": "str"  # Optional. A short plain string suitable as a title or
                       "headline".
                 }
                 # response body for status code(s): 422
@@ -16550,15 +16784,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -16639,15 +16875,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -17917,15 +18155,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -18006,15 +18246,17 @@
                           Used to specify identifying attributes of resources that are meaningful to
                           users but do not imply semantics in the dyff system.  The keys are DNS labels
                           with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
+                    },
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
                 }
 
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
```

### Comparing `dyff_client-0.6.0/dyff/client/_generated/operations/_patch.py` & `dyff_client-0.7.0/dyff/client/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/dyff/client/client.py` & `dyff_client-0.7.0/dyff/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # mypy: disable-error-code="import-untyped"
 from __future__ import annotations
 
 import json
 import sys
 import time
+from datetime import datetime
 from pathlib import Path
 from typing import Any, Callable, Optional, TypeVar
 from warnings import warn
 
 import httpx
 from azure.core.credentials import AccessToken, TokenCredential
 
@@ -50,14 +51,15 @@
 from dyff.schema.requests import (
     AnalysisCreateRequest,
     DatasetCreateRequest,
     DocumentationEditRequest,
     EvaluationCreateRequest,
     InferenceServiceCreateRequest,
     InferenceSessionCreateRequest,
+    InferenceSessionTokenCreateRequest,
     LabelUpdateRequest,
     MethodCreateRequest,
     ModelCreateRequest,
     ModuleCreateRequest,
     ReportCreateRequest,
 )
 
@@ -1086,25 +1088,29 @@
         :type session_id: str
         :return: The resulting status of the entity
         :rtype: dyff.schema.platform.Status
         :raises HttpResponseError:
         """
         return Status.parse_obj(self._raw_ops.terminate(session_id))
 
-    def token(self, session_id: str) -> str:
+    def token(self, session_id: str, *, expires: Optional[datetime] = None) -> str:
         """Create a session token.
 
         The session token is a short-lived token that allows the bearer to
         make inferences with the session (via an ``InferenceSessionClient``)
         and to call ``ready()``, ``get()``, and ``terminate()`` on the session.
 
         :param str session_id: The ID of the session.
+        :keyword Optional[datetime] expires: The expiration time of the token.
+            Must be < the expiration time of the session. Default: expiration
+            time of the session.
         :raises HttpResponseError:
         """
-        return str(self._raw_ops.token(session_id))
+        request = InferenceSessionTokenCreateRequest(expires=expires)
+        return str(self._raw_ops.token(session_id, request.dict()))
 
 
 class MeasurementsOperations:
     """Operations on :class:`~dyff.schema.platform.Measurement` entities.
 
     .. note::
```

### Comparing `dyff_client-0.6.0/dyff_client.egg-info/PKG-INFO` & `dyff_client-0.7.0/dyff_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_client-0.6.0/dyff_client.egg-info/SOURCES.txt` & `dyff_client-0.7.0/dyff_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/makefile` & `dyff_client-0.7.0/makefile`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/pyproject.toml` & `dyff_client-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py` & `dyff_client-0.7.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py` & `dyff_client-0.7.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/scripts/models/databricks--dolly-v2-3b.py` & `dyff_client-0.7.0/scripts/models/databricks--dolly-v2-3b.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/scripts/models/tiiuae--falcon-7b.py` & `dyff_client-0.7.0/scripts/models/tiiuae--falcon-7b.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.6.0/tests/test_import.py` & `dyff_client-0.7.0/tests/test_import.py`

 * *Files identical despite different names*

