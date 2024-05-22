# Comparing `tmp/dyff_schema-0.6.0.tar.gz` & `tmp/dyff_schema-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_schema-0.6.0.tar", last modified: Thu May 16 21:19:53 2024, max compression
+gzip compressed data, was "dyff_schema-0.7.0.tar", last modified: Tue May 21 20:09:55 2024, max compression
```

## Comparing `dyff_schema-0.6.0.tar` & `dyff_schema-0.7.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.901949 dyff_schema-0.6.0/
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3458 2024-05-16 21:19:53.901949 dyff_schema-0.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.886949 dyff_schema-0.6.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.893949 dyff_schema-0.6.0/dyff/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/copydoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.894949 dyff_schema-0.6.0/dyff/schema/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/dataset/vision.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.895949 dyff_schema-0.6.0/dyff/schema/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/platform.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/quantity.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.895949 dyff_schema-0.6.0/dyff/schema/v0/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.897949 dyff_schema-0.6.0/dyff/schema/v0/r1/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23552 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    17139 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.898949 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12312 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.898949 dyff_schema-0.6.0/dyff/schema/v0/r1/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)    60712 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     8490 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/test.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/v0/r1/version.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/dyff/schema/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.900949 dyff_schema-0.6.0/dyff_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3458 2024-05-16 21:19:53.000000 dyff_schema-0.6.0/dyff_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2024-05-16 21:19:53.000000 dyff_schema-0.6.0/dyff_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 21:19:53.000000 dyff_schema-0.6.0/dyff_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-16 21:19:53.000000 dyff_schema-0.6.0/dyff_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-16 21:19:53.000000 dyff_schema-0.6.0/dyff_schema.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 21:19:53.901949 dyff_schema-0.6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:19:53.900949 dyff_schema-0.6.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1449 2024-05-16 21:19:47.000000 dyff_schema-0.6.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.300689 dyff_schema-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-05-21 20:09:55.300689 dyff_schema-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.286689 dyff_schema-0.7.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.292688 dyff_schema-0.7.0/dyff/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/copydoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.293689 dyff_schema-0.7.0/dyff/schema/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/dataset/vision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/ids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.294689 dyff_schema-0.7.0/dyff/schema/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.294689 dyff_schema-0.7.0/dyff/schema/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.296689 dyff_schema-0.7.0/dyff/schema/v0/r1/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23552 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    17139 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.297689 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12312 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.298689 dyff_schema-0.7.0/dyff/schema/v0/r1/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)    60712 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     8860 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/v0/r1/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/dyff/schema/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.299689 dyff_schema-0.7.0/dyff_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-05-21 20:09:55.000000 dyff_schema-0.7.0/dyff_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-05-21 20:09:55.000000 dyff_schema-0.7.0/dyff_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 20:09:55.000000 dyff_schema-0.7.0/dyff_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-21 20:09:55.000000 dyff_schema-0.7.0/dyff_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-21 20:09:55.000000 dyff_schema-0.7.0/dyff_schema.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 20:09:55.300689 dyff_schema-0.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:09:55.299689 dyff_schema-0.7.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2024-05-21 20:09:49.000000 dyff_schema-0.7.0/tests/test_import.py
```

### Comparing `dyff_schema-0.6.0/.gitlab-ci.yml` & `dyff_schema-0.7.0/.gitlab-ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
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
       - python-build-sdist.yml
       - python-build-wheel.yml
       - python-isort.yml
       - python-mypy.yml
```

### Comparing `dyff_schema-0.6.0/.pre-commit-config.yaml` & `dyff_schema-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/.secrets.baseline` & `dyff_schema-0.7.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/CODE_OF_CONDUCT.md` & `dyff_schema-0.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/LICENSE` & `dyff_schema-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/PKG-INFO` & `dyff_schema-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.6.0
+Version: 0.7.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.6.0/README.md` & `dyff_schema-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff/schema/__init__.py` & `dyff_schema-0.7.0/dyff/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff/schema/copydoc.py` & `dyff_schema-0.7.0/dyff/schema/copydoc.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff/schema/ids.py` & `dyff_schema-0.7.0/dyff/schema/ids.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff/schema/quantity.py` & `dyff_schema-0.7.0/dyff/schema/quantity.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff/schema/v0/r1/adapters.py` & `dyff_schema-0.7.0/dyff/schema/v0/r1/adapters.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff/schema/v0/r1/base.py` & `dyff_schema-0.7.0/dyff/schema/v0/r1/base.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/__init__.py` & `dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/arrow.py` & `dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/arrow.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/binary.py` & `dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/binary.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff/schema/v0/r1/dataset/text.py` & `dyff_schema-0.7.0/dyff/schema/v0/r1/dataset/text.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff/schema/v0/r1/io/vllm.py` & `dyff_schema-0.7.0/dyff/schema/v0/r1/io/vllm.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff/schema/v0/r1/platform.py` & `dyff_schema-0.7.0/dyff/schema/v0/r1/platform.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff/schema/v0/r1/requests.py` & `dyff_schema-0.7.0/dyff/schema/v0/r1/requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 resource, the request will refer to the dependency by its ID, while the core
 resource will include the full dependency object as a sub-resource. The
 ``create`` endpoints take a request as input and return a full core resource
 in response.
 """
 
 
+from datetime import datetime
 from typing import Any, Optional, Union
 
 import pydantic
 
 from .base import DyffSchemaBaseModel
 from .platform import (
     AnalysisBase,
@@ -61,14 +62,22 @@
     )
 
 
 class InferenceSessionCreateRequest(DyffEntityCreateRequest, InferenceSessionBase):
     inferenceService: str = pydantic.Field(description="InferenceService ID")
 
 
+class InferenceSessionTokenCreateRequest(SchemaVersion, DyffSchemaBaseModel):
+    expires: Optional[datetime] = pydantic.Field(
+        default=None,
+        description="Expiration time of the token. Must be <= expiration time"
+        " of session. Default: expiration time of session.",
+    )
+
+
 class EvaluationInferenceSessionRequest(InferenceSessionBase):
     inferenceService: str = pydantic.Field(description="InferenceService ID")
 
 
 class EvaluationCreateRequest(DyffEntityCreateRequest, EvaluationBase):
     """A description of how to run an InferenceService on a Dataset to obtain a set of
     evaluation results."""
@@ -237,14 +246,15 @@
     "EvaluationCreateRequest",
     "EvaluationQueryRequest",
     "EvaluationInferenceSessionRequest",
     "InferenceServiceCreateRequest",
     "InferenceServiceQueryRequest",
     "InferenceSessionCreateRequest",
     "InferenceSessionQueryRequest",
+    "InferenceSessionTokenCreateRequest",
     "LabelUpdateRequest",
     "MeasurementQueryRequest",
     "MethodCreateRequest",
     "MethodQueryRequest",
     "ModelCreateRequest",
     "ModelQueryRequest",
     "ModuleCreateRequest",
```

### Comparing `dyff_schema-0.6.0/dyff/schema/v0/r1/test.py` & `dyff_schema-0.7.0/dyff/schema/v0/r1/test.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/dyff_schema.egg-info/PKG-INFO` & `dyff_schema-0.7.0/dyff_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.6.0
+Version: 0.7.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.6.0/dyff_schema.egg-info/SOURCES.txt` & `dyff_schema-0.7.0/dyff_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/pyproject.toml` & `dyff_schema-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.6.0/tests/test_import.py` & `dyff_schema-0.7.0/tests/test_import.py`

 * *Files identical despite different names*

