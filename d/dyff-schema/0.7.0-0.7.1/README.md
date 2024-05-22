# Comparing `tmp/dyff_schema-0.7.0.tar.gz` & `tmp/dyff_schema-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_schema-0.7.0.tar", last modified: Tue May 21 20:09:55 2024, max compression
+gzip compressed data, was "dyff_schema-0.7.1.tar", last modified: Wed May 22 00:59:44 2024, max compression
```

## Comparing `dyff_schema-0.7.0.tar` & `dyff_schema-0.7.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.300689 dyff_schema-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3458 2024-05-21 20:09:55.300689 dyff_schema-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.286689 dyff_schema-0.7.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.292688 dyff_schema-0.7.0/dyff/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/copydoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.293689 dyff_schema-0.7.0/dyff/schema/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/dataset/vision.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.294689 dyff_schema-0.7.0/dyff/schema/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/platform.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/quantity.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.294689 dyff_schema-0.7.0/dyff/schema/v0/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.296689 dyff_schema-0.7.0/dyff/schema/v0/r1/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23552 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    17139 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.297689 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12312 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.298689 dyff_schema-0.7.0/dyff/schema/v0/r1/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)    60712 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     8860 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/test.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/version.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.299689 dyff_schema-0.7.0/dyff_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3458 2024-05-21 20:09:55.000000 dyff_schema-0.7.0/dyff_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2024-05-21 20:09:55.000000 dyff_schema-0.7.0/dyff_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 20:09:55.000000 dyff_schema-0.7.0/dyff_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-21 20:09:55.000000 dyff_schema-0.7.0/dyff_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-21 20:09:55.000000 dyff_schema-0.7.0/dyff_schema.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 20:09:55.300689 dyff_schema-0.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.299689 dyff_schema-0.7.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1449 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 00:59:44.072331 dyff_schema-0.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-05-22 00:59:44.072331 dyff_schema-0.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 00:59:44.057331 dyff_schema-0.7.1/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 00:59:44.064331 dyff_schema-0.7.1/dyff/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/copydoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 00:59:44.065331 dyff_schema-0.7.1/dyff/schema/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/dataset/vision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/ids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 00:59:44.066331 dyff_schema-0.7.1/dyff/schema/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 00:59:44.066331 dyff_schema-0.7.1/dyff/schema/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 00:59:44.068331 dyff_schema-0.7.1/dyff/schema/v0/r1/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23552 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    17471 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 00:59:44.069332 dyff_schema-0.7.1/dyff/schema/v0/r1/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12312 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/dataset/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 00:59:44.070331 dyff_schema-0.7.1/dyff/schema/v0/r1/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)    60823 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     8913 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/v0/r1/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/dyff/schema/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 00:59:44.071331 dyff_schema-0.7.1/dyff_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-05-22 00:59:44.000000 dyff_schema-0.7.1/dyff_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-05-22 00:59:44.000000 dyff_schema-0.7.1/dyff_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 00:59:44.000000 dyff_schema-0.7.1/dyff_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-22 00:59:44.000000 dyff_schema-0.7.1/dyff_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-22 00:59:44.000000 dyff_schema-0.7.1/dyff_schema.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 00:59:44.072331 dyff_schema-0.7.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 00:59:44.071331 dyff_schema-0.7.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2024-05-22 00:59:37.000000 dyff_schema-0.7.1/tests/test_import.py
```

### Comparing `dyff_schema-0.7.0/.gitlab-ci.yml` & `dyff_schema-0.7.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/.pre-commit-config.yaml` & `dyff_schema-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/.secrets.baseline` & `dyff_schema-0.7.1/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/CODE_OF_CONDUCT.md` & `dyff_schema-0.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/LICENSE` & `dyff_schema-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/PKG-INFO` & `dyff_schema-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.7.0
+Version: 0.7.1
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.7.0/README.md` & `dyff_schema-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/dyff/schema/__init__.py` & `dyff_schema-0.7.1/dyff/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/dyff/schema/copydoc.py` & `dyff_schema-0.7.1/dyff/schema/copydoc.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/dyff/schema/ids.py` & `dyff_schema-0.7.1/dyff/schema/ids.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/dyff/schema/quantity.py` & `dyff_schema-0.7.1/dyff/schema/quantity.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/dyff/schema/v0/r1/adapters.py` & `dyff_schema-0.7.1/dyff/schema/v0/r1/adapters.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/dyff/schema/v0/r1/base.py` & `dyff_schema-0.7.1/dyff/schema/v0/r1/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
+from datetime import datetime
 from typing import Any, Generic, NamedTuple, Optional, Type, TypeVar
 
 import pydantic
 
 # ----------------------------------------------------------------------------
 # Fixed-width numeric type value bounds
 
@@ -559,14 +560,22 @@
 
     Overrides serialization functions to serialize by alias, so that "round-trip"
     serialization is the default for fields with aliases. We prefer aliases because we
     can 1) use _underscore_names_ as reserved names in our data schema, and 2) allow
     Python reserved words like 'bytes' as field names.
     """
 
+    @pydantic.root_validator
+    def _require_datetime_timezone_aware(cls, values):
+        for k, v in values.items():
+            if isinstance(v, datetime):
+                if v.tzinfo is None:
+                    raise ValueError(f"{cls.__qualname__}.{k}: timezone not set")
+        return values
+
     def dict(self, *, by_alias: bool = True, **kwargs) -> dict[str, Any]:
         return super().dict(by_alias=by_alias, **kwargs)
 
     def json(self, *, by_alias: bool = True, **kwargs) -> str:
         return super().json(by_alias=by_alias, **kwargs)
```

### Comparing `dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/__init__.py` & `dyff_schema-0.7.1/dyff/schema/v0/r1/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/arrow.py` & `dyff_schema-0.7.1/dyff/schema/v0/r1/dataset/arrow.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/binary.py` & `dyff_schema-0.7.1/dyff/schema/v0/r1/dataset/binary.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/text.py` & `dyff_schema-0.7.1/dyff/schema/v0/r1/dataset/text.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/dyff/schema/v0/r1/io/vllm.py` & `dyff_schema-0.7.1/dyff/schema/v0/r1/io/vllm.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/dyff/schema/v0/r1/platform.py` & `dyff_schema-0.7.1/dyff/schema/v0/r1/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,15 @@
     )
 
     reason: Optional[str] = pydantic.Field(
         default=None, description="Reason for current status (assigned by system)"
     )
 
 
-class Documentation(DyffSchemaBaseModel):
+class DocumentationBase(DyffSchemaBaseModel):
     title: Optional[str] = pydantic.Field(
         default=None,
         description='A short plain string suitable as a title or "headline".',
     )
 
     summary: Optional[str] = pydantic.Field(
         default=None,
@@ -314,17 +314,21 @@
     fullPage: Optional[str] = pydantic.Field(
         default=None,
         description="Long-form documentation. Interpreted as"
         " Markdown. There are no length constraints, but be reasonable.",
     )
 
 
+class Documentation(SchemaVersion, DocumentationBase):
+    pass
+
+
 class Documented(DyffSchemaBaseModel):
-    documentation: Documentation = pydantic.Field(
-        default_factory=Documentation,
+    documentation: DocumentationBase = pydantic.Field(
+        default_factory=DocumentationBase,
         description="Documentation of the resource. The content is used to"
         " populate various views in the web UI.",
     )
 
 
 class FamilyMemberKind(str, enum.Enum):
     """The kinds of entities that can be members of a Family.
@@ -376,16 +380,16 @@
     )
 
     tags: list[Tag] = pydantic.Field(
         default_factory=list,
         description="Tags mapping interpretable names to resource IDs.",
     )
 
-    documentation: Documentation = pydantic.Field(
-        default_factory=Documentation,
+    documentation: DocumentationBase = pydantic.Field(
+        default_factory=DocumentationBase,
         description="Documentation of the resource family. The content is used"
         " to populate various views in the web UI.",
     )
 
 
 class DyffEntity(Status, Labeled, SchemaVersion, DyffModelWithID):
     kind: Literal[
@@ -1857,14 +1861,15 @@
     "DatasetBase",
     "DatasetFilter",
     "DataSource",
     "DataSources",
     "DataView",
     "Digest",
     "Documentation",
+    "DocumentationBase",
     "DyffDataSchema",
     "DyffEntity",
     "DyffModelWithID",
     "DyffSchemaBaseModel",
     "Entities",
     "Evaluation",
     "EvaluationBase",
```

### Comparing `dyff_schema-0.7.0/dyff/schema/v0/r1/requests.py` & `dyff_schema-0.7.1/dyff/schema/v0/r1/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import pydantic
 
 from .base import DyffSchemaBaseModel
 from .platform import (
     AnalysisBase,
     DatasetBase,
     DataView,
-    Documentation,
+    DocumentationBase,
     EvaluationBase,
     InferenceServiceBase,
     InferenceSessionBase,
     Labeled,
     MethodBase,
     ModelSpec,
     ModuleBase,
@@ -48,15 +48,15 @@
     method: str = pydantic.Field(description="Method ID")
 
 
 class DatasetCreateRequest(DyffEntityCreateRequest, DatasetBase):
     pass
 
 
-class DocumentationEditRequest(Documentation):
+class DocumentationEditRequest(SchemaVersion, DocumentationBase):
     pass
 
 
 class InferenceServiceCreateRequest(DyffEntityCreateRequest, InferenceServiceBase):
     model: Optional[str] = pydantic.Field(
         default=None, description="ID of Model backing the service, if applicable"
     )
@@ -133,19 +133,19 @@
 
     evaluationView: Optional[Union[str, DataView]] = pydantic.Field(
         default=None,
         description="View of the evaluation output data required by the report.",
     )
 
 
-class TagCreateRequest(TagBase):
+class TagCreateRequest(SchemaVersion, TagBase):
     pass
 
 
-class LabelUpdateRequest(Labeled):
+class LabelUpdateRequest(SchemaVersion, Labeled):
     pass
 
 
 # Note: Query requests, as they currently exist, don't work with Versioned
 # because fastapi will assign None to every field that the client doesn't
 # specify. I think it's not that important, because all of the query parameters
 # will always be optional. There could be a problem if the semantics of a
```

### Comparing `dyff_schema-0.7.0/dyff/schema/v0/r1/test.py` & `dyff_schema-0.7.1/dyff/schema/v0/r1/test.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/dyff_schema.egg-info/PKG-INFO` & `dyff_schema-0.7.1/dyff_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.7.0
+Version: 0.7.1
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.7.0/dyff_schema.egg-info/SOURCES.txt` & `dyff_schema-0.7.1/dyff_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/pyproject.toml` & `dyff_schema-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.7.0/tests/test_import.py` & `dyff_schema-0.7.1/tests/test_import.py`

 * *Files identical despite different names*

